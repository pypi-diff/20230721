# Comparing `tmp/pz7z8-0.1.2.tar.gz` & `tmp/pz7z8-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz7z8-0.1.2.tar", last modified: Sat Jun 10 08:44:48 2023, max compression
+gzip compressed data, was "pz7z8-0.1.3.tar", last modified: Fri Jul 21 06:17:32 2023, max compression
```

## Comparing `pz7z8-0.1.2.tar` & `pz7z8-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/
--rwxrwxrwx   0 root         (0) root         (0)     1074 2022-03-26 03:22:28.000000 pz7z8-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-10 08:44:48.000000 pz7z8-0.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       26 2022-03-26 03:24:29.000000 pz7z8-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/pz7z8.egg-info/
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-26 04:05:10.000000 pz7z8-0.1.2/pz7z8.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 08:44:48.000000 pz7z8-0.1.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2081 2023-06-10 08:43:46.000000 pz7z8-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/z7z8/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 pz7z8-0.1.2/z7z8/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      544 2022-06-18 09:08:51.000000 pz7z8-0.1.2/z7z8/dfslow.py
--rwxrwxrwx   0 root         (0) root         (0)     1205 2022-04-11 03:00:33.000000 pz7z8-0.1.2/z7z8/dsync.py
--rwxrw-rw-   0 root         (0) root         (0)      683 2023-06-10 08:40:49.000000 pz7z8-0.1.2/z7z8/md2pdf.py
--rwxrw-rw-   0 root         (0) root         (0)     2830 2021-12-14 03:02:47.000000 pz7z8-0.1.2/z7z8/smod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 06:17:32.000000 pz7z8-0.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1074 2022-03-26 03:22:28.000000 pz7z8-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-21 06:17:32.000000 pz7z8-0.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       26 2022-03-26 03:24:29.000000 pz7z8-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-26 04:05:10.000000 pz7z8-0.1.3/pz7z8.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-21 06:17:31.000000 pz7z8-0.1.3/pz7z8.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 06:17:32.000000 pz7z8-0.1.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2081 2023-06-10 08:44:52.000000 pz7z8-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 06:17:32.000000 pz7z8-0.1.3/z7z8/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 pz7z8-0.1.3/z7z8/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      544 2022-06-18 09:08:51.000000 pz7z8-0.1.3/z7z8/dfslow.py
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2023-07-21 06:16:39.000000 pz7z8-0.1.3/z7z8/dsync.py
+-rwxrwxrwx   0 root         (0) root         (0)      683 2023-06-10 08:40:49.000000 pz7z8-0.1.3/z7z8/md2pdf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2830 2021-12-14 03:02:47.000000 pz7z8-0.1.3/z7z8/smod.py
```

### Comparing `pz7z8-0.1.2/LICENSE` & `pz7z8-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz7z8-0.1.2/setup.py` & `pz7z8-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     i=bytes(i,encoding="utf8")
             f.write(i)
         f.close()
         shutil.copy2("setup.py2","setup.py")
 
 setuptools.setup(
     name="pz7z8",
-    version="0.1.2",
+    version="0.1.3",
     author="Chen chuan",
     author_email="kcchen@139.com",
     description="一些杂乱的小工具集",
     long_description=long_description,
     long_description_content_type="text/markdown",
 #   url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `pz7z8-0.1.2/z7z8/dfslow.py` & `pz7z8-0.1.3/z7z8/dfslow.py`

 * *Files identical despite different names*

### Comparing `pz7z8-0.1.2/z7z8/md2pdf.py` & `pz7z8-0.1.3/z7z8/md2pdf.py`

 * *Files identical despite different names*

### Comparing `pz7z8-0.1.2/z7z8/smod.py` & `pz7z8-0.1.3/z7z8/smod.py`

 * *Files identical despite different names*

