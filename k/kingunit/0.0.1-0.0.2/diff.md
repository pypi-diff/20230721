# Comparing `tmp/kingunit-0.0.1.tar.gz` & `tmp/kingunit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-t1165f3y/kingunit-0.0.1.tar", last modified: Fri Jul 21 00:52:13 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-f30x15rz/kingunit-0.0.2.tar", last modified: Fri Jul 21 00:53:20 2023, max compression
```

## Comparing `kingunit-0.0.1.tar` & `kingunit-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.799074 kingunit-0.0.1/
--rw-r--r--   0 jiayu      (501) staff       (20)      750 2023-07-21 00:52:13.798814 kingunit-0.0.1/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      496 2023-07-19 05:51:15.000000 kingunit-0.0.1/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.793795 kingunit-0.0.1/kingunit/
--rw-r--r--   0 jiayu      (501) staff       (20)       45 2023-07-21 00:51:02.000000 kingunit-0.0.1/kingunit/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.795641 kingunit-0.0.1/kingunit/cmd/
--rw-r--r--   0 jiayu      (501) staff       (20)       18 2023-07-19 01:25:45.000000 kingunit-0.0.1/kingunit/cmd/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.1/kingunit/cmd/cmd.py
--rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.1/kingunit/cmd/main.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.796461 kingunit-0.0.1/kingunit/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.1/kingunit/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.1/kingunit/config/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3240 2023-07-21 00:48:38.000000 kingunit-0.0.1/kingunit/generator.py
--rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-19 07:27:41.000000 kingunit-0.0.1/kingunit/init.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.797555 kingunit-0.0.1/kingunit/utils/
--rw-r--r--   0 jiayu      (501) staff       (20)       42 2023-07-18 06:09:17.000000 kingunit-0.0.1/kingunit/utils/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.1/kingunit/utils/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.1/kingunit/utils/mail.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:52:13.794873 kingunit-0.0.1/kingunit.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)      750 2023-07-21 00:52:13.000000 kingunit-0.0.1/kingunit.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      438 2023-07-21 00:52:13.000000 kingunit-0.0.1/kingunit.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-21 00:52:13.000000 kingunit-0.0.1/kingunit.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-21 00:52:13.000000 kingunit-0.0.1/kingunit.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-21 00:52:13.000000 kingunit-0.0.1/kingunit.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-21 00:51:51.000000 kingunit-0.0.1/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-21 00:52:13.799179 kingunit-0.0.1/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.446532 kingunit-0.0.2/
+-rw-r--r--   0 jiayu      (501) staff       (20)      706 2023-07-21 00:53:20.446287 kingunit-0.0.2/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      452 2023-07-21 00:53:09.000000 kingunit-0.0.2/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.441815 kingunit-0.0.2/kingunit/
+-rw-r--r--   0 jiayu      (501) staff       (20)       45 2023-07-21 00:51:02.000000 kingunit-0.0.2/kingunit/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.443951 kingunit-0.0.2/kingunit/cmd/
+-rw-r--r--   0 jiayu      (501) staff       (20)       18 2023-07-19 01:25:45.000000 kingunit-0.0.2/kingunit/cmd/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.2/kingunit/cmd/cmd.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.2/kingunit/cmd/main.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.444711 kingunit-0.0.2/kingunit/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.2/kingunit/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.2/kingunit/config/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3240 2023-07-21 00:48:38.000000 kingunit-0.0.2/kingunit/generator.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-19 07:27:41.000000 kingunit-0.0.2/kingunit/init.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.445791 kingunit-0.0.2/kingunit/utils/
+-rw-r--r--   0 jiayu      (501) staff       (20)       42 2023-07-18 06:09:17.000000 kingunit-0.0.2/kingunit/utils/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.2/kingunit/utils/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.2/kingunit/utils/mail.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 00:53:20.443122 kingunit-0.0.2/kingunit.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)      706 2023-07-21 00:53:20.000000 kingunit-0.0.2/kingunit.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      438 2023-07-21 00:53:20.000000 kingunit-0.0.2/kingunit.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-21 00:53:20.000000 kingunit-0.0.2/kingunit.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-21 00:53:20.000000 kingunit-0.0.2/kingunit.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-21 00:53:20.000000 kingunit-0.0.2/kingunit.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-21 00:53:14.000000 kingunit-0.0.2/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-21 00:53:20.446602 kingunit-0.0.2/setup.cfg
```

### Comparing `kingunit-0.0.1/PKG-INFO` & `kingunit-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.1
+Version: 0.0.2
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
@@ -26,12 +26,7 @@
 Mac:
 
 ```bash
 brew install allure
 ```
 
 
-## 运行测试
-
-```bash
-python main.py
-```
```

### Comparing `kingunit-0.0.1/kingunit/cmd/cmd.py` & `kingunit-0.0.2/kingunit/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.1/kingunit/generator.py` & `kingunit-0.0.2/kingunit/generator.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.1/kingunit/init.py` & `kingunit-0.0.2/kingunit/init.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.1/kingunit/utils/mail.py` & `kingunit-0.0.2/kingunit/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.1/kingunit.egg-info/PKG-INFO` & `kingunit-0.0.2/kingunit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.1
+Version: 0.0.2
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
@@ -26,12 +26,7 @@
 Mac:
 
 ```bash
 brew install allure
 ```
 
 
-## 运行测试
-
-```bash
-python main.py
-```
```

