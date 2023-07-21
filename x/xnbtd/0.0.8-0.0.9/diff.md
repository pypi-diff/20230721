# Comparing `tmp/xnbtd-0.0.8.tar.gz` & `tmp/xnbtd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.8.tar", max compression
+gzip compressed data, was "xnbtd-0.0.9.tar", max compression
```

## Comparing `xnbtd-0.0.8.tar` & `xnbtd-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.8/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.8/README.md
--rwxr-xr-x   0        0        0     3622 2023-07-19 05:18:50.555078 xnbtd-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.8/xnbtd/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.8/xnbtd/administration/__init__.py
--rwxr-xr-x   0        0        0      279 2023-07-18 16:22:18.242992 xnbtd-0.0.8/xnbtd/administration/admin.py
--rwxr-xr-x   0        0        0      157 2023-07-18 16:28:05.569856 xnbtd-0.0.8/xnbtd/administration/apps.py
--rwxr-xr-x   0        0        0     1656 2023-07-19 05:07:41.241082 xnbtd-0.0.8/xnbtd/administration/templates/xnbtd/admin/index.html
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.8/xnbtd/asgi.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.8/xnbtd/plannings/__init__.py
--rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.8/xnbtd/plannings/admin.py
--rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.8/xnbtd/plannings/apps.py
--rwxr-xr-x   0        0        0      581 2023-07-18 17:07:15.000000 xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0      953 2023-07-18 17:06:20.379672 xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.8/xnbtd/plannings/migrations/0001_initial.py
--rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.8/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
--rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.8/xnbtd/plannings/migrations/__init__.py
--rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.8/xnbtd/plannings/models.py
--rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-0.0.8/xnbtd/plannings/templatetags/events.py
--rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.8/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.8/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5654 2023-07-18 16:47:07.219908 xnbtd-0.0.8/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.8/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.8/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.8/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.8/xnbtd/tours/__init__.py
--rwxr-xr-x   0        0        0     6654 2023-07-18 15:17:40.498280 xnbtd-0.0.8/xnbtd/tours/admin.py
--rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.8/xnbtd/tours/apps.py
--rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.8/xnbtd/tours/forms.py
--rwxr-xr-x   0        0        0     3731 2023-07-18 17:07:15.000000 xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     6438 2023-07-18 17:06:20.302659 xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.8/xnbtd/tours/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.8/xnbtd/tours/migrations/__init__.py
--rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.8/xnbtd/tours/models.py
--rwxr-xr-x   0        0        0      113 2023-07-18 13:08:06.430521 xnbtd-0.0.8/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.8/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.9/README.md
+-rwxr-xr-x   0        0        0     3622 2023-07-21 21:55:24.583110 xnbtd-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      222 2023-07-21 21:52:15.409174 xnbtd-0.0.9/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      281 2023-07-20 13:58:05.853446 xnbtd-0.0.9/xnbtd/admin.py
+-rwxr-xr-x   0        0        0      288 2023-07-21 21:49:55.059033 xnbtd-0.0.9/xnbtd/apps.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.9/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0      610 2023-07-21 21:03:24.000000 xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     1080 2023-07-21 21:02:51.383951 xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      794 2023-07-21 21:52:56.078123 xnbtd-0.0.9/xnbtd/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-21 21:39:32.426120 xnbtd-0.0.9/xnbtd/migrations/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.9/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.9/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.9/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-07-21 21:03:24.000000 xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      953 2023-07-21 21:02:51.303633 xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      914 2023-07-21 21:35:35.367721 xnbtd-0.0.9/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:50.131931 xnbtd-0.0.9/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.9/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.9/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.9/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5841 2023-07-21 20:58:24.764238 xnbtd-0.0.9/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.9/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.9/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.9/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0     1391 2023-07-21 21:31:26.839640 xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/change_list.html
+-rwxr-xr-x   0        0        0     1656 2023-07-20 12:50:03.246479 xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/index.html
+-rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-0.0.9/xnbtd/templatetags/events.py
+-rwxr-xr-x   0        0        0     1383 2023-07-21 21:53:11.656492 xnbtd-0.0.9/xnbtd/templatetags/tours.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.9/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0    10206 2023-07-21 21:53:23.129533 xnbtd-0.0.9/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.9/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.9/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     4392 2023-07-21 21:03:25.000000 xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     7986 2023-07-21 21:02:51.223602 xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     8264 2023-07-21 21:35:35.397000 xnbtd-0.0.9/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:44.075539 xnbtd-0.0.9/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     7296 2023-07-21 21:53:41.456419 xnbtd-0.0.9/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      120 2023-07-21 08:12:20.934692 xnbtd-0.0.9/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.9/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.9/PKG-INFO
```

### Comparing `xnbtd-0.0.8/LICENSE` & `xnbtd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/README.md` & `xnbtd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/pyproject.toml` & `xnbtd-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.8"
+version = "0.0.9"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-0.0.8/xnbtd/administration/templates/xnbtd/admin/index.html` & `xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/index.html`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/plannings/templatetags/events.py` & `xnbtd-0.0.9/xnbtd/templatetags/events.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/publish.py` & `xnbtd-0.0.9/xnbtd/publish.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/settings/base.py` & `xnbtd-0.0.9/xnbtd/settings/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,190 +1,191 @@
-"""
-    Django Project settings
-"""
-import logging
-import os as __os
-from pathlib import Path as __Path
-
-
-ENV_TYPE = __os.environ.get('ENV_TYPE', None)
-print(f'ENV_TYPE:{ENV_TYPE!r}')
-
-
-###############################################################################
-
-# Build paths relative to the project root:
-PROJECT_PATH = __Path(__file__).resolve().parent.parent.parent
-print(f'PROJECT_PATH:{PROJECT_PATH}')
-
-# Build paths relative to the current working directory:
-BASE_PATH = __Path().cwd().resolve()
-print(f'BASE_PATH:{BASE_PATH}')
-
-# Paths with Django dev. server:
-# BASE_PATH...: .../django-for-runners
-# PROJECT_PATH: .../django-for-runners
-
-# But the paths are different, if it's installed as python package!
-
-###############################################################################
-
-LOGIN_URL = 'admin:login'
-
-###############################################################################
-
-
-# SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = False
-TEMPLATE_DEBUG = False
-
-
-# SECURITY WARNING: keep the secret key used in production secret!
-__SECRET_FILE = __Path(BASE_PATH, 'secret.txt').resolve()
-if not __SECRET_FILE.is_file():
-    print(f'Generate {__SECRET_FILE}')
-    from secrets import token_urlsafe as __token_urlsafe
-
-    __SECRET_FILE.write_text(__token_urlsafe(128))
-
-SECRET_KEY = __SECRET_FILE.read_text().strip()
-
-
-# Application definition
-
-INSTALLED_APPS = [
-    'xnbtd.administration.apps.AdministrationConfig',
-    'xnbtd.tours.apps.ToursConfig',
-    'xnbtd.plannings.apps.PlanningsConfig',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'import_export',
-]
-
-ROOT_URLCONF = 'xnbtd.urls'
-WSGI_APPLICATION = 'xnbtd.wsgi.application'
-
-
-MIDDLEWARE = [
-    "django.middleware.security.SecurityMiddleware",
-    "django.contrib.sessions.middleware.SessionMiddleware",
-    "django.middleware.common.CommonMiddleware",
-    "django.middleware.csrf.CsrfViewMiddleware",
-    "django.contrib.auth.middleware.AuthenticationMiddleware",
-    "django.contrib.messages.middleware.MessageMiddleware",
-    "django.middleware.clickjacking.XFrameOptionsMiddleware",
-    'django.middleware.locale.LocaleMiddleware',
-]
-
-TEMPLATES = [
-    {
-        "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [str(__Path(PROJECT_PATH, 'xnbtd', 'administration', 'templates'))],
-        "APP_DIRS": True,
-        "OPTIONS": {
-            "context_processors": [
-                "django.template.context_processors.debug",
-                "django.template.context_processors.request",
-                "django.contrib.auth.context_processors.auth",
-                "django.contrib.messages.context_processors.messages",
-            ],
-        },
-    },
-]
-
-USE_TZ = True
-
-# _____________________________________________________________________________
-
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
-
-# _____________________________________________________________________________
-
-# Mark CSRF cookie as "secure" -> browsers sent cookie only with an HTTPS connection:
-CSRF_COOKIE_SECURE = True
-
-# Mark session cookie as "secure" -> browsers sent cookie only with an HTTPS connection:
-SESSION_COOKIE_SECURE = True
-
-# HTTP header/value combination that signifies a request is secure
-# Your nginx.conf must set "X-Forwarded-Protocol" proxy header!
-SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTOCOL', 'https')
-
-# SecurityMiddleware should redirects all non-HTTPS requests to HTTPS:
-SECURE_SSL_REDIRECT = True
-
-# SecurityMiddleware should preload directive to the HTTP Strict Transport Security header:
-SECURE_HSTS_PRELOAD = True
-
-# Instruct modern browsers to refuse to connect to your domain name via an insecure connection:
-SECURE_HSTS_SECONDS = 3600
-
-# SecurityMiddleware should add the "includeSubDomains" directive to the Strict-Transport-Security
-# header: All subdomains of your domain should be served exclusively via SSL!
-SECURE_HSTS_INCLUDE_SUBDOMAINS = True
-
-# _____________________________________________________________________________
-# Static files (CSS, JavaScript, Images)
-
-STATIC_URL = '/static/'
-STATIC_ROOT = str(__Path(BASE_PATH, 'static'))
-
-MEDIA_URL = '/media/'
-MEDIA_ROOT = str(__Path(BASE_PATH, 'media'))
-
-# _____________________________________________________________________________
-# cut 'pathname' in log output
-
-old_factory = logging.getLogRecordFactory()
-
-
-def cut_path(pathname, max_length):
-    if len(pathname) <= max_length:
-        return pathname
-    return f'...{pathname[-(max_length - 3):]}'
-
-
-def record_factory(*args, **kwargs):
-    record = old_factory(*args, **kwargs)
-    record.cut_path = cut_path(record.pathname, 30)
-    return record
-
-
-logging.setLogRecordFactory(record_factory)
-
-# -----------------------------------------------------------------------------
-
-LOGGING = {
-    'version': 1,
-    'disable_existing_loggers': True,
-    'formatters': {
-        'verbose': {
-            'format': '%(asctime)s %(levelname)8s %(cut_path)s:%(lineno)-3s %(message)s',
-        }
-    },
-    'handlers': {'console': {'class': 'logging.StreamHandler', 'formatter': 'verbose'}},
-    'loggers': {
-        'django': {'handlers': ['console'], 'level': 'INFO', 'propagate': False},
-        'xnbtd': {'handlers': ['console'], 'level': 'DEBUG', 'propagate': False},
-    },
-}
-
-# -----------------------------------------------------------------------------
-# Internationalization
-
-LANGUAGES = [
-    ('en', 'English'),
-    ('fr', 'Français'),
-]
-
-LANGUAGE_CODE = "en"
-
-LOCALE_PATHS = [BASE_PATH / 'locale']
-
-TIME_ZONE = "UTC"
-
-USE_I18N = True
-
-USE_TZ = True
+"""
+    Django Project settings
+"""
+import logging
+import os as __os
+from pathlib import Path as __Path
+
+
+ENV_TYPE = __os.environ.get('ENV_TYPE', None)
+print(f'ENV_TYPE:{ENV_TYPE!r}')
+
+
+###############################################################################
+
+# Build paths relative to the project root:
+PROJECT_PATH = __Path(__file__).resolve().parent.parent.parent
+print(f'PROJECT_PATH:{PROJECT_PATH}')
+
+# Build paths relative to the current working directory:
+BASE_PATH = __Path().cwd().resolve()
+print(f'BASE_PATH:{BASE_PATH}')
+
+# Paths with Django dev. server:
+# BASE_PATH...: .../django-for-runners
+# PROJECT_PATH: .../django-for-runners
+
+# But the paths are different, if it's installed as python package!
+
+###############################################################################
+
+LOGIN_URL = 'admin:login'
+
+###############################################################################
+
+
+# SECURITY WARNING: don't run with debug turned on in production!
+DEBUG = False
+TEMPLATE_DEBUG = False
+
+
+# SECURITY WARNING: keep the secret key used in production secret!
+__SECRET_FILE = __Path(BASE_PATH, 'secret.txt').resolve()
+if not __SECRET_FILE.is_file():
+    print(f'Generate {__SECRET_FILE}')
+    from secrets import token_urlsafe as __token_urlsafe
+
+    __SECRET_FILE.write_text(__token_urlsafe(128))
+
+SECRET_KEY = __SECRET_FILE.read_text().strip()
+
+
+# Application definition
+
+INSTALLED_APPS = [
+    'xnbtd.apps.XnbtdConfig',
+    'xnbtd.apps.XnbtdAdminConfig',
+    'xnbtd.tours.apps.ToursConfig',
+    'xnbtd.plannings.apps.PlanningsConfig',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'import_export',
+]
+
+ROOT_URLCONF = 'xnbtd.urls'
+WSGI_APPLICATION = 'xnbtd.wsgi.application'
+
+
+MIDDLEWARE = [
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    'django.middleware.locale.LocaleMiddleware',
+]
+
+TEMPLATES = [
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [str(__Path(PROJECT_PATH, 'xnbtd', 'templates'))],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
+            ],
+        },
+    },
+]
+
+USE_TZ = True
+
+# _____________________________________________________________________________
+
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+
+# _____________________________________________________________________________
+
+# Mark CSRF cookie as "secure" -> browsers sent cookie only with an HTTPS connection:
+CSRF_COOKIE_SECURE = True
+
+# Mark session cookie as "secure" -> browsers sent cookie only with an HTTPS connection:
+SESSION_COOKIE_SECURE = True
+
+# HTTP header/value combination that signifies a request is secure
+# Your nginx.conf must set "X-Forwarded-Protocol" proxy header!
+SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTOCOL', 'https')
+
+# SecurityMiddleware should redirects all non-HTTPS requests to HTTPS:
+SECURE_SSL_REDIRECT = True
+
+# SecurityMiddleware should preload directive to the HTTP Strict Transport Security header:
+SECURE_HSTS_PRELOAD = True
+
+# Instruct modern browsers to refuse to connect to your domain name via an insecure connection:
+SECURE_HSTS_SECONDS = 3600
+
+# SecurityMiddleware should add the "includeSubDomains" directive to the Strict-Transport-Security
+# header: All subdomains of your domain should be served exclusively via SSL!
+SECURE_HSTS_INCLUDE_SUBDOMAINS = True
+
+# _____________________________________________________________________________
+# Static files (CSS, JavaScript, Images)
+
+STATIC_URL = '/static/'
+STATIC_ROOT = str(__Path(BASE_PATH, 'static'))
+
+MEDIA_URL = '/media/'
+MEDIA_ROOT = str(__Path(BASE_PATH, 'media'))
+
+# _____________________________________________________________________________
+# cut 'pathname' in log output
+
+old_factory = logging.getLogRecordFactory()
+
+
+def cut_path(pathname, max_length):
+    if len(pathname) <= max_length:
+        return pathname
+    return f'...{pathname[-(max_length - 3):]}'
+
+
+def record_factory(*args, **kwargs):
+    record = old_factory(*args, **kwargs)
+    record.cut_path = cut_path(record.pathname, 30)
+    return record
+
+
+logging.setLogRecordFactory(record_factory)
+
+# -----------------------------------------------------------------------------
+
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': True,
+    'formatters': {
+        'verbose': {
+            'format': '%(asctime)s %(levelname)8s %(cut_path)s:%(lineno)-3s %(message)s',
+        }
+    },
+    'handlers': {'console': {'class': 'logging.StreamHandler', 'formatter': 'verbose'}},
+    'loggers': {
+        'django': {'handlers': ['console'], 'level': 'INFO', 'propagate': False},
+        'xnbtd': {'handlers': ['console'], 'level': 'DEBUG', 'propagate': False},
+    },
+}
+
+# -----------------------------------------------------------------------------
+# Internationalization
+
+LANGUAGES = [
+    ('en', 'English'),
+    ('fr', 'Français'),
+]
+
+LANGUAGE_CODE = "en"
+
+LOCALE_PATHS = [PROJECT_PATH / 'locale']
+
+TIME_ZONE = "UTC"
+
+USE_I18N = True
+
+USE_TZ = True
```

### Comparing `xnbtd-0.0.8/xnbtd/settings/local.py` & `xnbtd-0.0.9/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -13,14 +13,17 @@
 
 msgid "AVP Relay"
 msgstr "AVP Relais"
 
 msgid "Anomalies"
 msgstr "Anomalies"
 
+msgid "Beginning Hour"
+msgstr "début de la tournée"
+
 msgid "Breaks"
 msgstr "pauses"
 
 msgid "Charged Packages"
 msgstr "Colis chargé"
 
 msgid "Charged Points"
@@ -34,23 +37,23 @@
 
 msgid "Client numbers"
 msgstr "Nombres clients"
 
 msgid "EO"
 msgstr "EO"
 
+msgid "Ending Hour"
+msgstr "fin de la tournée"
+
 msgid "Full KM"
 msgstr "Plein / KM"
 
 msgid "GLS"
 msgstr "GLS"
 
-msgid "Hours"
-msgstr "heures"
-
 msgid "Including IP"
 msgstr "Dont IP"
 
 msgid "KM/Full"
 msgstr "KM/Plein"
 
 msgid "Overdue"
@@ -85,16 +88,37 @@
 
 msgid "SHD"
 msgstr "SHD"
 
 msgid "TNT - Fedex"
 msgstr "TNT - Fedex"
 
+msgid "Total Break Hours"
+msgstr "Total d’heures de pause"
+
+msgid "Total Clients"
+msgstr "Totals clients"
+
+msgid "Total Days"
+msgstr "Total de jours"
+
+msgid "Total Hour"
+msgstr "Durée de la tournée"
+
+msgid "Total Packages Delivered"
+msgstr "Total colis livrés"
+
 msgid "Total Points"
-msgstr "TOTAL POINTS"
+msgstr "Total points"
+
+msgid "Total Work Hours"
+msgstr "Total d’heures de travail"
+
+msgid "Total of Points"
+msgstr "Total de points"
 
 msgid "Tour Date"
 msgstr "date"
 
 msgid "Tour Name"
 msgstr "numéro de tournée"
 
@@ -106,14 +130,17 @@
 
 msgid "avp"
 msgstr "avp"
 
 msgid "avp_relay"
 msgstr "avp relais"
 
+msgid "beginning_hour"
+msgstr "début de la tournée"
+
 msgid "breaks"
 msgstr "pauses"
 
 msgid "cad"
 msgstr "cad"
 
 msgid "cad/return"
@@ -133,23 +160,23 @@
 
 msgid "date"
 msgstr "date"
 
 msgid "days"
 msgstr "jours"
 
+msgid "ending_hour"
+msgstr "fin de la tournée"
+
 msgid "eo"
 msgstr "eo"
 
 msgid "full_km"
 msgstr "plein / km"
 
-msgid "hours"
-msgstr "heures"
-
 msgid "including_ip"
 msgstr "dont ip"
 
 msgid "kilometers"
 msgstr "kilomètres"
 
 msgid "morning pickups"
@@ -217,14 +244,17 @@
 
 msgid "synchro"
 msgstr "synchro"
 
 msgid "total clients abductions"
 msgstr "totals clients enlèvements"
 
+msgid "total_hour"
+msgstr "Durée de la tournée"
+
 msgid "total_points"
 msgstr "total points"
 
 msgid "totals clients"
 msgstr "totals client"
 
 msgid "totals_clients"
```

### Comparing `xnbtd-0.0.8/xnbtd/tours/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -3,321 +3,370 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-18 17:06+0000\n"
+"POT-Creation-Date: 2023-07-21 21:01+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: xnbtd/tours/admin.py:11 xnbtd/tours/admin.py:34 xnbtd/tours/admin.py:60
-#: xnbtd/tours/admin.py:83
+#: xnbtd/tours/admin.py:14 xnbtd/tours/admin.py:41 xnbtd/tours/admin.py:69
+#: xnbtd/tours/admin.py:94
 msgid "name"
 msgstr "nom"
 
-#: xnbtd/tours/admin.py:12 xnbtd/tours/admin.py:35 xnbtd/tours/admin.py:61
-#: xnbtd/tours/admin.py:84
+#: xnbtd/tours/admin.py:15 xnbtd/tours/admin.py:42 xnbtd/tours/admin.py:70
+#: xnbtd/tours/admin.py:95
 msgid "date"
 msgstr "date"
 
-#: xnbtd/tours/admin.py:13
+#: xnbtd/tours/admin.py:16
 msgid "points_charges"
 msgstr "points chargés"
 
-#: xnbtd/tours/admin.py:15
+#: xnbtd/tours/admin.py:18
 msgid "points_delivered"
 msgstr "points livrés"
 
-#: xnbtd/tours/admin.py:18
+#: xnbtd/tours/admin.py:21
 msgid "packages_charges"
 msgstr "colis chargés"
 
-#: xnbtd/tours/admin.py:21
+#: xnbtd/tours/admin.py:24
 msgid "packages_delivered"
 msgstr "colis livrés"
 
-#: xnbtd/tours/admin.py:23
+#: xnbtd/tours/admin.py:26
 msgid "avp_relay"
 msgstr "avp relais"
 
-#: xnbtd/tours/admin.py:24
+#: xnbtd/tours/admin.py:27
 msgid "shd"
 msgstr "shd"
 
-#: xnbtd/tours/admin.py:25
+#: xnbtd/tours/admin.py:28
 msgid "eo"
 msgstr "eo"
 
-#: xnbtd/tours/admin.py:26
+#: xnbtd/tours/admin.py:29
 msgid "pickup_point"
 msgstr "point de ramasse"
 
-#: xnbtd/tours/admin.py:36
+#: xnbtd/tours/admin.py:30 xnbtd/tours/admin.py:58 xnbtd/tours/admin.py:83
+#: xnbtd/tours/admin.py:104 xnbtd/tours/models.py:96
+msgid "breaks"
+msgstr "pauses"
+
+#: xnbtd/tours/admin.py:31 xnbtd/tours/admin.py:59 xnbtd/tours/admin.py:84
+#: xnbtd/tours/admin.py:105
+msgid "beginning_hour"
+msgstr "début de la tournée"
+
+#: xnbtd/tours/admin.py:32 xnbtd/tours/admin.py:60 xnbtd/tours/admin.py:85
+#: xnbtd/tours/admin.py:106
+msgid "ending_hour"
+msgstr "fin de la tournée"
+
+#: xnbtd/tours/admin.py:33 xnbtd/tours/admin.py:61 xnbtd/tours/admin.py:86
+#: xnbtd/tours/admin.py:107
+msgid "total_hour"
+msgstr "Durée de la tournée"
+
+#: xnbtd/tours/admin.py:43
 msgid "client_numbers"
 msgstr "nombres clients"
 
-#: xnbtd/tours/admin.py:37
+#: xnbtd/tours/admin.py:44
 msgid "refused"
 msgstr "refuse"
 
-#: xnbtd/tours/admin.py:38 xnbtd/tours/admin.py:89 xnbtd/tours/models.py:54
-#: xnbtd/tours/models.py:87
+#: xnbtd/tours/admin.py:45 xnbtd/tours/admin.py:100 xnbtd/tours/models.py:89
+#: xnbtd/tours/models.py:138
 msgid "avp"
 msgstr "avp"
 
-#: xnbtd/tours/admin.py:39
+#: xnbtd/tours/admin.py:46
 msgid "cad"
 msgstr "cad"
 
-#: xnbtd/tours/admin.py:40
+#: xnbtd/tours/admin.py:47
 msgid "totals_clients"
 msgstr "totals client"
 
-#: xnbtd/tours/admin.py:42
+#: xnbtd/tours/admin.py:49
 msgid "occasional_abductions"
 msgstr "enlèvements occasionnels"
 
-#: xnbtd/tours/admin.py:45
+#: xnbtd/tours/admin.py:52
 msgid "regular_abductions"
 msgstr "enlèvements réguliers"
 
-#: xnbtd/tours/admin.py:48
+#: xnbtd/tours/admin.py:55
 msgid "totals_clients_abductions"
 msgstr "totals clients enlèvements"
 
-#: xnbtd/tours/admin.py:50 xnbtd/tours/admin.py:73 xnbtd/tours/models.py:60
-msgid "hours"
-msgstr "heures"
-
-#: xnbtd/tours/admin.py:51 xnbtd/tours/admin.py:74 xnbtd/tours/models.py:61
-msgid "breaks"
-msgstr "pauses"
-
-#: xnbtd/tours/admin.py:52
+#: xnbtd/tours/admin.py:57
 msgid "kilometers"
 msgstr "kilomètres"
 
-#: xnbtd/tours/admin.py:63
+#: xnbtd/tours/admin.py:72
 msgid "charged_packages"
 msgstr "colis chargé"
 
-#: xnbtd/tours/admin.py:65
+#: xnbtd/tours/admin.py:74
 msgid "charged_points"
 msgstr "points chargés"
 
-#: xnbtd/tours/admin.py:66
+#: xnbtd/tours/admin.py:75
 msgid "including_ip"
 msgstr "dont ip"
 
-#: xnbtd/tours/admin.py:67
+#: xnbtd/tours/admin.py:76
 msgid "relay"
 msgstr "relais"
 
-#: xnbtd/tours/admin.py:68
+#: xnbtd/tours/admin.py:77
 msgid "return_packages"
 msgstr "retour colis"
 
-#: xnbtd/tours/admin.py:69
+#: xnbtd/tours/admin.py:78
 msgid "return_points"
 msgstr "retour points"
 
-#: xnbtd/tours/admin.py:70
+#: xnbtd/tours/admin.py:79
 msgid "overdue"
 msgstr "hors délais"
 
-#: xnbtd/tours/admin.py:71
+#: xnbtd/tours/admin.py:80
 msgid "anomalies"
 msgstr "anomalies"
 
-#: xnbtd/tours/admin.py:72
+#: xnbtd/tours/admin.py:81
 msgid "total_points"
 msgstr "total points"
 
-#: xnbtd/tours/admin.py:75
+#: xnbtd/tours/admin.py:82
 msgid "full_km"
 msgstr "plein / km"
 
-#: xnbtd/tours/admin.py:85
+#: xnbtd/tours/admin.py:96
 msgid "type"
 msgstr "type"
 
-#: xnbtd/tours/admin.py:86
+#: xnbtd/tours/admin.py:97
 msgid "code"
 msgstr "code"
 
-#: xnbtd/tours/admin.py:87 xnbtd/tours/models.py:85
+#: xnbtd/tours/admin.py:98 xnbtd/tours/models.py:136
 msgid "nights"
 msgstr "nuits"
 
-#: xnbtd/tours/admin.py:88 xnbtd/tours/models.py:86
+#: xnbtd/tours/admin.py:99 xnbtd/tours/models.py:137
 msgid "days"
 msgstr "jours"
 
-#: xnbtd/tours/admin.py:90
+#: xnbtd/tours/admin.py:101
 msgid "spare_part"
 msgstr "spare part"
 
-#: xnbtd/tours/admin.py:91 xnbtd/tours/models.py:89
+#: xnbtd/tours/admin.py:102 xnbtd/tours/models.py:140
 msgid "synchro"
 msgstr "synchro"
 
-#: xnbtd/tours/admin.py:92
+#: xnbtd/tours/admin.py:103
 msgid "morning_pickup"
 msgstr "ramassages matin"
 
+#: xnbtd/tours/admin.py:136 xnbtd/tours/admin.py:171 xnbtd/tours/admin.py:207
+#: xnbtd/tours/admin.py:241
+msgid "Total Work Hours"
+msgstr "Total d’heures de travail"
+
+#: xnbtd/tours/admin.py:137 xnbtd/tours/admin.py:172 xnbtd/tours/admin.py:208
+#: xnbtd/tours/admin.py:242
+msgid "Total Break Hours"
+msgstr "Total d’heures de pause"
+
+#: xnbtd/tours/admin.py:138
+msgid "Total Packages Delivered"
+msgstr "Total colis livrés"
+
+#: xnbtd/tours/admin.py:173
+msgid "Total Clients"
+msgstr "Totals clients"
+
+#: xnbtd/tours/admin.py:209
+msgid "Total of Points"
+msgstr "Total de points"
+
+#: xnbtd/tours/admin.py:243
+msgid "Total Days"
+msgstr "Total de jours"
+
 #: xnbtd/tours/apps.py:8
 msgid "app_tours_name"
 msgstr "Tournées"
 
-#: xnbtd/tours/models.py:6 xnbtd/tours/models.py:26 xnbtd/tours/models.py:50
-#: xnbtd/tours/models.py:73
+#: xnbtd/tours/models.py:7 xnbtd/tours/models.py:45 xnbtd/tours/models.py:85
+#: xnbtd/tours/models.py:124
 msgid "Tour Name"
 msgstr "numéro de tournée"
 
-#: xnbtd/tours/models.py:7 xnbtd/tours/models.py:27 xnbtd/tours/models.py:51
-#: xnbtd/tours/models.py:84
+#: xnbtd/tours/models.py:8 xnbtd/tours/models.py:46 xnbtd/tours/models.py:86
+#: xnbtd/tours/models.py:135
 msgid "Tour Date"
 msgstr "date"
 
-#: xnbtd/tours/models.py:8
+#: xnbtd/tours/models.py:9
 msgid "Points Charges"
 msgstr "Points chargés"
 
-#: xnbtd/tours/models.py:9
+#: xnbtd/tours/models.py:10
 msgid "Points Delivered"
 msgstr "Points livrés"
 
-#: xnbtd/tours/models.py:10
+#: xnbtd/tours/models.py:11
 msgid "Packages Charges"
 msgstr "Colis chargés"
 
-#: xnbtd/tours/models.py:11
+#: xnbtd/tours/models.py:12
 msgid "Packages Delivered"
 msgstr "Colis livrés"
 
-#: xnbtd/tours/models.py:12
+#: xnbtd/tours/models.py:13
 msgid "AVP Relay"
 msgstr "AVP Relais"
 
-#: xnbtd/tours/models.py:13
+#: xnbtd/tours/models.py:14
 msgid "SHD"
 msgstr "SHD"
 
-#: xnbtd/tours/models.py:14
+#: xnbtd/tours/models.py:15
 msgid "EO"
 msgstr "EO"
 
-#: xnbtd/tours/models.py:15
+#: xnbtd/tours/models.py:16
 msgid "Pickup Point"
 msgstr "Point de ramasse"
 
-#: xnbtd/tours/models.py:21 xnbtd/tours/models.py:22
+#: xnbtd/tours/models.py:17 xnbtd/tours/models.py:57 xnbtd/tours/models.py:142
+msgid "Breaks"
+msgstr "pauses"
+
+#: xnbtd/tours/models.py:19 xnbtd/tours/models.py:59 xnbtd/tours/models.py:98
+#: xnbtd/tours/models.py:144
+msgid "Beginning Hour"
+msgstr "début de la tournée"
+
+#: xnbtd/tours/models.py:20 xnbtd/tours/models.py:60 xnbtd/tours/models.py:99
+#: xnbtd/tours/models.py:145
+msgid "Ending Hour"
+msgstr "fin de la tournée"
+
+#: xnbtd/tours/models.py:21 xnbtd/tours/models.py:61 xnbtd/tours/models.py:100
+#: xnbtd/tours/models.py:146
+msgid "Total Hour"
+msgstr "Durée de la tournée"
+
+#: xnbtd/tours/models.py:40 xnbtd/tours/models.py:41
 msgid "GLS"
 msgstr "GLS"
 
-#: xnbtd/tours/models.py:28
+#: xnbtd/tours/models.py:47
 msgid "Charged Packages"
 msgstr "Colis chargé"
 
-#: xnbtd/tours/models.py:29
+#: xnbtd/tours/models.py:48
 msgid "Charged Points"
 msgstr "Points chargés"
 
-#: xnbtd/tours/models.py:30
+#: xnbtd/tours/models.py:49
 msgid "Including IP"
 msgstr "Dont IP"
 
-#: xnbtd/tours/models.py:31
+#: xnbtd/tours/models.py:50
 msgid "Relay"
 msgstr "Relais"
 
-#: xnbtd/tours/models.py:32
+#: xnbtd/tours/models.py:51
 msgid "Return Packages"
 msgstr "Retour COLIS"
 
-#: xnbtd/tours/models.py:33
+#: xnbtd/tours/models.py:52
 msgid "Return Points"
 msgstr "Retour POINTS"
 
-#: xnbtd/tours/models.py:34
+#: xnbtd/tours/models.py:53
 msgid "Overdue"
 msgstr "HORS DELAIS"
 
-#: xnbtd/tours/models.py:35
+#: xnbtd/tours/models.py:54
 msgid "Anomalies"
 msgstr "Anomalies"
 
-#: xnbtd/tours/models.py:36
+#: xnbtd/tours/models.py:55
 msgid "Total Points"
-msgstr "TOTAL POINTS"
+msgstr "Total points"
 
-#: xnbtd/tours/models.py:37
-msgid "Hours"
-msgstr "heures"
-
-#: xnbtd/tours/models.py:38
-msgid "Breaks"
-msgstr "pauses"
-
-#: xnbtd/tours/models.py:39
+#: xnbtd/tours/models.py:56
 msgid "Full KM"
 msgstr "Plein / KM"
 
-#: xnbtd/tours/models.py:45 xnbtd/tours/models.py:46
+#: xnbtd/tours/models.py:80 xnbtd/tours/models.py:81
 msgid "Chronopost"
 msgstr "Chronopost"
 
-#: xnbtd/tours/models.py:52
+#: xnbtd/tours/models.py:87
 msgid "Client numbers"
 msgstr "Nombres clients"
 
-#: xnbtd/tours/models.py:53
+#: xnbtd/tours/models.py:88
 msgid "Refused"
 msgstr "refuse"
 
-#: xnbtd/tours/models.py:55
+#: xnbtd/tours/models.py:90
 msgid "cad/return"
 msgstr "cad/retour"
 
-#: xnbtd/tours/models.py:56
+#: xnbtd/tours/models.py:91
 msgid "totals clients"
 msgstr "totals client"
 
-#: xnbtd/tours/models.py:57
+#: xnbtd/tours/models.py:92
 msgid "occasional abductions"
 msgstr "enlèvements occasionnels"
 
-#: xnbtd/tours/models.py:58
+#: xnbtd/tours/models.py:93
 msgid "regular abductions"
 msgstr "enlèvements réguliers"
 
-#: xnbtd/tours/models.py:59
+#: xnbtd/tours/models.py:94
 msgid "total clients abductions"
 msgstr "totals clients enlèvements"
 
-#: xnbtd/tours/models.py:62
+#: xnbtd/tours/models.py:95
 msgid "KM/Full"
 msgstr "KM/Plein"
 
-#: xnbtd/tours/models.py:68 xnbtd/tours/models.py:69
+#: xnbtd/tours/models.py:119 xnbtd/tours/models.py:120
 msgid "TNT - Fedex"
 msgstr "TNT - Fedex"
 
-#: xnbtd/tours/models.py:88
+#: xnbtd/tours/models.py:139
 msgid "spare part"
 msgstr "spare part"
 
-#: xnbtd/tours/models.py:90
+#: xnbtd/tours/models.py:141
 msgid "morning pickups"
 msgstr "ramassages matin"
 
-#: xnbtd/tours/models.py:96 xnbtd/tours/models.py:97
+#: xnbtd/tours/models.py:165 xnbtd/tours/models.py:166
 msgid "Ciblex"
 msgstr "Ciblex"
```

### Comparing `xnbtd-0.0.8/PKG-INFO` & `xnbtd-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.8
+Version: 0.0.9
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

