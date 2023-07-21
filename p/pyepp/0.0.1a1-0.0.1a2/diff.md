# Comparing `tmp/pyepp-0.0.1a1.tar.gz` & `tmp/pyepp-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepp-0.0.1a1.tar", last modified: Fri Jul 21 00:20:43 2023, max compression
+gzip compressed data, was "pyepp-0.0.1a2.tar", last modified: Fri Jul 21 03:53:32 2023, max compression
```

## Comparing `pyepp-0.0.1a1.tar` & `pyepp-0.0.1a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ehsan      (501) staff       (20)        0 2023-07-21 00:20:43.364024 pyepp-0.0.1a1/
--rw-r--r--   0 ehsan      (501) staff       (20)    35149 2023-03-15 20:40:56.000000 pyepp-0.0.1a1/LICENSE
--rw-r--r--   0 ehsan      (501) staff       (20)     3835 2023-07-21 00:20:43.363848 pyepp-0.0.1a1/PKG-INFO
--rw-r--r--   0 ehsan      (501) staff       (20)     3323 2023-07-21 00:05:44.000000 pyepp-0.0.1a1/README.md
-drwxr-xr-x   0 ehsan      (501) staff       (20)        0 2023-07-21 00:20:43.361168 pyepp-0.0.1a1/pyepp/
--rw-r--r--   0 ehsan      (501) staff       (20)      110 2023-07-21 00:20:04.000000 pyepp-0.0.1a1/pyepp/__init__.py
--rw-r--r--   0 ehsan      (501) staff       (20)     3518 2023-06-15 02:29:29.000000 pyepp-0.0.1a1/pyepp/base_command.py
--rw-r--r--   0 ehsan      (501) staff       (20)    16036 2023-07-19 03:14:52.000000 pyepp-0.0.1a1/pyepp/command_templates.py
--rw-r--r--   0 ehsan      (501) staff       (20)     6800 2023-05-09 22:11:36.000000 pyepp-0.0.1a1/pyepp/contact.py
--rw-r--r--   0 ehsan      (501) staff       (20)    11670 2023-06-21 22:16:40.000000 pyepp-0.0.1a1/pyepp/domain.py
--rw-r--r--   0 ehsan      (501) staff       (20)     8951 2023-05-02 23:04:33.000000 pyepp-0.0.1a1/pyepp/epp.py
--rw-r--r--   0 ehsan      (501) staff       (20)      355 2023-04-28 01:55:58.000000 pyepp-0.0.1a1/pyepp/helper.py
--rw-r--r--   0 ehsan      (501) staff       (20)     5631 2023-07-19 03:14:52.000000 pyepp-0.0.1a1/pyepp/host.py
-drwxr-xr-x   0 ehsan      (501) staff       (20)        0 2023-07-21 00:20:43.361962 pyepp-0.0.1a1/pyepp.egg-info/
--rw-r--r--   0 ehsan      (501) staff       (20)     3835 2023-07-21 00:20:43.000000 pyepp-0.0.1a1/pyepp.egg-info/PKG-INFO
--rw-r--r--   0 ehsan      (501) staff       (20)      449 2023-07-21 00:20:43.000000 pyepp-0.0.1a1/pyepp.egg-info/SOURCES.txt
--rw-r--r--   0 ehsan      (501) staff       (20)        1 2023-07-21 00:20:43.000000 pyepp-0.0.1a1/pyepp.egg-info/dependency_links.txt
--rw-r--r--   0 ehsan      (501) staff       (20)       81 2023-07-21 00:20:43.000000 pyepp-0.0.1a1/pyepp.egg-info/requires.txt
--rw-r--r--   0 ehsan      (501) staff       (20)        6 2023-07-21 00:20:43.000000 pyepp-0.0.1a1/pyepp.egg-info/top_level.txt
--rw-r--r--   0 ehsan      (501) staff       (20)      837 2023-07-20 22:03:10.000000 pyepp-0.0.1a1/pyproject.toml
--rw-r--r--   0 ehsan      (501) staff       (20)       38 2023-07-21 00:20:43.364065 pyepp-0.0.1a1/setup.cfg
-drwxr-xr-x   0 ehsan      (501) staff       (20)        0 2023-07-21 00:20:43.363647 pyepp-0.0.1a1/tests/
--rw-r--r--   0 ehsan      (501) staff       (20)     5726 2023-05-02 23:04:33.000000 pyepp-0.0.1a1/tests/test_base_command.py
--rw-r--r--   0 ehsan      (501) staff       (20)    16944 2023-05-02 23:04:33.000000 pyepp-0.0.1a1/tests/test_contact.py
--rw-r--r--   0 ehsan      (501) staff       (20)    19399 2023-06-15 02:29:29.000000 pyepp-0.0.1a1/tests/test_domain.py
--rw-r--r--   0 ehsan      (501) staff       (20)       10 2023-04-28 01:55:58.000000 pyepp-0.0.1a1/tests/test_helper.py
--rw-r--r--   0 ehsan      (501) staff       (20)    14450 2023-07-19 03:14:52.000000 pyepp-0.0.1a1/tests/test_host.py
--rw-r--r--   0 ehsan      (501) staff       (20)    10903 2023-05-02 23:04:33.000000 pyepp-0.0.1a1/tests/test_pyepp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/pyepp/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/command_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/epp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyepp/host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/pyepp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-21 03:53:32.000000 pyepp-0.0.1a2/pyepp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 03:53:32.000000 pyepp-0.0.1a2/pyepp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:53:32.000000 pyepp-0.0.1a2/pyepp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 03:53:32.000000 pyepp-0.0.1a2/pyepp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 03:53:32.000000 pyepp-0.0.1a2/pyepp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:53:32.180803 pyepp-0.0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_base_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-21 03:52:54.000000 pyepp-0.0.1a2/tests/test_pyepp.py
```

### Comparing `pyepp-0.0.1a1/LICENSE` & `pyepp-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/PKG-INFO` & `pyepp-0.0.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepp
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Python API on top of the EPP protocol.
 Author-email: InternetNZ <ehsan@internetnz.net.nz>
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/InternetNZ/pyepp
 Project-URL: Repository, https://github.com/InternetNZ/pyepp
 Keywords: epp,registry
 Classifier: Programming Language :: Python
@@ -110,18 +110,26 @@
 renew_domain = domain.renew(domain_name='example-1.nz', expiry_date=date(2024, 2, 23), period=2)
 ```
 
 ## Development setup
 Clone this project. It's recommended to create virtual environment. Then install the dependencies and 
 development dependencies:
 
-```sh
+```shell
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
+Before creating any pull requests please make sure your code lints and there is no security issues in your code 
+by running below scripts:
+
+```shell
+./scripts/linter.sh
+./scripts/code-security-check.sh
+```
+
 Happy developing!
 ## Contributing
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md)
 
 <!-- Markdown link & img dfn's -->
 [wiki]: https://github.com/internetnz/pyepp/wiki
```

### Comparing `pyepp-0.0.1a1/README.md` & `pyepp-0.0.1a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -94,18 +94,26 @@
 renew_domain = domain.renew(domain_name='example-1.nz', expiry_date=date(2024, 2, 23), period=2)
 ```
 
 ## Development setup
 Clone this project. It's recommended to create virtual environment. Then install the dependencies and 
 development dependencies:
 
-```sh
+```shell
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
+Before creating any pull requests please make sure your code lints and there is no security issues in your code 
+by running below scripts:
+
+```shell
+./scripts/linter.sh
+./scripts/code-security-check.sh
+```
+
 Happy developing!
 ## Contributing
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md)
 
 <!-- Markdown link & img dfn's -->
 [wiki]: https://github.com/internetnz/pyepp/wiki
```

### Comparing `pyepp-0.0.1a1/pyepp/base_command.py` & `pyepp-0.0.1a2/pyepp/base_command.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp/command_templates.py` & `pyepp-0.0.1a2/pyepp/command_templates.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp/contact.py` & `pyepp-0.0.1a2/pyepp/contact.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp/domain.py` & `pyepp-0.0.1a2/pyepp/domain.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp/epp.py` & `pyepp-0.0.1a2/pyepp/epp.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp/host.py` & `pyepp-0.0.1a2/pyepp/host.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/pyepp.egg-info/PKG-INFO` & `pyepp-0.0.1a2/pyepp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepp
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Python API on top of the EPP protocol.
 Author-email: InternetNZ <ehsan@internetnz.net.nz>
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/InternetNZ/pyepp
 Project-URL: Repository, https://github.com/InternetNZ/pyepp
 Keywords: epp,registry
 Classifier: Programming Language :: Python
@@ -110,18 +110,26 @@
 renew_domain = domain.renew(domain_name='example-1.nz', expiry_date=date(2024, 2, 23), period=2)
 ```
 
 ## Development setup
 Clone this project. It's recommended to create virtual environment. Then install the dependencies and 
 development dependencies:
 
-```sh
+```shell
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
+Before creating any pull requests please make sure your code lints and there is no security issues in your code 
+by running below scripts:
+
+```shell
+./scripts/linter.sh
+./scripts/code-security-check.sh
+```
+
 Happy developing!
 ## Contributing
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md)
 
 <!-- Markdown link & img dfn's -->
 [wiki]: https://github.com/internetnz/pyepp/wiki
```

### Comparing `pyepp-0.0.1a1/pyproject.toml` & `pyepp-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/tests/test_base_command.py` & `pyepp-0.0.1a2/tests/test_base_command.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/tests/test_contact.py` & `pyepp-0.0.1a2/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/tests/test_domain.py` & `pyepp-0.0.1a2/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/tests/test_host.py` & `pyepp-0.0.1a2/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.1a1/tests/test_pyepp.py` & `pyepp-0.0.1a2/tests/test_pyepp.py`

 * *Files identical despite different names*

