# Comparing `tmp/mwj-apitest-1.0.1.tar.gz` & `tmp/mwj-apitest-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwj-apitest-1.0.1.tar", last modified: Wed May 31 11:12:34 2023, max compression
+gzip compressed data, was "mwj-apitest-1.1.1.tar", last modified: Fri Jul 21 09:38:18 2023, max compression
```

## Comparing `mwj-apitest-1.0.1.tar` & `mwj-apitest-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.726054 mwj-apitest-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      565 2023-05-31 11:12:34.725079 mwj-apitest-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-05-31 11:03:33.000000 mwj-apitest-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.715319 mwj-apitest-1.0.1/mwjApiTest/
--rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.0.1/mwjApiTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.716295 mwj-apitest-1.0.1/mwjApiTest/core/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.1/mwjApiTest/core/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-05-31 11:08:47.000000 mwj-apitest-1.0.1/mwjApiTest/manage.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.716295 mwj-apitest-1.0.1/mwjApiTest/utils/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.0.1/mwjApiTest/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:12:34.724103 mwj-apitest-1.0.1/mwj_apitest.egg-info/
--rw-rw-rw-   0        0        0      565 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 11:12:34.000000 mwj-apitest-1.0.1/mwj_apitest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 11:12:34.726054 mwj-apitest-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1482 2023-05-31 11:08:47.000000 mwj-apitest-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.029827 mwj-apitest-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-31 08:08:20.000000 mwj-apitest-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      969 2023-07-21 09:38:18.029827 mwj-apitest-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-21 08:25:51.000000 mwj-apitest-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:17.999177 mwj-apitest-1.1.1/mwjApiTest/
+-rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.1.1/mwjApiTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.009880 mwj-apitest-1.1.1/mwjApiTest/core/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.1/mwjApiTest/core/__init__.py
+-rw-rw-rw-   0        0        0     6001 2023-07-13 09:21:04.000000 mwj-apitest-1.1.1/mwjApiTest/core/basecase.py
+-rw-rw-rw-   0        0        0     5378 2023-07-12 09:40:57.000000 mwj-apitest-1.1.1/mwjApiTest/core/dataParser.py
+-rw-rw-rw-   0        0        0     1456 2023-07-10 08:19:16.000000 mwj-apitest-1.1.1/mwjApiTest/core/db_client.py
+-rw-rw-rw-   0        0        0     2559 2023-07-13 10:24:23.000000 mwj-apitest-1.1.1/mwjApiTest/core/env_prepare.py
+-rw-rw-rw-   0        0        0     3350 2023-07-14 08:08:04.000000 mwj-apitest-1.1.1/mwjApiTest/core/generateCase.py
+-rw-rw-rw-   0        0        0    22073 2023-07-21 09:16:40.000000 mwj-apitest-1.1.1/mwjApiTest/core/httptest.py
+-rw-rw-rw-   0        0        0     3653 2023-07-10 08:09:42.000000 mwj-apitest-1.1.1/mwjApiTest/core/log_operation.py
+-rw-rw-rw-   0        0        0     2117 2023-07-10 08:36:03.000000 mwj-apitest-1.1.1/mwjApiTest/core/make_data.py
+-rw-rw-rw-   0        0        0     6781 2023-07-11 03:09:03.000000 mwj-apitest-1.1.1/mwjApiTest/core/send_report.py
+-rw-rw-rw-   0        0        0    20285 2023-07-21 08:28:06.000000 mwj-apitest-1.1.1/mwjApiTest/core/testRunner.py
+-rw-rw-rw-   0        0        0     6743 2023-07-21 09:37:28.000000 mwj-apitest-1.1.1/mwjApiTest/manage.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.009880 mwj-apitest-1.1.1/mwjApiTest/templates/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.1/mwjApiTest/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.010877 mwj-apitest-1.1.1/mwjApiTest/templates/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.1.1/mwjApiTest/templates/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.013870 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/
+-rw-rw-rw-   0        0        0      190 2023-07-19 10:08:25.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.014867 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_json/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.016862 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_py/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_py/__init__.py
+-rw-rw-rw-   0        0        0     1232 2023-07-21 08:08:11.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.016862 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_yaml/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-07-14 06:35:52.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/funcTools.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.018856 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/logs/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/logs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.019854 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:28.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/reports/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-07-14 08:23:35.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/run.py
+-rw-rw-rw-   0        0        0     2117 2023-07-21 09:08:28.000000 mwj-apitest-1.1.1/mwjApiTest/templates/request_file_demo/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.020851 mwj-apitest-1.1.1/mwjApiTest/utils/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.1.1/mwjApiTest/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:38:18.028830 mwj-apitest-1.1.1/mwj_apitest.egg-info/
+-rw-rw-rw-   0        0        0      969 2023-07-21 09:38:17.000000 mwj-apitest-1.1.1/mwj_apitest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2023-07-21 09:38:17.000000 mwj-apitest-1.1.1/mwj_apitest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:38:17.000000 mwj-apitest-1.1.1/mwj_apitest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-21 09:38:17.000000 mwj-apitest-1.1.1/mwj_apitest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 09:38:17.000000 mwj-apitest-1.1.1/mwj_apitest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:38:18.030825 mwj-apitest-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-21 09:37:28.000000 mwj-apitest-1.1.1/setup.py
```

### Comparing `mwj-apitest-1.0.1/LICENSE` & `mwj-apitest-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.0.1/setup.py` & `mwj-apitest-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwj-apitest",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.1",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
+    version="1.1.1",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
     author="梦无矶小仔",  # 作者，可以写自己的姓名
     author_email="Lvan826199@163.com",  # 作者联系方式，可写自己的邮箱地址
-    description="A small example package",  # 包的简述
+    description="An execution engine for the interface automation platform",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Lvan826199/mwjApiTest",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     entry_points={
-        "console_scripts" : ['mwjApiTest = mwjApiTest.manage:main']
-    }, #安装成功后，在命令行输入mwjApiTest 就相当于执行了mwjApiTest.manage.py中的main了
+        "console_scripts": ['mwj = mwjApiTest.manage:main']
+    },  # 安装成功后，在命令行输入mwj 就相当于执行了mwjApiTest.manage.py中的main了
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',  # 对python的最低版本要求
 )
-
```

