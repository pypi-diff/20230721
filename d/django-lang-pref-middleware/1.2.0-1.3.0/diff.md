# Comparing `tmp/django-lang-pref-middleware-1.2.0.tar.gz` & `tmp/django-lang-pref-middleware-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lang-pref-middleware-1.2.0.tar", last modified: Wed Jan 26 14:46:27 2022, max compression
+gzip compressed data, was "django-lang-pref-middleware-1.3.0.tar", last modified: Fri Jul 21 13:41:03 2023, max compression
```

## Comparing `django-lang-pref-middleware-1.2.0.tar` & `django-lang-pref-middleware-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-01-26 14:46:27.000000 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-01-26 14:46:27.000000 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 14:46:27.000000 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-26 14:46:27.000000 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-26 14:46:27.000000 django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/lang_pref_middleware/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/lang_pref_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/lang_pref_middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/lang_pref_middleware/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-01-26 14:46:27.582984 django-lang-pref-middleware-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-01-26 14:46:22.000000 django-lang-pref-middleware-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:41:03.209295 django-lang-pref-middleware-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-21 13:41:03.209295 django-lang-pref-middleware-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:41:03.205295 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-21 13:41:03.000000 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-21 13:41:03.000000 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 13:41:03.000000 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-21 13:41:03.000000 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-21 13:41:03.000000 django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:41:03.205295 django-lang-pref-middleware-1.3.0/lang_pref_middleware/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/lang_pref_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/lang_pref_middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/lang_pref_middleware/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:41:03.209295 django-lang-pref-middleware-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-21 13:41:03.209295 django-lang-pref-middleware-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4615 2023-07-21 13:40:56.000000 django-lang-pref-middleware-1.3.0/setup.py
```

### Comparing `django-lang-pref-middleware-1.2.0/LICENSE.txt` & `django-lang-pref-middleware-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-lang-pref-middleware-1.2.0/NOTICE.txt` & `django-lang-pref-middleware-1.3.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `django-lang-pref-middleware-1.2.0/PKG-INFO` & `django-lang-pref-middleware-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: django-lang-pref-middleware
-Version: 1.2.0
+Version: 1.3.0
 Summary: Django middleware for setting the user's language preference at request time.
-Home-page: https://github.com/edx/django-lang-pref-middleware
+Home-page: https://github.com/openedx/django-lang-pref-middleware
 Author: edX
 Author-email: oscm@edx.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS
 
 Django Language Preference Middleware
@@ -42,12 +41,10 @@
 
 How to Contribute
 -----------------
 
 Contributions are very welcome, but for legal reasons, you must submit a signed
 [individual contributor's agreement](http://code.edx.org/individual-contributor-agreement.pdf)
 before we can accept your contribution. See our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
-
-
```

### Comparing `django-lang-pref-middleware-1.2.0/README.md` & `django-lang-pref-middleware-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 
 How to Contribute
 -----------------
 
 Contributions are very welcome, but for legal reasons, you must submit a signed
 [individual contributor's agreement](http://code.edx.org/individual-contributor-agreement.pdf)
 before we can accept your contribution. See our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
```

### Comparing `django-lang-pref-middleware-1.2.0/django_lang_pref_middleware.egg-info/PKG-INFO` & `django-lang-pref-middleware-1.3.0/django_lang_pref_middleware.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: django-lang-pref-middleware
-Version: 1.2.0
+Version: 1.3.0
 Summary: Django middleware for setting the user's language preference at request time.
-Home-page: https://github.com/edx/django-lang-pref-middleware
+Home-page: https://github.com/openedx/django-lang-pref-middleware
 Author: edX
 Author-email: oscm@edx.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS
 
 Django Language Preference Middleware
@@ -42,12 +41,10 @@
 
 How to Contribute
 -----------------
 
 Contributions are very welcome, but for legal reasons, you must submit a signed
 [individual contributor's agreement](http://code.edx.org/individual-contributor-agreement.pdf)
 before we can accept your contribution. See our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
-
-
```

### Comparing `django-lang-pref-middleware-1.2.0/lang_pref_middleware/middleware.py` & `django-lang-pref-middleware-1.3.0/lang_pref_middleware/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=missing-module-docstring
 from django.utils.deprecation import MiddlewareMixin
 
 
 class LanguagePreferenceMiddleware(MiddlewareMixin):
     """
     Middleware for user language preference.
```

### Comparing `django-lang-pref-middleware-1.2.0/lang_pref_middleware/tests.py` & `django-lang-pref-middleware-1.3.0/lang_pref_middleware/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+# pylint: disable=missing-module-docstring
 import uuid
+from unittest.mock import Mock
+
+from django.contrib.auth.models import User  # pylint: disable=imported-auth-user
+from django.contrib.sessions.middleware import SessionMiddleware
 from django.test import TestCase
 from django.test.client import RequestFactory
-from django.contrib.auth.models import User
-from django.contrib.sessions.middleware import SessionMiddleware
+
 from lang_pref_middleware.middleware import LanguagePreferenceMiddleware
 
 
-class LangPrefMiddlewareTestCaseMixin():
+class LangPrefMiddlewareTestCaseMixin():  # pylint: disable=missing-class-docstring
     middleware_class = None
 
     def setUp(self):
         # pylint: disable=not-callable
-        self.middleware = self.middleware_class()
-        self.session_middleware = SessionMiddleware()  # pylint: disable=no-value-for-parameter
+        self.mock_response = Mock()
+        self.middleware = self.middleware_class(self.mock_response)
+        self.session_middleware = SessionMiddleware(self.mock_response)
         self.user = self.get_user()
         self.request = RequestFactory().get('/somewhere')
         self.request.user = self.user
         self.session_middleware.process_request(self.request)
 
     def get_user(self):
         raise NotImplementedError
@@ -57,23 +62,23 @@
 class DummyLanguagePreferenceMiddleware(LanguagePreferenceMiddleware):
     """
     Simplified implementation of LanguagePreferenceMiddleware.
 
     This should not be used for any purpose outside of testing.
     """
 
-    def __init__(self):
+    def __init__(self, get_response):
         self._cache = {}
-        super().__init__()  # pylint: disable=no-value-for-parameter
+        super().__init__(get_response)
 
     def get_user_language_preference(self, user):
         return self._cache.get(user, None)
 
 
-class LangPrefMiddlewareTests(LangPrefMiddlewareTestCaseMixin, TestCase):
+class LangPrefMiddlewareTests(LangPrefMiddlewareTestCaseMixin, TestCase):  # pylint: disable=missing-class-docstring
     middleware_class = DummyLanguagePreferenceMiddleware
 
     def get_user(self):
         username = uuid.uuid4().hex[0:20]
         return User.objects.create_user(username)
 
     def set_user_language_preference(self, user, language):
```

### Comparing `django-lang-pref-middleware-1.2.0/requirements/constraints.txt` & `django-lang-pref-middleware-1.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `django-lang-pref-middleware-1.2.0/setup.py` & `django-lang-pref-middleware-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,22 @@
 
 setup(
     name='django-lang-pref-middleware',
     version=VERSION,
     packages=['lang_pref_middleware'],
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/django-lang-pref-middleware',
+    url='https://github.com/openedx/django-lang-pref-middleware',
     description="Django middleware for setting the user's language preference at request time.",
     long_description=open('README.md').read(),
     install_requires=load_requirements('requirements/base.in'),
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ]
 )
```

