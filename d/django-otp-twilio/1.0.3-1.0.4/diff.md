# Comparing `tmp/django-otp-twilio-1.0.3.tar.gz` & `tmp/django_otp_twilio-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-otp-twilio-1.0.3.tar", last modified: Tue Apr 25 17:51:13 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-otp-twilio-1.0.3.tar` & `django_otp_twilio-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,27 @@
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     4888 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/CHANGES.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1297 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/LICENSE
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      100 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/MANIFEST.in
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/PKG-INFO
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      710 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/README.rst
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5709 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/Makefile
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/ext/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      217 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/ext/otpdocs.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/source/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)       54 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/source/changes.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     8876 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/docs/source/conf.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     3029 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.3/docs/source/index.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      147 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/setup.cfg
--rwxrwxr-x   0 psagers   (1000) psagers   (1000)     1087 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/setup.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/PKG-INFO
--rw-r--r--   0 psagers   (1000) psagers   (1000)      752 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/SOURCES.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/dependency_links.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)       27 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/requires.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)       11 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/top_level.txt
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/otp_twilio/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      667 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      146 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/apps.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1053 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.3/src/otp_twilio/conf.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1411 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      540 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0002_last_t.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      463 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0003_longer_number.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1465 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0004_sidechanneldevice.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/__init__.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     4080 2023-04-25 17:47:23.000000 django-otp-twilio-1.0.3/src/otp_twilio/models.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     3209 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/tests.py
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/CHANGES.rst
+-rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/docs/ext/otpdocs.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/docs/source/changes.rst
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/docs/source/conf.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/admin.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/apps.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/conf.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/models.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/tests.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/migrations/0001_initial.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/migrations/0002_last_t.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/migrations/0003_longer_number.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/migrations/0004_sidechanneldevice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/src/otp_twilio/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/test/test_project/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/test/test_project/settings.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/test/test_project/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/test/test_project/templates/registration/logged_out.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/.hgignore
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/README.rst
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 django_otp_twilio-1.0.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-otp-twilio-1.0.3/CHANGES.rst` & `django_otp_twilio-1.0.4/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+v1.0.4 - July 20, 2023 - Add OTP_TWILIO_MESSAGING_SERVICE_SID setting
+--------------------------------------------------------------------------------
+
+`#9`_: OTP_TWILIO_MESSAGING_SERVICE_SID setting
+
+.. _#9: https://github.com/django-otp/django-otp-twilio/pull/9
+
+
 v1.0.3 - April 25, 2023 - Fix API key handling
 --------------------------------------------------------------------------------
 
 Fix `#6`_: Code uses "TWILIO_API_KEY" instead of "OTP_TWILIO_API_KEY"
 
 .. _#6: https://github.com/django-otp/django-otp-twilio/pull/6
 
@@ -15,156 +23,156 @@
 v1.0.1 - November 29, 2021 - Forward compatibility
 --------------------------------------------------------------------------------
 
 Default to AutoField to avoid spurious migrations.
 
 
 v1.0.0 - August 13, 2020 - Update test matrix
-------------------------------------------------------------
+--------------------------------------------------------------------------------
 
 - Added Django 3.1 to the test environments and fixed deprecation warnings.
 
 - Version bumped to align with the core django-otp project.
 
 
 v0.6.0 - May 06, 2020 - ThrottlingMixin and SideChannelDevice
--------------------------------------------------------------------------------
+--------------------------------------------------------------------------------
 
 TwilioSMSDevice is now a :class:`~django_otp.models.SideChannelDevice` and
 implements :class:`~django_otp.models.ThrottlingMixin`.
 
 This also drops support for old versions of Python (2.7) and Django (1.11,
 2.1).
 
 Note that this version includes migrations that will invalidate any in-flight
 tokens.
 
 
 v0.5.1 - August 26, 2019 - Housekeeping
----------------------------------------
+--------------------------------------------------------------------------------
 
 Build, test, and documentation cleanup.
 
 
 v0.5.0 - August 14, 2018 - Django 2.1 support
----------------------------------------------
+--------------------------------------------------------------------------------
 
 - Drop support for Django < 1.11.
 
 
 v0.4.2 - October 18, 2017 - Fix migration
------------------------------------------
+--------------------------------------------------------------------------------
 
 - Fix a spurious migration offered by makemigrations.
 
 
 v0.4.1 - August 29, 2017 - Default keys
----------------------------------------
+--------------------------------------------------------------------------------
 
 - Fix `#25`_: make sure default keys are unicode values.
 
 .. _#25: https://bitbucket.org/psagers/django-otp/issues/25/attributeerror-bytes-object-has-no
 
 
 v0.4.0 - July 19, 2017 - Update support matrix
-----------------------------------------------
+--------------------------------------------------------------------------------
 
 - Drop support for versions of Django that are past EOL.
 
 
 v0.3.6 - November 27, 2016 - Forward compatbility for Django 2.0
-----------------------------------------------------------------
+--------------------------------------------------------------------------------
 
 - Treat :attr:`~django.contrib.auth.models.User.is_authenticated` and
   :attr:`~django.contrib.auth.models.User.is_anonymous` as properties in Django
   1.10 and later.
 
 - Add explict on_delete behavior for all foreign keys.
 
 
 v0.3.5 - October 9, 2016 - Longer numbers
------------------------------------------
+--------------------------------------------------------------------------------
 
 - Support longer phone numbers.
 
 
 v0.3.4 - January 10, 2016 - Python 3 cleanup
---------------------------------------------
+--------------------------------------------------------------------------------
 
 - All modules include all four Python 3 __future__ imports for consistency.
 
 - Migrations no longer have byte strings in them.
 
 
 v0.3.3 - October 11, 2015 - Django 1.8
---------------------------------------
+--------------------------------------------------------------------------------
 
 - Use ModelAdmin.raw_id_fields for foreign keys to users.
 
 - General cleanup and compatibility with Django 1.9a1.
 
 
 v0.3.1 - March 1, 2015 - Token validity
----------------------------------------
+--------------------------------------------------------------------------------
 
 - The length of time that tokens are valid can now be configured with
   :setting:`OTP_TWILIO_TOKEN_VALIDITY`.
 
 - Tokens now become invalid as soon as they have been verified.
 
 
 v0.3.0 - February 7, 2015 - Support Django migrations
------------------------------------------------------
+--------------------------------------------------------------------------------
 
 - otp_twilio now has both Django and South migrations. Please see the `upgrade
   notes`_ for details on upgrading from previous versions.
 
 .. _upgrade notes: https://pythonhosted.org/django-otp/overview.html#upgrading
 
 
 v0.2.2 - Aug 20, 2014 - Challenge template
-------------------------------------------
+--------------------------------------------------------------------------------
 
 - :setting:`OTP_TWILIO_CHALLENGE_MESSAGE` allows you to customize the string
   returned to the user after the SMS is sent. It also accepts the {token}
   placeholder as a convenience for development.
 
 - Fixes for unit tests under the latest pre-release version of Django 1.7.
 
 
 v0.2.1 - May 8, 2014 - Message template
----------------------------------------
+--------------------------------------------------------------------------------
 
 - :setting:`OTP_TWILIO_TOKEN_TEMPLATE` allows you to customize the message that
   is sent by SMS.
 
 
 v0.2.0 - November 10, 2013 - Django 1.6
----------------------------------------
+--------------------------------------------------------------------------------
 
 - Now supports Django 1.4 to 1.6 on Python 2.6, 2.7, 3.2, and 3.3. This is the
   first release for Python 3.
 
 
 v0.1.3 - May 9, 2013 - Unit test improvements
----------------------------------------------
+--------------------------------------------------------------------------------
 
 Major unit test cleanup. Tests should pass or be skipped under all supported
 versions of Django, with or without custom users and timzeone support.
 
 
 v0.1.2 - March 24, 2013 - Bug fix
----------------------------------
+--------------------------------------------------------------------------------
 
 - Fix for requests integration.
 
 
 v0.1.1 - October 8, 2012 - Bug fix
-----------------------------------
+--------------------------------------------------------------------------------
 
 - Fix exception with an empty token form.
 
 
 v0.1.0 - August 20, 2012 - Initial Release
-------------------------------------------
+--------------------------------------------------------------------------------
 
 Initial release.
```

### Comparing `django-otp-twilio-1.0.3/docs/Makefile` & `django_otp_twilio-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.3/docs/source/conf.py` & `django_otp_twilio-1.0.4/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import os
 import sys
 
 # autodoc and viewcode need valid settings in order to process Django modules.
 import django
 import django.conf
 
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('../ext'))
 
 # -- General configuration -----------------------------------------------------
 
@@ -31,15 +30,14 @@
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.viewcode',
-
     'otpdocs',
 ]
 
 
 django.conf.settings.configure(
     DATABASES={
         'default': {
@@ -48,26 +46,27 @@
     },
     INSTALLED_APPS=[
         'django.contrib.admin',
         'django.contrib.auth',
         'django.contrib.contenttypes',
         'django.contrib.sessions',
         'django.contrib.messages',
-
         'django_otp',
         'otp_twilio',
     ],
     SECRET_KEY='properly-configured',
 )
 django.setup()
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
-    'django': ('https://docs.djangoproject.com/en/2.2/',
-               'https://docs.djangoproject.com/en/2.2/_objects/'),
+    'django': (
+        'https://docs.djangoproject.com/en/4.2/',
+        'https://docs.djangoproject.com/en/4.2/_objects/',
+    ),
     'django-otp': ('http://django-otp-official.readthedocs.io/en/latest/', None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
@@ -84,15 +83,15 @@
 copyright = u'2012, Peter Sagerson'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.0.3'
+release = '1.0.4'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
@@ -209,27 +208,30 @@
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ('index', 'django-otp-twilio.tex', u'django-otp-twilio Documentation',
-     'Peter Sagerson', 'manual'),
+    (
+        'index',
+        'django-otp-twilio.tex',
+        u'django-otp-twilio Documentation',
+        'Peter Sagerson',
+        'manual',
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -250,31 +252,42 @@
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'django-otp-twilio', u'django-otp-twilio Documentation',
-     [u'Peter Sagerson'], 1)
+    (
+        'index',
+        'django-otp-twilio',
+        u'django-otp-twilio Documentation',
+        [u'Peter Sagerson'],
+        1,
+    )
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'django-otp-twilio', u'django-otp-twilio Documentation',
-     'Peter Sagerson', 'django-otp-twilio', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        'index',
+        'django-otp-twilio',
+        u'django-otp-twilio Documentation',
+        'Peter Sagerson',
+        'django-otp-twilio',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
```

### Comparing `django-otp-twilio-1.0.3/docs/source/index.rst` & `django_otp_twilio-1.0.4/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 django-otp-twilio
 =================
 
 .. include:: ../../README.rst
+   :end-before: .. end-of-doc-intro
 
 
 Installation
 ------------
 
 django-otp-twilio can be installed via pip::
 
@@ -25,15 +26,15 @@
     ]
 
 
 Twilio SMS Devices
 ------------------
 
 .. autoclass:: otp_twilio.models.TwilioSMSDevice
-    :members:
+   :members:
 
 
 Admin
 -----
 
 The following :class:`~django.contrib.admin.ModelAdmin` subclass is registered
 with the default admin site. We recommend its use with custom admin sites as
@@ -98,14 +99,25 @@
 
 Default: ``None``
 
 The phone number to send SMS messages from. This must be one of your Twilio
 numbers.
 
 
+.. setting:: OTP_TWILIO_MESSAGING_SERVICE_SID
+
+**OTP_TWILIO_MESSAGING_SERVICE_SID**
+
+Default: ``None``
+
+The Twilio messaging service SID to send SMS messages from. This must be one of
+your Twilio messaging services. If supplied, this takes precedence over
+``OTP_TWILIO_FROM``.
+
+
 .. setting:: OTP_TWILIO_NO_DELIVERY
 
 **OTP_TWILIO_NO_DELIVERY**
 
 Default: ``False``
 
 Send tokens to the 'otp_twilio.models' logger instead of delivering them by SMS.
```

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/admin.py` & `django_otp_twilio-1.0.4/src/otp_twilio/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,28 @@
 
 
 class TwilioSMSDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~otp_twilio.models.TwilioSMSDevice`.
     """
+
     fieldsets = [
-        ('Identity', {
-            'fields': ['user', 'name', 'confirmed'],
-        }),
-        ('Configuration', {
-            'fields': ['number'],
-        }),
+        (
+            'Identity',
+            {
+                'fields': ['user', 'name', 'confirmed'],
+            },
+        ),
+        (
+            'Configuration',
+            {
+                'fields': ['number'],
+            },
+        ),
     ]
     raw_id_fields = ['user']
 
 
 try:
     admin.site.register(TwilioSMSDevice, TwilioSMSDeviceAdmin)
 except AlreadyRegistered:
```

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/conf.py` & `django_otp_twilio-1.0.4/src/otp_twilio/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 class Settings(object):
     """
     This is a simple class to take the place of the global settings object. An
     instance will contain all of our settings as attributes, with default
     values if they are not specified by the configuration.
     """
+
     _defaults = {
         'OTP_TWILIO_URL': "https://api.twilio.com",
         'OTP_TWILIO_ACCOUNT': None,
         'OTP_TWILIO_API_KEY': None,
         'OTP_TWILIO_AUTH': None,
         'OTP_TWILIO_CHALLENGE_MESSAGE': "Sent by SMS",
         'OTP_TWILIO_FROM': None,
+        'OTP_TWILIO_MESSAGING_SERVICE_SID': None,
         'OTP_TWILIO_NO_DELIVERY': False,
         'OTP_TWILIO_THROTTLE_FACTOR': 1,
         'OTP_TWILIO_TOKEN_TEMPLATE': '{token}',
         'OTP_TWILIO_TOKEN_VALIDITY': 30,
     }
 
     def __getattr__(self, name):
```

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0001_initial.py` & `django_otp_twilio-1.0.4/src/otp_twilio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0002_last_t.py` & `django_otp_twilio-1.0.4/src/otp_twilio/migrations/0002_last_t.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0004_sidechanneldevice.py` & `django_otp_twilio-1.0.4/src/otp_twilio/migrations/0004_sidechanneldevice.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/models.py` & `django_otp_twilio-1.0.4/src/otp_twilio/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import logging
 
-from django.core.exceptions import ImproperlyConfigured
-from django.db import models
-from django.utils.encoding import force_str
-
 from django_otp.models import SideChannelDevice, ThrottlingMixin
 from django_otp.util import hex_validator, random_hex
 import requests
 
-from .conf import settings
+from django.core.exceptions import ImproperlyConfigured
+from django.db import models
+from django.utils.encoding import force_str
 
+from .conf import settings
 
 logger = logging.getLogger(__name__)
 
 
 def default_key():  # pragma: no cover
-    """ Obsolete code here for migrations. """
+    """Obsolete code here for migrations."""
     return force_str(random_hex(20))
 
 
 def key_validator(value):  # pragma: no cover
-    """ Obsolete code here for migrations. """
+    """Obsolete code here for migrations."""
     return hex_validator(20)(value)
 
 
 class TwilioSMSDevice(ThrottlingMixin, SideChannelDevice):
     """
     A :class:`~django_otp.models.SideChannelDevice` that delivers a token via
     the Twilio SMS service.
@@ -38,17 +37,17 @@
         <https://www.twilio.com/docs/api/rest/sending-messages>`_ using the
         `E.164 <http://en.wikipedia.org/wiki/E.164>`_ format. For US numbers,
         this would look like '+15555555555'. At the time of writing, Twilio
         will try to infer the correct E.164 format if it is not used, but this
         should not be relied upon.
 
     """
+
     number = models.CharField(
-        max_length=30,
-        help_text="The mobile number to deliver tokens to (E.164)."
+        max_length=30, help_text="The mobile number to deliver tokens to (E.164)."
     )
 
     class Meta(SideChannelDevice.Meta):
         verbose_name = "Twilio SMS Device"
 
     def get_throttle_factor(self):
         return settings.OTP_TWILIO_THROTTLE_FACTOR
@@ -73,24 +72,35 @@
         challenge = settings.OTP_TWILIO_CHALLENGE_MESSAGE.format(token=self.token)
 
         return challenge
 
     def _deliver_token(self, token):
         self._validate_config()
 
-        url = '{0}/2010-04-01/Accounts/{1}/Messages.json'.format(settings.OTP_TWILIO_URL, settings.OTP_TWILIO_ACCOUNT)
+        url = '{0}/2010-04-01/Accounts/{1}/Messages.json'.format(
+            settings.OTP_TWILIO_URL, settings.OTP_TWILIO_ACCOUNT
+        )
         data = {
-            'From': settings.OTP_TWILIO_FROM,
             'To': self.number,
             'Body': str(token),
         }
+        if settings.OTP_TWILIO_MESSAGING_SERVICE_SID:
+            data['MessagingServiceSid'] = settings.OTP_TWILIO_MESSAGING_SERVICE_SID
+        else:
+            data['From'] = settings.OTP_TWILIO_FROM
 
         response = requests.post(
-            url, data=data,
-            auth=(settings.OTP_TWILIO_API_KEY if settings.OTP_TWILIO_API_KEY else settings.OTP_TWILIO_ACCOUNT, settings.OTP_TWILIO_AUTH)
+            url,
+            data=data,
+            auth=(
+                settings.OTP_TWILIO_API_KEY
+                if settings.OTP_TWILIO_API_KEY
+                else settings.OTP_TWILIO_ACCOUNT,
+                settings.OTP_TWILIO_AUTH,
+            ),
         )
 
         try:
             response.raise_for_status()
         except Exception as e:
             logger.exception('Error sending token by Twilio SMS: {0}'.format(e))
             raise
@@ -98,21 +108,27 @@
         if 'sid' not in response.json():
             message = response.json().get('message')
             logger.error('Error sending token by Twilio SMS: {0}'.format(message))
             raise Exception(message)
 
     def _validate_config(self):
         if settings.OTP_TWILIO_ACCOUNT is None:
-            raise ImproperlyConfigured('OTP_TWILIO_ACCOUNT must be set to your Twilio account identifier')
+            raise ImproperlyConfigured(
+                'OTP_TWILIO_ACCOUNT must be set to your Twilio account identifier'
+            )
 
         if settings.OTP_TWILIO_AUTH is None:
-            raise ImproperlyConfigured('OTP_TWILIO_AUTH must be set to your Twilio auth token')
+            raise ImproperlyConfigured(
+                'OTP_TWILIO_AUTH must be set to your Twilio auth token'
+            )
 
         if settings.OTP_TWILIO_FROM is None:
-            raise ImproperlyConfigured('OTP_TWILIO_FROM must be set to one of your Twilio phone numbers')
+            raise ImproperlyConfigured(
+                'OTP_TWILIO_FROM must be set to one of your Twilio phone numbers'
+            )
 
     def verify_token(self, token):
         verify_allowed, _ = self.verify_is_allowed()
         if verify_allowed:
             verified = super().verify_token(token)
 
             if verified:
```

### Comparing `django-otp-twilio-1.0.3/src/otp_twilio/tests.py` & `django_otp_twilio-1.0.4/src/otp_twilio/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import mock
 
-from django.db import IntegrityError
-from django.test.utils import override_settings
-
 from django_otp.tests import TestCase, ThrottlingTestMixin
 from freezegun import freeze_time
 
+from django.db import IntegrityError
+from django.test.utils import override_settings
+
 from .conf import settings
 
 
 class TwilioDeviceMixin:
     def setUp(self):
         try:
             alice = self.create_user('alice', 'password')
@@ -29,41 +29,41 @@
 class TestTwilioSMS(TwilioDeviceMixin, TestCase):
     def setUp(self):
         super().setUp()
 
         self._delivered = None
 
     def test_instant(self):
-        """ Verify a code the instant it was generated. """
+        """Verify a code the instant it was generated."""
         with freeze_time():
             token = self.device.generate_challenge()
             ok = self.device.verify_token(token)
 
         self.assertTrue(ok)
 
     def test_barely_made_it(self):
-        """ Verify a code at the last possible second. """
+        """Verify a code at the last possible second."""
         with freeze_time() as frozen_time:
             token = self.device.generate_challenge()
             frozen_time.tick(delta=(settings.OTP_TWILIO_TOKEN_VALIDITY - 1))
             ok = self.device.verify_token(token)
 
         self.assertTrue(ok)
 
     def test_too_late(self):
-        """ Try to verify a code one second after it expires. """
+        """Try to verify a code one second after it expires."""
         with freeze_time() as frozen_time:
             token = self.device.generate_challenge()
             frozen_time.tick(delta=(settings.OTP_TWILIO_TOKEN_VALIDITY + 1))
             ok = self.device.verify_token(token)
 
         self.assertFalse(ok)
 
     def test_code_reuse(self):
-        """ Try to verify the same code twice. """
+        """Try to verify the same code twice."""
         with freeze_time():
             token = self.device.generate_challenge()
             ok1 = self.device.verify_token(token)
             ok2 = self.device.verify_token(token)
 
         self.assertTrue(ok1)
         self.assertFalse(ok2)
@@ -76,15 +76,17 @@
         self.assertFalse(ok)
 
     @override_settings(
         OTP_TWILIO_NO_DELIVERY=False,
         OTP_TWILIO_TOKEN_TEMPLATE='Token is {token}',
     )
     def test_format(self):
-        with mock.patch('otp_twilio.models.TwilioSMSDevice._deliver_token', self._deliver_token):
+        with mock.patch(
+            'otp_twilio.models.TwilioSMSDevice._deliver_token', self._deliver_token
+        ):
             self.device.generate_challenge()
 
         self.assertEqual('Token is {}'.format(self.device.token), self._delivered)
 
     #
     # Utilities
     #
```

