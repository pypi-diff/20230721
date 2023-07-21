# Comparing `tmp/python_deploy-4.0.1-py3-none-any.whl.zip` & `tmp/python_deploy-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12622 bytes, number of entries: 16
--rw-r--r--  2.0 unx      121 b- defN 23-Jan-03 13:07 deploy/__init__.py
--rw-r--r--  2.0 unx       33 b- defN 23-Jan-03 13:07 deploy/__main__.py
--rw-r--r--  2.0 unx     8508 b- defN 23-Jan-03 13:07 deploy/deploy.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Jan-03 13:07 deploy/docker.py
--rw-r--r--  2.0 unx      497 b- defN 23-Jan-03 13:07 deploy/git.py
--rw-r--r--  2.0 unx     1665 b- defN 23-Jan-03 13:07 deploy/k8s.py
--rw-r--r--  2.0 unx      730 b- defN 23-Jan-03 13:07 deploy/schema.py
--rw-r--r--  2.0 unx    10132 b- defN 23-Jan-03 13:07 deploy/services.py
--rw-r--r--  2.0 unx     1381 b- defN 23-Jan-03 13:07 deploy/utils.py
--rwxr-xr-x  2.0 unx      206 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.data/scripts/kubernetes_use_token
--rw-r--r--  2.0 unx     1068 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7030 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1277 b- defN 23-Jan-03 13:07 python_deploy-4.0.1.dist-info/RECORD
-16 files, 33865 bytes uncompressed, 10522 bytes compressed:  68.9%
+Zip file size: 12627 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      121 b- defN 23-Jul-21 17:07 deploy/__init__.py
+-rw-r--r--  2.0 unx       33 b- defN 23-Jul-21 17:07 deploy/__main__.py
+-rw-r--r--  2.0 unx     8508 b- defN 23-Jul-21 17:07 deploy/deploy.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Jul-21 17:07 deploy/docker.py
+-rw-r--r--  2.0 unx      497 b- defN 23-Jul-21 17:07 deploy/git.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jul-21 17:07 deploy/k8s.py
+-rw-r--r--  2.0 unx      730 b- defN 23-Jul-21 17:07 deploy/schema.py
+-rw-r--r--  2.0 unx    10132 b- defN 23-Jul-21 17:07 deploy/services.py
+-rw-r--r--  2.0 unx     1381 b- defN 23-Jul-21 17:07 deploy/utils.py
+-rwxr-xr-x  2.0 unx      206 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.data/scripts/kubernetes_use_token
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7037 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1277 b- defN 23-Jul-21 17:07 python_deploy-4.0.2.dist-info/RECORD
+16 files, 33872 bytes uncompressed, 10527 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -21,29 +21,29 @@
 
 Filename: deploy/services.py
 Comment: 
 
 Filename: deploy/utils.py
 Comment: 
 
-Filename: python_deploy-4.0.1.data/scripts/kubernetes_use_token
+Filename: python_deploy-4.0.2.data/scripts/kubernetes_use_token
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/LICENSE
+Filename: python_deploy-4.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/METADATA
+Filename: python_deploy-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/WHEEL
+Filename: python_deploy-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/entry_points.txt
+Filename: python_deploy-4.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/top_level.txt
+Filename: python_deploy-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_deploy-4.0.1.dist-info/RECORD
+Filename: python_deploy-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_deploy-4.0.1.dist-info/LICENSE` & `python_deploy-4.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_deploy-4.0.1.dist-info/METADATA` & `python_deploy-4.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: python-deploy
-Version: 4.0.1
+Version: 4.0.2
 Summary: Build, push and deploy k8s services with single deploy.json file to provide common convention for multiple production services.
 Home-page: https://github.com/CERT-Polska/python-deploy
 Author: msm, psrok1
 Author-email: info@cert.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYAML (==5.4.1)
+Requires-Dist: PyYAML (<7.0.0,>=6.0.1)
 
 # deploy
 
 Build, push and deploy k8s services with single deploy.json file to provide common convention for
 multiple production services.
 
 ```
```

## Comparing `python_deploy-4.0.1.dist-info/RECORD` & `python_deploy-4.0.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 deploy/deploy.py,sha256=weyTgI7iF0Bz1bFIEoZQBS53t1yXOf7Oygb5cE6Hjic,8508
 deploy/docker.py,sha256=y8Ps6hwGXaFo6rVsZsoISukbXPi2bSJkytkAUYEpG3M,1078
 deploy/git.py,sha256=PQ-YRQ3CH0IzM1aEewr2vbT77rgCHLEIfOYJOA3_j9M,497
 deploy/k8s.py,sha256=_aSpyoFAz9Gblb9ZZ9SXFXczVI7_CX7OmPOrMQygJ3s,1665
 deploy/schema.py,sha256=nqDBnyuIk6b78If5YH5uOoNWXoziiLVOoCNp4zKykM0,730
 deploy/services.py,sha256=7yK2fYypcTyXeh-ovU1nSwuT7sVyQ60jpfH921CQCrs,10132
 deploy/utils.py,sha256=sEl-CTUrXURbQGQ2TytyJf0P9lNWBaE3jeGN1M1rIDM,1381
-python_deploy-4.0.1.data/scripts/kubernetes_use_token,sha256=bBUkGFSsRjaw0AZZej5ZSJFaljGZckNePz2_UgO5J48,206
-python_deploy-4.0.1.dist-info/LICENSE,sha256=EQpE_VUx-cRS-iZgpjBtKIjR3AS0oGiREep8yNuH7lE,1068
-python_deploy-4.0.1.dist-info/METADATA,sha256=GWfvEi3VzclBgmZFN-alG0jOzrYxtEGQ_l3YZ9Bg5jM,7030
-python_deploy-4.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-python_deploy-4.0.1.dist-info/entry_points.txt,sha256=WYsu8QH3hpMvZeZQEdHwVVGuWN9B38cSB90d7gRV3GU,40
-python_deploy-4.0.1.dist-info/top_level.txt,sha256=xvFnZzSzWjwmJ0zc3txKNOrT0LgVq20Gr9SlilW68Tw,7
-python_deploy-4.0.1.dist-info/RECORD,,
+python_deploy-4.0.2.data/scripts/kubernetes_use_token,sha256=bBUkGFSsRjaw0AZZej5ZSJFaljGZckNePz2_UgO5J48,206
+python_deploy-4.0.2.dist-info/LICENSE,sha256=EQpE_VUx-cRS-iZgpjBtKIjR3AS0oGiREep8yNuH7lE,1068
+python_deploy-4.0.2.dist-info/METADATA,sha256=8NGnOG1FwxbDpW8rP7NOvjWTsbJqHk_lQraUbdEAsqM,7037
+python_deploy-4.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+python_deploy-4.0.2.dist-info/entry_points.txt,sha256=WYsu8QH3hpMvZeZQEdHwVVGuWN9B38cSB90d7gRV3GU,40
+python_deploy-4.0.2.dist-info/top_level.txt,sha256=xvFnZzSzWjwmJ0zc3txKNOrT0LgVq20Gr9SlilW68Tw,7
+python_deploy-4.0.2.dist-info/RECORD,,
```

