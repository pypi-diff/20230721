# Comparing `tmp/pretix-sumup-1.0.0.tar.gz` & `tmp/pretix-sumup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.0.tar", last modified: Fri Jul 21 08:15:12 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.1.tar", last modified: Fri Jul 21 08:40:05 2023, max compression
```

## Comparing `pretix-sumup-1.0.0.tar` & `pretix-sumup-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.886076 pretix-sumup-1.0.0/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.886076 pretix-sumup-1.0.0/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.886076 pretix-sumup-1.0.0/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.886076 pretix-sumup-1.0.0/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.890076 pretix-sumup-1.0.0/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-07-21 08:15:12.000000 pretix-sumup-1.0.0/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 08:15:12.000000 pretix-sumup-1.0.0/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:15:12.000000 pretix-sumup-1.0.0/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 08:15:12.000000 pretix-sumup-1.0.0/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 08:15:12.000000 pretix-sumup-1.0.0/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:12.894076 pretix-sumup-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 08:13:49.000000 pretix-sumup-1.0.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.0/LICENSE` & `pretix-sumup-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/PKG-INFO` & `pretix-sumup-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -664,9 +664,61 @@
         You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
 Project-URL: homepage, https://github.com/highcanfly/pretix-sumup
 Project-URL: repository, https://github.com/highcanfly/pretix-sumup
 Keywords: pretix
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+---
+title: Sumup for Pretix
+---
+
+This is a plugin for [pretix](https://github.com/pretix/pretix).
+
+# Description
+
+This is an alpha stage payment plugin for Pretix 4, it allows to use
+Sumup online payment. You need to register an OAuth app in your Sumup
+developer account. You also to manually request the \"payment\" scope to
+Sumup.
+
+# Development setup
+
+1.  Make sure that you have a working [pretix development
+    setup](https://docs.pretix.eu/en/latest/development/setup.html).
+2.  Clone this repository.
+3.  Activate the virtual environment you use for pretix development.
+4.  Execute `python setup.py develop` within this directory to register
+    this application with pretix\'s plugin registry.
+5.  Execute `make` within this directory to compile translations.
+6.  Restart your local pretix server. You can now use the plugin from
+    this repository for your events by enabling it in the \'plugins\'
+    tab in the settings. supervisorctl -s unix:///tmp/supervisor.sock
+    restart pretixweb
+
+This plugin has CI set up to enforce a few code style rules. To check
+locally, you need these packages installed:
+
+    pip install flake8 isort black
+
+To check your plugin for rule violations, run:
+
+    black --check .
+    isort -c .
+    flake8 .
+
+You can auto-fix some of these issues by running:
+
+    isort .
+    black .
+
+To automatically check for these issues before you commit, you can run
+`.install-hooks`.
+
+# License
+
+Copyright 2023 Ronan Le Meillat
+
+Released under the terms of the GNU Affero General Public License v3
```

### Comparing `pretix-sumup-1.0.0/README.md` & `pretix-sumup-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/apps.py` & `pretix-sumup-1.0.1/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/payment.py` & `pretix-sumup-1.0.1/pretix_sumup/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/signals.py` & `pretix-sumup-1.0.1/pretix_sumup/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,15 @@
                 console.log('Body', body);
                 if (type == "success") {
                     document.getElementById('help-text').innerHTML = "";
                     sumupCard.unmount();
                     submitElm.classList.remove('hidden');
                     submitElm.disabled = false;
                     submitElm.innerHTML = "{{btn_text}}";
+                    document.querySelector("body > div.container.main-box > main > form").submit();
                 }
             }
         });
     })
 
 
 </script>
```

### Comparing `pretix-sumup-1.0.0/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.1/pretix_sumup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -664,9 +664,61 @@
         You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
 Project-URL: homepage, https://github.com/highcanfly/pretix-sumup
 Project-URL: repository, https://github.com/highcanfly/pretix-sumup
 Keywords: pretix
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+---
+title: Sumup for Pretix
+---
+
+This is a plugin for [pretix](https://github.com/pretix/pretix).
+
+# Description
+
+This is an alpha stage payment plugin for Pretix 4, it allows to use
+Sumup online payment. You need to register an OAuth app in your Sumup
+developer account. You also to manually request the \"payment\" scope to
+Sumup.
+
+# Development setup
+
+1.  Make sure that you have a working [pretix development
+    setup](https://docs.pretix.eu/en/latest/development/setup.html).
+2.  Clone this repository.
+3.  Activate the virtual environment you use for pretix development.
+4.  Execute `python setup.py develop` within this directory to register
+    this application with pretix\'s plugin registry.
+5.  Execute `make` within this directory to compile translations.
+6.  Restart your local pretix server. You can now use the plugin from
+    this repository for your events by enabling it in the \'plugins\'
+    tab in the settings. supervisorctl -s unix:///tmp/supervisor.sock
+    restart pretixweb
+
+This plugin has CI set up to enforce a few code style rules. To check
+locally, you need these packages installed:
+
+    pip install flake8 isort black
+
+To check your plugin for rule violations, run:
+
+    black --check .
+    isort -c .
+    flake8 .
+
+You can auto-fix some of these issues by running:
+
+    isort .
+    black .
+
+To automatically check for these issues before you commit, you can run
+`.install-hooks`.
+
+# License
+
+Copyright 2023 Ronan Le Meillat
+
+Released under the terms of the GNU Affero General Public License v3
```

### Comparing `pretix-sumup-1.0.0/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.1/pretix_sumup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.0/pyproject.toml` & `pretix-sumup-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pretix-sumup"
 dynamic = ["version"]
 description = "Sumup plugin"
-readme = "README.rst"
+readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["pretix"]
 authors = [
     {name = "Ronan Le Meillat", email = "ronan@highcanfly.club"},
 ]
 maintainers = [
     {name = "Ronan Le Meillat", email = "ronan@highcanfly.club"},
```

### Comparing `pretix-sumup-1.0.0/setup.cfg` & `pretix-sumup-1.0.1/setup.cfg`

 * *Files identical despite different names*

