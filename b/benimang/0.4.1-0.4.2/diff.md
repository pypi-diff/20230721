# Comparing `tmp/benimang-0.4.1.tar.gz` & `tmp/benimang-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.1.tar", last modified: Thu Jul 20 10:06:22 2023, max compression
+gzip compressed data, was "benimang-0.4.2.tar", last modified: Fri Jul 21 01:41:29 2023, max compression
```

## Comparing `benimang-0.4.1.tar` & `benimang-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.879927 benimang-0.4.1/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-20 10:06:22.879927 benimang-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.873926 benimang-0.4.1/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.1/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.1/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.1/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.1/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.1/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.1/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.1/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/btable.py
--rw-rw-rw-   0        0        0     4819 2023-07-20 09:58:58.000000 benimang-0.4.1/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.1/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.1/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.1/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.876926 benimang-0.4.1/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-20 10:06:22.000000 benimang-0.4.1/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-20 10:05:44.000000 benimang-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 10:06:22.879927 benimang-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 10:06:22.877926 benimang-0.4.1/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.1/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.180384 benimang-0.4.2/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-21 01:41:29.179382 benimang-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.173381 benimang-0.4.2/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.2/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.2/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.2/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.2/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.2/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.2/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.2/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/btable.py
+-rw-rw-rw-   0        0        0     4871 2023-07-21 01:29:06.000000 benimang-0.4.2/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.2/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.177382 benimang-0.4.2/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-21 01:31:52.000000 benimang-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 01:41:29.180384 benimang-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.178382 benimang-0.4.2/test/
+-rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.2/test/test_sample.py
```

### Comparing `benimang-0.4.1/beni/bbyte.py` & `benimang-0.4.2/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bcache.py` & `benimang-0.4.2/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bcolor.py` & `benimang-0.4.2/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bexecute.py` & `benimang-0.4.2/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bfile.py` & `benimang-0.4.2/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bfunc.py` & `benimang-0.4.2/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bhttp.py` & `benimang-0.4.2/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/binput.py` & `benimang-0.4.2/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/block.py` & `benimang-0.4.2/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/blog.py` & `benimang-0.4.2/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bpath.py` & `benimang-0.4.2/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bplaywright.py` & `benimang-0.4.2/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bprogress.py` & `benimang-0.4.2/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bqiniu.py` & `benimang-0.4.2/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bsqlite.py` & `benimang-0.4.2/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bstorage.py` & `benimang-0.4.2/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/btable.py` & `benimang-0.4.2/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/btask.py` & `benimang-0.4.2/beni/btask.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,17 @@
                 files = tasksDir.glob('*.py')
                 files = filter(lambda x: not x.name.startswith('_'), files)
                 for moduleName in [x.stem for x in files]:
                     exec(f'import {_TASKS}.{moduleName}')
                     module = eval(f'{_TASKS}.{moduleName}')
                     if hasattr(module, 'app'):
                         sub: Typer = getattr(module, 'app')
-                        sub.info.name = moduleName.replace('_', '-')
-                        app.add_typer(sub, name=sub.info.name)
+                        if sub is not app:
+                            sub.info.name = moduleName.replace('_', '-')
+                            app.add_typer(sub, name=sub.info.name)
                 app()
             except BaseException as ex:
                 if type(ex) is SystemExit and ex.code in (0, 2):
                     # 0 - 正常结束
                     # 2 - Error: Missing command.
                     pass
                 else:
```

### Comparing `benimang-0.4.1/beni/btime.py` & `benimang-0.4.2/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/beni/bzip.py` & `benimang-0.4.2/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/benimang.egg-info/SOURCES.txt` & `benimang-0.4.2/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.4.1/test/test_sample.py` & `benimang-0.4.2/test/test_sample.py`

 * *Files identical despite different names*

