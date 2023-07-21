# Comparing `tmp/dtogen-0.0.2.tar.gz` & `tmp/dtogen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtogen-0.0.2.tar", last modified: Thu Jul 20 21:35:02 2023, max compression
+gzip compressed data, was "dtogen-0.0.3.tar", last modified: Fri Jul 21 21:17:30 2023, max compression
```

## Comparing `dtogen-0.0.2.tar` & `dtogen-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-20 21:35:02.952021 dtogen-0.0.2/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-20 21:35:02.951860 dtogen-0.0.2/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.2/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-20 21:35:02.950577 dtogen-0.0.2/dtogen/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      940 2023-07-20 21:33:54.000000 dtogen-0.0.2/dtogen/__main__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1636 2023-07-20 21:12:11.000000 dtogen-0.0.2/dtogen/dtogenerator.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.2/dtogen/interfaces.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-20 21:35:02.951225 dtogen-0.0.2/dtogen.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-20 21:35:02.000000 dtogen-0.0.2/dtogen.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      250 2023-07-20 21:35:02.000000 dtogen-0.0.2/dtogen.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-20 21:35:02.000000 dtogen-0.0.2/dtogen.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2023-07-20 21:35:02.000000 dtogen-0.0.2/dtogen.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-20 21:35:02.952071 dtogen-0.0.2/setup.cfg
--rw-r--r--   0 mujdecisy   (501) staff       (20)      672 2023-07-20 21:34:45.000000 dtogen-0.0.2/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-20 21:35:02.951632 dtogen-0.0.2/test/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-20 21:12:11.000000 dtogen-0.0.2/test/test_dtogenerator.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-20 21:12:11.000000 dtogen-0.0.2/test/test_transform.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-21 21:17:30.473176 dtogen-0.0.3/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-21 21:17:30.472984 dtogen-0.0.3/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.3/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-21 21:17:30.471652 dtogen-0.0.3/dtogen/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      940 2023-07-21 21:15:24.000000 dtogen-0.0.3/dtogen/__main__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1636 2023-07-21 21:13:23.000000 dtogen-0.0.3/dtogen/dtogenerator.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.3/dtogen/interfaces.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-21 21:17:30.472339 dtogen-0.0.3/dtogen.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3099 2023-07-21 21:17:30.000000 dtogen-0.0.3/dtogen.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      250 2023-07-21 21:17:30.000000 dtogen-0.0.3/dtogen.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-21 21:17:30.000000 dtogen-0.0.3/dtogen.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2023-07-21 21:17:30.000000 dtogen-0.0.3/dtogen.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-21 21:17:30.473225 dtogen-0.0.3/setup.cfg
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      672 2023-07-21 21:16:52.000000 dtogen-0.0.3/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-21 21:17:30.472688 dtogen-0.0.3/test/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-21 21:13:23.000000 dtogen-0.0.3/test/test_dtogenerator.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-21 21:13:23.000000 dtogen-0.0.3/test/test_transform.py
```

### Comparing `dtogen-0.0.2/PKG-INFO` & `dtogen-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtogen
-Version: 0.0.2
+Version: 0.0.3
 Summary: DTO generator for Java, TypeScript, Python
 Home-page: https://github.com/mujdecisy/dtogen
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,DTO,generator
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dtogen-0.0.2/README.md` & `dtogen-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.2/dtogen/__main__.py` & `dtogen-0.0.3/dtogen/__main__.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.2/dtogen/dtogenerator.py` & `dtogen-0.0.3/dtogen/dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.2/dtogen/interfaces.py` & `dtogen-0.0.3/dtogen/interfaces.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.2/dtogen.egg-info/PKG-INFO` & `dtogen-0.0.3/dtogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtogen
-Version: 0.0.2
+Version: 0.0.3
 Summary: DTO generator for Java, TypeScript, Python
 Home-page: https://github.com/mujdecisy/dtogen
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,DTO,generator
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dtogen-0.0.2/setup.py` & `dtogen-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="dtogen",
-    version="0.0.2",
+    version="0.0.3",
     description="DTO generator for Java, TypeScript, Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/dtogen",
     keywords=["python", "DTO", "generator"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `dtogen-0.0.2/test/test_dtogenerator.py` & `dtogen-0.0.3/test/test_dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.2/test/test_transform.py` & `dtogen-0.0.3/test/test_transform.py`

 * *Files identical despite different names*

