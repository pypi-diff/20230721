# Comparing `tmp/django_payments_flow-0.1.2.tar.gz` & `tmp/django_payments_flow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_payments_flow-0.1.2.tar", max compression
+gzip compressed data, was "django_payments_flow-0.1.3.tar", max compression
```

## Comparing `django_payments_flow-0.1.2.tar` & `django_payments_flow-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-07-10 21:02:11.879443 django_payments_flow-0.1.2/LICENSE
--rw-r--r--   0        0        0     2489 2023-07-10 21:02:11.879443 django_payments_flow-0.1.2/README.md
--rw-r--r--   0        0        0     5935 2023-07-10 21:02:11.879443 django_payments_flow-0.1.2/django_payments_flow/KhipuProvider.py
--rw-r--r--   0        0        0       49 2023-07-10 21:02:11.879443 django_payments_flow-0.1.2/django_payments_flow/__init__.py
--rw-r--r--   0        0        0     1889 2023-07-10 21:02:11.879443 django_payments_flow-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 django_payments_flow-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2489 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/README.md
+-rw-r--r--   0        0        0       98 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/__init__.py
+-rw-r--r--   0        0        0     5633 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/provider.py
+-rw-r--r--   0        0        0       22 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/django_payments_flow/version.py
+-rw-r--r--   0        0        0     2202 2023-07-21 02:37:16.993545 django_payments_flow-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 django_payments_flow-0.1.3/PKG-INFO
```

### Comparing `django_payments_flow-0.1.2/LICENSE` & `django_payments_flow-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_payments_flow-0.1.2/README.md` & `django_payments_flow-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_payments_flow-0.1.2/django_payments_flow/KhipuProvider.py` & `django_payments_flow-0.1.3/django_payments_flow/provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-from typing import Any
+from typing import Any, Optional
 
 from django.http import JsonResponse
 from payments import PaymentError, PaymentStatus, RedirectNeeded
-from payments.core import BasicProvider
-from pykhipu.client import Client
-from pykhipu.errors import AuthorizationError, ServiceError, ValidationError
+from payments.core import BasicProvider, get_base_url
+from payments.forms import PaymentForm as BasePaymentForm
+from pyflowcl import Payment as FlowPayment
+from pyflowcl.Clients import ApiClient
 
 
-class KhipuProvider(BasicProvider):
+class FlowProvider(BasicProvider):
     """
-    KhipuProvider es una clase que proporciona integración con Khipu para procesar pagos.
+    FlowProvider es una clase que proporciona integración con Flow para procesar pagos.
+    Inicializa una instancia de FlowProvider con el key y el secreto de Flow.
+
+    Args:
+        key (str): ID de receptor de Khipu.
+        secret (str): Secreto de Khipu.
+        medio (int | None): Versión de la API de notificaciones a utilizar (Valor por defecto: 9).
+        **kwargs: Argumentos adicionales.
     """
 
-    receiver_id: str = None
+    form_class = BasePaymentForm
+    endpoint: str
+    key: str = None
     secret: str = None
-    use_notification: str | None = "1.3"
-    bank_id: str | None = None
+    medio: int = 9
     _client: Any = None
 
-    def __init__(self, receiver_id: str, secret: str, use_notification: str | None, bank_id: str | None, **kwargs):
-        """
-        Inicializa una instancia de KhipuProvider con el ID de receptor y el secreto de Khipu proporcionados.
-
-        Args:
-            receiver_id (str): ID de receptor de Khipu.
-            secret (str): Secreto de Khipu.
-            use_notification (str | None): Versión de la API de notificaciones a utilizar (opcional).
-            bank_id (str | None): Id de Banco para variante (opcional).
-            **kwargs: Argumentos adicionales.
-        """
+    def __init__(self, endpoint: str, key: str, secret: str, medio: int, **kwargs):
         super().__init__(**kwargs)
-        self.receiver_id = receiver_id
+        self.endpoint = endpoint
+        self.key = key
         self.secret = secret
-        self.use_notification = use_notification
-        self.bank_id = bank_id
-        self._client = Client(receiver_id=receiver_id, secret=secret)
+        self.medio = medio
+        self._client = ApiClient(self.endpoint, self.key, self.secret)
 
-    def get_form(self, payment, data: dict | None = None) -> Any:
+    def get_form(self, payment, data: Optional[dict] = None) -> Any:
         """
         Genera el formulario de pago para redirigir a la página de pago de Khipu.
 
         Args:
             payment: Objeto de pago.
             data (dict | None): Datos del formulario (opcional).
 
@@ -48,47 +47,47 @@
             Any: Formulario de pago redirigido a la página de pago de Khipu.
 
         Raises:
             RedirectNeeded: Redirige a la página de pago de Khipu.
 
         """
         if not payment.transaction_id:
-            datos_para_khipu = {
-                "transaction_id": payment.token,
-                "return_url": payment.get_success_url(),
-                "cancel_url": payment.get_failure_url(),
+            datos_para_flow = {
+                "commerceOrder": payment.token,
+                "urlReturn": payment.get_success_url(),
+                "urlConfirmation": f"{get_base_url()}{payment.get_process_url()}",
+                "subject": payment.description,
+                "amount": int(payment.total),
+                "paymentMethod": self.medio,
+                "currency": payment.currency,
             }
-            if self.use_notification:
-                datos_para_khipu.update({"notify_url": self.get_notification_url()})
-                datos_para_khipu.update({"notify_api_version": self.use_notification})
-
-            if self.bank_id:
-                datos_para_khipu.update({"bank_id": self.bank_id})
 
             if payment.billing_email:
-                datos_para_khipu.update({"payer_email": payment.billing_email})
+                datos_para_flow.update({"email": payment.billing_email})
+
+            datos_para_flow.update(**self._extra_data(payment.attrs))
+
+            try:
+                payment.attrs.datos_flow = datos_para_flow
+                payment.save()
+            except Exception as e:
+                raise PaymentError(f"Ocurrió un error al guardar attrs.datos_flow: {e}")
 
-            datos_para_khipu.update(**self._extra_data(payment.attrs))
             try:
-                payment = self._client.payments.post(
-                    payment.description, payment.currency, int(payment.total), **datos_para_khipu
-                )
+                pago = FlowPayment.create(self._client, datos_para_flow)
 
-            except (ValidationError, AuthorizationError, ServiceError) as pe:
+            except Exception as pe:
                 payment.change_status(PaymentStatus.ERROR, str(pe))
                 raise PaymentError(pe)
             else:
-                payment.transaction_id = payment.payment_id
-                payment.attrs.payment_response = payment
+                payment.transaction_id = pago.token
+                payment.attrs.respuesta_flow = {"url": pago.url, "token": pago.token, "flowOrder": pago.flowOrder}
                 payment.save()
 
-        if "payment_url" not in payment:
-            raise PaymentError("Khipu no envió una URL, revisa los logs en Khipu.")
-
-        raise RedirectNeeded(payment.get("payment_url"))
+            raise RedirectNeeded(f"{pago.url}?token={pago.token}")
 
     def process_data(self, payment, request) -> JsonResponse:
         """
         Procesa los datos del pago recibidos desde Khipu.
 
         Args:
             payment: Objeto de pago.
@@ -101,38 +100,38 @@
         return JsonResponse("process_data")
 
     def _extra_data(self, attrs) -> dict:
         if "datos_extra" not in attrs:
             return {}
 
         data = attrs.datos_extra
-        if "payer_email" in data:
-            del data["payer_email"]
+        if "commerceOrder" in data:
+            del data["commerceOrder"]
 
-        if "subject" in data:
-            del data["subject"]
+        if "urlReturn" in data:
+            del data["urlReturn"]
 
-        if "currency" in data:
-            del data["currency"]
+        if "urlConfirmation" in data:
+            del data["urlConfirmation"]
 
         if "amount" in data:
             del data["amount"]
 
-        if "transaction_id" in data:
-            del data["transaction_id"]
+        if "subject" in data:
+            del data["subject"]
 
-        if "notify_url" in data:
-            del data["notify_url"]
+        if "paymentMethod" in data:
+            del data["paymentMethod"]
 
-        if "notify_api_version" in data:
-            del data["notify_api_version"]
+        if "currency" in data:
+            del data["currency"]
 
         return data
 
-    def refund(self, payment, amount: int | None = None) -> int:
+    def refund(self, payment, amount: Optional[int] = None) -> int:
         """
         Realiza un reembolso del pago.
 
         Args:
             payment: Objeto de pago.
             amount (int | None): Monto a reembolsar (opcional).
 
@@ -145,15 +144,15 @@
         """
         if payment.status != PaymentStatus.CONFIRMED:
             raise PaymentError("El pago debe estar confirmado para reversarse.")
 
         to_refund = amount or payment.total
         try:
             refund = self._client.payments.post_refunds(payment.transaction_id, to_refund)
-        except (ValidationError, AuthorizationError, ServiceError) as pe:
+        except Exception as pe:
             raise PaymentError(pe)
         else:
             payment.attrs.refund = refund
             payment.save()
             payment.change_status(PaymentStatus.REFUNDED)
             return to_refund
```

### Comparing `django_payments_flow-0.1.2/pyproject.toml` & `django_payments_flow-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-payments-flow"
-version = "0.1.2"
+version = "0.1.3"
 description = "Soporte Flow para Django Payments"
 authors = ["Mario Hernandez <mariofix@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_payments_flow"}]
 repository = "https://github.com/mariofix/django-payments-flow"
 documentation = "https://mariofix.github.io/django-payments-flow/"
@@ -27,53 +27,58 @@
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Framework :: Django",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.8.10"
 django-payments = "2.0.0"
+pyflowcl = "1.1.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 black = "^23.3.0"
 isort = "^5.12.0"
 coverage = "^7.2.7"
 pytest = "^7.4.0"
-faker = "^18.13.0"
+faker = ">=18.13,<20.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.18"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 mkdocs-git-committers-plugin-2 = "^1.1.2"
 pillow = "^10.0.0"
 cairosvg = "^2.7.0"
 lxml = "^4.9.3"
+pytest-cov = "^4.1.0"
+pytest-django = "^4.5.2"
+pytest-mock = "^3.11.1"
+dj-database-url = "^2.0.0"
+factory-boy = "^3.3.0"
+tox = "^4.6.4"
+tox-gh-actions = "^3.1.3"
 
 
 
 [tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra"
-testpaths = [
-    "tests",
-]
-python_files =[
-    "test*.py"
-]
+# DJANGO_SETTINGS_MODULE = "tests.django_settings"
+addopts = "--cov=django_payments_flow/ --cov-branch --cov-report=term-missing --cov-report=xml"
 
 [tool.black]
-line-length = 120
+line-length = 119
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
-multi_line_output = 3
+line_length = 119
+multi_line_output = 5
 py_version = 38
+src_paths = ["django_payments_flow", "tests", "sandbox"]
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_payments_flow-0.1.2/PKG-INFO` & `django_payments_flow-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: django-payments-flow
-Version: 0.1.2
+Version: 0.1.3
 Summary: Soporte Flow para Django Payments
 Home-page: https://www.flow.cl/docs/api.html
 License: MIT
 Keywords: flow,pagos,django,payment,django-payments
 Author: Mario Hernandez
 Author-email: mariofix@proton.me
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.10,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django-payments (==2.0.0)
+Requires-Dist: pyflowcl (==1.1.2)
 Project-URL: Documentation, https://mariofix.github.io/django-payments-flow/
 Project-URL: Repository, https://github.com/mariofix/django-payments-flow
 Description-Content-Type: text/markdown
 
 # django-payments-flow
 
 `Proyecto en desarrollo activo, no listo para produccion`
```

