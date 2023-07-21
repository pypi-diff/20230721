# Comparing `tmp/vf-flags-0.2.3.tar.gz` & `tmp/vf-flags-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vf-flags-0.2.3.tar", last modified: Sun Feb 26 13:56:37 2023, max compression
+gzip compressed data, was "vf-flags-0.2.4.tar", last modified: Fri Jul 21 02:27:39 2023, max compression
```

## Comparing `vf-flags-0.2.3.tar` & `vf-flags-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 13:56:37.318143 vf-flags-0.2.3/
--rw-rw-rw-   0        0        0    35184 2023-01-13 17:01:05.000000 vf-flags-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    42996 2023-02-26 13:56:37.305130 vf-flags-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-01-13 23:16:44.000000 vf-flags-0.2.3/README.rst
--rw-rw-rw-   0        0        0     1111 2023-02-22 08:08:18.000000 vf-flags-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-26 13:56:37.332155 vf-flags-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-26 13:56:37.285112 vf-flags-0.2.3/vf_flags.egg-info/
--rw-rw-rw-   0        0        0    42996 2023-02-26 13:56:37.000000 vf-flags-0.2.3/vf_flags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-02-26 13:56:37.000000 vf-flags-0.2.3/vf_flags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 13:56:37.000000 vf-flags-0.2.3/vf_flags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-26 13:56:37.000000 vf-flags-0.2.3/vf_flags.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-26 13:56:37.000000 vf-flags-0.2.3/vf_flags.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-26 13:56:37.300125 vf-flags-0.2.3/vfflags/
--rw-rw-rw-   0        0        0     4661 2023-02-22 08:07:58.000000 vf-flags-0.2.3/vfflags/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-13 23:16:44.000000 vf-flags-0.2.3/vfflags/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.044876 vf-flags-0.2.4/
+-rw-rw-rw-   0        0        0    35184 2023-01-13 17:01:05.000000 vf-flags-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    42996 2023-07-21 02:27:39.043876 vf-flags-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-01-13 23:16:44.000000 vf-flags-0.2.4/README.rst
+-rw-rw-rw-   0        0        0     1111 2023-07-21 02:26:39.000000 vf-flags-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:27:39.044876 vf-flags-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.037871 vf-flags-0.2.4/vf_flags.egg-info/
+-rw-rw-rw-   0        0        0    42996 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-21 02:27:39.000000 vf-flags-0.2.4/vf_flags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.041874 vf-flags-0.2.4/vfflags/
+-rw-rw-rw-   0        0        0     4728 2023-07-21 02:26:23.000000 vf-flags-0.2.4/vfflags/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-13 23:16:44.000000 vf-flags-0.2.4/vfflags/py.typed
```

### Comparing `vf-flags-0.2.3/LICENSE` & `vf-flags-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vf-flags-0.2.3/PKG-INFO` & `vf-flags-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-flags
-Version: 0.2.3
+Version: 0.2.4
 Summary: A wrapper for easily making bitwise flags.
 Author-email: Kae Bartlett <kae@voxelfox.co.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `vf-flags-0.2.3/README.rst` & `vf-flags-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `vf-flags-0.2.3/pyproject.toml` & `vf-flags-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [tool.setuptools]
 packages.find.where = ["."]
 package-data.vfflags = ["*.pyi", "py.typed"]
 
 
 [project]
 name = "vf-flags"
-version = "0.2.3"
+version = "0.2.4"
 description = "A wrapper for easily making bitwise flags."
 authors = [
     {name = "Kae Bartlett", email = "kae@voxelfox.co.uk"},
 ]
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `vf-flags-0.2.3/vf_flags.egg-info/PKG-INFO` & `vf-flags-0.2.4/vf_flags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-flags
-Version: 0.2.3
+Version: 0.2.4
 Summary: A wrapper for easily making bitwise flags.
 Author-email: Kae Bartlett <kae@voxelfox.co.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `vf-flags-0.2.3/vfflags/__init__.py` & `vf-flags-0.2.4/vfflags/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
         self.value = value
         for i, o in kwargs.items():
             setattr(self, i, o)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(0b{self.value:_b})"
 
+    def __hash__(self) -> int:
+        return hash(repr(self))
+
     def walk(self) -> Generator[tuple[str, bool], None, None]:
         """
         Walk through the names and values of the flags.
         """
 
         for name in self.VALID_FLAGS:
             val: bool = getattr(self, name)
```

