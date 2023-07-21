# Comparing `tmp/wiretap-4.2.2-py3-none-any.whl.zip` & `tmp/wiretap-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4818 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      131 b- defN 23-May-13 15:30 wiretap/__init__.py
+Zip file size: 5380 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      140 b- defN 23-Jul-20 17:54 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat    12354 b- defN 23-May-15 09:06 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-May-15 09:06 wiretap-4.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 09:06 wiretap-4.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-15 09:06 wiretap-4.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      520 b- defN 23-May-15 09:06 wiretap-4.2.2.dist-info/RECORD
-7 files, 13969 bytes uncompressed, 3900 bytes compressed:  72.1%
+-rw-rw-rw-  2.0 fat    14455 b- defN 23-Jul-20 20:20 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/RECORD
+7 files, 16079 bytes uncompressed, 4462 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-4.2.2.dist-info/METADATA
+Filename: wiretap-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-4.2.2.dist-info/WHEEL
+Filename: wiretap-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-4.2.2.dist-info/top_level.txt
+Filename: wiretap-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-4.2.2.dist-info/RECORD
+Filename: wiretap-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .wiretap import (
     Logger,
     SerializeDetails,
     MultiFormatter,
     telemetry,
     telemetry_scope,
-    raw
+    Cancellation
 )
```

## wiretap/wiretap.py

```diff
@@ -8,23 +8,23 @@
 import logging
 import sys
 import uuid
 from collections.abc import Generator
 from contextvars import ContextVar
 from datetime import datetime, date
 from timeit import default_timer as timer
-from typing import Dict, Callable, Any, Protocol, Optional, Iterator, TypeVar, TypeAlias
+from types import TracebackType
+from typing import Dict, Callable, Any, Protocol, Optional, Iterator, TypeVar, TypeAlias, Generic
 
-FormatOptions: TypeAlias = str | Callable[[Any], Any]
+FormatOptions: TypeAlias = str | Callable[[Any], Any] | None
 TValue = TypeVar("TValue")
-NO_DETAILS: dict[str, Any] = {}
 
 DEFAULT_FORMATS: Dict[str, str] = {
-    "classic": "{asctime}.{msecs:.0f} | {levelname} | {module}.{funcName} | {message}",
-    "wiretap": "{asctime}.{msecs:.0f} {indent} {levelname} | {module}.{funcName} | {status} | {elapsed:.3f}s | {message} | {details} | node://{parent}/{node} | {attachment}",
+    "classic": "{asctime}.{msecs:03.0f} | {levelname} | {module}.{funcName} | {message}",
+    "wiretap": "{asctime}.{msecs:03.0f} {indent} {module}.{funcName} | {status} | {elapsed:.3f}s | {message} | {details} | node://{parent}/{node} | {attachment}",
 }
 
 _scope: ContextVar[Optional["Logger"]] = ContextVar("_scope", default=None)
 
 
 class SerializeDetails(Protocol):
     def __call__(self, value: Optional[Dict[str, Any]]) -> str | None: ...
@@ -51,63 +51,73 @@
         record.levelname = record.levelname.lower()
         record.__dict__.update(self.values or {})  # Unpack values.
 
         if hasattr(record, "details") and isinstance(record.details, dict):
             record.indent = self.indent * record.__dict__.pop("_depth", 1)
             record.details = self.serialize_details(record.details)
 
-        if hasattr(record, "status"):
-            self._style._fmt = self.formats["wiretap"] if "wiretap" in self.formats else DEFAULT_FORMATS["wiretap"]
-        else:
-            self._style._fmt = self.formats["classic"] if "classin" in self.formats else DEFAULT_FORMATS["classic"]
-
-        return super().format(record)
+        # determine which format to use
+        format_key = "wiretap" if hasattr(record, "status") else "classic"
 
+        # use custom format if specified or the default one
+        format_str = self.formats[format_key] if format_key in self.formats else DEFAULT_FORMATS[format_key]
+        self._style._fmt = format_str
 
-def raw(value: TValue) -> TValue:
-    return value
+        return super().format(record)
 
 
 def multi_format(value: Any, value_format: FormatOptions) -> Optional[Any]:
     if value is None:
+        # cancel as there is no value to format
         return None
 
+    if value_format is None:
+        # cancel as no format is specified
+        return value
+
     if isinstance(value_format, str):
+        # format using a format-string
         return format(value, value_format)
 
     if callable(value_format):
+        # format using a user defined function
         return value_format(value)
 
-    raise ValueError(f"Unsupported details format: {type(value_format)}. Expected: {FormatOptions}.")
+    # any other case means an error
+    raise ValueError(f"Unsupported value format: {type(value_format)}. Expected: {FormatOptions}.")
 
 
 def create_args_details(args: dict[str, Any], args_format: FormatOptions | dict[str, FormatOptions]) -> dict[str, Any]:
-    if args_format == NO_DETAILS:
+    if args_format is None:
+        # cancel as no format is specified
         return {}
 
     if not args:
-        return {"args": None}
+        # cancel as there's nothing to format
+        return {}
 
     if isinstance(args_format, dict):
+        # format each arg individually
         return {"args": {key: multi_format(args.get(key, None), args_format[key]) for key in args_format}}
-
-    return {"args": {key: multi_format(args.get(key, None), args_format) for key in args}}
+    else:
+        # format all args with common format
+        return {"args": {key: multi_format(args.get(key, None), args_format) for key in args}}
 
 
 def create_result_details(result: Any | None, result_format: FormatOptions | dict[str, FormatOptions]) -> dict[str, Any]:
-    if result_format == NO_DETAILS:
+    if result_format is None:
         return {}
 
     if result is None:
-        return {"result": None}
+        return {}
 
     if isinstance(result_format, dict):
         return {"result": {key: multi_format(result, result_format[key]) for key in result_format}}
-
-    return {"result": multi_format(result, result_format)}
+    else:
+        return {"result": multi_format(result, result_format)}
 
 
 class Logger:
 
     def __init__(self, module: Optional[str], scope: str, parent: Optional["Logger"] = None):
         self.id = uuid.uuid4()
         self.module = module
@@ -143,83 +153,106 @@
 
     def completed(
             self,
             message: Optional[str] = None,
             details: Optional[dict[str, Any]] = None,
             attachment: Optional[Any] = None,
             result: Optional[TValue] = None,
-            result_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+            result_format: FormatOptions | dict[str, FormatOptions] = None
     ) -> Optional[TValue]:
         self._logger.setLevel(logging.INFO)
         self._log(message, details, attachment, result, result_format)
         return result
 
     def canceled(
             self,
             message: Optional[str] = None,
             details: Optional[dict[str, Any]] = None,
             attachment: Optional[Any] = None,
             result: Optional[TValue] = None,
-            result_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+            result_format: FormatOptions | dict[str, FormatOptions] = None
     ) -> Optional[TValue]:
-        self._logger.setLevel(logging.WARNING)
+        self._logger.setLevel(logging.ERROR if sys.exc_info()[0] is Failure else logging.WARNING)
         self._log(message, details, attachment, result, result_format)
         return result
 
-    def faulted(
+    def failed(
             self,
             message: Optional[str] = None,
             details: Optional[dict[str, Any]] = None,
             attachment: Optional[Any] = None,
             result: Optional[TValue] = None,
-            result_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+            result_format: FormatOptions | dict[str, FormatOptions] = None
     ) -> Optional[TValue]:
         self._logger.setLevel(logging.ERROR)
-        self._log(message, details, attachment, result, result_format)
+
+        # process the exception only if it's not Failure
+        exc_cls, exc, exc_tb = sys.exc_info()
+        if exc and exc_cls is not Failure:
+            # the first 3 frames are the decorator traces; let's get rid of them
+            for _ in range(3):
+                # in case there aren't that many frames
+                if exc_tb.tb_next:
+                    exc_tb = exc_tb.tb_next
+                else:
+                    break
+            self._log(message, details, attachment, result, result_format, (exc_cls, exc, exc_tb))
+        else:
+            self._log(message, details, attachment, result, result_format)
+
         return result
 
     def _log(
             self,
             message: Optional[str],
             details: Optional[dict[str, Any]],
             attachment: Optional[Any],
             result: Optional[TValue] = None,
-            result_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+            result_format: FormatOptions | dict[str, FormatOptions] = None,
+            exc_info: Optional[tuple[type[BaseException], BaseException, TracebackType | None]] = None
     ):
         if self._finalized:
             return
 
         details = (details or {}) | create_result_details(result, result_format)
 
         status = inspect.stack()[1][3]
-        with _use_custom_log_record_factory(
-                _set_exc_text,
-                functools.partial(_set_module_name, name=self.module),
-                functools.partial(_set_func_name, name=self.scope),
-                functools.partial(_set_attachment, value=attachment),
-        ):
-            exc_info = all(sys.exc_info()) and status in [self.faulted.__name__]  # Dump the exception only when faulted.
+        record_actions = [
+            functools.partial(_set_module_name, name=self.module),
+            functools.partial(_set_func_name, name=self.scope),
+        ]
+        with _use_custom_log_record_factory(*record_actions):
             self._logger.log(level=self._logger.level, msg=message, exc_info=exc_info, extra={
                 "parent": self.parent.id if self.parent else None,
                 "node": self.id,
                 "status": status,
                 "elapsed": self.elapsed,
-                "details": details or NO_DETAILS,
+                "details": details or {},
+                "attachment": attachment,
                 "_depth": self.depth
             })
 
-        self._finalized = status in [self.completed.__name__, self.canceled.__name__, self.faulted.__name__]
+        self._finalized = status in [
+            self.completed.__name__,
+            self.canceled.__name__,
+            self.failed.__name__
+        ]
 
     def __iter__(self):
         current = self
         while current:
             yield current
             current = current.parent
 
 
+# Helps to prevent logging the same exception multiple times.
+class Failure(Exception):
+    pass
+
+
 @contextlib.contextmanager
 def telemetry_scope(
         module: Optional[str],
         name: str,
         message: Optional[str] = None,
         details: Optional[dict[str, Any]] = None,
         attachment: Optional[Any] = None
@@ -227,32 +260,48 @@
     """Begins a new telemetry scope."""
     logger = Logger(module, name, _scope.get())
     token = _scope.set(logger)
     try:
         logger.started(message, details, attachment)
         yield logger
         logger.completed()
-    except:  # noqa
-        logger.faulted()
+    except Failure:
+        logger.canceled(message="Unhandled exception has occurred.")
         raise
+    except Exception as e:  # noqa
+        logger.failed(message="Unhandled exception has occurred.")
+        raise Failure from e  # wrap the original exception in Failure to keep failing and prevent logging it multiple times
     finally:
         _scope.reset(token)
 
 
+class Cancellation(Exception):
+    def __init__(self, message: str, result: Any | None = None, result_format: FormatOptions | dict[str, FormatOptions] = None):
+        super().__init__(message)
+        self.result = result
+        self.result_format = result_format
+
+
 def telemetry(
         include_args: bool | FormatOptions | dict[str, FormatOptions] = False,
-        include_result: bool | FormatOptions | dict[str, FormatOptions] = False
+        include_result: bool | FormatOptions | dict[str, FormatOptions] = False,
+        message: Optional[str] = None,
+        details: Optional[dict[str, Any]] = None,
+        attachment: Optional[Any] = None
 ):
     """Provides telemetry for the decorated function."""
 
-    args_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+    def raw(value: TValue) -> TValue:
+        return value
+
+    args_format: FormatOptions | dict[str, FormatOptions] = None
     if include_args:
         args_format = raw if isinstance(include_args, bool) else include_args
 
-    result_format: FormatOptions | dict[str, FormatOptions] = NO_DETAILS
+    result_format: FormatOptions | dict[str, FormatOptions] = None
     if include_result:
         result_format = raw if isinstance(include_result, bool) else include_result
 
     def factory(decoratee):
         module = inspect.getmodule(decoratee)
         module_name = module.__name__ if module else None
         scope_name = decoratee.__name__
@@ -270,31 +319,37 @@
             return {t[0]: decoratee_args[t[1]] for t in arg_pairs} | decoratee_kwargs
             # No need to filter args as the logger is injected later.
             # return {k: v for k, v in result.items() if not isinstance(v, Logger)}
 
         if asyncio.iscoroutinefunction(decoratee):
             @functools.wraps(decoratee)
             async def decorator(*decoratee_args, **decoratee_kwargs):
-                details = create_args_details(params(*decoratee_args, **decoratee_kwargs), args_format)
-                with telemetry_scope(module_name, scope_name, details=details) as scope:
+                args_details = create_args_details(params(*decoratee_args, **decoratee_kwargs), args_format) | (details or {})
+                with telemetry_scope(module_name, scope_name, message=message, details=args_details, attachment=attachment) as scope:
                     inject_logger(scope, decoratee_kwargs)
-                    result = await decoratee(*decoratee_args, **decoratee_kwargs)
-                    return scope.completed(result=result, result_format=result_format)
+                    try:
+                        result = await decoratee(*decoratee_args, **decoratee_kwargs)
+                        return scope.completed(result=result, result_format=result_format)
+                    except Cancellation as e:
+                        return scope.canceled(result=e.result, result_format=e.result_format, message=str(e))
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
         else:
             @functools.wraps(decoratee)
             def decorator(*decoratee_args, **decoratee_kwargs):
-                details = create_args_details(params(*decoratee_args, **decoratee_kwargs), args_format)
-                with telemetry_scope(module_name, scope_name, details=details) as scope:
+                args_details = create_args_details(params(*decoratee_args, **decoratee_kwargs), args_format) | (details or {})
+                with telemetry_scope(module_name, scope_name, message=message, details=args_details, attachment=attachment) as scope:
                     inject_logger(scope, decoratee_kwargs)
-                    result = decoratee(*decoratee_args, **decoratee_kwargs)
-                    return scope.completed(result=result, result_format=result_format)
+                    try:
+                        result = decoratee(*decoratee_args, **decoratee_kwargs)
+                        return scope.completed(result=result, result_format=result_format)
+                    except Cancellation as e:
+                        return scope.canceled(result=e.result, result_format=e.result_format, message=str(e))
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
     return factory
 
 
@@ -317,16 +372,7 @@
 
 def _set_func_name(record: logging.LogRecord, name: str):
     record.funcName = name
 
 
 def _set_module_name(record: logging.LogRecord, name: str):
     record.module = name
-
-
-def _set_exc_text(record: logging.LogRecord):
-    if record.exc_info:
-        record.exc_text = logging.Formatter().formatException(record.exc_info)
-
-
-def _set_attachment(record: logging.LogRecord, value: Optional[Any]):
-    record.attachment = record.exc_text or value
```

## Comparing `wiretap-4.2.2.dist-info/RECORD` & `wiretap-5.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-wiretap/__init__.py,sha256=GIE5maAodEwZuEx88O1A-e9tjnv5Fl_lA6DfVQtGdCA,131
+wiretap/__init__.py,sha256=k7Ug6yarTCPvPv1NKjoHrC-Cw4cFZ25FGxBG88Ra7pM,140
 wiretap/layers.py,sha256=KUAcHoCD4DsiBqd85OndrxZpxl0YVYfr2UKm8Co0004,620
-wiretap/wiretap.py,sha256=s7Oq2E1VECPvXucwZXvLrkyiNemrvp4M5ZBQv-8wEFQ,12354
-wiretap-4.2.2.dist-info/METADATA,sha256=tJjA-En_vFGkxL0map9-nbMe2LYo29d3chWcm6Vv5iw,244
-wiretap-4.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-wiretap-4.2.2.dist-info/top_level.txt,sha256=qmBPPxbsuDq57r7kh5q29WKFFyvB8j8Mzgx5RKHnwAw,8
-wiretap-4.2.2.dist-info/RECORD,,
+wiretap/wiretap.py,sha256=UP7BLF0HoYJV5wamEihu-TNIq3znm6_7cpcgDpqn6yM,14455
+wiretap-5.0.0.dist-info/METADATA,sha256=yQ3aB3czjM2OUtoXdEA_5V_3LQy_r8-NhDwbADNbBCQ,244
+wiretap-5.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+wiretap-5.0.0.dist-info/top_level.txt,sha256=qmBPPxbsuDq57r7kh5q29WKFFyvB8j8Mzgx5RKHnwAw,8
+wiretap-5.0.0.dist-info/RECORD,,
```

