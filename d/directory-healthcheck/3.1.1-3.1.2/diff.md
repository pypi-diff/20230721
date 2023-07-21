# Comparing `tmp/directory_healthcheck-3.1.1-py3-none-any.whl.zip` & `tmp/directory_healthcheck-3.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5620 bytes, number of entries: 10
--rw-r--r--  2.0 unx       68 b- defN 23-May-24 14:05 directory_healthcheck/__init__.py
--rw-r--r--  2.0 unx      324 b- defN 23-May-24 14:05 directory_healthcheck/apps.py
--rw-r--r--  2.0 unx     2244 b- defN 23-May-24 14:05 directory_healthcheck/backends.py
--rw-r--r--  2.0 unx     1176 b- defN 23-May-24 14:05 directory_healthcheck/views.py
--rw-r--r--  2.0 unx      339 b- defN 23-May-24 14:05 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
--rw-r--r--  2.0 unx     1091 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4074 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      932 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/RECORD
-10 files, 10362 bytes uncompressed, 3990 bytes compressed:  61.5%
+Zip file size: 5615 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-21 08:41 directory_healthcheck/__init__.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Jul-21 08:41 directory_healthcheck/apps.py
+-rw-r--r--  2.0 unx     2244 b- defN 23-Jul-21 08:41 directory_healthcheck/backends.py
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jul-21 08:41 directory_healthcheck/views.py
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-21 08:41 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
+-rw-r--r--  2.0 unx     1091 b- defN 23-Jul-21 08:41 directory_healthcheck-3.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4054 b- defN 23-Jul-21 08:41 directory_healthcheck-3.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 08:41 directory_healthcheck-3.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-21 08:41 directory_healthcheck-3.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jul-21 08:41 directory_healthcheck-3.1.2.dist-info/RECORD
+10 files, 10342 bytes uncompressed, 3985 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_healthcheck/views.py
 Comment: 
 
 Filename: directory_healthcheck/templates/directory_healthcheck/healthcheck.html
 Comment: 
 
-Filename: directory_healthcheck-3.1.1.dist-info/LICENSE
+Filename: directory_healthcheck-3.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: directory_healthcheck-3.1.1.dist-info/METADATA
+Filename: directory_healthcheck-3.1.2.dist-info/METADATA
 Comment: 
 
-Filename: directory_healthcheck-3.1.1.dist-info/WHEEL
+Filename: directory_healthcheck-3.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: directory_healthcheck-3.1.1.dist-info/top_level.txt
+Filename: directory_healthcheck-3.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_healthcheck-3.1.1.dist-info/RECORD
+Filename: directory_healthcheck-3.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_healthcheck-3.1.1.dist-info/LICENSE` & `directory_healthcheck-3.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_healthcheck-3.1.1.dist-info/METADATA` & `directory_healthcheck-3.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-healthcheck
-Version: 3.1.1
+Version: 3.1.2
 Summary: Library to streamline healthchecks for Directory apps.
 Home-page: https://github.com/uktrade/directory-healthcheck
 Author: Department for International Trade
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,30 +20,30 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django-health-check (==3.17.0)
-Requires-Dist: django (<=4.1.9,>=3.2.18)
+Requires-Dist: django (<4.2,>=4.1.10)
 Provides-Extra: test
 Requires-Dist: pytest (==3.10.0) ; extra == 'test'
 Requires-Dist: pytest-cov (==2.7.1) ; extra == 'test'
 Requires-Dist: pytest-django (==3.5.0) ; extra == 'test'
 Requires-Dist: flake8 (==5.0.4) ; extra == 'test'
 Requires-Dist: codecov (>=2.0.16) ; extra == 'test'
 Requires-Dist: twine (<=4.0.2,>=1.11.0) ; extra == 'test'
 Requires-Dist: wheel (<1.0.0,>=0.31.0) ; extra == 'test'
 Requires-Dist: raven (==5.19.0) ; extra == 'test'
 Requires-Dist: setuptools (<66.1.0,>=59.6.0) ; extra == 'test'
 Requires-Dist: directory-sso-api-client ; extra == 'test'
 Requires-Dist: directory-api-client ; extra == 'test'
 Requires-Dist: directory-forms-api-client ; extra == 'test'
 Requires-Dist: directory-cms-client ; extra == 'test'
-Requires-Dist: directory-client-core (<7.1.0,>=4.3.0) ; extra == 'test'
+Requires-Dist: directory-client-core ; extra == 'test'
 
 # directory-healthcheck
 
 [![code-climate-image]][code-climate]
 [![circle-ci-image]][circle-ci]
 [![codecov-image]][codecov]
 [![pypi-image]][pypi]
```

## Comparing `directory_healthcheck-3.1.1.dist-info/RECORD` & `directory_healthcheck-3.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_healthcheck/__init__.py,sha256=MzxjIY-3JI1bs39tYXgNHjZdG8srfCVhLqfzp4nHh_U,68
 directory_healthcheck/apps.py,sha256=0YlRHNWpSolt1BeQ7kWG1IFauQ54GH-694hg26sQ4Bw,324
 directory_healthcheck/backends.py,sha256=-UOn5GJsRcuBAuqEWfPRnKpKIygqoDiEg68FvzIY0-Q,2244
 directory_healthcheck/views.py,sha256=Lz2XsOm2698urVIJuCi7rCwRCc67FtZszgRGQY47-C0,1176
 directory_healthcheck/templates/directory_healthcheck/healthcheck.html,sha256=Na6eXAmCvfSUOG1IEEIUn4UbhkkUJpbKLlamkZQrRBg,339
-directory_healthcheck-3.1.1.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
-directory_healthcheck-3.1.1.dist-info/METADATA,sha256=zhIf16meltt43XaiPhSs3xGH2Sr23LehvfUbXrsnvkI,4074
-directory_healthcheck-3.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-directory_healthcheck-3.1.1.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
-directory_healthcheck-3.1.1.dist-info/RECORD,,
+directory_healthcheck-3.1.2.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
+directory_healthcheck-3.1.2.dist-info/METADATA,sha256=coBncAqRwUJcTwAepcgM3loRS07ekFoOTgcNuFAMkzY,4054
+directory_healthcheck-3.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_healthcheck-3.1.2.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
+directory_healthcheck-3.1.2.dist-info/RECORD,,
```

