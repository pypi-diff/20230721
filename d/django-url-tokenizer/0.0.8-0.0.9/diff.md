# Comparing `tmp/django-url-tokenizer-0.0.8.tar.gz` & `tmp/django-url-tokenizer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-url-tokenizer-0.0.8.tar", last modified: Thu Jul 13 06:17:38 2023, max compression
+gzip compressed data, was "django-url-tokenizer-0.0.9.tar", last modified: Thu Jul 13 23:13:34 2023, max compression
```

## Comparing `django-url-tokenizer-0.0.8.tar` & `django-url-tokenizer-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.8/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.8/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 06:14:53.000000 django-url-tokenizer-0.0.8/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/urltokenizer/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/apps.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/urltokenizer/migrations/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/migrations/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      716 2023-07-13 03:03:12.000000 django-url-tokenizer-0.0.8/urltokenizer/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1506 2023-07-13 06:17:13.000000 django-url-tokenizer-0.0.8/urltokenizer/serializers.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/tests.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4609 2023-07-13 06:15:21.000000 django-url-tokenizer-0.0.8/urltokenizer/tokenizer.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.8/urltokenizer/views.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.9/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.9/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 23:13:34.000000 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 23:13:34.000000 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 23:13:34.000000 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 23:13:34.000000 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 23:13:34.000000 django-url-tokenizer-0.0.9/django_url_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 23:13:32.000000 django-url-tokenizer-0.0.9/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/urltokenizer/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.9/urltokenizer/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.9/urltokenizer/apps.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 23:13:34.489805 django-url-tokenizer-0.0.9/urltokenizer/migrations/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.9/urltokenizer/migrations/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1208 2023-07-13 22:49:25.000000 django-url-tokenizer-0.0.9/urltokenizer/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1506 2023-07-13 06:17:13.000000 django-url-tokenizer-0.0.9/urltokenizer/serializers.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.9/urltokenizer/tests.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     5549 2023-07-13 22:48:05.000000 django-url-tokenizer-0.0.9/urltokenizer/tokenizer.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.9/urltokenizer/views.py
```

### Comparing `django-url-tokenizer-0.0.8/LICENSE` & `django-url-tokenizer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.8/setup.py` & `django-url-tokenizer-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-url-tokenizer",
-    version="0.0.8",
+    version="0.0.9",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package that provides a Django app that allows you to
     generate tokenized urls and send them to users via email.""",
     url="https://github.com/nibblex/django-url-tokenizer",
     packages=setuptools.find_packages(),
     license="MIT",
```

### Comparing `django-url-tokenizer-0.0.8/urltokenizer/serializers.py` & `django-url-tokenizer-0.0.9/urltokenizer/serializers.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.8/urltokenizer/tokenizer.py` & `django-url-tokenizer-0.0.9/urltokenizer/tokenizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         attributes = [
             getattr(user, attribute)
             for attribute in self.token_config.get("attributes", [])
         ]
         return f"{user.pk}{timestamp}{attributes}"
 
     def check_token(self, user, token):
-        permissions = self.token_config["permissions"].items()
-        all(getattr(user, attribute) == value for attribute, value in permissions)
+        preconditions = self.token_config["preconditions"].items()
+        all(getattr(user, attribute) == value for attribute, value in preconditions)
         return super().check_token(user, token)
 
     def run_callbacks(self, user, **kwargs):
         callbacks = self.token_config.get("callbacks", [])
         for callback in callbacks:
             method = getattr(user, callback.get("method"), None)
             if method is None:
@@ -73,60 +73,104 @@
     def token_config(self) -> dict:
         return self._token_generator.token_config
 
     @property
     def user_model(self):
         return get_user_model()
 
+    # url config
+
+    @property
+    def protocol(self) -> str:
+        return self.token_config.get("protocol", self._settings.get("PROTOCOL", "http"))
+
+    @property
+    def port(self) -> str:
+        return self.token_config.get("port", self._settings.get("PORT", "80"))
+
+    @property
+    def domain(self) -> str:
+        return self.token_config.get(
+            "domain", self._settings.get("DOMAIN", "localhost")
+        )
+
+    # mailing
+
+    @property
+    def email_enabled(self) -> bool:
+        return self.token_config.get(
+            "email_enabled", self._settings.get("EMAIL_ENABLED", False)
+        )
+
+    @property
+    def email_subject(self) -> str:
+        return self.token_config.get(
+            "email_subject",
+            self._settings.get(
+                "EMAIL_SUBJECT", "link generated with django-url-tokenizer"
+            ),
+        )
+
+    # encoding
+
     @property
     def encoding_field(self) -> str:
-        return self.user_model.ENCODING_FIELD
+        return self.token_config.get(
+            "encoding_field", self._settings.get("ENCODING_FIELD", "pk")
+        )
 
     @staticmethod
     def encode(s: Any) -> str:
         return urlsafe_base64_encode(force_bytes(s))
 
     @staticmethod
     def decode(s: bytes | str) -> str:
         return force_str(urlsafe_base64_decode(s))
 
-    @property
-    def default_domain(self) -> str:
-        return self._settings.get("DEFAULT_DOMAIN", "")
+    # main methods
 
     def generate_tokenized_link(
-        self, user, domain: str = None, send_email: bool = False
+        self,
+        user,
+        domain: str = None,
+        protocol: str = None,
+        port: str = None,
+        send_email: bool = False,
     ) -> tuple[str, str, str, bool]:
-        uidb64 = self.encode(getattr(user, user.ENCODING_FIELD))
+        domain = domain or self.domain
+        protocol = protocol or self.protocol
+        port = port or self.port
+
+        uidb64 = self.encode(getattr(user, self.encoding_field))
         token = self._token_generator.make_token(user)
 
-        domain = domain or self.token_config.get("domain", self.default_domain)
-        link = f"http://www.{domain}/{self.token_type}?uid={uidb64}&key={token}"
+        link = (
+            f"{protocol}://{domain}:{port}/{self.token_type}?uid={uidb64}&key={token}"
+        )
 
         email_sent = 0
-        email_config = self.token_config.get("email", {})
-        if send_email and email_config.get("enabled", False):
+        if send_email and self.email_enabled:
             email_sent = send_mail(
-                subject=email_config.get("subject", ""),
+                subject=self.email_subject,
                 message=link,
                 from_email=settings.DEFAULT_FROM_EMAIL,
                 recipient_list=[getattr(user, user.EMAIL_FIELD, None)],
                 fail_silently=True,
             )
 
         return uidb64, token, link, email_sent > 0
 
     def check_token(self, uidb64: str, token: str, **kwargs):
         try:
-            encoding_attr = self.decode(uidb64)
+            decoded_attr = self.decode(uidb64)
         except DjangoUnicodeDecodeError:
             return None
 
         user = self.user_model.objects.filter(
-            **{self.encoding_field: encoding_attr}
+            **{self.encoding_field: decoded_attr}
         ).first()
         if not user:
             return None
 
         if not self._token_generator.check_token(user, token):
             return None
```

