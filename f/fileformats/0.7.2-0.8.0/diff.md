# Comparing `tmp/fileformats-0.7.2.tar.gz` & `tmp/fileformats-0.8.0.tar.gz`

## Comparing `fileformats-0.7.2.tar` & `fileformats-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/archive/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/converter.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/datatype.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/field.py
--rw-r--r--   0        0        0    45195 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/mark.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/mixin.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/image/base.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/testing/headers.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.7.2/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.7.2/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.7.2/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.7.2/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.7.2/README.rst
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fileformats-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    22348 2020-02-02 00:00:00.000000 fileformats-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/datatype.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/field.py
+-rw-r--r--   0        0        0    45604 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/mark.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    11540 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/model/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.0/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.0/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.8.0/README.rst
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fileformats-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    22348 2020-02-02 00:00:00.000000 fileformats-0.8.0/PKG-INFO
```

### Comparing `fileformats-0.7.2/fileformats/archive/__init__.py` & `fileformats-0.8.0/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/converter.py` & `fileformats-0.8.0/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/datatype.py` & `fileformats-0.8.0/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/exceptions.py` & `fileformats-0.8.0/fileformats/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/field.py` & `fileformats-0.8.0/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/fileset.py` & `fileformats-0.8.0/fileformats/core/fileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     fspaths: ty.FrozenSet[Path] = attrs.field(default=None, converter=fspaths_converter)
 
     # Explicitly set the Internet Assigned Numbers Authority (https://iana_mime.org) MIME
     # type to None for any base classes that should not correspond to a MIME or MIME-like
     # type.
     iana_mime = None
-    ext = ""
+    ext = None
 
     # Store converters registered by @converter decorator that convert to FileSet
     # NB: each class will have its own version of this dictionary
     converters = {}
 
     is_fileset = True
 
@@ -168,14 +168,25 @@
         if getattr(cls, "iana_mime", None) is not None:
             mime_type = cls.iana_mime
         else:
             format_name = to_mime_format_name(cls.__name__)
             mime_type = f"application/x-{format_name}"
         return mime_type
 
+    @classproperty
+    def strext(cls) -> str:
+        """Return extension that is guaranteed to be a string (i.e. not None)"""
+        return cls.ext if cls.ext is not None else ""
+
+    @classproperty
+    def unconstrained(cls) -> bool:
+        """Whether the file-format is unconstrained by extension, magic number or another
+        constraint"""
+        return not list(cls.required_properties())
+
     @classmethod
     def required_properties(cls):
         """Find all properties required to treat file-set as being in the format specified
         by the class
 
         Returns
         -------
@@ -323,15 +334,17 @@
         list[Path]
             the matching paths
 
         Raises
         ------
         FileFormatError
             When no paths match or more than one path matches the given extension"""
-        return [p for p in fspaths if any(str(p).endswith(e) for e in exts)]
+        return [
+            p for p in fspaths if any(e is None or str(p).endswith(e) for e in exts)
+        ]
 
     @classmethod
     def convert(cls, fileset, plugin="serial", task_name=None, **kwargs):
         """Convert a given file-set into the format specified by the class
 
         Parameters
         ----------
@@ -412,20 +425,20 @@
                     f"'{source_format.mime_like}':\n{available_str}"
                 ) from None
             elif not available_converters:
                 msg = (
                     f"Could not find converter between '{source_format.mime_like}' and "
                     f"'{cls.mime_like}' formats"
                 )
-                extras_imported, sub_pkg = import_extras_module(cls)
+                extras_imported, extras_pkg, extras_pypi = import_extras_module(cls)
                 if not extras_imported:
                     msg += (
-                        f'. Was not able to import "extras" module, fileformats.extras.{sub_pkg}, '
-                        f"you may want to try installing the 'fileformats-{sub_pkg}-extras' package "
-                        f"from PyPI (e.g. pip install fileformats-{sub_pkg}-extras)"
+                        f'. Was not able to import "extras" module, {extras_pkg}, '
+                        f"you may want to try installing the '{extras_pypi}' package "
+                        f"from PyPI (e.g. pip install {extras_pypi})"
                     )
                 raise FormatConversionError(msg) from None
             converter_tuple = available_converters[0]
             # Store mapping for future reference
             converters[source_format] = converter_tuple
         converter, conv_kwargs = converter_tuple
         if kwargs:
```

### Comparing `fileformats-0.7.2/fileformats/core/mark.py` & `fileformats-0.8.0/fileformats/core/mark.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,30 +128,29 @@
     """A decorator which uses singledispatch to facilitate the registering of
     "extra" functionality in external packages (e.g. "fileformats-extras")"""
 
     functools.wraps(method)
 
     def decorated(obj, *args, **kwargs):
         cls = type(obj)
-        extras_imported, sub_pkg = import_extras_module(cls)
+        extras_imported, extras_pkg, extras_pypi = import_extras_module(cls)
         try:
             return method(obj, *args, **kwargs)
         except NotImplementedError:
             if extras_imported:
                 msg = f"No implementation for '{method.__name__}' extra for {cls.__name__} types"
             else:
-                extras_pkg = f"fileformats-{sub_pkg}-extras"
                 try:
-                    if check_package_exists_on_pypi(extras_pkg):
+                    if check_package_exists_on_pypi(extras_pypi):
                         msg += (
-                            f'. An "extras" package exists on PyPI ({extras_pkg}), '
+                            f'. An "extras" package exists on PyPI ({extras_pypi}), '
                             "which may contain an implementation, try installing it "
-                            f"(e.g. 'pip install {extras_pkg}') and check again"
+                            f"(e.g. 'pip install {extras_pypi}') and check again"
                         )
                 except urllib.error.URLError:
                     msg += (
                         '. Was not able to check whether an "extras" package '
-                        f"({extras_pkg}) exists on PyPI or not"
+                        f"({extras_pypi}) exists on PyPI or not"
                     )
             raise FileFormatsExtrasError(msg)
 
     return functools.singledispatch(decorated)
```

### Comparing `fileformats-0.7.2/fileformats/core/mixin.py` & `fileformats-0.8.0/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/utils.py` & `fileformats-0.8.0/fileformats/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,31 +36,42 @@
     if flag:
         _excluded_subpackages.remove("testing")
     else:
         _excluded_subpackages.add("testing")
 
 
 def find_matching(
-    fspaths: ty.List[Path], standard_only: bool = False, include_generic: bool = False
+    fspaths: ty.List[Path],
+    candidates: ty.Sequence = None,
+    standard_only: bool = False,
+    include_generic: bool = False,
+    skip_unconstrained: bool = True,
 ):
     """Detect the corresponding file format from a set of file-system paths
 
     Parameters
     ----------
     fspaths : list[Path]
         file-system paths to detect the format of
+    candidates: sequence[DataType], optional
+        the candidates to select from, by default all file formats
     standard_only : bool, optional
         If you only want to return matches from the "standard" IANA types, by default False
-    include_generic : bool, optional
-        Include generic file-set types (i.e ones within the fileformats.generic package),
-        by default False
+    skip_unconstrained : bool, optional
+        skip formats that aren't constrained by extension, magic number or another check
     """
+    import fileformats.core.mixin
+
     fspaths = fspaths_converter(fspaths)
     matches = []
-    for frmt in fileformats.core.FileSet.all_formats:
+    if candidates is None:
+        candidates = fileformats.core.FileSet.all_formats
+    for frmt in candidates:
+        if skip_unconstrained and frmt.unconstrained:
+            continue
         namespace = frmt.namespace
         if (
             frmt.matches(fspaths)
             and (not standard_only or namespace in STANDARD_NAMESPACES)
             and (include_generic or namespace != "generic")
         ):
             matches.append(frmt)
@@ -115,17 +126,17 @@
         ty.Iterable[ty.Union[str, os.PathLike, bytes]],
         str,
         os.PathLike,
         bytes,
         fileformats.core.FileSet,
     ]
 ):
+    """Ensures fs-paths are a set of pathlib.Path"""
     import fileformats.core
 
-    """Ensures fs-paths are a set of pathlib.Path"""
     if isinstance(fspaths, fileformats.core.FileSet):
         fspaths = fspaths.fspaths
     elif isinstance(fspaths, (str, os.PathLike, bytes)):
         fspaths = [fspaths]
     return frozenset(Path(p).absolute() for p in fspaths)
 
 
@@ -169,37 +180,43 @@
 
 
 STANDARD_NAMESPACES = [
     "archive",
     "audio",
     "document",
     "image",
+    "misc",
+    "model",
     "numeric",
     "serialization",
     "text",
     "video",
 ]
 
 
 def to_mime_format_name(format_name: str):
     if "___" in format_name:
         raise FileFormatsError(
             f"Cannot convert name of format class {format_name} to mime string as it "
             "contains triple underscore"
         )
+    if format_name.startswith("_"):
+        format_name = format_name[1:]
     format_name = format_name[0].lower() + format_name[1:]
     format_name = re.sub("__([A-Z])", lambda m: "+" + m.group(1).lower(), format_name)
     format_name = re.sub("_([A-Z])", lambda m: "." + m.group(1).lower(), format_name)
     format_name = re.sub("([A-Z])", lambda m: "-" + m.group(1).lower(), format_name)
     return format_name
 
 
 def from_mime_format_name(format_name: str):
     if format_name.startswith("x-"):
         format_name = format_name[2:]
+    if re.match(r"^[0-9]", format_name):
+        format_name = "_" + format_name
     format_name = format_name.capitalize()
     format_name = re.sub(r"(\.)(\w)", lambda m: "_" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(\+)(\w)", lambda m: "__" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(-)(\w)", lambda m: m.group(2).upper(), format_name)
     return format_name
 
 
@@ -290,16 +307,21 @@
     if pkg_parts[0] != "fileformats":
         logger.debug(
             "There is no 'extras' module for classes not within the 'fileformats' package, "
             "not %s in %s",
             klass.__name__,
             klass.__module__,
         )
-        return True, None
+        return True, None, None
     sub_pkg = pkg_parts[1]
+    extras_pkg = "fileformats.extras." + sub_pkg
+    if sub_pkg in STANDARD_NAMESPACES:
+        extras_pypi = "fileformats-extras"
+    else:
+        extras_pypi = f"fileformats-{sub_pkg}-extras"
     try:
-        importlib.import_module("fileformats.extras." + sub_pkg)
+        importlib.import_module(extras_pkg)
     except ImportError:
         extras_imported = False
     else:
         extras_imported = True
-    return extras_imported, sub_pkg
+    return extras_imported, extras_pkg, extras_pypi
```

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.0/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_converter.py` & `fileformats-0.8.0/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_detection.py` & `fileformats-0.8.0/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_general.py` & `fileformats-0.8.0/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_mime.py` & `fileformats-0.8.0/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.0/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.0/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.0/fileformats/core/tests/test_test_extras.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/core/tests/test_utils.py` & `fileformats-0.8.0/fileformats/core/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,16 +285,19 @@
 def test_format_detection(work_dir):
     text_file = work_dir / "text.txt"
 
     with open(text_file, "w") as f:
         f.write("sample text")
 
     detected = find_matching(text_file, standard_only=True)
-    assert len(detected) == 1
-    assert detected[0] is fileformats.text.Plain
+    assert sorted(detected, key=lambda f: f.mime_like) == [
+        fileformats.text.Prs_Fallenstein_Rst,
+        fileformats.text.Prs_Prop_Logic,
+        fileformats.text.Unstructured,
+    ]
 
 
 def test_missing_dependency():
     missing_dep = MissingExtendedDependency("missing_dep", "fileformats.image")
 
     with pytest.raises(MissingExtendedDepenciesError):
         missing_dep.an_attr
```

### Comparing `fileformats-0.7.2/fileformats/document/__init__.py` & `fileformats-0.8.0/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/field/__init__.py` & `fileformats-0.8.0/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/field/tests/test_fields.py` & `fileformats-0.8.0/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.0/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/generic/__init__.py` & `fileformats-0.8.0/fileformats/generic/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,33 +30,48 @@
         to functions like file 'open'"""
         return str(self)
 
     @property
     def stem(self):
         return self.fspath.with_suffix("").name
 
+    @classproperty
+    def unconstrained(cls) -> bool:
+        """Whether the file-format is unconstrained by extension, magic number or another
+        constraint"""
+        # We have to subtract `fspath` from required properties as we defined unconstrained
+        # file-sets as ones that have more constraints than simply existing
+        return not (len(list(cls.required_properties())) - 1)
+
 
 class File(FsObject):
     """Generic file type"""
 
     binary = False
     is_dir = False
+    alternate_exts = ()
 
     @mark.required
     @property
     def fspath(self):
         fspath = self.select_by_ext()
         if fspath.is_dir():
             # fspath is guaranteed to exist
             raise FormatMismatchError(
                 f'Path that matches extension of {type(self)}, "{fspath}", '
                 f"is a directory not a file"
             )
         return fspath
 
+    @classproperty
+    def unconstrained(cls) -> bool:
+        """Whether the file-format is unconstrained by extension, magic number or another
+        constraint"""
+        return super().unconstrained and (cls.ext is None or None in cls.alternate_exts)
+
     @classmethod
     def copy_ext(
         cls,
         old_path: Path,
         new_path: Path,
         decomposition_mode=FileSet.ExtensionDecomposition.none,
     ):
@@ -176,14 +191,20 @@
         for content_type in self.content_types:
             for p in self.fspath.iterdir():
                 try:
                     yield content_type([p])
                 except FormatMismatchError:
                     continue
 
+    @classproperty
+    def unconstrained(cls) -> bool:
+        """Whether the file-format is unconstrained by extension, magic number or another
+        constraint"""
+        return super().unconstrained and not cls.content_types
+
     @mark.check
     def validate_contents(self):
         if not self.content_types:
             return
         not_found = set(self.content_types)
         for fspath in self.fspath.iterdir():
             for content_type in list(not_found):
```

### Comparing `fileformats-0.7.2/fileformats/image/raster.py` & `fileformats-0.8.0/fileformats/image/raster.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         return cls(fspath)
 
 
 class Bitmap(WithMagicNumber, RasterImage):
     ext = ".bmp"
     magic_number = b"BM"
     iana_mime = "image/bmp"
+    alternative_exts = (".dib",)
 
 
 class Gif(WithMagicNumber, RasterImage):
     ext = ".gif"
     iana_mime = "image/gif"
     magic_number = b"GIF8"
```

### Comparing `fileformats-0.7.2/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.0/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/testing/classifiers.py` & `fileformats-0.8.0/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/fileformats/testing/headers.py` & `fileformats-0.8.0/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/LICENSE` & `fileformats-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/README.rst` & `fileformats-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/pyproject.toml` & `fileformats-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.2/PKG-INFO` & `fileformats-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.7.2
+Version: 0.8.0
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

