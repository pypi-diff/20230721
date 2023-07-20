# Comparing `tmp/respx-0.8.3.tar.gz` & `tmp/respx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/respx-0.8.3.tar", last modified: Fri Jan 10 12:49:17 2020, max compression
+gzip compressed data, was "dist/respx-0.9.0.tar", last modified: Wed Jan 22 10:28:32 2020, max compression
```

## Comparing `respx-0.8.3.tar` & `respx-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-10 12:49:17.000000 respx-0.8.3/
--rw-r--r--   0 jonas      (501) staff       (20)     2496 2020-01-10 12:48:36.000000 respx-0.8.3/CHANGELOG.md
--rw-r--r--   0 jonas      (501) staff       (20)       62 2020-01-07 07:50:33.000000 respx-0.8.3/MANIFEST.in
--rw-r--r--   0 jonas      (501) staff       (20)     1898 2020-01-10 12:49:17.000000 respx-0.8.3/PKG-INFO
--rw-r--r--   0 jonas      (501) staff       (20)      867 2020-01-10 12:45:29.000000 respx-0.8.3/README.md
-drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-10 12:49:17.000000 respx-0.8.3/respx/
--rw-r--r--   0 jonas      (501) staff       (20)      349 2019-12-09 08:30:48.000000 respx-0.8.3/respx/__init__.py
--rw-r--r--   0 jonas      (501) staff       (20)       22 2020-01-10 12:46:10.000000 respx-0.8.3/respx/__version__.py
--rw-r--r--   0 jonas      (501) staff       (20)    13413 2020-01-10 12:45:29.000000 respx-0.8.3/respx/api.py
--rw-r--r--   0 jonas      (501) staff       (20)     7665 2020-01-10 12:45:29.000000 respx-0.8.3/respx/models.py
--rw-r--r--   0 jonas      (501) staff       (20)        0 2019-12-09 08:30:48.000000 respx-0.8.3/respx/py.typed
-drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/
--rw-r--r--   0 jonas      (501) staff       (20)     1898 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/PKG-INFO
--rw-r--r--   0 jonas      (501) staff       (20)      308 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/SOURCES.txt
--rw-r--r--   0 jonas      (501) staff       (20)        1 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/dependency_links.txt
--rw-r--r--   0 jonas      (501) staff       (20)        1 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/not-zip-safe
--rw-r--r--   0 jonas      (501) staff       (20)       24 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/requires.txt
--rw-r--r--   0 jonas      (501) staff       (20)        6 2020-01-10 12:49:17.000000 respx-0.8.3/respx.egg-info/top_level.txt
--rw-r--r--   0 jonas      (501) staff       (20)      937 2020-01-10 12:49:17.000000 respx-0.8.3/setup.cfg
--rw-r--r--   0 jonas      (501) staff       (20)     1275 2020-01-10 12:45:29.000000 respx-0.8.3/setup.py
+drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-22 10:28:32.000000 respx-0.9.0/
+-rw-r--r--   0 jonas      (501) staff       (20)     2496 2020-01-10 12:49:57.000000 respx-0.9.0/CHANGELOG.md
+-rw-r--r--   0 jonas      (501) staff       (20)       62 2020-01-07 07:50:33.000000 respx-0.9.0/MANIFEST.in
+-rw-r--r--   0 jonas      (501) staff       (20)     1898 2020-01-22 10:28:32.000000 respx-0.9.0/PKG-INFO
+-rw-r--r--   0 jonas      (501) staff       (20)      867 2020-01-10 12:45:29.000000 respx-0.9.0/README.md
+drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-22 10:28:32.000000 respx-0.9.0/respx/
+-rw-r--r--   0 jonas      (501) staff       (20)      336 2020-01-22 10:26:07.000000 respx-0.9.0/respx/__init__.py
+-rw-r--r--   0 jonas      (501) staff       (20)       22 2020-01-22 10:27:37.000000 respx-0.9.0/respx/__version__.py
+-rw-r--r--   0 jonas      (501) staff       (20)    15383 2020-01-22 10:26:07.000000 respx-0.9.0/respx/api.py
+-rw-r--r--   0 jonas      (501) staff       (20)      268 2020-01-22 10:26:07.000000 respx-0.9.0/respx/fixtures.py
+-rw-r--r--   0 jonas      (501) staff       (20)     7665 2020-01-17 07:51:24.000000 respx-0.9.0/respx/models.py
+-rw-r--r--   0 jonas      (501) staff       (20)        0 2019-12-09 08:30:48.000000 respx-0.9.0/respx/py.typed
+drwxr-xr-x   0 jonas      (501) staff       (20)        0 2020-01-22 10:28:32.000000 respx-0.9.0/respx.egg-info/
+-rw-r--r--   0 jonas      (501) staff       (20)     1898 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/PKG-INFO
+-rw-r--r--   0 jonas      (501) staff       (20)      326 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas      (501) staff       (20)        1 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas      (501) staff       (20)        1 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/not-zip-safe
+-rw-r--r--   0 jonas      (501) staff       (20)       28 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/requires.txt
+-rw-r--r--   0 jonas      (501) staff       (20)        6 2020-01-22 10:28:31.000000 respx-0.9.0/respx.egg-info/top_level.txt
+-rw-r--r--   0 jonas      (501) staff       (20)      984 2020-01-22 10:28:32.000000 respx-0.9.0/setup.cfg
+-rw-r--r--   0 jonas      (501) staff       (20)     1279 2020-01-22 10:26:07.000000 respx-0.9.0/setup.py
```

### Comparing `respx-0.8.3/CHANGELOG.md` & `respx-0.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `respx-0.8.3/PKG-INFO` & `respx-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: respx
-Version: 0.8.3
+Version: 0.9.0
 Summary: A utility for mocking out the Python HTTPX library.
 Home-page: https://github.com/lundberg/respx
 Author: Jonas Lundberg
 Author-email: jonas@5monkeys.se
 License: MIT
 Description: # RESPX
```

### Comparing `respx-0.8.3/README.md` & `respx-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `respx-0.8.3/respx/api.py` & `respx-0.9.0/respx/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
 class HTTPXMock:
     def __init__(
         self,
         assert_all_called: bool = True,
         assert_all_mocked: bool = True,
         base_url: typing.Optional[str] = None,
-        local: bool = True,
+        proxy: typing.Optional["HTTPXMock"] = None,
     ) -> None:
-        self._is_local = local
         self._assert_all_called = assert_all_called
         self._assert_all_mocked = assert_all_mocked
         self._base_url = base_url
+        self._proxy = proxy
+        self._mocks: typing.List[HTTPXMock] = []
         self._patchers: typing.List[asynctest.mock._patch] = []
         self._patterns: typing.List[RequestPattern] = []
         self.aliases: typing.Dict[str, RequestPattern] = {}
         self.stats = asynctest.mock.MagicMock()
         self.calls: typing.List[typing.Tuple[Request, typing.Optional[Response]]] = []
 
     def __call__(
@@ -47,101 +48,143 @@
         """
         Decorator or Context Manager.
 
         Use decorator/manager with parentheses for local state, or without parentheses
         for global state, i.e. shared patterns added outside of scope.
         """
         if func is None:
-            # A. First stage of "local" decorator, WITH parentheses.
-            # B. Only stage of "local" context manager, WITH parentheses,
-            #    "global" context maanager hits __enter__ directly.
-            settings: typing.Dict[str, typing.Any] = {"base_url": base_url}
+            # Parantheses used, branch out to new nested instance.
+            # - Only stage when using local ctx `with respx.mock(...) as httpx_mock:`
+            # - First stage when using local decorator `@respx.mock(...)`
+            #   FYI, global ctx `with respx.mock:` hits __enter__ directly
+            settings: typing.Dict[str, typing.Any] = {
+                "base_url": base_url,
+                "proxy": self,
+            }
             if assert_all_called is not None:
                 settings["assert_all_called"] = assert_all_called
             if assert_all_mocked is not None:
                 settings["assert_all_mocked"] = assert_all_mocked
             return self.__class__(**settings)
 
         # Async Decorator
         @wraps(func)
         async def async_decorator(*args, **kwargs):
             assert func is not None
-            if self._is_local:
+            if self._proxy:
                 kwargs["httpx_mock"] = self
             async with self:
                 return await func(*args, **kwargs)
 
         # Sync Decorator
         @wraps(func)
         def sync_decorator(*args, **kwargs):
             assert func is not None
-            if self._is_local:
+            if self._proxy:
                 kwargs["httpx_mock"] = self
             with self:
                 return func(*args, **kwargs)
 
-        # Dispatch async/sync decorator, depening on decorated function
-        # A. Second stage of "local" decorator, WITH parentheses.
-        # A. Only stage of "global" decorator, WITHOUT parentheses.
+        # Dispatch async/sync decorator, depening on decorated function.
+        # - Only stage when using global decorator `@respx.mock`
+        # - Second stage when using local decorator `@respx.mock(...)`
         return async_decorator if inspect.iscoroutinefunction(func) else sync_decorator
 
     def __enter__(self) -> "HTTPXMock":
         self.start()
         return self
 
+    def __exit__(self, *args: typing.Any) -> None:
+        self.stop()
+
     async def __aenter__(self) -> "HTTPXMock":
         return self.__enter__()
 
-    def __exit__(self, *args: typing.Any) -> None:
-        try:
-            if self._assert_all_called:
-                self.assert_all_called()
-        finally:
-            self.stop()
-
     async def __aexit__(self, *args: typing.Any) -> None:
         self.__exit__(*args)
 
     def start(self) -> None:
         """
-        Starts mocking httpx.
+        Register mock/patterns and starts patching HTTPX.
+        """
+        self._register(self)
+
+    def stop(self, clear: bool = True, reset: bool = True) -> None:
+        """
+        Unregister mock/patterns and stop patching HTTPX, when no registered mocks left.
         """
+        try:
+            if self._assert_all_called:
+                self.assert_all_called()
+        finally:
+            if clear:
+                self.clear()
+            if reset:
+                self.reset()
+
+            self._unregister(self)
+
+    def _register(self, httpx_mock: "HTTPXMock") -> None:
+        # Ensure we patch HTTPX using proxy instance
+        if self._proxy:
+            self._proxy._register(httpx_mock)
+            return
+
+        # Register given mock instance / patterns
+        self._mocks.append(httpx_mock)
+        self._patch()
+
+    def _unregister(self, httpx_mock: "HTTPXMock") -> None:
+        # Ensure we unpatch HTTPX using proxy instance
+        if self._proxy is not None:
+            self._proxy._unregister(httpx_mock)
+            return
+
+        # Unregister given mock instance / patterns
+        assert httpx_mock in self._mocks, "HTTPX mock already stopped!"
+        self._mocks.remove(httpx_mock)
+        self._unpatch()
+
+    def _patch(self) -> None:
+        # Ensure we only patch HTTPX once!
+        if self._patchers:
+            return
+
         # Unbound -> bound spy version of Client.send
         def unbound_sync_send(
             client: Client, request: Request, **kwargs: typing.Any
         ) -> Response:
             return self.__Client__send__spy(client, request, **kwargs)
 
         # Unbound -> bound spy version of AsyncClient.send
         async def unbound_async_send(
             client: AsyncClient, request: Request, **kwargs: typing.Any
         ) -> Response:
             return await self.__AsyncClient__send__spy(client, request, **kwargs)
 
+        # Start patching HTTPX
         mockers = (
             ("httpx.Client.send", unbound_sync_send),
             ("httpx.AsyncClient.send", unbound_async_send),
         )
         for target, mocker in mockers:
             patcher = asynctest.mock.patch(target, new=mocker)
             patcher.start()
             self._patchers.append(patcher)
 
-    def stop(self, reset: bool = True) -> None:
-        """
-        Stops mocking httpx.
-        """
+    def _unpatch(self) -> None:
+        # Ensure we don't stop patching HTTPX when registered mocks exists
+        if self._mocks:
+            return
+
+        # Stop patching HTTPX
         while self._patchers:
             patcher = self._patchers.pop()
             patcher.stop()
 
-        if reset:
-            self.clear()
-            self.reset()
-
     def clear(self) -> None:
         """
         Clears added patterns and aliases.
         """
         self._patterns.clear()
         self.aliases.clear()
 
@@ -204,58 +247,67 @@
 
     def __getitem__(self, alias: str) -> typing.Optional[RequestPattern]:
         return self.aliases.get(alias)
 
     def _match(
         self, request: Request
     ) -> typing.Tuple[
-        typing.Optional[RequestPattern], typing.Optional[ResponseTemplate]
+        "HTTPXMock", typing.Optional[RequestPattern], typing.Optional[ResponseTemplate]
     ]:
         matched_pattern: typing.Optional[RequestPattern] = None
         matched_pattern_index: typing.Optional[int] = None
         response: typing.Optional[ResponseTemplate] = None
+        # if request.url == "https://foo.bar/asgi/":
+        # import pdb; pdb.set_trace()
 
-        for i, pattern in enumerate(self._patterns):
-            match = pattern.match(request)
-            if not match:
-                continue
-
-            if matched_pattern_index is not None:
-                # Multiple matches found, drop and use the first one
-                self._patterns.pop(matched_pattern_index)
-                break
-
-            matched_pattern = pattern
-            matched_pattern_index = i
+        # Iterate all started mockers and their patterns
+        for httpx_mock in self._mocks:
+            patterns = httpx_mock._patterns
+
+            for i, pattern in enumerate(patterns):
+                match = pattern.match(request)
+                if not match:
+                    continue
+
+                if matched_pattern_index is not None:
+                    # Multiple matches found, drop and use the first one
+                    patterns.pop(matched_pattern_index)
+                    break
+
+                used_mock = httpx_mock
+                matched_pattern = pattern
+                matched_pattern_index = i
+
+                if isinstance(match, ResponseTemplate):
+                    # Mock response
+                    response = match
+                elif isinstance(match, Request):
+                    # Pass-through request
+                    response = None
+                else:
+                    raise ValueError(
+                        (
+                            "Matched request pattern must return either a "
+                            'ResponseTemplate or a Request, got "{}"'
+                        ).format(type(match))
+                    )
 
-            if isinstance(match, ResponseTemplate):
-                # Mock response
-                response = match
-            elif isinstance(match, Request):
-                # Pass-through request
-                response = None
-            else:
-                raise ValueError(
-                    (
-                        "Matched request pattern must return either a "
-                        'ResponseTemplate or a Request, got "{}"'
-                    ).format(type(match))
-                )
-
-        # Assert we always get a pattern match, if check is enabled
-        assert (
-            not self._assert_all_mocked
-            or self._assert_all_mocked
-            and matched_pattern is not None
-        ), f"RESPX: {request!r} not mocked!"
+            if matched_pattern:
+                break
 
         if matched_pattern is None:
+            # Assert we always get a pattern match, if check is enabled
+            allows_unmocked = tuple(m for m in self._mocks if not m._assert_all_mocked)
+            assert allows_unmocked, f"RESPX: {request!r} not mocked!"
+
+            # Relate default response to first mocker that allows unmocked requests
+            used_mock = allows_unmocked[0]
             response = ResponseTemplate()
 
-        return matched_pattern, response
+        return used_mock, matched_pattern, response
 
     def _capture(
         self,
         request: Request,
         response: typing.Optional[Response],
         pattern: typing.Optional[RequestPattern] = None,
     ) -> None:
@@ -269,21 +321,21 @@
 
         # Copy stats due to unwanted use of property refs in the high-level api
         self.calls[:] = (
             (request, response) for (request, response), _ in self.stats.call_args_list
         )
 
     @contextmanager
-    def _patch_backend(
+    def _patch_dispatcher(
         self, dispatch: typing.Union[SyncDispatcher, AsyncDispatcher], request: Request
     ) -> typing.Iterator[typing.Callable]:
         patchers = []
 
         # 1. Match request against added patterns
-        pattern, response = self._match(request)
+        httpx_mock, pattern, response = self._match(request)
 
         if response is not None:
             # 2. Patch request url with response for later pickup in patched dispatcher
             request.url = URLResponse(request.url, response)
 
             backend = getattr(dispatch, "backend", None)
             if isinstance(backend, ConcurrencyBackend):
@@ -301,66 +353,64 @@
 
             for obj, target, mocker in mockers:
                 patcher = asynctest.mock.patch.object(obj, target, mocker)
                 patcher.start()
                 patchers.append(patcher)
 
         try:
-            yield partial(self._capture, pattern=pattern)
+            yield partial(httpx_mock._capture, pattern=pattern)
         finally:
             # 4. Stop patching
             for patcher in patchers:
                 patcher.stop()
 
     def __Client__send__spy(
         self, client: Client, request: Request, **kwargs: typing.Any
     ) -> Response:
         """
         Spy for Client.send().
 
         Patches request.url and attaches matched response template,
-        and mocks client backend open stream methods.
+        and mocks client dispatcher send method.
         """
-        with self._patch_backend(client.dispatch, request) as capture:
+        with self._patch_dispatcher(client.dispatch, request) as capture:
             try:
                 response = None
                 response = _Client__send(client, request, **kwargs)
                 return response
             finally:
                 capture(request, response)
 
     async def __AsyncClient__send__spy(
         self, client: AsyncClient, request: Request, **kwargs: typing.Any
     ) -> Response:
         """
         Spy for AsyncClient.send().
 
         Patches request.url and attaches matched response template,
-        and mocks client backend open stream methods.
+        and mocks client concurrency backend open stream methods.
         """
-        with self._patch_backend(client.dispatch, request) as capture:
+        with self._patch_dispatcher(client.dispatch, request) as capture:
             try:
                 response = None
                 response = await _AsyncClient__send(client, request, **kwargs)
                 return response
             finally:
                 capture(request, response)
 
     def __SyncDispatcher__send__mock(
         self, request: Request, **kwargs: typing.Any
     ) -> Response:
-        # TODO: Support pass-through
         hostname = request.url.host
         response = getattr(hostname, "attachment", None)  # Pickup attached template
         return response.build(request)
 
     async def __AsyncDispatcher__send__mock(
         self, request: Request, **kwargs: typing.Any
     ) -> Response:
-        # TODO: Support pass-through
         hostname = request.url.host
         response = getattr(hostname, "attachment", None)  # Pickup attached template
         return await response.abuild(request)
 
     async def __Backend__open_tcp_stream__mock(
         self,
         hostname: str,
```

### Comparing `respx-0.8.3/respx/models.py` & `respx-0.9.0/respx/models.py`

 * *Files identical despite different names*

### Comparing `respx-0.8.3/respx.egg-info/PKG-INFO` & `respx-0.9.0/respx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: respx
-Version: 0.8.3
+Version: 0.9.0
 Summary: A utility for mocking out the Python HTTPX library.
 Home-page: https://github.com/lundberg/respx
 Author: Jonas Lundberg
 Author-email: jonas@5monkeys.se
 License: MIT
 Description: # RESPX
```

### Comparing `respx-0.8.3/setup.cfg` & `respx-0.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 disallow_incomplete_defs = True
 ignore_missing_imports = False
 warn_unused_configs = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_unreachable = True
 
+[mypy-pytest.*]
+ignore_missing_imports = True
+
 [mypy-asynctest.*]
 ignore_missing_imports = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `respx-0.8.3/setup.py` & `respx-0.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,9 +28,9 @@
         "Programming Language :: Python :: 3.8",
     ],
     packages=["respx"],
     package_data={"httpx": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.6",
-    install_requires=["httpx==0.11.0", "asynctest"],
+    install_requires=["httpx>=0.11,<0.12", "asynctest"],
 )
```

