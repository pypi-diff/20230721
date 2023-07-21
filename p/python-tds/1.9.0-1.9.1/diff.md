# Comparing `tmp/python-tds-1.9.0.tar.gz` & `tmp/python-tds-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-tds-1.9.0.tar", last modified: Sat Dec  9 16:40:46 2017, max compression
+gzip compressed data, was "dist\python-tds-1.9.1.tar", last modified: Sat Feb 10 02:16:48 2018, max compression
```

## Comparing `python-tds-1.9.0.tar` & `python-tds-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 denisenk (953893046) 1896053708        0 2017-12-09 16:40:46.000000 python-tds-1.9.0/
--rw-r--r--   0 denisenk (953893046) 1896053708       36 2017-12-09 16:05:35.000000 python-tds-1.9.0/test_requirements.txt
--rw-r--r--   0 denisenk (953893046) 1896053708      641 2017-12-09 16:40:46.000000 python-tds-1.9.0/PKG-INFO
--rw-r--r--   0 denisenk (953893046) 1896053708     2633 2017-07-16 17:30:45.000000 python-tds-1.9.0/version.py
--rw-r--r--   0 denisenk (953893046) 1896053708       11 2016-01-30 22:46:27.000000 python-tds-1.9.0/requirements.txt
--rw-r--r--   0 denisenk (953893046) 1896053708       74 2016-01-30 22:46:27.000000 python-tds-1.9.0/MANIFEST.in
--rw-r--r--   0 denisenk (953893046) 1896053708      905 2016-12-09 03:22:50.000000 python-tds-1.9.0/setup.py
--rw-r--r--   0 denisenk (953893046) 1896053708        6 2017-12-09 16:38:09.000000 python-tds-1.9.0/RELEASE-VERSION
--rw-r--r--   0 denisenk (953893046) 1896053708       38 2017-12-09 16:40:46.000000 python-tds-1.9.0/setup.cfg
--rw-r--r--   0 denisenk (953893046) 1896053708     2042 2017-12-09 16:29:38.000000 python-tds-1.9.0/README.rst
-drwxr-xr-x   0 denisenk (953893046) 1896053708        0 2017-12-09 16:40:46.000000 python-tds-1.9.0/pytds/
--rw-r--r--   0 denisenk (953893046) 1896053708     9587 2016-12-09 03:22:50.000000 python-tds-1.9.0/pytds/smp.py
--rw-r--r--   0 denisenk (953893046) 1896053708    18871 2016-01-30 22:46:27.000000 python-tds-1.9.0/pytds/lcid.py
--rw-r--r--   0 denisenk (953893046) 1896053708    10042 2016-12-09 03:22:50.000000 python-tds-1.9.0/pytds/collate.py
--rw-r--r--   0 denisenk (953893046) 1896053708    27514 2016-01-30 22:46:27.000000 python-tds-1.9.0/pytds/pyDes.py
--rw-r--r--   0 denisenk (953893046) 1896053708     1615 2016-12-09 03:22:50.000000 python-tds-1.9.0/pytds/tz.py
--rw-r--r--   0 denisenk (953893046) 1896053708    20485 2016-01-30 22:46:27.000000 python-tds-1.9.0/pytds/ntlm.py
--rw-r--r--   0 denisenk (953893046) 1896053708    67079 2017-12-09 16:00:40.000000 python-tds-1.9.0/pytds/tds.py
--rw-r--r--   0 denisenk (953893046) 1896053708    42367 2017-12-09 16:35:35.000000 python-tds-1.9.0/pytds/__init__.py
--rw-r--r--   0 denisenk (953893046) 1896053708    78479 2017-12-02 16:31:39.000000 python-tds-1.9.0/pytds/tds_types.py
--rw-r--r--   0 denisenk (953893046) 1896053708     3827 2017-12-09 16:00:40.000000 python-tds-1.9.0/pytds/tls.py
--rw-r--r--   0 denisenk (953893046) 1896053708      673 2016-04-30 14:10:21.000000 python-tds-1.9.0/pytds/extensions.py
--rw-r--r--   0 denisenk (953893046) 1896053708    15485 2016-12-09 03:22:50.000000 python-tds-1.9.0/pytds/sspi.py
--rw-r--r--   0 denisenk (953893046) 1896053708     3791 2016-12-09 03:22:50.000000 python-tds-1.9.0/pytds/login.py
--rw-r--r--   0 denisenk (953893046) 1896053708    15951 2017-12-09 16:00:40.000000 python-tds-1.9.0/pytds/tds_base.py
-drwxr-xr-x   0 denisenk (953893046) 1896053708        0 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/
--rw-r--r--   0 denisenk (953893046) 1896053708      641 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/PKG-INFO
--rw-r--r--   0 denisenk (953893046) 1896053708        1 2016-04-09 16:01:22.000000 python-tds-1.9.0/python_tds.egg-info/zip-safe
--rw-r--r--   0 denisenk (953893046) 1896053708      510 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/SOURCES.txt
--rw-r--r--   0 denisenk (953893046) 1896053708       11 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/requires.txt
--rw-r--r--   0 denisenk (953893046) 1896053708        6 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/top_level.txt
--rw-r--r--   0 denisenk (953893046) 1896053708        1 2017-12-09 16:40:46.000000 python-tds-1.9.0/python_tds.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2018-02-10 02:16:48.000000 python-tds-1.9.1/
+-rw-rw-rw-   0        0        0       75 2017-11-04 21:53:05.000000 python-tds-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      658 2018-02-10 02:16:48.000000 python-tds-1.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2018-02-10 02:16:48.000000 python-tds-1.9.1/pytds/
+-rw-rw-rw-   0        0        0    10317 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/collate.py
+-rw-rw-rw-   0        0        0      691 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/extensions.py
+-rw-rw-rw-   0        0        0    19376 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/lcid.py
+-rw-rw-rw-   0        0        0     3910 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/login.py
+-rw-rw-rw-   0        0        0    20956 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/ntlm.py
+-rw-rw-rw-   0        0        0    28366 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/pyDes.py
+-rw-rw-rw-   0        0        0     9842 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/smp.py
+-rw-rw-rw-   0        0        0    15931 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/sspi.py
+-rw-rw-rw-   0        0        0    68919 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/tds.py
+-rw-rw-rw-   0        0        0    16552 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/tds_base.py
+-rw-rw-rw-   0        0        0    81079 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/tds_types.py
+-rw-rw-rw-   0        0        0     4113 2018-02-10 01:57:15.000000 python-tds-1.9.1/pytds/tls.py
+-rw-rw-rw-   0        0        0     1693 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/tz.py
+-rw-rw-rw-   0        0        0    43589 2018-02-10 01:54:30.000000 python-tds-1.9.1/pytds/__init__.py
+drwxrwxrwx   0        0        0        0 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      658 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      510 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2018-02-10 02:16:48.000000 python-tds-1.9.1/python_tds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2018-02-10 02:05:27.000000 python-tds-1.9.1/python_tds.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     2118 2017-12-17 19:00:55.000000 python-tds-1.9.1/README.rst
+-rw-rw-rw-   0        0        0        7 2018-02-10 02:05:27.000000 python-tds-1.9.1/RELEASE-VERSION
+-rw-rw-rw-   0        0        0       12 2017-11-04 21:53:05.000000 python-tds-1.9.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2018-02-10 02:16:48.000000 python-tds-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      930 2018-02-10 01:54:30.000000 python-tds-1.9.1/setup.py
+-rw-rw-rw-   0        0        0       40 2018-02-10 01:54:30.000000 python-tds-1.9.1/test_requirements.txt
+-rw-rw-rw-   0        0        0     2733 2017-11-04 21:53:05.000000 python-tds-1.9.1/version.py
```

### Comparing `python-tds-1.9.0/PKG-INFO` & `python-tds-1.9.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 1.1
-Name: python-tds
-Version: 1.9.0
-Summary: Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation
-Home-page: https://github.com/denisenkom/pytds
-Author: Mikhail Denisenko
-Author-email: denisenkom@gmail.com
-License: MIT
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Metadata-Version: 1.1
+Name: python-tds
+Version: 1.9.1
+Summary: Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation
+Home-page: https://github.com/denisenkom/pytds
+Author: Mikhail Denisenko
+Author-email: denisenkom@gmail.com
+License: MIT
+Description-Content-Type: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
```

### Comparing `python-tds-1.9.0/version.py` & `python-tds-1.9.1/version.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-# -*- coding: utf-8 -*-
-# Author: Douglas Creager <dcreager@dcreager.net>
-# This file is placed into the public domain.
-
-# Calculates the current version number.  If possible, this is the
-# output of “git describe”, modified to conform to the versioning
-# scheme that setuptools uses.  If “git describe” returns an error
-# (most likely because we're in an unpacked copy of a release tarball,
-# rather than in a git working copy), then we fall back on reading the
-# contents of the RELEASE-VERSION file.
-#
-# To use this script, simply import it your setup.py file, and use the
-# results of get_git_version() as your package version:
-#
-# from version import *
-#
-# setup(
-#     version=get_git_version(),
-#     .
-#     .
-#     .
-# )
-#
-# This will automatically update the RELEASE-VERSION file, if
-# necessary.  Note that the RELEASE-VERSION file should *not* be
-# checked into git; please add it to your top-level .gitignore file.
-#
-# You'll probably want to distribute the RELEASE-VERSION file in your
-# sdist tarballs; to do this, just create a MANIFEST.in file that
-# contains the following line:
-#
-#   include RELEASE-VERSION
-
-__all__ = ("get_git_version")
-
-from subprocess import Popen, PIPE
-
-
-def call_git_describe(abbrev=4):
-    try:
-        p = Popen(['git', 'describe', '--abbrev=%d' % abbrev],
-                  stdout=PIPE, stderr=PIPE)
-        p.stderr.close()
-        line = p.stdout.readlines()[0]
-        return line.strip().decode('utf8')
-
-    except:
-        return None
-
-
-def read_release_version():
-    try:
-        f = open("RELEASE-VERSION", "rb")
-
-        try:
-            version = f.readlines()[0]
-            return version.strip().decode('utf8')
-
-        finally:
-            f.close()
-
-    except:
-        return None
-
-
-def write_release_version(version):
-    f = open("RELEASE-VERSION", "w")
-    f.write("%s\n" % version)
-    f.close()
-
-
-def get_git_version(abbrev=4):
-    # Read in the version that's currently in RELEASE-VERSION.
-
-    release_version = read_release_version()
-
-    # First try to get the current version using “git describe”.
-
-    version = call_git_describe(abbrev)
-
-    # If that doesn't work, fall back on the value that's in
-    # RELEASE-VERSION.
-
-    if version is None:
-        version = release_version
-
-    # If we still don't have anything, that's an error.
-
-    if version is None:
-        return 'unknown'
-
-    # If the current version is different from what's in the
-    # RELEASE-VERSION file, update the file to be current.
-
-    if version != release_version:
-        write_release_version(version)
-
-    # Finally, return the current version.
-
-    return version
+# -*- coding: utf-8 -*-
+# Author: Douglas Creager <dcreager@dcreager.net>
+# This file is placed into the public domain.
+
+# Calculates the current version number.  If possible, this is the
+# output of “git describe”, modified to conform to the versioning
+# scheme that setuptools uses.  If “git describe” returns an error
+# (most likely because we're in an unpacked copy of a release tarball,
+# rather than in a git working copy), then we fall back on reading the
+# contents of the RELEASE-VERSION file.
+#
+# To use this script, simply import it your setup.py file, and use the
+# results of get_git_version() as your package version:
+#
+# from version import *
+#
+# setup(
+#     version=get_git_version(),
+#     .
+#     .
+#     .
+# )
+#
+# This will automatically update the RELEASE-VERSION file, if
+# necessary.  Note that the RELEASE-VERSION file should *not* be
+# checked into git; please add it to your top-level .gitignore file.
+#
+# You'll probably want to distribute the RELEASE-VERSION file in your
+# sdist tarballs; to do this, just create a MANIFEST.in file that
+# contains the following line:
+#
+#   include RELEASE-VERSION
+
+__all__ = ("get_git_version")
+
+from subprocess import Popen, PIPE
+
+
+def call_git_describe(abbrev=4):
+    try:
+        p = Popen(['git', 'describe', '--abbrev=%d' % abbrev],
+                  stdout=PIPE, stderr=PIPE)
+        p.stderr.close()
+        line = p.stdout.readlines()[0]
+        return line.strip().decode('utf8')
+
+    except:
+        return None
+
+
+def read_release_version():
+    try:
+        f = open("RELEASE-VERSION", "rb")
+
+        try:
+            version = f.readlines()[0]
+            return version.strip().decode('utf8')
+
+        finally:
+            f.close()
+
+    except:
+        return None
+
+
+def write_release_version(version):
+    f = open("RELEASE-VERSION", "w")
+    f.write("%s\n" % version)
+    f.close()
+
+
+def get_git_version(abbrev=4):
+    # Read in the version that's currently in RELEASE-VERSION.
+
+    release_version = read_release_version()
+
+    # First try to get the current version using “git describe”.
+
+    version = call_git_describe(abbrev)
+
+    # If that doesn't work, fall back on the value that's in
+    # RELEASE-VERSION.
+
+    if version is None:
+        version = release_version
+
+    # If we still don't have anything, that's an error.
+
+    if version is None:
+        return 'unknown'
+
+    # If the current version is different from what's in the
+    # RELEASE-VERSION file, update the file to be current.
+
+    if version != release_version:
+        write_release_version(version)
+
+    # Finally, return the current version.
+
+    return version
```

### Comparing `python-tds-1.9.0/setup.py` & `python-tds-1.9.1/setup.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os
-from setuptools import setup
-import version
-
-requirements = list(open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), 'r').readlines())
-
-setup(name='python-tds',
-      version=version.get_git_version(),
-      description='Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation',
-      author='Mikhail Denisenko',
-      author_email='denisenkom@gmail.com',
-      url='https://github.com/denisenkom/pytds',
-      license="MIT",
-      packages=['pytds'],
-      classifiers=[
-          'Development Status :: 4 - Beta',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3.3',
-          'Programming Language :: Python :: 3.4',
-          'Programming Language :: Python :: 3.5',
-      ],
-      zip_safe=True,
-      install_requires=requirements,
-      )
+import os
+from setuptools import setup
+import version
+
+requirements = list(open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), 'r').readlines())
+
+setup(name='python-tds',
+      version=version.get_git_version(),
+      description='Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation',
+      author='Mikhail Denisenko',
+      author_email='denisenkom@gmail.com',
+      url='https://github.com/denisenkom/pytds',
+      license="MIT",
+      packages=['pytds'],
+      classifiers=[
+          'Development Status :: 4 - Beta',
+          'Programming Language :: Python',
+          'Programming Language :: Python :: 2.7',
+          'Programming Language :: Python :: 3.3',
+          'Programming Language :: Python :: 3.4',
+          'Programming Language :: Python :: 3.5',
+      ],
+      zip_safe=True,
+      install_requires=requirements,
+      )
```

### Comparing `python-tds-1.9.0/README.rst` & `python-tds-1.9.1/README.rst`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-pytds
-=====
-
-.. image:: https://secure.travis-ci.org/denisenkom/pytds.png?branch=master
-   :target: https://travis-ci.org/denisenkom/pytds
-
-.. image:: https://ci.appveyor.com/api/projects/status/a5h4y29063crqtet?svg=true
-   :target: https://ci.appveyor.com/project/denisenkom/pytds
-
-.. image:: http://img.shields.io/pypi/v/python-tds.svg
-   :target: https://pypi.python.org/pypi/python-tds/
-
-.. image:: https://codecov.io/gh/denisenkom/pytds/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/denisenkom/pytds
-
-
-`Python DBAPI`_ driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation.
-Doesn't depend on ADO or FreeTDS.  Can be used on any platform, including Linux, MacOS, Windows.
-
-It can be used with https://pypi.python.org/pypi/django-sqlserver as a Django database backend.
-
-Features
---------
-
-* Fully supports new MSSQL 2008 date types: datetime2, date, time, datetimeoffset
-* MARS
-* Bulk insert
-* Table-valued parameters
-* TLS connection encryption
-
-Installation
-------------
-
-To install run this command:
-
-.. code-block:: bash
-
-    $ pip install python-tds
-
-If you want to use TLS you should also install pyOpenSSL package:
-
-.. code-block:: bash
-
-   $ pip install pyOpenSSL
-
-For a better performance install bitarray package too:
-
-.. code-block:: bash
-
-    $ pip install bitarray
-
-Documentation
--------------
-Documentation is available at https://python-tds.readthedocs.io/en/latest/.
-
-Example
--------
-
-To connect to database do
-
-.. code-block:: python
-
-    import pytds
-    with pytds.connect('server', 'database', 'user', 'password') as conn:
-        with conn.cursor() as cur:
-            cur.execute("select 1")
-            cur.fetchall()
-
-
-To enable TLS you should also provide cafile parameter which should be a file name containing trusted CAs in PEM format.
-
-For detailed documentation of connection parameters see: `pytds.connect`_
-
-
-.. _Python DBAPI: http://legacy.python.org/dev/peps/pep-0249/
-.. _pytds.connect: https://python-tds.readthedocs.io/en/latest/pytds.html#pytds.connect
+pytds
+=====
+
+.. image:: https://secure.travis-ci.org/denisenkom/pytds.png?branch=master
+   :target: https://travis-ci.org/denisenkom/pytds
+
+.. image:: https://ci.appveyor.com/api/projects/status/a5h4y29063crqtet?svg=true
+   :target: https://ci.appveyor.com/project/denisenkom/pytds
+
+.. image:: http://img.shields.io/pypi/v/python-tds.svg
+   :target: https://pypi.python.org/pypi/python-tds/
+
+.. image:: https://codecov.io/gh/denisenkom/pytds/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/denisenkom/pytds
+
+
+`Python DBAPI`_ driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation.
+Doesn't depend on ADO or FreeTDS.  Can be used on any platform, including Linux, MacOS, Windows.
+
+It can be used with https://pypi.python.org/pypi/django-sqlserver as a Django database backend.
+
+Features
+--------
+
+* Fully supports new MSSQL 2008 date types: datetime2, date, time, datetimeoffset
+* MARS
+* Bulk insert
+* Table-valued parameters
+* TLS connection encryption
+
+Installation
+------------
+
+To install run this command:
+
+.. code-block:: bash
+
+    $ pip install python-tds
+
+If you want to use TLS you should also install pyOpenSSL package:
+
+.. code-block:: bash
+
+   $ pip install pyOpenSSL
+
+For a better performance install bitarray package too:
+
+.. code-block:: bash
+
+    $ pip install bitarray
+
+Documentation
+-------------
+Documentation is available at https://python-tds.readthedocs.io/en/latest/.
+
+Example
+-------
+
+To connect to database do
+
+.. code-block:: python
+
+    import pytds
+    with pytds.connect('server', 'database', 'user', 'password') as conn:
+        with conn.cursor() as cur:
+            cur.execute("select 1")
+            cur.fetchall()
+
+
+To enable TLS you should also provide cafile parameter which should be a file name containing trusted CAs in PEM format.
+
+For detailed documentation of connection parameters see: `pytds.connect`_
+
+
+.. _Python DBAPI: http://legacy.python.org/dev/peps/pep-0249/
+.. _pytds.connect: https://python-tds.readthedocs.io/en/latest/pytds.html#pytds.connect
```

### Comparing `python-tds-1.9.0/pytds/smp.py` & `python-tds-1.9.1/pytds/smp.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import struct
-import logging
-import threading
-import socket
-import errno
-from six.moves import range
-try:
-    from bitarray import bitarray
-except ImportError:
-    class BitArray(list):
-        def __init__(self, size):
-            super(BitArray, self).__init__()
-            self[:] = [False] * size
-
-        def setall(self, val):
-            for i in range(len(self)):
-                self[i] = val
-
-    bitarray = BitArray
-from .tds_base import Error, readall, skipall
-
-
-logger = logging.getLogger(__name__)
-
-
-class _SmpSession(object):
-    def __init__(self, mgr, session_id):
-        self.session_id = session_id
-        self.seq_num_for_send = 0
-        self.high_water_for_send = 4
-        self._seq_num_for_recv = 0
-        self.high_water_for_recv = 4
-        self._last_high_water_for_recv = 4
-        self._mgr = mgr
-        self.recv_queue = []
-        self.send_queue = []
-        self.state = 'new'
-        self._curr_buf_pos = 0
-        self._curr_buf = b''
-
-    def __repr__(self):
-        fmt = "<_SmpSession sid={} state={} recv_queue={} send_queue={} seq_num_for_send={}>"
-        return fmt.format(self.session_id, self.state, self.recv_queue, self.send_queue,
-                          self.seq_num_for_send)
-
-    def close(self):
-        self._mgr.close_smp_session(self)
-
-    def send(self, data, final):
-        self._mgr.send_packet(self, data)
-
-    def read(self, size):
-        if not self._curr_buf[self._curr_buf_pos:]:
-            self._curr_buf = self._mgr.recv_packet(self)
-            self._curr_buf_pos = 0
-            if not self._curr_buf:
-                return b''
-        res = self._curr_buf[self._curr_buf_pos:self._curr_buf_pos + size]
-        self._curr_buf_pos += len(res)
-        return res
-
-    def is_connected(self):
-        return self.state == 'SESSION ESTABLISHED'
-
-
-class SmpManager(object):
-    _smid = 0x53
-    _smp_header = struct.Struct('<BBHLLL')
-    _SYN = 0x1
-    _ACK = 0x2
-    _FIN = 0x4
-    _DATA = 0x8
-
-    def __init__(self, transport):
-        self._transport = transport
-        self._sessions = {}
-        self._used_ids_ba = bitarray(2 ** 16)
-        self._used_ids_ba.setall(False)
-        self._lock = threading.RLock()
-
-    def __repr__(self):
-        return "<SmpManager sessions={}>".format(self._sessions)
-
-    def create_session(self):
-        try:
-            session_id = self._used_ids_ba.index(False)
-        except ValueError:
-            raise Error("Can't create more MARS sessions, close some sessions and try again")
-        session = _SmpSession(self, session_id)
-        with self._lock:
-            self._sessions[session_id] = session
-            self._used_ids_ba[session_id] = True
-            hdr = self._smp_header.pack(
-                self._smid,
-                self._SYN,
-                session_id,
-                self._smp_header.size,
-                0,
-                session.high_water_for_recv,
-                )
-            self._transport.send(hdr, True)
-            session.state = 'SESSION ESTABLISHED'
-        return session
-
-    def close_smp_session(self, session):
-        if session.state in ('CLOSED', 'FIN SENT'):
-            return
-        elif session.state == 'SESSION ESTABLISHED':
-            with self._lock:
-                if self._transport.is_connected():
-                    hdr = self._smp_header.pack(
-                        self._smid,
-                        self._FIN,
-                        session.session_id,
-                        self._smp_header.size,
-                        session.seq_num_for_send,
-                        session.high_water_for_recv,
-                        )
-                    session.state = 'FIN SENT'
-                    try:
-                        self._transport.send(hdr, True)
-                        self.recv_packet(session)
-                    except (socket.error, OSError) as ex:
-                        if ex.errno in (errno.ECONNRESET, errno.EPIPE):
-                            session.state = 'CLOSED'
-                        else:
-                            raise ex
-                else:
-                    session.state = 'CLOSED'
-
-    def send_queued_packets(self, session):
-        with self._lock:
-            while session.send_queue and session.seq_num_for_send < session.high_water_for_send:
-                data = session.send_queue.pop(0)
-                self.send_packet(session, data)
-
-    @staticmethod
-    def _add_one_wrap(val):
-        return 0 if val == 2 ** 32 - 1 else val + 1
-
-    def send_packet(self, session, data):
-        with self._lock:
-            if session.seq_num_for_send < session.high_water_for_send:
-                l = self._smp_header.size + len(data)
-                seq_num = self._add_one_wrap(session.seq_num_for_send)
-                hdr = self._smp_header.pack(
-                    self._smid,
-                    self._DATA,
-                    session.session_id,
-                    l,
-                    seq_num,
-                    session.high_water_for_recv,
-                    )
-                session._last_high_water_for_recv = session.high_water_for_recv
-                self._transport.send(hdr + data, True)
-                session.seq_num_for_send = self._add_one_wrap(session.seq_num_for_send)
-            else:
-                session.send_queue.append(data)
-                self._read_smp_message()
-
-    def recv_packet(self, session):
-        with self._lock:
-            if session.state == 'CLOSED':
-                return b''
-            while not session.recv_queue:
-                self._read_smp_message()
-                if session.state in ('CLOSED', 'FIN RECEIVED'):
-                    return b''
-            session.high_water_for_recv = self._add_one_wrap(session.high_water_for_recv)
-            if session.high_water_for_recv - session._last_high_water_for_recv >= 2:
-                hdr = self._smp_header.pack(
-                    self._smid,
-                    self._ACK,
-                    session.session_id,
-                    self._smp_header.size,
-                    session.seq_num_for_send,
-                    session.high_water_for_recv,
-                    )
-                self._transport.send(hdr, True)
-                session._last_high_water_for_recv = session.high_water_for_recv
-            return session.recv_queue.pop(0)
-
-    @classmethod
-    def _type_to_str(cls, t):
-        if t == cls._SYN:
-            return 'SYN'
-        elif t == cls._ACK:
-            return 'ACK'
-        elif t == cls._DATA:
-            return 'DATA'
-        elif t == cls._FIN:
-            return 'FIN'
-
-    def _bad_stm(self, message):
-        self.close()
-        raise Error(message)
-
-    def _read_smp_message(self):
-        with self._lock:
-            smid, flags, sid, l, seq_num, wnd = self._smp_header.unpack(readall(self._transport, self._smp_header.size))
-            if smid != self._smid:
-                self._bad_stm('Invalid SMP packet signature')
-            try:
-                session = self._sessions[sid]
-            except KeyError:
-                self._bad_stm('Invalid SMP packet session id')
-            if wnd < session.high_water_for_send:
-                self._bad_stm('Invalid WNDW in packet from server')
-            if seq_num > session.high_water_for_recv:
-                self._bad_stm('Invalid SEQNUM in packet from server')
-            session._last_recv_seq_num = seq_num
-            if flags == self._ACK:
-                if session.state in ('FIN RECEIVED', 'CLOSED'):
-                    self._bad_stm('Unexpected SMP ACK packet from server')
-                if seq_num != session._seq_num_for_recv:
-                    self._bad_stm('Invalid SEQNUM in ACK packet from server')
-                session.high_water_for_send = wnd
-                self.send_queued_packets(session)
-            elif flags == self._DATA:
-                if session.state == 'SESSION ESTABLISHED':
-                    if seq_num != self._add_one_wrap(session._seq_num_for_recv):
-                        self._bad_stm('Invalid SEQNUM in ACK packet from server')
-                    session._seq_num_for_recv = seq_num
-                    data = readall(self._transport, l - self._smp_header.size)
-                    session.recv_queue.append(data)
-                    if wnd > session.high_water_for_send:
-                        session.high_water_for_send = wnd
-                        self.send_queued_packets(session)
-
-                elif session.state == 'FIN SENT':
-                    skipall(self._transport, l - self._smp_header.size)
-                else:
-                    self._bad_stm('Unexpected DATA packet from server')
-            elif flags == self._FIN:
-                if session.state == 'SESSION ESTABLISHED':
-                    session.state = 'FIN RECEIVED'
-                elif session.state == 'FIN SENT':
-                    session.state = 'CLOSED'
-                    del self._sessions[session.session_id]
-                    self._used_ids_ba[session.session_id] = False
-                elif session.state == 'FIN RECEIVED':
-                    self._bad_stm('Unexpected SMP FIN packet from server')
-                else:
-                    self._bad_stm('Invalid state: ' + session.state)
-            elif flags == self._SYN:
-                self._bad_stm('Unexpected SMP SYN packet from server')
-            else:
-                self._bad_stm('Unexpected SMP flags in packet from server')
-
-    def close(self):
-        self._transport.close()
-
-    def transport_closed(self):
-        for session in self._sessions.values():
-            session.state = 'CLOSED'
+import struct
+import logging
+import threading
+import socket
+import errno
+from six.moves import range
+try:
+    from bitarray import bitarray
+except ImportError:
+    class BitArray(list):
+        def __init__(self, size):
+            super(BitArray, self).__init__()
+            self[:] = [False] * size
+
+        def setall(self, val):
+            for i in range(len(self)):
+                self[i] = val
+
+    bitarray = BitArray
+from .tds_base import Error, readall, skipall
+
+
+logger = logging.getLogger(__name__)
+
+
+class _SmpSession(object):
+    def __init__(self, mgr, session_id):
+        self.session_id = session_id
+        self.seq_num_for_send = 0
+        self.high_water_for_send = 4
+        self._seq_num_for_recv = 0
+        self.high_water_for_recv = 4
+        self._last_high_water_for_recv = 4
+        self._mgr = mgr
+        self.recv_queue = []
+        self.send_queue = []
+        self.state = 'new'
+        self._curr_buf_pos = 0
+        self._curr_buf = b''
+
+    def __repr__(self):
+        fmt = "<_SmpSession sid={} state={} recv_queue={} send_queue={} seq_num_for_send={}>"
+        return fmt.format(self.session_id, self.state, self.recv_queue, self.send_queue,
+                          self.seq_num_for_send)
+
+    def close(self):
+        self._mgr.close_smp_session(self)
+
+    def send(self, data, final):
+        self._mgr.send_packet(self, data)
+
+    def read(self, size):
+        if not self._curr_buf[self._curr_buf_pos:]:
+            self._curr_buf = self._mgr.recv_packet(self)
+            self._curr_buf_pos = 0
+            if not self._curr_buf:
+                return b''
+        res = self._curr_buf[self._curr_buf_pos:self._curr_buf_pos + size]
+        self._curr_buf_pos += len(res)
+        return res
+
+    def is_connected(self):
+        return self.state == 'SESSION ESTABLISHED'
+
+
+class SmpManager(object):
+    _smid = 0x53
+    _smp_header = struct.Struct('<BBHLLL')
+    _SYN = 0x1
+    _ACK = 0x2
+    _FIN = 0x4
+    _DATA = 0x8
+
+    def __init__(self, transport):
+        self._transport = transport
+        self._sessions = {}
+        self._used_ids_ba = bitarray(2 ** 16)
+        self._used_ids_ba.setall(False)
+        self._lock = threading.RLock()
+
+    def __repr__(self):
+        return "<SmpManager sessions={}>".format(self._sessions)
+
+    def create_session(self):
+        try:
+            session_id = self._used_ids_ba.index(False)
+        except ValueError:
+            raise Error("Can't create more MARS sessions, close some sessions and try again")
+        session = _SmpSession(self, session_id)
+        with self._lock:
+            self._sessions[session_id] = session
+            self._used_ids_ba[session_id] = True
+            hdr = self._smp_header.pack(
+                self._smid,
+                self._SYN,
+                session_id,
+                self._smp_header.size,
+                0,
+                session.high_water_for_recv,
+                )
+            self._transport.send(hdr, True)
+            session.state = 'SESSION ESTABLISHED'
+        return session
+
+    def close_smp_session(self, session):
+        if session.state in ('CLOSED', 'FIN SENT'):
+            return
+        elif session.state == 'SESSION ESTABLISHED':
+            with self._lock:
+                if self._transport.is_connected():
+                    hdr = self._smp_header.pack(
+                        self._smid,
+                        self._FIN,
+                        session.session_id,
+                        self._smp_header.size,
+                        session.seq_num_for_send,
+                        session.high_water_for_recv,
+                        )
+                    session.state = 'FIN SENT'
+                    try:
+                        self._transport.send(hdr, True)
+                        self.recv_packet(session)
+                    except (socket.error, OSError) as ex:
+                        if ex.errno in (errno.ECONNRESET, errno.EPIPE):
+                            session.state = 'CLOSED'
+                        else:
+                            raise ex
+                else:
+                    session.state = 'CLOSED'
+
+    def send_queued_packets(self, session):
+        with self._lock:
+            while session.send_queue and session.seq_num_for_send < session.high_water_for_send:
+                data = session.send_queue.pop(0)
+                self.send_packet(session, data)
+
+    @staticmethod
+    def _add_one_wrap(val):
+        return 0 if val == 2 ** 32 - 1 else val + 1
+
+    def send_packet(self, session, data):
+        with self._lock:
+            if session.seq_num_for_send < session.high_water_for_send:
+                l = self._smp_header.size + len(data)
+                seq_num = self._add_one_wrap(session.seq_num_for_send)
+                hdr = self._smp_header.pack(
+                    self._smid,
+                    self._DATA,
+                    session.session_id,
+                    l,
+                    seq_num,
+                    session.high_water_for_recv,
+                    )
+                session._last_high_water_for_recv = session.high_water_for_recv
+                self._transport.send(hdr + data, True)
+                session.seq_num_for_send = self._add_one_wrap(session.seq_num_for_send)
+            else:
+                session.send_queue.append(data)
+                self._read_smp_message()
+
+    def recv_packet(self, session):
+        with self._lock:
+            if session.state == 'CLOSED':
+                return b''
+            while not session.recv_queue:
+                self._read_smp_message()
+                if session.state in ('CLOSED', 'FIN RECEIVED'):
+                    return b''
+            session.high_water_for_recv = self._add_one_wrap(session.high_water_for_recv)
+            if session.high_water_for_recv - session._last_high_water_for_recv >= 2:
+                hdr = self._smp_header.pack(
+                    self._smid,
+                    self._ACK,
+                    session.session_id,
+                    self._smp_header.size,
+                    session.seq_num_for_send,
+                    session.high_water_for_recv,
+                    )
+                self._transport.send(hdr, True)
+                session._last_high_water_for_recv = session.high_water_for_recv
+            return session.recv_queue.pop(0)
+
+    @classmethod
+    def _type_to_str(cls, t):
+        if t == cls._SYN:
+            return 'SYN'
+        elif t == cls._ACK:
+            return 'ACK'
+        elif t == cls._DATA:
+            return 'DATA'
+        elif t == cls._FIN:
+            return 'FIN'
+
+    def _bad_stm(self, message):
+        self.close()
+        raise Error(message)
+
+    def _read_smp_message(self):
+        with self._lock:
+            smid, flags, sid, l, seq_num, wnd = self._smp_header.unpack(readall(self._transport, self._smp_header.size))
+            if smid != self._smid:
+                self._bad_stm('Invalid SMP packet signature')
+            try:
+                session = self._sessions[sid]
+            except KeyError:
+                self._bad_stm('Invalid SMP packet session id')
+            if wnd < session.high_water_for_send:
+                self._bad_stm('Invalid WNDW in packet from server')
+            if seq_num > session.high_water_for_recv:
+                self._bad_stm('Invalid SEQNUM in packet from server')
+            session._last_recv_seq_num = seq_num
+            if flags == self._ACK:
+                if session.state in ('FIN RECEIVED', 'CLOSED'):
+                    self._bad_stm('Unexpected SMP ACK packet from server')
+                if seq_num != session._seq_num_for_recv:
+                    self._bad_stm('Invalid SEQNUM in ACK packet from server')
+                session.high_water_for_send = wnd
+                self.send_queued_packets(session)
+            elif flags == self._DATA:
+                if session.state == 'SESSION ESTABLISHED':
+                    if seq_num != self._add_one_wrap(session._seq_num_for_recv):
+                        self._bad_stm('Invalid SEQNUM in ACK packet from server')
+                    session._seq_num_for_recv = seq_num
+                    data = readall(self._transport, l - self._smp_header.size)
+                    session.recv_queue.append(data)
+                    if wnd > session.high_water_for_send:
+                        session.high_water_for_send = wnd
+                        self.send_queued_packets(session)
+
+                elif session.state == 'FIN SENT':
+                    skipall(self._transport, l - self._smp_header.size)
+                else:
+                    self._bad_stm('Unexpected DATA packet from server')
+            elif flags == self._FIN:
+                if session.state == 'SESSION ESTABLISHED':
+                    session.state = 'FIN RECEIVED'
+                elif session.state == 'FIN SENT':
+                    session.state = 'CLOSED'
+                    del self._sessions[session.session_id]
+                    self._used_ids_ba[session.session_id] = False
+                elif session.state == 'FIN RECEIVED':
+                    self._bad_stm('Unexpected SMP FIN packet from server')
+                else:
+                    self._bad_stm('Invalid state: ' + session.state)
+            elif flags == self._SYN:
+                self._bad_stm('Unexpected SMP SYN packet from server')
+            else:
+                self._bad_stm('Unexpected SMP flags in packet from server')
+
+    def close(self):
+        self._transport.close()
+
+    def transport_closed(self):
+        for session in self._sessions.values():
+            session.state = 'CLOSED'
```

### Comparing `python-tds-1.9.0/pytds/lcid.py` & `python-tds-1.9.1/pytds/lcid.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,505 +1,505 @@
-# Copyright 2010 Michael Murr
-#
-# This file is part of LibForensics.
-#
-# LibForensics is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# LibForensics is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with LibForensics.  If not, see <http://www.gnu.org/licenses/>.
-
-"""Constants for Locale IDs. (LCIDs)"""
-
-__docformat__ = "restructuredtext en"
-__all__ = [
-    "LANGID_AFRIKAANS", "LANGID_ALBANIAN", "LANGID_AMHARIC", "LANGID_ARABIC",
-    "LANGID_ARABIC_ALGERIA", "LANGID_ARABIC_BAHRAIN", "LANGID_ARABIC_EGYPT",
-    "LANGID_ARABIC_IRAQ", "LANGID_ARABIC_JORDAN", "LANGID_ARABIC_KUWAIT",
-    "LANGID_ARABIC_LEBANON", "LANGID_ARABIC_LIBYA", "LANGID_ARABIC_MOROCCO",
-    "LANGID_ARABIC_OMAN", "LANGID_ARABIC_QATAR", "LANGID_ARABIC_SYRIA",
-    "LANGID_ARABIC_TUNISIA", "LANGID_ARABIC_UAE", "LANGID_ARABIC_YEMEN",
-    "LANGID_ARMENIAN", "LANGID_ASSAMESE", "LANGID_AZERI_CYRILLIC",
-    "LANGID_AZERI_LATIN", "LANGID_BASQUE", "LANGID_BELGIAN_DUTCH",
-    "LANGID_BELGIAN_FRENCH", "LANGID_BENGALI", "LANGID_BULGARIAN",
-    "LANGID_BURMESE", "LANGID_BYELORUSSIAN", "LANGID_CATALAN",
-    "LANGID_CHEROKEE", "LANGID_CHINESE_HONG_KONG_SAR",
-    "LANGID_CHINESE_MACAO_SAR", "LANGID_CHINESE_SINGAPORE", "LANGID_CROATIAN",
-    "LANGID_CZECH", "LANGID_DANISH", "LANGID_DIVEHI", "LANGID_DUTCH",
-    "LANGID_EDO", "LANGID_ENGLISH_AUS", "LANGID_ENGLISH_BELIZE",
-    "LANGID_ENGLISH_CANADIAN", "LANGID_ENGLISH_CARIBBEAN",
-    "LANGID_ENGLISH_INDONESIA", "LANGID_ENGLISH_IRELAND",
-    "LANGID_ENGLISH_JAMAICA", "LANGID_ENGLISH_NEW_ZEALAND",
-    "LANGID_ENGLISH_PHILIPPINES", "LANGID_ENGLISH_SOUTH_AFRICA",
-    "LANGID_ENGLISH_TRINIDAD_TOBAGO", "LANGID_ENGLISH_UK", "LANGID_ENGLISH_US",
-    "LANGID_ENGLISH_ZIMBABWE", "LANGID_ESTONIAN", "LANGID_FAEROESE",
-    "LANGID_FILIPINO", "LANGID_FINNISH", "LANGID_FRENCH",
-    "LANGID_FRENCH_CAMEROON", "LANGID_FRENCH_CANADIAN",
-    "LANGID_FRENCH_CONGO_D_R_C", "LANGID_FRENCH_COTED_IVOIRE",
-    "LANGID_FRENCH_HAITI", "LANGID_FRENCH_LUXEMBOURG", "LANGID_FRENCH_MALI",
-    "LANGID_FRENCH_MONACO", "LANGID_FRENCH_MOROCCO", "LANGID_FRENCH_REUNION",
-    "LANGID_FRENCH_SENEGAL", "LANGID_FRENCH_WEST_INDIES",
-    "LANGID_FRISIAN_NETHERLANDS", "LANGID_FULFULDE", "LANGID_GAELIC_IRELAND",
-    "LANGID_GAELIC_SCOTLAND", "LANGID_GALICIAN", "LANGID_GEORGIAN",
-    "LANGID_GERMAN", "LANGID_GERMAN_AUSTRIA", "LANGID_GERMAN_LIECHTENSTEIN",
-    "LANGID_GERMAN_LUXEMBOURG", "LANGID_GREEK", "LANGID_GUARANI",
-    "LANGID_GUJARATI", "LANGID_HAUSA", "LANGID_HAWAIIAN", "LANGID_HEBREW",
-    "LANGID_HINDI", "LANGID_HUNGARIAN", "LANGID_IBIBIO", "LANGID_ICELANDIC",
-    "LANGID_IGBO", "LANGID_INDONESIAN", "LANGID_INUKTITUT", "LANGID_ITALIAN",
-    "LANGID_JAPANESE", "LANGID_KANNADA", "LANGID_KANURI", "LANGID_KASHMIRI",
-    "LANGID_KAZAKH", "LANGID_KHMER", "LANGID_KIRGHIZ", "LANGID_KONKANI",
-    "LANGID_KOREAN", "LANGID_KYRGYZ", "LANGID_LANGUAGE_NONE", "LANGID_LAO",
-    "LANGID_LATIN", "LANGID_LATVIAN", "LANGID_LITHUANIAN",
-    "LANGID_MACEDONIAN_FYROM", "LANGID_MALAYALAM", "LANGID_MALAYSIAN",
-    "LANGID_MALAY_BRUNEI_DARUSSALAM", "LANGID_MALTESE", "LANGID_MANIPURI",
-    "LANGID_MARATHI", "LANGID_MEXICAN_SPANISH", "LANGID_MONGOLIAN",
-    "LANGID_NEPALI", "LANGID_NORWEGIAN_BOKMOL", "LANGID_NORWEGIAN_NYNORSK",
-    "LANGID_NO_PROOFING", "LANGID_ORIYA", "LANGID_OROMO", "LANGID_PASHTO",
-    "LANGID_PERSIAN", "LANGID_POLISH", "LANGID_PORTUGUESE",
-    "LANGID_PORTUGUESE_BRAZIL", "LANGID_PUNJABI", "LANGID_RHAETO_ROMANIC",
-    "LANGID_ROMANIAN", "LANGID_ROMANIAN_MOLDOVA", "LANGID_RUSSIAN",
-    "LANGID_RUSSIAN_MOLDOVA", "LANGID_SAMI_LAPPISH", "LANGID_SANSKRIT",
-    "LANGID_SERBIAN_CYRILLIC", "LANGID_SERBIAN_LATIN", "LANGID_SESOTHO",
-    "LANGID_SIMPLIFIED_CHINESE", "LANGID_SINDHI", "LANGID_SINDHI_PAKISTAN",
-    "LANGID_SINHALESE", "LANGID_SLOVAK", "LANGID_SLOVENIAN", "LANGID_SOMALI",
-    "LANGID_SORBIAN", "LANGID_SPANISH", "LANGID_SPANISH_ARGENTINA",
-    "LANGID_SPANISH_BOLIVIA", "LANGID_SPANISH_CHILE",
-    "LANGID_SPANISH_COLOMBIA", "LANGID_SPANISH_COSTA_RICA",
-    "LANGID_SPANISH_DOMINICAN_REPUBLIC", "LANGID_SPANISH_ECUADOR",
-    "LANGID_SPANISH_EL_SALVADOR", "LANGID_SPANISH_GUATEMALA",
-    "LANGID_SPANISH_HONDURAS", "LANGID_SPANISH_MODERN_SORT",
-    "LANGID_SPANISH_NICARAGUA", "LANGID_SPANISH_PANAMA",
-    "LANGID_SPANISH_PARAGUAY", "LANGID_SPANISH_PERU",
-    "LANGID_SPANISH_PUERTO_RICO", "LANGID_SPANISH_URUGUAY",
-    "LANGID_SPANISH_VENEZUELA", "LANGID_SUTU", "LANGID_SWAHILI",
-    "LANGID_SWEDISH", "LANGID_SWEDISH_FINLAND", "LANGID_SWISS_FRENCH",
-    "LANGID_SWISS_GERMAN", "LANGID_SWISS_ITALIAN", "LANGID_SYRIAC",
-    "LANGID_TAJIK", "LANGID_TAMAZIGHT", "LANGID_TAMAZIGHT_LATIN",
-    "LANGID_TAMIL", "LANGID_TATAR", "LANGID_TELUGU", "LANGID_THAI",
-    "LANGID_TIBETAN", "LANGID_TIGRIGNA_ERITREA", "LANGID_TIGRIGNA_ETHIOPIC",
-    "LANGID_TRADITIONAL_CHINESE", "LANGID_TSONGA", "LANGID_TSWANA",
-    "LANGID_TURKISH", "LANGID_TURKMEN", "LANGID_UKRAINIAN", "LANGID_URDU",
-    "LANGID_UZBEK_CYRILLIC", "LANGID_UZBEK_LATIN", "LANGID_VENDA",
-    "LANGID_VIETNAMESE", "LANGID_WELSH", "LANGID_XHOSA", "LANGID_YI",
-    "LANGID_YIDDISH", "LANGID_YORUBA", "LANGID_ZULU",
-
-    "lang_id_names"
-]
-
-LANGID_AFRIKAANS = 1078
-LANGID_ALBANIAN = 1052
-LANGID_AMHARIC = 1118
-LANGID_ARABIC = 1025
-LANGID_ARABIC_ALGERIA = 5121
-LANGID_ARABIC_BAHRAIN = 15361
-LANGID_ARABIC_EGYPT = 3073
-LANGID_ARABIC_IRAQ = 2049
-LANGID_ARABIC_JORDAN = 11265
-LANGID_ARABIC_KUWAIT = 13313
-LANGID_ARABIC_LEBANON = 12289
-LANGID_ARABIC_LIBYA = 4097
-LANGID_ARABIC_MOROCCO = 6145
-LANGID_ARABIC_OMAN = 8193
-LANGID_ARABIC_QATAR = 16385
-LANGID_ARABIC_SYRIA = 10241
-LANGID_ARABIC_TUNISIA = 7169
-LANGID_ARABIC_UAE = 14337
-LANGID_ARABIC_YEMEN = 9217
-LANGID_ARMENIAN = 1067
-LANGID_ASSAMESE = 1101
-LANGID_AZERI_CYRILLIC = 2092
-LANGID_AZERI_LATIN = 1068
-LANGID_BASQUE = 1069
-LANGID_BELGIAN_DUTCH = 2067
-LANGID_BELGIAN_FRENCH = 2060
-LANGID_BENGALI = 1093
-LANGID_BULGARIAN = 1026
-LANGID_BURMESE = 1109
-LANGID_BYELORUSSIAN = 1059
-LANGID_CATALAN = 1027
-LANGID_CHEROKEE = 1116
-LANGID_CHINESE_HONG_KONG_SAR = 3076
-LANGID_CHINESE_MACAO_SAR = 5124
-LANGID_CHINESE_SINGAPORE = 4100
-LANGID_CROATIAN = 1050
-LANGID_CZECH = 1029
-LANGID_DANISH = 1030
-LANGID_DIVEHI = 1125
-LANGID_DUTCH = 1043
-LANGID_EDO = 1126
-LANGID_ENGLISH_AUS = 3081
-LANGID_ENGLISH_BELIZE = 10249
-LANGID_ENGLISH_CANADIAN = 4105
-LANGID_ENGLISH_CARIBBEAN = 9225
-LANGID_ENGLISH_INDONESIA = 14345
-LANGID_ENGLISH_IRELAND = 6153
-LANGID_ENGLISH_JAMAICA = 8201
-LANGID_ENGLISH_NEW_ZEALAND = 5129
-LANGID_ENGLISH_PHILIPPINES = 13321
-LANGID_ENGLISH_SOUTH_AFRICA = 7177
-LANGID_ENGLISH_TRINIDAD_TOBAGO = 11273
-LANGID_ENGLISH_UK = 2057
-LANGID_ENGLISH_US = 1033
-LANGID_ENGLISH_ZIMBABWE = 12297
-LANGID_ESTONIAN = 1061
-LANGID_FAEROESE = 1080
-LANGID_FILIPINO = 1124
-LANGID_FINNISH = 1035
-LANGID_FRENCH = 1036
-LANGID_FRENCH_CAMEROON = 11276
-LANGID_FRENCH_CANADIAN = 3084
-LANGID_FRENCH_CONGO_D_R_C = 9228
-LANGID_FRENCH_COTED_IVOIRE = 12300
-LANGID_FRENCH_HAITI = 15372
-LANGID_FRENCH_LUXEMBOURG = 5132
-LANGID_FRENCH_MALI = 13324
-LANGID_FRENCH_MONACO = 6156
-LANGID_FRENCH_MOROCCO = 14348
-LANGID_FRENCH_REUNION = 8204
-LANGID_FRENCH_SENEGAL = 10252
-LANGID_FRENCH_WEST_INDIES = 7180
-LANGID_FRISIAN_NETHERLANDS = 1122
-LANGID_FULFULDE = 1127
-LANGID_GAELIC_IRELAND = 2108
-LANGID_GAELIC_SCOTLAND = 1084
-LANGID_GALICIAN = 1110
-LANGID_GEORGIAN = 1079
-LANGID_GERMAN = 1031
-LANGID_GERMAN_AUSTRIA = 3079
-LANGID_GERMAN_LIECHTENSTEIN = 5127
-LANGID_GERMAN_LUXEMBOURG = 4103
-LANGID_GREEK = 1032
-LANGID_GUARANI = 1140
-LANGID_GUJARATI = 1095
-LANGID_HAUSA = 1128
-LANGID_HAWAIIAN = 1141
-LANGID_HEBREW = 1037
-LANGID_HINDI = 1081
-LANGID_HUNGARIAN = 1038
-LANGID_IBIBIO = 1129
-LANGID_ICELANDIC = 1039
-LANGID_IGBO = 1136
-LANGID_INDONESIAN = 1057
-LANGID_INUKTITUT = 1117
-LANGID_ITALIAN = 1040
-LANGID_JAPANESE = 1041
-LANGID_KANNADA = 1099
-LANGID_KANURI = 1137
-LANGID_KASHMIRI = 1120
-LANGID_KAZAKH = 1087
-LANGID_KHMER = 1107
-LANGID_KIRGHIZ = 1088
-LANGID_KONKANI = 1111
-LANGID_KOREAN = 1042
-LANGID_KYRGYZ = 1088
-LANGID_LANGUAGE_NONE = 0
-LANGID_LAO = 1108
-LANGID_LATIN = 1142
-LANGID_LATVIAN = 1062
-LANGID_LITHUANIAN = 1063
-LANGID_MACEDONIAN_FYROM = 1071
-LANGID_MALAYALAM = 1100
-LANGID_MALAY_BRUNEI_DARUSSALAM = 2110
-LANGID_MALAYSIAN = 1086
-LANGID_MALTESE = 1082
-LANGID_MANIPURI = 1112
-LANGID_MARATHI = 1102
-LANGID_MEXICAN_SPANISH = 2058
-LANGID_MONGOLIAN = 1104
-LANGID_NEPALI = 1121
-LANGID_NO_PROOFING = 1024
-LANGID_NORWEGIAN_BOKMOL = 1044
-LANGID_NORWEGIAN_NYNORSK = 2068
-LANGID_ORIYA = 1096
-LANGID_OROMO = 1138
-LANGID_PASHTO = 1123
-LANGID_PERSIAN = 1065
-LANGID_POLISH = 1045
-LANGID_PORTUGUESE = 2070
-LANGID_PORTUGUESE_BRAZIL = 1046
-LANGID_PUNJABI = 1094
-LANGID_RHAETO_ROMANIC = 1047
-LANGID_ROMANIAN = 1048
-LANGID_ROMANIAN_MOLDOVA = 2072
-LANGID_RUSSIAN = 1049
-LANGID_RUSSIAN_MOLDOVA = 2073
-LANGID_SAMI_LAPPISH = 1083
-LANGID_SANSKRIT = 1103
-LANGID_SERBIAN_CYRILLIC = 3098
-LANGID_SERBIAN_LATIN = 2074
-LANGID_SESOTHO = 1072
-LANGID_SIMPLIFIED_CHINESE = 2052
-LANGID_SINDHI = 1113
-LANGID_SINDHI_PAKISTAN = 2137
-LANGID_SINHALESE = 1115
-LANGID_SLOVAK = 1051
-LANGID_SLOVENIAN = 1060
-LANGID_SOMALI = 1143
-LANGID_SORBIAN = 1070
-LANGID_SPANISH = 1034
-LANGID_SPANISH_ARGENTINA = 11274
-LANGID_SPANISH_BOLIVIA = 16394
-LANGID_SPANISH_CHILE = 13322
-LANGID_SPANISH_COLOMBIA = 9226
-LANGID_SPANISH_COSTA_RICA = 5130
-LANGID_SPANISH_DOMINICAN_REPUBLIC = 7178
-LANGID_SPANISH_ECUADOR = 12298
-LANGID_SPANISH_EL_SALVADOR = 17418
-LANGID_SPANISH_GUATEMALA = 4106
-LANGID_SPANISH_HONDURAS = 18442
-LANGID_SPANISH_MODERN_SORT = 3082
-LANGID_SPANISH_NICARAGUA = 19466
-LANGID_SPANISH_PANAMA = 6154
-LANGID_SPANISH_PARAGUAY = 15370
-LANGID_SPANISH_PERU = 10250
-LANGID_SPANISH_PUERTO_RICO = 20490
-LANGID_SPANISH_URUGUAY = 14346
-LANGID_SPANISH_VENEZUELA = 8202
-LANGID_SUTU = 1072
-LANGID_SWAHILI = 1089
-LANGID_SWEDISH = 1053
-LANGID_SWEDISH_FINLAND = 2077
-LANGID_SWISS_FRENCH = 4108
-LANGID_SWISS_GERMAN = 2055
-LANGID_SWISS_ITALIAN = 2064
-LANGID_SYRIAC = 1114
-LANGID_TAJIK = 1064
-LANGID_TAMAZIGHT = 1119
-LANGID_TAMAZIGHT_LATIN = 2143
-LANGID_TAMIL = 1097
-LANGID_TATAR = 1092
-LANGID_TELUGU = 1098
-LANGID_THAI = 1054
-LANGID_TIBETAN = 1105
-LANGID_TIGRIGNA_ERITREA = 2163
-LANGID_TIGRIGNA_ETHIOPIC = 1139
-LANGID_TRADITIONAL_CHINESE = 1028
-LANGID_TSONGA = 1073
-LANGID_TSWANA = 1074
-LANGID_TURKISH = 1055
-LANGID_TURKMEN = 1090
-LANGID_UKRAINIAN = 1058
-LANGID_URDU = 1056
-LANGID_UZBEK_CYRILLIC = 2115
-LANGID_UZBEK_LATIN = 1091
-LANGID_VENDA = 1075
-LANGID_VIETNAMESE = 1066
-LANGID_WELSH = 1106
-LANGID_XHOSA = 1076
-LANGID_YI = 1144
-LANGID_YIDDISH = 1085
-LANGID_YORUBA = 1130
-LANGID_ZULU = 1077
-
-lang_id_names = {
-    LANGID_AFRIKAANS: "African",
-    LANGID_ALBANIAN: "Albanian",
-    LANGID_AMHARIC: "Amharic",
-    LANGID_ARABIC: "Arabic",
-    LANGID_ARABIC_ALGERIA: "Arabic Algerian",
-    LANGID_ARABIC_BAHRAIN: "Arabic Bahraini",
-    LANGID_ARABIC_EGYPT: "Arabic Egyptian",
-    LANGID_ARABIC_IRAQ: "Arabic Iraqi",
-    LANGID_ARABIC_JORDAN: "Arabic Jordanian",
-    LANGID_ARABIC_KUWAIT: "Arabic Kuwaiti",
-    LANGID_ARABIC_LEBANON: "Arabic Lebanese",
-    LANGID_ARABIC_LIBYA: "Arabic Libyan",
-    LANGID_ARABIC_MOROCCO: "Arabic Moroccan",
-    LANGID_ARABIC_OMAN: "Arabic Omani",
-    LANGID_ARABIC_QATAR: "Arabic Qatari",
-    LANGID_ARABIC_SYRIA: "Arabic Syrian",
-    LANGID_ARABIC_TUNISIA: "Arabic Tunisian",
-    LANGID_ARABIC_UAE: "Arabic United Arab Emirates",
-    LANGID_ARABIC_YEMEN: "Arabic Yemeni",
-    LANGID_ARMENIAN: "Armenian",
-    LANGID_ASSAMESE: "Assamese",
-    LANGID_AZERI_CYRILLIC: "Azeri Cyrillic",
-    LANGID_AZERI_LATIN: "Azeri Latin",
-    LANGID_BASQUE: "Basque",
-    LANGID_BELGIAN_DUTCH: "Belgian Dutch",
-    LANGID_BELGIAN_FRENCH: "Belgian French",
-    LANGID_BENGALI: "Bengali",
-    LANGID_BULGARIAN: "Bulgarian",
-    LANGID_BURMESE: "Burmese",
-    LANGID_BYELORUSSIAN: "Byelorussian",
-    LANGID_CATALAN: "Catalan",
-    LANGID_CHEROKEE: "Cherokee",
-    LANGID_CHINESE_HONG_KONG_SAR: "Chinese Hong Kong SAR",
-    LANGID_CHINESE_MACAO_SAR: "Chinese Macao SAR",
-    LANGID_CHINESE_SINGAPORE: "Chinese Singapore",
-    LANGID_CROATIAN: "Croatian",
-    LANGID_CZECH: "Czech",
-    LANGID_DANISH: "Danish",
-    LANGID_DIVEHI: "Divehi",
-    LANGID_DUTCH: "Dutch",
-    LANGID_EDO: "Edo",
-    LANGID_ENGLISH_AUS: "Australian English",
-    LANGID_ENGLISH_BELIZE: "Belize English",
-    LANGID_ENGLISH_CANADIAN: "Canadian English",
-    LANGID_ENGLISH_CARIBBEAN: "Caribbean English",
-    LANGID_ENGLISH_INDONESIA: "Indonesian English",
-    LANGID_ENGLISH_IRELAND: "Irish English",
-    LANGID_ENGLISH_JAMAICA: "Jamaican English",
-    LANGID_ENGLISH_NEW_ZEALAND: "New Zealand English",
-    LANGID_ENGLISH_PHILIPPINES: "Filipino English",
-    LANGID_ENGLISH_SOUTH_AFRICA: "South African English",
-    LANGID_ENGLISH_TRINIDAD_TOBAGO: "Tobago Trinidad English",
-    LANGID_ENGLISH_UK: "United Kingdom English",
-    LANGID_ENGLISH_US: "United States English",
-    LANGID_ENGLISH_ZIMBABWE: "Zimbabwe English",
-    LANGID_ESTONIAN: "Estonian",
-    LANGID_FAEROESE: "Faeroese",
-    LANGID_FILIPINO: "Filipino",
-    LANGID_FINNISH: "Finnish",
-    LANGID_FRENCH: "French",
-    LANGID_FRENCH_CAMEROON: "French Cameroon",
-    LANGID_FRENCH_CANADIAN: "French Canadian",
-    LANGID_FRENCH_CONGO_D_R_C: "French (Congo (DRC))",
-    LANGID_FRENCH_COTED_IVOIRE: "French Cote d'Ivoire",
-    LANGID_FRENCH_HAITI: "French Haiti",
-    LANGID_FRENCH_LUXEMBOURG: "French Luxembourg",
-    LANGID_FRENCH_MALI: "French Mali",
-    LANGID_FRENCH_MONACO: "French Monaco",
-    LANGID_FRENCH_MOROCCO: "French Morocco",
-    LANGID_FRENCH_REUNION: "French Reunion",
-    LANGID_FRENCH_SENEGAL: "French Senegal",
-    LANGID_FRENCH_WEST_INDIES: "French West Indies",
-    LANGID_FRISIAN_NETHERLANDS: "Frisian Netherlands",
-    LANGID_FULFULDE: "Fulfulde",
-    LANGID_GAELIC_IRELAND: "Gaelic Irish",
-    LANGID_GAELIC_SCOTLAND: "Gaelic Scottish",
-    LANGID_GALICIAN: "Galician",
-    LANGID_GEORGIAN: "Georgian",
-    LANGID_GERMAN: "German",
-    LANGID_GERMAN_AUSTRIA: "German Austrian",
-    LANGID_GERMAN_LIECHTENSTEIN: "German Liechtenstein",
-    LANGID_GERMAN_LUXEMBOURG: "German Luxembourg",
-    LANGID_GREEK: "Greek",
-    LANGID_GUARANI: "Guarani",
-    LANGID_GUJARATI: "Gujarati",
-    LANGID_HAUSA: "Hausa",
-    LANGID_HAWAIIAN: "Hawaiian",
-    LANGID_HEBREW: "Hebrew",
-    LANGID_HINDI: "Hindi",
-    LANGID_HUNGARIAN: "Hungarian",
-    LANGID_IBIBIO: "Ibibio",
-    LANGID_ICELANDIC: "Icelandic",
-    LANGID_IGBO: "Igbo",
-    LANGID_INDONESIAN: "Indonesian",
-    LANGID_INUKTITUT: "Inuktitut",
-    LANGID_ITALIAN: "Italian",
-    LANGID_JAPANESE: "Japanese",
-    LANGID_KANNADA: "Kannada",
-    LANGID_KANURI: "Kanuri",
-    LANGID_KASHMIRI: "Kashmiri",
-    LANGID_KAZAKH: "Kazakh",
-    LANGID_KHMER: "Khmer",
-    LANGID_KIRGHIZ: "Kirghiz",
-    LANGID_KONKANI: "Konkani",
-    LANGID_KOREAN: "Korean",
-    LANGID_KYRGYZ: "Kyrgyz",
-    LANGID_LANGUAGE_NONE: "No specified",
-    LANGID_LAO: "Lao",
-    LANGID_LATIN: "Latin",
-    LANGID_LATVIAN: "Latvian",
-    LANGID_LITHUANIAN: "Lithuanian",
-    LANGID_MACEDONIAN_FYROM: "Macedonian (FYROM)",
-    LANGID_MALAYALAM: "Malayalam",
-    LANGID_MALAY_BRUNEI_DARUSSALAM: "Malay Brunei Darussalam",
-    LANGID_MALAYSIAN: "Malaysian",
-    LANGID_MALTESE: "Maltese",
-    LANGID_MANIPURI: "Manipuri",
-    LANGID_MARATHI: "Marathi",
-    LANGID_MEXICAN_SPANISH: "Mexican Spanish",
-    LANGID_MONGOLIAN: "Mongolian",
-    LANGID_NEPALI: "Nepali",
-    LANGID_NO_PROOFING: "Disables proofing",
-    LANGID_NORWEGIAN_BOKMOL: "Norwegian Bokmol",
-    LANGID_NORWEGIAN_NYNORSK: "Norwegian Nynorsk",
-    LANGID_ORIYA: "Oriya",
-    LANGID_OROMO: "Oromo",
-    LANGID_PASHTO: "Pashto",
-    LANGID_PERSIAN: "Persian",
-    LANGID_POLISH: "Polish",
-    LANGID_PORTUGUESE: "Portuguese",
-    LANGID_PORTUGUESE_BRAZIL: "Portuguese (Brazil)",
-    LANGID_PUNJABI: "Punjabi",
-    LANGID_RHAETO_ROMANIC: "Rhaeto Romanic",
-    LANGID_ROMANIAN: "Romanian",
-    LANGID_ROMANIAN_MOLDOVA: "Romanian Moldova",
-    LANGID_RUSSIAN: "Russian",
-    LANGID_RUSSIAN_MOLDOVA: "Russian Moldova",
-    LANGID_SAMI_LAPPISH: "Sami Lappish",
-    LANGID_SANSKRIT: "Sanskrit",
-    LANGID_SERBIAN_CYRILLIC: "Serbian Cyrillic",
-    LANGID_SERBIAN_LATIN: "Serbian Latin",
-    LANGID_SESOTHO: "Sesotho",
-    LANGID_SIMPLIFIED_CHINESE: "Simplified Chinese",
-    LANGID_SINDHI: "Sindhi",
-    LANGID_SINDHI_PAKISTAN: "Sindhi (Pakistan)",
-    LANGID_SINHALESE: "Sinhalese",
-    LANGID_SLOVAK: "Slovakian",
-    LANGID_SLOVENIAN: "Slovenian",
-    LANGID_SOMALI: "Somali",
-    LANGID_SORBIAN: "Sorbian",
-    LANGID_SPANISH: "Spanish",
-    LANGID_SPANISH_ARGENTINA: "Spanish Argentina",
-    LANGID_SPANISH_BOLIVIA: "Spanish Bolivian",
-    LANGID_SPANISH_CHILE: "Spanish Chilean",
-    LANGID_SPANISH_COLOMBIA: "Spanish Colombian",
-    LANGID_SPANISH_COSTA_RICA: "Spanish Costa Rican",
-    LANGID_SPANISH_DOMINICAN_REPUBLIC: "Spanish Dominican Republic",
-    LANGID_SPANISH_ECUADOR: "Spanish Ecuadorian",
-    LANGID_SPANISH_EL_SALVADOR: "Spanish El Salvadorian",
-    LANGID_SPANISH_GUATEMALA: "Spanish Guatemala",
-    LANGID_SPANISH_HONDURAS: "Spanish Honduran",
-    LANGID_SPANISH_MODERN_SORT: "Spanish Modern Sort",
-    LANGID_SPANISH_NICARAGUA: "Spanish Nicaraguan",
-    LANGID_SPANISH_PANAMA: "Spanish Panamanian",
-    LANGID_SPANISH_PARAGUAY: "Spanish Paraguayan",
-    LANGID_SPANISH_PERU: "Spanish Peruvian",
-    LANGID_SPANISH_PUERTO_RICO: "Spanish Puerto Rican",
-    LANGID_SPANISH_URUGUAY: "Spanish Uruguayan",
-    LANGID_SPANISH_VENEZUELA: "Spanish Venezuelan",
-    LANGID_SUTU: "Sutu",
-    LANGID_SWAHILI: "Swahili",
-    LANGID_SWEDISH: "Swedish",
-    LANGID_SWEDISH_FINLAND: "Swedish Finnish",
-    LANGID_SWISS_FRENCH: "Swiss French",
-    LANGID_SWISS_GERMAN: "Swiss German",
-    LANGID_SWISS_ITALIAN: "Swiss Italian",
-    LANGID_SYRIAC: "Syriac",
-    LANGID_TAJIK: "Tajik",
-    LANGID_TAMAZIGHT: "Tamazight",
-    LANGID_TAMAZIGHT_LATIN: "Tamazight Latin",
-    LANGID_TAMIL: "Tamil",
-    LANGID_TATAR: "Tatar",
-    LANGID_TELUGU: "Telugu",
-    LANGID_THAI: "Thai",
-    LANGID_TIBETAN: "Tibetan",
-    LANGID_TIGRIGNA_ERITREA: "Tigrigna Eritrea",
-    LANGID_TIGRIGNA_ETHIOPIC: "Tigrigna Ethiopic",
-    LANGID_TRADITIONAL_CHINESE: "Traditional Chinese",
-    LANGID_TSONGA: "Tsonga",
-    LANGID_TSWANA: "Tswana",
-    LANGID_TURKISH: "Turkish",
-    LANGID_TURKMEN: "Turkmen",
-    LANGID_UKRAINIAN: "Ukrainian",
-    LANGID_URDU: "Urdu",
-    LANGID_UZBEK_CYRILLIC: "Uzbek Cyrillic",
-    LANGID_UZBEK_LATIN: "Uzbek Latin",
-    LANGID_VENDA: "Venda",
-    LANGID_VIETNAMESE: "Vietnamese",
-    LANGID_WELSH: "Welsh",
-    LANGID_XHOSA: "Xhosa",
-    LANGID_YI: "Yi",
-    LANGID_YIDDISH: "Yiddish",
-    LANGID_YORUBA: "Yoruba",
-    LANGID_ZULU: "Zulu"
-}
+# Copyright 2010 Michael Murr
+#
+# This file is part of LibForensics.
+#
+# LibForensics is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Lesser General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# LibForensics is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with LibForensics.  If not, see <http://www.gnu.org/licenses/>.
+
+"""Constants for Locale IDs. (LCIDs)"""
+
+__docformat__ = "restructuredtext en"
+__all__ = [
+    "LANGID_AFRIKAANS", "LANGID_ALBANIAN", "LANGID_AMHARIC", "LANGID_ARABIC",
+    "LANGID_ARABIC_ALGERIA", "LANGID_ARABIC_BAHRAIN", "LANGID_ARABIC_EGYPT",
+    "LANGID_ARABIC_IRAQ", "LANGID_ARABIC_JORDAN", "LANGID_ARABIC_KUWAIT",
+    "LANGID_ARABIC_LEBANON", "LANGID_ARABIC_LIBYA", "LANGID_ARABIC_MOROCCO",
+    "LANGID_ARABIC_OMAN", "LANGID_ARABIC_QATAR", "LANGID_ARABIC_SYRIA",
+    "LANGID_ARABIC_TUNISIA", "LANGID_ARABIC_UAE", "LANGID_ARABIC_YEMEN",
+    "LANGID_ARMENIAN", "LANGID_ASSAMESE", "LANGID_AZERI_CYRILLIC",
+    "LANGID_AZERI_LATIN", "LANGID_BASQUE", "LANGID_BELGIAN_DUTCH",
+    "LANGID_BELGIAN_FRENCH", "LANGID_BENGALI", "LANGID_BULGARIAN",
+    "LANGID_BURMESE", "LANGID_BYELORUSSIAN", "LANGID_CATALAN",
+    "LANGID_CHEROKEE", "LANGID_CHINESE_HONG_KONG_SAR",
+    "LANGID_CHINESE_MACAO_SAR", "LANGID_CHINESE_SINGAPORE", "LANGID_CROATIAN",
+    "LANGID_CZECH", "LANGID_DANISH", "LANGID_DIVEHI", "LANGID_DUTCH",
+    "LANGID_EDO", "LANGID_ENGLISH_AUS", "LANGID_ENGLISH_BELIZE",
+    "LANGID_ENGLISH_CANADIAN", "LANGID_ENGLISH_CARIBBEAN",
+    "LANGID_ENGLISH_INDONESIA", "LANGID_ENGLISH_IRELAND",
+    "LANGID_ENGLISH_JAMAICA", "LANGID_ENGLISH_NEW_ZEALAND",
+    "LANGID_ENGLISH_PHILIPPINES", "LANGID_ENGLISH_SOUTH_AFRICA",
+    "LANGID_ENGLISH_TRINIDAD_TOBAGO", "LANGID_ENGLISH_UK", "LANGID_ENGLISH_US",
+    "LANGID_ENGLISH_ZIMBABWE", "LANGID_ESTONIAN", "LANGID_FAEROESE",
+    "LANGID_FILIPINO", "LANGID_FINNISH", "LANGID_FRENCH",
+    "LANGID_FRENCH_CAMEROON", "LANGID_FRENCH_CANADIAN",
+    "LANGID_FRENCH_CONGO_D_R_C", "LANGID_FRENCH_COTED_IVOIRE",
+    "LANGID_FRENCH_HAITI", "LANGID_FRENCH_LUXEMBOURG", "LANGID_FRENCH_MALI",
+    "LANGID_FRENCH_MONACO", "LANGID_FRENCH_MOROCCO", "LANGID_FRENCH_REUNION",
+    "LANGID_FRENCH_SENEGAL", "LANGID_FRENCH_WEST_INDIES",
+    "LANGID_FRISIAN_NETHERLANDS", "LANGID_FULFULDE", "LANGID_GAELIC_IRELAND",
+    "LANGID_GAELIC_SCOTLAND", "LANGID_GALICIAN", "LANGID_GEORGIAN",
+    "LANGID_GERMAN", "LANGID_GERMAN_AUSTRIA", "LANGID_GERMAN_LIECHTENSTEIN",
+    "LANGID_GERMAN_LUXEMBOURG", "LANGID_GREEK", "LANGID_GUARANI",
+    "LANGID_GUJARATI", "LANGID_HAUSA", "LANGID_HAWAIIAN", "LANGID_HEBREW",
+    "LANGID_HINDI", "LANGID_HUNGARIAN", "LANGID_IBIBIO", "LANGID_ICELANDIC",
+    "LANGID_IGBO", "LANGID_INDONESIAN", "LANGID_INUKTITUT", "LANGID_ITALIAN",
+    "LANGID_JAPANESE", "LANGID_KANNADA", "LANGID_KANURI", "LANGID_KASHMIRI",
+    "LANGID_KAZAKH", "LANGID_KHMER", "LANGID_KIRGHIZ", "LANGID_KONKANI",
+    "LANGID_KOREAN", "LANGID_KYRGYZ", "LANGID_LANGUAGE_NONE", "LANGID_LAO",
+    "LANGID_LATIN", "LANGID_LATVIAN", "LANGID_LITHUANIAN",
+    "LANGID_MACEDONIAN_FYROM", "LANGID_MALAYALAM", "LANGID_MALAYSIAN",
+    "LANGID_MALAY_BRUNEI_DARUSSALAM", "LANGID_MALTESE", "LANGID_MANIPURI",
+    "LANGID_MARATHI", "LANGID_MEXICAN_SPANISH", "LANGID_MONGOLIAN",
+    "LANGID_NEPALI", "LANGID_NORWEGIAN_BOKMOL", "LANGID_NORWEGIAN_NYNORSK",
+    "LANGID_NO_PROOFING", "LANGID_ORIYA", "LANGID_OROMO", "LANGID_PASHTO",
+    "LANGID_PERSIAN", "LANGID_POLISH", "LANGID_PORTUGUESE",
+    "LANGID_PORTUGUESE_BRAZIL", "LANGID_PUNJABI", "LANGID_RHAETO_ROMANIC",
+    "LANGID_ROMANIAN", "LANGID_ROMANIAN_MOLDOVA", "LANGID_RUSSIAN",
+    "LANGID_RUSSIAN_MOLDOVA", "LANGID_SAMI_LAPPISH", "LANGID_SANSKRIT",
+    "LANGID_SERBIAN_CYRILLIC", "LANGID_SERBIAN_LATIN", "LANGID_SESOTHO",
+    "LANGID_SIMPLIFIED_CHINESE", "LANGID_SINDHI", "LANGID_SINDHI_PAKISTAN",
+    "LANGID_SINHALESE", "LANGID_SLOVAK", "LANGID_SLOVENIAN", "LANGID_SOMALI",
+    "LANGID_SORBIAN", "LANGID_SPANISH", "LANGID_SPANISH_ARGENTINA",
+    "LANGID_SPANISH_BOLIVIA", "LANGID_SPANISH_CHILE",
+    "LANGID_SPANISH_COLOMBIA", "LANGID_SPANISH_COSTA_RICA",
+    "LANGID_SPANISH_DOMINICAN_REPUBLIC", "LANGID_SPANISH_ECUADOR",
+    "LANGID_SPANISH_EL_SALVADOR", "LANGID_SPANISH_GUATEMALA",
+    "LANGID_SPANISH_HONDURAS", "LANGID_SPANISH_MODERN_SORT",
+    "LANGID_SPANISH_NICARAGUA", "LANGID_SPANISH_PANAMA",
+    "LANGID_SPANISH_PARAGUAY", "LANGID_SPANISH_PERU",
+    "LANGID_SPANISH_PUERTO_RICO", "LANGID_SPANISH_URUGUAY",
+    "LANGID_SPANISH_VENEZUELA", "LANGID_SUTU", "LANGID_SWAHILI",
+    "LANGID_SWEDISH", "LANGID_SWEDISH_FINLAND", "LANGID_SWISS_FRENCH",
+    "LANGID_SWISS_GERMAN", "LANGID_SWISS_ITALIAN", "LANGID_SYRIAC",
+    "LANGID_TAJIK", "LANGID_TAMAZIGHT", "LANGID_TAMAZIGHT_LATIN",
+    "LANGID_TAMIL", "LANGID_TATAR", "LANGID_TELUGU", "LANGID_THAI",
+    "LANGID_TIBETAN", "LANGID_TIGRIGNA_ERITREA", "LANGID_TIGRIGNA_ETHIOPIC",
+    "LANGID_TRADITIONAL_CHINESE", "LANGID_TSONGA", "LANGID_TSWANA",
+    "LANGID_TURKISH", "LANGID_TURKMEN", "LANGID_UKRAINIAN", "LANGID_URDU",
+    "LANGID_UZBEK_CYRILLIC", "LANGID_UZBEK_LATIN", "LANGID_VENDA",
+    "LANGID_VIETNAMESE", "LANGID_WELSH", "LANGID_XHOSA", "LANGID_YI",
+    "LANGID_YIDDISH", "LANGID_YORUBA", "LANGID_ZULU",
+
+    "lang_id_names"
+]
+
+LANGID_AFRIKAANS = 1078
+LANGID_ALBANIAN = 1052
+LANGID_AMHARIC = 1118
+LANGID_ARABIC = 1025
+LANGID_ARABIC_ALGERIA = 5121
+LANGID_ARABIC_BAHRAIN = 15361
+LANGID_ARABIC_EGYPT = 3073
+LANGID_ARABIC_IRAQ = 2049
+LANGID_ARABIC_JORDAN = 11265
+LANGID_ARABIC_KUWAIT = 13313
+LANGID_ARABIC_LEBANON = 12289
+LANGID_ARABIC_LIBYA = 4097
+LANGID_ARABIC_MOROCCO = 6145
+LANGID_ARABIC_OMAN = 8193
+LANGID_ARABIC_QATAR = 16385
+LANGID_ARABIC_SYRIA = 10241
+LANGID_ARABIC_TUNISIA = 7169
+LANGID_ARABIC_UAE = 14337
+LANGID_ARABIC_YEMEN = 9217
+LANGID_ARMENIAN = 1067
+LANGID_ASSAMESE = 1101
+LANGID_AZERI_CYRILLIC = 2092
+LANGID_AZERI_LATIN = 1068
+LANGID_BASQUE = 1069
+LANGID_BELGIAN_DUTCH = 2067
+LANGID_BELGIAN_FRENCH = 2060
+LANGID_BENGALI = 1093
+LANGID_BULGARIAN = 1026
+LANGID_BURMESE = 1109
+LANGID_BYELORUSSIAN = 1059
+LANGID_CATALAN = 1027
+LANGID_CHEROKEE = 1116
+LANGID_CHINESE_HONG_KONG_SAR = 3076
+LANGID_CHINESE_MACAO_SAR = 5124
+LANGID_CHINESE_SINGAPORE = 4100
+LANGID_CROATIAN = 1050
+LANGID_CZECH = 1029
+LANGID_DANISH = 1030
+LANGID_DIVEHI = 1125
+LANGID_DUTCH = 1043
+LANGID_EDO = 1126
+LANGID_ENGLISH_AUS = 3081
+LANGID_ENGLISH_BELIZE = 10249
+LANGID_ENGLISH_CANADIAN = 4105
+LANGID_ENGLISH_CARIBBEAN = 9225
+LANGID_ENGLISH_INDONESIA = 14345
+LANGID_ENGLISH_IRELAND = 6153
+LANGID_ENGLISH_JAMAICA = 8201
+LANGID_ENGLISH_NEW_ZEALAND = 5129
+LANGID_ENGLISH_PHILIPPINES = 13321
+LANGID_ENGLISH_SOUTH_AFRICA = 7177
+LANGID_ENGLISH_TRINIDAD_TOBAGO = 11273
+LANGID_ENGLISH_UK = 2057
+LANGID_ENGLISH_US = 1033
+LANGID_ENGLISH_ZIMBABWE = 12297
+LANGID_ESTONIAN = 1061
+LANGID_FAEROESE = 1080
+LANGID_FILIPINO = 1124
+LANGID_FINNISH = 1035
+LANGID_FRENCH = 1036
+LANGID_FRENCH_CAMEROON = 11276
+LANGID_FRENCH_CANADIAN = 3084
+LANGID_FRENCH_CONGO_D_R_C = 9228
+LANGID_FRENCH_COTED_IVOIRE = 12300
+LANGID_FRENCH_HAITI = 15372
+LANGID_FRENCH_LUXEMBOURG = 5132
+LANGID_FRENCH_MALI = 13324
+LANGID_FRENCH_MONACO = 6156
+LANGID_FRENCH_MOROCCO = 14348
+LANGID_FRENCH_REUNION = 8204
+LANGID_FRENCH_SENEGAL = 10252
+LANGID_FRENCH_WEST_INDIES = 7180
+LANGID_FRISIAN_NETHERLANDS = 1122
+LANGID_FULFULDE = 1127
+LANGID_GAELIC_IRELAND = 2108
+LANGID_GAELIC_SCOTLAND = 1084
+LANGID_GALICIAN = 1110
+LANGID_GEORGIAN = 1079
+LANGID_GERMAN = 1031
+LANGID_GERMAN_AUSTRIA = 3079
+LANGID_GERMAN_LIECHTENSTEIN = 5127
+LANGID_GERMAN_LUXEMBOURG = 4103
+LANGID_GREEK = 1032
+LANGID_GUARANI = 1140
+LANGID_GUJARATI = 1095
+LANGID_HAUSA = 1128
+LANGID_HAWAIIAN = 1141
+LANGID_HEBREW = 1037
+LANGID_HINDI = 1081
+LANGID_HUNGARIAN = 1038
+LANGID_IBIBIO = 1129
+LANGID_ICELANDIC = 1039
+LANGID_IGBO = 1136
+LANGID_INDONESIAN = 1057
+LANGID_INUKTITUT = 1117
+LANGID_ITALIAN = 1040
+LANGID_JAPANESE = 1041
+LANGID_KANNADA = 1099
+LANGID_KANURI = 1137
+LANGID_KASHMIRI = 1120
+LANGID_KAZAKH = 1087
+LANGID_KHMER = 1107
+LANGID_KIRGHIZ = 1088
+LANGID_KONKANI = 1111
+LANGID_KOREAN = 1042
+LANGID_KYRGYZ = 1088
+LANGID_LANGUAGE_NONE = 0
+LANGID_LAO = 1108
+LANGID_LATIN = 1142
+LANGID_LATVIAN = 1062
+LANGID_LITHUANIAN = 1063
+LANGID_MACEDONIAN_FYROM = 1071
+LANGID_MALAYALAM = 1100
+LANGID_MALAY_BRUNEI_DARUSSALAM = 2110
+LANGID_MALAYSIAN = 1086
+LANGID_MALTESE = 1082
+LANGID_MANIPURI = 1112
+LANGID_MARATHI = 1102
+LANGID_MEXICAN_SPANISH = 2058
+LANGID_MONGOLIAN = 1104
+LANGID_NEPALI = 1121
+LANGID_NO_PROOFING = 1024
+LANGID_NORWEGIAN_BOKMOL = 1044
+LANGID_NORWEGIAN_NYNORSK = 2068
+LANGID_ORIYA = 1096
+LANGID_OROMO = 1138
+LANGID_PASHTO = 1123
+LANGID_PERSIAN = 1065
+LANGID_POLISH = 1045
+LANGID_PORTUGUESE = 2070
+LANGID_PORTUGUESE_BRAZIL = 1046
+LANGID_PUNJABI = 1094
+LANGID_RHAETO_ROMANIC = 1047
+LANGID_ROMANIAN = 1048
+LANGID_ROMANIAN_MOLDOVA = 2072
+LANGID_RUSSIAN = 1049
+LANGID_RUSSIAN_MOLDOVA = 2073
+LANGID_SAMI_LAPPISH = 1083
+LANGID_SANSKRIT = 1103
+LANGID_SERBIAN_CYRILLIC = 3098
+LANGID_SERBIAN_LATIN = 2074
+LANGID_SESOTHO = 1072
+LANGID_SIMPLIFIED_CHINESE = 2052
+LANGID_SINDHI = 1113
+LANGID_SINDHI_PAKISTAN = 2137
+LANGID_SINHALESE = 1115
+LANGID_SLOVAK = 1051
+LANGID_SLOVENIAN = 1060
+LANGID_SOMALI = 1143
+LANGID_SORBIAN = 1070
+LANGID_SPANISH = 1034
+LANGID_SPANISH_ARGENTINA = 11274
+LANGID_SPANISH_BOLIVIA = 16394
+LANGID_SPANISH_CHILE = 13322
+LANGID_SPANISH_COLOMBIA = 9226
+LANGID_SPANISH_COSTA_RICA = 5130
+LANGID_SPANISH_DOMINICAN_REPUBLIC = 7178
+LANGID_SPANISH_ECUADOR = 12298
+LANGID_SPANISH_EL_SALVADOR = 17418
+LANGID_SPANISH_GUATEMALA = 4106
+LANGID_SPANISH_HONDURAS = 18442
+LANGID_SPANISH_MODERN_SORT = 3082
+LANGID_SPANISH_NICARAGUA = 19466
+LANGID_SPANISH_PANAMA = 6154
+LANGID_SPANISH_PARAGUAY = 15370
+LANGID_SPANISH_PERU = 10250
+LANGID_SPANISH_PUERTO_RICO = 20490
+LANGID_SPANISH_URUGUAY = 14346
+LANGID_SPANISH_VENEZUELA = 8202
+LANGID_SUTU = 1072
+LANGID_SWAHILI = 1089
+LANGID_SWEDISH = 1053
+LANGID_SWEDISH_FINLAND = 2077
+LANGID_SWISS_FRENCH = 4108
+LANGID_SWISS_GERMAN = 2055
+LANGID_SWISS_ITALIAN = 2064
+LANGID_SYRIAC = 1114
+LANGID_TAJIK = 1064
+LANGID_TAMAZIGHT = 1119
+LANGID_TAMAZIGHT_LATIN = 2143
+LANGID_TAMIL = 1097
+LANGID_TATAR = 1092
+LANGID_TELUGU = 1098
+LANGID_THAI = 1054
+LANGID_TIBETAN = 1105
+LANGID_TIGRIGNA_ERITREA = 2163
+LANGID_TIGRIGNA_ETHIOPIC = 1139
+LANGID_TRADITIONAL_CHINESE = 1028
+LANGID_TSONGA = 1073
+LANGID_TSWANA = 1074
+LANGID_TURKISH = 1055
+LANGID_TURKMEN = 1090
+LANGID_UKRAINIAN = 1058
+LANGID_URDU = 1056
+LANGID_UZBEK_CYRILLIC = 2115
+LANGID_UZBEK_LATIN = 1091
+LANGID_VENDA = 1075
+LANGID_VIETNAMESE = 1066
+LANGID_WELSH = 1106
+LANGID_XHOSA = 1076
+LANGID_YI = 1144
+LANGID_YIDDISH = 1085
+LANGID_YORUBA = 1130
+LANGID_ZULU = 1077
+
+lang_id_names = {
+    LANGID_AFRIKAANS: "African",
+    LANGID_ALBANIAN: "Albanian",
+    LANGID_AMHARIC: "Amharic",
+    LANGID_ARABIC: "Arabic",
+    LANGID_ARABIC_ALGERIA: "Arabic Algerian",
+    LANGID_ARABIC_BAHRAIN: "Arabic Bahraini",
+    LANGID_ARABIC_EGYPT: "Arabic Egyptian",
+    LANGID_ARABIC_IRAQ: "Arabic Iraqi",
+    LANGID_ARABIC_JORDAN: "Arabic Jordanian",
+    LANGID_ARABIC_KUWAIT: "Arabic Kuwaiti",
+    LANGID_ARABIC_LEBANON: "Arabic Lebanese",
+    LANGID_ARABIC_LIBYA: "Arabic Libyan",
+    LANGID_ARABIC_MOROCCO: "Arabic Moroccan",
+    LANGID_ARABIC_OMAN: "Arabic Omani",
+    LANGID_ARABIC_QATAR: "Arabic Qatari",
+    LANGID_ARABIC_SYRIA: "Arabic Syrian",
+    LANGID_ARABIC_TUNISIA: "Arabic Tunisian",
+    LANGID_ARABIC_UAE: "Arabic United Arab Emirates",
+    LANGID_ARABIC_YEMEN: "Arabic Yemeni",
+    LANGID_ARMENIAN: "Armenian",
+    LANGID_ASSAMESE: "Assamese",
+    LANGID_AZERI_CYRILLIC: "Azeri Cyrillic",
+    LANGID_AZERI_LATIN: "Azeri Latin",
+    LANGID_BASQUE: "Basque",
+    LANGID_BELGIAN_DUTCH: "Belgian Dutch",
+    LANGID_BELGIAN_FRENCH: "Belgian French",
+    LANGID_BENGALI: "Bengali",
+    LANGID_BULGARIAN: "Bulgarian",
+    LANGID_BURMESE: "Burmese",
+    LANGID_BYELORUSSIAN: "Byelorussian",
+    LANGID_CATALAN: "Catalan",
+    LANGID_CHEROKEE: "Cherokee",
+    LANGID_CHINESE_HONG_KONG_SAR: "Chinese Hong Kong SAR",
+    LANGID_CHINESE_MACAO_SAR: "Chinese Macao SAR",
+    LANGID_CHINESE_SINGAPORE: "Chinese Singapore",
+    LANGID_CROATIAN: "Croatian",
+    LANGID_CZECH: "Czech",
+    LANGID_DANISH: "Danish",
+    LANGID_DIVEHI: "Divehi",
+    LANGID_DUTCH: "Dutch",
+    LANGID_EDO: "Edo",
+    LANGID_ENGLISH_AUS: "Australian English",
+    LANGID_ENGLISH_BELIZE: "Belize English",
+    LANGID_ENGLISH_CANADIAN: "Canadian English",
+    LANGID_ENGLISH_CARIBBEAN: "Caribbean English",
+    LANGID_ENGLISH_INDONESIA: "Indonesian English",
+    LANGID_ENGLISH_IRELAND: "Irish English",
+    LANGID_ENGLISH_JAMAICA: "Jamaican English",
+    LANGID_ENGLISH_NEW_ZEALAND: "New Zealand English",
+    LANGID_ENGLISH_PHILIPPINES: "Filipino English",
+    LANGID_ENGLISH_SOUTH_AFRICA: "South African English",
+    LANGID_ENGLISH_TRINIDAD_TOBAGO: "Tobago Trinidad English",
+    LANGID_ENGLISH_UK: "United Kingdom English",
+    LANGID_ENGLISH_US: "United States English",
+    LANGID_ENGLISH_ZIMBABWE: "Zimbabwe English",
+    LANGID_ESTONIAN: "Estonian",
+    LANGID_FAEROESE: "Faeroese",
+    LANGID_FILIPINO: "Filipino",
+    LANGID_FINNISH: "Finnish",
+    LANGID_FRENCH: "French",
+    LANGID_FRENCH_CAMEROON: "French Cameroon",
+    LANGID_FRENCH_CANADIAN: "French Canadian",
+    LANGID_FRENCH_CONGO_D_R_C: "French (Congo (DRC))",
+    LANGID_FRENCH_COTED_IVOIRE: "French Cote d'Ivoire",
+    LANGID_FRENCH_HAITI: "French Haiti",
+    LANGID_FRENCH_LUXEMBOURG: "French Luxembourg",
+    LANGID_FRENCH_MALI: "French Mali",
+    LANGID_FRENCH_MONACO: "French Monaco",
+    LANGID_FRENCH_MOROCCO: "French Morocco",
+    LANGID_FRENCH_REUNION: "French Reunion",
+    LANGID_FRENCH_SENEGAL: "French Senegal",
+    LANGID_FRENCH_WEST_INDIES: "French West Indies",
+    LANGID_FRISIAN_NETHERLANDS: "Frisian Netherlands",
+    LANGID_FULFULDE: "Fulfulde",
+    LANGID_GAELIC_IRELAND: "Gaelic Irish",
+    LANGID_GAELIC_SCOTLAND: "Gaelic Scottish",
+    LANGID_GALICIAN: "Galician",
+    LANGID_GEORGIAN: "Georgian",
+    LANGID_GERMAN: "German",
+    LANGID_GERMAN_AUSTRIA: "German Austrian",
+    LANGID_GERMAN_LIECHTENSTEIN: "German Liechtenstein",
+    LANGID_GERMAN_LUXEMBOURG: "German Luxembourg",
+    LANGID_GREEK: "Greek",
+    LANGID_GUARANI: "Guarani",
+    LANGID_GUJARATI: "Gujarati",
+    LANGID_HAUSA: "Hausa",
+    LANGID_HAWAIIAN: "Hawaiian",
+    LANGID_HEBREW: "Hebrew",
+    LANGID_HINDI: "Hindi",
+    LANGID_HUNGARIAN: "Hungarian",
+    LANGID_IBIBIO: "Ibibio",
+    LANGID_ICELANDIC: "Icelandic",
+    LANGID_IGBO: "Igbo",
+    LANGID_INDONESIAN: "Indonesian",
+    LANGID_INUKTITUT: "Inuktitut",
+    LANGID_ITALIAN: "Italian",
+    LANGID_JAPANESE: "Japanese",
+    LANGID_KANNADA: "Kannada",
+    LANGID_KANURI: "Kanuri",
+    LANGID_KASHMIRI: "Kashmiri",
+    LANGID_KAZAKH: "Kazakh",
+    LANGID_KHMER: "Khmer",
+    LANGID_KIRGHIZ: "Kirghiz",
+    LANGID_KONKANI: "Konkani",
+    LANGID_KOREAN: "Korean",
+    LANGID_KYRGYZ: "Kyrgyz",
+    LANGID_LANGUAGE_NONE: "No specified",
+    LANGID_LAO: "Lao",
+    LANGID_LATIN: "Latin",
+    LANGID_LATVIAN: "Latvian",
+    LANGID_LITHUANIAN: "Lithuanian",
+    LANGID_MACEDONIAN_FYROM: "Macedonian (FYROM)",
+    LANGID_MALAYALAM: "Malayalam",
+    LANGID_MALAY_BRUNEI_DARUSSALAM: "Malay Brunei Darussalam",
+    LANGID_MALAYSIAN: "Malaysian",
+    LANGID_MALTESE: "Maltese",
+    LANGID_MANIPURI: "Manipuri",
+    LANGID_MARATHI: "Marathi",
+    LANGID_MEXICAN_SPANISH: "Mexican Spanish",
+    LANGID_MONGOLIAN: "Mongolian",
+    LANGID_NEPALI: "Nepali",
+    LANGID_NO_PROOFING: "Disables proofing",
+    LANGID_NORWEGIAN_BOKMOL: "Norwegian Bokmol",
+    LANGID_NORWEGIAN_NYNORSK: "Norwegian Nynorsk",
+    LANGID_ORIYA: "Oriya",
+    LANGID_OROMO: "Oromo",
+    LANGID_PASHTO: "Pashto",
+    LANGID_PERSIAN: "Persian",
+    LANGID_POLISH: "Polish",
+    LANGID_PORTUGUESE: "Portuguese",
+    LANGID_PORTUGUESE_BRAZIL: "Portuguese (Brazil)",
+    LANGID_PUNJABI: "Punjabi",
+    LANGID_RHAETO_ROMANIC: "Rhaeto Romanic",
+    LANGID_ROMANIAN: "Romanian",
+    LANGID_ROMANIAN_MOLDOVA: "Romanian Moldova",
+    LANGID_RUSSIAN: "Russian",
+    LANGID_RUSSIAN_MOLDOVA: "Russian Moldova",
+    LANGID_SAMI_LAPPISH: "Sami Lappish",
+    LANGID_SANSKRIT: "Sanskrit",
+    LANGID_SERBIAN_CYRILLIC: "Serbian Cyrillic",
+    LANGID_SERBIAN_LATIN: "Serbian Latin",
+    LANGID_SESOTHO: "Sesotho",
+    LANGID_SIMPLIFIED_CHINESE: "Simplified Chinese",
+    LANGID_SINDHI: "Sindhi",
+    LANGID_SINDHI_PAKISTAN: "Sindhi (Pakistan)",
+    LANGID_SINHALESE: "Sinhalese",
+    LANGID_SLOVAK: "Slovakian",
+    LANGID_SLOVENIAN: "Slovenian",
+    LANGID_SOMALI: "Somali",
+    LANGID_SORBIAN: "Sorbian",
+    LANGID_SPANISH: "Spanish",
+    LANGID_SPANISH_ARGENTINA: "Spanish Argentina",
+    LANGID_SPANISH_BOLIVIA: "Spanish Bolivian",
+    LANGID_SPANISH_CHILE: "Spanish Chilean",
+    LANGID_SPANISH_COLOMBIA: "Spanish Colombian",
+    LANGID_SPANISH_COSTA_RICA: "Spanish Costa Rican",
+    LANGID_SPANISH_DOMINICAN_REPUBLIC: "Spanish Dominican Republic",
+    LANGID_SPANISH_ECUADOR: "Spanish Ecuadorian",
+    LANGID_SPANISH_EL_SALVADOR: "Spanish El Salvadorian",
+    LANGID_SPANISH_GUATEMALA: "Spanish Guatemala",
+    LANGID_SPANISH_HONDURAS: "Spanish Honduran",
+    LANGID_SPANISH_MODERN_SORT: "Spanish Modern Sort",
+    LANGID_SPANISH_NICARAGUA: "Spanish Nicaraguan",
+    LANGID_SPANISH_PANAMA: "Spanish Panamanian",
+    LANGID_SPANISH_PARAGUAY: "Spanish Paraguayan",
+    LANGID_SPANISH_PERU: "Spanish Peruvian",
+    LANGID_SPANISH_PUERTO_RICO: "Spanish Puerto Rican",
+    LANGID_SPANISH_URUGUAY: "Spanish Uruguayan",
+    LANGID_SPANISH_VENEZUELA: "Spanish Venezuelan",
+    LANGID_SUTU: "Sutu",
+    LANGID_SWAHILI: "Swahili",
+    LANGID_SWEDISH: "Swedish",
+    LANGID_SWEDISH_FINLAND: "Swedish Finnish",
+    LANGID_SWISS_FRENCH: "Swiss French",
+    LANGID_SWISS_GERMAN: "Swiss German",
+    LANGID_SWISS_ITALIAN: "Swiss Italian",
+    LANGID_SYRIAC: "Syriac",
+    LANGID_TAJIK: "Tajik",
+    LANGID_TAMAZIGHT: "Tamazight",
+    LANGID_TAMAZIGHT_LATIN: "Tamazight Latin",
+    LANGID_TAMIL: "Tamil",
+    LANGID_TATAR: "Tatar",
+    LANGID_TELUGU: "Telugu",
+    LANGID_THAI: "Thai",
+    LANGID_TIBETAN: "Tibetan",
+    LANGID_TIGRIGNA_ERITREA: "Tigrigna Eritrea",
+    LANGID_TIGRIGNA_ETHIOPIC: "Tigrigna Ethiopic",
+    LANGID_TRADITIONAL_CHINESE: "Traditional Chinese",
+    LANGID_TSONGA: "Tsonga",
+    LANGID_TSWANA: "Tswana",
+    LANGID_TURKISH: "Turkish",
+    LANGID_TURKMEN: "Turkmen",
+    LANGID_UKRAINIAN: "Ukrainian",
+    LANGID_URDU: "Urdu",
+    LANGID_UZBEK_CYRILLIC: "Uzbek Cyrillic",
+    LANGID_UZBEK_LATIN: "Uzbek Latin",
+    LANGID_VENDA: "Venda",
+    LANGID_VIETNAMESE: "Vietnamese",
+    LANGID_WELSH: "Welsh",
+    LANGID_XHOSA: "Xhosa",
+    LANGID_YI: "Yi",
+    LANGID_YIDDISH: "Yiddish",
+    LANGID_YORUBA: "Yoruba",
+    LANGID_ZULU: "Zulu"
+}
```

### Comparing `python-tds-1.9.0/pytds/pyDes.py` & `python-tds-1.9.1/pytds/pyDes.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,852 +1,852 @@
-#############################################################################
-# 				Documentation				    #
-#############################################################################
-
-# Author:   Todd Whiteman
-# Date:     16th March, 2009
-# Verion:   2.0.0
-# License:  Public Domain - free to do as you wish
-# Homepage: http://twhiteman.netfirms.com/des.html
-#
-# This is a pure python implementation of the DES encryption algorithm.
-# It's pure python to avoid portability issues, since most DES 
-# implementations are programmed in C (for performance reasons).
-#
-# Triple DES class is also implemented, utilising the DES base. Triple DES
-# is either DES-EDE3 with a 24 byte key, or DES-EDE2 with a 16 byte key.
-#
-# See the README.txt that should come with this python module for the
-# implementation methods used.
-#
-# Thanks to:
-#  * David Broadwell for ideas, comments and suggestions.
-#  * Mario Wolff for pointing out and debugging some triple des CBC errors.
-#  * Santiago Palladino for providing the PKCS5 padding technique.
-#  * Shaya for correcting the PAD_PKCS5 triple des CBC errors.
-#
-"""A pure python implementation of the DES and TRIPLE DES encryption algorithms.
-
-Class initialization
---------------------
-pyDes.des(key, [mode], [IV], [pad], [padmode])
-pyDes.triple_des(key, [mode], [IV], [pad], [padmode])
-
-key     -> Bytes containing the encryption key. 8 bytes for DES, 16 or 24 bytes
-	   for Triple DES
-mode    -> Optional argument for encryption type, can be either
-	   pyDes.ECB (Electronic Code Book) or pyDes.CBC (Cypher Block Chaining)
-IV      -> Optional Initial Value bytes, must be supplied if using CBC mode.
-	   Length must be 8 bytes.
-pad     -> Optional argument, set the pad character (PAD_NORMAL) to use during
-	   all encrypt/decrpt operations done with this instance.
-padmode -> Optional argument, set the padding mode (PAD_NORMAL or PAD_PKCS5)
-	   to use during all encrypt/decrpt operations done with this instance.
-
-I recommend to use PAD_PKCS5 padding, as then you never need to worry about any
-padding issues, as the padding can be removed unambiguously upon decrypting
-data that was encrypted using PAD_PKCS5 padmode.
-
-Common methods
---------------
-encrypt(data, [pad], [padmode])
-decrypt(data, [pad], [padmode])
-
-data    -> Bytes to be encrypted/decrypted
-pad     -> Optional argument. Only when using padmode of PAD_NORMAL. For
-	   encryption, adds this characters to the end of the data block when
-	   data is not a multiple of 8 bytes. For decryption, will remove the
-	   trailing characters that match this pad character from the last 8
-	   bytes of the unencrypted data block.
-padmode -> Optional argument, set the padding mode, must be one of PAD_NORMAL
-	   or PAD_PKCS5). Defaults to PAD_NORMAL.
-	  
-
-Example
--------
-from pyDes import *
-
-data = "Please encrypt my data"
-k = des("DESCRYPT", CBC, "\0\0\0\0\0\0\0\0", pad=None, padmode=PAD_PKCS5)
-# For Python3, you'll need to use bytes, i.e.:
-#   data = b"Please encrypt my data"
-#   k = des(b"DESCRYPT", CBC, b"\0\0\0\0\0\0\0\0", pad=None, padmode=PAD_PKCS5)
-d = k.encrypt(data)
-print "Encrypted: %r" % d
-print "Decrypted: %r" % k.decrypt(d)
-assert k.decrypt(d, padmode=PAD_PKCS5) == data
-
-
-See the module source (pyDes.py) for more examples of use.
-You can also run the pyDes.py file without and arguments to see a simple test.
-
-Note: This code was not written for high-end systems needing a fast
-      implementation, but rather a handy portable solution with small usage.
-
-"""
-
-import sys
-
-# _pythonMajorVersion is used to handle Python2 and Python3 differences.
-_pythonMajorVersion = sys.version_info[0]
-
-# Modes of crypting / cyphering
-ECB =	0
-CBC =	1
-
-# Modes of padding
-PAD_NORMAL = 1
-PAD_PKCS5 = 2
-
-# PAD_PKCS5: is a method that will unambiguously remove all padding
-#            characters after decryption, when originally encrypted with
-#            this padding mode.
-# For a good description of the PKCS5 padding technique, see:
-# http://www.faqs.org/rfcs/rfc1423.html
-
-# The base class shared by des and triple des.
-class _baseDes(object):
-	def __init__(self, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
-		if IV:
-			IV = self._guardAgainstUnicode(IV)
-		if pad:
-			pad = self._guardAgainstUnicode(pad)
-		self.block_size = 8
-		# Sanity checking of arguments.
-		if pad and padmode == PAD_PKCS5:
-			raise ValueError("Cannot use a pad character with PAD_PKCS5")
-		if IV and len(IV) != self.block_size:
-			raise ValueError("Invalid Initial Value (IV), must be a multiple of " + str(self.block_size) + " bytes")
-
-		# Set the passed in variables
-		self._mode = mode
-		self._iv = IV
-		self._padding = pad
-		self._padmode = padmode
-
-	def getKey(self):
-		"""getKey() -> bytes"""
-		return self.__key
-
-	def setKey(self, key):
-		"""Will set the crypting key for this object."""
-		key = self._guardAgainstUnicode(key)
-		self.__key = key
-
-	def getMode(self):
-		"""getMode() -> pyDes.ECB or pyDes.CBC"""
-		return self._mode
-
-	def setMode(self, mode):
-		"""Sets the type of crypting mode, pyDes.ECB or pyDes.CBC"""
-		self._mode = mode
-
-	def getPadding(self):
-		"""getPadding() -> bytes of length 1. Padding character."""
-		return self._padding
-
-	def setPadding(self, pad):
-		"""setPadding() -> bytes of length 1. Padding character."""
-		if pad is not None:
-			pad = self._guardAgainstUnicode(pad)
-		self._padding = pad
-
-	def getPadMode(self):
-		"""getPadMode() -> pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
-		return self._padmode
-		
-	def setPadMode(self, mode):
-		"""Sets the type of padding mode, pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
-		self._padmode = mode
-
-	def getIV(self):
-		"""getIV() -> bytes"""
-		return self._iv
-
-	def setIV(self, IV):
-		"""Will set the Initial Value, used in conjunction with CBC mode"""
-		if not IV or len(IV) != self.block_size:
-			raise ValueError("Invalid Initial Value (IV), must be a multiple of " + str(self.block_size) + " bytes")
-		IV = self._guardAgainstUnicode(IV)
-		self._iv = IV
-
-	def _padData(self, data, pad, padmode):
-		# Pad data depending on the mode
-		if padmode is None:
-			# Get the default padding mode.
-			padmode = self.getPadMode()
-		if pad and padmode == PAD_PKCS5:
-			raise ValueError("Cannot use a pad character with PAD_PKCS5")
-
-		if padmode == PAD_NORMAL:
-			if len(data) % self.block_size == 0:
-				# No padding required.
-				return data
-
-			if not pad:
-				# Get the default padding.
-				pad = self.getPadding()
-			if not pad:
-				raise ValueError("Data must be a multiple of " + str(self.block_size) + " bytes in length. Use padmode=PAD_PKCS5 or set the pad character.")
-			data += (self.block_size - (len(data) % self.block_size)) * pad
-		
-		elif padmode == PAD_PKCS5:
-			pad_len = 8 - (len(data) % self.block_size)
-			if _pythonMajorVersion < 3:
-				data += pad_len * chr(pad_len)
-			else:
-				data += bytes([pad_len] * pad_len)
-
-		return data
-
-	def _unpadData(self, data, pad, padmode):
-		# Unpad data depending on the mode.
-		if not data:
-			return data
-		if pad and padmode == PAD_PKCS5:
-			raise ValueError("Cannot use a pad character with PAD_PKCS5")
-		if padmode is None:
-			# Get the default padding mode.
-			padmode = self.getPadMode()
-
-		if padmode == PAD_NORMAL:
-			if not pad:
-				# Get the default padding.
-				pad = self.getPadding()
-			if pad:
-				data = data[:-self.block_size] + \
-				       data[-self.block_size:].rstrip(pad)
-
-		elif padmode == PAD_PKCS5:
-			if _pythonMajorVersion < 3:
-				pad_len = ord(data[-1])
-			else:
-				pad_len = data[-1]
-			data = data[:-pad_len]
-
-		return data
-
-	def _guardAgainstUnicode(self, data):
-		# Only accept byte strings or ascii unicode values, otherwise
-		# there is no way to correctly decode the data into bytes.
-		if _pythonMajorVersion < 3:
-			if isinstance(data, unicode):
-				raise ValueError("pyDes can only work with bytes, not Unicode strings.")
-		else:
-			if isinstance(data, str):
-				# Only accept ascii unicode values.
-				try:
-					return data.encode('ascii')
-				except UnicodeEncodeError:
-					pass
-				raise ValueError("pyDes can only work with encoded strings, not Unicode.")
-		return data
-
-#############################################################################
-# 				    DES					    #
-#############################################################################
-class des(_baseDes):
-	"""DES encryption/decrytpion class
-
-	Supports ECB (Electronic Code Book) and CBC (Cypher Block Chaining) modes.
-
-	pyDes.des(key,[mode], [IV])
-
-	key  -> Bytes containing the encryption key, must be exactly 8 bytes
-	mode -> Optional argument for encryption type, can be either pyDes.ECB
-		(Electronic Code Book), pyDes.CBC (Cypher Block Chaining)
-	IV   -> Optional Initial Value bytes, must be supplied if using CBC mode.
-		Must be 8 bytes in length.
-	pad  -> Optional argument, set the pad character (PAD_NORMAL) to use
-		during all encrypt/decrpt operations done with this instance.
-	padmode -> Optional argument, set the padding mode (PAD_NORMAL or
-		PAD_PKCS5) to use during all encrypt/decrpt operations done
-		with this instance.
-	"""
-
-
-	# Permutation and translation tables for DES
-	__pc1 = [56, 48, 40, 32, 24, 16,  8,
-		  0, 57, 49, 41, 33, 25, 17,
-		  9,  1, 58, 50, 42, 34, 26,
-		 18, 10,  2, 59, 51, 43, 35,
-		 62, 54, 46, 38, 30, 22, 14,
-		  6, 61, 53, 45, 37, 29, 21,
-		 13,  5, 60, 52, 44, 36, 28,
-		 20, 12,  4, 27, 19, 11,  3
-	]
-
-	# number left rotations of pc1
-	__left_rotations = [
-		1, 1, 2, 2, 2, 2, 2, 2, 1, 2, 2, 2, 2, 2, 2, 1
-	]
-
-	# permuted choice key (table 2)
-	__pc2 = [
-		13, 16, 10, 23,  0,  4,
-		 2, 27, 14,  5, 20,  9,
-		22, 18, 11,  3, 25,  7,
-		15,  6, 26, 19, 12,  1,
-		40, 51, 30, 36, 46, 54,
-		29, 39, 50, 44, 32, 47,
-		43, 48, 38, 55, 33, 52,
-		45, 41, 49, 35, 28, 31
-	]
-
-	# initial permutation IP
-	__ip = [57, 49, 41, 33, 25, 17, 9,  1,
-		59, 51, 43, 35, 27, 19, 11, 3,
-		61, 53, 45, 37, 29, 21, 13, 5,
-		63, 55, 47, 39, 31, 23, 15, 7,
-		56, 48, 40, 32, 24, 16, 8,  0,
-		58, 50, 42, 34, 26, 18, 10, 2,
-		60, 52, 44, 36, 28, 20, 12, 4,
-		62, 54, 46, 38, 30, 22, 14, 6
-	]
-
-	# Expansion table for turning 32 bit blocks into 48 bits
-	__expansion_table = [
-		31,  0,  1,  2,  3,  4,
-		 3,  4,  5,  6,  7,  8,
-		 7,  8,  9, 10, 11, 12,
-		11, 12, 13, 14, 15, 16,
-		15, 16, 17, 18, 19, 20,
-		19, 20, 21, 22, 23, 24,
-		23, 24, 25, 26, 27, 28,
-		27, 28, 29, 30, 31,  0
-	]
-
-	# The (in)famous S-boxes
-	__sbox = [
-		# S1
-		[14, 4, 13, 1, 2, 15, 11, 8, 3, 10, 6, 12, 5, 9, 0, 7,
-		 0, 15, 7, 4, 14, 2, 13, 1, 10, 6, 12, 11, 9, 5, 3, 8,
-		 4, 1, 14, 8, 13, 6, 2, 11, 15, 12, 9, 7, 3, 10, 5, 0,
-		 15, 12, 8, 2, 4, 9, 1, 7, 5, 11, 3, 14, 10, 0, 6, 13],
-
-		# S2
-		[15, 1, 8, 14, 6, 11, 3, 4, 9, 7, 2, 13, 12, 0, 5, 10,
-		 3, 13, 4, 7, 15, 2, 8, 14, 12, 0, 1, 10, 6, 9, 11, 5,
-		 0, 14, 7, 11, 10, 4, 13, 1, 5, 8, 12, 6, 9, 3, 2, 15,
-		 13, 8, 10, 1, 3, 15, 4, 2, 11, 6, 7, 12, 0, 5, 14, 9],
-
-		# S3
-		[10, 0, 9, 14, 6, 3, 15, 5, 1, 13, 12, 7, 11, 4, 2, 8,
-		 13, 7, 0, 9, 3, 4, 6, 10, 2, 8, 5, 14, 12, 11, 15, 1,
-		 13, 6, 4, 9, 8, 15, 3, 0, 11, 1, 2, 12, 5, 10, 14, 7,
-		 1, 10, 13, 0, 6, 9, 8, 7, 4, 15, 14, 3, 11, 5, 2, 12],
-
-		# S4
-		[7, 13, 14, 3, 0, 6, 9, 10, 1, 2, 8, 5, 11, 12, 4, 15,
-		 13, 8, 11, 5, 6, 15, 0, 3, 4, 7, 2, 12, 1, 10, 14, 9,
-		 10, 6, 9, 0, 12, 11, 7, 13, 15, 1, 3, 14, 5, 2, 8, 4,
-		 3, 15, 0, 6, 10, 1, 13, 8, 9, 4, 5, 11, 12, 7, 2, 14],
-
-		# S5
-		[2, 12, 4, 1, 7, 10, 11, 6, 8, 5, 3, 15, 13, 0, 14, 9,
-		 14, 11, 2, 12, 4, 7, 13, 1, 5, 0, 15, 10, 3, 9, 8, 6,
-		 4, 2, 1, 11, 10, 13, 7, 8, 15, 9, 12, 5, 6, 3, 0, 14,
-		 11, 8, 12, 7, 1, 14, 2, 13, 6, 15, 0, 9, 10, 4, 5, 3],
-
-		# S6
-		[12, 1, 10, 15, 9, 2, 6, 8, 0, 13, 3, 4, 14, 7, 5, 11,
-		 10, 15, 4, 2, 7, 12, 9, 5, 6, 1, 13, 14, 0, 11, 3, 8,
-		 9, 14, 15, 5, 2, 8, 12, 3, 7, 0, 4, 10, 1, 13, 11, 6,
-		 4, 3, 2, 12, 9, 5, 15, 10, 11, 14, 1, 7, 6, 0, 8, 13],
-
-		# S7
-		[4, 11, 2, 14, 15, 0, 8, 13, 3, 12, 9, 7, 5, 10, 6, 1,
-		 13, 0, 11, 7, 4, 9, 1, 10, 14, 3, 5, 12, 2, 15, 8, 6,
-		 1, 4, 11, 13, 12, 3, 7, 14, 10, 15, 6, 8, 0, 5, 9, 2,
-		 6, 11, 13, 8, 1, 4, 10, 7, 9, 5, 0, 15, 14, 2, 3, 12],
-
-		# S8
-		[13, 2, 8, 4, 6, 15, 11, 1, 10, 9, 3, 14, 5, 0, 12, 7,
-		 1, 15, 13, 8, 10, 3, 7, 4, 12, 5, 6, 11, 0, 14, 9, 2,
-		 7, 11, 4, 1, 9, 12, 14, 2, 0, 6, 10, 13, 15, 3, 5, 8,
-		 2, 1, 14, 7, 4, 10, 8, 13, 15, 12, 9, 0, 3, 5, 6, 11],
-	]
-
-
-	# 32-bit permutation function P used on the output of the S-boxes
-	__p = [
-		15, 6, 19, 20, 28, 11,
-		27, 16, 0, 14, 22, 25,
-		4, 17, 30, 9, 1, 7,
-		23,13, 31, 26, 2, 8,
-		18, 12, 29, 5, 21, 10,
-		3, 24
-	]
-
-	# final permutation IP^-1
-	__fp = [
-		39,  7, 47, 15, 55, 23, 63, 31,
-		38,  6, 46, 14, 54, 22, 62, 30,
-		37,  5, 45, 13, 53, 21, 61, 29,
-		36,  4, 44, 12, 52, 20, 60, 28,
-		35,  3, 43, 11, 51, 19, 59, 27,
-		34,  2, 42, 10, 50, 18, 58, 26,
-		33,  1, 41,  9, 49, 17, 57, 25,
-		32,  0, 40,  8, 48, 16, 56, 24
-	]
-
-	# Type of crypting being done
-	ENCRYPT =	0x00
-	DECRYPT =	0x01
-
-	# Initialisation
-	def __init__(self, key, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
-		# Sanity checking of arguments.
-		if len(key) != 8:
-			raise ValueError("Invalid DES key size. Key must be exactly 8 bytes long.")
-		_baseDes.__init__(self, mode, IV, pad, padmode)
-		self.key_size = 8
-
-		self.L = []
-		self.R = []
-		self.Kn = [ [0] * 48 ] * 16	# 16 48-bit keys (K1 - K16)
-		self.final = []
-
-		self.setKey(key)
-
-	def setKey(self, key):
-		"""Will set the crypting key for this object. Must be 8 bytes."""
-		_baseDes.setKey(self, key)
-		self.__create_sub_keys()
-
-	def __String_to_BitList(self, data):
-		"""Turn the string data, into a list of bits (1, 0)'s"""
-		if _pythonMajorVersion < 3:
-			# Turn the strings into integers. Python 3 uses a bytes
-			# class, which already has this behaviour.
-			data = [ord(c) for c in data]
-		l = len(data) * 8
-		result = [0] * l
-		pos = 0
-		for ch in data:
-			i = 7
-			while i >= 0:
-				if ch & (1 << i) != 0:
-					result[pos] = 1
-				else:
-					result[pos] = 0
-				pos += 1
-				i -= 1
-
-		return result
-
-	def __BitList_to_String(self, data):
-		"""Turn the list of bits -> data, into a string"""
-		result = []
-		pos = 0
-		c = 0
-		while pos < len(data):
-			c += data[pos] << (7 - (pos % 8))
-			if (pos % 8) == 7:
-				result.append(c)
-				c = 0
-			pos += 1
-
-		if _pythonMajorVersion < 3:
-			return ''.join([ chr(c) for c in result ])
-		else:
-			return bytes(result)
-
-	def __permutate(self, table, block):
-		"""Permutate this block with the specified table"""
-		return list(map(lambda x: block[x], table))
-	
-	# Transform the secret key, so that it is ready for data processing
-	# Create the 16 subkeys, K[1] - K[16]
-	def __create_sub_keys(self):
-		"""Create the 16 subkeys K[1] to K[16] from the given key"""
-		key = self.__permutate(des.__pc1, self.__String_to_BitList(self.getKey()))
-		i = 0
-		# Split into Left and Right sections
-		self.L = key[:28]
-		self.R = key[28:]
-		while i < 16:
-			j = 0
-			# Perform circular left shifts
-			while j < des.__left_rotations[i]:
-				self.L.append(self.L[0])
-				del self.L[0]
-
-				self.R.append(self.R[0])
-				del self.R[0]
-
-				j += 1
-
-			# Create one of the 16 subkeys through pc2 permutation
-			self.Kn[i] = self.__permutate(des.__pc2, self.L + self.R)
-
-			i += 1
-
-	# Main part of the encryption algorithm, the number cruncher :)
-	def __des_crypt(self, block, crypt_type):
-		"""Crypt the block of data through DES bit-manipulation"""
-		block = self.__permutate(des.__ip, block)
-		self.L = block[:32]
-		self.R = block[32:]
-
-		# Encryption starts from Kn[1] through to Kn[16]
-		if crypt_type == des.ENCRYPT:
-			iteration = 0
-			iteration_adjustment = 1
-		# Decryption starts from Kn[16] down to Kn[1]
-		else:
-			iteration = 15
-			iteration_adjustment = -1
-
-		i = 0
-		while i < 16:
-			# Make a copy of R[i-1], this will later become L[i]
-			tempR = self.R[:]
-
-			# Permutate R[i - 1] to start creating R[i]
-			self.R = self.__permutate(des.__expansion_table, self.R)
-
-			# Exclusive or R[i - 1] with K[i], create B[1] to B[8] whilst here
-			self.R = list(map(lambda x, y: x ^ y, self.R, self.Kn[iteration]))
-			B = [self.R[:6], self.R[6:12], self.R[12:18], self.R[18:24], self.R[24:30], self.R[30:36], self.R[36:42], self.R[42:]]
-			# Optimization: Replaced below commented code with above
-			#j = 0
-			#B = []
-			#while j < len(self.R):
-			#	self.R[j] = self.R[j] ^ self.Kn[iteration][j]
-			#	j += 1
-			#	if j % 6 == 0:
-			#		B.append(self.R[j-6:j])
-
-			# Permutate B[1] to B[8] using the S-Boxes
-			j = 0
-			Bn = [0] * 32
-			pos = 0
-			while j < 8:
-				# Work out the offsets
-				m = (B[j][0] << 1) + B[j][5]
-				n = (B[j][1] << 3) + (B[j][2] << 2) + (B[j][3] << 1) + B[j][4]
-
-				# Find the permutation value
-				v = des.__sbox[j][(m << 4) + n]
-
-				# Turn value into bits, add it to result: Bn
-				Bn[pos] = (v & 8) >> 3
-				Bn[pos + 1] = (v & 4) >> 2
-				Bn[pos + 2] = (v & 2) >> 1
-				Bn[pos + 3] = v & 1
-
-				pos += 4
-				j += 1
-
-			# Permutate the concatination of B[1] to B[8] (Bn)
-			self.R = self.__permutate(des.__p, Bn)
-
-			# Xor with L[i - 1]
-			self.R = list(map(lambda x, y: x ^ y, self.R, self.L))
-			# Optimization: This now replaces the below commented code
-			#j = 0
-			#while j < len(self.R):
-			#	self.R[j] = self.R[j] ^ self.L[j]
-			#	j += 1
-
-			# L[i] becomes R[i - 1]
-			self.L = tempR
-
-			i += 1
-			iteration += iteration_adjustment
-		
-		# Final permutation of R[16]L[16]
-		self.final = self.__permutate(des.__fp, self.R + self.L)
-		return self.final
-
-
-	# Data to be encrypted/decrypted
-	def crypt(self, data, crypt_type):
-		"""Crypt the data in blocks, running it through des_crypt()"""
-
-		# Error check the data
-		if not data:
-			return ''
-		if len(data) % self.block_size != 0:
-			if crypt_type == des.DECRYPT: # Decryption must work on 8 byte blocks
-				raise ValueError("Invalid data length, data must be a multiple of " + str(self.block_size) + " bytes\n.")
-			if not self.getPadding():
-				raise ValueError("Invalid data length, data must be a multiple of " + str(self.block_size) + " bytes\n. Try setting the optional padding character")
-			else:
-				data += (self.block_size - (len(data) % self.block_size)) * self.getPadding()
-			# print "Len of data: %f" % (len(data) / self.block_size)
-
-		if self.getMode() == CBC:
-			if self.getIV():
-				iv = self.__String_to_BitList(self.getIV())
-			else:
-				raise ValueError("For CBC mode, you must supply the Initial Value (IV) for ciphering")
-
-		# Split the data into blocks, crypting each one seperately
-		i = 0
-		dict = {}
-		result = []
-		#cached = 0
-		#lines = 0
-		while i < len(data):
-			# Test code for caching encryption results
-			#lines += 1
-			#if dict.has_key(data[i:i+8]):
-				#print "Cached result for: %s" % data[i:i+8]
-			#	cached += 1
-			#	result.append(dict[data[i:i+8]])
-			#	i += 8
-			#	continue
-				
-			block = self.__String_to_BitList(data[i:i+8])
-
-			# Xor with IV if using CBC mode
-			if self.getMode() == CBC:
-				if crypt_type == des.ENCRYPT:
-					block = list(map(lambda x, y: x ^ y, block, iv))
-					#j = 0
-					#while j < len(block):
-					#	block[j] = block[j] ^ iv[j]
-					#	j += 1
-
-				processed_block = self.__des_crypt(block, crypt_type)
-
-				if crypt_type == des.DECRYPT:
-					processed_block = list(map(lambda x, y: x ^ y, processed_block, iv))
-					#j = 0
-					#while j < len(processed_block):
-					#	processed_block[j] = processed_block[j] ^ iv[j]
-					#	j += 1
-					iv = block
-				else:
-					iv = processed_block
-			else:
-				processed_block = self.__des_crypt(block, crypt_type)
-
-
-			# Add the resulting crypted block to our list
-			#d = self.__BitList_to_String(processed_block)
-			#result.append(d)
-			result.append(self.__BitList_to_String(processed_block))
-			#dict[data[i:i+8]] = d
-			i += 8
-
-		# print "Lines: %d, cached: %d" % (lines, cached)
-
-		# Return the full crypted string
-		if _pythonMajorVersion < 3:
-			return ''.join(result)
-		else:
-			return bytes.fromhex('').join(result)
-
-	def encrypt(self, data, pad=None, padmode=None):
-		"""encrypt(data, [pad], [padmode]) -> bytes
-
-		data : Bytes to be encrypted
-		pad  : Optional argument for encryption padding. Must only be one byte
-		padmode : Optional argument for overriding the padding mode.
-
-		The data must be a multiple of 8 bytes and will be encrypted
-		with the already specified key. Data does not have to be a
-		multiple of 8 bytes if the padding character is supplied, or
-		the padmode is set to PAD_PKCS5, as bytes will then added to
-		ensure the be padded data is a multiple of 8 bytes.
-		"""
-		data = self._guardAgainstUnicode(data)
-		if pad is not None:
-			pad = self._guardAgainstUnicode(pad)
-		data = self._padData(data, pad, padmode)
-		return self.crypt(data, des.ENCRYPT)
-
-	def decrypt(self, data, pad=None, padmode=None):
-		"""decrypt(data, [pad], [padmode]) -> bytes
-
-		data : Bytes to be encrypted
-		pad  : Optional argument for decryption padding. Must only be one byte
-		padmode : Optional argument for overriding the padding mode.
-
-		The data must be a multiple of 8 bytes and will be decrypted
-		with the already specified key. In PAD_NORMAL mode, if the
-		optional padding character is supplied, then the un-encrypted
-		data will have the padding characters removed from the end of
-		the bytes. This pad removal only occurs on the last 8 bytes of
-		the data (last data block). In PAD_PKCS5 mode, the special
-		padding end markers will be removed from the data after decrypting.
-		"""
-		data = self._guardAgainstUnicode(data)
-		if pad is not None:
-			pad = self._guardAgainstUnicode(pad)
-		data = self.crypt(data, des.DECRYPT)
-		return self._unpadData(data, pad, padmode)
-
-
-
-#############################################################################
-# 				Triple DES				    #
-#############################################################################
-class triple_des(_baseDes):
-	"""Triple DES encryption/decrytpion class
-
-	This algorithm uses the DES-EDE3 (when a 24 byte key is supplied) or
-	the DES-EDE2 (when a 16 byte key is supplied) encryption methods.
-	Supports ECB (Electronic Code Book) and CBC (Cypher Block Chaining) modes.
-
-	pyDes.des(key, [mode], [IV])
-
-	key  -> Bytes containing the encryption key, must be either 16 or
-	        24 bytes long
-	mode -> Optional argument for encryption type, can be either pyDes.ECB
-		(Electronic Code Book), pyDes.CBC (Cypher Block Chaining)
-	IV   -> Optional Initial Value bytes, must be supplied if using CBC mode.
-		Must be 8 bytes in length.
-	pad  -> Optional argument, set the pad character (PAD_NORMAL) to use
-		during all encrypt/decrpt operations done with this instance.
-	padmode -> Optional argument, set the padding mode (PAD_NORMAL or
-		PAD_PKCS5) to use during all encrypt/decrpt operations done
-		with this instance.
-	"""
-	def __init__(self, key, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
-		_baseDes.__init__(self, mode, IV, pad, padmode)
-		self.setKey(key)
-
-	def setKey(self, key):
-		"""Will set the crypting key for this object. Either 16 or 24 bytes long."""
-		self.key_size = 24  # Use DES-EDE3 mode
-		if len(key) != self.key_size:
-			if len(key) == 16: # Use DES-EDE2 mode
-				self.key_size = 16
-			else:
-				raise ValueError("Invalid triple DES key size. Key must be either 16 or 24 bytes long")
-		if self.getMode() == CBC:
-			if not self.getIV():
-				# Use the first 8 bytes of the key
-				self._iv = key[:self.block_size]
-			if len(self.getIV()) != self.block_size:
-				raise ValueError("Invalid IV, must be 8 bytes in length")
-		self.__key1 = des(key[:8], self._mode, self._iv,
-				  self._padding, self._padmode)
-		self.__key2 = des(key[8:16], self._mode, self._iv,
-				  self._padding, self._padmode)
-		if self.key_size == 16:
-			self.__key3 = self.__key1
-		else:
-			self.__key3 = des(key[16:], self._mode, self._iv,
-					  self._padding, self._padmode)
-		_baseDes.setKey(self, key)
-
-	# Override setter methods to work on all 3 keys.
-
-	def setMode(self, mode):
-		"""Sets the type of crypting mode, pyDes.ECB or pyDes.CBC"""
-		_baseDes.setMode(self, mode)
-		for key in (self.__key1, self.__key2, self.__key3):
-			key.setMode(mode)
-
-	def setPadding(self, pad):
-		"""setPadding() -> bytes of length 1. Padding character."""
-		_baseDes.setPadding(self, pad)
-		for key in (self.__key1, self.__key2, self.__key3):
-			key.setPadding(pad)
-
-	def setPadMode(self, mode):
-		"""Sets the type of padding mode, pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
-		_baseDes.setPadMode(self, mode)
-		for key in (self.__key1, self.__key2, self.__key3):
-			key.setPadMode(mode)
-
-	def setIV(self, IV):
-		"""Will set the Initial Value, used in conjunction with CBC mode"""
-		_baseDes.setIV(self, IV)
-		for key in (self.__key1, self.__key2, self.__key3):
-			key.setIV(IV)
-
-	def encrypt(self, data, pad=None, padmode=None):
-		"""encrypt(data, [pad], [padmode]) -> bytes
-
-		data : bytes to be encrypted
-		pad  : Optional argument for encryption padding. Must only be one byte
-		padmode : Optional argument for overriding the padding mode.
-
-		The data must be a multiple of 8 bytes and will be encrypted
-		with the already specified key. Data does not have to be a
-		multiple of 8 bytes if the padding character is supplied, or
-		the padmode is set to PAD_PKCS5, as bytes will then added to
-		ensure the be padded data is a multiple of 8 bytes.
-		"""
-		ENCRYPT = des.ENCRYPT
-		DECRYPT = des.DECRYPT
-		data = self._guardAgainstUnicode(data)
-		if pad is not None:
-			pad = self._guardAgainstUnicode(pad)
-		# Pad the data accordingly.
-		data = self._padData(data, pad, padmode)
-		if self.getMode() == CBC:
-			self.__key1.setIV(self.getIV())
-			self.__key2.setIV(self.getIV())
-			self.__key3.setIV(self.getIV())
-			i = 0
-			result = []
-			while i < len(data):
-				block = self.__key1.crypt(data[i:i+8], ENCRYPT)
-				block = self.__key2.crypt(block, DECRYPT)
-				block = self.__key3.crypt(block, ENCRYPT)
-				self.__key1.setIV(block)
-				self.__key2.setIV(block)
-				self.__key3.setIV(block)
-				result.append(block)
-				i += 8
-			if _pythonMajorVersion < 3:
-				return ''.join(result)
-			else:
-				return bytes.fromhex('').join(result)
-		else:
-			data = self.__key1.crypt(data, ENCRYPT)
-			data = self.__key2.crypt(data, DECRYPT)
-			return self.__key3.crypt(data, ENCRYPT)
-
-	def decrypt(self, data, pad=None, padmode=None):
-		"""decrypt(data, [pad], [padmode]) -> bytes
-
-		data : bytes to be encrypted
-		pad  : Optional argument for decryption padding. Must only be one byte
-		padmode : Optional argument for overriding the padding mode.
-
-		The data must be a multiple of 8 bytes and will be decrypted
-		with the already specified key. In PAD_NORMAL mode, if the
-		optional padding character is supplied, then the un-encrypted
-		data will have the padding characters removed from the end of
-		the bytes. This pad removal only occurs on the last 8 bytes of
-		the data (last data block). In PAD_PKCS5 mode, the special
-		padding end markers will be removed from the data after
-		decrypting, no pad character is required for PAD_PKCS5.
-		"""
-		ENCRYPT = des.ENCRYPT
-		DECRYPT = des.DECRYPT
-		data = self._guardAgainstUnicode(data)
-		if pad is not None:
-			pad = self._guardAgainstUnicode(pad)
-		if self.getMode() == CBC:
-			self.__key1.setIV(self.getIV())
-			self.__key2.setIV(self.getIV())
-			self.__key3.setIV(self.getIV())
-			i = 0
-			result = []
-			while i < len(data):
-				iv = data[i:i+8]
-				block = self.__key3.crypt(iv,    DECRYPT)
-				block = self.__key2.crypt(block, ENCRYPT)
-				block = self.__key1.crypt(block, DECRYPT)
-				self.__key1.setIV(iv)
-				self.__key2.setIV(iv)
-				self.__key3.setIV(iv)
-				result.append(block)
-				i += 8
-			if _pythonMajorVersion < 3:
-				data = ''.join(result)
-			else:
-				data = bytes.fromhex('').join(result)
-		else:
-			data = self.__key3.crypt(data, DECRYPT)
-			data = self.__key2.crypt(data, ENCRYPT)
-			data = self.__key1.crypt(data, DECRYPT)
-		return self._unpadData(data, pad, padmode)
+#############################################################################
+# 				Documentation				    #
+#############################################################################
+
+# Author:   Todd Whiteman
+# Date:     16th March, 2009
+# Verion:   2.0.0
+# License:  Public Domain - free to do as you wish
+# Homepage: http://twhiteman.netfirms.com/des.html
+#
+# This is a pure python implementation of the DES encryption algorithm.
+# It's pure python to avoid portability issues, since most DES 
+# implementations are programmed in C (for performance reasons).
+#
+# Triple DES class is also implemented, utilising the DES base. Triple DES
+# is either DES-EDE3 with a 24 byte key, or DES-EDE2 with a 16 byte key.
+#
+# See the README.txt that should come with this python module for the
+# implementation methods used.
+#
+# Thanks to:
+#  * David Broadwell for ideas, comments and suggestions.
+#  * Mario Wolff for pointing out and debugging some triple des CBC errors.
+#  * Santiago Palladino for providing the PKCS5 padding technique.
+#  * Shaya for correcting the PAD_PKCS5 triple des CBC errors.
+#
+"""A pure python implementation of the DES and TRIPLE DES encryption algorithms.
+
+Class initialization
+--------------------
+pyDes.des(key, [mode], [IV], [pad], [padmode])
+pyDes.triple_des(key, [mode], [IV], [pad], [padmode])
+
+key     -> Bytes containing the encryption key. 8 bytes for DES, 16 or 24 bytes
+	   for Triple DES
+mode    -> Optional argument for encryption type, can be either
+	   pyDes.ECB (Electronic Code Book) or pyDes.CBC (Cypher Block Chaining)
+IV      -> Optional Initial Value bytes, must be supplied if using CBC mode.
+	   Length must be 8 bytes.
+pad     -> Optional argument, set the pad character (PAD_NORMAL) to use during
+	   all encrypt/decrpt operations done with this instance.
+padmode -> Optional argument, set the padding mode (PAD_NORMAL or PAD_PKCS5)
+	   to use during all encrypt/decrpt operations done with this instance.
+
+I recommend to use PAD_PKCS5 padding, as then you never need to worry about any
+padding issues, as the padding can be removed unambiguously upon decrypting
+data that was encrypted using PAD_PKCS5 padmode.
+
+Common methods
+--------------
+encrypt(data, [pad], [padmode])
+decrypt(data, [pad], [padmode])
+
+data    -> Bytes to be encrypted/decrypted
+pad     -> Optional argument. Only when using padmode of PAD_NORMAL. For
+	   encryption, adds this characters to the end of the data block when
+	   data is not a multiple of 8 bytes. For decryption, will remove the
+	   trailing characters that match this pad character from the last 8
+	   bytes of the unencrypted data block.
+padmode -> Optional argument, set the padding mode, must be one of PAD_NORMAL
+	   or PAD_PKCS5). Defaults to PAD_NORMAL.
+	  
+
+Example
+-------
+from pyDes import *
+
+data = "Please encrypt my data"
+k = des("DESCRYPT", CBC, "\0\0\0\0\0\0\0\0", pad=None, padmode=PAD_PKCS5)
+# For Python3, you'll need to use bytes, i.e.:
+#   data = b"Please encrypt my data"
+#   k = des(b"DESCRYPT", CBC, b"\0\0\0\0\0\0\0\0", pad=None, padmode=PAD_PKCS5)
+d = k.encrypt(data)
+print "Encrypted: %r" % d
+print "Decrypted: %r" % k.decrypt(d)
+assert k.decrypt(d, padmode=PAD_PKCS5) == data
+
+
+See the module source (pyDes.py) for more examples of use.
+You can also run the pyDes.py file without and arguments to see a simple test.
+
+Note: This code was not written for high-end systems needing a fast
+      implementation, but rather a handy portable solution with small usage.
+
+"""
+
+import sys
+
+# _pythonMajorVersion is used to handle Python2 and Python3 differences.
+_pythonMajorVersion = sys.version_info[0]
+
+# Modes of crypting / cyphering
+ECB =	0
+CBC =	1
+
+# Modes of padding
+PAD_NORMAL = 1
+PAD_PKCS5 = 2
+
+# PAD_PKCS5: is a method that will unambiguously remove all padding
+#            characters after decryption, when originally encrypted with
+#            this padding mode.
+# For a good description of the PKCS5 padding technique, see:
+# http://www.faqs.org/rfcs/rfc1423.html
+
+# The base class shared by des and triple des.
+class _baseDes(object):
+	def __init__(self, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
+		if IV:
+			IV = self._guardAgainstUnicode(IV)
+		if pad:
+			pad = self._guardAgainstUnicode(pad)
+		self.block_size = 8
+		# Sanity checking of arguments.
+		if pad and padmode == PAD_PKCS5:
+			raise ValueError("Cannot use a pad character with PAD_PKCS5")
+		if IV and len(IV) != self.block_size:
+			raise ValueError("Invalid Initial Value (IV), must be a multiple of " + str(self.block_size) + " bytes")
+
+		# Set the passed in variables
+		self._mode = mode
+		self._iv = IV
+		self._padding = pad
+		self._padmode = padmode
+
+	def getKey(self):
+		"""getKey() -> bytes"""
+		return self.__key
+
+	def setKey(self, key):
+		"""Will set the crypting key for this object."""
+		key = self._guardAgainstUnicode(key)
+		self.__key = key
+
+	def getMode(self):
+		"""getMode() -> pyDes.ECB or pyDes.CBC"""
+		return self._mode
+
+	def setMode(self, mode):
+		"""Sets the type of crypting mode, pyDes.ECB or pyDes.CBC"""
+		self._mode = mode
+
+	def getPadding(self):
+		"""getPadding() -> bytes of length 1. Padding character."""
+		return self._padding
+
+	def setPadding(self, pad):
+		"""setPadding() -> bytes of length 1. Padding character."""
+		if pad is not None:
+			pad = self._guardAgainstUnicode(pad)
+		self._padding = pad
+
+	def getPadMode(self):
+		"""getPadMode() -> pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
+		return self._padmode
+		
+	def setPadMode(self, mode):
+		"""Sets the type of padding mode, pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
+		self._padmode = mode
+
+	def getIV(self):
+		"""getIV() -> bytes"""
+		return self._iv
+
+	def setIV(self, IV):
+		"""Will set the Initial Value, used in conjunction with CBC mode"""
+		if not IV or len(IV) != self.block_size:
+			raise ValueError("Invalid Initial Value (IV), must be a multiple of " + str(self.block_size) + " bytes")
+		IV = self._guardAgainstUnicode(IV)
+		self._iv = IV
+
+	def _padData(self, data, pad, padmode):
+		# Pad data depending on the mode
+		if padmode is None:
+			# Get the default padding mode.
+			padmode = self.getPadMode()
+		if pad and padmode == PAD_PKCS5:
+			raise ValueError("Cannot use a pad character with PAD_PKCS5")
+
+		if padmode == PAD_NORMAL:
+			if len(data) % self.block_size == 0:
+				# No padding required.
+				return data
+
+			if not pad:
+				# Get the default padding.
+				pad = self.getPadding()
+			if not pad:
+				raise ValueError("Data must be a multiple of " + str(self.block_size) + " bytes in length. Use padmode=PAD_PKCS5 or set the pad character.")
+			data += (self.block_size - (len(data) % self.block_size)) * pad
+		
+		elif padmode == PAD_PKCS5:
+			pad_len = 8 - (len(data) % self.block_size)
+			if _pythonMajorVersion < 3:
+				data += pad_len * chr(pad_len)
+			else:
+				data += bytes([pad_len] * pad_len)
+
+		return data
+
+	def _unpadData(self, data, pad, padmode):
+		# Unpad data depending on the mode.
+		if not data:
+			return data
+		if pad and padmode == PAD_PKCS5:
+			raise ValueError("Cannot use a pad character with PAD_PKCS5")
+		if padmode is None:
+			# Get the default padding mode.
+			padmode = self.getPadMode()
+
+		if padmode == PAD_NORMAL:
+			if not pad:
+				# Get the default padding.
+				pad = self.getPadding()
+			if pad:
+				data = data[:-self.block_size] + \
+				       data[-self.block_size:].rstrip(pad)
+
+		elif padmode == PAD_PKCS5:
+			if _pythonMajorVersion < 3:
+				pad_len = ord(data[-1])
+			else:
+				pad_len = data[-1]
+			data = data[:-pad_len]
+
+		return data
+
+	def _guardAgainstUnicode(self, data):
+		# Only accept byte strings or ascii unicode values, otherwise
+		# there is no way to correctly decode the data into bytes.
+		if _pythonMajorVersion < 3:
+			if isinstance(data, unicode):
+				raise ValueError("pyDes can only work with bytes, not Unicode strings.")
+		else:
+			if isinstance(data, str):
+				# Only accept ascii unicode values.
+				try:
+					return data.encode('ascii')
+				except UnicodeEncodeError:
+					pass
+				raise ValueError("pyDes can only work with encoded strings, not Unicode.")
+		return data
+
+#############################################################################
+# 				    DES					    #
+#############################################################################
+class des(_baseDes):
+	"""DES encryption/decrytpion class
+
+	Supports ECB (Electronic Code Book) and CBC (Cypher Block Chaining) modes.
+
+	pyDes.des(key,[mode], [IV])
+
+	key  -> Bytes containing the encryption key, must be exactly 8 bytes
+	mode -> Optional argument for encryption type, can be either pyDes.ECB
+		(Electronic Code Book), pyDes.CBC (Cypher Block Chaining)
+	IV   -> Optional Initial Value bytes, must be supplied if using CBC mode.
+		Must be 8 bytes in length.
+	pad  -> Optional argument, set the pad character (PAD_NORMAL) to use
+		during all encrypt/decrpt operations done with this instance.
+	padmode -> Optional argument, set the padding mode (PAD_NORMAL or
+		PAD_PKCS5) to use during all encrypt/decrpt operations done
+		with this instance.
+	"""
+
+
+	# Permutation and translation tables for DES
+	__pc1 = [56, 48, 40, 32, 24, 16,  8,
+		  0, 57, 49, 41, 33, 25, 17,
+		  9,  1, 58, 50, 42, 34, 26,
+		 18, 10,  2, 59, 51, 43, 35,
+		 62, 54, 46, 38, 30, 22, 14,
+		  6, 61, 53, 45, 37, 29, 21,
+		 13,  5, 60, 52, 44, 36, 28,
+		 20, 12,  4, 27, 19, 11,  3
+	]
+
+	# number left rotations of pc1
+	__left_rotations = [
+		1, 1, 2, 2, 2, 2, 2, 2, 1, 2, 2, 2, 2, 2, 2, 1
+	]
+
+	# permuted choice key (table 2)
+	__pc2 = [
+		13, 16, 10, 23,  0,  4,
+		 2, 27, 14,  5, 20,  9,
+		22, 18, 11,  3, 25,  7,
+		15,  6, 26, 19, 12,  1,
+		40, 51, 30, 36, 46, 54,
+		29, 39, 50, 44, 32, 47,
+		43, 48, 38, 55, 33, 52,
+		45, 41, 49, 35, 28, 31
+	]
+
+	# initial permutation IP
+	__ip = [57, 49, 41, 33, 25, 17, 9,  1,
+		59, 51, 43, 35, 27, 19, 11, 3,
+		61, 53, 45, 37, 29, 21, 13, 5,
+		63, 55, 47, 39, 31, 23, 15, 7,
+		56, 48, 40, 32, 24, 16, 8,  0,
+		58, 50, 42, 34, 26, 18, 10, 2,
+		60, 52, 44, 36, 28, 20, 12, 4,
+		62, 54, 46, 38, 30, 22, 14, 6
+	]
+
+	# Expansion table for turning 32 bit blocks into 48 bits
+	__expansion_table = [
+		31,  0,  1,  2,  3,  4,
+		 3,  4,  5,  6,  7,  8,
+		 7,  8,  9, 10, 11, 12,
+		11, 12, 13, 14, 15, 16,
+		15, 16, 17, 18, 19, 20,
+		19, 20, 21, 22, 23, 24,
+		23, 24, 25, 26, 27, 28,
+		27, 28, 29, 30, 31,  0
+	]
+
+	# The (in)famous S-boxes
+	__sbox = [
+		# S1
+		[14, 4, 13, 1, 2, 15, 11, 8, 3, 10, 6, 12, 5, 9, 0, 7,
+		 0, 15, 7, 4, 14, 2, 13, 1, 10, 6, 12, 11, 9, 5, 3, 8,
+		 4, 1, 14, 8, 13, 6, 2, 11, 15, 12, 9, 7, 3, 10, 5, 0,
+		 15, 12, 8, 2, 4, 9, 1, 7, 5, 11, 3, 14, 10, 0, 6, 13],
+
+		# S2
+		[15, 1, 8, 14, 6, 11, 3, 4, 9, 7, 2, 13, 12, 0, 5, 10,
+		 3, 13, 4, 7, 15, 2, 8, 14, 12, 0, 1, 10, 6, 9, 11, 5,
+		 0, 14, 7, 11, 10, 4, 13, 1, 5, 8, 12, 6, 9, 3, 2, 15,
+		 13, 8, 10, 1, 3, 15, 4, 2, 11, 6, 7, 12, 0, 5, 14, 9],
+
+		# S3
+		[10, 0, 9, 14, 6, 3, 15, 5, 1, 13, 12, 7, 11, 4, 2, 8,
+		 13, 7, 0, 9, 3, 4, 6, 10, 2, 8, 5, 14, 12, 11, 15, 1,
+		 13, 6, 4, 9, 8, 15, 3, 0, 11, 1, 2, 12, 5, 10, 14, 7,
+		 1, 10, 13, 0, 6, 9, 8, 7, 4, 15, 14, 3, 11, 5, 2, 12],
+
+		# S4
+		[7, 13, 14, 3, 0, 6, 9, 10, 1, 2, 8, 5, 11, 12, 4, 15,
+		 13, 8, 11, 5, 6, 15, 0, 3, 4, 7, 2, 12, 1, 10, 14, 9,
+		 10, 6, 9, 0, 12, 11, 7, 13, 15, 1, 3, 14, 5, 2, 8, 4,
+		 3, 15, 0, 6, 10, 1, 13, 8, 9, 4, 5, 11, 12, 7, 2, 14],
+
+		# S5
+		[2, 12, 4, 1, 7, 10, 11, 6, 8, 5, 3, 15, 13, 0, 14, 9,
+		 14, 11, 2, 12, 4, 7, 13, 1, 5, 0, 15, 10, 3, 9, 8, 6,
+		 4, 2, 1, 11, 10, 13, 7, 8, 15, 9, 12, 5, 6, 3, 0, 14,
+		 11, 8, 12, 7, 1, 14, 2, 13, 6, 15, 0, 9, 10, 4, 5, 3],
+
+		# S6
+		[12, 1, 10, 15, 9, 2, 6, 8, 0, 13, 3, 4, 14, 7, 5, 11,
+		 10, 15, 4, 2, 7, 12, 9, 5, 6, 1, 13, 14, 0, 11, 3, 8,
+		 9, 14, 15, 5, 2, 8, 12, 3, 7, 0, 4, 10, 1, 13, 11, 6,
+		 4, 3, 2, 12, 9, 5, 15, 10, 11, 14, 1, 7, 6, 0, 8, 13],
+
+		# S7
+		[4, 11, 2, 14, 15, 0, 8, 13, 3, 12, 9, 7, 5, 10, 6, 1,
+		 13, 0, 11, 7, 4, 9, 1, 10, 14, 3, 5, 12, 2, 15, 8, 6,
+		 1, 4, 11, 13, 12, 3, 7, 14, 10, 15, 6, 8, 0, 5, 9, 2,
+		 6, 11, 13, 8, 1, 4, 10, 7, 9, 5, 0, 15, 14, 2, 3, 12],
+
+		# S8
+		[13, 2, 8, 4, 6, 15, 11, 1, 10, 9, 3, 14, 5, 0, 12, 7,
+		 1, 15, 13, 8, 10, 3, 7, 4, 12, 5, 6, 11, 0, 14, 9, 2,
+		 7, 11, 4, 1, 9, 12, 14, 2, 0, 6, 10, 13, 15, 3, 5, 8,
+		 2, 1, 14, 7, 4, 10, 8, 13, 15, 12, 9, 0, 3, 5, 6, 11],
+	]
+
+
+	# 32-bit permutation function P used on the output of the S-boxes
+	__p = [
+		15, 6, 19, 20, 28, 11,
+		27, 16, 0, 14, 22, 25,
+		4, 17, 30, 9, 1, 7,
+		23,13, 31, 26, 2, 8,
+		18, 12, 29, 5, 21, 10,
+		3, 24
+	]
+
+	# final permutation IP^-1
+	__fp = [
+		39,  7, 47, 15, 55, 23, 63, 31,
+		38,  6, 46, 14, 54, 22, 62, 30,
+		37,  5, 45, 13, 53, 21, 61, 29,
+		36,  4, 44, 12, 52, 20, 60, 28,
+		35,  3, 43, 11, 51, 19, 59, 27,
+		34,  2, 42, 10, 50, 18, 58, 26,
+		33,  1, 41,  9, 49, 17, 57, 25,
+		32,  0, 40,  8, 48, 16, 56, 24
+	]
+
+	# Type of crypting being done
+	ENCRYPT =	0x00
+	DECRYPT =	0x01
+
+	# Initialisation
+	def __init__(self, key, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
+		# Sanity checking of arguments.
+		if len(key) != 8:
+			raise ValueError("Invalid DES key size. Key must be exactly 8 bytes long.")
+		_baseDes.__init__(self, mode, IV, pad, padmode)
+		self.key_size = 8
+
+		self.L = []
+		self.R = []
+		self.Kn = [ [0] * 48 ] * 16	# 16 48-bit keys (K1 - K16)
+		self.final = []
+
+		self.setKey(key)
+
+	def setKey(self, key):
+		"""Will set the crypting key for this object. Must be 8 bytes."""
+		_baseDes.setKey(self, key)
+		self.__create_sub_keys()
+
+	def __String_to_BitList(self, data):
+		"""Turn the string data, into a list of bits (1, 0)'s"""
+		if _pythonMajorVersion < 3:
+			# Turn the strings into integers. Python 3 uses a bytes
+			# class, which already has this behaviour.
+			data = [ord(c) for c in data]
+		l = len(data) * 8
+		result = [0] * l
+		pos = 0
+		for ch in data:
+			i = 7
+			while i >= 0:
+				if ch & (1 << i) != 0:
+					result[pos] = 1
+				else:
+					result[pos] = 0
+				pos += 1
+				i -= 1
+
+		return result
+
+	def __BitList_to_String(self, data):
+		"""Turn the list of bits -> data, into a string"""
+		result = []
+		pos = 0
+		c = 0
+		while pos < len(data):
+			c += data[pos] << (7 - (pos % 8))
+			if (pos % 8) == 7:
+				result.append(c)
+				c = 0
+			pos += 1
+
+		if _pythonMajorVersion < 3:
+			return ''.join([ chr(c) for c in result ])
+		else:
+			return bytes(result)
+
+	def __permutate(self, table, block):
+		"""Permutate this block with the specified table"""
+		return list(map(lambda x: block[x], table))
+	
+	# Transform the secret key, so that it is ready for data processing
+	# Create the 16 subkeys, K[1] - K[16]
+	def __create_sub_keys(self):
+		"""Create the 16 subkeys K[1] to K[16] from the given key"""
+		key = self.__permutate(des.__pc1, self.__String_to_BitList(self.getKey()))
+		i = 0
+		# Split into Left and Right sections
+		self.L = key[:28]
+		self.R = key[28:]
+		while i < 16:
+			j = 0
+			# Perform circular left shifts
+			while j < des.__left_rotations[i]:
+				self.L.append(self.L[0])
+				del self.L[0]
+
+				self.R.append(self.R[0])
+				del self.R[0]
+
+				j += 1
+
+			# Create one of the 16 subkeys through pc2 permutation
+			self.Kn[i] = self.__permutate(des.__pc2, self.L + self.R)
+
+			i += 1
+
+	# Main part of the encryption algorithm, the number cruncher :)
+	def __des_crypt(self, block, crypt_type):
+		"""Crypt the block of data through DES bit-manipulation"""
+		block = self.__permutate(des.__ip, block)
+		self.L = block[:32]
+		self.R = block[32:]
+
+		# Encryption starts from Kn[1] through to Kn[16]
+		if crypt_type == des.ENCRYPT:
+			iteration = 0
+			iteration_adjustment = 1
+		# Decryption starts from Kn[16] down to Kn[1]
+		else:
+			iteration = 15
+			iteration_adjustment = -1
+
+		i = 0
+		while i < 16:
+			# Make a copy of R[i-1], this will later become L[i]
+			tempR = self.R[:]
+
+			# Permutate R[i - 1] to start creating R[i]
+			self.R = self.__permutate(des.__expansion_table, self.R)
+
+			# Exclusive or R[i - 1] with K[i], create B[1] to B[8] whilst here
+			self.R = list(map(lambda x, y: x ^ y, self.R, self.Kn[iteration]))
+			B = [self.R[:6], self.R[6:12], self.R[12:18], self.R[18:24], self.R[24:30], self.R[30:36], self.R[36:42], self.R[42:]]
+			# Optimization: Replaced below commented code with above
+			#j = 0
+			#B = []
+			#while j < len(self.R):
+			#	self.R[j] = self.R[j] ^ self.Kn[iteration][j]
+			#	j += 1
+			#	if j % 6 == 0:
+			#		B.append(self.R[j-6:j])
+
+			# Permutate B[1] to B[8] using the S-Boxes
+			j = 0
+			Bn = [0] * 32
+			pos = 0
+			while j < 8:
+				# Work out the offsets
+				m = (B[j][0] << 1) + B[j][5]
+				n = (B[j][1] << 3) + (B[j][2] << 2) + (B[j][3] << 1) + B[j][4]
+
+				# Find the permutation value
+				v = des.__sbox[j][(m << 4) + n]
+
+				# Turn value into bits, add it to result: Bn
+				Bn[pos] = (v & 8) >> 3
+				Bn[pos + 1] = (v & 4) >> 2
+				Bn[pos + 2] = (v & 2) >> 1
+				Bn[pos + 3] = v & 1
+
+				pos += 4
+				j += 1
+
+			# Permutate the concatination of B[1] to B[8] (Bn)
+			self.R = self.__permutate(des.__p, Bn)
+
+			# Xor with L[i - 1]
+			self.R = list(map(lambda x, y: x ^ y, self.R, self.L))
+			# Optimization: This now replaces the below commented code
+			#j = 0
+			#while j < len(self.R):
+			#	self.R[j] = self.R[j] ^ self.L[j]
+			#	j += 1
+
+			# L[i] becomes R[i - 1]
+			self.L = tempR
+
+			i += 1
+			iteration += iteration_adjustment
+		
+		# Final permutation of R[16]L[16]
+		self.final = self.__permutate(des.__fp, self.R + self.L)
+		return self.final
+
+
+	# Data to be encrypted/decrypted
+	def crypt(self, data, crypt_type):
+		"""Crypt the data in blocks, running it through des_crypt()"""
+
+		# Error check the data
+		if not data:
+			return ''
+		if len(data) % self.block_size != 0:
+			if crypt_type == des.DECRYPT: # Decryption must work on 8 byte blocks
+				raise ValueError("Invalid data length, data must be a multiple of " + str(self.block_size) + " bytes\n.")
+			if not self.getPadding():
+				raise ValueError("Invalid data length, data must be a multiple of " + str(self.block_size) + " bytes\n. Try setting the optional padding character")
+			else:
+				data += (self.block_size - (len(data) % self.block_size)) * self.getPadding()
+			# print "Len of data: %f" % (len(data) / self.block_size)
+
+		if self.getMode() == CBC:
+			if self.getIV():
+				iv = self.__String_to_BitList(self.getIV())
+			else:
+				raise ValueError("For CBC mode, you must supply the Initial Value (IV) for ciphering")
+
+		# Split the data into blocks, crypting each one seperately
+		i = 0
+		dict = {}
+		result = []
+		#cached = 0
+		#lines = 0
+		while i < len(data):
+			# Test code for caching encryption results
+			#lines += 1
+			#if dict.has_key(data[i:i+8]):
+				#print "Cached result for: %s" % data[i:i+8]
+			#	cached += 1
+			#	result.append(dict[data[i:i+8]])
+			#	i += 8
+			#	continue
+				
+			block = self.__String_to_BitList(data[i:i+8])
+
+			# Xor with IV if using CBC mode
+			if self.getMode() == CBC:
+				if crypt_type == des.ENCRYPT:
+					block = list(map(lambda x, y: x ^ y, block, iv))
+					#j = 0
+					#while j < len(block):
+					#	block[j] = block[j] ^ iv[j]
+					#	j += 1
+
+				processed_block = self.__des_crypt(block, crypt_type)
+
+				if crypt_type == des.DECRYPT:
+					processed_block = list(map(lambda x, y: x ^ y, processed_block, iv))
+					#j = 0
+					#while j < len(processed_block):
+					#	processed_block[j] = processed_block[j] ^ iv[j]
+					#	j += 1
+					iv = block
+				else:
+					iv = processed_block
+			else:
+				processed_block = self.__des_crypt(block, crypt_type)
+
+
+			# Add the resulting crypted block to our list
+			#d = self.__BitList_to_String(processed_block)
+			#result.append(d)
+			result.append(self.__BitList_to_String(processed_block))
+			#dict[data[i:i+8]] = d
+			i += 8
+
+		# print "Lines: %d, cached: %d" % (lines, cached)
+
+		# Return the full crypted string
+		if _pythonMajorVersion < 3:
+			return ''.join(result)
+		else:
+			return bytes.fromhex('').join(result)
+
+	def encrypt(self, data, pad=None, padmode=None):
+		"""encrypt(data, [pad], [padmode]) -> bytes
+
+		data : Bytes to be encrypted
+		pad  : Optional argument for encryption padding. Must only be one byte
+		padmode : Optional argument for overriding the padding mode.
+
+		The data must be a multiple of 8 bytes and will be encrypted
+		with the already specified key. Data does not have to be a
+		multiple of 8 bytes if the padding character is supplied, or
+		the padmode is set to PAD_PKCS5, as bytes will then added to
+		ensure the be padded data is a multiple of 8 bytes.
+		"""
+		data = self._guardAgainstUnicode(data)
+		if pad is not None:
+			pad = self._guardAgainstUnicode(pad)
+		data = self._padData(data, pad, padmode)
+		return self.crypt(data, des.ENCRYPT)
+
+	def decrypt(self, data, pad=None, padmode=None):
+		"""decrypt(data, [pad], [padmode]) -> bytes
+
+		data : Bytes to be encrypted
+		pad  : Optional argument for decryption padding. Must only be one byte
+		padmode : Optional argument for overriding the padding mode.
+
+		The data must be a multiple of 8 bytes and will be decrypted
+		with the already specified key. In PAD_NORMAL mode, if the
+		optional padding character is supplied, then the un-encrypted
+		data will have the padding characters removed from the end of
+		the bytes. This pad removal only occurs on the last 8 bytes of
+		the data (last data block). In PAD_PKCS5 mode, the special
+		padding end markers will be removed from the data after decrypting.
+		"""
+		data = self._guardAgainstUnicode(data)
+		if pad is not None:
+			pad = self._guardAgainstUnicode(pad)
+		data = self.crypt(data, des.DECRYPT)
+		return self._unpadData(data, pad, padmode)
+
+
+
+#############################################################################
+# 				Triple DES				    #
+#############################################################################
+class triple_des(_baseDes):
+	"""Triple DES encryption/decrytpion class
+
+	This algorithm uses the DES-EDE3 (when a 24 byte key is supplied) or
+	the DES-EDE2 (when a 16 byte key is supplied) encryption methods.
+	Supports ECB (Electronic Code Book) and CBC (Cypher Block Chaining) modes.
+
+	pyDes.des(key, [mode], [IV])
+
+	key  -> Bytes containing the encryption key, must be either 16 or
+	        24 bytes long
+	mode -> Optional argument for encryption type, can be either pyDes.ECB
+		(Electronic Code Book), pyDes.CBC (Cypher Block Chaining)
+	IV   -> Optional Initial Value bytes, must be supplied if using CBC mode.
+		Must be 8 bytes in length.
+	pad  -> Optional argument, set the pad character (PAD_NORMAL) to use
+		during all encrypt/decrpt operations done with this instance.
+	padmode -> Optional argument, set the padding mode (PAD_NORMAL or
+		PAD_PKCS5) to use during all encrypt/decrpt operations done
+		with this instance.
+	"""
+	def __init__(self, key, mode=ECB, IV=None, pad=None, padmode=PAD_NORMAL):
+		_baseDes.__init__(self, mode, IV, pad, padmode)
+		self.setKey(key)
+
+	def setKey(self, key):
+		"""Will set the crypting key for this object. Either 16 or 24 bytes long."""
+		self.key_size = 24  # Use DES-EDE3 mode
+		if len(key) != self.key_size:
+			if len(key) == 16: # Use DES-EDE2 mode
+				self.key_size = 16
+			else:
+				raise ValueError("Invalid triple DES key size. Key must be either 16 or 24 bytes long")
+		if self.getMode() == CBC:
+			if not self.getIV():
+				# Use the first 8 bytes of the key
+				self._iv = key[:self.block_size]
+			if len(self.getIV()) != self.block_size:
+				raise ValueError("Invalid IV, must be 8 bytes in length")
+		self.__key1 = des(key[:8], self._mode, self._iv,
+				  self._padding, self._padmode)
+		self.__key2 = des(key[8:16], self._mode, self._iv,
+				  self._padding, self._padmode)
+		if self.key_size == 16:
+			self.__key3 = self.__key1
+		else:
+			self.__key3 = des(key[16:], self._mode, self._iv,
+					  self._padding, self._padmode)
+		_baseDes.setKey(self, key)
+
+	# Override setter methods to work on all 3 keys.
+
+	def setMode(self, mode):
+		"""Sets the type of crypting mode, pyDes.ECB or pyDes.CBC"""
+		_baseDes.setMode(self, mode)
+		for key in (self.__key1, self.__key2, self.__key3):
+			key.setMode(mode)
+
+	def setPadding(self, pad):
+		"""setPadding() -> bytes of length 1. Padding character."""
+		_baseDes.setPadding(self, pad)
+		for key in (self.__key1, self.__key2, self.__key3):
+			key.setPadding(pad)
+
+	def setPadMode(self, mode):
+		"""Sets the type of padding mode, pyDes.PAD_NORMAL or pyDes.PAD_PKCS5"""
+		_baseDes.setPadMode(self, mode)
+		for key in (self.__key1, self.__key2, self.__key3):
+			key.setPadMode(mode)
+
+	def setIV(self, IV):
+		"""Will set the Initial Value, used in conjunction with CBC mode"""
+		_baseDes.setIV(self, IV)
+		for key in (self.__key1, self.__key2, self.__key3):
+			key.setIV(IV)
+
+	def encrypt(self, data, pad=None, padmode=None):
+		"""encrypt(data, [pad], [padmode]) -> bytes
+
+		data : bytes to be encrypted
+		pad  : Optional argument for encryption padding. Must only be one byte
+		padmode : Optional argument for overriding the padding mode.
+
+		The data must be a multiple of 8 bytes and will be encrypted
+		with the already specified key. Data does not have to be a
+		multiple of 8 bytes if the padding character is supplied, or
+		the padmode is set to PAD_PKCS5, as bytes will then added to
+		ensure the be padded data is a multiple of 8 bytes.
+		"""
+		ENCRYPT = des.ENCRYPT
+		DECRYPT = des.DECRYPT
+		data = self._guardAgainstUnicode(data)
+		if pad is not None:
+			pad = self._guardAgainstUnicode(pad)
+		# Pad the data accordingly.
+		data = self._padData(data, pad, padmode)
+		if self.getMode() == CBC:
+			self.__key1.setIV(self.getIV())
+			self.__key2.setIV(self.getIV())
+			self.__key3.setIV(self.getIV())
+			i = 0
+			result = []
+			while i < len(data):
+				block = self.__key1.crypt(data[i:i+8], ENCRYPT)
+				block = self.__key2.crypt(block, DECRYPT)
+				block = self.__key3.crypt(block, ENCRYPT)
+				self.__key1.setIV(block)
+				self.__key2.setIV(block)
+				self.__key3.setIV(block)
+				result.append(block)
+				i += 8
+			if _pythonMajorVersion < 3:
+				return ''.join(result)
+			else:
+				return bytes.fromhex('').join(result)
+		else:
+			data = self.__key1.crypt(data, ENCRYPT)
+			data = self.__key2.crypt(data, DECRYPT)
+			return self.__key3.crypt(data, ENCRYPT)
+
+	def decrypt(self, data, pad=None, padmode=None):
+		"""decrypt(data, [pad], [padmode]) -> bytes
+
+		data : bytes to be encrypted
+		pad  : Optional argument for decryption padding. Must only be one byte
+		padmode : Optional argument for overriding the padding mode.
+
+		The data must be a multiple of 8 bytes and will be decrypted
+		with the already specified key. In PAD_NORMAL mode, if the
+		optional padding character is supplied, then the un-encrypted
+		data will have the padding characters removed from the end of
+		the bytes. This pad removal only occurs on the last 8 bytes of
+		the data (last data block). In PAD_PKCS5 mode, the special
+		padding end markers will be removed from the data after
+		decrypting, no pad character is required for PAD_PKCS5.
+		"""
+		ENCRYPT = des.ENCRYPT
+		DECRYPT = des.DECRYPT
+		data = self._guardAgainstUnicode(data)
+		if pad is not None:
+			pad = self._guardAgainstUnicode(pad)
+		if self.getMode() == CBC:
+			self.__key1.setIV(self.getIV())
+			self.__key2.setIV(self.getIV())
+			self.__key3.setIV(self.getIV())
+			i = 0
+			result = []
+			while i < len(data):
+				iv = data[i:i+8]
+				block = self.__key3.crypt(iv,    DECRYPT)
+				block = self.__key2.crypt(block, ENCRYPT)
+				block = self.__key1.crypt(block, DECRYPT)
+				self.__key1.setIV(iv)
+				self.__key2.setIV(iv)
+				self.__key3.setIV(iv)
+				result.append(block)
+				i += 8
+			if _pythonMajorVersion < 3:
+				data = ''.join(result)
+			else:
+				data = bytes.fromhex('').join(result)
+		else:
+			data = self.__key3.crypt(data, DECRYPT)
+			data = self.__key2.crypt(data, ENCRYPT)
+			data = self.__key1.crypt(data, DECRYPT)
+		return self._unpadData(data, pad, padmode)
```

### Comparing `python-tds-1.9.0/pytds/tz.py` & `python-tds-1.9.1/pytds/tz.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import time as _time
-from datetime import tzinfo, timedelta
-
-ZERO = timedelta(0)
-HOUR = timedelta(hours=1)
-
-
-class UTC(tzinfo):
-    """UTC"""
-
-    def utcoffset(self, dt):
-        return ZERO
-
-    def tzname(self, dt):
-        return "UTC"
-
-    def dst(self, dt):
-        return ZERO
-
-utc = UTC()
-
-# A class building tzinfo objects for fixed-offset time zones.
-# Note that FixedOffset(0, "UTC") is a different way to build a
-# UTC tzinfo object.
-
-
-class FixedOffsetTimezone(tzinfo):
-    """Fixed offset in minutes east from UTC."""
-
-    def __init__(self, offset, name=None):
-        self.__offset = timedelta(minutes=offset)
-        self.__name = name
-
-    def utcoffset(self, dt):
-        return self.__offset
-
-    def tzname(self, dt):
-        return self.__name
-
-    def dst(self, dt):
-        return ZERO
-
-
-STDOFFSET = timedelta(seconds=-_time.timezone)
-if _time.daylight:
-    DSTOFFSET = timedelta(seconds=-_time.altzone)
-else:
-    DSTOFFSET = STDOFFSET
-
-DSTDIFF = DSTOFFSET - STDOFFSET
-
-
-class LocalTimezone(tzinfo):
-
-    def utcoffset(self, dt):
-        if self._isdst(dt):
-            return DSTOFFSET
-        else:
-            return STDOFFSET
-
-    def dst(self, dt):
-        if self._isdst(dt):
-            return DSTDIFF
-        else:
-            return ZERO
-
-    def tzname(self, dt):
-        return _time.tzname[self._isdst(dt)]
-
-    def _isdst(self, dt):
-        tt = (dt.year, dt.month, dt.day,
-              dt.hour, dt.minute, dt.second,
-              dt.weekday(), 0, 0)
-        stamp = _time.mktime(tt)
-        tt = _time.localtime(stamp)
-        return tt.tm_isdst > 0
-
-local = LocalTimezone()
+import time as _time
+from datetime import tzinfo, timedelta
+
+ZERO = timedelta(0)
+HOUR = timedelta(hours=1)
+
+
+class UTC(tzinfo):
+    """UTC"""
+
+    def utcoffset(self, dt):
+        return ZERO
+
+    def tzname(self, dt):
+        return "UTC"
+
+    def dst(self, dt):
+        return ZERO
+
+utc = UTC()
+
+# A class building tzinfo objects for fixed-offset time zones.
+# Note that FixedOffset(0, "UTC") is a different way to build a
+# UTC tzinfo object.
+
+
+class FixedOffsetTimezone(tzinfo):
+    """Fixed offset in minutes east from UTC."""
+
+    def __init__(self, offset, name=None):
+        self.__offset = timedelta(minutes=offset)
+        self.__name = name
+
+    def utcoffset(self, dt):
+        return self.__offset
+
+    def tzname(self, dt):
+        return self.__name
+
+    def dst(self, dt):
+        return ZERO
+
+
+STDOFFSET = timedelta(seconds=-_time.timezone)
+if _time.daylight:
+    DSTOFFSET = timedelta(seconds=-_time.altzone)
+else:
+    DSTOFFSET = STDOFFSET
+
+DSTDIFF = DSTOFFSET - STDOFFSET
+
+
+class LocalTimezone(tzinfo):
+
+    def utcoffset(self, dt):
+        if self._isdst(dt):
+            return DSTOFFSET
+        else:
+            return STDOFFSET
+
+    def dst(self, dt):
+        if self._isdst(dt):
+            return DSTDIFF
+        else:
+            return ZERO
+
+    def tzname(self, dt):
+        return _time.tzname[self._isdst(dt)]
+
+    def _isdst(self, dt):
+        tt = (dt.year, dt.month, dt.day,
+              dt.hour, dt.minute, dt.second,
+              dt.weekday(), 0, 0)
+        stamp = _time.mktime(tt)
+        tt = _time.localtime(stamp)
+        return tt.tm_isdst > 0
+
+local = LocalTimezone()
```

### Comparing `python-tds-1.9.0/pytds/ntlm.py` & `python-tds-1.9.1/pytds/ntlm.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-# This library is free software: you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public
-# License as published by the Free Software Foundation, either
-# version 3 of the License, or (at your option) any later version.
-
-# This library is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public
-# License along with this library.  If not, see <http://www.gnu.org/licenses/> or <http://www.gnu.org/licenses/lgpl.txt>.
-
-import struct
-import base64
-import string
-import hashlib
-import hmac
-import random
-import re
-import binascii
-from socket import gethostname
-from six import print_, int2byte
-from . import pyDes
-
-NTLM_NegotiateUnicode                = 0x00000001
-NTLM_NegotiateOEM                    = 0x00000002
-NTLM_RequestTarget                   = 0x00000004
-NTLM_Unknown9                        = 0x00000008
-NTLM_NegotiateSign                   = 0x00000010
-NTLM_NegotiateSeal                   = 0x00000020
-NTLM_NegotiateDatagram               = 0x00000040
-NTLM_NegotiateLanManagerKey          = 0x00000080
-NTLM_Unknown8                        = 0x00000100
-NTLM_NegotiateNTLM                   = 0x00000200
-NTLM_NegotiateNTOnly                 = 0x00000400
-NTLM_Anonymous                       = 0x00000800
-NTLM_NegotiateOemDomainSupplied      = 0x00001000
-NTLM_NegotiateOemWorkstationSupplied = 0x00002000
-NTLM_Unknown6                        = 0x00004000
-NTLM_NegotiateAlwaysSign             = 0x00008000
-NTLM_TargetTypeDomain                = 0x00010000
-NTLM_TargetTypeServer                = 0x00020000
-NTLM_TargetTypeShare                 = 0x00040000
-NTLM_NegotiateExtendedSecurity       = 0x00080000
-NTLM_NegotiateIdentify               = 0x00100000
-NTLM_Unknown5                        = 0x00200000
-NTLM_RequestNonNTSessionKey          = 0x00400000
-NTLM_NegotiateTargetInfo             = 0x00800000
-NTLM_Unknown4                        = 0x01000000
-NTLM_NegotiateVersion                = 0x02000000
-NTLM_Unknown3                        = 0x04000000
-NTLM_Unknown2                        = 0x08000000
-NTLM_Unknown1                        = 0x10000000
-NTLM_Negotiate128                    = 0x20000000
-NTLM_NegotiateKeyExchange            = 0x40000000
-NTLM_Negotiate56                     = 0x80000000
-
-# we send these flags with our type 1 message
-NTLM_TYPE1_FLAGS = (NTLM_NegotiateUnicode |
-                    NTLM_NegotiateOEM |
-                    NTLM_RequestTarget |
-                    NTLM_NegotiateNTLM |
-                    NTLM_NegotiateOemDomainSupplied |
-                    NTLM_NegotiateOemWorkstationSupplied |
-                    NTLM_NegotiateAlwaysSign |
-                    NTLM_NegotiateExtendedSecurity |
-                    NTLM_NegotiateVersion |
-                    NTLM_Negotiate128 |
-                    NTLM_Negotiate56)
-NTLM_TYPE2_FLAGS = (NTLM_NegotiateUnicode |
-                    NTLM_RequestTarget |
-                    NTLM_NegotiateNTLM |
-                    NTLM_NegotiateAlwaysSign |
-                    NTLM_NegotiateExtendedSecurity |
-                    NTLM_NegotiateTargetInfo |
-                    NTLM_NegotiateVersion |
-                    NTLM_Negotiate128 |
-                    NTLM_Negotiate56)
-
-NTLM_MsvAvEOL             = 0  # Indicates that this is the last AV_PAIR in the list. AvLen MUST be 0. This type of information MUST be present in the AV pair list.
-NTLM_MsvAvNbComputerName  = 1  # The server's NetBIOS computer name. The name MUST be in Unicode, and is not null-terminated. This type of information MUST be present in the AV_pair list.
-NTLM_MsvAvNbDomainName    = 2  # The server's NetBIOS domain name. The name MUST be in Unicode, and is not null-terminated. This type of information MUST be present in the AV_pair list.
-NTLM_MsvAvDnsComputerName = 3  # The server's Active Directory DNS computer name. The name MUST be in Unicode, and is not null-terminated.
-NTLM_MsvAvDnsDomainName   = 4  # The server's Active Directory DNS domain name. The name MUST be in Unicode, and is not null-terminated.
-NTLM_MsvAvDnsTreeName     = 5  # The server's Active Directory (AD) DNS forest tree name. The name MUST be in Unicode, and is not null-terminated.
-NTLM_MsvAvFlags           = 6  # A field containing a 32-bit value indicating server or client configuration. 0x00000001: indicates to the client that the account authentication is constrained. 0x00000002: indicates that the client is providing message integrity in the MIC field (section 2.2.1.3) in the AUTHENTICATE_MESSAGE.
-NTLM_MsvAvTimestamp       = 7  # A FILETIME structure ([MS-DTYP] section 2.3.1) in little-endian byte order that contains the server local time.<12>
-NTLM_MsAvRestrictions     = 8  # A Restriction_Encoding structure (section 2.2.2.2). The Value field contains a structure representing the integrity level of the security principal, as well as a MachineID created at computer startup to identify the calling machine. <13>
-
-
-#
-# utility functions for Microsoft NTLM authentication
-#
-# References:
-# [MS-NLMP]: NT LAN Manager (NTLM) Authentication Protocol Specification
-# http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NLMP%5D.pdf
-#
-# [MS-NTHT]: NTLM Over HTTP Protocol Specification
-# http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NTHT%5D.pdf
-#
-# Cntlm Authentication Proxy
-# http://cntlm.awk.cz/
-#
-# NTLM Authorization Proxy Server
-# http://sourceforge.net/projects/ntlmaps/
-#
-# Optimized Attack for NTLM2 Session Response
-# http://www.blackhat.com/presentations/bh-asia-04/bh-jp-04-pdfs/bh-jp-04-seki.pdf
-#
-def dump_NegotiateFlags(NegotiateFlags):
-    if NegotiateFlags & NTLM_NegotiateUnicode:
-        print_("NTLM_NegotiateUnicode set")
-    if NegotiateFlags & NTLM_NegotiateOEM:
-        print_("NTLM_NegotiateOEM set")
-    if NegotiateFlags & NTLM_RequestTarget:
-        print_("NTLM_RequestTarget set")
-    if NegotiateFlags & NTLM_Unknown9:
-        print_("NTLM_Unknown9 set")
-    if NegotiateFlags & NTLM_NegotiateSign:
-        print_("NTLM_NegotiateSign set")
-    if NegotiateFlags & NTLM_NegotiateSeal:
-        print_("NTLM_NegotiateSeal set")
-    if NegotiateFlags & NTLM_NegotiateDatagram:
-        print_("NTLM_NegotiateDatagram set")
-    if NegotiateFlags & NTLM_NegotiateLanManagerKey:
-        print_("NTLM_NegotiateLanManagerKey set")
-    if NegotiateFlags & NTLM_Unknown8:
-        print_("NTLM_Unknown8 set")
-    if NegotiateFlags & NTLM_NegotiateNTLM:
-        print_("NTLM_NegotiateNTLM set")
-    if NegotiateFlags & NTLM_NegotiateNTOnly:
-        print_("NTLM_NegotiateNTOnly set")
-    if NegotiateFlags & NTLM_Anonymous:
-        print_("NTLM_Anonymous set")
-    if NegotiateFlags & NTLM_NegotiateOemDomainSupplied:
-        print_("NTLM_NegotiateOemDomainSupplied set")
-    if NegotiateFlags & NTLM_NegotiateOemWorkstationSupplied:
-        print_("NTLM_NegotiateOemWorkstationSupplied set")
-    if NegotiateFlags & NTLM_Unknown6:
-        print_("NTLM_Unknown6 set")
-    if NegotiateFlags & NTLM_NegotiateAlwaysSign:
-        print_("NTLM_NegotiateAlwaysSign set")
-    if NegotiateFlags & NTLM_TargetTypeDomain:
-        print_("NTLM_TargetTypeDomain set")
-    if NegotiateFlags & NTLM_TargetTypeServer:
-        print_("NTLM_TargetTypeServer set")
-    if NegotiateFlags & NTLM_TargetTypeShare:
-        print_("NTLM_TargetTypeShare set")
-    if NegotiateFlags & NTLM_NegotiateExtendedSecurity:
-        print_("NTLM_NegotiateExtendedSecurity set")
-    if NegotiateFlags & NTLM_NegotiateIdentify:
-        print_("NTLM_NegotiateIdentify set")
-    if NegotiateFlags & NTLM_Unknown5:
-        print_("NTLM_Unknown5 set")
-    if NegotiateFlags & NTLM_RequestNonNTSessionKey:
-        print_("NTLM_RequestNonNTSessionKey set")
-    if NegotiateFlags & NTLM_NegotiateTargetInfo:
-        print_("NTLM_NegotiateTargetInfo set")
-    if NegotiateFlags & NTLM_Unknown4:
-        print_("NTLM_Unknown4 set")
-    if NegotiateFlags & NTLM_NegotiateVersion:
-        print_("NTLM_NegotiateVersion set")
-    if NegotiateFlags & NTLM_Unknown3:
-        print_("NTLM_Unknown3 set")
-    if NegotiateFlags & NTLM_Unknown2:
-        print_("NTLM_Unknown2 set")
-    if NegotiateFlags & NTLM_Unknown1:
-        print_("NTLM_Unknown1 set")
-    if NegotiateFlags & NTLM_Negotiate128:
-        print_("NTLM_Negotiate128 set")
-    if NegotiateFlags & NTLM_NegotiateKeyExchange:
-        print_("NTLM_NegotiateKeyExchange set")
-    if NegotiateFlags & NTLM_Negotiate56:
-        print_("NTLM_Negotiate56 set")
-
-
-def create_NTLM_NEGOTIATE_MESSAGE_raw(workstation, domain, type1_flags=NTLM_TYPE1_FLAGS):
-    BODY_LENGTH = 40
-    Payload_start = BODY_LENGTH  # in bytes
-    protocol = b'NTLMSSP\0'    # name
-
-    type = struct.pack('<I', 1)  # type 1
-
-    flags = struct.pack('<I', type1_flags)
-    Workstation = workstation.upper().encode('ascii')
-    DomainName = domain.upper().encode('ascii')
-
-    WorkstationLen = struct.pack('<H', len(Workstation))
-    WorkstationMaxLen = struct.pack('<H', len(Workstation))
-    WorkstationBufferOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(Workstation)
-    DomainNameLen = struct.pack('<H', len(DomainName))
-    DomainNameMaxLen = struct.pack('<H', len(DomainName))
-    DomainNameBufferOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(DomainName)
-    ProductMajorVersion = struct.pack('<B', 5)
-    ProductMinorVersion = struct.pack('<B', 1)
-    ProductBuild = struct.pack('<H', 2600)
-    VersionReserved1 = struct.pack('<B', 0)
-    VersionReserved2 = struct.pack('<B', 0)
-    VersionReserved3 = struct.pack('<B', 0)
-    NTLMRevisionCurrent = struct.pack('<B', 15)
-
-    msg1 = protocol + type + flags + \
-        DomainNameLen + DomainNameMaxLen + DomainNameBufferOffset + \
-        WorkstationLen + WorkstationMaxLen + WorkstationBufferOffset + \
-        ProductMajorVersion + ProductMinorVersion + ProductBuild + \
-        VersionReserved1 + VersionReserved2 + VersionReserved3 + NTLMRevisionCurrent
-    assert BODY_LENGTH == len(msg1), "BODY_LENGTH: %d != msg1: %d" % (BODY_LENGTH, len(msg1))
-    msg1 += Workstation + DomainName
-    return msg1
-
-
-def create_NTLM_NEGOTIATE_MESSAGE(user, type1_flags=NTLM_TYPE1_FLAGS):
-    workstation = gethostname()
-    user_parts = user.split('\\', 1)
-    msg1 = create_NTLM_NEGOTIATE_MESSAGE_raw(workstation, user_parts[0], type1_flags)
-    msg1 = base64.encodestring(msg1)
-    msg1 = string.replace(msg1, '\n', '')
-    return msg1
-
-
-def parse_NTLM_CHALLENGE_MESSAGE_raw(msg2):
-    ""
-    Signature = msg2[0:8]
-    msg_type = struct.unpack("<I", msg2[8:12])[0]
-    assert(msg_type == 2)
-    TargetNameLen = struct.unpack("<H", msg2[12:14])[0]
-    TargetNameMaxLen = struct.unpack("<H", msg2[14:16])[0]
-    TargetNameOffset = struct.unpack("<I", msg2[16:20])[0]
-    TargetName = msg2[TargetNameOffset:TargetNameOffset + TargetNameMaxLen]
-    NegotiateFlags = struct.unpack("<I", msg2[20:24])[0]
-    ServerChallenge = msg2[24:32]
-    Reserved = msg2[32:40]
-    TargetInfoLen = struct.unpack("<H", msg2[40:42])[0]
-    TargetInfoMaxLen = struct.unpack("<H", msg2[42:44])[0]
-    TargetInfoOffset = struct.unpack("<I", msg2[44:48])[0]
-    TargetInfo = msg2[TargetInfoOffset:TargetInfoOffset + TargetInfoLen]
-    i = 0
-    TimeStamp = '\0' * 8
-    while(i < TargetInfoLen):
-        AvId = struct.unpack("<H", TargetInfo[i:i + 2])[0]
-        AvLen = struct.unpack("<H", TargetInfo[i + 2:i + 4])[0]
-        AvValue = TargetInfo[i + 4:i + 4 + AvLen]
-        i = i + 4 + AvLen
-        if AvId == NTLM_MsvAvTimestamp:
-            TimeStamp = AvValue
-        #~ print AvId, AvValue.decode('utf-16')
-    return (ServerChallenge, NegotiateFlags)
-
-
-def parse_NTLM_CHALLENGE_MESSAGE(msg2):
-    return parse_NTLM_CHALLENGE_MESSAGE(base64.decodestring(msg2))
-
-
-def create_NTLM_AUTHENTICATE_MESSAGE_raw(nonce, user, domain, password, NegotiateFlags):
-    ""
-    is_unicode = NegotiateFlags & NTLM_NegotiateUnicode
-    is_NegotiateExtendedSecurity = NegotiateFlags & NTLM_NegotiateExtendedSecurity
-
-    flags = struct.pack('<I', NTLM_TYPE2_FLAGS)
-
-    BODY_LENGTH = 72
-    Payload_start = BODY_LENGTH  # in bytes
-
-    Workstation = gethostname().upper()
-    DomainName = domain.upper()
-    UserName = user
-    EncryptedRandomSessionKey = ""
-    if is_unicode:
-        Workstation = Workstation.encode('utf-16-le')
-        DomainName = DomainName.encode('utf-16-le')
-        UserName = UserName.encode('utf-16-le')
-        EncryptedRandomSessionKey = EncryptedRandomSessionKey.encode('utf-16-le')
-    LmChallengeResponse = calc_resp(create_LM_hashed_password_v1(password), nonce)
-    NtChallengeResponse = calc_resp(create_NT_hashed_password_v1(password), nonce)
-
-    if is_NegotiateExtendedSecurity:
-        pwhash = create_NT_hashed_password_v1(password, UserName, DomainName)
-        ClientChallenge = b""
-        for i in range(8):
-            ClientChallenge += int2byte(random.getrandbits(8))
-        (NtChallengeResponse, LmChallengeResponse) = ntlm2sr_calc_resp(pwhash, nonce, ClientChallenge)
-    Signature = b'NTLMSSP\0'
-    MessageType = struct.pack('<I', 3)   # type 3
-
-    DomainNameLen = struct.pack('<H', len(DomainName))
-    DomainNameMaxLen = struct.pack('<H', len(DomainName))
-    DomainNameOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(DomainName)
-
-    UserNameLen = struct.pack('<H', len(UserName))
-    UserNameMaxLen = struct.pack('<H', len(UserName))
-    UserNameOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(UserName)
-
-    WorkstationLen = struct.pack('<H', len(Workstation))
-    WorkstationMaxLen = struct.pack('<H', len(Workstation))
-    WorkstationOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(Workstation)
-
-    LmChallengeResponseLen = struct.pack('<H', len(LmChallengeResponse))
-    LmChallengeResponseMaxLen = struct.pack('<H', len(LmChallengeResponse))
-    LmChallengeResponseOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(LmChallengeResponse)
-
-    NtChallengeResponseLen = struct.pack('<H', len(NtChallengeResponse))
-    NtChallengeResponseMaxLen = struct.pack('<H', len(NtChallengeResponse))
-    NtChallengeResponseOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(NtChallengeResponse)
-
-    EncryptedRandomSessionKeyLen = struct.pack('<H', len(EncryptedRandomSessionKey))
-    EncryptedRandomSessionKeyMaxLen = struct.pack('<H', len(EncryptedRandomSessionKey))
-    EncryptedRandomSessionKeyOffset = struct.pack('<I', Payload_start)
-    Payload_start += len(EncryptedRandomSessionKey)
-    NegotiateFlags = flags
-
-    ProductMajorVersion = struct.pack('<B', 5)
-    ProductMinorVersion = struct.pack('<B', 1)
-    ProductBuild = struct.pack('<H', 2600)
-    VersionReserved1 = struct.pack('<B', 0)
-    VersionReserved2 = struct.pack('<B', 0)
-    VersionReserved3 = struct.pack('<B', 0)
-    NTLMRevisionCurrent = struct.pack('<B', 15)
-
-    MIC = struct.pack('<IIII', 0, 0, 0, 0)
-    msg3 = Signature + MessageType + \
-        LmChallengeResponseLen + LmChallengeResponseMaxLen + LmChallengeResponseOffset + \
-        NtChallengeResponseLen + NtChallengeResponseMaxLen + NtChallengeResponseOffset + \
-        DomainNameLen + DomainNameMaxLen + DomainNameOffset + \
-        UserNameLen + UserNameMaxLen + UserNameOffset + \
-        WorkstationLen + WorkstationMaxLen + WorkstationOffset + \
-        EncryptedRandomSessionKeyLen + EncryptedRandomSessionKeyMaxLen + EncryptedRandomSessionKeyOffset + \
-        NegotiateFlags + \
-        ProductMajorVersion + ProductMinorVersion + ProductBuild + \
-        VersionReserved1 + VersionReserved2 + VersionReserved3 + NTLMRevisionCurrent
-    assert BODY_LENGTH == len(msg3), "BODY_LENGTH: %d != msg3: %d" % (BODY_LENGTH, len(msg3))
-    Payload = DomainName + UserName + Workstation + LmChallengeResponse + NtChallengeResponse + EncryptedRandomSessionKey
-    msg3 += Payload
-    return msg3
-
-
-def create_NTLM_AUTHENTICATE_MESSAGE(nonce, user, domain, password, NegotiateFlags):
-    msg3 = create_NTLM_AUTHENTICATE_MESSAGE(nonce, user, domain, password, NegotiateFlags)
-    msg3 = base64.encodestring(msg3)
-    msg3 = string.replace(msg3, '\n', '')
-    return msg3
-
-
-def calc_resp(password_hash, server_challenge):
-    """calc_resp generates the LM response given a 16-byte password hash and the
-        challenge from the Type-2 message.
-        @param password_hash
-            16-byte password hash
-        @param server_challenge
-            8-byte challenge from Type-2 message
-        returns
-            24-byte buffer to contain the LM response upon return
-    """
-    # padding with zeros to make the hash 21 bytes long
-    password_hash = password_hash + b'\0' * (21 - len(password_hash))
-    res = b''
-    dobj = pyDes.des(key56_to_key64(password_hash[0:7]))
-    res = res + dobj.encrypt(server_challenge[0:8])
-
-    dobj = pyDes.des(key56_to_key64(password_hash[7:14]))
-    res = res + dobj.encrypt(server_challenge[0:8])
-
-    dobj = pyDes.des(key56_to_key64(password_hash[14:21]))
-    res = res + dobj.encrypt(server_challenge[0:8])
-    return res
-
-
-def ComputeResponse(ResponseKeyNT, ResponseKeyLM, ServerChallenge, ServerName, ClientChallenge=b'\xaa' * 8, Time=b'\0' * 8):
-    LmChallengeResponse = hmac.new(ResponseKeyLM, ServerChallenge + ClientChallenge).digest() + ClientChallenge
-
-    Responserversion = b'\x01'
-    HiResponserversion = b'\x01'
-    temp = Responserversion + HiResponserversion + b'\0' * 6 + Time + ClientChallenge + b'\0' * 4 + ServerChallenge + b'\0' * 4
-    NTProofStr = hmac.new(ResponseKeyNT, ServerChallenge + temp).digest()
-    NtChallengeResponse = NTProofStr + temp
-
-    SessionBaseKey = hmac.new(ResponseKeyNT, NTProofStr).digest()
-    return (NtChallengeResponse, LmChallengeResponse)
-
-
-def ntlm2sr_calc_resp(ResponseKeyNT, ServerChallenge, ClientChallenge=b'\xaa' * 8):
-    LmChallengeResponse = ClientChallenge + b'\0' * 16
-    sess = hashlib.md5(ServerChallenge + ClientChallenge).digest()
-    NtChallengeResponse = calc_resp(ResponseKeyNT, sess[0:8])
-    return (NtChallengeResponse, LmChallengeResponse)
-
-
-def create_LM_hashed_password_v1(passwd):
-    "setup LanManager password"
-    "create LanManager hashed password"
-    # if the passwd provided is already a hash, we just return the first half
-    if re.match(r'^[\w]{32}:[\w]{32}$', passwd):
-        return binascii.unhexlify(passwd.split(':')[0])
-
-    # fix the password length to 14 bytes
-    passwd = passwd.upper().encode('ascii')
-    lm_pw = passwd + b'\0' * (14 - len(passwd))
-    lm_pw = lm_pw[0:14]
-
-    # do hash
-    magic_str = b"KGS!@#$%"  # page 57 in [MS-NLMP]
-
-    res = b''
-    dobj = pyDes.des(key56_to_key64(lm_pw[0:7]))
-    res = res + dobj.encrypt(magic_str)
-
-    dobj = pyDes.des(key56_to_key64(lm_pw[7:14]))
-    res = res + dobj.encrypt(magic_str)
-
-    return res
-
-
-def create_NT_hashed_password_v1(passwd, user=None, domain=None):
-    "create NT hashed password"
-    # if the passwd provided is already a hash, we just return the second half
-    if re.match(r'^[\w]{32}:[\w]{32}$', passwd):
-        return binascii.unhexlify(passwd.split(':')[1])
-
-    digest = hashlib.new('md4', passwd.encode('utf-16le')).digest()
-    return digest
-
-
-def create_NT_hashed_password_v2(passwd, user, domain):
-    "create NT hashed password"
-    digest = create_NT_hashed_password_v1(passwd)
-
-    return hmac.new(digest, (user.upper() + domain).encode('utf-16le')).digest()
-    return digest
-
-
-def create_sessionbasekey(password):
-    return hashlib.new('md4', create_NT_hashed_password_v1(password)).digest()
-
-
-def key56_to_key64(key_56):
-    ""
-    assert len(key_56) == 7
-    key = bytearray(8)
-    key_56 = bytearray(key_56)
-
-    key[0] = key_56[0]
-    key[1] = ((key_56[0] << 7) & 0xFF) | (key_56[1] >> 1)
-    key[2] = ((key_56[1] << 6) & 0xFF) | (key_56[2] >> 2)
-    key[3] = ((key_56[2] << 5) & 0xFF) | (key_56[3] >> 3)
-    key[4] = ((key_56[3] << 4) & 0xFF) | (key_56[4] >> 4)
-    key[5] = ((key_56[4] << 3) & 0xFF) | (key_56[5] >> 5)
-    key[6] = ((key_56[5] << 2) & 0xFF) | (key_56[6] >> 6)
-    key[7] = (key_56[6] << 1) & 0xFF
-
-    #key = set_key_odd_parity(key)
-
-    return bytes(key)
-
-
-#def set_key_odd_parity(key):
-#    ""
-#    for i in range(len(key)):
-#        for k in range(7):
-#            bit = 0
-#            t = key[i] >> k
-#            bit = (t ^ bit) & 0x1
-#        key[i] = (key[i] & 0xFE) | bit
-#
-#    return key
+# This library is free software: you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation, either
+# version 3 of the License, or (at your option) any later version.
+
+# This library is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public
+# License along with this library.  If not, see <http://www.gnu.org/licenses/> or <http://www.gnu.org/licenses/lgpl.txt>.
+
+import struct
+import base64
+import string
+import hashlib
+import hmac
+import random
+import re
+import binascii
+from socket import gethostname
+from six import print_, int2byte
+from . import pyDes
+
+NTLM_NegotiateUnicode                = 0x00000001
+NTLM_NegotiateOEM                    = 0x00000002
+NTLM_RequestTarget                   = 0x00000004
+NTLM_Unknown9                        = 0x00000008
+NTLM_NegotiateSign                   = 0x00000010
+NTLM_NegotiateSeal                   = 0x00000020
+NTLM_NegotiateDatagram               = 0x00000040
+NTLM_NegotiateLanManagerKey          = 0x00000080
+NTLM_Unknown8                        = 0x00000100
+NTLM_NegotiateNTLM                   = 0x00000200
+NTLM_NegotiateNTOnly                 = 0x00000400
+NTLM_Anonymous                       = 0x00000800
+NTLM_NegotiateOemDomainSupplied      = 0x00001000
+NTLM_NegotiateOemWorkstationSupplied = 0x00002000
+NTLM_Unknown6                        = 0x00004000
+NTLM_NegotiateAlwaysSign             = 0x00008000
+NTLM_TargetTypeDomain                = 0x00010000
+NTLM_TargetTypeServer                = 0x00020000
+NTLM_TargetTypeShare                 = 0x00040000
+NTLM_NegotiateExtendedSecurity       = 0x00080000
+NTLM_NegotiateIdentify               = 0x00100000
+NTLM_Unknown5                        = 0x00200000
+NTLM_RequestNonNTSessionKey          = 0x00400000
+NTLM_NegotiateTargetInfo             = 0x00800000
+NTLM_Unknown4                        = 0x01000000
+NTLM_NegotiateVersion                = 0x02000000
+NTLM_Unknown3                        = 0x04000000
+NTLM_Unknown2                        = 0x08000000
+NTLM_Unknown1                        = 0x10000000
+NTLM_Negotiate128                    = 0x20000000
+NTLM_NegotiateKeyExchange            = 0x40000000
+NTLM_Negotiate56                     = 0x80000000
+
+# we send these flags with our type 1 message
+NTLM_TYPE1_FLAGS = (NTLM_NegotiateUnicode |
+                    NTLM_NegotiateOEM |
+                    NTLM_RequestTarget |
+                    NTLM_NegotiateNTLM |
+                    NTLM_NegotiateOemDomainSupplied |
+                    NTLM_NegotiateOemWorkstationSupplied |
+                    NTLM_NegotiateAlwaysSign |
+                    NTLM_NegotiateExtendedSecurity |
+                    NTLM_NegotiateVersion |
+                    NTLM_Negotiate128 |
+                    NTLM_Negotiate56)
+NTLM_TYPE2_FLAGS = (NTLM_NegotiateUnicode |
+                    NTLM_RequestTarget |
+                    NTLM_NegotiateNTLM |
+                    NTLM_NegotiateAlwaysSign |
+                    NTLM_NegotiateExtendedSecurity |
+                    NTLM_NegotiateTargetInfo |
+                    NTLM_NegotiateVersion |
+                    NTLM_Negotiate128 |
+                    NTLM_Negotiate56)
+
+NTLM_MsvAvEOL             = 0  # Indicates that this is the last AV_PAIR in the list. AvLen MUST be 0. This type of information MUST be present in the AV pair list.
+NTLM_MsvAvNbComputerName  = 1  # The server's NetBIOS computer name. The name MUST be in Unicode, and is not null-terminated. This type of information MUST be present in the AV_pair list.
+NTLM_MsvAvNbDomainName    = 2  # The server's NetBIOS domain name. The name MUST be in Unicode, and is not null-terminated. This type of information MUST be present in the AV_pair list.
+NTLM_MsvAvDnsComputerName = 3  # The server's Active Directory DNS computer name. The name MUST be in Unicode, and is not null-terminated.
+NTLM_MsvAvDnsDomainName   = 4  # The server's Active Directory DNS domain name. The name MUST be in Unicode, and is not null-terminated.
+NTLM_MsvAvDnsTreeName     = 5  # The server's Active Directory (AD) DNS forest tree name. The name MUST be in Unicode, and is not null-terminated.
+NTLM_MsvAvFlags           = 6  # A field containing a 32-bit value indicating server or client configuration. 0x00000001: indicates to the client that the account authentication is constrained. 0x00000002: indicates that the client is providing message integrity in the MIC field (section 2.2.1.3) in the AUTHENTICATE_MESSAGE.
+NTLM_MsvAvTimestamp       = 7  # A FILETIME structure ([MS-DTYP] section 2.3.1) in little-endian byte order that contains the server local time.<12>
+NTLM_MsAvRestrictions     = 8  # A Restriction_Encoding structure (section 2.2.2.2). The Value field contains a structure representing the integrity level of the security principal, as well as a MachineID created at computer startup to identify the calling machine. <13>
+
+
+#
+# utility functions for Microsoft NTLM authentication
+#
+# References:
+# [MS-NLMP]: NT LAN Manager (NTLM) Authentication Protocol Specification
+# http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NLMP%5D.pdf
+#
+# [MS-NTHT]: NTLM Over HTTP Protocol Specification
+# http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NTHT%5D.pdf
+#
+# Cntlm Authentication Proxy
+# http://cntlm.awk.cz/
+#
+# NTLM Authorization Proxy Server
+# http://sourceforge.net/projects/ntlmaps/
+#
+# Optimized Attack for NTLM2 Session Response
+# http://www.blackhat.com/presentations/bh-asia-04/bh-jp-04-pdfs/bh-jp-04-seki.pdf
+#
+def dump_NegotiateFlags(NegotiateFlags):
+    if NegotiateFlags & NTLM_NegotiateUnicode:
+        print_("NTLM_NegotiateUnicode set")
+    if NegotiateFlags & NTLM_NegotiateOEM:
+        print_("NTLM_NegotiateOEM set")
+    if NegotiateFlags & NTLM_RequestTarget:
+        print_("NTLM_RequestTarget set")
+    if NegotiateFlags & NTLM_Unknown9:
+        print_("NTLM_Unknown9 set")
+    if NegotiateFlags & NTLM_NegotiateSign:
+        print_("NTLM_NegotiateSign set")
+    if NegotiateFlags & NTLM_NegotiateSeal:
+        print_("NTLM_NegotiateSeal set")
+    if NegotiateFlags & NTLM_NegotiateDatagram:
+        print_("NTLM_NegotiateDatagram set")
+    if NegotiateFlags & NTLM_NegotiateLanManagerKey:
+        print_("NTLM_NegotiateLanManagerKey set")
+    if NegotiateFlags & NTLM_Unknown8:
+        print_("NTLM_Unknown8 set")
+    if NegotiateFlags & NTLM_NegotiateNTLM:
+        print_("NTLM_NegotiateNTLM set")
+    if NegotiateFlags & NTLM_NegotiateNTOnly:
+        print_("NTLM_NegotiateNTOnly set")
+    if NegotiateFlags & NTLM_Anonymous:
+        print_("NTLM_Anonymous set")
+    if NegotiateFlags & NTLM_NegotiateOemDomainSupplied:
+        print_("NTLM_NegotiateOemDomainSupplied set")
+    if NegotiateFlags & NTLM_NegotiateOemWorkstationSupplied:
+        print_("NTLM_NegotiateOemWorkstationSupplied set")
+    if NegotiateFlags & NTLM_Unknown6:
+        print_("NTLM_Unknown6 set")
+    if NegotiateFlags & NTLM_NegotiateAlwaysSign:
+        print_("NTLM_NegotiateAlwaysSign set")
+    if NegotiateFlags & NTLM_TargetTypeDomain:
+        print_("NTLM_TargetTypeDomain set")
+    if NegotiateFlags & NTLM_TargetTypeServer:
+        print_("NTLM_TargetTypeServer set")
+    if NegotiateFlags & NTLM_TargetTypeShare:
+        print_("NTLM_TargetTypeShare set")
+    if NegotiateFlags & NTLM_NegotiateExtendedSecurity:
+        print_("NTLM_NegotiateExtendedSecurity set")
+    if NegotiateFlags & NTLM_NegotiateIdentify:
+        print_("NTLM_NegotiateIdentify set")
+    if NegotiateFlags & NTLM_Unknown5:
+        print_("NTLM_Unknown5 set")
+    if NegotiateFlags & NTLM_RequestNonNTSessionKey:
+        print_("NTLM_RequestNonNTSessionKey set")
+    if NegotiateFlags & NTLM_NegotiateTargetInfo:
+        print_("NTLM_NegotiateTargetInfo set")
+    if NegotiateFlags & NTLM_Unknown4:
+        print_("NTLM_Unknown4 set")
+    if NegotiateFlags & NTLM_NegotiateVersion:
+        print_("NTLM_NegotiateVersion set")
+    if NegotiateFlags & NTLM_Unknown3:
+        print_("NTLM_Unknown3 set")
+    if NegotiateFlags & NTLM_Unknown2:
+        print_("NTLM_Unknown2 set")
+    if NegotiateFlags & NTLM_Unknown1:
+        print_("NTLM_Unknown1 set")
+    if NegotiateFlags & NTLM_Negotiate128:
+        print_("NTLM_Negotiate128 set")
+    if NegotiateFlags & NTLM_NegotiateKeyExchange:
+        print_("NTLM_NegotiateKeyExchange set")
+    if NegotiateFlags & NTLM_Negotiate56:
+        print_("NTLM_Negotiate56 set")
+
+
+def create_NTLM_NEGOTIATE_MESSAGE_raw(workstation, domain, type1_flags=NTLM_TYPE1_FLAGS):
+    BODY_LENGTH = 40
+    Payload_start = BODY_LENGTH  # in bytes
+    protocol = b'NTLMSSP\0'    # name
+
+    type = struct.pack('<I', 1)  # type 1
+
+    flags = struct.pack('<I', type1_flags)
+    Workstation = workstation.upper().encode('ascii')
+    DomainName = domain.upper().encode('ascii')
+
+    WorkstationLen = struct.pack('<H', len(Workstation))
+    WorkstationMaxLen = struct.pack('<H', len(Workstation))
+    WorkstationBufferOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(Workstation)
+    DomainNameLen = struct.pack('<H', len(DomainName))
+    DomainNameMaxLen = struct.pack('<H', len(DomainName))
+    DomainNameBufferOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(DomainName)
+    ProductMajorVersion = struct.pack('<B', 5)
+    ProductMinorVersion = struct.pack('<B', 1)
+    ProductBuild = struct.pack('<H', 2600)
+    VersionReserved1 = struct.pack('<B', 0)
+    VersionReserved2 = struct.pack('<B', 0)
+    VersionReserved3 = struct.pack('<B', 0)
+    NTLMRevisionCurrent = struct.pack('<B', 15)
+
+    msg1 = protocol + type + flags + \
+        DomainNameLen + DomainNameMaxLen + DomainNameBufferOffset + \
+        WorkstationLen + WorkstationMaxLen + WorkstationBufferOffset + \
+        ProductMajorVersion + ProductMinorVersion + ProductBuild + \
+        VersionReserved1 + VersionReserved2 + VersionReserved3 + NTLMRevisionCurrent
+    assert BODY_LENGTH == len(msg1), "BODY_LENGTH: %d != msg1: %d" % (BODY_LENGTH, len(msg1))
+    msg1 += Workstation + DomainName
+    return msg1
+
+
+def create_NTLM_NEGOTIATE_MESSAGE(user, type1_flags=NTLM_TYPE1_FLAGS):
+    workstation = gethostname()
+    user_parts = user.split('\\', 1)
+    msg1 = create_NTLM_NEGOTIATE_MESSAGE_raw(workstation, user_parts[0], type1_flags)
+    msg1 = base64.encodestring(msg1)
+    msg1 = string.replace(msg1, '\n', '')
+    return msg1
+
+
+def parse_NTLM_CHALLENGE_MESSAGE_raw(msg2):
+    ""
+    Signature = msg2[0:8]
+    msg_type = struct.unpack("<I", msg2[8:12])[0]
+    assert(msg_type == 2)
+    TargetNameLen = struct.unpack("<H", msg2[12:14])[0]
+    TargetNameMaxLen = struct.unpack("<H", msg2[14:16])[0]
+    TargetNameOffset = struct.unpack("<I", msg2[16:20])[0]
+    TargetName = msg2[TargetNameOffset:TargetNameOffset + TargetNameMaxLen]
+    NegotiateFlags = struct.unpack("<I", msg2[20:24])[0]
+    ServerChallenge = msg2[24:32]
+    Reserved = msg2[32:40]
+    TargetInfoLen = struct.unpack("<H", msg2[40:42])[0]
+    TargetInfoMaxLen = struct.unpack("<H", msg2[42:44])[0]
+    TargetInfoOffset = struct.unpack("<I", msg2[44:48])[0]
+    TargetInfo = msg2[TargetInfoOffset:TargetInfoOffset + TargetInfoLen]
+    i = 0
+    TimeStamp = '\0' * 8
+    while(i < TargetInfoLen):
+        AvId = struct.unpack("<H", TargetInfo[i:i + 2])[0]
+        AvLen = struct.unpack("<H", TargetInfo[i + 2:i + 4])[0]
+        AvValue = TargetInfo[i + 4:i + 4 + AvLen]
+        i = i + 4 + AvLen
+        if AvId == NTLM_MsvAvTimestamp:
+            TimeStamp = AvValue
+        #~ print AvId, AvValue.decode('utf-16')
+    return (ServerChallenge, NegotiateFlags)
+
+
+def parse_NTLM_CHALLENGE_MESSAGE(msg2):
+    return parse_NTLM_CHALLENGE_MESSAGE(base64.decodestring(msg2))
+
+
+def create_NTLM_AUTHENTICATE_MESSAGE_raw(nonce, user, domain, password, NegotiateFlags):
+    ""
+    is_unicode = NegotiateFlags & NTLM_NegotiateUnicode
+    is_NegotiateExtendedSecurity = NegotiateFlags & NTLM_NegotiateExtendedSecurity
+
+    flags = struct.pack('<I', NTLM_TYPE2_FLAGS)
+
+    BODY_LENGTH = 72
+    Payload_start = BODY_LENGTH  # in bytes
+
+    Workstation = gethostname().upper()
+    DomainName = domain.upper()
+    UserName = user
+    EncryptedRandomSessionKey = ""
+    if is_unicode:
+        Workstation = Workstation.encode('utf-16-le')
+        DomainName = DomainName.encode('utf-16-le')
+        UserName = UserName.encode('utf-16-le')
+        EncryptedRandomSessionKey = EncryptedRandomSessionKey.encode('utf-16-le')
+    LmChallengeResponse = calc_resp(create_LM_hashed_password_v1(password), nonce)
+    NtChallengeResponse = calc_resp(create_NT_hashed_password_v1(password), nonce)
+
+    if is_NegotiateExtendedSecurity:
+        pwhash = create_NT_hashed_password_v1(password, UserName, DomainName)
+        ClientChallenge = b""
+        for i in range(8):
+            ClientChallenge += int2byte(random.getrandbits(8))
+        (NtChallengeResponse, LmChallengeResponse) = ntlm2sr_calc_resp(pwhash, nonce, ClientChallenge)
+    Signature = b'NTLMSSP\0'
+    MessageType = struct.pack('<I', 3)   # type 3
+
+    DomainNameLen = struct.pack('<H', len(DomainName))
+    DomainNameMaxLen = struct.pack('<H', len(DomainName))
+    DomainNameOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(DomainName)
+
+    UserNameLen = struct.pack('<H', len(UserName))
+    UserNameMaxLen = struct.pack('<H', len(UserName))
+    UserNameOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(UserName)
+
+    WorkstationLen = struct.pack('<H', len(Workstation))
+    WorkstationMaxLen = struct.pack('<H', len(Workstation))
+    WorkstationOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(Workstation)
+
+    LmChallengeResponseLen = struct.pack('<H', len(LmChallengeResponse))
+    LmChallengeResponseMaxLen = struct.pack('<H', len(LmChallengeResponse))
+    LmChallengeResponseOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(LmChallengeResponse)
+
+    NtChallengeResponseLen = struct.pack('<H', len(NtChallengeResponse))
+    NtChallengeResponseMaxLen = struct.pack('<H', len(NtChallengeResponse))
+    NtChallengeResponseOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(NtChallengeResponse)
+
+    EncryptedRandomSessionKeyLen = struct.pack('<H', len(EncryptedRandomSessionKey))
+    EncryptedRandomSessionKeyMaxLen = struct.pack('<H', len(EncryptedRandomSessionKey))
+    EncryptedRandomSessionKeyOffset = struct.pack('<I', Payload_start)
+    Payload_start += len(EncryptedRandomSessionKey)
+    NegotiateFlags = flags
+
+    ProductMajorVersion = struct.pack('<B', 5)
+    ProductMinorVersion = struct.pack('<B', 1)
+    ProductBuild = struct.pack('<H', 2600)
+    VersionReserved1 = struct.pack('<B', 0)
+    VersionReserved2 = struct.pack('<B', 0)
+    VersionReserved3 = struct.pack('<B', 0)
+    NTLMRevisionCurrent = struct.pack('<B', 15)
+
+    MIC = struct.pack('<IIII', 0, 0, 0, 0)
+    msg3 = Signature + MessageType + \
+        LmChallengeResponseLen + LmChallengeResponseMaxLen + LmChallengeResponseOffset + \
+        NtChallengeResponseLen + NtChallengeResponseMaxLen + NtChallengeResponseOffset + \
+        DomainNameLen + DomainNameMaxLen + DomainNameOffset + \
+        UserNameLen + UserNameMaxLen + UserNameOffset + \
+        WorkstationLen + WorkstationMaxLen + WorkstationOffset + \
+        EncryptedRandomSessionKeyLen + EncryptedRandomSessionKeyMaxLen + EncryptedRandomSessionKeyOffset + \
+        NegotiateFlags + \
+        ProductMajorVersion + ProductMinorVersion + ProductBuild + \
+        VersionReserved1 + VersionReserved2 + VersionReserved3 + NTLMRevisionCurrent
+    assert BODY_LENGTH == len(msg3), "BODY_LENGTH: %d != msg3: %d" % (BODY_LENGTH, len(msg3))
+    Payload = DomainName + UserName + Workstation + LmChallengeResponse + NtChallengeResponse + EncryptedRandomSessionKey
+    msg3 += Payload
+    return msg3
+
+
+def create_NTLM_AUTHENTICATE_MESSAGE(nonce, user, domain, password, NegotiateFlags):
+    msg3 = create_NTLM_AUTHENTICATE_MESSAGE(nonce, user, domain, password, NegotiateFlags)
+    msg3 = base64.encodestring(msg3)
+    msg3 = string.replace(msg3, '\n', '')
+    return msg3
+
+
+def calc_resp(password_hash, server_challenge):
+    """calc_resp generates the LM response given a 16-byte password hash and the
+        challenge from the Type-2 message.
+        @param password_hash
+            16-byte password hash
+        @param server_challenge
+            8-byte challenge from Type-2 message
+        returns
+            24-byte buffer to contain the LM response upon return
+    """
+    # padding with zeros to make the hash 21 bytes long
+    password_hash = password_hash + b'\0' * (21 - len(password_hash))
+    res = b''
+    dobj = pyDes.des(key56_to_key64(password_hash[0:7]))
+    res = res + dobj.encrypt(server_challenge[0:8])
+
+    dobj = pyDes.des(key56_to_key64(password_hash[7:14]))
+    res = res + dobj.encrypt(server_challenge[0:8])
+
+    dobj = pyDes.des(key56_to_key64(password_hash[14:21]))
+    res = res + dobj.encrypt(server_challenge[0:8])
+    return res
+
+
+def ComputeResponse(ResponseKeyNT, ResponseKeyLM, ServerChallenge, ServerName, ClientChallenge=b'\xaa' * 8, Time=b'\0' * 8):
+    LmChallengeResponse = hmac.new(ResponseKeyLM, ServerChallenge + ClientChallenge).digest() + ClientChallenge
+
+    Responserversion = b'\x01'
+    HiResponserversion = b'\x01'
+    temp = Responserversion + HiResponserversion + b'\0' * 6 + Time + ClientChallenge + b'\0' * 4 + ServerChallenge + b'\0' * 4
+    NTProofStr = hmac.new(ResponseKeyNT, ServerChallenge + temp).digest()
+    NtChallengeResponse = NTProofStr + temp
+
+    SessionBaseKey = hmac.new(ResponseKeyNT, NTProofStr).digest()
+    return (NtChallengeResponse, LmChallengeResponse)
+
+
+def ntlm2sr_calc_resp(ResponseKeyNT, ServerChallenge, ClientChallenge=b'\xaa' * 8):
+    LmChallengeResponse = ClientChallenge + b'\0' * 16
+    sess = hashlib.md5(ServerChallenge + ClientChallenge).digest()
+    NtChallengeResponse = calc_resp(ResponseKeyNT, sess[0:8])
+    return (NtChallengeResponse, LmChallengeResponse)
+
+
+def create_LM_hashed_password_v1(passwd):
+    "setup LanManager password"
+    "create LanManager hashed password"
+    # if the passwd provided is already a hash, we just return the first half
+    if re.match(r'^[\w]{32}:[\w]{32}$', passwd):
+        return binascii.unhexlify(passwd.split(':')[0])
+
+    # fix the password length to 14 bytes
+    passwd = passwd.upper().encode('ascii')
+    lm_pw = passwd + b'\0' * (14 - len(passwd))
+    lm_pw = lm_pw[0:14]
+
+    # do hash
+    magic_str = b"KGS!@#$%"  # page 57 in [MS-NLMP]
+
+    res = b''
+    dobj = pyDes.des(key56_to_key64(lm_pw[0:7]))
+    res = res + dobj.encrypt(magic_str)
+
+    dobj = pyDes.des(key56_to_key64(lm_pw[7:14]))
+    res = res + dobj.encrypt(magic_str)
+
+    return res
+
+
+def create_NT_hashed_password_v1(passwd, user=None, domain=None):
+    "create NT hashed password"
+    # if the passwd provided is already a hash, we just return the second half
+    if re.match(r'^[\w]{32}:[\w]{32}$', passwd):
+        return binascii.unhexlify(passwd.split(':')[1])
+
+    digest = hashlib.new('md4', passwd.encode('utf-16le')).digest()
+    return digest
+
+
+def create_NT_hashed_password_v2(passwd, user, domain):
+    "create NT hashed password"
+    digest = create_NT_hashed_password_v1(passwd)
+
+    return hmac.new(digest, (user.upper() + domain).encode('utf-16le')).digest()
+    return digest
+
+
+def create_sessionbasekey(password):
+    return hashlib.new('md4', create_NT_hashed_password_v1(password)).digest()
+
+
+def key56_to_key64(key_56):
+    ""
+    assert len(key_56) == 7
+    key = bytearray(8)
+    key_56 = bytearray(key_56)
+
+    key[0] = key_56[0]
+    key[1] = ((key_56[0] << 7) & 0xFF) | (key_56[1] >> 1)
+    key[2] = ((key_56[1] << 6) & 0xFF) | (key_56[2] >> 2)
+    key[3] = ((key_56[2] << 5) & 0xFF) | (key_56[3] >> 3)
+    key[4] = ((key_56[3] << 4) & 0xFF) | (key_56[4] >> 4)
+    key[5] = ((key_56[4] << 3) & 0xFF) | (key_56[5] >> 5)
+    key[6] = ((key_56[5] << 2) & 0xFF) | (key_56[6] >> 6)
+    key[7] = (key_56[6] << 1) & 0xFF
+
+    #key = set_key_odd_parity(key)
+
+    return bytes(key)
+
+
+#def set_key_odd_parity(key):
+#    ""
+#    for i in range(len(key)):
+#        for k in range(7):
+#            bit = 0
+#            t = key[i] >> k
+#            bit = (t ^ bit) & 0x1
+#        key[i] = (key[i] & 0xFE) | bit
+#
+#    return key
```

### Comparing `python-tds-1.9.0/pytds/tds.py` & `python-tds-1.9.1/pytds/tds.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,1840 +1,1840 @@
-import codecs
-import contextlib
-import logging
-import datetime
-import six
-import socket
-import struct
-
-from .collate import ucs2_codec, Collation, lcid2charset, raw_collation
-from . import tds_base
-from . import tds_types
-from . import tls
-from .tds_base import readall, readall_fast, skipall, PreLoginEnc
-
-logger = logging.getLogger()
-
-# packet header
-# https://msdn.microsoft.com/en-us/library/dd340948.aspx
-_header = struct.Struct('>BBHHBx')
-
-_byte = struct.Struct('B')
-_smallint_le = struct.Struct('<h')
-_smallint_be = struct.Struct('>h')
-_usmallint_le = struct.Struct('<H')
-_usmallint_be = struct.Struct('>H')
-_int_le = struct.Struct('<l')
-_int_be = struct.Struct('>l')
-_uint_le = struct.Struct('<L')
-_uint_be = struct.Struct('>L')
-_int8_le = struct.Struct('<q')
-_int8_be = struct.Struct('>q')
-_uint8_le = struct.Struct('<Q')
-_uint8_be = struct.Struct('>Q')
-
-
-class SimpleLoadBalancer(object):
-    def __init__(self, hosts):
-        self._hosts = hosts
-
-    def choose(self):
-        for host in self._hosts:
-            yield host
-
-
-# stored procedure output parameter
-class output(object):
-    @property
-    def type(self):
-        """
-        This is either the sql type declaration or python type instance
-        of the parameter.
-        """
-        return self._type
-
-    @property
-    def value(self):
-        """
-        This is the value of the parameter.
-        """
-        return self._value
-
-    def __init__(self, value=None, param_type=None):
-        """ Creates procedure output parameter.
-
-        :param param_type: either sql type declaration or python type
-        :param value: value to pass into procedure
-        """
-        if param_type is None:
-            if value is None or value is default:
-                raise ValueError('Output type cannot be autodetected')
-        elif isinstance(param_type, type) and value is not None:
-            if value is not default and not isinstance(value, param_type):
-                raise ValueError('value should match param_type', value, param_type)
-        self._type = param_type
-        self._value = value
-
-
-class _Default(object):
-    pass
-
-default = _Default()
-
-
-def tds7_crypt_pass(password):
-    """ Mangle password according to tds rules
-
-    :param password: Password str
-    :returns: Byte-string with encoded password
-    """
-    encoded = bytearray(ucs2_codec.encode(password)[0])
-    for i, ch in enumerate(encoded):
-        encoded[i] = ((ch << 4) & 0xff | (ch >> 4)) ^ 0xA5
-    return encoded
-
-
-class _TdsEnv:
-    def __init__(self):
-        self.database = None
-        self.language = None
-        self.charset = None
-
-
-class _TdsReader(object):
-    """ TDS stream reader
-
-    Provides stream-like interface for TDS packeted stream.
-    Also provides convinience methods to decode primitive data like
-    different kinds of integers etc.
-    """
-    def __init__(self, session):
-        self._buf = ''
-        self._pos = 0  # position in the buffer
-        self._have = 0  # number of bytes read from packet
-        self._size = 0  # size of current packet
-        self._session = session
-        self._transport = session._transport
-        self._type = None
-        self._status = None
-
-    @property
-    def session(self):
-        """ Link to :class:`_TdsSession` object
-        """
-        return self._session
-
-    @property
-    def packet_type(self):
-        """ Type of current packet
-
-        Possible values are TDS_QUERY, TDS_LOGIN, etc.
-        """
-        return self._type
-
-    def read_fast(self, size):
-        """ Faster version of read
-
-        Instead of returning sliced buffer it returns reference to internal
-        buffer and the offset to this buffer.
-
-        :param size: Number of bytes to read
-        :returns: Tuple of bytes buffer, and offset in this buffer
-        """
-        if self._pos >= len(self._buf):
-            if self._have >= self._size:
-                self._read_packet()
-            else:
-                self._buf = self._transport.read(self._size - self._have)
-                self._pos = 0
-                self._have += len(self._buf)
-        offset = self._pos
-        self._pos += size
-        return self._buf, offset
-
-    def unpack(self, struc):
-        """ Unpacks given structure from stream
-
-        :param struc: A struct.Struct instance
-        :returns: Result of unpacking
-        """
-        buf, offset = readall_fast(self, struc.size)
-        return struc.unpack_from(buf, offset)
-
-    def get_byte(self):
-        """ Reads one byte from stream """
-        return self.unpack(_byte)[0]
-
-    def get_smallint(self):
-        """ Reads 16bit signed integer from the stream """
-        return self.unpack(_smallint_le)[0]
-
-    def get_usmallint(self):
-        """ Reads 16bit unsigned integer from the stream """
-        return self.unpack(_usmallint_le)[0]
-
-    def get_int(self):
-        """ Reads 32bit signed integer from the stream """
-        return self.unpack(_int_le)[0]
-
-    def get_uint(self):
-        """ Reads 32bit unsigned integer from the stream """
-        return self.unpack(_uint_le)[0]
-
-    def get_uint_be(self):
-        """ Reads 32bit unsigned big-endian integer from the stream """
-        return self.unpack(_uint_be)[0]
-
-    def get_uint8(self):
-        """ Reads 64bit unsigned integer from the stream """
-        return self.unpack(_uint8_le)[0]
-
-    def get_int8(self):
-        """ Reads 64bit signed integer from the stream """
-        return self.unpack(_int8_le)[0]
-
-    def read_ucs2(self, num_chars):
-        """ Reads num_chars UCS2 string from the stream """
-        buf = readall(self, num_chars * 2)
-        return ucs2_codec.decode(buf)[0]
-
-    def read_str(self, size, codec):
-        """ Reads byte string from the stream and decodes it
-
-        :param size: Size of string in bytes
-        :param codec: Instance of codec to decode string
-        :returns: Unicode string
-        """
-        return codec.decode(readall(self, size))[0]
-
-    def get_collation(self):
-        """ Reads :class:`Collation` object from stream """
-        buf = readall(self, Collation.wire_size)
-        return Collation.unpack(buf)
-
-    def unget_byte(self):
-        """ Returns one last read byte to stream
-
-        Can only be called once per read byte.
-        """
-        # this is a one trick pony...don't call it twice
-        assert self._pos > 0
-        self._pos -= 1
-
-    def peek(self):
-        """ Returns next byte from stream without consuming it
-        """
-        res = self.get_byte()
-        self.unget_byte()
-        return res
-
-    def read(self, size):
-        """ Reads size bytes from buffer
-
-        May return fewer bytes than requested
-        :param size: Number of bytes to read
-        :returns: Bytes buffer, possibly shorter than requested,
-                  returns empty buffer in case of EOF
-        """
-        buf, offset = self.read_fast(size)
-        return buf[offset:offset + size]
-
-    def _read_packet(self):
-        """ Reads next TDS packet from the underlying transport
-
-        If timeout is happened during reading of packet's header will
-        cancel current request.
-        Can only be called when transport's read pointer is at the begining
-        of the packet.
-        """
-        try:
-            header = readall(self._transport, _header.size)
-        except tds_base.TimeoutError:
-            self._session.put_cancel()
-            raise
-        self._pos = 0
-        self._type, self._status, self._size, self._session._spid, _ = _header.unpack(header)
-        self._have = _header.size
-        assert self._size > self._have, 'Empty packet doesn make any sense'
-        self._buf = self._transport.read(self._size - self._have)
-        self._have += len(self._buf)
-
-    def read_whole_packet(self):
-        """ Reads single packet and returns bytes payload of the packet
-
-        Can only be called when transport's read pointer is at the beginning
-        of the packet.
-        """
-        self._read_packet()
-        return readall(self, self._size - _header.size)
-
-
-class _TdsWriter(object):
-    """ TDS stream writer
-
-    Handles splitting of incoming data into TDS packets according to TDS protocol.
-    Provides convinience methods for writing primitive data types.
-    """
-    def __init__(self, session, bufsize):
-        self._session = session
-        self._tds = session
-        self._transport = session
-        self._pos = 0
-        self._buf = bytearray(bufsize)
-        self._packet_no = 0
-        self._type = 0
-
-    @property
-    def session(self):
-        """ Back reference to parent :class:`_TdsSession` object """
-        return self._session
-
-    @property
-    def bufsize(self):
-        """ Size of the buffer """
-        return len(self._buf)
-
-    @bufsize.setter
-    def bufsize(self, bufsize):
-        if len(self._buf) == bufsize:
-            return
-
-        if bufsize > len(self._buf):
-            self._buf.extend(b'\0' * (bufsize - len(self._buf)))
-        else:
-            self._buf = self._buf[0:bufsize]
-
-    def begin_packet(self, packet_type):
-        """ Starts new packet stream
-
-        :param packet_type: Type of TDS stream, e.g. TDS_PRELOGIN, TDS_QUERY etc.
-        """
-        self._type = packet_type
-        self._pos = 8
-
-    def pack(self, struc, *args):
-        """ Packs and writes structure into stream """
-        self.write(struc.pack(*args))
-
-    def put_byte(self, value):
-        """ Writes single byte into stream """
-        self.pack(_byte, value)
-
-    def put_smallint(self, value):
-        """ Writes 16-bit signed integer into the stream """
-        self.pack(_smallint_le, value)
-
-    def put_usmallint(self, value):
-        """ Writes 16-bit unsigned integer into the stream """
-        self.pack(_usmallint_le, value)
-
-    def put_smallint_be(self, value):
-        """ Writes 16-bit signed big-endian integer into the stream """
-        self.pack(_smallint_be, value)
-
-    def put_usmallint_be(self, value):
-        """ Writes 16-bit unsigned big-endian integer into the stream """
-        self.pack(_usmallint_be, value)
-
-    def put_int(self, value):
-        """ Writes 32-bit signed integer into the stream """
-        self.pack(_int_le, value)
-
-    def put_uint(self, value):
-        """ Writes 32-bit unsigned integer into the stream """
-        self.pack(_uint_le, value)
-
-    def put_int_be(self, value):
-        """ Writes 32-bit signed big-endian integer into the stream """
-        self.pack(_int_be, value)
-
-    def put_uint_be(self, value):
-        """ Writes 32-bit unsigned big-endian integer into the stream """
-        self.pack(_uint_be, value)
-
-    def put_int8(self, value):
-        """ Writes 64-bit signed integer into the stream """
-        self.pack(_int8_le, value)
-
-    def put_uint8(self, value):
-        """ Writes 64-bit unsigned integer into the stream """
-        self.pack(_uint8_le, value)
-
-    def put_collation(self, collation):
-        """ Writes :class:`Collation` structure into the stream """
-        self.write(collation.pack())
-
-    def write(self, data):
-        """ Writes given bytes buffer into the stream
-
-        Function returns only when entire buffer is written
-        """
-        data_off = 0
-        while data_off < len(data):
-            left = len(self._buf) - self._pos
-            if left <= 0:
-                self._write_packet(final=False)
-            else:
-                to_write = min(left, len(data) - data_off)
-                self._buf[self._pos:self._pos + to_write] = data[data_off:data_off + to_write]
-                self._pos += to_write
-                data_off += to_write
-
-    def write_b_varchar(self, s):
-        self.put_byte(len(s))
-        self.write_ucs2(s)
-
-    def write_ucs2(self, s):
-        """ Write string encoding it in UCS2 into stream """
-        self.write_string(s, ucs2_codec)
-
-    def write_string(self, s, codec):
-        """ Write string encoding it with codec into stream """
-        for i in range(0, len(s), self.bufsize):
-            chunk = s[i:i + self.bufsize]
-            buf, consumed = codec.encode(chunk)
-            assert consumed == len(chunk)
-            self.write(buf)
-
-    def flush(self):
-        """ Closes current packet stream """
-        return self._write_packet(final=True)
-
-    def _write_packet(self, final):
-        """ Writes single TDS packet into underlying transport.
-
-        Data for the packet is taken from internal buffer.
-
-        :param final: True means this is the final packet in substream.
-        """
-        status = 1 if final else 0
-        _header.pack_into(self._buf, 0, self._type, status, self._pos, 0, self._packet_no)
-        self._packet_no = (self._packet_no + 1) % 256
-        self._transport.send(self._buf[:self._pos], final)
-        self._pos = 8
-
-
-class MemoryChunkedHandler(object):
-    def __init__(self):
-        self.size = 0
-        self._chunks = []
-        self._column = None
-
-    def begin(self, column, size):
-        self.size = size
-        self._chunks = []
-        self._column = column
-
-    def new_chunk(self, val):
-        self._chunks.append(val)
-
-    def end(self):
-        return b''.join(self._chunks)
-
-
-class MemoryStrChunkedHandler(object):
-    def __init__(self):
-        self.size = 0
-        self._chunks = []
-        self._column = None
-
-    def begin(self, column, size):
-        self.size = size
-        self._chunks = []
-        self._column = column
-
-    def new_chunk(self, val):
-        self._chunks.append(val)
-
-    def end(self):
-        return ''.join(self._chunks)
-
-
-def _create_exception_by_message(msg, custom_error_msg=None):
-    msg_no = msg['msgno']
-    if custom_error_msg is not None:
-        error_msg = custom_error_msg
-    else:
-        error_msg = msg['message']
-    if msg_no in tds_base.prog_errors:
-        ex = tds_base.ProgrammingError(error_msg)
-    elif msg_no in tds_base.integrity_errors:
-        ex = tds_base.IntegrityError(error_msg)
-    else:
-        ex = tds_base.OperationalError(error_msg)
-    ex.msg_no = msg['msgno']
-    ex.text = msg['message']
-    ex.srvname = msg['server']
-    ex.procname = msg['proc_name']
-    ex.number = msg['msgno']
-    ex.severity = msg['severity']
-    ex.state = msg['state']
-    ex.line = msg['line_number']
-    return ex
-
-
-class _TdsSession(object):
-    """ TDS session
-
-    Represents a single TDS session within MARS connection, when MARS enabled there could be multiple TDS sessions
-    within one connection.
-    """
-    def __init__(self, tds, transport, tzinfo_factory):
-        self.out_pos = 8
-        self.res_info = None
-        self.in_cancel = False
-        self.wire_mtx = None
-        self.param_info = None
-        self.has_status = False
-        self.ret_status = None
-        self.skipped_to_status = False
-        self._transport = transport
-        self._reader = _TdsReader(self)
-        self._reader._transport = transport
-        self._writer = _TdsWriter(self, tds.bufsize)
-        self._writer._transport = transport
-        self.in_buf_max = 0
-        self.state = tds_base.TDS_IDLE
-        self._tds = tds
-        self.messages = []
-        self.chunk_handler = tds.chunk_handler
-        self.rows_affected = -1
-        self.use_tz = tds.use_tz
-        self._spid = 0
-        self.tzinfo_factory = tzinfo_factory
-        self.more_rows = False
-        self.done_flags = 0
-        self.internal_sp_called = 0
-        self.output_params = {}
-        self.authentication = None
-        self.return_value_index = 0
-        self._out_params_indexes = []
-        self.row = None
-        self.end_marker = 0
-
-    def __repr__(self):
-        fmt = "<_TdsSession state={} tds={} messages={} rows_affected={} use_tz={} spid={} in_cancel={}>"
-        res = fmt.format(repr(self.state), repr(self._tds), repr(self.messages),
-                         repr(self.rows_affected), repr(self.use_tz), repr(self._spid),
-                         self.in_cancel)
-        return res
-
-    def raise_db_exception(self):
-        """ Raises exception from last server message
-
-        This function will skip messages: The statement has been terminated
-        """
-        if not self.messages:
-            raise tds_base.Error("Request failed, server didn't send error message")
-        msg = None
-        while True:
-            msg = self.messages[-1]
-            if msg['msgno'] == 3621:  # the statement has been terminated
-                self.messages = self.messages[:-1]
-            else:
-                break
-
-        error_msg = ' '.join(m['message'] for m in self.messages)
-        ex = _create_exception_by_message(msg, error_msg)
-        raise ex
-
-    def get_type_info(self, curcol):
-        """ Reads TYPE_INFO structure (http://msdn.microsoft.com/en-us/library/dd358284.aspx)
-
-        :param curcol: An instance of :class:`Column` that will receive read information
-        """
-        r = self._reader
-        # User defined data type of the column
-        curcol.column_usertype = r.get_uint() if tds_base.IS_TDS72_PLUS(self) else r.get_usmallint()
-        curcol.flags = r.get_usmallint()  # Flags
-        type_id = r.get_byte()
-        serializer_class = self._tds.type_factory.get_type_serializer(type_id)
-        curcol.serializer = serializer_class.from_stream(r)
-
-    def tds7_process_result(self):
-        """ Reads and processes COLMETADATA stream
-
-        This stream contains a list of returned columns.
-        Stream format link: http://msdn.microsoft.com/en-us/library/dd357363.aspx
-        """
-        r = self._reader
-
-        # read number of columns and allocate the columns structure
-
-        num_cols = r.get_smallint()
-
-        # This can be a DUMMY results token from a cursor fetch
-
-        if num_cols == -1:
-            return
-
-        self.param_info = None
-        self.has_status = False
-        self.ret_status = None
-        self.skipped_to_status = False
-        self.rows_affected = tds_base.TDS_NO_COUNT
-        self.more_rows = True
-        self.row = [None] * num_cols
-        self.res_info = info = _Results()
-
-        #
-        # loop through the columns populating COLINFO struct from
-        # server response
-        #
-        header_tuple = []
-        for col in range(num_cols):
-            curcol = tds_base.Column()
-            info.columns.append(curcol)
-            self.get_type_info(curcol)
-
-            curcol.column_name = r.read_ucs2(r.get_byte())
-            precision = curcol.serializer.precision
-            scale = curcol.serializer.scale
-            size = curcol.serializer.size
-            header_tuple.append(
-                (curcol.column_name,
-                 curcol.serializer.get_typeid(),
-                 None,
-                 size,
-                 precision,
-                 scale,
-                 curcol.flags & tds_base.Column.fNullable))
-        info.description = tuple(header_tuple)
-        return info
-
-    def process_param(self):
-        """ Reads and processes RETURNVALUE stream.
-
-        This stream is used to send OUTPUT parameters from RPC to client.
-        Stream format url: http://msdn.microsoft.com/en-us/library/dd303881.aspx
-        """
-        r = self._reader
-        if tds_base.IS_TDS72_PLUS(self):
-            ordinal = r.get_usmallint()
-        else:
-            r.get_usmallint()  # ignore size
-            ordinal = self._out_params_indexes[self.return_value_index]
-        name = r.read_ucs2(r.get_byte())
-        r.get_byte()  # 1 - OUTPUT of sp, 2 - result of udf
-        param = tds_base.Column()
-        param.column_name = name
-        self.get_type_info(param)
-        param.value = param.serializer.read(r)
-        self.output_params[ordinal] = param
-        self.return_value_index += 1
-
-    def process_cancel(self):
-        """
-        Process the incoming token stream until it finds
-        an end token DONE with the cancel flag set.
-        At that point the connection should be ready to handle a new query.
-
-        In case when no cancel request is pending this function does nothing.
-        """
-        # silly cases, nothing to do
-        if not self.in_cancel:
-            return
-
-        while True:
-            token_id = self.get_token_id()
-            self.process_token(token_id)
-            if not self.in_cancel:
-                return
-
-    def process_msg(self, marker):
-        """ Reads and processes ERROR/INFO streams
-
-        Stream formats:
-
-        - ERROR: http://msdn.microsoft.com/en-us/library/dd304156.aspx
-        - INFO: http://msdn.microsoft.com/en-us/library/dd303398.aspx
-
-        :param marker: TDS_ERROR_TOKEN or TDS_INFO_TOKEN
-        """
-        r = self._reader
-        r.get_smallint()  # size
-        msg = {'marker': marker, 'msgno': r.get_int(), 'state': r.get_byte(), 'severity': r.get_byte(),
-               'sql_state': None}
-        has_eed = False
-        if marker == tds_base.TDS_EED_TOKEN:
-            if msg['severity'] <= 10:
-                msg['priv_msg_type'] = 0
-            else:
-                msg['priv_msg_type'] = 1
-            len_sqlstate = r.get_byte()
-            msg['sql_state'] = readall(r, len_sqlstate)
-            has_eed = r.get_byte()
-            # junk status and transaction state
-            r.get_smallint()
-        elif marker == tds_base.TDS_INFO_TOKEN:
-            msg['priv_msg_type'] = 0
-        elif marker == tds_base.TDS_ERROR_TOKEN:
-            msg['priv_msg_type'] = 1
-        else:
-            logger.error('tds_process_msg() called with unknown marker "{0}"'.format(marker))
-        msg['message'] = r.read_ucs2(r.get_smallint())
-        # server name
-        msg['server'] = r.read_ucs2(r.get_byte())
-        # stored proc name if available
-        msg['proc_name'] = r.read_ucs2(r.get_byte())
-        msg['line_number'] = r.get_int() if tds_base.IS_TDS72_PLUS(self) else r.get_smallint()
-        # in case extended error data is sent, we just try to discard it
-        if has_eed:
-            while True:
-                next_marker = r.get_byte()
-                if next_marker in (tds_base.TDS5_PARAMFMT_TOKEN,
-                                   tds_base.TDS5_PARAMFMT2_TOKEN,
-                                   tds_base.TDS5_PARAMS_TOKEN):
-                    self.process_token(next_marker)
-                else:
-                    break
-            r.unget_byte()
-
-        # special case
-        self.messages.append(msg)
-
-    def process_row(self):
-        """ Reads and handles ROW stream.
-
-        This stream contains list of values of one returned row.
-        Stream format url: http://msdn.microsoft.com/en-us/library/dd357254.aspx
-        """
-        r = self._reader
-        info = self.res_info
-        info.row_count += 1
-        for i, curcol in enumerate(info.columns):
-            curcol.value = self.row[i] = curcol.serializer.read(r)
-
-    def process_nbcrow(self):
-        """ Reads and handles NBCROW stream.
-
-        This stream contains list of values of one returned row in a compressed way,
-        introduced in TDS 7.3.B
-        Stream format url: http://msdn.microsoft.com/en-us/library/dd304783.aspx
-        """
-        r = self._reader
-        info = self.res_info
-        if not info:
-            self.bad_stream('got row without info')
-        assert len(info.columns) > 0
-        info.row_count += 1
-
-        # reading bitarray for nulls, 1 represent null values for
-        # corresponding fields
-        nbc = readall(r, (len(info.columns) + 7) // 8)
-        for i, curcol in enumerate(info.columns):
-            if tds_base.my_ord(nbc[i // 8]) & (1 << (i % 8)):
-                value = None
-            else:
-                value = curcol.serializer.read(r)
-            self.row[i] = value
-
-    def process_orderby(self):
-        """ Reads and processes ORDER stream
-
-        Used to inform client by which column dataset is ordered.
-        Stream format url: http://msdn.microsoft.com/en-us/library/dd303317.aspx
-        """
-        r = self._reader
-        skipall(r, r.get_smallint())
-
-    def process_orderby2(self):
-        r = self._reader
-        skipall(r, r.get_int())
-
-    def process_end(self, marker):
-        """ Reads and processes DONE/DONEINPROC/DONEPROC streams
-
-        Stream format urls:
-
-        - DONE: http://msdn.microsoft.com/en-us/library/dd340421.aspx
-        - DONEINPROC: http://msdn.microsoft.com/en-us/library/dd340553.aspx
-        - DONEPROC: http://msdn.microsoft.com/en-us/library/dd340753.aspx
-
-        :param marker: Can be TDS_DONE_TOKEN or TDS_DONEINPROC_TOKEN or TDS_DONEPROC_TOKEN
-        """
-        self.end_marker = marker
-        self.more_rows = False
-        r = self._reader
-        status = r.get_usmallint()
-        r.get_usmallint()  # cur_cmd
-        more_results = status & tds_base.TDS_DONE_MORE_RESULTS != 0
-        was_cancelled = status & tds_base.TDS_DONE_CANCELLED != 0
-        done_count_valid = status & tds_base.TDS_DONE_COUNT != 0
-        if self.res_info:
-            self.res_info.more_results = more_results
-        rows_affected = r.get_int8() if tds_base.IS_TDS72_PLUS(self) else r.get_int()
-        if was_cancelled or (not more_results and not self.in_cancel):
-            self.in_cancel = False
-            self.set_state(tds_base.TDS_IDLE)
-        if done_count_valid:
-            self.rows_affected = rows_affected
-        else:
-            self.rows_affected = -1
-        self.done_flags = status
-        if self.done_flags & tds_base.TDS_DONE_ERROR and not was_cancelled and not self.in_cancel:
-            self.raise_db_exception()
-
-    def process_env_chg(self):
-        """ Reads and processes ENVCHANGE stream.
-
-        Stream info url: http://msdn.microsoft.com/en-us/library/dd303449.aspx
-        """
-        r = self._reader
-        size = r.get_smallint()
-        type_id = r.get_byte()
-        if type_id == tds_base.TDS_ENV_SQLCOLLATION:
-            size = r.get_byte()
-            self.conn.collation = r.get_collation()
-            skipall(r, size - 5)
-            # discard old one
-            skipall(r, r.get_byte())
-        elif type_id == tds_base.TDS_ENV_BEGINTRANS:
-            size = r.get_byte()
-            assert size == 8
-            self.conn.tds72_transaction = r.get_uint8()
-            skipall(r, r.get_byte())
-        elif type_id == tds_base.TDS_ENV_COMMITTRANS or type_id == tds_base.TDS_ENV_ROLLBACKTRANS:
-            self.conn.tds72_transaction = 0
-            skipall(r, r.get_byte())
-            skipall(r, r.get_byte())
-        elif type_id == tds_base.TDS_ENV_PACKSIZE:
-            newval = r.read_ucs2(r.get_byte())
-            r.read_ucs2(r.get_byte())
-            new_block_size = int(newval)
-            if new_block_size >= 512:
-                # Is possible to have a shrink if server limits packet
-                # size more than what we specified
-                #
-                # Reallocate buffer if possible (strange values from server or out of memory) use older buffer */
-                self._writer.bufsize = new_block_size
-        elif type_id == tds_base.TDS_ENV_DATABASE:
-            newval = r.read_ucs2(r.get_byte())
-            r.read_ucs2(r.get_byte())
-            self.conn.env.database = newval
-        elif type_id == tds_base.TDS_ENV_LANG:
-            newval = r.read_ucs2(r.get_byte())
-            r.read_ucs2(r.get_byte())
-            self.conn.env.language = newval
-        elif type_id == tds_base.TDS_ENV_CHARSET:
-            newval = r.read_ucs2(r.get_byte())
-            r.read_ucs2(r.get_byte())
-            self.conn.env.charset = newval
-            remap = {'iso_1': 'iso8859-1'}
-            self.conn.server_codec = codecs.lookup(remap.get(newval, newval))
-        elif type_id == tds_base.TDS_ENV_DB_MIRRORING_PARTNER:
-            r.read_ucs2(r.get_byte())
-            r.read_ucs2(r.get_byte())
-        elif type_id == tds_base.TDS_ENV_LCID:
-            lcid = int(r.read_ucs2(r.get_byte()))
-            self.conn.server_codec = codecs.lookup(lcid2charset(lcid))
-            r.read_ucs2(r.get_byte())
-        else:
-            logger.warning("unknown env type: {0}, skipping".format(type_id))
-            # discard byte values, not still supported
-            skipall(r, size - 1)
-
-    def process_auth(self):
-        """ Reads and processes SSPI stream.
-
-        Stream info: http://msdn.microsoft.com/en-us/library/dd302844.aspx
-        """
-        r = self._reader
-        w = self._writer
-        pdu_size = r.get_smallint()
-        if not self.authentication:
-            raise tds_base.Error('Got unexpected token')
-        packet = self.authentication.handle_next(readall(r, pdu_size))
-        if packet:
-            w.write(packet)
-            w.flush()
-
-    def is_connected(self):
-        """
-        :return: True if transport is connected
-        """
-        return self._transport.is_connected()
-
-    def bad_stream(self, msg):
-        """ Called when input stream contains unexpected data.
-
-        Will close stream and raise :class:`InterfaceError`
-        :param msg: Message for InterfaceError exception.
-        :return: Never returns, always raises exception.
-        """
-        self.close()
-        raise tds_base.InterfaceError(msg)
-
-    @property
-    def tds_version(self):
-        """ Returns integer encoded current TDS protocol version
-        """
-        return self._tds.tds_version
-
-    @property
-    def conn(self):
-        """ Reference to owning :class:`_TdsSocket`
-        """
-        return self._tds
-
-    def close(self):
-        self._transport.close()
-
-    def set_state(self, state):
-        """ Switches state of the TDS session.
-
-        It also does state transitions checks.
-        :param state: New state, one of TDS_PENDING/TDS_READING/TDS_IDLE/TDS_DEAD/TDS_QUERING
-        """
-        prior_state = self.state
-        if state == prior_state:
-            return state
-        if state == tds_base.TDS_PENDING:
-            if prior_state in (tds_base.TDS_READING, tds_base.TDS_QUERYING):
-                self.state = tds_base.TDS_PENDING
-            else:
-                raise tds_base.InterfaceError('logic error: cannot chage query state from {0} to {1}'.
-                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
-        elif state == tds_base.TDS_READING:
-            # transition to READING are valid only from PENDING
-            if self.state != tds_base.TDS_PENDING:
-                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
-                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
-            else:
-                self.state = state
-        elif state == tds_base.TDS_IDLE:
-            if prior_state == tds_base.TDS_DEAD:
-                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
-                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
-            self.state = state
-        elif state == tds_base.TDS_DEAD:
-            self.state = state
-        elif state == tds_base.TDS_QUERYING:
-            if self.state == tds_base.TDS_DEAD:
-                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
-                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
-            elif self.state != tds_base.TDS_IDLE:
-                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
-                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
-            else:
-                self.rows_affected = tds_base.TDS_NO_COUNT
-                self.internal_sp_called = 0
-                self.state = state
-        else:
-            assert False
-        return self.state
-
-    @contextlib.contextmanager
-    def querying_context(self, packet_type):
-        """ Context manager for querying.
-
-        Sets state to TDS_QUERYING, and reverts it to TDS_IDLE if exception happens inside managed block,
-        and to TDS_PENDING if managed block succeeds and flushes buffer.
-        """
-        if self.set_state(tds_base.TDS_QUERYING) != tds_base.TDS_QUERYING:
-            raise tds_base.Error("Couldn't switch to state")
-        self._writer.begin_packet(packet_type)
-        try:
-            yield
-        except:
-            if self.state != tds_base.TDS_DEAD:
-                self.set_state(tds_base.TDS_IDLE)
-            raise
-        else:
-            self.set_state(tds_base.TDS_PENDING)
-            self._writer.flush()
-
-    def make_param(self, name, value):
-        """ Generates instance of :class:`Column` from value and name
-
-        Value can also be of a special types:
-
-        - An instance of :class:`Column`, in which case it is just returned.
-        - An instance of :class:`output`, in which case parameter will become
-          an output parameter.
-        - A singleton :var:`default`, in which case default value will be passed
-          into a stored proc.
-
-        :param name: Name of the parameter, will populate column_name property of returned column.
-        :param value: Value of the parameter, also used to guess the type of parameter.
-        :return: An instance of :class:`Column`
-        """
-        if isinstance(value, tds_base.Column):
-            value.column_name = name
-            return value
-        column = tds_base.Column()
-        column.column_name = name
-        column.flags = 0
-        
-        if isinstance(value, output):
-            column.flags |= tds_base.fByRefValue
-            if isinstance(value.type, six.string_types):
-                column.type = tds_types.sql_type_by_declaration(value.type)
-            elif value.type:
-                column.type = self.conn.type_inferrer.from_class(value.type)
-            value = value.value
-
-        if value is default:
-            column.flags |= tds_base.fDefaultValue
-            value = None
-
-        column.value = value
-        if column.type is None:
-            column.type = self.conn.type_inferrer.from_value(value)
-        return column
-
-    def _convert_params(self, parameters):
-        """ Converts a dict of list of parameters into a list of :class:`Column` instances.
-
-        :param parameters: Can be a list of parameter values, or a dict of parameter names to values.
-        :return: A list of :class:`Column` instances.
-        """
-        if isinstance(parameters, dict):
-            return [self.make_param(name, value)
-                    for name, value in parameters.items()]
-        else:
-            params = []
-            for parameter in parameters:
-                params.append(self.make_param('', parameter))
-            return params
-
-    def cancel_if_pending(self):
-        """ Cancels current pending request.
-
-        Does nothing if no request is pending, otherwise sends cancel request,
-        and waits for response.
-        """
-        if self.state == tds_base.TDS_IDLE:
-            return
-        if not self.in_cancel:
-            self.put_cancel()
-        self.process_cancel()
-
-    def submit_rpc(self, rpc_name, params, flags):
-        """ Sends an RPC request.
-
-        This call will transition session into pending state.
-        If some operation is currently pending on the session, it will be
-        cancelled before sending this request.
-
-        Spec: http://msdn.microsoft.com/en-us/library/dd357576.aspx
-
-        :param rpc_name: Name of the RPC to call, can be an instance of :class:`InternalProc`
-        :param params: Stored proc parameters, should be a list of :class:`Column` instances.
-        :param flags: See spec for possible flags.
-        """
-        self.messages = []
-        self.output_params = {}
-        self.cancel_if_pending()
-        self.res_info = None
-        w = self._writer
-        with self.querying_context(tds_base.TDS_RPC):
-            if tds_base.IS_TDS72_PLUS(self):
-                self._start_query()
-            if tds_base.IS_TDS71_PLUS(self) and isinstance(rpc_name, tds_base.InternalProc):
-                w.put_smallint(-1)
-                w.put_smallint(rpc_name.proc_id)
-            else:
-                if isinstance(rpc_name, tds_base.InternalProc):
-                    rpc_name = rpc_name.name
-                w.put_smallint(len(rpc_name))
-                w.write_ucs2(rpc_name)
-            #
-            # TODO support flags
-            # bit 0 (1 as flag) in TDS7/TDS5 is "recompile"
-            # bit 1 (2 as flag) in TDS7+ is "no metadata" bit this will prevent sending of column infos
-            #
-            w.put_usmallint(flags)
-            self._out_params_indexes = []
-            for i, param in enumerate(params):
-                if param.flags & tds_base.fByRefValue:
-                    self._out_params_indexes.append(i)
-                w.put_byte(len(param.column_name))
-                w.write_ucs2(param.column_name)
-                #
-                # TODO support other flags (use defaul null/no metadata)
-                # bit 1 (2 as flag) in TDS7+ is "default value" bit
-                # (what's the meaning of "default value" ?)
-                #
-                w.put_byte(param.flags)
-
-                # TYPE_INFO structure: https://msdn.microsoft.com/en-us/library/dd358284.aspx
-                serializer = param.choose_serializer(
-                    type_factory=self._tds.type_factory,
-                    collation=self._tds.collation or raw_collation
-                )
-                type_id = serializer.type
-                w.put_byte(type_id)
-                serializer.write_info(w)
-
-                serializer.write(w, param.value)
-
-    def submit_plain_query(self, operation):
-        """ Sends a plain query to server.
-
-        This call will transition session into pending state.
-        If some operation is currently pending on the session, it will be
-        cancelled before sending this request.
-
-        Spec: http://msdn.microsoft.com/en-us/library/dd358575.aspx
-
-        :param operation: A string representing sql statement.
-        """
-        self.messages = []
-        self.cancel_if_pending()
-        self.res_info = None
-        w = self._writer
-        with self.querying_context(tds_base.TDS_QUERY):
-            if tds_base.IS_TDS72_PLUS(self):
-                self._start_query()
-            w.write_ucs2(operation)
-
-    def submit_bulk(self, metadata, rows):
-        """ Sends insert bulk command.
-
-        Spec: http://msdn.microsoft.com/en-us/library/dd358082.aspx
-
-        :param metadata: A list of :class:`Column` instances.
-        :param rows: A collection of rows, each row is a collection of values.
-        :return:
-        """
-        num_cols = len(metadata)
-        w = self._writer
-        serializers = []
-        with self.querying_context(tds_base.TDS_BULK):
-            w.put_byte(tds_base.TDS7_RESULT_TOKEN)
-            w.put_usmallint(num_cols)
-            for col in metadata:
-                if tds_base.IS_TDS72_PLUS(self):
-                    w.put_uint(col.column_usertype)
-                else:
-                    w.put_usmallint(col.column_usertype)
-                w.put_usmallint(col.flags)
-                serializer = col.choose_serializer(
-                    type_factory=self._tds.type_factory,
-                    collation=self._tds.collation,
-                )
-                type_id = serializer.type
-                w.put_byte(type_id)
-                serializers.append(serializer)
-                serializer.write_info(w)
-                w.put_byte(len(col.column_name))
-                w.write_ucs2(col.column_name)
-            for row in rows:
-                w.put_byte(tds_base.TDS_ROW_TOKEN)
-                for i, col in enumerate(metadata):
-                    serializers[i].write(w, row[i])
-
-            w.put_byte(tds_base.TDS_DONE_TOKEN)
-            w.put_usmallint(tds_base.TDS_DONE_FINAL)
-            w.put_usmallint(0)  # curcmd
-            if tds_base.IS_TDS72_PLUS(self):
-                w.put_int8(0)
-            else:
-                w.put_int(0)
-
-    def put_cancel(self):
-        """ Sends a cancel request to the server.
-
-        Switches connection to IN_CANCEL state.
-        """
-        self._writer.begin_packet(tds_base.TDS_CANCEL)
-        self._writer.flush()
-        self.in_cancel = 1
-
-    _begin_tran_struct_72 = struct.Struct('<HBB')
-
-    def begin_tran(self, isolation_level=0):
-        self.submit_begin_tran(isolation_level=isolation_level)
-        self.process_simple_request()
-
-    def submit_begin_tran(self, isolation_level=0):
-        if tds_base.IS_TDS72_PLUS(self):
-            self.messages = []
-            self.cancel_if_pending()
-            w = self._writer
-            with self.querying_context(tds_base.TDS7_TRANS):
-                self._start_query()
-                w.pack(
-                    self._begin_tran_struct_72,
-                    5,  # TM_BEGIN_XACT
-                    isolation_level,
-                    0,  # new transaction name
-                    )
-        else:
-            self.submit_plain_query("BEGIN TRANSACTION")
-            self.conn.tds72_transaction = 1
-
-    _commit_rollback_tran_struct72_hdr = struct.Struct('<HBB')
-    _continue_tran_struct72 = struct.Struct('<BB')
-
-    def rollback(self, cont, isolation_level=0):
-        self.submit_rollback(cont, isolation_level=isolation_level)
-        prev_timeout = self._tds.sock.gettimeout()
-        self._tds.sock.settimeout(None)
-        try:
-            self.process_simple_request()
-        finally:
-            self._tds.sock.settimeout(prev_timeout)
-
-    def submit_rollback(self, cont, isolation_level=0):
-        if tds_base.IS_TDS72_PLUS(self):
-            self.messages = []
-            self.cancel_if_pending()
-            w = self._writer
-            with self.querying_context(tds_base.TDS7_TRANS):
-                self._start_query()
-                flags = 0
-                if cont:
-                    flags |= 1
-                w.pack(
-                    self._commit_rollback_tran_struct72_hdr,
-                    8,  # TM_ROLLBACK_XACT
-                    0,  # transaction name
-                    flags,
-                    )
-                if cont:
-                    w.pack(
-                        self._continue_tran_struct72,
-                        isolation_level,
-                        0,  # new transaction name
-                        )
-        else:
-            self.submit_plain_query(
-                "IF @@TRANCOUNT > 0 ROLLBACK BEGIN TRANSACTION" if cont else "IF @@TRANCOUNT > 0 ROLLBACK")
-            self.conn.tds72_transaction = 1 if cont else 0
-
-    def commit(self, cont, isolation_level=0):
-        self.submit_commit(cont, isolation_level=isolation_level)
-        prev_timeout = self._tds.sock.gettimeout()
-        self._tds.sock.settimeout(None)
-        try:
-            self.process_simple_request()
-        finally:
-            self._tds.sock.settimeout(prev_timeout)
-
-    def submit_commit(self, cont, isolation_level=0):
-        if tds_base.IS_TDS72_PLUS(self):
-            self.messages = []
-            self.cancel_if_pending()
-            w = self._writer
-            with self.querying_context(tds_base.TDS7_TRANS):
-                self._start_query()
-                flags = 0
-                if cont:
-                    flags |= 1
-                w.pack(
-                    self._commit_rollback_tran_struct72_hdr,
-                    7,  # TM_COMMIT_XACT
-                    0,  # transaction name
-                    flags,
-                    )
-                if cont:
-                    w.pack(
-                        self._continue_tran_struct72,
-                        isolation_level,
-                        0,  # new transaction name
-                        )
-        else:
-            self.submit_plain_query(
-                "IF @@TRANCOUNT > 0 COMMIT BEGIN TRANSACTION" if cont else "IF @@TRANCOUNT > 0 COMMIT")
-            self.conn.tds72_transaction = 1 if cont else 0
-
-    _tds72_query_start = struct.Struct('<IIHQI')
-
-    def _start_query(self):
-        w = self._writer
-        w.pack(_TdsSession._tds72_query_start,
-               0x16,  # total length
-               0x12,  # length
-               2,  # type
-               self.conn.tds72_transaction,
-               1,  # request count
-               )
-
-    VERSION = 0
-    ENCRYPTION = 1
-    INSTOPT = 2
-    THREADID = 3
-    MARS = 4
-    TRACEID = 5
-    TERMINATOR = 0xff
-
-    def send_prelogin(self, login):
-        # https://msdn.microsoft.com/en-us/library/dd357559.aspx
-        instance_name = login.instance_name or 'MSSQLServer'
-        instance_name = instance_name.encode('ascii')
-        if len(instance_name) > 65490:
-            raise ValueError('Instance name is too long')
-        if tds_base.IS_TDS72_PLUS(self):
-            start_pos = 26
-            buf = struct.pack(
-                b'>BHHBHHBHHBHHBHHB',
-                # netlib version
-                self.VERSION, start_pos, 6,
-                # encryption
-                self.ENCRYPTION, start_pos + 6, 1,
-                # instance
-                self.INSTOPT, start_pos + 6 + 1, len(instance_name) + 1,
-                # thread id
-                self.THREADID, start_pos + 6 + 1 + len(instance_name) + 1, 4,
-                # MARS enabled
-                self.MARS, start_pos + 6 + 1 + len(instance_name) + 1 + 4, 1,
-                # end
-                self.TERMINATOR
-                )
-        else:
-            start_pos = 21
-            buf = struct.pack(
-                b'>BHHBHHBHHBHHB',
-                # netlib version
-                self.VERSION, start_pos, 6,
-                # encryption
-                self.ENCRYPTION, start_pos + 6, 1,
-                # instance
-                self.INSTOPT, start_pos + 6 + 1, len(instance_name) + 1,
-                # thread id
-                self.THREADID, start_pos + 6 + 1 + len(instance_name) + 1, 4,
-                # end
-                self.TERMINATOR
-                )
-        assert start_pos == len(buf)
-        w = self._writer
-        w.begin_packet(tds_base.TDS71_PRELOGIN)
-        w.write(buf)
-        from . import intversion
-        w.put_uint_be(intversion)
-        w.put_usmallint_be(0)  # build number
-        # encryption flag
-        w.put_byte(login.enc_flag)
-        w.write(instance_name)
-        w.put_byte(0)  # zero terminate instance_name
-        w.put_int(0)  # TODO: change this to thread id
-        if tds_base.IS_TDS72_PLUS(self):
-            # MARS (1 enabled)
-            w.put_byte(1 if login.use_mars else 0)
-        w.flush()
-
-    def process_prelogin(self, login):
-        # https://msdn.microsoft.com/en-us/library/dd357559.aspx
-        p = self._reader.read_whole_packet()
-        size = len(p)
-        if size <= 0 or self._reader.packet_type != 4:
-            self.bad_stream('Invalid packet type: {0}, expected PRELOGIN(4)'.format(self._reader.packet_type))
-        # default 2, no certificate, no encryptption
-        crypt_flag = 2
-        i = 0
-        byte_struct = struct.Struct('B')
-        off_len_struct = struct.Struct('>HH')
-        prod_version_struct = struct.Struct('>LH')
-        while True:
-            if i >= size:
-                self.bad_stream('Invalid size of PRELOGIN structure')
-            type_id, = byte_struct.unpack_from(p, i)
-            if type_id == 0xff:
-                break
-            if i + 4 > size:
-                self.bad_stream('Invalid size of PRELOGIN structure')
-            off, l = off_len_struct.unpack_from(p, i + 1)
-            if off > size or off + l > size:
-                self.bad_stream('Invalid offset in PRELOGIN structure')
-            if type_id == self.VERSION:
-                self.conn.server_library_version = prod_version_struct.unpack_from(p, off)
-            elif type_id == self.ENCRYPTION and l >= 1:
-                crypt_flag, = byte_struct.unpack_from(p, off)
-            elif type_id == self.MARS:
-                self.conn._mars_enabled = bool(byte_struct.unpack_from(p, off)[0])
-            elif type_id == self.INSTOPT:
-                # ignore instance name mismatch
-                pass
-            i += 5
-        # if server do not has certificate do normal login
-        login.server_enc_flag = crypt_flag
-        if crypt_flag == PreLoginEnc.ENCRYPT_OFF:
-            if login.enc_flag == PreLoginEnc.ENCRYPT_ON:
-                raise tds_base.Error('Server returned unexpected ENCRYPT_ON value')
-            else:
-                # encrypt login packet only
-                tls.establish_channel(self)
-        elif crypt_flag == PreLoginEnc.ENCRYPT_ON:
-            # encrypt entire connection
-            tls.establish_channel(self)
-        elif crypt_flag == PreLoginEnc.ENCRYPT_REQ:
-            if login.enc_flag == PreLoginEnc.ENCRYPT_NOT_SUP:
-                raise tds_base.Error('Client does not have encryption enabled but it is required by server, '
-                                     'enable encryption and try connecting again')
-            else:
-                # encrypt entire connection
-                tls.establish_channel(self)
-        elif crypt_flag == PreLoginEnc.ENCRYPT_NOT_SUP:
-            if login.enc_flag == PreLoginEnc.ENCRYPT_ON:
-                raise tds_base.Error('You requested encryption but it is not supported by server')
-            # do not encrypt anything
-
-    def tds7_send_login(self, login):
-        # https://msdn.microsoft.com/en-us/library/dd304019.aspx
-        option_flag2 = login.option_flag2
-        user_name = login.user_name
-        if len(user_name) > 128:
-            raise ValueError('User name should be no longer that 128 characters')
-        if len(login.password) > 128:
-            raise ValueError('Password should be not longer than 128 characters')
-        if len(login.change_password) > 128:
-            raise ValueError('Password should be not longer than 128 characters')
-        if len(login.client_host_name) > 128:
-            raise ValueError('Host name should be not longer than 128 characters')
-        if len(login.app_name) > 128:
-            raise ValueError('App name should be not longer than 128 characters')
-        if len(login.server_name) > 128:
-            raise ValueError('Server name should be not longer than 128 characters')
-        if len(login.database) > 128:
-            raise ValueError('Database name should be not longer than 128 characters')
-        if len(login.language) > 128:
-            raise ValueError('Language should be not longer than 128 characters')
-        if len(login.attach_db_file) > 260:
-            raise ValueError('File path should be not longer than 260 characters')
-        w = self._writer
-        w.begin_packet(tds_base.TDS7_LOGIN)
-        self.authentication = None
-        current_pos = 86 + 8 if tds_base.IS_TDS72_PLUS(self) else 86
-        client_host_name = login.client_host_name
-        login.client_host_name = client_host_name
-        packet_size = current_pos + (len(client_host_name) + len(login.app_name) + len(login.server_name) +
-                                     len(login.library) + len(login.language) + len(login.database)) * 2
-        if login.auth:
-            self.authentication = login.auth
-            auth_packet = login.auth.create_packet()
-            packet_size += len(auth_packet)
-        else:
-            auth_packet = ''
-            packet_size += (len(user_name) + len(login.password)) * 2
-        w.put_int(packet_size)
-        w.put_uint(login.tds_version)
-        w.put_int(w.bufsize)
-        from . import intversion
-        w.put_uint(intversion)
-        w.put_int(login.pid)
-        w.put_uint(0)  # connection id
-        option_flag1 = tds_base.TDS_SET_LANG_ON | tds_base.TDS_USE_DB_NOTIFY | tds_base.TDS_INIT_DB_FATAL
-        if not login.bulk_copy:
-            option_flag1 |= tds_base.TDS_DUMPLOAD_OFF
-        w.put_byte(option_flag1)
-        if self.authentication:
-            option_flag2 |= tds_base.TDS_INTEGRATED_SECURITY_ON
-        w.put_byte(option_flag2)
-        type_flags = 0
-        if login.readonly:
-            type_flags |= (2 << 5)
-        w.put_byte(type_flags)
-        option_flag3 = tds_base.TDS_UNKNOWN_COLLATION_HANDLING
-        w.put_byte(option_flag3 if tds_base.IS_TDS73_PLUS(self) else 0)
-        mins_fix = int(login.client_tz.utcoffset(datetime.datetime.now()).total_seconds()) // 60
-        w.put_int(mins_fix)
-        w.put_int(login.client_lcid)
-        w.put_smallint(current_pos)
-        w.put_smallint(len(client_host_name))
-        current_pos += len(client_host_name) * 2
-        if self.authentication:
-            w.put_smallint(0)
-            w.put_smallint(0)
-            w.put_smallint(0)
-            w.put_smallint(0)
-        else:
-            w.put_smallint(current_pos)
-            w.put_smallint(len(user_name))
-            current_pos += len(user_name) * 2
-            w.put_smallint(current_pos)
-            w.put_smallint(len(login.password))
-            current_pos += len(login.password) * 2
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.app_name))
-        current_pos += len(login.app_name) * 2
-        # server name
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.server_name))
-        current_pos += len(login.server_name) * 2
-        # reserved
-        w.put_smallint(0)
-        w.put_smallint(0)
-        # library name
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.library))
-        current_pos += len(login.library) * 2
-        # language
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.language))
-        current_pos += len(login.language) * 2
-        # database name
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.database))
-        current_pos += len(login.database) * 2
-        # ClientID
-        client_id = struct.pack('>Q', login.client_id)[2:]
-        w.write(client_id)
-        # authentication
-        w.put_smallint(current_pos)
-        w.put_smallint(len(auth_packet))
-        current_pos += len(auth_packet)
-        # db file
-        w.put_smallint(current_pos)
-        w.put_smallint(len(login.attach_db_file))
-        current_pos += len(login.attach_db_file) * 2
-        if tds_base.IS_TDS72_PLUS(self):
-            # new password
-            w.put_smallint(current_pos)
-            w.put_smallint(len(login.change_password))
-            # sspi long
-            w.put_int(0)
-        w.write_ucs2(client_host_name)
-        if not self.authentication:
-            w.write_ucs2(user_name)
-            w.write(tds7_crypt_pass(login.password))
-        w.write_ucs2(login.app_name)
-        w.write_ucs2(login.server_name)
-        w.write_ucs2(login.library)
-        w.write_ucs2(login.language)
-        w.write_ucs2(login.database)
-        if self.authentication:
-            w.write(auth_packet)
-        w.write_ucs2(login.attach_db_file)
-        w.write_ucs2(login.change_password)
-        w.flush()
-
-    _SERVER_TO_CLIENT_MAPPING = {
-        0x07000000: tds_base.TDS70,
-        0x07010000: tds_base.TDS71,
-        0x71000001: tds_base.TDS71rev1,
-        tds_base.TDS72: tds_base.TDS72,
-        tds_base.TDS73A: tds_base.TDS73A,
-        tds_base.TDS73B: tds_base.TDS73B,
-        tds_base.TDS74: tds_base.TDS74,
-        }
-
-    def process_login_tokens(self):
-        r = self._reader
-        succeed = False
-        while True:
-            marker = r.get_byte()
-            if marker == tds_base.TDS_LOGINACK_TOKEN:
-                succeed = True
-                size = r.get_smallint()
-                r.get_byte()  # interface
-                version = r.get_uint_be()
-                self.conn.tds_version = self._SERVER_TO_CLIENT_MAPPING.get(version, version)
-                if not tds_base.IS_TDS7_PLUS(self):
-                    self.bad_stream('Only TDS 7.0 and higher are supported')
-                # get server product name
-                # ignore product name length, some servers seem to set it incorrectly
-                r.get_byte()
-                size -= 10
-                self.conn.product_name = r.read_ucs2(size // 2)
-                product_version = r.get_uint_be()
-                # MSSQL 6.5 and 7.0 seem to return strange values for this
-                # using TDS 4.2, something like 5F 06 32 FF for 6.50
-                self.conn.product_version = product_version
-                if self.conn.authentication:
-                    self.conn.authentication.close()
-                    self.conn.authentication = None
-            else:
-                self.process_token(marker)
-                if marker == tds_base.TDS_DONE_TOKEN:
-                    break
-        return succeed
-
-    def process_returnstatus(self):
-        self.ret_status = self._reader.get_int()
-        self.has_status = True
-
-    def process_token(self, marker):
-        handler = _token_map.get(marker)
-        if not handler:
-            self.bad_stream('Invalid TDS marker: {0}({0:x})'.format(marker))
-        return handler(self)
-
-    def get_token_id(self):
-        self.set_state(tds_base.TDS_READING)
-        try:
-            marker = self._reader.get_byte()
-        except tds_base.TimeoutError:
-            self.set_state(tds_base.TDS_PENDING)
-            raise
-        except:
-            self._tds.close()
-            raise
-        return marker
-
-    def process_simple_request(self):
-        while True:
-            marker = self.get_token_id()
-            if marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
-                self.process_end(marker)
-                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS:
-                    # skip results that don't event have rowcount
-                    continue
-                return
-            else:
-                self.process_token(marker)
-
-    def next_set(self):
-        while self.more_rows:
-            self.next_row()
-        if self.state == tds_base.TDS_IDLE:
-            return False
-        if self.find_result_or_done():
-            return True
-
-    def fetchone(self):
-        if self.res_info is None:
-            raise tds_base.ProgrammingError("Previous statement didn't produce any results")
-
-        if self.skipped_to_status:
-            raise tds_base.ProgrammingError("Unable to fetch any rows after accessing return_status")
-
-        if not self.next_row():
-            return None
-
-        return self.row
-
-    def next_row(self):
-        if not self.more_rows:
-            return False
-        while True:
-            marker = self.get_token_id()
-            if marker in (tds_base.TDS_ROW_TOKEN, tds_base.TDS_NBC_ROW_TOKEN):
-                self.process_token(marker)
-                return True
-            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
-                self.process_end(marker)
-                return False
-            else:
-                self.process_token(marker)
-
-    def find_result_or_done(self):
-        self.done_flags = 0
-        while True:
-            marker = self.get_token_id()
-            if marker == tds_base.TDS7_RESULT_TOKEN:
-                self.process_token(marker)
-                return True
-            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
-                self.process_end(marker)
-                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS:
-                    if self.done_flags & tds_base.TDS_DONE_COUNT:
-                        return True
-                    else:
-                        # skip results without rowcount
-                        continue
-                else:
-                    return False
-            else:
-                self.process_token(marker)
-
-    def process_rpc(self):
-        self.done_flags = 0
-        self.return_value_index = 0
-        while True:
-            marker = self.get_token_id()
-            if marker == tds_base.TDS7_RESULT_TOKEN:
-                self.process_token(marker)
-                return True
-            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN):
-                self.process_end(marker)
-                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS and not self.done_flags & tds_base.TDS_DONE_COUNT:
-                    # skip results that don't event have rowcount
-                    continue
-                return False
-            else:
-                self.process_token(marker)
-
-    def find_return_status(self):
-        self.skipped_to_status = True
-        while True:
-            marker = self.get_token_id()
-            self.process_token(marker)
-            if marker == tds_base.TDS_RETURNSTATUS_TOKEN:
-                return
-
-
-_token_map = {
-    tds_base.TDS_AUTH_TOKEN: _TdsSession.process_auth,
-    tds_base.TDS_ENVCHANGE_TOKEN: _TdsSession.process_env_chg,
-    tds_base.TDS_DONE_TOKEN: lambda self: self.process_end(tds_base.TDS_DONE_TOKEN),
-    tds_base.TDS_DONEPROC_TOKEN: lambda self: self.process_end(tds_base.TDS_DONEPROC_TOKEN),
-    tds_base.TDS_DONEINPROC_TOKEN: lambda self: self.process_end(tds_base.TDS_DONEINPROC_TOKEN),
-    tds_base.TDS_ERROR_TOKEN: lambda self: self.process_msg(tds_base.TDS_ERROR_TOKEN),
-    tds_base.TDS_INFO_TOKEN: lambda self: self.process_msg(tds_base.TDS_INFO_TOKEN),
-    tds_base.TDS_EED_TOKEN: lambda self: self.process_msg(tds_base.TDS_EED_TOKEN),
-    tds_base.TDS_CAPABILITY_TOKEN: lambda self: self.process_msg(tds_base.TDS_CAPABILITY_TOKEN),
-    tds_base.TDS_PARAM_TOKEN: lambda self: self.process_param(),
-    tds_base.TDS7_RESULT_TOKEN: lambda self: self.tds7_process_result(),
-    tds_base.TDS_ROW_TOKEN: lambda self: self.process_row(),
-    tds_base.TDS_NBC_ROW_TOKEN: lambda self: self.process_nbcrow(),
-    tds_base.TDS_ORDERBY2_TOKEN: lambda self: self.process_orderby2(),
-    tds_base.TDS_ORDERBY_TOKEN: lambda self: self.process_orderby(),
-    tds_base.TDS_RETURNSTATUS_TOKEN: lambda self: self.process_returnstatus(),
-    }
-
-
-class _TdsSocket(object):
-    def __init__(self, use_tz=None):
-        self._is_connected = False
-        self.env = _TdsEnv()
-        self.collation = None
-        self.tds72_transaction = 0
-        self.authentication = None
-        self._mars_enabled = False
-        self.chunk_handler = MemoryChunkedHandler()
-        self.sock = None
-        self.bufsize = 4096
-        self.tds_version = tds_base.TDS74
-        self.use_tz = use_tz
-        self.type_factory = tds_types.SerializerFactory(self.tds_version)
-        self.type_inferrer = None
-        self.query_timeout = 0
-        self._smp_manager = None
-        self._main_session = None
-        self._login = None
-
-    def __repr__(self):
-        fmt = "<_TdsSocket tran={} mars={} tds_version={} use_tz={}>"
-        return fmt.format(self.tds72_transaction, self._mars_enabled,
-                          self.tds_version, self.use_tz)
-
-    def login(self, login, sock, tzinfo_factory):
-        self._login = login
-        self.bufsize = login.blocksize
-        self.query_timeout = login.query_timeout
-        self._main_session = _TdsSession(self, self, tzinfo_factory)
-        self.sock = sock
-        self.tds_version = login.tds_version
-        login.server_enc_flag = PreLoginEnc.ENCRYPT_NOT_SUP
-        if tds_base.IS_TDS71_PLUS(self):
-            self._main_session.send_prelogin(login)
-            self._main_session.process_prelogin(login)
-        if tds_base.IS_TDS7_PLUS(self):
-            self._main_session.tds7_send_login(login)
-        else:
-            raise ValueError('This TDS version is not supported')
-        if login.server_enc_flag == PreLoginEnc.ENCRYPT_OFF:
-            tls.revert_to_clear(self._main_session)
-        if not self._main_session.process_login_tokens():
-            self._main_session.raise_db_exception()
-        self.type_factory = tds_types.SerializerFactory(self.tds_version)
-        self.type_inferrer = tds_types.TdsTypeInferrer(
-            type_factory=self.type_factory,
-            collation=self.collation,
-            bytes_to_unicode=self._login.bytes_to_unicode,
-            allow_tz=not self.use_tz
-        )
-        text_size = login.text_size
-        if self._mars_enabled:
-            from .smp import SmpManager
-            self._smp_manager = SmpManager(self)
-            self._main_session = _TdsSession(
-                self,
-                self._smp_manager.create_session(),
-                tzinfo_factory)
-        self._is_connected = True
-        q = []
-        if text_size:
-            q.append('set textsize {0}'.format(int(text_size)))
-        if login.database and self.env.database != login.database:
-            q.append('use ' + tds_base.tds_quote_id(login.database))
-        if q:
-            self._main_session.submit_plain_query(''.join(q))
-            self._main_session.process_simple_request()
-
-    @property
-    def mars_enabled(self):
-        return self._mars_enabled
-
-    @property
-    def main_session(self):
-        return self._main_session
-
-    def create_session(self, tzinfo_factory):
-        return _TdsSession(
-            self, self._smp_manager.create_session(),
-            tzinfo_factory)
-
-    def read(self, size):
-        buf = self.sock.recv(size)
-        if len(buf) == 0:
-            self.close()
-            raise tds_base.ClosedConnectionError()
-        return buf
-
-    def _write(self, data, final):
-        try:
-            flags = 0
-            if hasattr(socket, 'MSG_NOSIGNAL'):
-                flags |= socket.MSG_NOSIGNAL
-            if not final:
-                if hasattr(socket, 'MSG_MORE'):
-                    flags |= socket.MSG_MORE
-            self.sock.sendall(data, flags)
-        except:
-            self.close()
-            raise
-
-    send = _write
-
-    def is_connected(self):
-        return self._is_connected
-
-    def close(self):
-        self._is_connected = False
-        if self.sock is not None:
-            self.sock.close()
-        if self._smp_manager:
-            self._smp_manager.transport_closed()
-        self._main_session.state = tds_base.TDS_DEAD
-        if self.authentication:
-            self.authentication.close()
-            self.authentication = None
-
-
-class _Results(object):
-    def __init__(self):
-            self.columns = []
-            self.row_count = 0
-
-
-def _parse_instances(msg):
-    name = None
-    if len(msg) > 3 and tds_base.my_ord(msg[0]) == 5:
-        tokens = msg[3:].decode('ascii').split(';')
-        results = {}
-        instdict = {}
-        got_name = False
-        for token in tokens:
-            if got_name:
-                instdict[name] = token
-                got_name = False
-            else:
-                name = token
-                if not name:
-                    if not instdict:
-                        break
-                    results[instdict['InstanceName'].upper()] = instdict
-                    instdict = {}
-                    continue
-                got_name = True
-        return results
-
-
-#
-# Get port of all instances
-# @return default port number or 0 if error
-# @remark experimental, cf. MC-SQLR.pdf.
-#
-def tds7_get_instances(ip_addr, timeout=5):
-    s = socket.socket(type=socket.SOCK_DGRAM)
-    s.settimeout(timeout)
-    try:
-        # send the request
-        s.sendto(b'\x03', (ip_addr, 1434))
-        msg = s.recv(16 * 1024 - 1)
-        # got data, read and parse
-        return _parse_instances(msg)
-    finally:
-        s.close()
+import codecs
+import contextlib
+import logging
+import datetime
+import six
+import socket
+import struct
+
+from .collate import ucs2_codec, Collation, lcid2charset, raw_collation
+from . import tds_base
+from . import tds_types
+from . import tls
+from .tds_base import readall, readall_fast, skipall, PreLoginEnc
+
+logger = logging.getLogger()
+
+# packet header
+# https://msdn.microsoft.com/en-us/library/dd340948.aspx
+_header = struct.Struct('>BBHHBx')
+
+_byte = struct.Struct('B')
+_smallint_le = struct.Struct('<h')
+_smallint_be = struct.Struct('>h')
+_usmallint_le = struct.Struct('<H')
+_usmallint_be = struct.Struct('>H')
+_int_le = struct.Struct('<l')
+_int_be = struct.Struct('>l')
+_uint_le = struct.Struct('<L')
+_uint_be = struct.Struct('>L')
+_int8_le = struct.Struct('<q')
+_int8_be = struct.Struct('>q')
+_uint8_le = struct.Struct('<Q')
+_uint8_be = struct.Struct('>Q')
+
+
+class SimpleLoadBalancer(object):
+    def __init__(self, hosts):
+        self._hosts = hosts
+
+    def choose(self):
+        for host in self._hosts:
+            yield host
+
+
+# stored procedure output parameter
+class output(object):
+    @property
+    def type(self):
+        """
+        This is either the sql type declaration or python type instance
+        of the parameter.
+        """
+        return self._type
+
+    @property
+    def value(self):
+        """
+        This is the value of the parameter.
+        """
+        return self._value
+
+    def __init__(self, value=None, param_type=None):
+        """ Creates procedure output parameter.
+
+        :param param_type: either sql type declaration or python type
+        :param value: value to pass into procedure
+        """
+        if param_type is None:
+            if value is None or value is default:
+                raise ValueError('Output type cannot be autodetected')
+        elif isinstance(param_type, type) and value is not None:
+            if value is not default and not isinstance(value, param_type):
+                raise ValueError('value should match param_type', value, param_type)
+        self._type = param_type
+        self._value = value
+
+
+class _Default(object):
+    pass
+
+default = _Default()
+
+
+def tds7_crypt_pass(password):
+    """ Mangle password according to tds rules
+
+    :param password: Password str
+    :returns: Byte-string with encoded password
+    """
+    encoded = bytearray(ucs2_codec.encode(password)[0])
+    for i, ch in enumerate(encoded):
+        encoded[i] = ((ch << 4) & 0xff | (ch >> 4)) ^ 0xA5
+    return encoded
+
+
+class _TdsEnv:
+    def __init__(self):
+        self.database = None
+        self.language = None
+        self.charset = None
+
+
+class _TdsReader(object):
+    """ TDS stream reader
+
+    Provides stream-like interface for TDS packeted stream.
+    Also provides convinience methods to decode primitive data like
+    different kinds of integers etc.
+    """
+    def __init__(self, session):
+        self._buf = ''
+        self._pos = 0  # position in the buffer
+        self._have = 0  # number of bytes read from packet
+        self._size = 0  # size of current packet
+        self._session = session
+        self._transport = session._transport
+        self._type = None
+        self._status = None
+
+    @property
+    def session(self):
+        """ Link to :class:`_TdsSession` object
+        """
+        return self._session
+
+    @property
+    def packet_type(self):
+        """ Type of current packet
+
+        Possible values are TDS_QUERY, TDS_LOGIN, etc.
+        """
+        return self._type
+
+    def read_fast(self, size):
+        """ Faster version of read
+
+        Instead of returning sliced buffer it returns reference to internal
+        buffer and the offset to this buffer.
+
+        :param size: Number of bytes to read
+        :returns: Tuple of bytes buffer, and offset in this buffer
+        """
+        if self._pos >= len(self._buf):
+            if self._have >= self._size:
+                self._read_packet()
+            else:
+                self._buf = self._transport.read(self._size - self._have)
+                self._pos = 0
+                self._have += len(self._buf)
+        offset = self._pos
+        self._pos += size
+        return self._buf, offset
+
+    def unpack(self, struc):
+        """ Unpacks given structure from stream
+
+        :param struc: A struct.Struct instance
+        :returns: Result of unpacking
+        """
+        buf, offset = readall_fast(self, struc.size)
+        return struc.unpack_from(buf, offset)
+
+    def get_byte(self):
+        """ Reads one byte from stream """
+        return self.unpack(_byte)[0]
+
+    def get_smallint(self):
+        """ Reads 16bit signed integer from the stream """
+        return self.unpack(_smallint_le)[0]
+
+    def get_usmallint(self):
+        """ Reads 16bit unsigned integer from the stream """
+        return self.unpack(_usmallint_le)[0]
+
+    def get_int(self):
+        """ Reads 32bit signed integer from the stream """
+        return self.unpack(_int_le)[0]
+
+    def get_uint(self):
+        """ Reads 32bit unsigned integer from the stream """
+        return self.unpack(_uint_le)[0]
+
+    def get_uint_be(self):
+        """ Reads 32bit unsigned big-endian integer from the stream """
+        return self.unpack(_uint_be)[0]
+
+    def get_uint8(self):
+        """ Reads 64bit unsigned integer from the stream """
+        return self.unpack(_uint8_le)[0]
+
+    def get_int8(self):
+        """ Reads 64bit signed integer from the stream """
+        return self.unpack(_int8_le)[0]
+
+    def read_ucs2(self, num_chars):
+        """ Reads num_chars UCS2 string from the stream """
+        buf = readall(self, num_chars * 2)
+        return ucs2_codec.decode(buf)[0]
+
+    def read_str(self, size, codec):
+        """ Reads byte string from the stream and decodes it
+
+        :param size: Size of string in bytes
+        :param codec: Instance of codec to decode string
+        :returns: Unicode string
+        """
+        return codec.decode(readall(self, size))[0]
+
+    def get_collation(self):
+        """ Reads :class:`Collation` object from stream """
+        buf = readall(self, Collation.wire_size)
+        return Collation.unpack(buf)
+
+    def unget_byte(self):
+        """ Returns one last read byte to stream
+
+        Can only be called once per read byte.
+        """
+        # this is a one trick pony...don't call it twice
+        assert self._pos > 0
+        self._pos -= 1
+
+    def peek(self):
+        """ Returns next byte from stream without consuming it
+        """
+        res = self.get_byte()
+        self.unget_byte()
+        return res
+
+    def read(self, size):
+        """ Reads size bytes from buffer
+
+        May return fewer bytes than requested
+        :param size: Number of bytes to read
+        :returns: Bytes buffer, possibly shorter than requested,
+                  returns empty buffer in case of EOF
+        """
+        buf, offset = self.read_fast(size)
+        return buf[offset:offset + size]
+
+    def _read_packet(self):
+        """ Reads next TDS packet from the underlying transport
+
+        If timeout is happened during reading of packet's header will
+        cancel current request.
+        Can only be called when transport's read pointer is at the begining
+        of the packet.
+        """
+        try:
+            header = readall(self._transport, _header.size)
+        except tds_base.TimeoutError:
+            self._session.put_cancel()
+            raise
+        self._pos = 0
+        self._type, self._status, self._size, self._session._spid, _ = _header.unpack(header)
+        self._have = _header.size
+        assert self._size > self._have, 'Empty packet doesn make any sense'
+        self._buf = self._transport.read(self._size - self._have)
+        self._have += len(self._buf)
+
+    def read_whole_packet(self):
+        """ Reads single packet and returns bytes payload of the packet
+
+        Can only be called when transport's read pointer is at the beginning
+        of the packet.
+        """
+        self._read_packet()
+        return readall(self, self._size - _header.size)
+
+
+class _TdsWriter(object):
+    """ TDS stream writer
+
+    Handles splitting of incoming data into TDS packets according to TDS protocol.
+    Provides convinience methods for writing primitive data types.
+    """
+    def __init__(self, session, bufsize):
+        self._session = session
+        self._tds = session
+        self._transport = session
+        self._pos = 0
+        self._buf = bytearray(bufsize)
+        self._packet_no = 0
+        self._type = 0
+
+    @property
+    def session(self):
+        """ Back reference to parent :class:`_TdsSession` object """
+        return self._session
+
+    @property
+    def bufsize(self):
+        """ Size of the buffer """
+        return len(self._buf)
+
+    @bufsize.setter
+    def bufsize(self, bufsize):
+        if len(self._buf) == bufsize:
+            return
+
+        if bufsize > len(self._buf):
+            self._buf.extend(b'\0' * (bufsize - len(self._buf)))
+        else:
+            self._buf = self._buf[0:bufsize]
+
+    def begin_packet(self, packet_type):
+        """ Starts new packet stream
+
+        :param packet_type: Type of TDS stream, e.g. TDS_PRELOGIN, TDS_QUERY etc.
+        """
+        self._type = packet_type
+        self._pos = 8
+
+    def pack(self, struc, *args):
+        """ Packs and writes structure into stream """
+        self.write(struc.pack(*args))
+
+    def put_byte(self, value):
+        """ Writes single byte into stream """
+        self.pack(_byte, value)
+
+    def put_smallint(self, value):
+        """ Writes 16-bit signed integer into the stream """
+        self.pack(_smallint_le, value)
+
+    def put_usmallint(self, value):
+        """ Writes 16-bit unsigned integer into the stream """
+        self.pack(_usmallint_le, value)
+
+    def put_smallint_be(self, value):
+        """ Writes 16-bit signed big-endian integer into the stream """
+        self.pack(_smallint_be, value)
+
+    def put_usmallint_be(self, value):
+        """ Writes 16-bit unsigned big-endian integer into the stream """
+        self.pack(_usmallint_be, value)
+
+    def put_int(self, value):
+        """ Writes 32-bit signed integer into the stream """
+        self.pack(_int_le, value)
+
+    def put_uint(self, value):
+        """ Writes 32-bit unsigned integer into the stream """
+        self.pack(_uint_le, value)
+
+    def put_int_be(self, value):
+        """ Writes 32-bit signed big-endian integer into the stream """
+        self.pack(_int_be, value)
+
+    def put_uint_be(self, value):
+        """ Writes 32-bit unsigned big-endian integer into the stream """
+        self.pack(_uint_be, value)
+
+    def put_int8(self, value):
+        """ Writes 64-bit signed integer into the stream """
+        self.pack(_int8_le, value)
+
+    def put_uint8(self, value):
+        """ Writes 64-bit unsigned integer into the stream """
+        self.pack(_uint8_le, value)
+
+    def put_collation(self, collation):
+        """ Writes :class:`Collation` structure into the stream """
+        self.write(collation.pack())
+
+    def write(self, data):
+        """ Writes given bytes buffer into the stream
+
+        Function returns only when entire buffer is written
+        """
+        data_off = 0
+        while data_off < len(data):
+            left = len(self._buf) - self._pos
+            if left <= 0:
+                self._write_packet(final=False)
+            else:
+                to_write = min(left, len(data) - data_off)
+                self._buf[self._pos:self._pos + to_write] = data[data_off:data_off + to_write]
+                self._pos += to_write
+                data_off += to_write
+
+    def write_b_varchar(self, s):
+        self.put_byte(len(s))
+        self.write_ucs2(s)
+
+    def write_ucs2(self, s):
+        """ Write string encoding it in UCS2 into stream """
+        self.write_string(s, ucs2_codec)
+
+    def write_string(self, s, codec):
+        """ Write string encoding it with codec into stream """
+        for i in range(0, len(s), self.bufsize):
+            chunk = s[i:i + self.bufsize]
+            buf, consumed = codec.encode(chunk)
+            assert consumed == len(chunk)
+            self.write(buf)
+
+    def flush(self):
+        """ Closes current packet stream """
+        return self._write_packet(final=True)
+
+    def _write_packet(self, final):
+        """ Writes single TDS packet into underlying transport.
+
+        Data for the packet is taken from internal buffer.
+
+        :param final: True means this is the final packet in substream.
+        """
+        status = 1 if final else 0
+        _header.pack_into(self._buf, 0, self._type, status, self._pos, 0, self._packet_no)
+        self._packet_no = (self._packet_no + 1) % 256
+        self._transport.send(self._buf[:self._pos], final)
+        self._pos = 8
+
+
+class MemoryChunkedHandler(object):
+    def __init__(self):
+        self.size = 0
+        self._chunks = []
+        self._column = None
+
+    def begin(self, column, size):
+        self.size = size
+        self._chunks = []
+        self._column = column
+
+    def new_chunk(self, val):
+        self._chunks.append(val)
+
+    def end(self):
+        return b''.join(self._chunks)
+
+
+class MemoryStrChunkedHandler(object):
+    def __init__(self):
+        self.size = 0
+        self._chunks = []
+        self._column = None
+
+    def begin(self, column, size):
+        self.size = size
+        self._chunks = []
+        self._column = column
+
+    def new_chunk(self, val):
+        self._chunks.append(val)
+
+    def end(self):
+        return ''.join(self._chunks)
+
+
+def _create_exception_by_message(msg, custom_error_msg=None):
+    msg_no = msg['msgno']
+    if custom_error_msg is not None:
+        error_msg = custom_error_msg
+    else:
+        error_msg = msg['message']
+    if msg_no in tds_base.prog_errors:
+        ex = tds_base.ProgrammingError(error_msg)
+    elif msg_no in tds_base.integrity_errors:
+        ex = tds_base.IntegrityError(error_msg)
+    else:
+        ex = tds_base.OperationalError(error_msg)
+    ex.msg_no = msg['msgno']
+    ex.text = msg['message']
+    ex.srvname = msg['server']
+    ex.procname = msg['proc_name']
+    ex.number = msg['msgno']
+    ex.severity = msg['severity']
+    ex.state = msg['state']
+    ex.line = msg['line_number']
+    return ex
+
+
+class _TdsSession(object):
+    """ TDS session
+
+    Represents a single TDS session within MARS connection, when MARS enabled there could be multiple TDS sessions
+    within one connection.
+    """
+    def __init__(self, tds, transport, tzinfo_factory):
+        self.out_pos = 8
+        self.res_info = None
+        self.in_cancel = False
+        self.wire_mtx = None
+        self.param_info = None
+        self.has_status = False
+        self.ret_status = None
+        self.skipped_to_status = False
+        self._transport = transport
+        self._reader = _TdsReader(self)
+        self._reader._transport = transport
+        self._writer = _TdsWriter(self, tds.bufsize)
+        self._writer._transport = transport
+        self.in_buf_max = 0
+        self.state = tds_base.TDS_IDLE
+        self._tds = tds
+        self.messages = []
+        self.chunk_handler = tds.chunk_handler
+        self.rows_affected = -1
+        self.use_tz = tds.use_tz
+        self._spid = 0
+        self.tzinfo_factory = tzinfo_factory
+        self.more_rows = False
+        self.done_flags = 0
+        self.internal_sp_called = 0
+        self.output_params = {}
+        self.authentication = None
+        self.return_value_index = 0
+        self._out_params_indexes = []
+        self.row = None
+        self.end_marker = 0
+
+    def __repr__(self):
+        fmt = "<_TdsSession state={} tds={} messages={} rows_affected={} use_tz={} spid={} in_cancel={}>"
+        res = fmt.format(repr(self.state), repr(self._tds), repr(self.messages),
+                         repr(self.rows_affected), repr(self.use_tz), repr(self._spid),
+                         self.in_cancel)
+        return res
+
+    def raise_db_exception(self):
+        """ Raises exception from last server message
+
+        This function will skip messages: The statement has been terminated
+        """
+        if not self.messages:
+            raise tds_base.Error("Request failed, server didn't send error message")
+        msg = None
+        while True:
+            msg = self.messages[-1]
+            if msg['msgno'] == 3621:  # the statement has been terminated
+                self.messages = self.messages[:-1]
+            else:
+                break
+
+        error_msg = ' '.join(m['message'] for m in self.messages)
+        ex = _create_exception_by_message(msg, error_msg)
+        raise ex
+
+    def get_type_info(self, curcol):
+        """ Reads TYPE_INFO structure (http://msdn.microsoft.com/en-us/library/dd358284.aspx)
+
+        :param curcol: An instance of :class:`Column` that will receive read information
+        """
+        r = self._reader
+        # User defined data type of the column
+        curcol.column_usertype = r.get_uint() if tds_base.IS_TDS72_PLUS(self) else r.get_usmallint()
+        curcol.flags = r.get_usmallint()  # Flags
+        type_id = r.get_byte()
+        serializer_class = self._tds.type_factory.get_type_serializer(type_id)
+        curcol.serializer = serializer_class.from_stream(r)
+
+    def tds7_process_result(self):
+        """ Reads and processes COLMETADATA stream
+
+        This stream contains a list of returned columns.
+        Stream format link: http://msdn.microsoft.com/en-us/library/dd357363.aspx
+        """
+        r = self._reader
+
+        # read number of columns and allocate the columns structure
+
+        num_cols = r.get_smallint()
+
+        # This can be a DUMMY results token from a cursor fetch
+
+        if num_cols == -1:
+            return
+
+        self.param_info = None
+        self.has_status = False
+        self.ret_status = None
+        self.skipped_to_status = False
+        self.rows_affected = tds_base.TDS_NO_COUNT
+        self.more_rows = True
+        self.row = [None] * num_cols
+        self.res_info = info = _Results()
+
+        #
+        # loop through the columns populating COLINFO struct from
+        # server response
+        #
+        header_tuple = []
+        for col in range(num_cols):
+            curcol = tds_base.Column()
+            info.columns.append(curcol)
+            self.get_type_info(curcol)
+
+            curcol.column_name = r.read_ucs2(r.get_byte())
+            precision = curcol.serializer.precision
+            scale = curcol.serializer.scale
+            size = curcol.serializer.size
+            header_tuple.append(
+                (curcol.column_name,
+                 curcol.serializer.get_typeid(),
+                 None,
+                 size,
+                 precision,
+                 scale,
+                 curcol.flags & tds_base.Column.fNullable))
+        info.description = tuple(header_tuple)
+        return info
+
+    def process_param(self):
+        """ Reads and processes RETURNVALUE stream.
+
+        This stream is used to send OUTPUT parameters from RPC to client.
+        Stream format url: http://msdn.microsoft.com/en-us/library/dd303881.aspx
+        """
+        r = self._reader
+        if tds_base.IS_TDS72_PLUS(self):
+            ordinal = r.get_usmallint()
+        else:
+            r.get_usmallint()  # ignore size
+            ordinal = self._out_params_indexes[self.return_value_index]
+        name = r.read_ucs2(r.get_byte())
+        r.get_byte()  # 1 - OUTPUT of sp, 2 - result of udf
+        param = tds_base.Column()
+        param.column_name = name
+        self.get_type_info(param)
+        param.value = param.serializer.read(r)
+        self.output_params[ordinal] = param
+        self.return_value_index += 1
+
+    def process_cancel(self):
+        """
+        Process the incoming token stream until it finds
+        an end token DONE with the cancel flag set.
+        At that point the connection should be ready to handle a new query.
+
+        In case when no cancel request is pending this function does nothing.
+        """
+        # silly cases, nothing to do
+        if not self.in_cancel:
+            return
+
+        while True:
+            token_id = self.get_token_id()
+            self.process_token(token_id)
+            if not self.in_cancel:
+                return
+
+    def process_msg(self, marker):
+        """ Reads and processes ERROR/INFO streams
+
+        Stream formats:
+
+        - ERROR: http://msdn.microsoft.com/en-us/library/dd304156.aspx
+        - INFO: http://msdn.microsoft.com/en-us/library/dd303398.aspx
+
+        :param marker: TDS_ERROR_TOKEN or TDS_INFO_TOKEN
+        """
+        r = self._reader
+        r.get_smallint()  # size
+        msg = {'marker': marker, 'msgno': r.get_int(), 'state': r.get_byte(), 'severity': r.get_byte(),
+               'sql_state': None}
+        has_eed = False
+        if marker == tds_base.TDS_EED_TOKEN:
+            if msg['severity'] <= 10:
+                msg['priv_msg_type'] = 0
+            else:
+                msg['priv_msg_type'] = 1
+            len_sqlstate = r.get_byte()
+            msg['sql_state'] = readall(r, len_sqlstate)
+            has_eed = r.get_byte()
+            # junk status and transaction state
+            r.get_smallint()
+        elif marker == tds_base.TDS_INFO_TOKEN:
+            msg['priv_msg_type'] = 0
+        elif marker == tds_base.TDS_ERROR_TOKEN:
+            msg['priv_msg_type'] = 1
+        else:
+            logger.error('tds_process_msg() called with unknown marker "{0}"'.format(marker))
+        msg['message'] = r.read_ucs2(r.get_smallint())
+        # server name
+        msg['server'] = r.read_ucs2(r.get_byte())
+        # stored proc name if available
+        msg['proc_name'] = r.read_ucs2(r.get_byte())
+        msg['line_number'] = r.get_int() if tds_base.IS_TDS72_PLUS(self) else r.get_smallint()
+        # in case extended error data is sent, we just try to discard it
+        if has_eed:
+            while True:
+                next_marker = r.get_byte()
+                if next_marker in (tds_base.TDS5_PARAMFMT_TOKEN,
+                                   tds_base.TDS5_PARAMFMT2_TOKEN,
+                                   tds_base.TDS5_PARAMS_TOKEN):
+                    self.process_token(next_marker)
+                else:
+                    break
+            r.unget_byte()
+
+        # special case
+        self.messages.append(msg)
+
+    def process_row(self):
+        """ Reads and handles ROW stream.
+
+        This stream contains list of values of one returned row.
+        Stream format url: http://msdn.microsoft.com/en-us/library/dd357254.aspx
+        """
+        r = self._reader
+        info = self.res_info
+        info.row_count += 1
+        for i, curcol in enumerate(info.columns):
+            curcol.value = self.row[i] = curcol.serializer.read(r)
+
+    def process_nbcrow(self):
+        """ Reads and handles NBCROW stream.
+
+        This stream contains list of values of one returned row in a compressed way,
+        introduced in TDS 7.3.B
+        Stream format url: http://msdn.microsoft.com/en-us/library/dd304783.aspx
+        """
+        r = self._reader
+        info = self.res_info
+        if not info:
+            self.bad_stream('got row without info')
+        assert len(info.columns) > 0
+        info.row_count += 1
+
+        # reading bitarray for nulls, 1 represent null values for
+        # corresponding fields
+        nbc = readall(r, (len(info.columns) + 7) // 8)
+        for i, curcol in enumerate(info.columns):
+            if tds_base.my_ord(nbc[i // 8]) & (1 << (i % 8)):
+                value = None
+            else:
+                value = curcol.serializer.read(r)
+            self.row[i] = value
+
+    def process_orderby(self):
+        """ Reads and processes ORDER stream
+
+        Used to inform client by which column dataset is ordered.
+        Stream format url: http://msdn.microsoft.com/en-us/library/dd303317.aspx
+        """
+        r = self._reader
+        skipall(r, r.get_smallint())
+
+    def process_orderby2(self):
+        r = self._reader
+        skipall(r, r.get_int())
+
+    def process_end(self, marker):
+        """ Reads and processes DONE/DONEINPROC/DONEPROC streams
+
+        Stream format urls:
+
+        - DONE: http://msdn.microsoft.com/en-us/library/dd340421.aspx
+        - DONEINPROC: http://msdn.microsoft.com/en-us/library/dd340553.aspx
+        - DONEPROC: http://msdn.microsoft.com/en-us/library/dd340753.aspx
+
+        :param marker: Can be TDS_DONE_TOKEN or TDS_DONEINPROC_TOKEN or TDS_DONEPROC_TOKEN
+        """
+        self.end_marker = marker
+        self.more_rows = False
+        r = self._reader
+        status = r.get_usmallint()
+        r.get_usmallint()  # cur_cmd
+        more_results = status & tds_base.TDS_DONE_MORE_RESULTS != 0
+        was_cancelled = status & tds_base.TDS_DONE_CANCELLED != 0
+        done_count_valid = status & tds_base.TDS_DONE_COUNT != 0
+        if self.res_info:
+            self.res_info.more_results = more_results
+        rows_affected = r.get_int8() if tds_base.IS_TDS72_PLUS(self) else r.get_int()
+        if was_cancelled or (not more_results and not self.in_cancel):
+            self.in_cancel = False
+            self.set_state(tds_base.TDS_IDLE)
+        if done_count_valid:
+            self.rows_affected = rows_affected
+        else:
+            self.rows_affected = -1
+        self.done_flags = status
+        if self.done_flags & tds_base.TDS_DONE_ERROR and not was_cancelled and not self.in_cancel:
+            self.raise_db_exception()
+
+    def process_env_chg(self):
+        """ Reads and processes ENVCHANGE stream.
+
+        Stream info url: http://msdn.microsoft.com/en-us/library/dd303449.aspx
+        """
+        r = self._reader
+        size = r.get_smallint()
+        type_id = r.get_byte()
+        if type_id == tds_base.TDS_ENV_SQLCOLLATION:
+            size = r.get_byte()
+            self.conn.collation = r.get_collation()
+            skipall(r, size - 5)
+            # discard old one
+            skipall(r, r.get_byte())
+        elif type_id == tds_base.TDS_ENV_BEGINTRANS:
+            size = r.get_byte()
+            assert size == 8
+            self.conn.tds72_transaction = r.get_uint8()
+            skipall(r, r.get_byte())
+        elif type_id == tds_base.TDS_ENV_COMMITTRANS or type_id == tds_base.TDS_ENV_ROLLBACKTRANS:
+            self.conn.tds72_transaction = 0
+            skipall(r, r.get_byte())
+            skipall(r, r.get_byte())
+        elif type_id == tds_base.TDS_ENV_PACKSIZE:
+            newval = r.read_ucs2(r.get_byte())
+            r.read_ucs2(r.get_byte())
+            new_block_size = int(newval)
+            if new_block_size >= 512:
+                # Is possible to have a shrink if server limits packet
+                # size more than what we specified
+                #
+                # Reallocate buffer if possible (strange values from server or out of memory) use older buffer */
+                self._writer.bufsize = new_block_size
+        elif type_id == tds_base.TDS_ENV_DATABASE:
+            newval = r.read_ucs2(r.get_byte())
+            r.read_ucs2(r.get_byte())
+            self.conn.env.database = newval
+        elif type_id == tds_base.TDS_ENV_LANG:
+            newval = r.read_ucs2(r.get_byte())
+            r.read_ucs2(r.get_byte())
+            self.conn.env.language = newval
+        elif type_id == tds_base.TDS_ENV_CHARSET:
+            newval = r.read_ucs2(r.get_byte())
+            r.read_ucs2(r.get_byte())
+            self.conn.env.charset = newval
+            remap = {'iso_1': 'iso8859-1'}
+            self.conn.server_codec = codecs.lookup(remap.get(newval, newval))
+        elif type_id == tds_base.TDS_ENV_DB_MIRRORING_PARTNER:
+            r.read_ucs2(r.get_byte())
+            r.read_ucs2(r.get_byte())
+        elif type_id == tds_base.TDS_ENV_LCID:
+            lcid = int(r.read_ucs2(r.get_byte()))
+            self.conn.server_codec = codecs.lookup(lcid2charset(lcid))
+            r.read_ucs2(r.get_byte())
+        else:
+            logger.warning("unknown env type: {0}, skipping".format(type_id))
+            # discard byte values, not still supported
+            skipall(r, size - 1)
+
+    def process_auth(self):
+        """ Reads and processes SSPI stream.
+
+        Stream info: http://msdn.microsoft.com/en-us/library/dd302844.aspx
+        """
+        r = self._reader
+        w = self._writer
+        pdu_size = r.get_smallint()
+        if not self.authentication:
+            raise tds_base.Error('Got unexpected token')
+        packet = self.authentication.handle_next(readall(r, pdu_size))
+        if packet:
+            w.write(packet)
+            w.flush()
+
+    def is_connected(self):
+        """
+        :return: True if transport is connected
+        """
+        return self._transport.is_connected()
+
+    def bad_stream(self, msg):
+        """ Called when input stream contains unexpected data.
+
+        Will close stream and raise :class:`InterfaceError`
+        :param msg: Message for InterfaceError exception.
+        :return: Never returns, always raises exception.
+        """
+        self.close()
+        raise tds_base.InterfaceError(msg)
+
+    @property
+    def tds_version(self):
+        """ Returns integer encoded current TDS protocol version
+        """
+        return self._tds.tds_version
+
+    @property
+    def conn(self):
+        """ Reference to owning :class:`_TdsSocket`
+        """
+        return self._tds
+
+    def close(self):
+        self._transport.close()
+
+    def set_state(self, state):
+        """ Switches state of the TDS session.
+
+        It also does state transitions checks.
+        :param state: New state, one of TDS_PENDING/TDS_READING/TDS_IDLE/TDS_DEAD/TDS_QUERING
+        """
+        prior_state = self.state
+        if state == prior_state:
+            return state
+        if state == tds_base.TDS_PENDING:
+            if prior_state in (tds_base.TDS_READING, tds_base.TDS_QUERYING):
+                self.state = tds_base.TDS_PENDING
+            else:
+                raise tds_base.InterfaceError('logic error: cannot chage query state from {0} to {1}'.
+                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
+        elif state == tds_base.TDS_READING:
+            # transition to READING are valid only from PENDING
+            if self.state != tds_base.TDS_PENDING:
+                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
+                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
+            else:
+                self.state = state
+        elif state == tds_base.TDS_IDLE:
+            if prior_state == tds_base.TDS_DEAD:
+                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
+                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
+            self.state = state
+        elif state == tds_base.TDS_DEAD:
+            self.state = state
+        elif state == tds_base.TDS_QUERYING:
+            if self.state == tds_base.TDS_DEAD:
+                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
+                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
+            elif self.state != tds_base.TDS_IDLE:
+                raise tds_base.InterfaceError('logic error: cannot change query state from {0} to {1}'.
+                                              format(tds_base.state_names[prior_state], tds_base.state_names[state]))
+            else:
+                self.rows_affected = tds_base.TDS_NO_COUNT
+                self.internal_sp_called = 0
+                self.state = state
+        else:
+            assert False
+        return self.state
+
+    @contextlib.contextmanager
+    def querying_context(self, packet_type):
+        """ Context manager for querying.
+
+        Sets state to TDS_QUERYING, and reverts it to TDS_IDLE if exception happens inside managed block,
+        and to TDS_PENDING if managed block succeeds and flushes buffer.
+        """
+        if self.set_state(tds_base.TDS_QUERYING) != tds_base.TDS_QUERYING:
+            raise tds_base.Error("Couldn't switch to state")
+        self._writer.begin_packet(packet_type)
+        try:
+            yield
+        except:
+            if self.state != tds_base.TDS_DEAD:
+                self.set_state(tds_base.TDS_IDLE)
+            raise
+        else:
+            self.set_state(tds_base.TDS_PENDING)
+            self._writer.flush()
+
+    def make_param(self, name, value):
+        """ Generates instance of :class:`Column` from value and name
+
+        Value can also be of a special types:
+
+        - An instance of :class:`Column`, in which case it is just returned.
+        - An instance of :class:`output`, in which case parameter will become
+          an output parameter.
+        - A singleton :var:`default`, in which case default value will be passed
+          into a stored proc.
+
+        :param name: Name of the parameter, will populate column_name property of returned column.
+        :param value: Value of the parameter, also used to guess the type of parameter.
+        :return: An instance of :class:`Column`
+        """
+        if isinstance(value, tds_base.Column):
+            value.column_name = name
+            return value
+        column = tds_base.Column()
+        column.column_name = name
+        column.flags = 0
+        
+        if isinstance(value, output):
+            column.flags |= tds_base.fByRefValue
+            if isinstance(value.type, six.string_types):
+                column.type = tds_types.sql_type_by_declaration(value.type)
+            elif value.type:
+                column.type = self.conn.type_inferrer.from_class(value.type)
+            value = value.value
+
+        if value is default:
+            column.flags |= tds_base.fDefaultValue
+            value = None
+
+        column.value = value
+        if column.type is None:
+            column.type = self.conn.type_inferrer.from_value(value)
+        return column
+
+    def _convert_params(self, parameters):
+        """ Converts a dict of list of parameters into a list of :class:`Column` instances.
+
+        :param parameters: Can be a list of parameter values, or a dict of parameter names to values.
+        :return: A list of :class:`Column` instances.
+        """
+        if isinstance(parameters, dict):
+            return [self.make_param(name, value)
+                    for name, value in parameters.items()]
+        else:
+            params = []
+            for parameter in parameters:
+                params.append(self.make_param('', parameter))
+            return params
+
+    def cancel_if_pending(self):
+        """ Cancels current pending request.
+
+        Does nothing if no request is pending, otherwise sends cancel request,
+        and waits for response.
+        """
+        if self.state == tds_base.TDS_IDLE:
+            return
+        if not self.in_cancel:
+            self.put_cancel()
+        self.process_cancel()
+
+    def submit_rpc(self, rpc_name, params, flags):
+        """ Sends an RPC request.
+
+        This call will transition session into pending state.
+        If some operation is currently pending on the session, it will be
+        cancelled before sending this request.
+
+        Spec: http://msdn.microsoft.com/en-us/library/dd357576.aspx
+
+        :param rpc_name: Name of the RPC to call, can be an instance of :class:`InternalProc`
+        :param params: Stored proc parameters, should be a list of :class:`Column` instances.
+        :param flags: See spec for possible flags.
+        """
+        self.messages = []
+        self.output_params = {}
+        self.cancel_if_pending()
+        self.res_info = None
+        w = self._writer
+        with self.querying_context(tds_base.TDS_RPC):
+            if tds_base.IS_TDS72_PLUS(self):
+                self._start_query()
+            if tds_base.IS_TDS71_PLUS(self) and isinstance(rpc_name, tds_base.InternalProc):
+                w.put_smallint(-1)
+                w.put_smallint(rpc_name.proc_id)
+            else:
+                if isinstance(rpc_name, tds_base.InternalProc):
+                    rpc_name = rpc_name.name
+                w.put_smallint(len(rpc_name))
+                w.write_ucs2(rpc_name)
+            #
+            # TODO support flags
+            # bit 0 (1 as flag) in TDS7/TDS5 is "recompile"
+            # bit 1 (2 as flag) in TDS7+ is "no metadata" bit this will prevent sending of column infos
+            #
+            w.put_usmallint(flags)
+            self._out_params_indexes = []
+            for i, param in enumerate(params):
+                if param.flags & tds_base.fByRefValue:
+                    self._out_params_indexes.append(i)
+                w.put_byte(len(param.column_name))
+                w.write_ucs2(param.column_name)
+                #
+                # TODO support other flags (use defaul null/no metadata)
+                # bit 1 (2 as flag) in TDS7+ is "default value" bit
+                # (what's the meaning of "default value" ?)
+                #
+                w.put_byte(param.flags)
+
+                # TYPE_INFO structure: https://msdn.microsoft.com/en-us/library/dd358284.aspx
+                serializer = param.choose_serializer(
+                    type_factory=self._tds.type_factory,
+                    collation=self._tds.collation or raw_collation
+                )
+                type_id = serializer.type
+                w.put_byte(type_id)
+                serializer.write_info(w)
+
+                serializer.write(w, param.value)
+
+    def submit_plain_query(self, operation):
+        """ Sends a plain query to server.
+
+        This call will transition session into pending state.
+        If some operation is currently pending on the session, it will be
+        cancelled before sending this request.
+
+        Spec: http://msdn.microsoft.com/en-us/library/dd358575.aspx
+
+        :param operation: A string representing sql statement.
+        """
+        self.messages = []
+        self.cancel_if_pending()
+        self.res_info = None
+        w = self._writer
+        with self.querying_context(tds_base.TDS_QUERY):
+            if tds_base.IS_TDS72_PLUS(self):
+                self._start_query()
+            w.write_ucs2(operation)
+
+    def submit_bulk(self, metadata, rows):
+        """ Sends insert bulk command.
+
+        Spec: http://msdn.microsoft.com/en-us/library/dd358082.aspx
+
+        :param metadata: A list of :class:`Column` instances.
+        :param rows: A collection of rows, each row is a collection of values.
+        :return:
+        """
+        num_cols = len(metadata)
+        w = self._writer
+        serializers = []
+        with self.querying_context(tds_base.TDS_BULK):
+            w.put_byte(tds_base.TDS7_RESULT_TOKEN)
+            w.put_usmallint(num_cols)
+            for col in metadata:
+                if tds_base.IS_TDS72_PLUS(self):
+                    w.put_uint(col.column_usertype)
+                else:
+                    w.put_usmallint(col.column_usertype)
+                w.put_usmallint(col.flags)
+                serializer = col.choose_serializer(
+                    type_factory=self._tds.type_factory,
+                    collation=self._tds.collation,
+                )
+                type_id = serializer.type
+                w.put_byte(type_id)
+                serializers.append(serializer)
+                serializer.write_info(w)
+                w.put_byte(len(col.column_name))
+                w.write_ucs2(col.column_name)
+            for row in rows:
+                w.put_byte(tds_base.TDS_ROW_TOKEN)
+                for i, col in enumerate(metadata):
+                    serializers[i].write(w, row[i])
+
+            w.put_byte(tds_base.TDS_DONE_TOKEN)
+            w.put_usmallint(tds_base.TDS_DONE_FINAL)
+            w.put_usmallint(0)  # curcmd
+            if tds_base.IS_TDS72_PLUS(self):
+                w.put_int8(0)
+            else:
+                w.put_int(0)
+
+    def put_cancel(self):
+        """ Sends a cancel request to the server.
+
+        Switches connection to IN_CANCEL state.
+        """
+        self._writer.begin_packet(tds_base.TDS_CANCEL)
+        self._writer.flush()
+        self.in_cancel = 1
+
+    _begin_tran_struct_72 = struct.Struct('<HBB')
+
+    def begin_tran(self, isolation_level=0):
+        self.submit_begin_tran(isolation_level=isolation_level)
+        self.process_simple_request()
+
+    def submit_begin_tran(self, isolation_level=0):
+        if tds_base.IS_TDS72_PLUS(self):
+            self.messages = []
+            self.cancel_if_pending()
+            w = self._writer
+            with self.querying_context(tds_base.TDS7_TRANS):
+                self._start_query()
+                w.pack(
+                    self._begin_tran_struct_72,
+                    5,  # TM_BEGIN_XACT
+                    isolation_level,
+                    0,  # new transaction name
+                    )
+        else:
+            self.submit_plain_query("BEGIN TRANSACTION")
+            self.conn.tds72_transaction = 1
+
+    _commit_rollback_tran_struct72_hdr = struct.Struct('<HBB')
+    _continue_tran_struct72 = struct.Struct('<BB')
+
+    def rollback(self, cont, isolation_level=0):
+        self.submit_rollback(cont, isolation_level=isolation_level)
+        prev_timeout = self._tds.sock.gettimeout()
+        self._tds.sock.settimeout(None)
+        try:
+            self.process_simple_request()
+        finally:
+            self._tds.sock.settimeout(prev_timeout)
+
+    def submit_rollback(self, cont, isolation_level=0):
+        if tds_base.IS_TDS72_PLUS(self):
+            self.messages = []
+            self.cancel_if_pending()
+            w = self._writer
+            with self.querying_context(tds_base.TDS7_TRANS):
+                self._start_query()
+                flags = 0
+                if cont:
+                    flags |= 1
+                w.pack(
+                    self._commit_rollback_tran_struct72_hdr,
+                    8,  # TM_ROLLBACK_XACT
+                    0,  # transaction name
+                    flags,
+                    )
+                if cont:
+                    w.pack(
+                        self._continue_tran_struct72,
+                        isolation_level,
+                        0,  # new transaction name
+                        )
+        else:
+            self.submit_plain_query(
+                "IF @@TRANCOUNT > 0 ROLLBACK BEGIN TRANSACTION" if cont else "IF @@TRANCOUNT > 0 ROLLBACK")
+            self.conn.tds72_transaction = 1 if cont else 0
+
+    def commit(self, cont, isolation_level=0):
+        self.submit_commit(cont, isolation_level=isolation_level)
+        prev_timeout = self._tds.sock.gettimeout()
+        self._tds.sock.settimeout(None)
+        try:
+            self.process_simple_request()
+        finally:
+            self._tds.sock.settimeout(prev_timeout)
+
+    def submit_commit(self, cont, isolation_level=0):
+        if tds_base.IS_TDS72_PLUS(self):
+            self.messages = []
+            self.cancel_if_pending()
+            w = self._writer
+            with self.querying_context(tds_base.TDS7_TRANS):
+                self._start_query()
+                flags = 0
+                if cont:
+                    flags |= 1
+                w.pack(
+                    self._commit_rollback_tran_struct72_hdr,
+                    7,  # TM_COMMIT_XACT
+                    0,  # transaction name
+                    flags,
+                    )
+                if cont:
+                    w.pack(
+                        self._continue_tran_struct72,
+                        isolation_level,
+                        0,  # new transaction name
+                        )
+        else:
+            self.submit_plain_query(
+                "IF @@TRANCOUNT > 0 COMMIT BEGIN TRANSACTION" if cont else "IF @@TRANCOUNT > 0 COMMIT")
+            self.conn.tds72_transaction = 1 if cont else 0
+
+    _tds72_query_start = struct.Struct('<IIHQI')
+
+    def _start_query(self):
+        w = self._writer
+        w.pack(_TdsSession._tds72_query_start,
+               0x16,  # total length
+               0x12,  # length
+               2,  # type
+               self.conn.tds72_transaction,
+               1,  # request count
+               )
+
+    VERSION = 0
+    ENCRYPTION = 1
+    INSTOPT = 2
+    THREADID = 3
+    MARS = 4
+    TRACEID = 5
+    TERMINATOR = 0xff
+
+    def send_prelogin(self, login):
+        # https://msdn.microsoft.com/en-us/library/dd357559.aspx
+        instance_name = login.instance_name or 'MSSQLServer'
+        instance_name = instance_name.encode('ascii')
+        if len(instance_name) > 65490:
+            raise ValueError('Instance name is too long')
+        if tds_base.IS_TDS72_PLUS(self):
+            start_pos = 26
+            buf = struct.pack(
+                b'>BHHBHHBHHBHHBHHB',
+                # netlib version
+                self.VERSION, start_pos, 6,
+                # encryption
+                self.ENCRYPTION, start_pos + 6, 1,
+                # instance
+                self.INSTOPT, start_pos + 6 + 1, len(instance_name) + 1,
+                # thread id
+                self.THREADID, start_pos + 6 + 1 + len(instance_name) + 1, 4,
+                # MARS enabled
+                self.MARS, start_pos + 6 + 1 + len(instance_name) + 1 + 4, 1,
+                # end
+                self.TERMINATOR
+                )
+        else:
+            start_pos = 21
+            buf = struct.pack(
+                b'>BHHBHHBHHBHHB',
+                # netlib version
+                self.VERSION, start_pos, 6,
+                # encryption
+                self.ENCRYPTION, start_pos + 6, 1,
+                # instance
+                self.INSTOPT, start_pos + 6 + 1, len(instance_name) + 1,
+                # thread id
+                self.THREADID, start_pos + 6 + 1 + len(instance_name) + 1, 4,
+                # end
+                self.TERMINATOR
+                )
+        assert start_pos == len(buf)
+        w = self._writer
+        w.begin_packet(tds_base.TDS71_PRELOGIN)
+        w.write(buf)
+        from . import intversion
+        w.put_uint_be(intversion)
+        w.put_usmallint_be(0)  # build number
+        # encryption flag
+        w.put_byte(login.enc_flag)
+        w.write(instance_name)
+        w.put_byte(0)  # zero terminate instance_name
+        w.put_int(0)  # TODO: change this to thread id
+        if tds_base.IS_TDS72_PLUS(self):
+            # MARS (1 enabled)
+            w.put_byte(1 if login.use_mars else 0)
+        w.flush()
+
+    def process_prelogin(self, login):
+        # https://msdn.microsoft.com/en-us/library/dd357559.aspx
+        p = self._reader.read_whole_packet()
+        size = len(p)
+        if size <= 0 or self._reader.packet_type != 4:
+            self.bad_stream('Invalid packet type: {0}, expected PRELOGIN(4)'.format(self._reader.packet_type))
+        # default 2, no certificate, no encryptption
+        crypt_flag = 2
+        i = 0
+        byte_struct = struct.Struct('B')
+        off_len_struct = struct.Struct('>HH')
+        prod_version_struct = struct.Struct('>LH')
+        while True:
+            if i >= size:
+                self.bad_stream('Invalid size of PRELOGIN structure')
+            type_id, = byte_struct.unpack_from(p, i)
+            if type_id == 0xff:
+                break
+            if i + 4 > size:
+                self.bad_stream('Invalid size of PRELOGIN structure')
+            off, l = off_len_struct.unpack_from(p, i + 1)
+            if off > size or off + l > size:
+                self.bad_stream('Invalid offset in PRELOGIN structure')
+            if type_id == self.VERSION:
+                self.conn.server_library_version = prod_version_struct.unpack_from(p, off)
+            elif type_id == self.ENCRYPTION and l >= 1:
+                crypt_flag, = byte_struct.unpack_from(p, off)
+            elif type_id == self.MARS:
+                self.conn._mars_enabled = bool(byte_struct.unpack_from(p, off)[0])
+            elif type_id == self.INSTOPT:
+                # ignore instance name mismatch
+                pass
+            i += 5
+        # if server do not has certificate do normal login
+        login.server_enc_flag = crypt_flag
+        if crypt_flag == PreLoginEnc.ENCRYPT_OFF:
+            if login.enc_flag == PreLoginEnc.ENCRYPT_ON:
+                raise tds_base.Error('Server returned unexpected ENCRYPT_ON value')
+            else:
+                # encrypt login packet only
+                tls.establish_channel(self)
+        elif crypt_flag == PreLoginEnc.ENCRYPT_ON:
+            # encrypt entire connection
+            tls.establish_channel(self)
+        elif crypt_flag == PreLoginEnc.ENCRYPT_REQ:
+            if login.enc_flag == PreLoginEnc.ENCRYPT_NOT_SUP:
+                raise tds_base.Error('Client does not have encryption enabled but it is required by server, '
+                                     'enable encryption and try connecting again')
+            else:
+                # encrypt entire connection
+                tls.establish_channel(self)
+        elif crypt_flag == PreLoginEnc.ENCRYPT_NOT_SUP:
+            if login.enc_flag == PreLoginEnc.ENCRYPT_ON:
+                raise tds_base.Error('You requested encryption but it is not supported by server')
+            # do not encrypt anything
+
+    def tds7_send_login(self, login):
+        # https://msdn.microsoft.com/en-us/library/dd304019.aspx
+        option_flag2 = login.option_flag2
+        user_name = login.user_name
+        if len(user_name) > 128:
+            raise ValueError('User name should be no longer that 128 characters')
+        if len(login.password) > 128:
+            raise ValueError('Password should be not longer than 128 characters')
+        if len(login.change_password) > 128:
+            raise ValueError('Password should be not longer than 128 characters')
+        if len(login.client_host_name) > 128:
+            raise ValueError('Host name should be not longer than 128 characters')
+        if len(login.app_name) > 128:
+            raise ValueError('App name should be not longer than 128 characters')
+        if len(login.server_name) > 128:
+            raise ValueError('Server name should be not longer than 128 characters')
+        if len(login.database) > 128:
+            raise ValueError('Database name should be not longer than 128 characters')
+        if len(login.language) > 128:
+            raise ValueError('Language should be not longer than 128 characters')
+        if len(login.attach_db_file) > 260:
+            raise ValueError('File path should be not longer than 260 characters')
+        w = self._writer
+        w.begin_packet(tds_base.TDS7_LOGIN)
+        self.authentication = None
+        current_pos = 86 + 8 if tds_base.IS_TDS72_PLUS(self) else 86
+        client_host_name = login.client_host_name
+        login.client_host_name = client_host_name
+        packet_size = current_pos + (len(client_host_name) + len(login.app_name) + len(login.server_name) +
+                                     len(login.library) + len(login.language) + len(login.database)) * 2
+        if login.auth:
+            self.authentication = login.auth
+            auth_packet = login.auth.create_packet()
+            packet_size += len(auth_packet)
+        else:
+            auth_packet = ''
+            packet_size += (len(user_name) + len(login.password)) * 2
+        w.put_int(packet_size)
+        w.put_uint(login.tds_version)
+        w.put_int(w.bufsize)
+        from . import intversion
+        w.put_uint(intversion)
+        w.put_int(login.pid)
+        w.put_uint(0)  # connection id
+        option_flag1 = tds_base.TDS_SET_LANG_ON | tds_base.TDS_USE_DB_NOTIFY | tds_base.TDS_INIT_DB_FATAL
+        if not login.bulk_copy:
+            option_flag1 |= tds_base.TDS_DUMPLOAD_OFF
+        w.put_byte(option_flag1)
+        if self.authentication:
+            option_flag2 |= tds_base.TDS_INTEGRATED_SECURITY_ON
+        w.put_byte(option_flag2)
+        type_flags = 0
+        if login.readonly:
+            type_flags |= (2 << 5)
+        w.put_byte(type_flags)
+        option_flag3 = tds_base.TDS_UNKNOWN_COLLATION_HANDLING
+        w.put_byte(option_flag3 if tds_base.IS_TDS73_PLUS(self) else 0)
+        mins_fix = int(login.client_tz.utcoffset(datetime.datetime.now()).total_seconds()) // 60
+        w.put_int(mins_fix)
+        w.put_int(login.client_lcid)
+        w.put_smallint(current_pos)
+        w.put_smallint(len(client_host_name))
+        current_pos += len(client_host_name) * 2
+        if self.authentication:
+            w.put_smallint(0)
+            w.put_smallint(0)
+            w.put_smallint(0)
+            w.put_smallint(0)
+        else:
+            w.put_smallint(current_pos)
+            w.put_smallint(len(user_name))
+            current_pos += len(user_name) * 2
+            w.put_smallint(current_pos)
+            w.put_smallint(len(login.password))
+            current_pos += len(login.password) * 2
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.app_name))
+        current_pos += len(login.app_name) * 2
+        # server name
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.server_name))
+        current_pos += len(login.server_name) * 2
+        # reserved
+        w.put_smallint(0)
+        w.put_smallint(0)
+        # library name
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.library))
+        current_pos += len(login.library) * 2
+        # language
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.language))
+        current_pos += len(login.language) * 2
+        # database name
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.database))
+        current_pos += len(login.database) * 2
+        # ClientID
+        client_id = struct.pack('>Q', login.client_id)[2:]
+        w.write(client_id)
+        # authentication
+        w.put_smallint(current_pos)
+        w.put_smallint(len(auth_packet))
+        current_pos += len(auth_packet)
+        # db file
+        w.put_smallint(current_pos)
+        w.put_smallint(len(login.attach_db_file))
+        current_pos += len(login.attach_db_file) * 2
+        if tds_base.IS_TDS72_PLUS(self):
+            # new password
+            w.put_smallint(current_pos)
+            w.put_smallint(len(login.change_password))
+            # sspi long
+            w.put_int(0)
+        w.write_ucs2(client_host_name)
+        if not self.authentication:
+            w.write_ucs2(user_name)
+            w.write(tds7_crypt_pass(login.password))
+        w.write_ucs2(login.app_name)
+        w.write_ucs2(login.server_name)
+        w.write_ucs2(login.library)
+        w.write_ucs2(login.language)
+        w.write_ucs2(login.database)
+        if self.authentication:
+            w.write(auth_packet)
+        w.write_ucs2(login.attach_db_file)
+        w.write_ucs2(login.change_password)
+        w.flush()
+
+    _SERVER_TO_CLIENT_MAPPING = {
+        0x07000000: tds_base.TDS70,
+        0x07010000: tds_base.TDS71,
+        0x71000001: tds_base.TDS71rev1,
+        tds_base.TDS72: tds_base.TDS72,
+        tds_base.TDS73A: tds_base.TDS73A,
+        tds_base.TDS73B: tds_base.TDS73B,
+        tds_base.TDS74: tds_base.TDS74,
+        }
+
+    def process_login_tokens(self):
+        r = self._reader
+        succeed = False
+        while True:
+            marker = r.get_byte()
+            if marker == tds_base.TDS_LOGINACK_TOKEN:
+                succeed = True
+                size = r.get_smallint()
+                r.get_byte()  # interface
+                version = r.get_uint_be()
+                self.conn.tds_version = self._SERVER_TO_CLIENT_MAPPING.get(version, version)
+                if not tds_base.IS_TDS7_PLUS(self):
+                    self.bad_stream('Only TDS 7.0 and higher are supported')
+                # get server product name
+                # ignore product name length, some servers seem to set it incorrectly
+                r.get_byte()
+                size -= 10
+                self.conn.product_name = r.read_ucs2(size // 2)
+                product_version = r.get_uint_be()
+                # MSSQL 6.5 and 7.0 seem to return strange values for this
+                # using TDS 4.2, something like 5F 06 32 FF for 6.50
+                self.conn.product_version = product_version
+                if self.conn.authentication:
+                    self.conn.authentication.close()
+                    self.conn.authentication = None
+            else:
+                self.process_token(marker)
+                if marker == tds_base.TDS_DONE_TOKEN:
+                    break
+        return succeed
+
+    def process_returnstatus(self):
+        self.ret_status = self._reader.get_int()
+        self.has_status = True
+
+    def process_token(self, marker):
+        handler = _token_map.get(marker)
+        if not handler:
+            self.bad_stream('Invalid TDS marker: {0}({0:x})'.format(marker))
+        return handler(self)
+
+    def get_token_id(self):
+        self.set_state(tds_base.TDS_READING)
+        try:
+            marker = self._reader.get_byte()
+        except tds_base.TimeoutError:
+            self.set_state(tds_base.TDS_PENDING)
+            raise
+        except:
+            self._tds.close()
+            raise
+        return marker
+
+    def process_simple_request(self):
+        while True:
+            marker = self.get_token_id()
+            if marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
+                self.process_end(marker)
+                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS:
+                    # skip results that don't event have rowcount
+                    continue
+                return
+            else:
+                self.process_token(marker)
+
+    def next_set(self):
+        while self.more_rows:
+            self.next_row()
+        if self.state == tds_base.TDS_IDLE:
+            return False
+        if self.find_result_or_done():
+            return True
+
+    def fetchone(self):
+        if self.res_info is None:
+            raise tds_base.ProgrammingError("Previous statement didn't produce any results")
+
+        if self.skipped_to_status:
+            raise tds_base.ProgrammingError("Unable to fetch any rows after accessing return_status")
+
+        if not self.next_row():
+            return None
+
+        return self.row
+
+    def next_row(self):
+        if not self.more_rows:
+            return False
+        while True:
+            marker = self.get_token_id()
+            if marker in (tds_base.TDS_ROW_TOKEN, tds_base.TDS_NBC_ROW_TOKEN):
+                self.process_token(marker)
+                return True
+            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
+                self.process_end(marker)
+                return False
+            else:
+                self.process_token(marker)
+
+    def find_result_or_done(self):
+        self.done_flags = 0
+        while True:
+            marker = self.get_token_id()
+            if marker == tds_base.TDS7_RESULT_TOKEN:
+                self.process_token(marker)
+                return True
+            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN, tds_base.TDS_DONEINPROC_TOKEN):
+                self.process_end(marker)
+                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS:
+                    if self.done_flags & tds_base.TDS_DONE_COUNT:
+                        return True
+                    else:
+                        # skip results without rowcount
+                        continue
+                else:
+                    return False
+            else:
+                self.process_token(marker)
+
+    def process_rpc(self):
+        self.done_flags = 0
+        self.return_value_index = 0
+        while True:
+            marker = self.get_token_id()
+            if marker == tds_base.TDS7_RESULT_TOKEN:
+                self.process_token(marker)
+                return True
+            elif marker in (tds_base.TDS_DONE_TOKEN, tds_base.TDS_DONEPROC_TOKEN):
+                self.process_end(marker)
+                if self.done_flags & tds_base.TDS_DONE_MORE_RESULTS and not self.done_flags & tds_base.TDS_DONE_COUNT:
+                    # skip results that don't event have rowcount
+                    continue
+                return False
+            else:
+                self.process_token(marker)
+
+    def find_return_status(self):
+        self.skipped_to_status = True
+        while True:
+            marker = self.get_token_id()
+            self.process_token(marker)
+            if marker == tds_base.TDS_RETURNSTATUS_TOKEN:
+                return
+
+
+_token_map = {
+    tds_base.TDS_AUTH_TOKEN: _TdsSession.process_auth,
+    tds_base.TDS_ENVCHANGE_TOKEN: _TdsSession.process_env_chg,
+    tds_base.TDS_DONE_TOKEN: lambda self: self.process_end(tds_base.TDS_DONE_TOKEN),
+    tds_base.TDS_DONEPROC_TOKEN: lambda self: self.process_end(tds_base.TDS_DONEPROC_TOKEN),
+    tds_base.TDS_DONEINPROC_TOKEN: lambda self: self.process_end(tds_base.TDS_DONEINPROC_TOKEN),
+    tds_base.TDS_ERROR_TOKEN: lambda self: self.process_msg(tds_base.TDS_ERROR_TOKEN),
+    tds_base.TDS_INFO_TOKEN: lambda self: self.process_msg(tds_base.TDS_INFO_TOKEN),
+    tds_base.TDS_EED_TOKEN: lambda self: self.process_msg(tds_base.TDS_EED_TOKEN),
+    tds_base.TDS_CAPABILITY_TOKEN: lambda self: self.process_msg(tds_base.TDS_CAPABILITY_TOKEN),
+    tds_base.TDS_PARAM_TOKEN: lambda self: self.process_param(),
+    tds_base.TDS7_RESULT_TOKEN: lambda self: self.tds7_process_result(),
+    tds_base.TDS_ROW_TOKEN: lambda self: self.process_row(),
+    tds_base.TDS_NBC_ROW_TOKEN: lambda self: self.process_nbcrow(),
+    tds_base.TDS_ORDERBY2_TOKEN: lambda self: self.process_orderby2(),
+    tds_base.TDS_ORDERBY_TOKEN: lambda self: self.process_orderby(),
+    tds_base.TDS_RETURNSTATUS_TOKEN: lambda self: self.process_returnstatus(),
+    }
+
+
+class _TdsSocket(object):
+    def __init__(self, use_tz=None):
+        self._is_connected = False
+        self.env = _TdsEnv()
+        self.collation = None
+        self.tds72_transaction = 0
+        self.authentication = None
+        self._mars_enabled = False
+        self.chunk_handler = MemoryChunkedHandler()
+        self.sock = None
+        self.bufsize = 4096
+        self.tds_version = tds_base.TDS74
+        self.use_tz = use_tz
+        self.type_factory = tds_types.SerializerFactory(self.tds_version)
+        self.type_inferrer = None
+        self.query_timeout = 0
+        self._smp_manager = None
+        self._main_session = None
+        self._login = None
+
+    def __repr__(self):
+        fmt = "<_TdsSocket tran={} mars={} tds_version={} use_tz={}>"
+        return fmt.format(self.tds72_transaction, self._mars_enabled,
+                          self.tds_version, self.use_tz)
+
+    def login(self, login, sock, tzinfo_factory):
+        self._login = login
+        self.bufsize = login.blocksize
+        self.query_timeout = login.query_timeout
+        self._main_session = _TdsSession(self, self, tzinfo_factory)
+        self.sock = sock
+        self.tds_version = login.tds_version
+        login.server_enc_flag = PreLoginEnc.ENCRYPT_NOT_SUP
+        if tds_base.IS_TDS71_PLUS(self):
+            self._main_session.send_prelogin(login)
+            self._main_session.process_prelogin(login)
+        if tds_base.IS_TDS7_PLUS(self):
+            self._main_session.tds7_send_login(login)
+        else:
+            raise ValueError('This TDS version is not supported')
+        if login.server_enc_flag == PreLoginEnc.ENCRYPT_OFF:
+            tls.revert_to_clear(self._main_session)
+        if not self._main_session.process_login_tokens():
+            self._main_session.raise_db_exception()
+        self.type_factory = tds_types.SerializerFactory(self.tds_version)
+        self.type_inferrer = tds_types.TdsTypeInferrer(
+            type_factory=self.type_factory,
+            collation=self.collation,
+            bytes_to_unicode=self._login.bytes_to_unicode,
+            allow_tz=not self.use_tz
+        )
+        text_size = login.text_size
+        if self._mars_enabled:
+            from .smp import SmpManager
+            self._smp_manager = SmpManager(self)
+            self._main_session = _TdsSession(
+                self,
+                self._smp_manager.create_session(),
+                tzinfo_factory)
+        self._is_connected = True
+        q = []
+        if text_size:
+            q.append('set textsize {0}'.format(int(text_size)))
+        if login.database and self.env.database != login.database:
+            q.append('use ' + tds_base.tds_quote_id(login.database))
+        if q:
+            self._main_session.submit_plain_query(''.join(q))
+            self._main_session.process_simple_request()
+
+    @property
+    def mars_enabled(self):
+        return self._mars_enabled
+
+    @property
+    def main_session(self):
+        return self._main_session
+
+    def create_session(self, tzinfo_factory):
+        return _TdsSession(
+            self, self._smp_manager.create_session(),
+            tzinfo_factory)
+
+    def read(self, size):
+        buf = self.sock.recv(size)
+        if len(buf) == 0:
+            self.close()
+            raise tds_base.ClosedConnectionError()
+        return buf
+
+    def _write(self, data, final):
+        try:
+            flags = 0
+            if hasattr(socket, 'MSG_NOSIGNAL'):
+                flags |= socket.MSG_NOSIGNAL
+            if not final:
+                if hasattr(socket, 'MSG_MORE'):
+                    flags |= socket.MSG_MORE
+            self.sock.sendall(data, flags)
+        except:
+            self.close()
+            raise
+
+    send = _write
+
+    def is_connected(self):
+        return self._is_connected
+
+    def close(self):
+        self._is_connected = False
+        if self.sock is not None:
+            self.sock.close()
+        if self._smp_manager:
+            self._smp_manager.transport_closed()
+        self._main_session.state = tds_base.TDS_DEAD
+        if self.authentication:
+            self.authentication.close()
+            self.authentication = None
+
+
+class _Results(object):
+    def __init__(self):
+            self.columns = []
+            self.row_count = 0
+
+
+def _parse_instances(msg):
+    name = None
+    if len(msg) > 3 and tds_base.my_ord(msg[0]) == 5:
+        tokens = msg[3:].decode('ascii').split(';')
+        results = {}
+        instdict = {}
+        got_name = False
+        for token in tokens:
+            if got_name:
+                instdict[name] = token
+                got_name = False
+            else:
+                name = token
+                if not name:
+                    if not instdict:
+                        break
+                    results[instdict['InstanceName'].upper()] = instdict
+                    instdict = {}
+                    continue
+                got_name = True
+        return results
+
+
+#
+# Get port of all instances
+# @return default port number or 0 if error
+# @remark experimental, cf. MC-SQLR.pdf.
+#
+def tds7_get_instances(ip_addr, timeout=5):
+    s = socket.socket(type=socket.SOCK_DGRAM)
+    s.settimeout(timeout)
+    try:
+        # send the request
+        s.sendto(b'\x03', (ip_addr, 1434))
+        msg = s.recv(16 * 1024 - 1)
+        # got data, read and parse
+        return _parse_instances(msg)
+    finally:
+        s.close()
```

### Comparing `python-tds-1.9.0/pytds/tds_types.py` & `python-tds-1.9.1/pytds/tds_types.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,2600 +1,2600 @@
-import itertools
-import datetime
-import decimal
-import struct
-import re
-import uuid
-import six
-import functools
-
-from . import tds_base
-from .collate import ucs2_codec, raw_collation
-from . import tz
-
-
-_flt4_struct = struct.Struct('f')
-_flt8_struct = struct.Struct('d')
-_utc = tz.utc
-
-
-def _applytz(dt, tzinfo):
-    if not tzinfo:
-        return dt
-    dt = dt.replace(tzinfo=tzinfo)
-    return dt
-
-
-def _decode_num(buf):
-    """ Decodes little-endian integer from buffer
-
-    Buffer can be of any size
-    """
-    return functools.reduce(lambda acc, val: acc * 256 + tds_base.my_ord(val), reversed(buf), 0)
-
-
-class PlpReader(object):
-    """ Partially length prefixed reader
-
-    Spec: http://msdn.microsoft.com/en-us/library/dd340469.aspx
-    """
-    def __init__(self, r):
-        """
-        :param r: An instance of :class:`_TdsReader`
-        """
-        self._rdr = r
-        size = r.get_uint8()
-        self._size = size
-
-    def is_null(self):
-        """
-        :return: True if stored value is NULL
-        """
-        return self._size == tds_base.PLP_NULL
-
-    def is_unknown_len(self):
-        """
-        :return: True if total size is unknown upfront
-        """
-        return self._size == tds_base.PLP_UNKNOWN
-
-    def size(self):
-        """
-        :return: Total size in bytes if is_uknown_len and is_null are both False
-        """
-        return self._size
-
-    def chunks(self):
-        """ Generates chunks from stream, each chunk is an instace of bytes.
-        """
-        if self.is_null():
-            return
-        total = 0
-        while True:
-            chunk_len = self._rdr.get_uint()
-            if chunk_len == 0:
-                if not self.is_unknown_len() and total != self._size:
-                    msg = "PLP actual length (%d) doesn't match reported length (%d)" % (total, self._size)
-                    self._rdr.session.bad_stream(msg)
-
-                return
-
-            total += chunk_len
-            left = chunk_len
-            while left:
-                buf = self._rdr.read(left)
-                yield buf
-                left -= len(buf)
-
-
-class SqlTypeMetaclass(tds_base.CommonEqualityMixin):
-    def __repr__(self):
-        return '<sqltype:{}>'.format(self.get_declaration())
-
-    def get_declaration(self):
-        raise NotImplementedError()
-
-
-class ImageType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'IMAGE'
-
-
-class BinaryType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'BINARY({})'.format(self._size)
-
-
-class VarBinaryType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'VARBINARY({})'.format(self._size)
-
-
-class VarBinaryMaxType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'VARBINARY(MAX)'
-
-
-class CharType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'CHAR({})'.format(self._size)
-
-
-class VarCharType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'VARCHAR({})'.format(self._size)
-
-
-class VarCharMaxType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'VARCHAR(MAX)'
-
-
-class NCharType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'NCHAR({})'.format(self._size)
-
-
-class NVarCharType(SqlTypeMetaclass):
-    def __init__(self, size=30):
-        self._size = size
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_declaration(self):
-        return 'NVARCHAR({})'.format(self._size)
-
-
-class NVarCharMaxType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'NVARCHAR(MAX)'
-
-
-class TextType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'TEXT'
-
-
-class NTextType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'NTEXT'
-
-
-class XmlType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'XML'
-
-
-class SmallMoneyType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'SMALLMONEY'
-
-
-class MoneyType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'MONEY'
-
-
-class DecimalType(SqlTypeMetaclass):
-    def __init__(self, precision=18, scale=0):
-        self._precision = precision
-        self._scale = scale
-
-    @classmethod
-    def from_value(cls, value):
-        if not (-10 ** 38 + 1 <= value <= 10 ** 38 - 1):
-            raise tds_base.DataError('Decimal value is out of range')
-        value = value.normalize()
-        _, digits, exp = value.as_tuple()
-        if exp > 0:
-            scale = 0
-            prec = len(digits) + exp
-        else:
-            scale = -exp
-            prec = max(len(digits), scale)
-        return cls(precision=prec, scale=scale)
-
-    @property
-    def precision(self):
-        return self._precision
-
-    @property
-    def scale(self):
-        return self._scale
-
-    def get_declaration(self):
-        return 'DECIMAL({}, {})'.format(self._precision, self._scale)
-
-
-class UniqueIdentifierType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'UNIQUEIDENTIFIER'
-
-
-class VariantType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'SQL_VARIANT'
-
-
-class SqlValueMetaclass(tds_base.CommonEqualityMixin):
-    pass
-
-
-class BaseTypeSerializer(tds_base.CommonEqualityMixin):
-    """ Base type for TDS data types.
-
-    All TDS types should derive from it.
-    In addition actual types should provide the following:
-
-    - type - class variable storing type identifier
-    """
-    type = 0
-
-    def __init__(self, precision=None, scale=None, size=None):
-        self._precision = precision
-        self._scale = scale
-        self._size = size
-
-    @property
-    def precision(self):
-        return self._precision
-
-    @property
-    def scale(self):
-        return self._scale
-
-    @property
-    def size(self):
-        return self._size
-
-    def get_typeid(self):
-        """ Returns type identifier of type. """
-        return self.type
-
-    @classmethod
-    def from_stream(cls, r):
-        """ Class method that reads and returns a type instance.
-
-        :param r: An instance of :class:`_TdsReader` to read type from.
-
-        Should be implemented in actual types.
-        """
-        raise NotImplementedError
-
-    def write_info(self, w):
-        """ Writes type info into w stream.
-
-        :param w: An instance of :class:`_TdsWriter` to write into.
-
-        Should be symmetrical to from_stream method.
-        Should be implemented in actual types.
-        """
-        raise NotImplementedError
-
-    def write(self, w, value):
-        """ Writes type's value into stream
-
-        :param w: An instance of :class:`_TdsWriter` to write into.
-        :param value: A value to be stored, should be compatible with the type
-
-        Should be implemented in actual types.
-        """
-        raise NotImplementedError
-
-    def read(self, r):
-        """ Reads value from the stream.
-
-        :param r: An instance of :class:`_TdsReader` to read value from.
-        :return: A read value.
-
-        Should be implemented in actual types.
-        """
-        raise NotImplementedError
-
-
-class BasePrimitiveTypeSerializer(BaseTypeSerializer):
-    """ Base type for primitive TDS data types.
-
-    Primitive type is a fixed size type with no type arguments.
-    All primitive TDS types should derive from it.
-    In addition actual types should provide the following:
-
-    - type - class variable storing type identifier
-    - declaration - class variable storing name of sql type
-    - isntance - class variable storing instance of class
-    """
-
-    def write(self, w, value):
-        raise NotImplementedError
-
-    def read(self, r):
-        raise NotImplementedError
-
-    instance = None
-
-    @classmethod
-    def from_stream(cls, r):
-        return cls.instance
-
-    def write_info(self, w):
-        pass
-
-
-class BaseTypeSerializerN(BaseTypeSerializer):
-    """ Base type for nullable TDS data types.
-
-    All nullable TDS types should derive from it.
-    In addition actual types should provide the following:
-
-    - type - class variable storing type identifier
-    - subtypes - class variable storing dict {subtype_size: subtype_instance}
-    """
-    subtypes = {}
-
-    def __init__(self, size):
-        super(BaseTypeSerializerN, self).__init__(size=size)
-        assert size in self.subtypes
-        self._current_subtype = self.subtypes[size]
-
-    def get_typeid(self):
-        return self._current_subtype.get_typeid()
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_byte()
-        if size not in cls.subtypes:
-            raise tds_base.InterfaceError('Invalid %s size' % cls.type, size)
-        return cls(size)
-
-    def write_info(self, w):
-        w.put_byte(self.size)
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        if size not in self.subtypes:
-            raise r.session.bad_stream('Invalid %s size' % self.type, size)
-        return self.subtypes[size].read(r)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_byte(0)
-            return
-        w.put_byte(self.size)
-        self._current_subtype.write(w, val)
-
-
-class BitType(SqlTypeMetaclass):
-    type = tds_base.SYBBITN
-
-    def get_declaration(self):
-        return 'BIT'
-
-
-class TinyIntType(SqlTypeMetaclass):
-    type = tds_base.SYBINTN
-    size = 1
-
-    def get_declaration(self):
-        return 'TINYINT'
-
-
-class SmallIntType(SqlTypeMetaclass):
-    type = tds_base.SYBINTN
-    size = 2
-
-    def get_declaration(self):
-        return 'SMALLINT'
-
-
-class IntType(SqlTypeMetaclass):
-    type = tds_base.SYBINTN
-    size = 4
-
-    def get_declaration(self):
-        return 'INT'
-
-
-class BigIntType(SqlTypeMetaclass):
-    type = tds_base.SYBINTN
-    size = 8
-
-    def get_declaration(self):
-        return 'BIGINT'
-
-
-class RealType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'REAL'
-
-
-class FloatType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'FLOAT'
-
-
-class BitSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBBIT
-    declaration = 'BIT'
-
-    def write(self, w, value):
-        w.put_byte(1 if value else 0)
-
-    def read(self, r):
-        return bool(r.get_byte())
-
-BitSerializer.instance = BitSerializer()
-
-
-class BitNSerializer(BaseTypeSerializerN):
-    type = tds_base.SYBBITN
-    subtypes = {1: BitSerializer.instance}
-
-    def __init__(self, typ):
-        super(BitNSerializer, self).__init__(size=1)
-        self._typ = typ
-
-    def __repr__(self):
-        return 'BitNSerializer({})'.format(self._typ)
-
-
-BitNSerializer.instance = BitNSerializer(BitType())
-
-
-class TinyIntSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBINT1
-    declaration = 'TINYINT'
-
-    def write(self, w, val):
-        w.put_byte(val)
-
-    def read(self, r):
-        return r.get_byte()
-
-TinyIntSerializer.instance = TinyIntSerializer()
-
-
-class SmallIntSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBINT2
-    declaration = 'SMALLINT'
-
-    def write(self, w, val):
-        w.put_smallint(val)
-
-    def read(self, r):
-        return r.get_smallint()
-
-SmallIntSerializer.instance = SmallIntSerializer()
-
-
-class IntSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBINT4
-    declaration = 'INT'
-
-    def write(self, w, val):
-        w.put_int(val)
-
-    def read(self, r):
-        return r.get_int()
-
-IntSerializer.instance = IntSerializer()
-
-
-class BigIntSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBINT8
-    declaration = 'BIGINT'
-
-    def write(self, w, val):
-        w.put_int8(val)
-
-    def read(self, r):
-        return r.get_int8()
-
-BigIntSerializer.instance = BigIntSerializer()
-
-
-class IntNSerializer(BaseTypeSerializerN):
-    type = tds_base.SYBINTN
-
-    subtypes = {
-        1: TinyIntSerializer.instance,
-        2: SmallIntSerializer.instance,
-        4: IntSerializer.instance,
-        8: BigIntSerializer.instance,
-    }
-
-    type_by_size = {
-        1: TinyIntType(),
-        2: SmallIntType(),
-        4: IntType(),
-        8: BigIntType(),
-    }
-
-    def __init__(self, typ):
-        super(IntNSerializer, self).__init__(size=typ.size)
-        self._typ = typ
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_byte()
-        if size not in cls.subtypes:
-            raise tds_base.InterfaceError('Invalid %s size' % cls.type, size)
-        return cls(cls.type_by_size[size])
-
-    def __repr__(self):
-        return 'IntN({})'.format(self.size)
-
-
-class RealSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBREAL
-    declaration = 'REAL'
-
-    def write(self, w, val):
-        w.pack(_flt4_struct, val)
-
-    def read(self, r):
-        return r.unpack(_flt4_struct)[0]
-
-RealSerializer.instance = RealSerializer()
-
-
-class FloatSerializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBFLT8
-    declaration = 'FLOAT'
-
-    def write(self, w, val):
-        w.pack(_flt8_struct, val)
-
-    def read(self, r):
-        return r.unpack(_flt8_struct)[0]
-
-FloatSerializer.instance = FloatSerializer()
-
-
-class FloatNSerializer(BaseTypeSerializerN):
-    type = tds_base.SYBFLTN
-
-    subtypes = {
-        4: RealSerializer.instance,
-        8: FloatSerializer.instance,
-    }
-
-
-class VarChar(SqlValueMetaclass):
-    def __init__(self, val, collation=raw_collation):
-        self._val = val
-        self._collation = collation
-
-    @property
-    def collation(self):
-        return self._collation
-
-    @property
-    def val(self):
-        return self._val
-
-    def __str__(self):
-        return self._val
-
-
-class VarChar70Serializer(BaseTypeSerializer):
-    type = tds_base.XSYBVARCHAR
-
-    def __init__(self, size, collation=raw_collation, codec=None):
-        super(VarChar70Serializer, self).__init__(size=size)
-        self._collation = collation
-        if codec:
-            self._codec = codec
-        else:
-            self._codec = collation.get_codec()
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_smallint()
-        return cls(size, codec=r.session.conn.server_codec)
-
-    def write_info(self, w):
-        w.put_smallint(self.size)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_smallint(-1)
-        else:
-            if w._tds._tds._login.bytes_to_unicode:
-                val = tds_base.force_unicode(val)
-            if isinstance(val, six.text_type):
-                val, _ = self._codec.encode(val)
-            w.put_smallint(len(val))
-            w.write(val)
-
-    def read(self, r):
-        size = r.get_smallint()
-        if size < 0:
-            return None
-        if r._session._tds._login.bytes_to_unicode:
-            return r.read_str(size, self._codec)
-        else:
-            return tds_base.readall(r, size)
-
-
-class VarChar71Serializer(VarChar70Serializer):
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_smallint()
-        collation = r.get_collation()
-        return cls(size, collation)
-
-    def write_info(self, w):
-        super(VarChar71Serializer, self).write_info(w)
-        w.put_collation(self._collation)
-
-
-class VarChar72Serializer(VarChar71Serializer):
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        collation = r.get_collation()
-        if size == 0xffff:
-            return VarCharMaxSerializer(collation)
-        return cls(size, collation)
-
-
-class VarCharMaxSerializer(VarChar72Serializer):
-    def __init__(self, collation=raw_collation):
-        super(VarChar72Serializer, self).__init__(0, collation)
-
-    def write_info(self, w):
-        w.put_usmallint(tds_base.PLP_MARKER)
-        w.put_collation(self._collation)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_uint8(tds_base.PLP_NULL)
-        else:
-            if w._tds._tds._login.bytes_to_unicode:
-                val = tds_base.force_unicode(val)
-            if isinstance(val, six.text_type):
-                val, _ = self._codec.encode(val)
-            w.put_int8(len(val))
-            if len(val) > 0:
-                w.put_int(len(val))
-                w.write(val)
-            w.put_int(0)
-
-    def read(self, r):
-        login = r._session._tds._login
-        r = PlpReader(r)
-        if r.is_null():
-            return None
-        if login.bytes_to_unicode:
-            return ''.join(tds_base.iterdecode(r.chunks(), self._codec))
-        else:
-            return six.b('').join(r.chunks())
-
-
-class NVarChar70Serializer(BaseTypeSerializer):
-    type = tds_base.XSYBNVARCHAR
-
-    def __init__(self, size, collation=raw_collation):
-        super(NVarChar70Serializer, self).__init__(size=size)
-        self._collation = collation
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        return cls(size / 2)
-
-    def write_info(self, w):
-        w.put_usmallint(self.size * 2)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_usmallint(0xffff)
-        else:
-            if isinstance(val, bytes):
-                val = tds_base.force_unicode(val)
-            buf, _ = ucs2_codec.encode(val)
-            l = len(buf)
-            w.put_usmallint(l)
-            w.write(buf)
-
-    def read(self, r):
-        size = r.get_usmallint()
-        if size == 0xffff:
-            return None
-        return r.read_str(size, ucs2_codec)
-
-
-class NVarChar71Serializer(NVarChar70Serializer):
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        collation = r.get_collation()
-        return cls(size / 2, collation)
-
-    def write_info(self, w):
-        super(NVarChar71Serializer, self).write_info(w)
-        w.put_collation(self._collation)
-
-
-class NVarChar72Serializer(NVarChar71Serializer):
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        collation = r.get_collation()
-        if size == 0xffff:
-            return NVarCharMaxSerializer(collation=collation)
-        return cls(size / 2, collation=collation)
-
-
-class NVarCharMaxSerializer(NVarChar72Serializer):
-    def __init__(self, collation=raw_collation):
-        super(NVarCharMaxSerializer, self).__init__(size=-1, collation=collation)
-
-    def __repr__(self):
-        return 'NVarCharMax(s={},c={})'.format(self.size, repr(self._collation))
-
-    def get_typeid(self):
-        return tds_base.SYBNTEXT
-
-    def write_info(self, w):
-        w.put_usmallint(tds_base.PLP_MARKER)
-        w.put_collation(self._collation)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_uint8(tds_base.PLP_NULL)
-        else:
-            if isinstance(val, bytes):
-                val = tds_base.force_unicode(val)
-            val, _ = ucs2_codec.encode(val)
-            w.put_uint8(len(val))
-            if len(val) > 0:
-                w.put_uint(len(val))
-                w.write(val)
-            w.put_uint(0)
-
-    def read(self, r):
-        r = PlpReader(r)
-        if r.is_null():
-            return None
-        res = ''.join(tds_base.iterdecode(r.chunks(), ucs2_codec))
-        return res
-
-
-class XmlSerializer(NVarCharMaxSerializer):
-    type = tds_base.SYBMSXML
-    declaration = 'XML'
-
-    def __init__(self, schema=None):
-        super(XmlSerializer, self).__init__(0)
-        self._schema = schema or {}
-
-    def __repr__(self):
-        return 'XmlSerializer(schema={})'.format(repr(self._schema))
-
-    def get_typeid(self):
-        return self.type
-
-    @classmethod
-    def from_stream(cls, r):
-        has_schema = r.get_byte()
-        schema = {}
-        if has_schema:
-            schema['dbname'] = r.read_ucs2(r.get_byte())
-            schema['owner'] = r.read_ucs2(r.get_byte())
-            schema['collection'] = r.read_ucs2(r.get_smallint())
-        return cls(schema)
-
-    def write_info(self, w):
-        if self._schema:
-            w.put_byte(1)
-            w.put_byte(len(self._schema['dbname']))
-            w.write_ucs2(self._schema['dbname'])
-            w.put_byte(len(self._schema['owner']))
-            w.write_ucs2(self._schema['owner'])
-            w.put_usmallint(len(self._schema['collection']))
-            w.write_ucs2(self._schema['collection'])
-        else:
-            w.put_byte(0)
-
-
-class Text70Serializer(BaseTypeSerializer):
-    type = tds_base.SYBTEXT
-    declaration = 'TEXT'
-
-    def __init__(self, size=0, table_name='', collation=raw_collation, codec=None):
-        super(Text70Serializer, self).__init__(size=size)
-        self._table_name = table_name
-        self._collation = collation
-        if codec:
-            self._codec = codec
-        else:
-            self._codec = collation.get_codec()
-
-    def __repr__(self):
-        return 'Text70(size={},table_name={},codec={})'.format(self.size, self._table_name, self._codec)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        table_name = r.read_ucs2(r.get_smallint())
-        return cls(size, table_name, codec=r.session.conn.server_codec)
-
-    def write_info(self, w):
-        w.put_int(self.size)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_int(-1)
-        else:
-            if w._tds._tds._login.bytes_to_unicode:
-                val = tds_base.force_unicode(val)
-            if isinstance(val, six.text_type):
-                val, _ = self._codec.encode(val)
-            w.put_int(len(val))
-            w.write(val)
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        tds_base.readall(r, size)  # textptr
-        tds_base.readall(r, 8)  # timestamp
-        colsize = r.get_int()
-        if r._session._tds._login.bytes_to_unicode:
-            return r.read_str(colsize, self._codec)
-        else:
-            return tds_base.readall(r, colsize)
-
-
-class Text71Serializer(Text70Serializer):
-    def __repr__(self):
-        return 'Text71(size={}, table_name={}, collation={})'.format(
-            self.size, self._table_name, repr(self._collation)
-        )
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        collation = r.get_collation()
-        table_name = r.read_ucs2(r.get_smallint())
-        return cls(size, table_name, collation)
-
-    def write_info(self, w):
-        w.put_int(self.size)
-        w.put_collation(self._collation)
-
-
-class Text72Serializer(Text71Serializer):
-    def __init__(self, size=0, table_name_parts=(), collation=raw_collation):
-        super(Text72Serializer, self).__init__(size=size, table_name='.'.join(table_name_parts), collation=collation)
-        self._table_name_parts = table_name_parts
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        collation = r.get_collation()
-        num_parts = r.get_byte()
-        parts = []
-        for _ in range(num_parts):
-            parts.append(r.read_ucs2(r.get_smallint()))
-        return cls(size, parts, collation)
-
-
-class NText70Serializer(BaseTypeSerializer):
-    type = tds_base.SYBNTEXT
-    declaration = 'NTEXT'
-
-    def __init__(self, size=0, table_name='', collation=raw_collation):
-        super(NText70Serializer, self).__init__(size=size)
-        self._collation = collation
-        self._table_name = table_name
-
-    def __repr__(self):
-        return 'NText70(size={}, table_name={})'.format(self.size, self._table_name)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        table_name = r.read_ucs2(r.get_smallint())
-        return cls(size, table_name)
-
-    def read(self, r):
-        textptr_size = r.get_byte()
-        if textptr_size == 0:
-            return None
-        tds_base.readall(r, textptr_size)  # textptr
-        tds_base.readall(r, 8)  # timestamp
-        colsize = r.get_int()
-        return r.read_str(colsize, ucs2_codec)
-
-    def write_info(self, w):
-        w.put_int(self.size * 2)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_int(-1)
-        else:
-            w.put_int(len(val) * 2)
-            w.write_ucs2(val)
-
-
-class NText71Serializer(NText70Serializer):
-    def __repr__(self):
-        return 'NText71(size={}, table_name={}, collation={})'.format(self.size,
-                                                                      self._table_name,
-                                                                      repr(self._collation))
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        collation = r.get_collation()
-        table_name = r.read_ucs2(r.get_smallint())
-        return cls(size, table_name, collation)
-
-    def write_info(self, w):
-        w.put_int(self.size)
-        w.put_collation(self._collation)
-
-    def read(self, r):
-        textptr_size = r.get_byte()
-        if textptr_size == 0:
-            return None
-        tds_base.readall(r, textptr_size)  # textptr
-        tds_base.readall(r, 8)  # timestamp
-        colsize = r.get_int()
-        return r.read_str(colsize, ucs2_codec)
-
-
-class NText72Serializer(NText71Serializer):
-    def __init__(self, size=0, table_name_parts=(), collation=raw_collation):
-        super(NText72Serializer, self).__init__(size=size, collation=collation)
-        self._table_name_parts = table_name_parts
-
-    def __repr__(self):
-        return 'NText72Serializer(s={},table_name={},coll={})'.format(
-            self.size, self._table_name_parts, self._collation)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        collation = r.get_collation()
-        num_parts = r.get_byte()
-        parts = []
-        for _ in range(num_parts):
-            parts.append(r.read_ucs2(r.get_smallint()))
-        return cls(size, parts, collation)
-
-
-class Binary(bytes, SqlValueMetaclass):
-    def __repr__(self):
-        return 'Binary({0})'.format(super(Binary, self).__repr__())
-
-
-class VarBinarySerializer(BaseTypeSerializer):
-    type = tds_base.XSYBVARBINARY
-
-    def __init__(self, size):
-        super(VarBinarySerializer, self).__init__(size=size)
-
-    def __repr__(self):
-        return 'VarBinary({})'.format(self.size)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        return cls(size)
-
-    def write_info(self, w):
-        w.put_usmallint(self.size)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_usmallint(0xffff)
-        else:
-            w.put_usmallint(len(val))
-            w.write(val)
-
-    def read(self, r):
-        size = r.get_usmallint()
-        if size == 0xffff:
-            return None
-        return tds_base.readall(r, size)
-
-
-class VarBinarySerializer72(VarBinarySerializer):
-    def __repr__(self):
-        return 'VarBinary72({})'.format(self.size)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_usmallint()
-        if size == 0xffff:
-            return VarBinarySerializerMax()
-        return cls(size)
-
-
-class VarBinarySerializerMax(VarBinarySerializer):
-    def __init__(self):
-        super(VarBinarySerializerMax, self).__init__(0)
-
-    def __repr__(self):
-        return 'VarBinaryMax()'
-
-    def write_info(self, w):
-        w.put_usmallint(tds_base.PLP_MARKER)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_uint8(tds_base.PLP_NULL)
-        else:
-            w.put_uint8(len(val))
-            if val:
-                w.put_uint(len(val))
-                w.write(val)
-            w.put_uint(0)
-
-    def read(self, r):
-        r = PlpReader(r)
-        if r.is_null():
-            return None
-        return b''.join(r.chunks())
-
-class UDT72Serializer(BaseTypeSerializer):
-    # Data type definition stream used for UDT_INFO in TYPE_INFO
-    # https://msdn.microsoft.com/en-us/library/a57df60e-d0a6-4e7e-a2e5-ccacd277c673/
-    def __init__(self, max_byte_size, db_name, schema_name, type_name,
-                 assembly_qualified_name):
-        self.max_byte_size = max_byte_size
-        self.db_name = db_name
-        self.schema_name = schema_name
-        self.type_name = type_name
-        self.assembly_qualified_name = assembly_qualified_name
-        super(UDT72Serializer, self).__init__()
-
-    def __repr__(self):
-        return ('UDT72Serializer(max_byte_size={}, db_name={}, '
-                'schema_name={}, type_name={}, '
-                'assembly_qualified_name={})'.format(
-                    *map(repr, (
-                        self.max_byte_size, self.db_name, self.schema_name,
-                        self.type_name, self.assembly_qualified_name)))
-        )
-
-    @classmethod
-    def from_stream(cls, r):
-        # MAX_BYTE_SIZE
-        max_byte_size = r.get_usmallint()
-        assert max_byte_size == 0xffff or 1 < max_byte_size < 8000
-        # DB_NAME -- B_VARCHAR
-        db_name = r.read_ucs2(r.get_byte())
-        # SCHEMA_NAME -- B_VARCHAR
-        schema_name = r.read_ucs2(r.get_byte())
-        # TYPE_NAME -- B_VARCHAR
-        type_name = r.read_ucs2(r.get_byte())
-        # UDT_METADATA --
-        # a US_VARCHAR (2 bytes length prefix)
-        # containing ASSEMBLY_QUALIFIED_NAME
-        assembly_qualified_name = r.read_ucs2(r.get_smallint())
-        return cls(max_byte_size, db_name, schema_name, type_name,
-                   assembly_qualified_name)
-
-    def read(self, r):
-        r = PlpReader(r)
-        if r.is_null():
-            return None
-        return b''.join(r.chunks())
-
-class UDT72SerializerMax(UDT72Serializer):
-    def __init__(self, *args, **kwargs):
-        super(UDT72SerializerMax, self).__init__(0, *args, **kwargs)
-
-class Image70Serializer(BaseTypeSerializer):
-    type = tds_base.SYBIMAGE
-    declaration = 'IMAGE'
-
-    def __init__(self, size=0, table_name=''):
-        super(Image70Serializer, self).__init__(size=size)
-        self._table_name = table_name
-
-    def __repr__(self):
-        return 'Image70(tn={},s={})'.format(repr(self._table_name), self.size)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        table_name = r.read_ucs2(r.get_smallint())
-        return cls(size, table_name)
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 16:  # Jeff's hack
-            tds_base.readall(r, 16)  # textptr
-            tds_base.readall(r, 8)  # timestamp
-            colsize = r.get_int()
-            return tds_base.readall(r, colsize)
-        else:
-            return None
-
-    def write(self, w, val):
-        if val is None:
-            w.put_int(-1)
-            return
-        w.put_int(len(val))
-        w.write(val)
-
-    def write_info(self, w):
-        w.put_int(self.size)
-
-
-class Image72Serializer(Image70Serializer):
-    def __init__(self, size=0, parts=()):
-        super(Image72Serializer, self).__init__(size=size, table_name='.'.join(parts))
-        self._parts = parts
-
-    def __repr__(self):
-        return 'Image72(p={},s={})'.format(self._parts, self.size)
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        num_parts = r.get_byte()
-        parts = []
-        for _ in range(num_parts):
-            parts.append(r.read_ucs2(r.get_usmallint()))
-        return Image72Serializer(size, parts)
-
-
-_datetime_base_date = datetime.datetime(1900, 1, 1)
-
-
-class SmallDateTimeType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'SMALLDATETIME'
-
-
-class DateTimeType(SqlTypeMetaclass):
-    def get_declaration(self):
-        return 'DATETIME'
-
-
-class SmallDateTime(SqlValueMetaclass):
-    """Corresponds to MSSQL smalldatetime"""
-    def __init__(self, days, minutes):
-        """
-
-        @param days: Days since 1900-01-01
-        @param minutes: Minutes since 00:00:00
-        """
-        self._days = days
-        self._minutes = minutes
-
-    @property
-    def days(self):
-        return self._days
-
-    @property
-    def minutes(self):
-        return self._minutes
-
-    def to_pydatetime(self):
-        return _datetime_base_date + datetime.timedelta(days=self._days, minutes=self._minutes)
-
-    @classmethod
-    def from_pydatetime(cls, dt):
-        days = (dt - _datetime_base_date).days
-        minutes = dt.hour * 60 + dt.minute
-        return cls(days=days, minutes=minutes)
-
-
-class BaseDateTimeSerializer(BaseTypeSerializer):
-    def write(self, w, value):
-        raise NotImplementedError
-
-    def write_info(self, w):
-        raise NotImplementedError
-
-    def read(self, r):
-        raise NotImplementedError
-
-    @classmethod
-    def from_stream(cls, r):
-        raise NotImplementedError
-
-
-class SmallDateTimeSerializer(BasePrimitiveTypeSerializer, BaseDateTimeSerializer):
-    type = tds_base.SYBDATETIME4
-    declaration = 'SMALLDATETIME'
-
-    _struct = struct.Struct('<HH')
-
-    def write(self, w, val):
-        if val.tzinfo:
-            if not w.session.use_tz:
-                raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
-            val = val.astimezone(w.session.use_tz).replace(tzinfo=None)
-        dt = SmallDateTime.from_pydatetime(val)
-        w.pack(self._struct, dt.days, dt.minutes)
-
-    def read(self, r):
-        days, minutes = r.unpack(self._struct)
-        dt = SmallDateTime(days=days, minutes=minutes)
-        tzinfo = None
-        if r.session.tzinfo_factory is not None:
-            tzinfo = r.session.tzinfo_factory(0)
-        return dt.to_pydatetime().replace(tzinfo=tzinfo)
-
-SmallDateTimeSerializer.instance = SmallDateTimeSerializer()
-
-
-class DateTime(SqlValueMetaclass):
-    """Corresponds to MSSQL datetime"""
-    MIN_PYDATETIME = datetime.datetime(1753, 1, 1, 0, 0, 0)
-    MAX_PYDATETIME = datetime.datetime(9999, 12, 31, 23, 59, 59, 997000)
-
-    def __init__(self, days, time_part):
-        """
-
-        @param days: Days since 1900-01-01
-        @param time_part: Number of 1/300 of seconds since 00:00:00
-        """
-        self._days = days
-        self._time_part = time_part
-
-    @property
-    def days(self):
-        return self._days
-
-    @property
-    def time_part(self):
-        return self._time_part
-
-    def to_pydatetime(self):
-        ms = int(round(self._time_part % 300 * 10 / 3.0))
-        secs = self._time_part // 300
-        return _datetime_base_date + datetime.timedelta(days=self._days, seconds=secs, milliseconds=ms)
-
-    @classmethod
-    def from_pydatetime(cls, dt):
-        if not (cls.MIN_PYDATETIME <= dt <= cls.MAX_PYDATETIME):
-            raise tds_base.DataError('Datetime is out of range')
-        days = (dt - _datetime_base_date).days
-        ms = dt.microsecond // 1000
-        tm = (dt.hour * 60 * 60 + dt.minute * 60 + dt.second) * 300 + int(round(ms * 3 / 10.0))
-        return cls(days=days, time_part=tm)
-
-
-class DateTimeSerializer(BasePrimitiveTypeSerializer, BaseDateTimeSerializer):
-    type = tds_base.SYBDATETIME
-    declaration = 'DATETIME'
-
-    _struct = struct.Struct('<ll')
-
-    def write(self, w, val):
-        if val.tzinfo:
-            if not w.session.use_tz:
-                raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
-            val = val.astimezone(w.session.use_tz).replace(tzinfo=None)
-        w.write(self.encode(val))
-
-    def read(self, r):
-        days, t = r.unpack(self._struct)
-        tzinfo = None
-        if r.session.tzinfo_factory is not None:
-            tzinfo = r.session.tzinfo_factory(0)
-        return _applytz(self.decode(days, t), tzinfo)
-
-    @classmethod
-    def encode(cls, value):
-        if type(value) == datetime.date:
-            value = datetime.datetime.combine(value, datetime.time(0, 0, 0))
-        dt = DateTime.from_pydatetime(value)
-        return cls._struct.pack(dt.days, dt.time_part)
-
-    @classmethod
-    def decode(cls, days, time_part):
-        dt = DateTime(days=days, time_part=time_part)
-        return dt.to_pydatetime()
-
-DateTimeSerializer.instance = DateTimeSerializer()
-
-
-class DateTimeNSerializer(BaseTypeSerializerN, BaseDateTimeSerializer):
-    type = tds_base.SYBDATETIMN
-    subtypes = {
-        4: SmallDateTimeSerializer.instance,
-        8: DateTimeSerializer.instance,
-    }
-
-
-_datetime2_base_date = datetime.datetime(1, 1, 1)
-
-
-class DateType(SqlTypeMetaclass):
-    type = tds_base.SYBMSDATE
-
-    def get_declaration(self):
-        return "DATE"
-
-
-class Date(SqlValueMetaclass):
-    MIN_PYDATE = datetime.date(1, 1, 1)
-    MAX_PYDATE = datetime.date(9999, 12, 31)
-
-    def __init__(self, days):
-        """
-        Creates sql date object
-        @param days: Days since 0001-01-01
-        """
-        self._days = days
-
-    @property
-    def days(self):
-        return self._days
-
-    def to_pydate(self):
-        """
-        Converts sql date to Python date
-        @return: Python date
-        """
-        return (_datetime2_base_date + datetime.timedelta(days=self._days)).date()
-
-    @classmethod
-    def from_pydate(cls, pydate):
-        """
-        Creates sql date object from Python date object.
-        @param pydate: Python date
-        @return: sql date
-        """
-        return cls(days=(datetime.datetime.combine(pydate, datetime.time(0, 0, 0)) - _datetime2_base_date).days)
-
-
-class TimeType(SqlTypeMetaclass):
-    type = tds_base.SYBMSTIME
-
-    def __init__(self, precision=7):
-        self._precision = precision
-
-    @property
-    def precision(self):
-        return self._precision
-
-    def get_declaration(self):
-        return 'TIME({0})'.format(self.precision)
-
-
-class Time(SqlValueMetaclass):
-    def __init__(self, nsec):
-        """
-        Creates sql time object.
-        Maximum precision which sql server supports is 100 nanoseconds.
-        Values more precise than 100 nanoseconds will be truncated.
-        @param nsec: Nanoseconds from 00:00:00
-        """
-        self._nsec = nsec
-
-    @property
-    def nsec(self):
-        return self._nsec
-
-    def to_pytime(self):
-        """
-        Converts sql time object into Python's time object
-        this will truncate nanoseconds to microseconds
-        @return: naive time
-        """
-        nanoseconds = self._nsec
-        hours = nanoseconds // 1000000000 // 60 // 60
-        nanoseconds -= hours * 60 * 60 * 1000000000
-        minutes = nanoseconds // 1000000000 // 60
-        nanoseconds -= minutes * 60 * 1000000000
-        seconds = nanoseconds // 1000000000
-        nanoseconds -= seconds * 1000000000
-        return datetime.time(hours, minutes, seconds, nanoseconds // 1000)
-
-    @classmethod
-    def from_pytime(cls, pytime):
-        """
-        Converts Python time object to sql time object
-        ignoring timezone
-        @param pytime: Python time object
-        @return: sql time object
-        """
-        secs = pytime.hour * 60 * 60 + pytime.minute * 60 + pytime.second
-        nsec = secs * 10 ** 9 + pytime.microsecond * 1000
-        return cls(nsec=nsec)
-
-
-class DateTime2Type(SqlTypeMetaclass):
-    type = tds_base.SYBMSDATETIME2
-
-    def __init__(self, precision=7):
-        self._precision = precision
-
-    @property
-    def precision(self):
-        return self._precision
-
-    def get_declaration(self):
-        return 'DATETIME2({0})'.format(self.precision)
-
-
-class DateTime2(SqlValueMetaclass):
-    type = tds_base.SYBMSDATETIME2
-
-    def __init__(self, date, time):
-        """
-        Creates datetime2 object
-        @param date: sql date object
-        @param time: sql time object
-        """
-        self._date = date
-        self._time = time
-
-    @property
-    def date(self):
-        return self._date
-
-    @property
-    def time(self):
-        return self._time
-
-    def to_pydatetime(self):
-        """
-        Converts datetime2 object into Python's datetime.datetime object
-        @return: naive datetime.datetime
-        """
-        return datetime.datetime.combine(self._date.to_pydate(), self._time.to_pytime())
-
-    @classmethod
-    def from_pydatetime(cls, pydatetime):
-        """
-        Creates sql datetime2 object from Python datetime object
-        ignoring timezone
-        @param pydatetime: Python datetime object
-        @return: sql datetime2 object
-        """
-        return cls(date=Date.from_pydate(pydatetime.date),
-                   time=Time.from_pytime(pydatetime.time))
-
-
-class DateTimeOffsetType(SqlTypeMetaclass):
-    type = tds_base.SYBMSDATETIMEOFFSET
-
-    def __init__(self, precision=7):
-        self._precision = precision
-
-    @property
-    def precision(self):
-        return self._precision
-
-    def get_declaration(self):
-        return 'DATETIMEOFFSET({0})'.format(self.precision)
-
-
-class DateTimeOffset(SqlValueMetaclass):
-    def __init__(self, date, time, offset):
-        """
-        Creates datetime2 object
-        @param date: sql date object in UTC
-        @param time: sql time object in UTC
-        @param offset: time zone offset in minutes
-        """
-        self._date = date
-        self._time = time
-        self._offset = offset
-
-    def to_pydatetime(self):
-        """
-        Converts datetimeoffset object into Python's datetime.datetime object
-        @return: time zone aware datetime.datetime
-        """
-        dt = datetime.datetime.combine(self._date.to_pydate(), self._time.to_pytime())
-        from .tz import FixedOffsetTimezone
-        return dt.replace(tzinfo=_utc).astimezone(FixedOffsetTimezone(self._offset))
-
-
-class BaseDateTime73Serializer(BaseTypeSerializer):
-    def write(self, w, value):
-        raise NotImplementedError
-
-    def write_info(self, w):
-        raise NotImplementedError
-
-    def read(self, r):
-        raise NotImplementedError
-
-    @classmethod
-    def from_stream(cls, r):
-        raise NotImplementedError
-
-    _precision_to_len = {
-        0: 3,
-        1: 3,
-        2: 3,
-        3: 4,
-        4: 4,
-        5: 5,
-        6: 5,
-        7: 5,
-    }
-
-    def _write_time(self, w, t, prec):
-        val = t.nsec // (10 ** (9 - prec))
-        w.write(struct.pack('<Q', val)[:self._precision_to_len[prec]])
-
-    @staticmethod
-    def _read_time(r, size, prec):
-        time_buf = tds_base.readall(r, size)
-        val = _decode_num(time_buf)
-        val *= 10 ** (7 - prec)
-        nanoseconds = val * 100
-        return Time(nsec=nanoseconds)
-
-    @staticmethod
-    def _write_date(w, value):
-        days = value.days
-        buf = struct.pack('<l', days)[:3]
-        w.write(buf)
-
-    @staticmethod
-    def _read_date(r):
-        days = _decode_num(tds_base.readall(r, 3))
-        return Date(days=days)
-
-
-class MsDateSerializer(BasePrimitiveTypeSerializer, BaseDateTime73Serializer):
-    type = tds_base.SYBMSDATE
-    declaration = 'DATE'
-
-    def __init__(self, typ):
-        super(MsDateSerializer, self).__init__()
-        self._typ = typ
-
-    @classmethod
-    def from_stream(cls, r):
-        return cls(DateType())
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-        else:
-            w.put_byte(3)
-            self._write_date(w, Date.from_pydate(value))
-
-    def read_fixed(self, r):
-        return self._read_date(r).to_pydate()
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        return self._read_date(r).to_pydate()
-
-
-class MsTimeSerializer(BaseDateTime73Serializer):
-    type = tds_base.SYBMSTIME
-
-    def __init__(self, typ):
-        super(MsTimeSerializer, self).__init__(precision=typ.precision, size=self._precision_to_len[typ.precision])
-        self._typ = typ
-
-    @classmethod
-    def read_type(cls, r):
-        prec = r.get_byte()
-        return TimeType(precision=prec)
-
-    @classmethod
-    def from_stream(cls, r):
-        return cls(cls.read_type(r))
-
-    def write_info(self, w):
-        w.put_byte(self._typ.precision)
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-        else:
-            if value.tzinfo:
-                if not w.session.use_tz:
-                    raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
-                value = value.astimezone(w.session.use_tz).replace(tzinfo=None)
-            w.put_byte(self.size)
-            self._write_time(w, Time.from_pytime(value), self._typ.precision)
-
-    def read_fixed(self, r, size):
-        res = self._read_time(r, size, self._typ.precision).to_pytime()
-        if r.session.tzinfo_factory is not None:
-            tzinfo = r.session.tzinfo_factory(0)
-            res = res.replace(tzinfo=tzinfo)
-        return res
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        return self.read_fixed(r, size)
-
-
-class DateTime2Serializer(BaseDateTime73Serializer):
-    type = tds_base.SYBMSDATETIME2
-
-    def __init__(self, typ):
-        super(DateTime2Serializer, self).__init__(precision=typ.precision,
-                                                  size=self._precision_to_len[typ.precision] + 3)
-        self._typ = typ
-
-    @classmethod
-    def from_stream(cls, r):
-        prec = r.get_byte()
-        return cls(DateTime2Type(precision=prec))
-
-    def write_info(self, w):
-        w.put_byte(self._typ.precision)
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-        else:
-            if value.tzinfo:
-                if not w.session.use_tz:
-                    raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
-                value = value.astimezone(w.session.use_tz).replace(tzinfo=None)
-            w.put_byte(self.size)
-            self._write_time(w, Time.from_pytime(value), self._typ.precision)
-            self._write_date(w, Date.from_pydate(value))
-
-    def read_fixed(self, r, size):
-        time = self._read_time(r, size - 3, self._typ.precision)
-        date = self._read_date(r)
-        dt = DateTime2(date=date, time=time)
-        res = dt.to_pydatetime()
-        if r.session.tzinfo_factory is not None:
-            tzinfo = r.session.tzinfo_factory(0)
-            res = res.replace(tzinfo=tzinfo)
-        return res
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        return self.read_fixed(r, size)
-
-
-class DateTimeOffsetSerializer(BaseDateTime73Serializer):
-    type = tds_base.SYBMSDATETIMEOFFSET
-
-    def __init__(self, typ):
-        super(DateTimeOffsetSerializer, self).__init__(precision=typ.precision,
-                                                       size=self._precision_to_len[typ.precision] + 5)
-        self._typ = typ
-
-    @classmethod
-    def from_stream(cls, r):
-        prec = r.get_byte()
-        return cls(DateTimeOffsetType(precision=prec))
-
-    def write_info(self, w):
-        w.put_byte(self._typ.precision)
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-        else:
-            utcoffset = value.utcoffset()
-            value = value.astimezone(_utc).replace(tzinfo=None)
-
-            w.put_byte(self.size)
-            self._write_time(w, Time.from_pytime(value), self._typ.precision)
-            self._write_date(w, Date.from_pydate(value))
-            w.put_smallint(int(tds_base.total_seconds(utcoffset)) // 60)
-
-    def read_fixed(self, r, size):
-        time = self._read_time(r, size - 5, self._typ.precision)
-        date = self._read_date(r)
-        offset = r.get_smallint()
-        dt = DateTimeOffset(date=date, time=time, offset=offset)
-        return dt.to_pydatetime()
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        return self.read_fixed(r, size)
-
-
-class MsDecimalSerializer(BaseTypeSerializer):
-    type = tds_base.SYBDECIMAL
-
-    _max_size = 17
-
-    _bytes_per_prec = [
-        #
-        # precision can't be 0 but using a value > 0 assure no
-        # core if for some bug it's 0...
-        #
-        1,
-        5, 5, 5, 5, 5, 5, 5, 5, 5,
-        9, 9, 9, 9, 9, 9, 9, 9, 9, 9,
-        13, 13, 13, 13, 13, 13, 13, 13, 13,
-        17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
-    ]
-
-    _info_struct = struct.Struct('BBB')
-
-    def __init__(self, precision=18, scale=0):
-        super(MsDecimalSerializer, self).__init__(precision=precision,
-                                                  scale=scale,
-                                                  size=self._bytes_per_prec[precision])
-        if precision > 38:
-            raise tds_base.DataError('Precision of decimal value is out of range')
-
-    def __repr__(self):
-        return 'MsDecimal(scale={}, prec={})'.format(self.scale, self.precision)
-
-    @classmethod
-    def from_value(cls, value):
-        sql_type = DecimalType.from_value(value)
-        return cls(scale=sql_type.scale, prec=sql_type.precision)
-
-    @classmethod
-    def from_stream(cls, r):
-        size, prec, scale = r.unpack(cls._info_struct)
-        return cls(scale=scale, precision=prec)
-
-    def write_info(self, w):
-        w.pack(self._info_struct, self.size, self.precision, self.scale)
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-            return
-        if not isinstance(value, decimal.Decimal):
-            value = decimal.Decimal(value)
-        value = value.normalize()
-        scale = self.scale
-        size = self.size
-        w.put_byte(size)
-        val = value
-        positive = 1 if val > 0 else 0
-        w.put_byte(positive)  # sign
-        with decimal.localcontext() as ctx:
-            ctx.prec = 38
-            if not positive:
-                val *= -1
-            size -= 1
-            val *= 10 ** scale
-        for i in range(size):
-            w.put_byte(int(val % 256))
-            val //= 256
-        assert val == 0
-
-    def _decode(self, positive, buf):
-        val = _decode_num(buf)
-        val = decimal.Decimal(val)
-        with decimal.localcontext() as ctx:
-            ctx.prec = 38
-            if not positive:
-                val *= -1
-            val /= 10 ** self._scale
-        return val
-
-    def read_fixed(self, r, size):
-        positive = r.get_byte()
-        buf = tds_base.readall(r, size - 1)
-        return self._decode(positive, buf)
-
-    def read(self, r):
-        size = r.get_byte()
-        if size <= 0:
-            return None
-        return self.read_fixed(r, size)
-
-
-class Money4Serializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBMONEY4
-    declaration = 'SMALLMONEY'
-
-    def read(self, r):
-        return decimal.Decimal(r.get_int()) / 10000
-
-    def write(self, w, val):
-        val = int(val * 10000)
-        w.put_int(val)
-
-Money4Serializer.instance = Money4Serializer()
-
-
-class Money8Serializer(BasePrimitiveTypeSerializer):
-    type = tds_base.SYBMONEY
-    declaration = 'MONEY'
-
-    _struct = struct.Struct('<lL')
-
-    def read(self, r):
-        hi, lo = r.unpack(self._struct)
-        val = hi * (2 ** 32) + lo
-        return decimal.Decimal(val) / 10000
-
-    def write(self, w, val):
-        val *= 10000
-        hi = int(val // (2 ** 32))
-        lo = int(val % (2 ** 32))
-        w.pack(self._struct, hi, lo)
-
-Money8Serializer.instance = Money8Serializer()
-
-
-class MoneyNSerializer(BaseTypeSerializerN):
-    type = tds_base.SYBMONEYN
-
-    subtypes = {
-        4: Money4Serializer.instance,
-        8: Money8Serializer.instance,
-    }
-
-
-class MsUniqueSerializer(BaseTypeSerializer):
-    type = tds_base.SYBUNIQUE
-    declaration = 'UNIQUEIDENTIFIER'
-    instance = None
-
-    def __repr__(self):
-        return 'MsUniqueSerializer()'
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_byte()
-        if size != 16:
-            raise tds_base.InterfaceError('Invalid size of UNIQUEIDENTIFIER field')
-        return cls.instance
-
-    def write_info(self, w):
-        w.put_byte(16)
-
-    def write(self, w, value):
-        if value is None:
-            w.put_byte(0)
-        else:
-            w.put_byte(16)
-            w.write(value.bytes_le)
-
-    @staticmethod
-    def read_fixed(r, size):
-        return uuid.UUID(bytes_le=tds_base.readall(r, size))
-
-    def read(self, r):
-        size = r.get_byte()
-        if size == 0:
-            return None
-        if size != 16:
-            raise tds_base.InterfaceError('Invalid size of UNIQUEIDENTIFIER field')
-        return self.read_fixed(r, size)
-MsUniqueSerializer.instance = MsUniqueSerializer()
-
-
-def _variant_read_str(r, size):
-    collation = r.get_collation()
-    r.get_usmallint()
-    return r.read_str(size, collation.get_codec())
-
-
-def _variant_read_nstr(r, size):
-    r.get_collation()
-    r.get_usmallint()
-    return r.read_str(size, ucs2_codec)
-
-
-def _variant_read_decimal(r, size):
-    prec, scale = r.unpack(VariantSerializer.decimal_info_struct)
-    return MsDecimalSerializer(precision=prec, scale=scale).read_fixed(r, size)
-
-
-def _variant_read_binary(r, size):
-    r.get_usmallint()
-    return tds_base.readall(r, size)
-
-
-class VariantSerializer(BaseTypeSerializer):
-    type = tds_base.SYBVARIANT
-    declaration = 'SQL_VARIANT'
-
-    decimal_info_struct = struct.Struct('BB')
-
-    _type_map = {
-        tds_base.GUIDTYPE: lambda r, size: MsUniqueSerializer.instance.read_fixed(r, size),
-        tds_base.BITTYPE: lambda r, size: BitSerializer.instance.read(r),
-        tds_base.INT1TYPE: lambda r, size: TinyIntSerializer.instance.read(r),
-        tds_base.INT2TYPE: lambda r, size: SmallIntSerializer.instance.read(r),
-        tds_base.INT4TYPE: lambda r, size: IntSerializer.instance.read(r),
-        tds_base.INT8TYPE: lambda r, size: BigIntSerializer.instance.read(r),
-        tds_base.DATETIMETYPE: lambda r, size: DateTimeSerializer.instance.read(r),
-        tds_base.DATETIM4TYPE: lambda r, size: SmallDateTimeSerializer.instance.read(r),
-        tds_base.FLT4TYPE: lambda r, size: RealSerializer.instance.read(r),
-        tds_base.FLT8TYPE: lambda r, size: FloatSerializer.instance.read(r),
-        tds_base.MONEYTYPE: lambda r, size: Money8Serializer.instance.read(r),
-        tds_base.MONEY4TYPE: lambda r, size: Money4Serializer.instance.read(r),
-        tds_base.DATENTYPE: lambda r, size: MsDateSerializer(DateType()).read_fixed(r),
-
-        tds_base.TIMENTYPE: lambda r, size: MsTimeSerializer(TimeType(precision=r.get_byte())).read_fixed(r, size),
-        tds_base.DATETIME2NTYPE: lambda r, size: DateTime2Serializer(
-            DateTime2Type(precision=r.get_byte())).read_fixed(r, size),
-        tds_base.DATETIMEOFFSETNTYPE: lambda r, size: DateTimeOffsetSerializer(
-            DateTimeOffsetType(precision=r.get_byte())).read_fixed(r, size),
-
-        tds_base.BIGVARBINTYPE: _variant_read_binary,
-        tds_base.BIGBINARYTYPE: _variant_read_binary,
-
-        tds_base.NUMERICNTYPE: _variant_read_decimal,
-        tds_base.DECIMALNTYPE: _variant_read_decimal,
-
-        tds_base.BIGVARCHRTYPE: _variant_read_str,
-        tds_base.BIGCHARTYPE: _variant_read_str,
-        tds_base.NVARCHARTYPE: _variant_read_nstr,
-        tds_base.NCHARTYPE: _variant_read_nstr,
-
-    }
-
-    @classmethod
-    def from_stream(cls, r):
-        size = r.get_int()
-        return VariantSerializer(size)
-
-    def write_info(self, w):
-        w.put_int(self.size)
-
-    def read(self, r):
-        size = r.get_int()
-        if size == 0:
-            return None
-
-        type_id = r.get_byte()
-        prop_bytes = r.get_byte()
-        type_factory = self._type_map.get(type_id)
-        if not type_factory:
-            r.session.bad_stream('Variant type invalid', type_id)
-        return type_factory(r, size - prop_bytes - 2)
-
-    def write(self, w, val):
-        if val is None:
-            w.put_int(0)
-            return
-        raise NotImplementedError
-
-
-class TableType(SqlTypeMetaclass):
-    """
-    Used to serialize table valued parameters
-
-    spec: https://msdn.microsoft.com/en-us/library/dd304813.aspx
-    """
-    def __init__(self, typ_schema, typ_name, columns):
-        """
-        @param typ_schema: Schema where TVP type defined
-        @param typ_name: Name of TVP type
-        @param columns: List of column types
-        """
-        if len(typ_schema) > 128:
-            raise ValueError("Schema part of TVP name should be no longer than 128 characters")
-        if len(typ_name) > 128:
-            raise ValueError("Name part of TVP name should be no longer than 128 characters")
-        if columns is not None:
-            if len(columns) > 1024:
-                raise ValueError("TVP cannot have more than 1024 columns")
-            if len(columns) < 1:
-                raise ValueError("TVP must have at least one column")
-        self._typ_dbname = ''  # dbname should always be empty string for TVP according to spec
-        self._typ_schema = typ_schema
-        self._typ_name = typ_name
-        self._columns = columns
-
-    def __repr__(self):
-        return 'TableType(s={},n={},cols={})'.format(
-            self._typ_schema, self._typ_name, repr(self._columns)
-        )
-
-    def get_declaration(self):
-        assert not self._typ_dbname
-        if self._typ_schema:
-            full_name = '{}.{}'.format(self._typ_schema, self._typ_name)
-        else:
-            full_name = self._typ_name
-        return '{} READONLY'.format(full_name)
-
-    @property
-    def typ_schema(self):
-        return self._typ_schema
-
-    @property
-    def typ_name(self):
-        return self._typ_name
-
-    @property
-    def columns(self):
-        return self._columns
-
-
-class TableValuedParam(SqlValueMetaclass):
-    """
-    Used to represent a value of table-valued parameter
-    """
-    def __init__(self, type_name=None, columns=None, rows=None):
-        # parsing type name
-        self._typ_schema = ''
-        self._typ_name = ''
-        if type_name:
-            parts = type_name.split('.')
-            if len(parts) > 2:
-                raise ValueError('Type name should consist of at most 2 parts, e.g. dbo.MyType')
-            self._typ_name = parts[-1]
-            if len(parts) > 1:
-                self._typ_schema = parts[0]
-
-        self._columns = columns
-        self._rows = rows
-
-    @property
-    def typ_name(self):
-        return self._typ_name
-
-    @property
-    def typ_schema(self):
-        return self._typ_schema
-
-    @property
-    def columns(self):
-        return self._columns
-
-    @property
-    def rows(self):
-        return self._rows
-
-    def is_null(self):
-        return self._rows is None
-
-    def peek_row(self):
-        try:
-            rows = iter(self._rows)
-        except TypeError:
-            raise tds_base.DataError('rows should be iterable')
-
-        try:
-            row = next(rows)
-        except StopIteration:
-            # no rows
-            raise tds_base.DataError("Cannot infer columns from rows for TVP because there are no rows")
-        else:
-            # put row back
-            self._rows = itertools.chain([row], rows)
-        return row
-
-
-class TableSerializer(BaseTypeSerializer):
-    """
-    Used to serialize table valued parameters
-
-    spec: https://msdn.microsoft.com/en-us/library/dd304813.aspx
-    """
-
-    type = tds_base.TVPTYPE
-
-    def read(self, r):
-        """ According to spec TDS does not support output TVP values """
-        raise NotImplementedError
-
-    @classmethod
-    def from_stream(cls, r):
-        """ According to spec TDS does not support output TVP values """
-        raise NotImplementedError
-
-    def __init__(self, table_type, columns_serializers):
-        super(TableSerializer, self).__init__()
-        self._table_type = table_type
-        self._columns_serializers = columns_serializers
-
-    @property
-    def table_type(self):
-        return self._table_type
-
-    def __repr__(self):
-        return 'TableSerializer(t={},c={})'.format(
-            repr(self._table_type), repr(self._columns_serializers)
-        )
-
-    def write_info(self, w):
-        """
-        Writes TVP_TYPENAME structure
-
-        spec: https://msdn.microsoft.com/en-us/library/dd302994.aspx
-        @param w: TdsWriter
-        @return:
-        """
-        w.write_b_varchar("")  # db_name, should be empty
-        w.write_b_varchar(self._table_type.typ_schema)
-        w.write_b_varchar(self._table_type.typ_name)
-
-    def write(self, w, val):
-        """
-        Writes remaining part of TVP_TYPE_INFO structure, resuming from TVP_COLMETADATA
-
-        specs:
-        https://msdn.microsoft.com/en-us/library/dd302994.aspx
-        https://msdn.microsoft.com/en-us/library/dd305261.aspx
-        https://msdn.microsoft.com/en-us/library/dd303230.aspx
-
-        @param w: TdsWriter
-        @param val: TableValuedParam or None
-        @return:
-        """
-        if val.is_null():
-            w.put_usmallint(tds_base.TVP_NULL_TOKEN)
-        else:
-            columns = self._table_type.columns
-            w.put_usmallint(len(columns))
-            for i, column in enumerate(columns):
-                w.put_uint(column.column_usertype)
-
-                w.put_usmallint(column.flags)
-
-                # TYPE_INFO structure: https://msdn.microsoft.com/en-us/library/dd358284.aspx
-
-                serializer = self._columns_serializers[i]
-                type_id = serializer.type
-                w.put_byte(type_id)
-                serializer.write_info(w)
-
-                w.write_b_varchar('')  # ColName, must be empty in TVP according to spec
-
-        # here can optionally send TVP_ORDER_UNIQUE and TVP_COLUMN_ORDERING
-        # https://msdn.microsoft.com/en-us/library/dd305261.aspx
-
-        # terminating optional metadata
-        w.put_byte(tds_base.TVP_END_TOKEN)
-
-        # now sending rows using TVP_ROW
-        # https://msdn.microsoft.com/en-us/library/dd305261.aspx
-        if val.rows:
-            for row in val.rows:
-                w.put_byte(tds_base.TVP_ROW_TOKEN)
-                for i, col in enumerate(self._table_type.columns):
-                    if not col.flags & tds_base.TVP_COLUMN_DEFAULT_FLAG:
-                        self._columns_serializers[i].write(w, row[i])
-
-        # terminating rows
-        w.put_byte(tds_base.TVP_END_TOKEN)
-
-
-_type_map = {
-    tds_base.SYBINT1: TinyIntSerializer,
-    tds_base.SYBINT2: SmallIntSerializer,
-    tds_base.SYBINT4: IntSerializer,
-    tds_base.SYBINT8: BigIntSerializer,
-    tds_base.SYBINTN: IntNSerializer,
-    tds_base.SYBBIT: BitSerializer,
-    tds_base.SYBBITN: BitNSerializer,
-    tds_base.SYBREAL: RealSerializer,
-    tds_base.SYBFLT8: FloatSerializer,
-    tds_base.SYBFLTN: FloatNSerializer,
-    tds_base.SYBMONEY4: Money4Serializer,
-    tds_base.SYBMONEY: Money8Serializer,
-    tds_base.SYBMONEYN: MoneyNSerializer,
-    tds_base.XSYBCHAR: VarChar70Serializer,
-    tds_base.XSYBVARCHAR: VarChar70Serializer,
-    tds_base.XSYBNCHAR: NVarChar70Serializer,
-    tds_base.XSYBNVARCHAR: NVarChar70Serializer,
-    tds_base.SYBTEXT: Text70Serializer,
-    tds_base.SYBNTEXT: NText70Serializer,
-    tds_base.SYBMSXML: XmlSerializer,
-    tds_base.XSYBBINARY: VarBinarySerializer,
-    tds_base.XSYBVARBINARY: VarBinarySerializer,
-    tds_base.SYBIMAGE: Image70Serializer,
-    tds_base.SYBNUMERIC: MsDecimalSerializer,
-    tds_base.SYBDECIMAL: MsDecimalSerializer,
-    tds_base.SYBVARIANT: VariantSerializer,
-    tds_base.SYBMSDATE: MsDateSerializer,
-    tds_base.SYBMSTIME: MsTimeSerializer,
-    tds_base.SYBMSDATETIME2: DateTime2Serializer,
-    tds_base.SYBMSDATETIMEOFFSET: DateTimeOffsetSerializer,
-    tds_base.SYBDATETIME4: SmallDateTimeSerializer,
-    tds_base.SYBDATETIME: DateTimeSerializer,
-    tds_base.SYBDATETIMN: DateTimeNSerializer,
-    tds_base.SYBUNIQUE: MsUniqueSerializer,
-}
-
-_type_map71 = _type_map.copy()
-_type_map71.update({
-    tds_base.XSYBCHAR: VarChar71Serializer,
-    tds_base.XSYBNCHAR: NVarChar71Serializer,
-    tds_base.XSYBVARCHAR: VarChar71Serializer,
-    tds_base.XSYBNVARCHAR: NVarChar71Serializer,
-    tds_base.SYBTEXT: Text71Serializer,
-    tds_base.SYBNTEXT: NText71Serializer,
-})
-
-_type_map72 = _type_map.copy()
-_type_map72.update({
-    tds_base.XSYBCHAR: VarChar72Serializer,
-    tds_base.XSYBNCHAR: NVarChar72Serializer,
-    tds_base.XSYBVARCHAR: VarChar72Serializer,
-    tds_base.XSYBNVARCHAR: NVarChar72Serializer,
-    tds_base.SYBTEXT: Text72Serializer,
-    tds_base.SYBNTEXT: NText72Serializer,
-    tds_base.XSYBBINARY: VarBinarySerializer72,
-    tds_base.XSYBVARBINARY: VarBinarySerializer72,
-    tds_base.SYBIMAGE: Image72Serializer,
-    tds_base.UDTTYPE: UDT72Serializer,
-})
-
-_type_map73 = _type_map72.copy()
-_type_map73.update({
-    tds_base.TVPTYPE: TableSerializer,
-})
-
-
-def sql_type_by_declaration(declaration):
-    return _declarations_parser.parse(declaration)
-
-
-class SerializerFactory(object):
-    """
-    Factory class for TDS data types
-    """
-    def __init__(self, tds_ver):
-        self._tds_ver = tds_ver
-        if self._tds_ver >= tds_base.TDS73:
-            self._type_map = _type_map73
-        elif self._tds_ver >= tds_base.TDS72:
-            self._type_map = _type_map72
-        elif self._tds_ver >= tds_base.TDS71:
-            self._type_map = _type_map71
-        else:
-            self._type_map = _type_map
-
-    def get_type_serializer(self, tds_type_id):
-        type_class = self._type_map.get(tds_type_id)
-        if not type_class:
-            raise tds_base.InterfaceError('Invalid type id {}'.format(tds_type_id))
-        return type_class
-
-    def long_binary_type(self):
-        if self._tds_ver >= tds_base.TDS72:
-            return VarBinaryMaxType()
-        else:
-            return ImageType()
-
-    def long_varchar_type(self):
-        if self._tds_ver >= tds_base.TDS72:
-            return VarCharMaxType()
-        else:
-            return TextType()
-
-    def long_string_type(self):
-        if self._tds_ver >= tds_base.TDS72:
-            return NVarCharMaxType()
-        else:
-            return NTextType()
-
-    def datetime(self, precision):
-        if self._tds_ver >= tds_base.TDS72:
-            return DateTime2Type(precision=precision)
-        else:
-            return DateTimeType()
-
-    def has_datetime_with_tz(self):
-        return self._tds_ver >= tds_base.TDS72
-
-    def datetime_with_tz(self, precision):
-        if self._tds_ver >= tds_base.TDS72:
-            return DateTimeOffsetType(precision=precision)
-        else:
-            raise tds_base.DataError('Given TDS version does not support DATETIMEOFFSET type')
-
-    def date(self):
-        if self._tds_ver >= tds_base.TDS72:
-            return DateType()
-        else:
-            return DateTimeType()
-
-    def time(self, precision):
-        if self._tds_ver >= tds_base.TDS72:
-            return TimeType(precision=precision)
-        else:
-            raise tds_base.DataError('Given TDS version does not support TIME type')
-
-    def serializer_by_declaration(self, declaration, connection):
-        sql_type = sql_type_by_declaration(declaration)
-        return self.serializer_by_type(sql_type=sql_type, collation=connection.collation)
-
-    def serializer_by_type(self, sql_type, collation=raw_collation):
-        typ = sql_type
-        if isinstance(typ, BitType):
-            return BitNSerializer(typ)
-        elif isinstance(typ, TinyIntType):
-            return IntNSerializer(typ)
-        elif isinstance(typ, SmallIntType):
-            return IntNSerializer(typ)
-        elif isinstance(typ, IntType):
-            return IntNSerializer(typ)
-        elif isinstance(typ, BigIntType):
-            return IntNSerializer(typ)
-        elif isinstance(typ, RealType):
-            return FloatNSerializer(size=4)
-        elif isinstance(typ, FloatType):
-            return FloatNSerializer(size=8)
-        elif isinstance(typ, SmallMoneyType):
-            return self._type_map[tds_base.SYBMONEYN](size=4)
-        elif isinstance(typ, MoneyType):
-            return self._type_map[tds_base.SYBMONEYN](size=8)
-        elif isinstance(typ, CharType):
-            return self._type_map[tds_base.XSYBCHAR](size=typ.size, collation=collation)
-        elif isinstance(typ, VarCharType):
-            return self._type_map[tds_base.XSYBVARCHAR](size=typ.size, collation=collation)
-        elif isinstance(typ, VarCharMaxType):
-            return VarCharMaxSerializer(collation=collation)
-        elif isinstance(typ, NCharType):
-            return self._type_map[tds_base.XSYBNCHAR](size=typ.size, collation=collation)
-        elif isinstance(typ, NVarCharType):
-            return self._type_map[tds_base.XSYBNVARCHAR](size=typ.size, collation=collation)
-        elif isinstance(typ, NVarCharMaxType):
-            return NVarCharMaxSerializer(collation=collation)
-        elif isinstance(typ, TextType):
-            return self._type_map[tds_base.SYBTEXT](collation=collation)
-        elif isinstance(typ, NTextType):
-            return self._type_map[tds_base.SYBNTEXT](collation=collation)
-        elif isinstance(typ, XmlType):
-            return self._type_map[tds_base.SYBMSXML]()
-        elif isinstance(typ, BinaryType):
-            return self._type_map[tds_base.XSYBBINARY]()
-        elif isinstance(typ, VarBinaryType):
-            return self._type_map[tds_base.XSYBVARBINARY](size=typ.size)
-        elif isinstance(typ, VarBinaryMaxType):
-            return VarBinarySerializerMax()
-        elif isinstance(typ, ImageType):
-            return self._type_map[tds_base.SYBIMAGE]()
-        elif isinstance(typ, DecimalType):
-            return self._type_map[tds_base.SYBDECIMAL](scale=typ.scale, precision=typ.precision)
-        elif isinstance(typ, VariantType):
-            return self._type_map[tds_base.SYBVARIANT](size=0)
-        elif isinstance(typ, SmallDateTimeType):
-            return self._type_map[tds_base.SYBDATETIMN](size=4)
-        elif isinstance(typ, DateTimeType):
-            return self._type_map[tds_base.SYBDATETIMN](size=8)
-        elif isinstance(typ, DateType):
-            return self._type_map[tds_base.SYBMSDATE](typ)
-        elif isinstance(typ, TimeType):
-            return self._type_map[tds_base.SYBMSTIME](typ)
-        elif isinstance(typ, DateTime2Type):
-            return self._type_map[tds_base.SYBMSDATETIME2](typ)
-        elif isinstance(typ, DateTimeOffsetType):
-            return self._type_map[tds_base.SYBMSDATETIMEOFFSET](typ)
-        elif isinstance(typ, UniqueIdentifierType):
-            return self._type_map[tds_base.SYBUNIQUE]()
-        elif isinstance(typ, TableType):
-            columns_serializers = None
-            if typ.columns is not None:
-                columns_serializers = [self.serializer_by_type(col.type) for col in typ.columns]
-            return TableSerializer(table_type=typ, columns_serializers=columns_serializers)
-        else:
-            raise ValueError('Cannot map type {} to serializer.'.format(typ))
-
-
-class DeclarationsParser(object):
-    def __init__(self):
-        declaration_parsers = [
-            ('bit', BitType),
-            ('tinyint', TinyIntType),
-            ('smallint', SmallIntType),
-            ('(?:int|integer)', IntType),
-            ('bigint', BigIntType),
-            ('real', RealType),
-            ('(?:float|double precision)', FloatType),
-            ('(?:char|character)', CharType),
-            (r'(?:char|character)\((\d+)\)', lambda size_str: CharType(size=int(size_str))),
-            (r'(?:varchar|char(?:|acter)\s+varying)', VarCharType),
-            (r'(?:varchar|char(?:|acter)\s+varying)\((\d+)\)', lambda size_str: VarCharType(size=int(size_str))),
-            (r'varchar\(max\)', VarCharMaxType),
-            (r'(?:nchar|national\s+(?:char|character))', NCharType),
-            (r'(?:nchar|national\s+(?:char|character))\((\d+)\)', lambda size_str: NCharType(size=int(size_str))),
-            (r'(?:nvarchar|national\s+(?:char|character)\s+varying)', NVarCharType),
-            (r'(?:nvarchar|national\s+(?:char|character)\s+varying)\((\d+)\)',
-             lambda size_str: NVarCharType(size=int(size_str))),
-            (r'nvarchar\(max\)', NVarCharMaxType),
-            ('xml', XmlType),
-            ('text', TextType),
-            (r'(?:ntext|national\s+text)', NTextType),
-            ('binary', BinaryType),
-            ('binary\((\d+)\)', lambda size_str: BinaryType(size=int(size_str))),
-            ('(?:varbinary|binary varying)', VarBinaryType),
-            (r'(?:varbinary|binary varying)\((\d+)\)', lambda size_str: VarBinaryType(size=int(size_str))),
-            (r'varbinary\(max\)', VarBinaryMaxType),
-            ('image', ImageType),
-            ('smalldatetime', SmallDateTimeType),
-            ('datetime', DateTimeType),
-            ('date', DateType),
-            (r'time', TimeType),
-            (r'time\((\d+)\)', lambda precision_str: TimeType(precision=int(precision_str))),
-            ('datetime2', DateTime2Type),
-            (r'datetime2\((\d+)\)', lambda precision_str: DateTime2Type(precision=int(precision_str))),
-            ('datetimeoffset', DateTimeOffsetType),
-            (r'datetimeoffset\((\d+)\)',
-             lambda precision_str: DateTimeOffsetType(precision=int(precision_str))),
-            ('(?:decimal|dec|numeric)', DecimalType),
-            ('(?:decimal|dec|numeric)\((\d+)\)',
-             lambda precision_str: DecimalType(precision=int(precision_str))),
-            ('(?:decimal|dec|numeric)\((\d+), (\d+)\)',
-             lambda precision_str, scale_str: DecimalType(precision=int(precision_str), scale=int(scale_str))),
-            ('smallmoney', SmallMoneyType),
-            ('money', MoneyType),
-            ('uniqueidentifier', UniqueIdentifierType),
-            ('sql_variant', VariantType),
-        ]
-        self._compiled = [(re.compile(r'^' + regex + '$', re.IGNORECASE), constructor)
-                          for regex, constructor in declaration_parsers]
-
-    def parse(self, declaration):
-        """
-        Parse sql type declaration, e.g. varchar(10) and return instance of corresponding type class,
-        e.g. VarCharType(10)
-
-        @param declaration: Sql declaration to parse, e.g. varchar(10)
-        @return: instance of SqlTypeMetaclass
-        """
-        declaration = declaration.strip()
-        for regex, constructor in self._compiled:
-            m = regex.match(declaration)
-            if m:
-                return constructor(*m.groups())
-        raise ValueError('Unable to parse type declaration', declaration)
-
-
-_declarations_parser = DeclarationsParser()
-
-
-class TdsTypeInferrer(object):
-    def __init__(self, type_factory, collation=None, bytes_to_unicode=False, allow_tz=False):
-        """
-        Class used to do TDS type inference
-
-        :param type_factory: Instance of TypeFactory
-        :param collation: Collation to use for strings
-        :param bytes_to_unicode: Treat bytes type as unicode string
-        :param allow_tz: Allow usage of DATETIMEOFFSET type
-        """
-        self._type_factory = type_factory
-        self._collation = collation
-        self._bytes_to_unicode = bytes_to_unicode
-        self._allow_tz = allow_tz
-
-    def from_value(self, value):
-        """ Function infers TDS type from Python value.
-
-        :param value: value from which to infer TDS type
-        :return: An instance of subclass of :class:`BaseType`
-        """
-        if value is None:
-            sql_type = NVarCharType(size=1)
-        else:
-            sql_type = self._from_class_value(value, type(value))
-        return sql_type
-
-    def from_class(self, cls):
-        """ Function infers TDS type from Python class.
-
-        :param cls: Class from which to infer type
-        :return: An instance of subclass of :class:`BaseType`
-        """
-        return self._from_class_value(None, cls)
-
-    def _from_class_value(self, value, value_type):
-        type_factory = self._type_factory
-        bytes_to_unicode = self._bytes_to_unicode
-        allow_tz = self._allow_tz
-
-        if issubclass(value_type, bool):
-            return BitType()
-        elif issubclass(value_type, six.integer_types):
-            if value is None:
-                return IntType()
-            if -2 ** 31 <= value <= 2 ** 31 - 1:
-                return IntType()
-            elif -2 ** 63 <= value <= 2 ** 63 - 1:
-                return BigIntType()
-            elif -10 ** 38 + 1 <= value <= 10 ** 38 - 1:
-                return DecimalType(precision=38)
-            else:
-                return VarCharMaxType()
-        elif issubclass(value_type, float):
-            return FloatType()
-        elif issubclass(value_type, Binary):
-            if value is None or len(value) <= 8000:
-                return VarBinaryType(size=8000)
-            else:
-                return type_factory.long_binary_type()
-        elif issubclass(value_type, six.binary_type):
-            if bytes_to_unicode:
-                return type_factory.long_string_type()
-            else:
-                return type_factory.long_varchar_type()
-        elif issubclass(value_type, six.string_types):
-            return type_factory.long_string_type()
-        elif issubclass(value_type, datetime.datetime):
-            if value and value.tzinfo and allow_tz:
-                return type_factory.datetime_with_tz(precision=6)
-            else:
-                return type_factory.datetime(precision=6)
-        elif issubclass(value_type, datetime.date):
-            return type_factory.date()
-        elif issubclass(value_type, datetime.time):
-            return type_factory.time(precision=6)
-        elif issubclass(value_type, decimal.Decimal):
-            if value is None:
-                return DecimalType()
-            else:
-                return DecimalType.from_value(value)
-        elif issubclass(value_type, uuid.UUID):
-            return UniqueIdentifierType()
-        elif issubclass(value_type, TableValuedParam):
-            columns = value.columns
-            rows = value.rows
-            if columns is None:
-                # trying to auto detect columns using data from first row
-                if rows is None:
-                    # rows are not present too, this means
-                    # entire tvp has value of NULL
-                    pass
-                else:
-                    # use first row to infer types of columns
-                    row = value.peek_row()
-                    columns = []
-                    try:
-                        cell_iter = iter(row)
-                    except TypeError:
-                        raise tds_base.DataError('Each row in table should be an iterable')
-                    for cell in cell_iter:
-                        if isinstance(cell, TableValuedParam):
-                            raise tds_base.DataError('TVP type cannot have nested TVP types')
-                        col_type = self.from_value(cell)
-                        col = tds_base.Column(type=col_type)
-                        columns.append(col)
-
-            return TableType(typ_schema=value.typ_schema, typ_name=value.typ_name, columns=columns)
-        else:
-            raise tds_base.DataError('Cannot infer TDS type from Python value: {!r}'.format(value))
+import itertools
+import datetime
+import decimal
+import struct
+import re
+import uuid
+import six
+import functools
+
+from . import tds_base
+from .collate import ucs2_codec, raw_collation
+from . import tz
+
+
+_flt4_struct = struct.Struct('f')
+_flt8_struct = struct.Struct('d')
+_utc = tz.utc
+
+
+def _applytz(dt, tzinfo):
+    if not tzinfo:
+        return dt
+    dt = dt.replace(tzinfo=tzinfo)
+    return dt
+
+
+def _decode_num(buf):
+    """ Decodes little-endian integer from buffer
+
+    Buffer can be of any size
+    """
+    return functools.reduce(lambda acc, val: acc * 256 + tds_base.my_ord(val), reversed(buf), 0)
+
+
+class PlpReader(object):
+    """ Partially length prefixed reader
+
+    Spec: http://msdn.microsoft.com/en-us/library/dd340469.aspx
+    """
+    def __init__(self, r):
+        """
+        :param r: An instance of :class:`_TdsReader`
+        """
+        self._rdr = r
+        size = r.get_uint8()
+        self._size = size
+
+    def is_null(self):
+        """
+        :return: True if stored value is NULL
+        """
+        return self._size == tds_base.PLP_NULL
+
+    def is_unknown_len(self):
+        """
+        :return: True if total size is unknown upfront
+        """
+        return self._size == tds_base.PLP_UNKNOWN
+
+    def size(self):
+        """
+        :return: Total size in bytes if is_uknown_len and is_null are both False
+        """
+        return self._size
+
+    def chunks(self):
+        """ Generates chunks from stream, each chunk is an instace of bytes.
+        """
+        if self.is_null():
+            return
+        total = 0
+        while True:
+            chunk_len = self._rdr.get_uint()
+            if chunk_len == 0:
+                if not self.is_unknown_len() and total != self._size:
+                    msg = "PLP actual length (%d) doesn't match reported length (%d)" % (total, self._size)
+                    self._rdr.session.bad_stream(msg)
+
+                return
+
+            total += chunk_len
+            left = chunk_len
+            while left:
+                buf = self._rdr.read(left)
+                yield buf
+                left -= len(buf)
+
+
+class SqlTypeMetaclass(tds_base.CommonEqualityMixin):
+    def __repr__(self):
+        return '<sqltype:{}>'.format(self.get_declaration())
+
+    def get_declaration(self):
+        raise NotImplementedError()
+
+
+class ImageType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'IMAGE'
+
+
+class BinaryType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'BINARY({})'.format(self._size)
+
+
+class VarBinaryType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'VARBINARY({})'.format(self._size)
+
+
+class VarBinaryMaxType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'VARBINARY(MAX)'
+
+
+class CharType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'CHAR({})'.format(self._size)
+
+
+class VarCharType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'VARCHAR({})'.format(self._size)
+
+
+class VarCharMaxType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'VARCHAR(MAX)'
+
+
+class NCharType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'NCHAR({})'.format(self._size)
+
+
+class NVarCharType(SqlTypeMetaclass):
+    def __init__(self, size=30):
+        self._size = size
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_declaration(self):
+        return 'NVARCHAR({})'.format(self._size)
+
+
+class NVarCharMaxType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'NVARCHAR(MAX)'
+
+
+class TextType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'TEXT'
+
+
+class NTextType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'NTEXT'
+
+
+class XmlType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'XML'
+
+
+class SmallMoneyType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'SMALLMONEY'
+
+
+class MoneyType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'MONEY'
+
+
+class DecimalType(SqlTypeMetaclass):
+    def __init__(self, precision=18, scale=0):
+        self._precision = precision
+        self._scale = scale
+
+    @classmethod
+    def from_value(cls, value):
+        if not (-10 ** 38 + 1 <= value <= 10 ** 38 - 1):
+            raise tds_base.DataError('Decimal value is out of range')
+        value = value.normalize()
+        _, digits, exp = value.as_tuple()
+        if exp > 0:
+            scale = 0
+            prec = len(digits) + exp
+        else:
+            scale = -exp
+            prec = max(len(digits), scale)
+        return cls(precision=prec, scale=scale)
+
+    @property
+    def precision(self):
+        return self._precision
+
+    @property
+    def scale(self):
+        return self._scale
+
+    def get_declaration(self):
+        return 'DECIMAL({}, {})'.format(self._precision, self._scale)
+
+
+class UniqueIdentifierType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'UNIQUEIDENTIFIER'
+
+
+class VariantType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'SQL_VARIANT'
+
+
+class SqlValueMetaclass(tds_base.CommonEqualityMixin):
+    pass
+
+
+class BaseTypeSerializer(tds_base.CommonEqualityMixin):
+    """ Base type for TDS data types.
+
+    All TDS types should derive from it.
+    In addition actual types should provide the following:
+
+    - type - class variable storing type identifier
+    """
+    type = 0
+
+    def __init__(self, precision=None, scale=None, size=None):
+        self._precision = precision
+        self._scale = scale
+        self._size = size
+
+    @property
+    def precision(self):
+        return self._precision
+
+    @property
+    def scale(self):
+        return self._scale
+
+    @property
+    def size(self):
+        return self._size
+
+    def get_typeid(self):
+        """ Returns type identifier of type. """
+        return self.type
+
+    @classmethod
+    def from_stream(cls, r):
+        """ Class method that reads and returns a type instance.
+
+        :param r: An instance of :class:`_TdsReader` to read type from.
+
+        Should be implemented in actual types.
+        """
+        raise NotImplementedError
+
+    def write_info(self, w):
+        """ Writes type info into w stream.
+
+        :param w: An instance of :class:`_TdsWriter` to write into.
+
+        Should be symmetrical to from_stream method.
+        Should be implemented in actual types.
+        """
+        raise NotImplementedError
+
+    def write(self, w, value):
+        """ Writes type's value into stream
+
+        :param w: An instance of :class:`_TdsWriter` to write into.
+        :param value: A value to be stored, should be compatible with the type
+
+        Should be implemented in actual types.
+        """
+        raise NotImplementedError
+
+    def read(self, r):
+        """ Reads value from the stream.
+
+        :param r: An instance of :class:`_TdsReader` to read value from.
+        :return: A read value.
+
+        Should be implemented in actual types.
+        """
+        raise NotImplementedError
+
+
+class BasePrimitiveTypeSerializer(BaseTypeSerializer):
+    """ Base type for primitive TDS data types.
+
+    Primitive type is a fixed size type with no type arguments.
+    All primitive TDS types should derive from it.
+    In addition actual types should provide the following:
+
+    - type - class variable storing type identifier
+    - declaration - class variable storing name of sql type
+    - isntance - class variable storing instance of class
+    """
+
+    def write(self, w, value):
+        raise NotImplementedError
+
+    def read(self, r):
+        raise NotImplementedError
+
+    instance = None
+
+    @classmethod
+    def from_stream(cls, r):
+        return cls.instance
+
+    def write_info(self, w):
+        pass
+
+
+class BaseTypeSerializerN(BaseTypeSerializer):
+    """ Base type for nullable TDS data types.
+
+    All nullable TDS types should derive from it.
+    In addition actual types should provide the following:
+
+    - type - class variable storing type identifier
+    - subtypes - class variable storing dict {subtype_size: subtype_instance}
+    """
+    subtypes = {}
+
+    def __init__(self, size):
+        super(BaseTypeSerializerN, self).__init__(size=size)
+        assert size in self.subtypes
+        self._current_subtype = self.subtypes[size]
+
+    def get_typeid(self):
+        return self._current_subtype.get_typeid()
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_byte()
+        if size not in cls.subtypes:
+            raise tds_base.InterfaceError('Invalid %s size' % cls.type, size)
+        return cls(size)
+
+    def write_info(self, w):
+        w.put_byte(self.size)
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        if size not in self.subtypes:
+            raise r.session.bad_stream('Invalid %s size' % self.type, size)
+        return self.subtypes[size].read(r)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_byte(0)
+            return
+        w.put_byte(self.size)
+        self._current_subtype.write(w, val)
+
+
+class BitType(SqlTypeMetaclass):
+    type = tds_base.SYBBITN
+
+    def get_declaration(self):
+        return 'BIT'
+
+
+class TinyIntType(SqlTypeMetaclass):
+    type = tds_base.SYBINTN
+    size = 1
+
+    def get_declaration(self):
+        return 'TINYINT'
+
+
+class SmallIntType(SqlTypeMetaclass):
+    type = tds_base.SYBINTN
+    size = 2
+
+    def get_declaration(self):
+        return 'SMALLINT'
+
+
+class IntType(SqlTypeMetaclass):
+    type = tds_base.SYBINTN
+    size = 4
+
+    def get_declaration(self):
+        return 'INT'
+
+
+class BigIntType(SqlTypeMetaclass):
+    type = tds_base.SYBINTN
+    size = 8
+
+    def get_declaration(self):
+        return 'BIGINT'
+
+
+class RealType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'REAL'
+
+
+class FloatType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'FLOAT'
+
+
+class BitSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBBIT
+    declaration = 'BIT'
+
+    def write(self, w, value):
+        w.put_byte(1 if value else 0)
+
+    def read(self, r):
+        return bool(r.get_byte())
+
+BitSerializer.instance = BitSerializer()
+
+
+class BitNSerializer(BaseTypeSerializerN):
+    type = tds_base.SYBBITN
+    subtypes = {1: BitSerializer.instance}
+
+    def __init__(self, typ):
+        super(BitNSerializer, self).__init__(size=1)
+        self._typ = typ
+
+    def __repr__(self):
+        return 'BitNSerializer({})'.format(self._typ)
+
+
+BitNSerializer.instance = BitNSerializer(BitType())
+
+
+class TinyIntSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBINT1
+    declaration = 'TINYINT'
+
+    def write(self, w, val):
+        w.put_byte(val)
+
+    def read(self, r):
+        return r.get_byte()
+
+TinyIntSerializer.instance = TinyIntSerializer()
+
+
+class SmallIntSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBINT2
+    declaration = 'SMALLINT'
+
+    def write(self, w, val):
+        w.put_smallint(val)
+
+    def read(self, r):
+        return r.get_smallint()
+
+SmallIntSerializer.instance = SmallIntSerializer()
+
+
+class IntSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBINT4
+    declaration = 'INT'
+
+    def write(self, w, val):
+        w.put_int(val)
+
+    def read(self, r):
+        return r.get_int()
+
+IntSerializer.instance = IntSerializer()
+
+
+class BigIntSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBINT8
+    declaration = 'BIGINT'
+
+    def write(self, w, val):
+        w.put_int8(val)
+
+    def read(self, r):
+        return r.get_int8()
+
+BigIntSerializer.instance = BigIntSerializer()
+
+
+class IntNSerializer(BaseTypeSerializerN):
+    type = tds_base.SYBINTN
+
+    subtypes = {
+        1: TinyIntSerializer.instance,
+        2: SmallIntSerializer.instance,
+        4: IntSerializer.instance,
+        8: BigIntSerializer.instance,
+    }
+
+    type_by_size = {
+        1: TinyIntType(),
+        2: SmallIntType(),
+        4: IntType(),
+        8: BigIntType(),
+    }
+
+    def __init__(self, typ):
+        super(IntNSerializer, self).__init__(size=typ.size)
+        self._typ = typ
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_byte()
+        if size not in cls.subtypes:
+            raise tds_base.InterfaceError('Invalid %s size' % cls.type, size)
+        return cls(cls.type_by_size[size])
+
+    def __repr__(self):
+        return 'IntN({})'.format(self.size)
+
+
+class RealSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBREAL
+    declaration = 'REAL'
+
+    def write(self, w, val):
+        w.pack(_flt4_struct, val)
+
+    def read(self, r):
+        return r.unpack(_flt4_struct)[0]
+
+RealSerializer.instance = RealSerializer()
+
+
+class FloatSerializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBFLT8
+    declaration = 'FLOAT'
+
+    def write(self, w, val):
+        w.pack(_flt8_struct, val)
+
+    def read(self, r):
+        return r.unpack(_flt8_struct)[0]
+
+FloatSerializer.instance = FloatSerializer()
+
+
+class FloatNSerializer(BaseTypeSerializerN):
+    type = tds_base.SYBFLTN
+
+    subtypes = {
+        4: RealSerializer.instance,
+        8: FloatSerializer.instance,
+    }
+
+
+class VarChar(SqlValueMetaclass):
+    def __init__(self, val, collation=raw_collation):
+        self._val = val
+        self._collation = collation
+
+    @property
+    def collation(self):
+        return self._collation
+
+    @property
+    def val(self):
+        return self._val
+
+    def __str__(self):
+        return self._val
+
+
+class VarChar70Serializer(BaseTypeSerializer):
+    type = tds_base.XSYBVARCHAR
+
+    def __init__(self, size, collation=raw_collation, codec=None):
+        super(VarChar70Serializer, self).__init__(size=size)
+        self._collation = collation
+        if codec:
+            self._codec = codec
+        else:
+            self._codec = collation.get_codec()
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_smallint()
+        return cls(size, codec=r.session.conn.server_codec)
+
+    def write_info(self, w):
+        w.put_smallint(self.size)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_smallint(-1)
+        else:
+            if w._tds._tds._login.bytes_to_unicode:
+                val = tds_base.force_unicode(val)
+            if isinstance(val, six.text_type):
+                val, _ = self._codec.encode(val)
+            w.put_smallint(len(val))
+            w.write(val)
+
+    def read(self, r):
+        size = r.get_smallint()
+        if size < 0:
+            return None
+        if r._session._tds._login.bytes_to_unicode:
+            return r.read_str(size, self._codec)
+        else:
+            return tds_base.readall(r, size)
+
+
+class VarChar71Serializer(VarChar70Serializer):
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_smallint()
+        collation = r.get_collation()
+        return cls(size, collation)
+
+    def write_info(self, w):
+        super(VarChar71Serializer, self).write_info(w)
+        w.put_collation(self._collation)
+
+
+class VarChar72Serializer(VarChar71Serializer):
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        collation = r.get_collation()
+        if size == 0xffff:
+            return VarCharMaxSerializer(collation)
+        return cls(size, collation)
+
+
+class VarCharMaxSerializer(VarChar72Serializer):
+    def __init__(self, collation=raw_collation):
+        super(VarChar72Serializer, self).__init__(0, collation)
+
+    def write_info(self, w):
+        w.put_usmallint(tds_base.PLP_MARKER)
+        w.put_collation(self._collation)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_uint8(tds_base.PLP_NULL)
+        else:
+            if w._tds._tds._login.bytes_to_unicode:
+                val = tds_base.force_unicode(val)
+            if isinstance(val, six.text_type):
+                val, _ = self._codec.encode(val)
+            w.put_int8(len(val))
+            if len(val) > 0:
+                w.put_int(len(val))
+                w.write(val)
+            w.put_int(0)
+
+    def read(self, r):
+        login = r._session._tds._login
+        r = PlpReader(r)
+        if r.is_null():
+            return None
+        if login.bytes_to_unicode:
+            return ''.join(tds_base.iterdecode(r.chunks(), self._codec))
+        else:
+            return six.b('').join(r.chunks())
+
+
+class NVarChar70Serializer(BaseTypeSerializer):
+    type = tds_base.XSYBNVARCHAR
+
+    def __init__(self, size, collation=raw_collation):
+        super(NVarChar70Serializer, self).__init__(size=size)
+        self._collation = collation
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        return cls(size / 2)
+
+    def write_info(self, w):
+        w.put_usmallint(self.size * 2)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_usmallint(0xffff)
+        else:
+            if isinstance(val, bytes):
+                val = tds_base.force_unicode(val)
+            buf, _ = ucs2_codec.encode(val)
+            l = len(buf)
+            w.put_usmallint(l)
+            w.write(buf)
+
+    def read(self, r):
+        size = r.get_usmallint()
+        if size == 0xffff:
+            return None
+        return r.read_str(size, ucs2_codec)
+
+
+class NVarChar71Serializer(NVarChar70Serializer):
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        collation = r.get_collation()
+        return cls(size / 2, collation)
+
+    def write_info(self, w):
+        super(NVarChar71Serializer, self).write_info(w)
+        w.put_collation(self._collation)
+
+
+class NVarChar72Serializer(NVarChar71Serializer):
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        collation = r.get_collation()
+        if size == 0xffff:
+            return NVarCharMaxSerializer(collation=collation)
+        return cls(size / 2, collation=collation)
+
+
+class NVarCharMaxSerializer(NVarChar72Serializer):
+    def __init__(self, collation=raw_collation):
+        super(NVarCharMaxSerializer, self).__init__(size=-1, collation=collation)
+
+    def __repr__(self):
+        return 'NVarCharMax(s={},c={})'.format(self.size, repr(self._collation))
+
+    def get_typeid(self):
+        return tds_base.SYBNTEXT
+
+    def write_info(self, w):
+        w.put_usmallint(tds_base.PLP_MARKER)
+        w.put_collation(self._collation)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_uint8(tds_base.PLP_NULL)
+        else:
+            if isinstance(val, bytes):
+                val = tds_base.force_unicode(val)
+            val, _ = ucs2_codec.encode(val)
+            w.put_uint8(len(val))
+            if len(val) > 0:
+                w.put_uint(len(val))
+                w.write(val)
+            w.put_uint(0)
+
+    def read(self, r):
+        r = PlpReader(r)
+        if r.is_null():
+            return None
+        res = ''.join(tds_base.iterdecode(r.chunks(), ucs2_codec))
+        return res
+
+
+class XmlSerializer(NVarCharMaxSerializer):
+    type = tds_base.SYBMSXML
+    declaration = 'XML'
+
+    def __init__(self, schema=None):
+        super(XmlSerializer, self).__init__(0)
+        self._schema = schema or {}
+
+    def __repr__(self):
+        return 'XmlSerializer(schema={})'.format(repr(self._schema))
+
+    def get_typeid(self):
+        return self.type
+
+    @classmethod
+    def from_stream(cls, r):
+        has_schema = r.get_byte()
+        schema = {}
+        if has_schema:
+            schema['dbname'] = r.read_ucs2(r.get_byte())
+            schema['owner'] = r.read_ucs2(r.get_byte())
+            schema['collection'] = r.read_ucs2(r.get_smallint())
+        return cls(schema)
+
+    def write_info(self, w):
+        if self._schema:
+            w.put_byte(1)
+            w.put_byte(len(self._schema['dbname']))
+            w.write_ucs2(self._schema['dbname'])
+            w.put_byte(len(self._schema['owner']))
+            w.write_ucs2(self._schema['owner'])
+            w.put_usmallint(len(self._schema['collection']))
+            w.write_ucs2(self._schema['collection'])
+        else:
+            w.put_byte(0)
+
+
+class Text70Serializer(BaseTypeSerializer):
+    type = tds_base.SYBTEXT
+    declaration = 'TEXT'
+
+    def __init__(self, size=0, table_name='', collation=raw_collation, codec=None):
+        super(Text70Serializer, self).__init__(size=size)
+        self._table_name = table_name
+        self._collation = collation
+        if codec:
+            self._codec = codec
+        else:
+            self._codec = collation.get_codec()
+
+    def __repr__(self):
+        return 'Text70(size={},table_name={},codec={})'.format(self.size, self._table_name, self._codec)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        table_name = r.read_ucs2(r.get_smallint())
+        return cls(size, table_name, codec=r.session.conn.server_codec)
+
+    def write_info(self, w):
+        w.put_int(self.size)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_int(-1)
+        else:
+            if w._tds._tds._login.bytes_to_unicode:
+                val = tds_base.force_unicode(val)
+            if isinstance(val, six.text_type):
+                val, _ = self._codec.encode(val)
+            w.put_int(len(val))
+            w.write(val)
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        tds_base.readall(r, size)  # textptr
+        tds_base.readall(r, 8)  # timestamp
+        colsize = r.get_int()
+        if r._session._tds._login.bytes_to_unicode:
+            return r.read_str(colsize, self._codec)
+        else:
+            return tds_base.readall(r, colsize)
+
+
+class Text71Serializer(Text70Serializer):
+    def __repr__(self):
+        return 'Text71(size={}, table_name={}, collation={})'.format(
+            self.size, self._table_name, repr(self._collation)
+        )
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        collation = r.get_collation()
+        table_name = r.read_ucs2(r.get_smallint())
+        return cls(size, table_name, collation)
+
+    def write_info(self, w):
+        w.put_int(self.size)
+        w.put_collation(self._collation)
+
+
+class Text72Serializer(Text71Serializer):
+    def __init__(self, size=0, table_name_parts=(), collation=raw_collation):
+        super(Text72Serializer, self).__init__(size=size, table_name='.'.join(table_name_parts), collation=collation)
+        self._table_name_parts = table_name_parts
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        collation = r.get_collation()
+        num_parts = r.get_byte()
+        parts = []
+        for _ in range(num_parts):
+            parts.append(r.read_ucs2(r.get_smallint()))
+        return cls(size, parts, collation)
+
+
+class NText70Serializer(BaseTypeSerializer):
+    type = tds_base.SYBNTEXT
+    declaration = 'NTEXT'
+
+    def __init__(self, size=0, table_name='', collation=raw_collation):
+        super(NText70Serializer, self).__init__(size=size)
+        self._collation = collation
+        self._table_name = table_name
+
+    def __repr__(self):
+        return 'NText70(size={}, table_name={})'.format(self.size, self._table_name)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        table_name = r.read_ucs2(r.get_smallint())
+        return cls(size, table_name)
+
+    def read(self, r):
+        textptr_size = r.get_byte()
+        if textptr_size == 0:
+            return None
+        tds_base.readall(r, textptr_size)  # textptr
+        tds_base.readall(r, 8)  # timestamp
+        colsize = r.get_int()
+        return r.read_str(colsize, ucs2_codec)
+
+    def write_info(self, w):
+        w.put_int(self.size * 2)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_int(-1)
+        else:
+            w.put_int(len(val) * 2)
+            w.write_ucs2(val)
+
+
+class NText71Serializer(NText70Serializer):
+    def __repr__(self):
+        return 'NText71(size={}, table_name={}, collation={})'.format(self.size,
+                                                                      self._table_name,
+                                                                      repr(self._collation))
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        collation = r.get_collation()
+        table_name = r.read_ucs2(r.get_smallint())
+        return cls(size, table_name, collation)
+
+    def write_info(self, w):
+        w.put_int(self.size)
+        w.put_collation(self._collation)
+
+    def read(self, r):
+        textptr_size = r.get_byte()
+        if textptr_size == 0:
+            return None
+        tds_base.readall(r, textptr_size)  # textptr
+        tds_base.readall(r, 8)  # timestamp
+        colsize = r.get_int()
+        return r.read_str(colsize, ucs2_codec)
+
+
+class NText72Serializer(NText71Serializer):
+    def __init__(self, size=0, table_name_parts=(), collation=raw_collation):
+        super(NText72Serializer, self).__init__(size=size, collation=collation)
+        self._table_name_parts = table_name_parts
+
+    def __repr__(self):
+        return 'NText72Serializer(s={},table_name={},coll={})'.format(
+            self.size, self._table_name_parts, self._collation)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        collation = r.get_collation()
+        num_parts = r.get_byte()
+        parts = []
+        for _ in range(num_parts):
+            parts.append(r.read_ucs2(r.get_smallint()))
+        return cls(size, parts, collation)
+
+
+class Binary(bytes, SqlValueMetaclass):
+    def __repr__(self):
+        return 'Binary({0})'.format(super(Binary, self).__repr__())
+
+
+class VarBinarySerializer(BaseTypeSerializer):
+    type = tds_base.XSYBVARBINARY
+
+    def __init__(self, size):
+        super(VarBinarySerializer, self).__init__(size=size)
+
+    def __repr__(self):
+        return 'VarBinary({})'.format(self.size)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        return cls(size)
+
+    def write_info(self, w):
+        w.put_usmallint(self.size)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_usmallint(0xffff)
+        else:
+            w.put_usmallint(len(val))
+            w.write(val)
+
+    def read(self, r):
+        size = r.get_usmallint()
+        if size == 0xffff:
+            return None
+        return tds_base.readall(r, size)
+
+
+class VarBinarySerializer72(VarBinarySerializer):
+    def __repr__(self):
+        return 'VarBinary72({})'.format(self.size)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_usmallint()
+        if size == 0xffff:
+            return VarBinarySerializerMax()
+        return cls(size)
+
+
+class VarBinarySerializerMax(VarBinarySerializer):
+    def __init__(self):
+        super(VarBinarySerializerMax, self).__init__(0)
+
+    def __repr__(self):
+        return 'VarBinaryMax()'
+
+    def write_info(self, w):
+        w.put_usmallint(tds_base.PLP_MARKER)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_uint8(tds_base.PLP_NULL)
+        else:
+            w.put_uint8(len(val))
+            if val:
+                w.put_uint(len(val))
+                w.write(val)
+            w.put_uint(0)
+
+    def read(self, r):
+        r = PlpReader(r)
+        if r.is_null():
+            return None
+        return b''.join(r.chunks())
+
+class UDT72Serializer(BaseTypeSerializer):
+    # Data type definition stream used for UDT_INFO in TYPE_INFO
+    # https://msdn.microsoft.com/en-us/library/a57df60e-d0a6-4e7e-a2e5-ccacd277c673/
+    def __init__(self, max_byte_size, db_name, schema_name, type_name,
+                 assembly_qualified_name):
+        self.max_byte_size = max_byte_size
+        self.db_name = db_name
+        self.schema_name = schema_name
+        self.type_name = type_name
+        self.assembly_qualified_name = assembly_qualified_name
+        super(UDT72Serializer, self).__init__()
+
+    def __repr__(self):
+        return ('UDT72Serializer(max_byte_size={}, db_name={}, '
+                'schema_name={}, type_name={}, '
+                'assembly_qualified_name={})'.format(
+                    *map(repr, (
+                        self.max_byte_size, self.db_name, self.schema_name,
+                        self.type_name, self.assembly_qualified_name)))
+        )
+
+    @classmethod
+    def from_stream(cls, r):
+        # MAX_BYTE_SIZE
+        max_byte_size = r.get_usmallint()
+        assert max_byte_size == 0xffff or 1 < max_byte_size < 8000
+        # DB_NAME -- B_VARCHAR
+        db_name = r.read_ucs2(r.get_byte())
+        # SCHEMA_NAME -- B_VARCHAR
+        schema_name = r.read_ucs2(r.get_byte())
+        # TYPE_NAME -- B_VARCHAR
+        type_name = r.read_ucs2(r.get_byte())
+        # UDT_METADATA --
+        # a US_VARCHAR (2 bytes length prefix)
+        # containing ASSEMBLY_QUALIFIED_NAME
+        assembly_qualified_name = r.read_ucs2(r.get_smallint())
+        return cls(max_byte_size, db_name, schema_name, type_name,
+                   assembly_qualified_name)
+
+    def read(self, r):
+        r = PlpReader(r)
+        if r.is_null():
+            return None
+        return b''.join(r.chunks())
+
+class UDT72SerializerMax(UDT72Serializer):
+    def __init__(self, *args, **kwargs):
+        super(UDT72SerializerMax, self).__init__(0, *args, **kwargs)
+
+class Image70Serializer(BaseTypeSerializer):
+    type = tds_base.SYBIMAGE
+    declaration = 'IMAGE'
+
+    def __init__(self, size=0, table_name=''):
+        super(Image70Serializer, self).__init__(size=size)
+        self._table_name = table_name
+
+    def __repr__(self):
+        return 'Image70(tn={},s={})'.format(repr(self._table_name), self.size)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        table_name = r.read_ucs2(r.get_smallint())
+        return cls(size, table_name)
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 16:  # Jeff's hack
+            tds_base.readall(r, 16)  # textptr
+            tds_base.readall(r, 8)  # timestamp
+            colsize = r.get_int()
+            return tds_base.readall(r, colsize)
+        else:
+            return None
+
+    def write(self, w, val):
+        if val is None:
+            w.put_int(-1)
+            return
+        w.put_int(len(val))
+        w.write(val)
+
+    def write_info(self, w):
+        w.put_int(self.size)
+
+
+class Image72Serializer(Image70Serializer):
+    def __init__(self, size=0, parts=()):
+        super(Image72Serializer, self).__init__(size=size, table_name='.'.join(parts))
+        self._parts = parts
+
+    def __repr__(self):
+        return 'Image72(p={},s={})'.format(self._parts, self.size)
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        num_parts = r.get_byte()
+        parts = []
+        for _ in range(num_parts):
+            parts.append(r.read_ucs2(r.get_usmallint()))
+        return Image72Serializer(size, parts)
+
+
+_datetime_base_date = datetime.datetime(1900, 1, 1)
+
+
+class SmallDateTimeType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'SMALLDATETIME'
+
+
+class DateTimeType(SqlTypeMetaclass):
+    def get_declaration(self):
+        return 'DATETIME'
+
+
+class SmallDateTime(SqlValueMetaclass):
+    """Corresponds to MSSQL smalldatetime"""
+    def __init__(self, days, minutes):
+        """
+
+        @param days: Days since 1900-01-01
+        @param minutes: Minutes since 00:00:00
+        """
+        self._days = days
+        self._minutes = minutes
+
+    @property
+    def days(self):
+        return self._days
+
+    @property
+    def minutes(self):
+        return self._minutes
+
+    def to_pydatetime(self):
+        return _datetime_base_date + datetime.timedelta(days=self._days, minutes=self._minutes)
+
+    @classmethod
+    def from_pydatetime(cls, dt):
+        days = (dt - _datetime_base_date).days
+        minutes = dt.hour * 60 + dt.minute
+        return cls(days=days, minutes=minutes)
+
+
+class BaseDateTimeSerializer(BaseTypeSerializer):
+    def write(self, w, value):
+        raise NotImplementedError
+
+    def write_info(self, w):
+        raise NotImplementedError
+
+    def read(self, r):
+        raise NotImplementedError
+
+    @classmethod
+    def from_stream(cls, r):
+        raise NotImplementedError
+
+
+class SmallDateTimeSerializer(BasePrimitiveTypeSerializer, BaseDateTimeSerializer):
+    type = tds_base.SYBDATETIME4
+    declaration = 'SMALLDATETIME'
+
+    _struct = struct.Struct('<HH')
+
+    def write(self, w, val):
+        if val.tzinfo:
+            if not w.session.use_tz:
+                raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
+            val = val.astimezone(w.session.use_tz).replace(tzinfo=None)
+        dt = SmallDateTime.from_pydatetime(val)
+        w.pack(self._struct, dt.days, dt.minutes)
+
+    def read(self, r):
+        days, minutes = r.unpack(self._struct)
+        dt = SmallDateTime(days=days, minutes=minutes)
+        tzinfo = None
+        if r.session.tzinfo_factory is not None:
+            tzinfo = r.session.tzinfo_factory(0)
+        return dt.to_pydatetime().replace(tzinfo=tzinfo)
+
+SmallDateTimeSerializer.instance = SmallDateTimeSerializer()
+
+
+class DateTime(SqlValueMetaclass):
+    """Corresponds to MSSQL datetime"""
+    MIN_PYDATETIME = datetime.datetime(1753, 1, 1, 0, 0, 0)
+    MAX_PYDATETIME = datetime.datetime(9999, 12, 31, 23, 59, 59, 997000)
+
+    def __init__(self, days, time_part):
+        """
+
+        @param days: Days since 1900-01-01
+        @param time_part: Number of 1/300 of seconds since 00:00:00
+        """
+        self._days = days
+        self._time_part = time_part
+
+    @property
+    def days(self):
+        return self._days
+
+    @property
+    def time_part(self):
+        return self._time_part
+
+    def to_pydatetime(self):
+        ms = int(round(self._time_part % 300 * 10 / 3.0))
+        secs = self._time_part // 300
+        return _datetime_base_date + datetime.timedelta(days=self._days, seconds=secs, milliseconds=ms)
+
+    @classmethod
+    def from_pydatetime(cls, dt):
+        if not (cls.MIN_PYDATETIME <= dt <= cls.MAX_PYDATETIME):
+            raise tds_base.DataError('Datetime is out of range')
+        days = (dt - _datetime_base_date).days
+        ms = dt.microsecond // 1000
+        tm = (dt.hour * 60 * 60 + dt.minute * 60 + dt.second) * 300 + int(round(ms * 3 / 10.0))
+        return cls(days=days, time_part=tm)
+
+
+class DateTimeSerializer(BasePrimitiveTypeSerializer, BaseDateTimeSerializer):
+    type = tds_base.SYBDATETIME
+    declaration = 'DATETIME'
+
+    _struct = struct.Struct('<ll')
+
+    def write(self, w, val):
+        if val.tzinfo:
+            if not w.session.use_tz:
+                raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
+            val = val.astimezone(w.session.use_tz).replace(tzinfo=None)
+        w.write(self.encode(val))
+
+    def read(self, r):
+        days, t = r.unpack(self._struct)
+        tzinfo = None
+        if r.session.tzinfo_factory is not None:
+            tzinfo = r.session.tzinfo_factory(0)
+        return _applytz(self.decode(days, t), tzinfo)
+
+    @classmethod
+    def encode(cls, value):
+        if type(value) == datetime.date:
+            value = datetime.datetime.combine(value, datetime.time(0, 0, 0))
+        dt = DateTime.from_pydatetime(value)
+        return cls._struct.pack(dt.days, dt.time_part)
+
+    @classmethod
+    def decode(cls, days, time_part):
+        dt = DateTime(days=days, time_part=time_part)
+        return dt.to_pydatetime()
+
+DateTimeSerializer.instance = DateTimeSerializer()
+
+
+class DateTimeNSerializer(BaseTypeSerializerN, BaseDateTimeSerializer):
+    type = tds_base.SYBDATETIMN
+    subtypes = {
+        4: SmallDateTimeSerializer.instance,
+        8: DateTimeSerializer.instance,
+    }
+
+
+_datetime2_base_date = datetime.datetime(1, 1, 1)
+
+
+class DateType(SqlTypeMetaclass):
+    type = tds_base.SYBMSDATE
+
+    def get_declaration(self):
+        return "DATE"
+
+
+class Date(SqlValueMetaclass):
+    MIN_PYDATE = datetime.date(1, 1, 1)
+    MAX_PYDATE = datetime.date(9999, 12, 31)
+
+    def __init__(self, days):
+        """
+        Creates sql date object
+        @param days: Days since 0001-01-01
+        """
+        self._days = days
+
+    @property
+    def days(self):
+        return self._days
+
+    def to_pydate(self):
+        """
+        Converts sql date to Python date
+        @return: Python date
+        """
+        return (_datetime2_base_date + datetime.timedelta(days=self._days)).date()
+
+    @classmethod
+    def from_pydate(cls, pydate):
+        """
+        Creates sql date object from Python date object.
+        @param pydate: Python date
+        @return: sql date
+        """
+        return cls(days=(datetime.datetime.combine(pydate, datetime.time(0, 0, 0)) - _datetime2_base_date).days)
+
+
+class TimeType(SqlTypeMetaclass):
+    type = tds_base.SYBMSTIME
+
+    def __init__(self, precision=7):
+        self._precision = precision
+
+    @property
+    def precision(self):
+        return self._precision
+
+    def get_declaration(self):
+        return 'TIME({0})'.format(self.precision)
+
+
+class Time(SqlValueMetaclass):
+    def __init__(self, nsec):
+        """
+        Creates sql time object.
+        Maximum precision which sql server supports is 100 nanoseconds.
+        Values more precise than 100 nanoseconds will be truncated.
+        @param nsec: Nanoseconds from 00:00:00
+        """
+        self._nsec = nsec
+
+    @property
+    def nsec(self):
+        return self._nsec
+
+    def to_pytime(self):
+        """
+        Converts sql time object into Python's time object
+        this will truncate nanoseconds to microseconds
+        @return: naive time
+        """
+        nanoseconds = self._nsec
+        hours = nanoseconds // 1000000000 // 60 // 60
+        nanoseconds -= hours * 60 * 60 * 1000000000
+        minutes = nanoseconds // 1000000000 // 60
+        nanoseconds -= minutes * 60 * 1000000000
+        seconds = nanoseconds // 1000000000
+        nanoseconds -= seconds * 1000000000
+        return datetime.time(hours, minutes, seconds, nanoseconds // 1000)
+
+    @classmethod
+    def from_pytime(cls, pytime):
+        """
+        Converts Python time object to sql time object
+        ignoring timezone
+        @param pytime: Python time object
+        @return: sql time object
+        """
+        secs = pytime.hour * 60 * 60 + pytime.minute * 60 + pytime.second
+        nsec = secs * 10 ** 9 + pytime.microsecond * 1000
+        return cls(nsec=nsec)
+
+
+class DateTime2Type(SqlTypeMetaclass):
+    type = tds_base.SYBMSDATETIME2
+
+    def __init__(self, precision=7):
+        self._precision = precision
+
+    @property
+    def precision(self):
+        return self._precision
+
+    def get_declaration(self):
+        return 'DATETIME2({0})'.format(self.precision)
+
+
+class DateTime2(SqlValueMetaclass):
+    type = tds_base.SYBMSDATETIME2
+
+    def __init__(self, date, time):
+        """
+        Creates datetime2 object
+        @param date: sql date object
+        @param time: sql time object
+        """
+        self._date = date
+        self._time = time
+
+    @property
+    def date(self):
+        return self._date
+
+    @property
+    def time(self):
+        return self._time
+
+    def to_pydatetime(self):
+        """
+        Converts datetime2 object into Python's datetime.datetime object
+        @return: naive datetime.datetime
+        """
+        return datetime.datetime.combine(self._date.to_pydate(), self._time.to_pytime())
+
+    @classmethod
+    def from_pydatetime(cls, pydatetime):
+        """
+        Creates sql datetime2 object from Python datetime object
+        ignoring timezone
+        @param pydatetime: Python datetime object
+        @return: sql datetime2 object
+        """
+        return cls(date=Date.from_pydate(pydatetime.date),
+                   time=Time.from_pytime(pydatetime.time))
+
+
+class DateTimeOffsetType(SqlTypeMetaclass):
+    type = tds_base.SYBMSDATETIMEOFFSET
+
+    def __init__(self, precision=7):
+        self._precision = precision
+
+    @property
+    def precision(self):
+        return self._precision
+
+    def get_declaration(self):
+        return 'DATETIMEOFFSET({0})'.format(self.precision)
+
+
+class DateTimeOffset(SqlValueMetaclass):
+    def __init__(self, date, time, offset):
+        """
+        Creates datetime2 object
+        @param date: sql date object in UTC
+        @param time: sql time object in UTC
+        @param offset: time zone offset in minutes
+        """
+        self._date = date
+        self._time = time
+        self._offset = offset
+
+    def to_pydatetime(self):
+        """
+        Converts datetimeoffset object into Python's datetime.datetime object
+        @return: time zone aware datetime.datetime
+        """
+        dt = datetime.datetime.combine(self._date.to_pydate(), self._time.to_pytime())
+        from .tz import FixedOffsetTimezone
+        return dt.replace(tzinfo=_utc).astimezone(FixedOffsetTimezone(self._offset))
+
+
+class BaseDateTime73Serializer(BaseTypeSerializer):
+    def write(self, w, value):
+        raise NotImplementedError
+
+    def write_info(self, w):
+        raise NotImplementedError
+
+    def read(self, r):
+        raise NotImplementedError
+
+    @classmethod
+    def from_stream(cls, r):
+        raise NotImplementedError
+
+    _precision_to_len = {
+        0: 3,
+        1: 3,
+        2: 3,
+        3: 4,
+        4: 4,
+        5: 5,
+        6: 5,
+        7: 5,
+    }
+
+    def _write_time(self, w, t, prec):
+        val = t.nsec // (10 ** (9 - prec))
+        w.write(struct.pack('<Q', val)[:self._precision_to_len[prec]])
+
+    @staticmethod
+    def _read_time(r, size, prec):
+        time_buf = tds_base.readall(r, size)
+        val = _decode_num(time_buf)
+        val *= 10 ** (7 - prec)
+        nanoseconds = val * 100
+        return Time(nsec=nanoseconds)
+
+    @staticmethod
+    def _write_date(w, value):
+        days = value.days
+        buf = struct.pack('<l', days)[:3]
+        w.write(buf)
+
+    @staticmethod
+    def _read_date(r):
+        days = _decode_num(tds_base.readall(r, 3))
+        return Date(days=days)
+
+
+class MsDateSerializer(BasePrimitiveTypeSerializer, BaseDateTime73Serializer):
+    type = tds_base.SYBMSDATE
+    declaration = 'DATE'
+
+    def __init__(self, typ):
+        super(MsDateSerializer, self).__init__()
+        self._typ = typ
+
+    @classmethod
+    def from_stream(cls, r):
+        return cls(DateType())
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+        else:
+            w.put_byte(3)
+            self._write_date(w, Date.from_pydate(value))
+
+    def read_fixed(self, r):
+        return self._read_date(r).to_pydate()
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        return self._read_date(r).to_pydate()
+
+
+class MsTimeSerializer(BaseDateTime73Serializer):
+    type = tds_base.SYBMSTIME
+
+    def __init__(self, typ):
+        super(MsTimeSerializer, self).__init__(precision=typ.precision, size=self._precision_to_len[typ.precision])
+        self._typ = typ
+
+    @classmethod
+    def read_type(cls, r):
+        prec = r.get_byte()
+        return TimeType(precision=prec)
+
+    @classmethod
+    def from_stream(cls, r):
+        return cls(cls.read_type(r))
+
+    def write_info(self, w):
+        w.put_byte(self._typ.precision)
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+        else:
+            if value.tzinfo:
+                if not w.session.use_tz:
+                    raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
+                value = value.astimezone(w.session.use_tz).replace(tzinfo=None)
+            w.put_byte(self.size)
+            self._write_time(w, Time.from_pytime(value), self._typ.precision)
+
+    def read_fixed(self, r, size):
+        res = self._read_time(r, size, self._typ.precision).to_pytime()
+        if r.session.tzinfo_factory is not None:
+            tzinfo = r.session.tzinfo_factory(0)
+            res = res.replace(tzinfo=tzinfo)
+        return res
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        return self.read_fixed(r, size)
+
+
+class DateTime2Serializer(BaseDateTime73Serializer):
+    type = tds_base.SYBMSDATETIME2
+
+    def __init__(self, typ):
+        super(DateTime2Serializer, self).__init__(precision=typ.precision,
+                                                  size=self._precision_to_len[typ.precision] + 3)
+        self._typ = typ
+
+    @classmethod
+    def from_stream(cls, r):
+        prec = r.get_byte()
+        return cls(DateTime2Type(precision=prec))
+
+    def write_info(self, w):
+        w.put_byte(self._typ.precision)
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+        else:
+            if value.tzinfo:
+                if not w.session.use_tz:
+                    raise tds_base.DataError('Timezone-aware datetime is used without specifying use_tz')
+                value = value.astimezone(w.session.use_tz).replace(tzinfo=None)
+            w.put_byte(self.size)
+            self._write_time(w, Time.from_pytime(value), self._typ.precision)
+            self._write_date(w, Date.from_pydate(value))
+
+    def read_fixed(self, r, size):
+        time = self._read_time(r, size - 3, self._typ.precision)
+        date = self._read_date(r)
+        dt = DateTime2(date=date, time=time)
+        res = dt.to_pydatetime()
+        if r.session.tzinfo_factory is not None:
+            tzinfo = r.session.tzinfo_factory(0)
+            res = res.replace(tzinfo=tzinfo)
+        return res
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        return self.read_fixed(r, size)
+
+
+class DateTimeOffsetSerializer(BaseDateTime73Serializer):
+    type = tds_base.SYBMSDATETIMEOFFSET
+
+    def __init__(self, typ):
+        super(DateTimeOffsetSerializer, self).__init__(precision=typ.precision,
+                                                       size=self._precision_to_len[typ.precision] + 5)
+        self._typ = typ
+
+    @classmethod
+    def from_stream(cls, r):
+        prec = r.get_byte()
+        return cls(DateTimeOffsetType(precision=prec))
+
+    def write_info(self, w):
+        w.put_byte(self._typ.precision)
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+        else:
+            utcoffset = value.utcoffset()
+            value = value.astimezone(_utc).replace(tzinfo=None)
+
+            w.put_byte(self.size)
+            self._write_time(w, Time.from_pytime(value), self._typ.precision)
+            self._write_date(w, Date.from_pydate(value))
+            w.put_smallint(int(tds_base.total_seconds(utcoffset)) // 60)
+
+    def read_fixed(self, r, size):
+        time = self._read_time(r, size - 5, self._typ.precision)
+        date = self._read_date(r)
+        offset = r.get_smallint()
+        dt = DateTimeOffset(date=date, time=time, offset=offset)
+        return dt.to_pydatetime()
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        return self.read_fixed(r, size)
+
+
+class MsDecimalSerializer(BaseTypeSerializer):
+    type = tds_base.SYBDECIMAL
+
+    _max_size = 17
+
+    _bytes_per_prec = [
+        #
+        # precision can't be 0 but using a value > 0 assure no
+        # core if for some bug it's 0...
+        #
+        1,
+        5, 5, 5, 5, 5, 5, 5, 5, 5,
+        9, 9, 9, 9, 9, 9, 9, 9, 9, 9,
+        13, 13, 13, 13, 13, 13, 13, 13, 13,
+        17, 17, 17, 17, 17, 17, 17, 17, 17, 17,
+    ]
+
+    _info_struct = struct.Struct('BBB')
+
+    def __init__(self, precision=18, scale=0):
+        super(MsDecimalSerializer, self).__init__(precision=precision,
+                                                  scale=scale,
+                                                  size=self._bytes_per_prec[precision])
+        if precision > 38:
+            raise tds_base.DataError('Precision of decimal value is out of range')
+
+    def __repr__(self):
+        return 'MsDecimal(scale={}, prec={})'.format(self.scale, self.precision)
+
+    @classmethod
+    def from_value(cls, value):
+        sql_type = DecimalType.from_value(value)
+        return cls(scale=sql_type.scale, prec=sql_type.precision)
+
+    @classmethod
+    def from_stream(cls, r):
+        size, prec, scale = r.unpack(cls._info_struct)
+        return cls(scale=scale, precision=prec)
+
+    def write_info(self, w):
+        w.pack(self._info_struct, self.size, self.precision, self.scale)
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+            return
+        if not isinstance(value, decimal.Decimal):
+            value = decimal.Decimal(value)
+        value = value.normalize()
+        scale = self.scale
+        size = self.size
+        w.put_byte(size)
+        val = value
+        positive = 1 if val > 0 else 0
+        w.put_byte(positive)  # sign
+        with decimal.localcontext() as ctx:
+            ctx.prec = 38
+            if not positive:
+                val *= -1
+            size -= 1
+            val *= 10 ** scale
+        for i in range(size):
+            w.put_byte(int(val % 256))
+            val //= 256
+        assert val == 0
+
+    def _decode(self, positive, buf):
+        val = _decode_num(buf)
+        val = decimal.Decimal(val)
+        with decimal.localcontext() as ctx:
+            ctx.prec = 38
+            if not positive:
+                val *= -1
+            val /= 10 ** self._scale
+        return val
+
+    def read_fixed(self, r, size):
+        positive = r.get_byte()
+        buf = tds_base.readall(r, size - 1)
+        return self._decode(positive, buf)
+
+    def read(self, r):
+        size = r.get_byte()
+        if size <= 0:
+            return None
+        return self.read_fixed(r, size)
+
+
+class Money4Serializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBMONEY4
+    declaration = 'SMALLMONEY'
+
+    def read(self, r):
+        return decimal.Decimal(r.get_int()) / 10000
+
+    def write(self, w, val):
+        val = int(val * 10000)
+        w.put_int(val)
+
+Money4Serializer.instance = Money4Serializer()
+
+
+class Money8Serializer(BasePrimitiveTypeSerializer):
+    type = tds_base.SYBMONEY
+    declaration = 'MONEY'
+
+    _struct = struct.Struct('<lL')
+
+    def read(self, r):
+        hi, lo = r.unpack(self._struct)
+        val = hi * (2 ** 32) + lo
+        return decimal.Decimal(val) / 10000
+
+    def write(self, w, val):
+        val *= 10000
+        hi = int(val // (2 ** 32))
+        lo = int(val % (2 ** 32))
+        w.pack(self._struct, hi, lo)
+
+Money8Serializer.instance = Money8Serializer()
+
+
+class MoneyNSerializer(BaseTypeSerializerN):
+    type = tds_base.SYBMONEYN
+
+    subtypes = {
+        4: Money4Serializer.instance,
+        8: Money8Serializer.instance,
+    }
+
+
+class MsUniqueSerializer(BaseTypeSerializer):
+    type = tds_base.SYBUNIQUE
+    declaration = 'UNIQUEIDENTIFIER'
+    instance = None
+
+    def __repr__(self):
+        return 'MsUniqueSerializer()'
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_byte()
+        if size != 16:
+            raise tds_base.InterfaceError('Invalid size of UNIQUEIDENTIFIER field')
+        return cls.instance
+
+    def write_info(self, w):
+        w.put_byte(16)
+
+    def write(self, w, value):
+        if value is None:
+            w.put_byte(0)
+        else:
+            w.put_byte(16)
+            w.write(value.bytes_le)
+
+    @staticmethod
+    def read_fixed(r, size):
+        return uuid.UUID(bytes_le=tds_base.readall(r, size))
+
+    def read(self, r):
+        size = r.get_byte()
+        if size == 0:
+            return None
+        if size != 16:
+            raise tds_base.InterfaceError('Invalid size of UNIQUEIDENTIFIER field')
+        return self.read_fixed(r, size)
+MsUniqueSerializer.instance = MsUniqueSerializer()
+
+
+def _variant_read_str(r, size):
+    collation = r.get_collation()
+    r.get_usmallint()
+    return r.read_str(size, collation.get_codec())
+
+
+def _variant_read_nstr(r, size):
+    r.get_collation()
+    r.get_usmallint()
+    return r.read_str(size, ucs2_codec)
+
+
+def _variant_read_decimal(r, size):
+    prec, scale = r.unpack(VariantSerializer.decimal_info_struct)
+    return MsDecimalSerializer(precision=prec, scale=scale).read_fixed(r, size)
+
+
+def _variant_read_binary(r, size):
+    r.get_usmallint()
+    return tds_base.readall(r, size)
+
+
+class VariantSerializer(BaseTypeSerializer):
+    type = tds_base.SYBVARIANT
+    declaration = 'SQL_VARIANT'
+
+    decimal_info_struct = struct.Struct('BB')
+
+    _type_map = {
+        tds_base.GUIDTYPE: lambda r, size: MsUniqueSerializer.instance.read_fixed(r, size),
+        tds_base.BITTYPE: lambda r, size: BitSerializer.instance.read(r),
+        tds_base.INT1TYPE: lambda r, size: TinyIntSerializer.instance.read(r),
+        tds_base.INT2TYPE: lambda r, size: SmallIntSerializer.instance.read(r),
+        tds_base.INT4TYPE: lambda r, size: IntSerializer.instance.read(r),
+        tds_base.INT8TYPE: lambda r, size: BigIntSerializer.instance.read(r),
+        tds_base.DATETIMETYPE: lambda r, size: DateTimeSerializer.instance.read(r),
+        tds_base.DATETIM4TYPE: lambda r, size: SmallDateTimeSerializer.instance.read(r),
+        tds_base.FLT4TYPE: lambda r, size: RealSerializer.instance.read(r),
+        tds_base.FLT8TYPE: lambda r, size: FloatSerializer.instance.read(r),
+        tds_base.MONEYTYPE: lambda r, size: Money8Serializer.instance.read(r),
+        tds_base.MONEY4TYPE: lambda r, size: Money4Serializer.instance.read(r),
+        tds_base.DATENTYPE: lambda r, size: MsDateSerializer(DateType()).read_fixed(r),
+
+        tds_base.TIMENTYPE: lambda r, size: MsTimeSerializer(TimeType(precision=r.get_byte())).read_fixed(r, size),
+        tds_base.DATETIME2NTYPE: lambda r, size: DateTime2Serializer(
+            DateTime2Type(precision=r.get_byte())).read_fixed(r, size),
+        tds_base.DATETIMEOFFSETNTYPE: lambda r, size: DateTimeOffsetSerializer(
+            DateTimeOffsetType(precision=r.get_byte())).read_fixed(r, size),
+
+        tds_base.BIGVARBINTYPE: _variant_read_binary,
+        tds_base.BIGBINARYTYPE: _variant_read_binary,
+
+        tds_base.NUMERICNTYPE: _variant_read_decimal,
+        tds_base.DECIMALNTYPE: _variant_read_decimal,
+
+        tds_base.BIGVARCHRTYPE: _variant_read_str,
+        tds_base.BIGCHARTYPE: _variant_read_str,
+        tds_base.NVARCHARTYPE: _variant_read_nstr,
+        tds_base.NCHARTYPE: _variant_read_nstr,
+
+    }
+
+    @classmethod
+    def from_stream(cls, r):
+        size = r.get_int()
+        return VariantSerializer(size)
+
+    def write_info(self, w):
+        w.put_int(self.size)
+
+    def read(self, r):
+        size = r.get_int()
+        if size == 0:
+            return None
+
+        type_id = r.get_byte()
+        prop_bytes = r.get_byte()
+        type_factory = self._type_map.get(type_id)
+        if not type_factory:
+            r.session.bad_stream('Variant type invalid', type_id)
+        return type_factory(r, size - prop_bytes - 2)
+
+    def write(self, w, val):
+        if val is None:
+            w.put_int(0)
+            return
+        raise NotImplementedError
+
+
+class TableType(SqlTypeMetaclass):
+    """
+    Used to serialize table valued parameters
+
+    spec: https://msdn.microsoft.com/en-us/library/dd304813.aspx
+    """
+    def __init__(self, typ_schema, typ_name, columns):
+        """
+        @param typ_schema: Schema where TVP type defined
+        @param typ_name: Name of TVP type
+        @param columns: List of column types
+        """
+        if len(typ_schema) > 128:
+            raise ValueError("Schema part of TVP name should be no longer than 128 characters")
+        if len(typ_name) > 128:
+            raise ValueError("Name part of TVP name should be no longer than 128 characters")
+        if columns is not None:
+            if len(columns) > 1024:
+                raise ValueError("TVP cannot have more than 1024 columns")
+            if len(columns) < 1:
+                raise ValueError("TVP must have at least one column")
+        self._typ_dbname = ''  # dbname should always be empty string for TVP according to spec
+        self._typ_schema = typ_schema
+        self._typ_name = typ_name
+        self._columns = columns
+
+    def __repr__(self):
+        return 'TableType(s={},n={},cols={})'.format(
+            self._typ_schema, self._typ_name, repr(self._columns)
+        )
+
+    def get_declaration(self):
+        assert not self._typ_dbname
+        if self._typ_schema:
+            full_name = '{}.{}'.format(self._typ_schema, self._typ_name)
+        else:
+            full_name = self._typ_name
+        return '{} READONLY'.format(full_name)
+
+    @property
+    def typ_schema(self):
+        return self._typ_schema
+
+    @property
+    def typ_name(self):
+        return self._typ_name
+
+    @property
+    def columns(self):
+        return self._columns
+
+
+class TableValuedParam(SqlValueMetaclass):
+    """
+    Used to represent a value of table-valued parameter
+    """
+    def __init__(self, type_name=None, columns=None, rows=None):
+        # parsing type name
+        self._typ_schema = ''
+        self._typ_name = ''
+        if type_name:
+            parts = type_name.split('.')
+            if len(parts) > 2:
+                raise ValueError('Type name should consist of at most 2 parts, e.g. dbo.MyType')
+            self._typ_name = parts[-1]
+            if len(parts) > 1:
+                self._typ_schema = parts[0]
+
+        self._columns = columns
+        self._rows = rows
+
+    @property
+    def typ_name(self):
+        return self._typ_name
+
+    @property
+    def typ_schema(self):
+        return self._typ_schema
+
+    @property
+    def columns(self):
+        return self._columns
+
+    @property
+    def rows(self):
+        return self._rows
+
+    def is_null(self):
+        return self._rows is None
+
+    def peek_row(self):
+        try:
+            rows = iter(self._rows)
+        except TypeError:
+            raise tds_base.DataError('rows should be iterable')
+
+        try:
+            row = next(rows)
+        except StopIteration:
+            # no rows
+            raise tds_base.DataError("Cannot infer columns from rows for TVP because there are no rows")
+        else:
+            # put row back
+            self._rows = itertools.chain([row], rows)
+        return row
+
+
+class TableSerializer(BaseTypeSerializer):
+    """
+    Used to serialize table valued parameters
+
+    spec: https://msdn.microsoft.com/en-us/library/dd304813.aspx
+    """
+
+    type = tds_base.TVPTYPE
+
+    def read(self, r):
+        """ According to spec TDS does not support output TVP values """
+        raise NotImplementedError
+
+    @classmethod
+    def from_stream(cls, r):
+        """ According to spec TDS does not support output TVP values """
+        raise NotImplementedError
+
+    def __init__(self, table_type, columns_serializers):
+        super(TableSerializer, self).__init__()
+        self._table_type = table_type
+        self._columns_serializers = columns_serializers
+
+    @property
+    def table_type(self):
+        return self._table_type
+
+    def __repr__(self):
+        return 'TableSerializer(t={},c={})'.format(
+            repr(self._table_type), repr(self._columns_serializers)
+        )
+
+    def write_info(self, w):
+        """
+        Writes TVP_TYPENAME structure
+
+        spec: https://msdn.microsoft.com/en-us/library/dd302994.aspx
+        @param w: TdsWriter
+        @return:
+        """
+        w.write_b_varchar("")  # db_name, should be empty
+        w.write_b_varchar(self._table_type.typ_schema)
+        w.write_b_varchar(self._table_type.typ_name)
+
+    def write(self, w, val):
+        """
+        Writes remaining part of TVP_TYPE_INFO structure, resuming from TVP_COLMETADATA
+
+        specs:
+        https://msdn.microsoft.com/en-us/library/dd302994.aspx
+        https://msdn.microsoft.com/en-us/library/dd305261.aspx
+        https://msdn.microsoft.com/en-us/library/dd303230.aspx
+
+        @param w: TdsWriter
+        @param val: TableValuedParam or None
+        @return:
+        """
+        if val.is_null():
+            w.put_usmallint(tds_base.TVP_NULL_TOKEN)
+        else:
+            columns = self._table_type.columns
+            w.put_usmallint(len(columns))
+            for i, column in enumerate(columns):
+                w.put_uint(column.column_usertype)
+
+                w.put_usmallint(column.flags)
+
+                # TYPE_INFO structure: https://msdn.microsoft.com/en-us/library/dd358284.aspx
+
+                serializer = self._columns_serializers[i]
+                type_id = serializer.type
+                w.put_byte(type_id)
+                serializer.write_info(w)
+
+                w.write_b_varchar('')  # ColName, must be empty in TVP according to spec
+
+        # here can optionally send TVP_ORDER_UNIQUE and TVP_COLUMN_ORDERING
+        # https://msdn.microsoft.com/en-us/library/dd305261.aspx
+
+        # terminating optional metadata
+        w.put_byte(tds_base.TVP_END_TOKEN)
+
+        # now sending rows using TVP_ROW
+        # https://msdn.microsoft.com/en-us/library/dd305261.aspx
+        if val.rows:
+            for row in val.rows:
+                w.put_byte(tds_base.TVP_ROW_TOKEN)
+                for i, col in enumerate(self._table_type.columns):
+                    if not col.flags & tds_base.TVP_COLUMN_DEFAULT_FLAG:
+                        self._columns_serializers[i].write(w, row[i])
+
+        # terminating rows
+        w.put_byte(tds_base.TVP_END_TOKEN)
+
+
+_type_map = {
+    tds_base.SYBINT1: TinyIntSerializer,
+    tds_base.SYBINT2: SmallIntSerializer,
+    tds_base.SYBINT4: IntSerializer,
+    tds_base.SYBINT8: BigIntSerializer,
+    tds_base.SYBINTN: IntNSerializer,
+    tds_base.SYBBIT: BitSerializer,
+    tds_base.SYBBITN: BitNSerializer,
+    tds_base.SYBREAL: RealSerializer,
+    tds_base.SYBFLT8: FloatSerializer,
+    tds_base.SYBFLTN: FloatNSerializer,
+    tds_base.SYBMONEY4: Money4Serializer,
+    tds_base.SYBMONEY: Money8Serializer,
+    tds_base.SYBMONEYN: MoneyNSerializer,
+    tds_base.XSYBCHAR: VarChar70Serializer,
+    tds_base.XSYBVARCHAR: VarChar70Serializer,
+    tds_base.XSYBNCHAR: NVarChar70Serializer,
+    tds_base.XSYBNVARCHAR: NVarChar70Serializer,
+    tds_base.SYBTEXT: Text70Serializer,
+    tds_base.SYBNTEXT: NText70Serializer,
+    tds_base.SYBMSXML: XmlSerializer,
+    tds_base.XSYBBINARY: VarBinarySerializer,
+    tds_base.XSYBVARBINARY: VarBinarySerializer,
+    tds_base.SYBIMAGE: Image70Serializer,
+    tds_base.SYBNUMERIC: MsDecimalSerializer,
+    tds_base.SYBDECIMAL: MsDecimalSerializer,
+    tds_base.SYBVARIANT: VariantSerializer,
+    tds_base.SYBMSDATE: MsDateSerializer,
+    tds_base.SYBMSTIME: MsTimeSerializer,
+    tds_base.SYBMSDATETIME2: DateTime2Serializer,
+    tds_base.SYBMSDATETIMEOFFSET: DateTimeOffsetSerializer,
+    tds_base.SYBDATETIME4: SmallDateTimeSerializer,
+    tds_base.SYBDATETIME: DateTimeSerializer,
+    tds_base.SYBDATETIMN: DateTimeNSerializer,
+    tds_base.SYBUNIQUE: MsUniqueSerializer,
+}
+
+_type_map71 = _type_map.copy()
+_type_map71.update({
+    tds_base.XSYBCHAR: VarChar71Serializer,
+    tds_base.XSYBNCHAR: NVarChar71Serializer,
+    tds_base.XSYBVARCHAR: VarChar71Serializer,
+    tds_base.XSYBNVARCHAR: NVarChar71Serializer,
+    tds_base.SYBTEXT: Text71Serializer,
+    tds_base.SYBNTEXT: NText71Serializer,
+})
+
+_type_map72 = _type_map.copy()
+_type_map72.update({
+    tds_base.XSYBCHAR: VarChar72Serializer,
+    tds_base.XSYBNCHAR: NVarChar72Serializer,
+    tds_base.XSYBVARCHAR: VarChar72Serializer,
+    tds_base.XSYBNVARCHAR: NVarChar72Serializer,
+    tds_base.SYBTEXT: Text72Serializer,
+    tds_base.SYBNTEXT: NText72Serializer,
+    tds_base.XSYBBINARY: VarBinarySerializer72,
+    tds_base.XSYBVARBINARY: VarBinarySerializer72,
+    tds_base.SYBIMAGE: Image72Serializer,
+    tds_base.UDTTYPE: UDT72Serializer,
+})
+
+_type_map73 = _type_map72.copy()
+_type_map73.update({
+    tds_base.TVPTYPE: TableSerializer,
+})
+
+
+def sql_type_by_declaration(declaration):
+    return _declarations_parser.parse(declaration)
+
+
+class SerializerFactory(object):
+    """
+    Factory class for TDS data types
+    """
+    def __init__(self, tds_ver):
+        self._tds_ver = tds_ver
+        if self._tds_ver >= tds_base.TDS73:
+            self._type_map = _type_map73
+        elif self._tds_ver >= tds_base.TDS72:
+            self._type_map = _type_map72
+        elif self._tds_ver >= tds_base.TDS71:
+            self._type_map = _type_map71
+        else:
+            self._type_map = _type_map
+
+    def get_type_serializer(self, tds_type_id):
+        type_class = self._type_map.get(tds_type_id)
+        if not type_class:
+            raise tds_base.InterfaceError('Invalid type id {}'.format(tds_type_id))
+        return type_class
+
+    def long_binary_type(self):
+        if self._tds_ver >= tds_base.TDS72:
+            return VarBinaryMaxType()
+        else:
+            return ImageType()
+
+    def long_varchar_type(self):
+        if self._tds_ver >= tds_base.TDS72:
+            return VarCharMaxType()
+        else:
+            return TextType()
+
+    def long_string_type(self):
+        if self._tds_ver >= tds_base.TDS72:
+            return NVarCharMaxType()
+        else:
+            return NTextType()
+
+    def datetime(self, precision):
+        if self._tds_ver >= tds_base.TDS72:
+            return DateTime2Type(precision=precision)
+        else:
+            return DateTimeType()
+
+    def has_datetime_with_tz(self):
+        return self._tds_ver >= tds_base.TDS72
+
+    def datetime_with_tz(self, precision):
+        if self._tds_ver >= tds_base.TDS72:
+            return DateTimeOffsetType(precision=precision)
+        else:
+            raise tds_base.DataError('Given TDS version does not support DATETIMEOFFSET type')
+
+    def date(self):
+        if self._tds_ver >= tds_base.TDS72:
+            return DateType()
+        else:
+            return DateTimeType()
+
+    def time(self, precision):
+        if self._tds_ver >= tds_base.TDS72:
+            return TimeType(precision=precision)
+        else:
+            raise tds_base.DataError('Given TDS version does not support TIME type')
+
+    def serializer_by_declaration(self, declaration, connection):
+        sql_type = sql_type_by_declaration(declaration)
+        return self.serializer_by_type(sql_type=sql_type, collation=connection.collation)
+
+    def serializer_by_type(self, sql_type, collation=raw_collation):
+        typ = sql_type
+        if isinstance(typ, BitType):
+            return BitNSerializer(typ)
+        elif isinstance(typ, TinyIntType):
+            return IntNSerializer(typ)
+        elif isinstance(typ, SmallIntType):
+            return IntNSerializer(typ)
+        elif isinstance(typ, IntType):
+            return IntNSerializer(typ)
+        elif isinstance(typ, BigIntType):
+            return IntNSerializer(typ)
+        elif isinstance(typ, RealType):
+            return FloatNSerializer(size=4)
+        elif isinstance(typ, FloatType):
+            return FloatNSerializer(size=8)
+        elif isinstance(typ, SmallMoneyType):
+            return self._type_map[tds_base.SYBMONEYN](size=4)
+        elif isinstance(typ, MoneyType):
+            return self._type_map[tds_base.SYBMONEYN](size=8)
+        elif isinstance(typ, CharType):
+            return self._type_map[tds_base.XSYBCHAR](size=typ.size, collation=collation)
+        elif isinstance(typ, VarCharType):
+            return self._type_map[tds_base.XSYBVARCHAR](size=typ.size, collation=collation)
+        elif isinstance(typ, VarCharMaxType):
+            return VarCharMaxSerializer(collation=collation)
+        elif isinstance(typ, NCharType):
+            return self._type_map[tds_base.XSYBNCHAR](size=typ.size, collation=collation)
+        elif isinstance(typ, NVarCharType):
+            return self._type_map[tds_base.XSYBNVARCHAR](size=typ.size, collation=collation)
+        elif isinstance(typ, NVarCharMaxType):
+            return NVarCharMaxSerializer(collation=collation)
+        elif isinstance(typ, TextType):
+            return self._type_map[tds_base.SYBTEXT](collation=collation)
+        elif isinstance(typ, NTextType):
+            return self._type_map[tds_base.SYBNTEXT](collation=collation)
+        elif isinstance(typ, XmlType):
+            return self._type_map[tds_base.SYBMSXML]()
+        elif isinstance(typ, BinaryType):
+            return self._type_map[tds_base.XSYBBINARY]()
+        elif isinstance(typ, VarBinaryType):
+            return self._type_map[tds_base.XSYBVARBINARY](size=typ.size)
+        elif isinstance(typ, VarBinaryMaxType):
+            return VarBinarySerializerMax()
+        elif isinstance(typ, ImageType):
+            return self._type_map[tds_base.SYBIMAGE]()
+        elif isinstance(typ, DecimalType):
+            return self._type_map[tds_base.SYBDECIMAL](scale=typ.scale, precision=typ.precision)
+        elif isinstance(typ, VariantType):
+            return self._type_map[tds_base.SYBVARIANT](size=0)
+        elif isinstance(typ, SmallDateTimeType):
+            return self._type_map[tds_base.SYBDATETIMN](size=4)
+        elif isinstance(typ, DateTimeType):
+            return self._type_map[tds_base.SYBDATETIMN](size=8)
+        elif isinstance(typ, DateType):
+            return self._type_map[tds_base.SYBMSDATE](typ)
+        elif isinstance(typ, TimeType):
+            return self._type_map[tds_base.SYBMSTIME](typ)
+        elif isinstance(typ, DateTime2Type):
+            return self._type_map[tds_base.SYBMSDATETIME2](typ)
+        elif isinstance(typ, DateTimeOffsetType):
+            return self._type_map[tds_base.SYBMSDATETIMEOFFSET](typ)
+        elif isinstance(typ, UniqueIdentifierType):
+            return self._type_map[tds_base.SYBUNIQUE]()
+        elif isinstance(typ, TableType):
+            columns_serializers = None
+            if typ.columns is not None:
+                columns_serializers = [self.serializer_by_type(col.type) for col in typ.columns]
+            return TableSerializer(table_type=typ, columns_serializers=columns_serializers)
+        else:
+            raise ValueError('Cannot map type {} to serializer.'.format(typ))
+
+
+class DeclarationsParser(object):
+    def __init__(self):
+        declaration_parsers = [
+            ('bit', BitType),
+            ('tinyint', TinyIntType),
+            ('smallint', SmallIntType),
+            ('(?:int|integer)', IntType),
+            ('bigint', BigIntType),
+            ('real', RealType),
+            ('(?:float|double precision)', FloatType),
+            ('(?:char|character)', CharType),
+            (r'(?:char|character)\((\d+)\)', lambda size_str: CharType(size=int(size_str))),
+            (r'(?:varchar|char(?:|acter)\s+varying)', VarCharType),
+            (r'(?:varchar|char(?:|acter)\s+varying)\((\d+)\)', lambda size_str: VarCharType(size=int(size_str))),
+            (r'varchar\(max\)', VarCharMaxType),
+            (r'(?:nchar|national\s+(?:char|character))', NCharType),
+            (r'(?:nchar|national\s+(?:char|character))\((\d+)\)', lambda size_str: NCharType(size=int(size_str))),
+            (r'(?:nvarchar|national\s+(?:char|character)\s+varying)', NVarCharType),
+            (r'(?:nvarchar|national\s+(?:char|character)\s+varying)\((\d+)\)',
+             lambda size_str: NVarCharType(size=int(size_str))),
+            (r'nvarchar\(max\)', NVarCharMaxType),
+            ('xml', XmlType),
+            ('text', TextType),
+            (r'(?:ntext|national\s+text)', NTextType),
+            ('binary', BinaryType),
+            ('binary\((\d+)\)', lambda size_str: BinaryType(size=int(size_str))),
+            ('(?:varbinary|binary varying)', VarBinaryType),
+            (r'(?:varbinary|binary varying)\((\d+)\)', lambda size_str: VarBinaryType(size=int(size_str))),
+            (r'varbinary\(max\)', VarBinaryMaxType),
+            ('image', ImageType),
+            ('smalldatetime', SmallDateTimeType),
+            ('datetime', DateTimeType),
+            ('date', DateType),
+            (r'time', TimeType),
+            (r'time\((\d+)\)', lambda precision_str: TimeType(precision=int(precision_str))),
+            ('datetime2', DateTime2Type),
+            (r'datetime2\((\d+)\)', lambda precision_str: DateTime2Type(precision=int(precision_str))),
+            ('datetimeoffset', DateTimeOffsetType),
+            (r'datetimeoffset\((\d+)\)',
+             lambda precision_str: DateTimeOffsetType(precision=int(precision_str))),
+            ('(?:decimal|dec|numeric)', DecimalType),
+            ('(?:decimal|dec|numeric)\((\d+)\)',
+             lambda precision_str: DecimalType(precision=int(precision_str))),
+            ('(?:decimal|dec|numeric)\((\d+), (\d+)\)',
+             lambda precision_str, scale_str: DecimalType(precision=int(precision_str), scale=int(scale_str))),
+            ('smallmoney', SmallMoneyType),
+            ('money', MoneyType),
+            ('uniqueidentifier', UniqueIdentifierType),
+            ('sql_variant', VariantType),
+        ]
+        self._compiled = [(re.compile(r'^' + regex + '$', re.IGNORECASE), constructor)
+                          for regex, constructor in declaration_parsers]
+
+    def parse(self, declaration):
+        """
+        Parse sql type declaration, e.g. varchar(10) and return instance of corresponding type class,
+        e.g. VarCharType(10)
+
+        @param declaration: Sql declaration to parse, e.g. varchar(10)
+        @return: instance of SqlTypeMetaclass
+        """
+        declaration = declaration.strip()
+        for regex, constructor in self._compiled:
+            m = regex.match(declaration)
+            if m:
+                return constructor(*m.groups())
+        raise ValueError('Unable to parse type declaration', declaration)
+
+
+_declarations_parser = DeclarationsParser()
+
+
+class TdsTypeInferrer(object):
+    def __init__(self, type_factory, collation=None, bytes_to_unicode=False, allow_tz=False):
+        """
+        Class used to do TDS type inference
+
+        :param type_factory: Instance of TypeFactory
+        :param collation: Collation to use for strings
+        :param bytes_to_unicode: Treat bytes type as unicode string
+        :param allow_tz: Allow usage of DATETIMEOFFSET type
+        """
+        self._type_factory = type_factory
+        self._collation = collation
+        self._bytes_to_unicode = bytes_to_unicode
+        self._allow_tz = allow_tz
+
+    def from_value(self, value):
+        """ Function infers TDS type from Python value.
+
+        :param value: value from which to infer TDS type
+        :return: An instance of subclass of :class:`BaseType`
+        """
+        if value is None:
+            sql_type = NVarCharType(size=1)
+        else:
+            sql_type = self._from_class_value(value, type(value))
+        return sql_type
+
+    def from_class(self, cls):
+        """ Function infers TDS type from Python class.
+
+        :param cls: Class from which to infer type
+        :return: An instance of subclass of :class:`BaseType`
+        """
+        return self._from_class_value(None, cls)
+
+    def _from_class_value(self, value, value_type):
+        type_factory = self._type_factory
+        bytes_to_unicode = self._bytes_to_unicode
+        allow_tz = self._allow_tz
+
+        if issubclass(value_type, bool):
+            return BitType()
+        elif issubclass(value_type, six.integer_types):
+            if value is None:
+                return IntType()
+            if -2 ** 31 <= value <= 2 ** 31 - 1:
+                return IntType()
+            elif -2 ** 63 <= value <= 2 ** 63 - 1:
+                return BigIntType()
+            elif -10 ** 38 + 1 <= value <= 10 ** 38 - 1:
+                return DecimalType(precision=38)
+            else:
+                return VarCharMaxType()
+        elif issubclass(value_type, float):
+            return FloatType()
+        elif issubclass(value_type, Binary):
+            if value is None or len(value) <= 8000:
+                return VarBinaryType(size=8000)
+            else:
+                return type_factory.long_binary_type()
+        elif issubclass(value_type, six.binary_type):
+            if bytes_to_unicode:
+                return type_factory.long_string_type()
+            else:
+                return type_factory.long_varchar_type()
+        elif issubclass(value_type, six.string_types):
+            return type_factory.long_string_type()
+        elif issubclass(value_type, datetime.datetime):
+            if value and value.tzinfo and allow_tz:
+                return type_factory.datetime_with_tz(precision=6)
+            else:
+                return type_factory.datetime(precision=6)
+        elif issubclass(value_type, datetime.date):
+            return type_factory.date()
+        elif issubclass(value_type, datetime.time):
+            return type_factory.time(precision=6)
+        elif issubclass(value_type, decimal.Decimal):
+            if value is None:
+                return DecimalType()
+            else:
+                return DecimalType.from_value(value)
+        elif issubclass(value_type, uuid.UUID):
+            return UniqueIdentifierType()
+        elif issubclass(value_type, TableValuedParam):
+            columns = value.columns
+            rows = value.rows
+            if columns is None:
+                # trying to auto detect columns using data from first row
+                if rows is None:
+                    # rows are not present too, this means
+                    # entire tvp has value of NULL
+                    pass
+                else:
+                    # use first row to infer types of columns
+                    row = value.peek_row()
+                    columns = []
+                    try:
+                        cell_iter = iter(row)
+                    except TypeError:
+                        raise tds_base.DataError('Each row in table should be an iterable')
+                    for cell in cell_iter:
+                        if isinstance(cell, TableValuedParam):
+                            raise tds_base.DataError('TVP type cannot have nested TVP types')
+                        col_type = self.from_value(cell)
+                        col = tds_base.Column(type=col_type)
+                        columns.append(col)
+
+            return TableType(typ_schema=value.typ_schema, typ_name=value.typ_name, columns=columns)
+        else:
+            raise tds_base.DataError('Cannot infer TDS type from Python value: {!r}'.format(value))
```

### Comparing `python-tds-1.9.0/pytds/tls.py` & `python-tds-1.9.1/pytds/tls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,136 @@
-try:
-    import OpenSSL.SSL
-    import cryptography.hazmat.backends.openssl.backend
-except ImportError:
-    OPENSSL_AVAILABLE = False
-else:
-    OPENSSL_AVAILABLE = True
-
-from . import tds_base
-
-
-BUFSIZE = 65536
-
-
-class EncryptedSocket(object):
-    def __init__(self, transport, tls_conn):
-        self._transport = transport
-        self._tls_conn = tls_conn
-
-    def sendall(self, data, flags=0):
-        # TLS.Connection does not support bytearrays, need to convert to bytes first
-        if isinstance(data, bytearray):
-            data = bytes(data)
-
-        res = self._tls_conn.sendall(data)
-        buf = self._tls_conn.bio_read(BUFSIZE)
-        self._transport.sendall(buf)
-        return res
-
-    def send(self, data):
-        while True:
-            try:
-                return self._tls_conn.send(data)
-            except OpenSSL.SSL.WantWriteError:
-                buf = self._tls_conn.bio_read(BUFSIZE)
-                self._transport.sendall(buf)
-
-    def recv(self, bufsize):
-        while True:
-            try:
-                return self._tls_conn.recv(bufsize)
-            except OpenSSL.SSL.WantReadError:
-                buf = self._transport.recv(BUFSIZE)
-                self._tls_conn.bio_write(buf)
-
-    def close(self):
-        self._tls_conn.shutdown()
-        self._transport.close()
-
-    def shutdown(self):
-        self._tls_conn.shutdown()
-
-
-def verify_cb(conn, cert, err_num, err_depth, ret_code):
-    return ret_code == 1
-
-
-def validate_host(cert, name):
-    """
-    Validates host name against certificate
-
-    @param cert: Certificate returned by host
-    @param name: Actual host name used for connection
-    @return: Returns true if host name matches certificate
-    """
-    cn = None
-    for t, v in cert.get_subject().get_components():
-        if t == b'CN':
-            cn = v
-            break
-
-    # TODO check SAN extensions
-    # TODO handle wildcards
-    return cn == name
-
-
-def create_context(cafile):
-    ctx = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
-    ctx.set_options(OpenSSL.SSL.OP_NO_SSLv2)
-    ctx.set_options(OpenSSL.SSL.OP_NO_SSLv3)
-    ctx.set_verify(OpenSSL.SSL.VERIFY_PEER, verify_cb)
-    #print("verify depth:", ctx.get_verify_depth())
-    #print("verify mode:", ctx.get_verify_mode())
-    #print("openssl version:", cryptography.hazmat.backends.openssl.backend.openssl_version_text())
-    ctx.load_verify_locations(cafile=cafile)
-    return ctx
-
-
-# https://msdn.microsoft.com/en-us/library/dd357559.aspx
-def establish_channel(tds_sock):
-    w = tds_sock._writer
-    r = tds_sock._reader
-    login = tds_sock.conn._login
-
-    bhost = login.server_name.encode('ascii')
-
-    conn = OpenSSL.SSL.Connection(login.tls_ctx)
-    conn.set_tlsext_host_name(bhost)
-    conn.set_connect_state()
-    while True:
-        try:
-            conn.do_handshake()
-        except OpenSSL.SSL.WantReadError:
-            req = conn.bio_read(BUFSIZE)
-            w.begin_packet(tds_base.TDS71_PRELOGIN)
-            w.write(req)
-            w.flush()
-            resp = r.read_whole_packet()
-            # TODO validate r.packet_type
-            conn.bio_write(resp)
-        else:
-            if login.validate_host:
-                if not validate_host(cert=conn.get_peer_certificate(), name=bhost):
-                    # TODO throw correct exception class
-                    raise Exception("Certificate does not match host name '{}'".format(login.server_name))
-            tds_sock.conn.sock = EncryptedSocket(transport=tds_sock.conn.sock, tls_conn=conn)
-            return
-
-
-def revert_to_clear(tds_sock):
-    """
-    Reverts connection back to non-encrypted mode
-    Used when client sent ENCRYPT_OFF flag
-    @param tds_sock:
-    @return:
-    """
-    enc_conn = tds_sock.conn.sock
-    clear_conn = enc_conn._transport
-    enc_conn.shutdown()
+try:
+    import OpenSSL.SSL
+    import cryptography.hazmat.backends.openssl.backend
+except ImportError:
+    OPENSSL_AVAILABLE = False
+else:
+    OPENSSL_AVAILABLE = True
+
+from . import tds_base
+
+
+BUFSIZE = 65536
+
+
+class EncryptedSocket(object):
+    def __init__(self, transport, tls_conn):
+        self._transport = transport
+        self._tls_conn = tls_conn
+
+    def gettimeout(self):
+        return self._transport.gettimeout()
+
+    def settimeout(self, timeout):
+        self._transport.settimeout(timeout)
+
+    def sendall(self, data, flags=0):
+        # TLS.Connection does not support bytearrays, need to convert to bytes first
+        if isinstance(data, bytearray):
+            data = bytes(data)
+
+        res = self._tls_conn.sendall(data)
+        buf = self._tls_conn.bio_read(BUFSIZE)
+        self._transport.sendall(buf)
+        return res
+
+    def send(self, data):
+        while True:
+            try:
+                return self._tls_conn.send(data)
+            except OpenSSL.SSL.WantWriteError:
+                buf = self._tls_conn.bio_read(BUFSIZE)
+                self._transport.sendall(buf)
+
+    def recv(self, bufsize):
+        while True:
+            try:
+                return self._tls_conn.recv(bufsize)
+            except OpenSSL.SSL.WantReadError:
+                buf = self._transport.recv(BUFSIZE)
+                self._tls_conn.bio_write(buf)
+
+    def close(self):
+        self._tls_conn.shutdown()
+        self._transport.close()
+
+    def shutdown(self):
+        self._tls_conn.shutdown()
+
+
+def verify_cb(conn, cert, err_num, err_depth, ret_code):
+    return ret_code == 1
+
+
+def validate_host(cert, name):
+    """
+    Validates host name against certificate
+
+    @param cert: Certificate returned by host
+    @param name: Actual host name used for connection
+    @return: Returns true if host name matches certificate
+    """
+    cn = None
+    for t, v in cert.get_subject().get_components():
+        if t == b'CN':
+            cn = v
+            break
+
+    # TODO check SAN extensions
+    # TODO handle wildcards
+    return cn == name
+
+
+def create_context(cafile):
+    ctx = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
+    ctx.set_options(OpenSSL.SSL.OP_NO_SSLv2)
+    ctx.set_options(OpenSSL.SSL.OP_NO_SSLv3)
+    ctx.set_verify(OpenSSL.SSL.VERIFY_PEER, verify_cb)
+    #print("verify depth:", ctx.get_verify_depth())
+    #print("verify mode:", ctx.get_verify_mode())
+    #print("openssl version:", cryptography.hazmat.backends.openssl.backend.openssl_version_text())
+    ctx.load_verify_locations(cafile=cafile)
+    return ctx
+
+
+# https://msdn.microsoft.com/en-us/library/dd357559.aspx
+def establish_channel(tds_sock):
+    w = tds_sock._writer
+    r = tds_sock._reader
+    login = tds_sock.conn._login
+
+    bhost = login.server_name.encode('ascii')
+
+    conn = OpenSSL.SSL.Connection(login.tls_ctx)
+    conn.set_tlsext_host_name(bhost)
+    conn.set_connect_state()
+    while True:
+        try:
+            conn.do_handshake()
+        except OpenSSL.SSL.WantReadError:
+            req = conn.bio_read(BUFSIZE)
+            w.begin_packet(tds_base.TDS71_PRELOGIN)
+            w.write(req)
+            w.flush()
+            resp = r.read_whole_packet()
+            # TODO validate r.packet_type
+            conn.bio_write(resp)
+        else:
+            if login.validate_host:
+                if not validate_host(cert=conn.get_peer_certificate(), name=bhost):
+                    # TODO throw correct exception class
+                    raise Exception("Certificate does not match host name '{}'".format(login.server_name))
+            tds_sock.conn.sock = EncryptedSocket(transport=tds_sock.conn.sock, tls_conn=conn)
+            return
+
+
+def revert_to_clear(tds_sock):
+    """
+    Reverts connection back to non-encrypted mode
+    Used when client sent ENCRYPT_OFF flag
+    @param tds_sock:
+    @return:
+    """
+    enc_conn = tds_sock.conn.sock
+    clear_conn = enc_conn._transport
+    enc_conn.shutdown()
     tds_sock.conn.sock = clear_conn
```

### Comparing `python-tds-1.9.0/pytds/sspi.py` & `python-tds-1.9.1/pytds/sspi.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,446 +1,446 @@
-import six
-from ctypes import c_ulong, c_ushort, c_void_p, c_ulonglong, POINTER,\
-    Structure, c_wchar_p, WINFUNCTYPE, windll, byref, cast
-
-
-class Status(object):
-    SEC_E_OK = 0
-    SEC_I_CONTINUE_NEEDED = 0x00090312
-    SEC_I_COMPLETE_AND_CONTINUE = 0x00090314
-    SEC_I_INCOMPLETE_CREDENTIALS = 0x00090320
-    SEC_E_INSUFFICIENT_MEMORY = 0x80090300 - 0x100000000
-    SEC_E_INVALID_HANDLE = 0x80090301 - 0x100000000
-    SEC_E_UNSUPPORTED_FUNCTION = 0x80090302 - 0x100000000
-    SEC_E_INTERNAL_ERROR = 0x80090304 - 0x100000000
-    SEC_E_SECPKG_NOT_FOUND = 0x80090305 - 0x100000000
-    SEC_E_NOT_OWNER = 0x80090306 - 0x100000000
-    SEC_E_INVALID_TOKEN = 0x80090308 - 0x100000000
-    SEC_E_NO_IMPERSONATION = 0x8009030B - 0x100000000
-    SEC_E_LOGON_DENIED = 0x8009030C - 0x100000000
-    SEC_E_UNKNOWN_CREDENTIALS = 0x8009030D - 0x100000000
-    SEC_E_NO_CREDENTIALS = 0x8009030E - 0x100000000
-    SEC_E_OUT_OF_SEQUENCE = 0x80090310 - 0x100000000
-    SEC_E_NO_AUTHENTICATING_AUTHORITY = 0x80090311 - 0x100000000
-    SEC_E_BUFFER_TOO_SMALL = 0x80090321 - 0x100000000
-    SEC_E_WRONG_PRINCIPAL = 0x80090322 - 0x100000000
-    SEC_E_ALGORITHM_MISMATCH = 0x80090331 - 0x100000000
-
-    @classmethod
-    def getname(cls, value):
-        for name in dir(cls):
-            if name.startswith('SEC_E_') and getattr(cls, name) == value:
-                return name
-        return 'unknown value {0:x}'.format(0x100000000 + value)
-
-#define SECBUFFER_EMPTY             0   // Undefined, replaced by provider
-#define SECBUFFER_DATA              1   // Packet data
-SECBUFFER_TOKEN = 2
-#define SECBUFFER_PKG_PARAMS        3   // Package specific parameters
-#define SECBUFFER_MISSING           4   // Missing Data indicator
-#define SECBUFFER_EXTRA             5   // Extra data
-#define SECBUFFER_STREAM_TRAILER    6   // Security Trailer
-#define SECBUFFER_STREAM_HEADER     7   // Security Header
-#define SECBUFFER_NEGOTIATION_INFO  8   // Hints from the negotiation pkg
-#define SECBUFFER_PADDING           9   // non-data padding
-#define SECBUFFER_STREAM            10  // whole encrypted message
-#define SECBUFFER_MECHLIST          11
-#define SECBUFFER_MECHLIST_SIGNATURE 12
-#define SECBUFFER_TARGET            13  // obsolete
-#define SECBUFFER_CHANNEL_BINDINGS  14
-#define SECBUFFER_CHANGE_PASS_RESPONSE 15
-#define SECBUFFER_TARGET_HOST       16
-#define SECBUFFER_ALERT             17
-
-SECPKG_CRED_INBOUND = 0x00000001
-SECPKG_CRED_OUTBOUND = 0x00000002
-SECPKG_CRED_BOTH = 0x00000003
-SECPKG_CRED_DEFAULT = 0x00000004
-SECPKG_CRED_RESERVED = 0xF0000000
-
-SECBUFFER_VERSION = 0
-
-#define ISC_REQ_DELEGATE                0x00000001
-#define ISC_REQ_MUTUAL_AUTH             0x00000002
-ISC_REQ_REPLAY_DETECT = 4
-#define ISC_REQ_SEQUENCE_DETECT         0x00000008
-ISC_REQ_CONFIDENTIALITY = 0x10
-ISC_REQ_USE_SESSION_KEY = 0x00000020
-ISC_REQ_PROMPT_FOR_CREDS = 0x00000040
-ISC_REQ_USE_SUPPLIED_CREDS = 0x00000080
-ISC_REQ_ALLOCATE_MEMORY = 0x00000100
-ISC_REQ_USE_DCE_STYLE = 0x00000200
-ISC_REQ_DATAGRAM = 0x00000400
-ISC_REQ_CONNECTION = 0x00000800
-#define ISC_REQ_CALL_LEVEL              0x00001000
-#define ISC_REQ_FRAGMENT_SUPPLIED       0x00002000
-#define ISC_REQ_EXTENDED_ERROR          0x00004000
-#define ISC_REQ_STREAM                  0x00008000
-#define ISC_REQ_INTEGRITY               0x00010000
-#define ISC_REQ_IDENTIFY                0x00020000
-#define ISC_REQ_NULL_SESSION            0x00040000
-#define ISC_REQ_MANUAL_CRED_VALIDATION  0x00080000
-#define ISC_REQ_RESERVED1               0x00100000
-#define ISC_REQ_FRAGMENT_TO_FIT         0x00200000
-#// This exists only in Windows Vista and greater
-#define ISC_REQ_FORWARD_CREDENTIALS     0x00400000
-#define ISC_REQ_NO_INTEGRITY            0x00800000 // honored only by SPNEGO
-#define ISC_REQ_USE_HTTP_STYLE          0x01000000
-#define ISC_REQ_UNVERIFIED_TARGET_NAME  0x20000000
-#define ISC_REQ_CONFIDENTIALITY_ONLY    0x40000000 // honored by SPNEGO/Kerberos
-
-SECURITY_NETWORK_DREP = 0
-SECURITY_NATIVE_DREP = 0x10
-
-SECPKG_CRED_ATTR_NAMES = 1
-
-ULONG = c_ulong
-USHORT = c_ushort
-PULONG = POINTER(ULONG)
-PVOID = c_void_p
-TimeStamp = c_ulonglong
-PTimeStamp = POINTER(c_ulonglong)
-PLUID = POINTER(c_ulonglong)
-
-
-class SecHandle(Structure):
-    _fields_ = [
-        ('lower', c_void_p),
-        ('upper', c_void_p),
-    ]
-PSecHandle = POINTER(SecHandle)
-CredHandle = SecHandle
-PCredHandle = PSecHandle
-PCtxtHandle = PSecHandle
-
-
-class SecBuffer(Structure):
-    _fields_ = [
-        ('cbBuffer', ULONG),
-        ('BufferType', ULONG),
-        ('pvBuffer', PVOID),
-    ]
-PSecBuffer = POINTER(SecBuffer)
-
-
-class SecBufferDesc(Structure):
-    _fields_ = [
-        ('ulVersion', ULONG),
-        ('cBuffers', ULONG),
-        ('pBuffers', PSecBuffer),
-    ]
-PSecBufferDesc = POINTER(SecBufferDesc)
-
-
-class SEC_WINNT_AUTH_IDENTITY(Structure):
-    _fields_ = [
-        ('User', c_wchar_p),
-        ('UserLength', c_ulong),
-        ('Domain', c_wchar_p),
-        ('DomainLength', c_ulong),
-        ('Password', c_wchar_p),
-        ('PasswordLength', c_ulong),
-        ('Flags', c_ulong),
-        ]
-
-
-class SecPkgInfo(Structure):
-    _fields_ = [
-        ('fCapabilities', ULONG),
-        ('wVersion', USHORT),
-        ('wRPCID', USHORT),
-        ('cbMaxToken', ULONG),
-        ('Name', c_wchar_p),
-        ('Comment', c_wchar_p),
-    ]
-PSecPkgInfo = POINTER(SecPkgInfo)
-
-
-class SecPkgCredentials_Names(Structure):
-    _fields_ = [('UserName', c_wchar_p)]
-
-
-def ret_val(value):
-    if value < 0:
-        raise Exception('SSPI Error {0}'.format(Status.getname(value)))
-    return value
-
-
-ENUMERATE_SECURITY_PACKAGES_FN = WINFUNCTYPE(
-    ret_val,
-    POINTER(c_ulong),
-    POINTER(POINTER(SecPkgInfo)))
-
-ACQUIRE_CREDENTIALS_HANDLE_FN = WINFUNCTYPE(
-    ret_val,
-    c_wchar_p,    # principal
-    c_wchar_p,    # package
-    ULONG,        # fCredentialUse
-    PLUID,        # pvLogonID
-    PVOID,        # pAuthData
-    PVOID,        # pGetKeyFn
-    PVOID,        # pvGetKeyArgument
-    PCredHandle,  # phCredential
-    PTimeStamp    # ptsExpiry
-    )
-FREE_CREDENTIALS_HANDLE_FN = WINFUNCTYPE(ret_val, POINTER(SecHandle))
-INITIALIZE_SECURITY_CONTEXT_FN = WINFUNCTYPE(
-    ret_val,
-    PCredHandle,
-    PCtxtHandle,     # phContext,
-    c_wchar_p,       # pszTargetName,
-    ULONG,           # fContextReq,
-    ULONG,           # Reserved1,
-    ULONG,           # TargetDataRep,
-    PSecBufferDesc,  # pInput,
-    ULONG,           # Reserved2,
-    PCtxtHandle,     # phNewContext,
-    PSecBufferDesc,  # pOutput,
-    PULONG,          # pfContextAttr,
-    PTimeStamp,      # ptsExpiry
-    )
-COMPLETE_AUTH_TOKEN_FN = WINFUNCTYPE(
-    ret_val,
-    PCtxtHandle,     # phContext
-    PSecBufferDesc,  # pToken
-    )
-
-FREE_CONTEXT_BUFFER_FN = WINFUNCTYPE(ret_val, PVOID)
-
-QUERY_CREDENTIAL_ATTRIBUTES_FN = WINFUNCTYPE(
-    ret_val,
-    PCredHandle,    # cred
-    ULONG,          # attribute
-    PVOID,          # out buffer
-    )
-ACCEPT_SECURITY_CONTEXT_FN = PVOID
-DELETE_SECURITY_CONTEXT_FN = WINFUNCTYPE(ret_val, PCtxtHandle)
-APPLY_CONTROL_TOKEN_FN = PVOID
-QUERY_CONTEXT_ATTRIBUTES_FN = PVOID
-IMPERSONATE_SECURITY_CONTEXT_FN = PVOID
-REVERT_SECURITY_CONTEXT_FN = PVOID
-MAKE_SIGNATURE_FN = PVOID
-VERIFY_SIGNATURE_FN = PVOID
-QUERY_SECURITY_PACKAGE_INFO_FN = WINFUNCTYPE(
-    ret_val,
-    c_wchar_p,  # package name
-    POINTER(PSecPkgInfo),
-    )
-EXPORT_SECURITY_CONTEXT_FN = PVOID
-IMPORT_SECURITY_CONTEXT_FN = PVOID
-ADD_CREDENTIALS_FN = PVOID
-QUERY_SECURITY_CONTEXT_TOKEN_FN = PVOID
-ENCRYPT_MESSAGE_FN = PVOID
-DECRYPT_MESSAGE_FN = PVOID
-SET_CONTEXT_ATTRIBUTES_FN = PVOID
-
-
-class SECURITY_FUNCTION_TABLE(Structure):
-    _fields_ = [
-        ('dwVersion', c_ulong),
-        ('EnumerateSecurityPackages', ENUMERATE_SECURITY_PACKAGES_FN),
-        ('QueryCredentialsAttributes', QUERY_CREDENTIAL_ATTRIBUTES_FN),
-        ('AcquireCredentialsHandle', ACQUIRE_CREDENTIALS_HANDLE_FN),
-        ('FreeCredentialsHandle', FREE_CREDENTIALS_HANDLE_FN),
-        ('Reserved2', c_void_p),
-        ('InitializeSecurityContext', INITIALIZE_SECURITY_CONTEXT_FN),
-        ('AcceptSecurityContext', ACCEPT_SECURITY_CONTEXT_FN),
-        ('CompleteAuthToken', COMPLETE_AUTH_TOKEN_FN),
-        ('DeleteSecurityContext', DELETE_SECURITY_CONTEXT_FN),
-        ('ApplyControlToken', APPLY_CONTROL_TOKEN_FN),
-        ('QueryContextAttributes', QUERY_CONTEXT_ATTRIBUTES_FN),
-        ('ImpersonateSecurityContext', IMPERSONATE_SECURITY_CONTEXT_FN),
-        ('RevertSecurityContext', REVERT_SECURITY_CONTEXT_FN),
-        ('MakeSignature', MAKE_SIGNATURE_FN),
-        ('VerifySignature', VERIFY_SIGNATURE_FN),
-        ('FreeContextBuffer', FREE_CONTEXT_BUFFER_FN),
-        ('QuerySecurityPackageInfo', QUERY_SECURITY_PACKAGE_INFO_FN),
-        ('Reserved3', c_void_p),
-        ('Reserved4', c_void_p),
-        ('ExportSecurityContext', EXPORT_SECURITY_CONTEXT_FN),
-        ('ImportSecurityContext', IMPORT_SECURITY_CONTEXT_FN),
-        ('AddCredentials', ADD_CREDENTIALS_FN),
-        ('Reserved8', c_void_p),
-        ('QuerySecurityContextToken', QUERY_SECURITY_CONTEXT_TOKEN_FN),
-        ('EncryptMessage', ENCRYPT_MESSAGE_FN),
-        ('DecryptMessage', DECRYPT_MESSAGE_FN),
-        ('SetContextAttributes', SET_CONTEXT_ATTRIBUTES_FN),
-        ]
-
-_PInitSecurityInterface = WINFUNCTYPE(POINTER(SECURITY_FUNCTION_TABLE))
-InitSecurityInterface = _PInitSecurityInterface(('InitSecurityInterfaceW', windll.secur32))
-
-sec_fn = InitSecurityInterface()
-if not sec_fn:
-    raise Exception('InitSecurityInterface failed')
-sec_fn = sec_fn.contents
-
-
-class _SecContext(object):
-    def close(self):
-        if self._handle.lower and self._handle.upper:
-            sec_fn.DeleteSecurityContext(self._handle)
-            self._handle.lower = self._handle.upper = 0
-
-    def __del__(self):
-        self.close()
-
-    def complete_auth_token(self, bufs):
-        sec_fn.CompleteAuthToken(
-            byref(self._handle),
-            byref(_make_buffers_desc(bufs)))
-
-    def next(self,
-             flags,
-             target_name=None,
-             byte_ordering='network',
-             input_buffers=None,
-             output_buffers=None):
-        input_buffers_desc = _make_buffers_desc(input_buffers) if input_buffers else None
-        output_buffers_desc = _make_buffers_desc(output_buffers) if output_buffers else None
-        status = sec_fn.InitializeSecurityContext(
-            byref(self._cred._handle),
-            byref(self._handle),
-            target_name,
-            flags,
-            0,
-            SECURITY_NETWORK_DREP if byte_ordering == 'network' else SECURITY_NATIVE_DREP,
-            byref(input_buffers_desc) if input_buffers_desc else None,
-            0,
-            byref(self._handle),
-            byref(output_buffers_desc) if input_buffers_desc else None,
-            byref(self._attrs),
-            byref(self._ts))
-        result_buffers = []
-        for i, (type, buf) in enumerate(output_buffers):
-            buf = buf[:output_buffers_desc.pBuffers[i].cbBuffer]
-            result_buffers.append((type, buf))
-        return status, result_buffers
-
-
-class SspiCredentials(object):
-    def __init__(self, package, use, identity=None):
-        self._handle = SecHandle()
-        self._ts = TimeStamp()
-        sec_fn.AcquireCredentialsHandle(
-            None, package, use,
-            None, byref(identity) if identity and identity.Domain else None,
-            None, None, byref(self._handle), byref(self._ts))
-
-    def close(self):
-        if self._handle.lower or self._handle.upper:
-            sec_fn.FreeCredentialsHandle(byref(self._handle))
-            self._handle.lower = 0
-            self._handle.upper = 0
-
-    def __del__(self):
-        self.close()
-
-    def query_user_name(self):
-        names = SecPkgCredentials_Names()
-        try:
-            sec_fn.QueryCredentialsAttributes(
-                byref(self._handle),
-                SECPKG_CRED_ATTR_NAMES,
-                byref(names))
-            user_name = six.text_type(names.UserName)
-        finally:
-            p = c_wchar_p.from_buffer(names, SecPkgCredentials_Names.UserName.offset)
-            sec_fn.FreeContextBuffer(p)
-        return user_name
-
-    def create_context(
-            self,
-            flags,
-            target_name=None,
-            byte_ordering='network',
-            input_buffers=None,
-            output_buffers=None):
-        ctx = _SecContext()
-        ctx._cred = self
-        ctx._handle = SecHandle()
-        ctx._ts = TimeStamp()
-        ctx._attrs = ULONG()
-        input_buffers_desc = _make_buffers_desc(input_buffers) if input_buffers else None
-        output_buffers_desc = _make_buffers_desc(output_buffers) if output_buffers else None
-        status = sec_fn.InitializeSecurityContext(
-            byref(self._handle),
-            None,
-            target_name,
-            flags,
-            0,
-            SECURITY_NETWORK_DREP if byte_ordering == 'network' else SECURITY_NATIVE_DREP,
-            byref(input_buffers_desc) if input_buffers_desc else None,
-            0,
-            byref(ctx._handle),
-            byref(output_buffers_desc) if output_buffers_desc else None,
-            byref(ctx._attrs),
-            byref(ctx._ts))
-        result_buffers = []
-        for i, (type, buf) in enumerate(output_buffers):
-            buf = buf[:output_buffers_desc.pBuffers[i].cbBuffer]
-            result_buffers.append((type, buf))
-        return ctx, status, result_buffers
-
-
-def _make_buffers_desc(buffers):
-    desc = SecBufferDesc()
-    desc.ulVersion = SECBUFFER_VERSION
-    bufs_array = (SecBuffer * len(buffers))()
-    for i, (type, buf) in enumerate(buffers):
-        bufs_array[i].BufferType = type
-        bufs_array[i].cbBuffer = len(buf)
-        bufs_array[i].pvBuffer = cast(buf, PVOID)
-    desc.pBuffers = bufs_array
-    desc.cBuffers = len(buffers)
-    return desc
-
-
-def make_winnt_identity(domain, user_name, password):
-    identity = SEC_WINNT_AUTH_IDENTITY()
-    identity.Flags = 2  # SEC_WINNT_AUTH_IDENTITY_UNICODE
-    identity.Password = password
-    identity.PasswordLength = len(password)
-    identity.Domain = domain
-    identity.DomainLength = len(domain)
-    identity.User = user_name
-    identity.UserLength = len(user_name)
-    return identity
-
-#class SspiSecBuffer(object):
-#    def __init__(self, type, buflen=4096):
-#        self._buf = create_string_buffer(int(buflen))
-#        self._desc = SecBuffer()
-#        self._desc.cbBuffer = buflen
-#        self._desc.BufferType = type
-#        self._desc.pvBuffer = cast(self._buf, PVOID)
-#
-#class SspiSecBuffers(object):
-#    def __init__(self):
-#        self._desc = SecBufferDesc()
-#        self._desc.ulVersion = SECBUFFER_VERSION
-#        self._descrs = (SecBuffer * 8)()
-#        self._desc.pBuffers = self._descrs
-#
-#    def append(self, buf):
-#        if len(self._descrs) <= self._desc.cBuffers:
-#            newdescrs = (SecBuffer * (len(self._descrs) * 2))(*self._descrs)
-#            self._descrs = newdescrs
-#            self._desc.pBuffers = newdescrs
-#        self._descrs[self._desc.cBuffers] = buf._desc
-#        self._desc.cBuffers += 1
-
-
-def enum_security_packages():
-    num = ULONG()
-    infos = POINTER(SecPkgInfo)()
-    status = sec_fn.EnumerateSecurityPackages(byref(num), byref(infos))
-    try:
-        return [{'caps': infos[i].fCapabilities,
-                 'version': infos[i].wVersion,
-                 'rpcid': infos[i].wRPCID,
-                 'max_token': infos[i].cbMaxToken,
-                 'name': infos[i].Name,
-                 'comment': infos[i].Comment,
-                 } for i in range(num.value)]
-    finally:
-        sec_fn.FreeContextBuffer(infos)
+import six
+from ctypes import c_ulong, c_ushort, c_void_p, c_ulonglong, POINTER,\
+    Structure, c_wchar_p, WINFUNCTYPE, windll, byref, cast
+
+
+class Status(object):
+    SEC_E_OK = 0
+    SEC_I_CONTINUE_NEEDED = 0x00090312
+    SEC_I_COMPLETE_AND_CONTINUE = 0x00090314
+    SEC_I_INCOMPLETE_CREDENTIALS = 0x00090320
+    SEC_E_INSUFFICIENT_MEMORY = 0x80090300 - 0x100000000
+    SEC_E_INVALID_HANDLE = 0x80090301 - 0x100000000
+    SEC_E_UNSUPPORTED_FUNCTION = 0x80090302 - 0x100000000
+    SEC_E_INTERNAL_ERROR = 0x80090304 - 0x100000000
+    SEC_E_SECPKG_NOT_FOUND = 0x80090305 - 0x100000000
+    SEC_E_NOT_OWNER = 0x80090306 - 0x100000000
+    SEC_E_INVALID_TOKEN = 0x80090308 - 0x100000000
+    SEC_E_NO_IMPERSONATION = 0x8009030B - 0x100000000
+    SEC_E_LOGON_DENIED = 0x8009030C - 0x100000000
+    SEC_E_UNKNOWN_CREDENTIALS = 0x8009030D - 0x100000000
+    SEC_E_NO_CREDENTIALS = 0x8009030E - 0x100000000
+    SEC_E_OUT_OF_SEQUENCE = 0x80090310 - 0x100000000
+    SEC_E_NO_AUTHENTICATING_AUTHORITY = 0x80090311 - 0x100000000
+    SEC_E_BUFFER_TOO_SMALL = 0x80090321 - 0x100000000
+    SEC_E_WRONG_PRINCIPAL = 0x80090322 - 0x100000000
+    SEC_E_ALGORITHM_MISMATCH = 0x80090331 - 0x100000000
+
+    @classmethod
+    def getname(cls, value):
+        for name in dir(cls):
+            if name.startswith('SEC_E_') and getattr(cls, name) == value:
+                return name
+        return 'unknown value {0:x}'.format(0x100000000 + value)
+
+#define SECBUFFER_EMPTY             0   // Undefined, replaced by provider
+#define SECBUFFER_DATA              1   // Packet data
+SECBUFFER_TOKEN = 2
+#define SECBUFFER_PKG_PARAMS        3   // Package specific parameters
+#define SECBUFFER_MISSING           4   // Missing Data indicator
+#define SECBUFFER_EXTRA             5   // Extra data
+#define SECBUFFER_STREAM_TRAILER    6   // Security Trailer
+#define SECBUFFER_STREAM_HEADER     7   // Security Header
+#define SECBUFFER_NEGOTIATION_INFO  8   // Hints from the negotiation pkg
+#define SECBUFFER_PADDING           9   // non-data padding
+#define SECBUFFER_STREAM            10  // whole encrypted message
+#define SECBUFFER_MECHLIST          11
+#define SECBUFFER_MECHLIST_SIGNATURE 12
+#define SECBUFFER_TARGET            13  // obsolete
+#define SECBUFFER_CHANNEL_BINDINGS  14
+#define SECBUFFER_CHANGE_PASS_RESPONSE 15
+#define SECBUFFER_TARGET_HOST       16
+#define SECBUFFER_ALERT             17
+
+SECPKG_CRED_INBOUND = 0x00000001
+SECPKG_CRED_OUTBOUND = 0x00000002
+SECPKG_CRED_BOTH = 0x00000003
+SECPKG_CRED_DEFAULT = 0x00000004
+SECPKG_CRED_RESERVED = 0xF0000000
+
+SECBUFFER_VERSION = 0
+
+#define ISC_REQ_DELEGATE                0x00000001
+#define ISC_REQ_MUTUAL_AUTH             0x00000002
+ISC_REQ_REPLAY_DETECT = 4
+#define ISC_REQ_SEQUENCE_DETECT         0x00000008
+ISC_REQ_CONFIDENTIALITY = 0x10
+ISC_REQ_USE_SESSION_KEY = 0x00000020
+ISC_REQ_PROMPT_FOR_CREDS = 0x00000040
+ISC_REQ_USE_SUPPLIED_CREDS = 0x00000080
+ISC_REQ_ALLOCATE_MEMORY = 0x00000100
+ISC_REQ_USE_DCE_STYLE = 0x00000200
+ISC_REQ_DATAGRAM = 0x00000400
+ISC_REQ_CONNECTION = 0x00000800
+#define ISC_REQ_CALL_LEVEL              0x00001000
+#define ISC_REQ_FRAGMENT_SUPPLIED       0x00002000
+#define ISC_REQ_EXTENDED_ERROR          0x00004000
+#define ISC_REQ_STREAM                  0x00008000
+#define ISC_REQ_INTEGRITY               0x00010000
+#define ISC_REQ_IDENTIFY                0x00020000
+#define ISC_REQ_NULL_SESSION            0x00040000
+#define ISC_REQ_MANUAL_CRED_VALIDATION  0x00080000
+#define ISC_REQ_RESERVED1               0x00100000
+#define ISC_REQ_FRAGMENT_TO_FIT         0x00200000
+#// This exists only in Windows Vista and greater
+#define ISC_REQ_FORWARD_CREDENTIALS     0x00400000
+#define ISC_REQ_NO_INTEGRITY            0x00800000 // honored only by SPNEGO
+#define ISC_REQ_USE_HTTP_STYLE          0x01000000
+#define ISC_REQ_UNVERIFIED_TARGET_NAME  0x20000000
+#define ISC_REQ_CONFIDENTIALITY_ONLY    0x40000000 // honored by SPNEGO/Kerberos
+
+SECURITY_NETWORK_DREP = 0
+SECURITY_NATIVE_DREP = 0x10
+
+SECPKG_CRED_ATTR_NAMES = 1
+
+ULONG = c_ulong
+USHORT = c_ushort
+PULONG = POINTER(ULONG)
+PVOID = c_void_p
+TimeStamp = c_ulonglong
+PTimeStamp = POINTER(c_ulonglong)
+PLUID = POINTER(c_ulonglong)
+
+
+class SecHandle(Structure):
+    _fields_ = [
+        ('lower', c_void_p),
+        ('upper', c_void_p),
+    ]
+PSecHandle = POINTER(SecHandle)
+CredHandle = SecHandle
+PCredHandle = PSecHandle
+PCtxtHandle = PSecHandle
+
+
+class SecBuffer(Structure):
+    _fields_ = [
+        ('cbBuffer', ULONG),
+        ('BufferType', ULONG),
+        ('pvBuffer', PVOID),
+    ]
+PSecBuffer = POINTER(SecBuffer)
+
+
+class SecBufferDesc(Structure):
+    _fields_ = [
+        ('ulVersion', ULONG),
+        ('cBuffers', ULONG),
+        ('pBuffers', PSecBuffer),
+    ]
+PSecBufferDesc = POINTER(SecBufferDesc)
+
+
+class SEC_WINNT_AUTH_IDENTITY(Structure):
+    _fields_ = [
+        ('User', c_wchar_p),
+        ('UserLength', c_ulong),
+        ('Domain', c_wchar_p),
+        ('DomainLength', c_ulong),
+        ('Password', c_wchar_p),
+        ('PasswordLength', c_ulong),
+        ('Flags', c_ulong),
+        ]
+
+
+class SecPkgInfo(Structure):
+    _fields_ = [
+        ('fCapabilities', ULONG),
+        ('wVersion', USHORT),
+        ('wRPCID', USHORT),
+        ('cbMaxToken', ULONG),
+        ('Name', c_wchar_p),
+        ('Comment', c_wchar_p),
+    ]
+PSecPkgInfo = POINTER(SecPkgInfo)
+
+
+class SecPkgCredentials_Names(Structure):
+    _fields_ = [('UserName', c_wchar_p)]
+
+
+def ret_val(value):
+    if value < 0:
+        raise Exception('SSPI Error {0}'.format(Status.getname(value)))
+    return value
+
+
+ENUMERATE_SECURITY_PACKAGES_FN = WINFUNCTYPE(
+    ret_val,
+    POINTER(c_ulong),
+    POINTER(POINTER(SecPkgInfo)))
+
+ACQUIRE_CREDENTIALS_HANDLE_FN = WINFUNCTYPE(
+    ret_val,
+    c_wchar_p,    # principal
+    c_wchar_p,    # package
+    ULONG,        # fCredentialUse
+    PLUID,        # pvLogonID
+    PVOID,        # pAuthData
+    PVOID,        # pGetKeyFn
+    PVOID,        # pvGetKeyArgument
+    PCredHandle,  # phCredential
+    PTimeStamp    # ptsExpiry
+    )
+FREE_CREDENTIALS_HANDLE_FN = WINFUNCTYPE(ret_val, POINTER(SecHandle))
+INITIALIZE_SECURITY_CONTEXT_FN = WINFUNCTYPE(
+    ret_val,
+    PCredHandle,
+    PCtxtHandle,     # phContext,
+    c_wchar_p,       # pszTargetName,
+    ULONG,           # fContextReq,
+    ULONG,           # Reserved1,
+    ULONG,           # TargetDataRep,
+    PSecBufferDesc,  # pInput,
+    ULONG,           # Reserved2,
+    PCtxtHandle,     # phNewContext,
+    PSecBufferDesc,  # pOutput,
+    PULONG,          # pfContextAttr,
+    PTimeStamp,      # ptsExpiry
+    )
+COMPLETE_AUTH_TOKEN_FN = WINFUNCTYPE(
+    ret_val,
+    PCtxtHandle,     # phContext
+    PSecBufferDesc,  # pToken
+    )
+
+FREE_CONTEXT_BUFFER_FN = WINFUNCTYPE(ret_val, PVOID)
+
+QUERY_CREDENTIAL_ATTRIBUTES_FN = WINFUNCTYPE(
+    ret_val,
+    PCredHandle,    # cred
+    ULONG,          # attribute
+    PVOID,          # out buffer
+    )
+ACCEPT_SECURITY_CONTEXT_FN = PVOID
+DELETE_SECURITY_CONTEXT_FN = WINFUNCTYPE(ret_val, PCtxtHandle)
+APPLY_CONTROL_TOKEN_FN = PVOID
+QUERY_CONTEXT_ATTRIBUTES_FN = PVOID
+IMPERSONATE_SECURITY_CONTEXT_FN = PVOID
+REVERT_SECURITY_CONTEXT_FN = PVOID
+MAKE_SIGNATURE_FN = PVOID
+VERIFY_SIGNATURE_FN = PVOID
+QUERY_SECURITY_PACKAGE_INFO_FN = WINFUNCTYPE(
+    ret_val,
+    c_wchar_p,  # package name
+    POINTER(PSecPkgInfo),
+    )
+EXPORT_SECURITY_CONTEXT_FN = PVOID
+IMPORT_SECURITY_CONTEXT_FN = PVOID
+ADD_CREDENTIALS_FN = PVOID
+QUERY_SECURITY_CONTEXT_TOKEN_FN = PVOID
+ENCRYPT_MESSAGE_FN = PVOID
+DECRYPT_MESSAGE_FN = PVOID
+SET_CONTEXT_ATTRIBUTES_FN = PVOID
+
+
+class SECURITY_FUNCTION_TABLE(Structure):
+    _fields_ = [
+        ('dwVersion', c_ulong),
+        ('EnumerateSecurityPackages', ENUMERATE_SECURITY_PACKAGES_FN),
+        ('QueryCredentialsAttributes', QUERY_CREDENTIAL_ATTRIBUTES_FN),
+        ('AcquireCredentialsHandle', ACQUIRE_CREDENTIALS_HANDLE_FN),
+        ('FreeCredentialsHandle', FREE_CREDENTIALS_HANDLE_FN),
+        ('Reserved2', c_void_p),
+        ('InitializeSecurityContext', INITIALIZE_SECURITY_CONTEXT_FN),
+        ('AcceptSecurityContext', ACCEPT_SECURITY_CONTEXT_FN),
+        ('CompleteAuthToken', COMPLETE_AUTH_TOKEN_FN),
+        ('DeleteSecurityContext', DELETE_SECURITY_CONTEXT_FN),
+        ('ApplyControlToken', APPLY_CONTROL_TOKEN_FN),
+        ('QueryContextAttributes', QUERY_CONTEXT_ATTRIBUTES_FN),
+        ('ImpersonateSecurityContext', IMPERSONATE_SECURITY_CONTEXT_FN),
+        ('RevertSecurityContext', REVERT_SECURITY_CONTEXT_FN),
+        ('MakeSignature', MAKE_SIGNATURE_FN),
+        ('VerifySignature', VERIFY_SIGNATURE_FN),
+        ('FreeContextBuffer', FREE_CONTEXT_BUFFER_FN),
+        ('QuerySecurityPackageInfo', QUERY_SECURITY_PACKAGE_INFO_FN),
+        ('Reserved3', c_void_p),
+        ('Reserved4', c_void_p),
+        ('ExportSecurityContext', EXPORT_SECURITY_CONTEXT_FN),
+        ('ImportSecurityContext', IMPORT_SECURITY_CONTEXT_FN),
+        ('AddCredentials', ADD_CREDENTIALS_FN),
+        ('Reserved8', c_void_p),
+        ('QuerySecurityContextToken', QUERY_SECURITY_CONTEXT_TOKEN_FN),
+        ('EncryptMessage', ENCRYPT_MESSAGE_FN),
+        ('DecryptMessage', DECRYPT_MESSAGE_FN),
+        ('SetContextAttributes', SET_CONTEXT_ATTRIBUTES_FN),
+        ]
+
+_PInitSecurityInterface = WINFUNCTYPE(POINTER(SECURITY_FUNCTION_TABLE))
+InitSecurityInterface = _PInitSecurityInterface(('InitSecurityInterfaceW', windll.secur32))
+
+sec_fn = InitSecurityInterface()
+if not sec_fn:
+    raise Exception('InitSecurityInterface failed')
+sec_fn = sec_fn.contents
+
+
+class _SecContext(object):
+    def close(self):
+        if self._handle.lower and self._handle.upper:
+            sec_fn.DeleteSecurityContext(self._handle)
+            self._handle.lower = self._handle.upper = 0
+
+    def __del__(self):
+        self.close()
+
+    def complete_auth_token(self, bufs):
+        sec_fn.CompleteAuthToken(
+            byref(self._handle),
+            byref(_make_buffers_desc(bufs)))
+
+    def next(self,
+             flags,
+             target_name=None,
+             byte_ordering='network',
+             input_buffers=None,
+             output_buffers=None):
+        input_buffers_desc = _make_buffers_desc(input_buffers) if input_buffers else None
+        output_buffers_desc = _make_buffers_desc(output_buffers) if output_buffers else None
+        status = sec_fn.InitializeSecurityContext(
+            byref(self._cred._handle),
+            byref(self._handle),
+            target_name,
+            flags,
+            0,
+            SECURITY_NETWORK_DREP if byte_ordering == 'network' else SECURITY_NATIVE_DREP,
+            byref(input_buffers_desc) if input_buffers_desc else None,
+            0,
+            byref(self._handle),
+            byref(output_buffers_desc) if input_buffers_desc else None,
+            byref(self._attrs),
+            byref(self._ts))
+        result_buffers = []
+        for i, (type, buf) in enumerate(output_buffers):
+            buf = buf[:output_buffers_desc.pBuffers[i].cbBuffer]
+            result_buffers.append((type, buf))
+        return status, result_buffers
+
+
+class SspiCredentials(object):
+    def __init__(self, package, use, identity=None):
+        self._handle = SecHandle()
+        self._ts = TimeStamp()
+        sec_fn.AcquireCredentialsHandle(
+            None, package, use,
+            None, byref(identity) if identity and identity.Domain else None,
+            None, None, byref(self._handle), byref(self._ts))
+
+    def close(self):
+        if self._handle.lower or self._handle.upper:
+            sec_fn.FreeCredentialsHandle(byref(self._handle))
+            self._handle.lower = 0
+            self._handle.upper = 0
+
+    def __del__(self):
+        self.close()
+
+    def query_user_name(self):
+        names = SecPkgCredentials_Names()
+        try:
+            sec_fn.QueryCredentialsAttributes(
+                byref(self._handle),
+                SECPKG_CRED_ATTR_NAMES,
+                byref(names))
+            user_name = six.text_type(names.UserName)
+        finally:
+            p = c_wchar_p.from_buffer(names, SecPkgCredentials_Names.UserName.offset)
+            sec_fn.FreeContextBuffer(p)
+        return user_name
+
+    def create_context(
+            self,
+            flags,
+            target_name=None,
+            byte_ordering='network',
+            input_buffers=None,
+            output_buffers=None):
+        ctx = _SecContext()
+        ctx._cred = self
+        ctx._handle = SecHandle()
+        ctx._ts = TimeStamp()
+        ctx._attrs = ULONG()
+        input_buffers_desc = _make_buffers_desc(input_buffers) if input_buffers else None
+        output_buffers_desc = _make_buffers_desc(output_buffers) if output_buffers else None
+        status = sec_fn.InitializeSecurityContext(
+            byref(self._handle),
+            None,
+            target_name,
+            flags,
+            0,
+            SECURITY_NETWORK_DREP if byte_ordering == 'network' else SECURITY_NATIVE_DREP,
+            byref(input_buffers_desc) if input_buffers_desc else None,
+            0,
+            byref(ctx._handle),
+            byref(output_buffers_desc) if output_buffers_desc else None,
+            byref(ctx._attrs),
+            byref(ctx._ts))
+        result_buffers = []
+        for i, (type, buf) in enumerate(output_buffers):
+            buf = buf[:output_buffers_desc.pBuffers[i].cbBuffer]
+            result_buffers.append((type, buf))
+        return ctx, status, result_buffers
+
+
+def _make_buffers_desc(buffers):
+    desc = SecBufferDesc()
+    desc.ulVersion = SECBUFFER_VERSION
+    bufs_array = (SecBuffer * len(buffers))()
+    for i, (type, buf) in enumerate(buffers):
+        bufs_array[i].BufferType = type
+        bufs_array[i].cbBuffer = len(buf)
+        bufs_array[i].pvBuffer = cast(buf, PVOID)
+    desc.pBuffers = bufs_array
+    desc.cBuffers = len(buffers)
+    return desc
+
+
+def make_winnt_identity(domain, user_name, password):
+    identity = SEC_WINNT_AUTH_IDENTITY()
+    identity.Flags = 2  # SEC_WINNT_AUTH_IDENTITY_UNICODE
+    identity.Password = password
+    identity.PasswordLength = len(password)
+    identity.Domain = domain
+    identity.DomainLength = len(domain)
+    identity.User = user_name
+    identity.UserLength = len(user_name)
+    return identity
+
+#class SspiSecBuffer(object):
+#    def __init__(self, type, buflen=4096):
+#        self._buf = create_string_buffer(int(buflen))
+#        self._desc = SecBuffer()
+#        self._desc.cbBuffer = buflen
+#        self._desc.BufferType = type
+#        self._desc.pvBuffer = cast(self._buf, PVOID)
+#
+#class SspiSecBuffers(object):
+#    def __init__(self):
+#        self._desc = SecBufferDesc()
+#        self._desc.ulVersion = SECBUFFER_VERSION
+#        self._descrs = (SecBuffer * 8)()
+#        self._desc.pBuffers = self._descrs
+#
+#    def append(self, buf):
+#        if len(self._descrs) <= self._desc.cBuffers:
+#            newdescrs = (SecBuffer * (len(self._descrs) * 2))(*self._descrs)
+#            self._descrs = newdescrs
+#            self._desc.pBuffers = newdescrs
+#        self._descrs[self._desc.cBuffers] = buf._desc
+#        self._desc.cBuffers += 1
+
+
+def enum_security_packages():
+    num = ULONG()
+    infos = POINTER(SecPkgInfo)()
+    status = sec_fn.EnumerateSecurityPackages(byref(num), byref(infos))
+    try:
+        return [{'caps': infos[i].fCapabilities,
+                 'version': infos[i].wVersion,
+                 'rpcid': infos[i].wRPCID,
+                 'max_token': infos[i].cbMaxToken,
+                 'name': infos[i].Name,
+                 'comment': infos[i].Comment,
+                 } for i in range(num.value)]
+    finally:
+        sec_fn.FreeContextBuffer(infos)
```

### Comparing `python-tds-1.9.0/pytds/login.py` & `python-tds-1.9.1/pytds/login.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-# vim: set fileencoding=utf8 :
-"""
-.. module:: login
-   :platform: Unix, Windows, MacOSX
-   :synopsis: Login classes
-
-.. moduleauthor:: Mikhail Denisenko <denisenkom@gmail.com>
-"""
-import socket
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-class SspiAuth(object):
-    """ SSPI authentication
-
-    :platform: Windows
-
-    Required parameters are server_name and port or spn
-
-    :keyword user_name: User name, if not provided current security context will be used
-    :type user_name: str
-    :keyword password: User password, if not provided current security context will be used
-    :type password: str
-    :keyword server_name: MSSQL server host name
-    :type server_name: str
-    :keyword port: MSSQL server port
-    :type port: int
-    :keyword spn: Service name
-    :type spn: str
-    """
-    def __init__(self, user_name='', password='', server_name='', port=None, spn=None):
-        from . import sspi
-        # parse username/password informations
-        if '\\' in user_name:
-            domain, user_name = user_name.split('\\')
-        else:
-            domain = ''
-        if domain and user_name:
-            self._identity = sspi.make_winnt_identity(
-                domain,
-                user_name,
-                password)
-        else:
-            self._identity = None
-        # build SPN
-        if spn:
-            self._sname = spn
-        else:
-            primary_host_name, _, _ = socket.gethostbyname_ex(server_name)
-            self._sname = 'MSSQLSvc/{0}:{1}'.format(primary_host_name, port)
-
-        # using Negotiate system will use proper protocol (either NTLM or Kerberos)
-        self._cred = sspi.SspiCredentials(
-            package='Negotiate',
-            use=sspi.SECPKG_CRED_OUTBOUND,
-            identity=self._identity)
-
-        self._flags = sspi.ISC_REQ_CONFIDENTIALITY | sspi.ISC_REQ_REPLAY_DETECT | sspi.ISC_REQ_CONNECTION
-        self._ctx = None
-
-    def create_packet(self):
-        from . import sspi
-        import ctypes
-        buf = ctypes.create_string_buffer(4096)
-        self._ctx, status, bufs = self._cred.create_context(
-            flags=self._flags,
-            byte_ordering='network',
-            target_name=self._sname,
-            output_buffers=[(sspi.SECBUFFER_TOKEN, buf)])
-        if status == sspi.Status.SEC_I_COMPLETE_AND_CONTINUE:
-            self._ctx.complete_auth_token(bufs)
-        return bufs[0][1]
-
-    def handle_next(self, packet):
-        from . import sspi
-        import ctypes
-        buf = ctypes.create_string_buffer(4096)
-        status, buffers = self._ctx.next(
-            flags=self._flags,
-            byte_ordering='network',
-            target_name=self._sname,
-            input_buffers=[(sspi.SECBUFFER_TOKEN, packet)],
-            output_buffers=[(sspi.SECBUFFER_TOKEN, buf)])
-        return buffers[0][1]
-
-    def close(self):
-        self._ctx.close()
-        self._cred.close()
-
-
-class NtlmAuth(object):
-    """ NTLM authentication, uses Python implementation
-
-    :param user_name: User name
-    :type user_name: str
-    :param password: User password
-    :type password: str
-    """
-    def __init__(self, user_name, password):
-        if '\\' in user_name:
-            self._domain, self._user = user_name.split('\\', 1)
-        else:
-            self._domain = 'workspace'
-            self._user = user_name
-        self._password = password
-
-    def create_packet(self):
-        from . import ntlm
-        return ntlm.create_NTLM_NEGOTIATE_MESSAGE_raw(socket.gethostname(), self._domain)
-
-    def handle_next(self, packet):
-        from . import ntlm
-        nonce, flags = ntlm.parse_NTLM_CHALLENGE_MESSAGE_raw(packet)
-        return ntlm.create_NTLM_AUTHENTICATE_MESSAGE_raw(nonce, self._user, self._domain, self._password, flags)
-
-    def close(self):
-        pass
+# vim: set fileencoding=utf8 :
+"""
+.. module:: login
+   :platform: Unix, Windows, MacOSX
+   :synopsis: Login classes
+
+.. moduleauthor:: Mikhail Denisenko <denisenkom@gmail.com>
+"""
+import socket
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+class SspiAuth(object):
+    """ SSPI authentication
+
+    :platform: Windows
+
+    Required parameters are server_name and port or spn
+
+    :keyword user_name: User name, if not provided current security context will be used
+    :type user_name: str
+    :keyword password: User password, if not provided current security context will be used
+    :type password: str
+    :keyword server_name: MSSQL server host name
+    :type server_name: str
+    :keyword port: MSSQL server port
+    :type port: int
+    :keyword spn: Service name
+    :type spn: str
+    """
+    def __init__(self, user_name='', password='', server_name='', port=None, spn=None):
+        from . import sspi
+        # parse username/password informations
+        if '\\' in user_name:
+            domain, user_name = user_name.split('\\')
+        else:
+            domain = ''
+        if domain and user_name:
+            self._identity = sspi.make_winnt_identity(
+                domain,
+                user_name,
+                password)
+        else:
+            self._identity = None
+        # build SPN
+        if spn:
+            self._sname = spn
+        else:
+            primary_host_name, _, _ = socket.gethostbyname_ex(server_name)
+            self._sname = 'MSSQLSvc/{0}:{1}'.format(primary_host_name, port)
+
+        # using Negotiate system will use proper protocol (either NTLM or Kerberos)
+        self._cred = sspi.SspiCredentials(
+            package='Negotiate',
+            use=sspi.SECPKG_CRED_OUTBOUND,
+            identity=self._identity)
+
+        self._flags = sspi.ISC_REQ_CONFIDENTIALITY | sspi.ISC_REQ_REPLAY_DETECT | sspi.ISC_REQ_CONNECTION
+        self._ctx = None
+
+    def create_packet(self):
+        from . import sspi
+        import ctypes
+        buf = ctypes.create_string_buffer(4096)
+        self._ctx, status, bufs = self._cred.create_context(
+            flags=self._flags,
+            byte_ordering='network',
+            target_name=self._sname,
+            output_buffers=[(sspi.SECBUFFER_TOKEN, buf)])
+        if status == sspi.Status.SEC_I_COMPLETE_AND_CONTINUE:
+            self._ctx.complete_auth_token(bufs)
+        return bufs[0][1]
+
+    def handle_next(self, packet):
+        from . import sspi
+        import ctypes
+        buf = ctypes.create_string_buffer(4096)
+        status, buffers = self._ctx.next(
+            flags=self._flags,
+            byte_ordering='network',
+            target_name=self._sname,
+            input_buffers=[(sspi.SECBUFFER_TOKEN, packet)],
+            output_buffers=[(sspi.SECBUFFER_TOKEN, buf)])
+        return buffers[0][1]
+
+    def close(self):
+        self._ctx.close()
+        self._cred.close()
+
+
+class NtlmAuth(object):
+    """ NTLM authentication, uses Python implementation
+
+    :param user_name: User name
+    :type user_name: str
+    :param password: User password
+    :type password: str
+    """
+    def __init__(self, user_name, password):
+        if '\\' in user_name:
+            self._domain, self._user = user_name.split('\\', 1)
+        else:
+            self._domain = 'workspace'
+            self._user = user_name
+        self._password = password
+
+    def create_packet(self):
+        from . import ntlm
+        return ntlm.create_NTLM_NEGOTIATE_MESSAGE_raw(socket.gethostname(), self._domain)
+
+    def handle_next(self, packet):
+        from . import ntlm
+        nonce, flags = ntlm.parse_NTLM_CHALLENGE_MESSAGE_raw(packet)
+        return ntlm.create_NTLM_AUTHENTICATE_MESSAGE_raw(nonce, self._user, self._domain, self._password, flags)
+
+    def close(self):
+        pass
```

### Comparing `python-tds-1.9.0/pytds/tds_base.py` & `python-tds-1.9.1/pytds/tds_base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,601 +1,601 @@
-import socket
-import sys
-
-import six
-
-# tds protocol versions
-TDS70 = 0x70000000
-TDS71 = 0x71000000
-TDS71rev1 = 0x71000001
-TDS72 = 0x72090002
-TDS73A = 0x730A0003
-TDS73 = TDS73A
-TDS73B = 0x730B0003
-TDS74 = 0x74000004
-
-IS_TDS7_PLUS = lambda x: x.tds_version >= TDS70
-IS_TDS71_PLUS = lambda x: x.tds_version >= TDS71
-IS_TDS72_PLUS = lambda x: x.tds_version >= TDS72
-IS_TDS73_PLUS = lambda x: x.tds_version >= TDS73A
-
-# packet types
-TDS_QUERY = 1
-TDS_LOGIN = 2
-TDS_RPC = 3
-TDS_REPLY = 4
-TDS_CANCEL = 6
-TDS_BULK = 7
-TDS7_TRANS = 14  # transaction management
-TDS_NORMAL = 15
-TDS7_LOGIN = 16
-TDS7_AUTH = 17
-TDS71_PRELOGIN = 18
-
-# mssql login options flags
-# option_flag1_values
-TDS_BYTE_ORDER_X86 = 0
-TDS_CHARSET_ASCII = 0
-TDS_DUMPLOAD_ON = 0
-TDS_FLOAT_IEEE_754 = 0
-TDS_INIT_DB_WARN = 0
-TDS_SET_LANG_OFF = 0
-TDS_USE_DB_SILENT = 0
-TDS_BYTE_ORDER_68000 = 0x01
-TDS_CHARSET_EBDDIC = 0x02
-TDS_FLOAT_VAX = 0x04
-TDS_FLOAT_ND5000 = 0x08
-TDS_DUMPLOAD_OFF = 0x10  # prevent BCP
-TDS_USE_DB_NOTIFY = 0x20
-TDS_INIT_DB_FATAL = 0x40
-TDS_SET_LANG_ON = 0x80
-
-# enum option_flag2_values
-TDS_INIT_LANG_WARN = 0
-TDS_INTEGRATED_SECURTY_OFF = 0
-TDS_ODBC_OFF = 0
-TDS_USER_NORMAL = 0  # SQL Server login
-TDS_INIT_LANG_REQUIRED = 0x01
-TDS_ODBC_ON = 0x02
-TDS_TRANSACTION_BOUNDARY71 = 0x04  # removed in TDS 7.2
-TDS_CACHE_CONNECT71 = 0x08  # removed in TDS 7.2
-TDS_USER_SERVER = 0x10  # reserved
-TDS_USER_REMUSER = 0x20  # DQ login
-TDS_USER_SQLREPL = 0x40  # replication login
-TDS_INTEGRATED_SECURITY_ON = 0x80
-
-# enum option_flag3_values TDS 7.3+
-TDS_RESTRICTED_COLLATION = 0
-TDS_CHANGE_PASSWORD = 0x01
-TDS_SEND_YUKON_BINARY_XML = 0x02
-TDS_REQUEST_USER_INSTANCE = 0x04
-TDS_UNKNOWN_COLLATION_HANDLING = 0x08
-TDS_ANY_COLLATION = 0x10
-
-TDS5_PARAMFMT2_TOKEN = 32  # 0x20
-TDS_LANGUAGE_TOKEN = 33  # 0x20    TDS 5.0 only
-TDS_ORDERBY2_TOKEN = 34  # 0x22
-TDS_ROWFMT2_TOKEN = 97  # 0x61    TDS 5.0 only
-TDS_LOGOUT_TOKEN = 113  # 0x71    TDS 5.0 only?
-TDS_RETURNSTATUS_TOKEN = 121  # 0x79
-TDS_PROCID_TOKEN = 124  # 0x7C    TDS 4.2 only
-TDS7_RESULT_TOKEN = 129  # 0x81    TDS 7.0 only
-TDS7_COMPUTE_RESULT_TOKEN = 136  # 0x88    TDS 7.0 only
-TDS_COLNAME_TOKEN = 160  # 0xA0    TDS 4.2 only
-TDS_COLFMT_TOKEN = 161  # 0xA1    TDS 4.2 only
-TDS_DYNAMIC2_TOKEN = 163  # 0xA3
-TDS_TABNAME_TOKEN = 164  # 0xA4
-TDS_COLINFO_TOKEN = 165  # 0xA5
-TDS_OPTIONCMD_TOKEN = 166  # 0xA6
-TDS_COMPUTE_NAMES_TOKEN = 167  # 0xA7
-TDS_COMPUTE_RESULT_TOKEN = 168  # 0xA8
-TDS_ORDERBY_TOKEN = 169  # 0xA9
-TDS_ERROR_TOKEN = 170  # 0xAA
-TDS_INFO_TOKEN = 171  # 0xAB
-TDS_PARAM_TOKEN = 172  # 0xAC
-TDS_LOGINACK_TOKEN = 173  # 0xAD
-TDS_CONTROL_TOKEN = 174  # 0xAE
-TDS_ROW_TOKEN = 209  # 0xD1
-TDS_NBC_ROW_TOKEN = 210  # 0xD2    as of TDS 7.3.B
-TDS_CMP_ROW_TOKEN = 211  # 0xD3
-TDS5_PARAMS_TOKEN = 215  # 0xD7    TDS 5.0 only
-TDS_CAPABILITY_TOKEN = 226  # 0xE2
-TDS_ENVCHANGE_TOKEN = 227  # 0xE3
-TDS_EED_TOKEN = 229  # 0xE5
-TDS_DBRPC_TOKEN = 230  # 0xE6
-TDS5_DYNAMIC_TOKEN = 231  # 0xE7    TDS 5.0 only
-TDS5_PARAMFMT_TOKEN = 236  # 0xEC    TDS 5.0 only
-TDS_AUTH_TOKEN = 237  # 0xED    TDS 7.0 only
-TDS_RESULT_TOKEN = 238  # 0xEE
-TDS_DONE_TOKEN = 253  # 0xFD
-TDS_DONEPROC_TOKEN = 254  # 0xFE
-TDS_DONEINPROC_TOKEN = 255  # 0xFF
-
-# CURSOR support: TDS 5.0 only
-TDS_CURCLOSE_TOKEN = 128  # 0x80    TDS 5.0 only
-TDS_CURDELETE_TOKEN = 129  # 0x81    TDS 5.0 only
-TDS_CURFETCH_TOKEN = 130  # 0x82    TDS 5.0 only
-TDS_CURINFO_TOKEN = 131  # 0x83    TDS 5.0 only
-TDS_CUROPEN_TOKEN = 132  # 0x84    TDS 5.0 only
-TDS_CURDECLARE_TOKEN = 134  # 0x86    TDS 5.0 only
-
-# environment type field
-TDS_ENV_DATABASE = 1
-TDS_ENV_LANG = 2
-TDS_ENV_CHARSET = 3
-TDS_ENV_PACKSIZE = 4
-TDS_ENV_LCID = 5
-TDS_ENV_SQLCOLLATION = 7
-TDS_ENV_BEGINTRANS = 8
-TDS_ENV_COMMITTRANS = 9
-TDS_ENV_ROLLBACKTRANS = 10
-TDS_ENV_ENLIST_DTC_TRANS = 11
-TDS_ENV_DEFECT_TRANS = 12
-TDS_ENV_DB_MIRRORING_PARTNER = 13
-TDS_ENV_PROMOTE_TRANS = 15
-TDS_ENV_TRANS_MANAGER_ADDR = 16
-TDS_ENV_TRANS_ENDED = 17
-TDS_ENV_RESET_COMPLETION_ACK = 18
-TDS_ENV_INSTANCE_INFO = 19
-TDS_ENV_ROUTING = 20
-
-# Microsoft internal stored procedure id's
-TDS_SP_CURSOR = 1
-TDS_SP_CURSOROPEN = 2
-TDS_SP_CURSORPREPARE = 3
-TDS_SP_CURSOREXECUTE = 4
-TDS_SP_CURSORPREPEXEC = 5
-TDS_SP_CURSORUNPREPARE = 6
-TDS_SP_CURSORFETCH = 7
-TDS_SP_CURSOROPTION = 8
-TDS_SP_CURSORCLOSE = 9
-TDS_SP_EXECUTESQL = 10
-TDS_SP_PREPARE = 11
-TDS_SP_EXECUTE = 12
-TDS_SP_PREPEXEC = 13
-TDS_SP_PREPEXECRPC = 14
-TDS_SP_UNPREPARE = 15
-
-# Flags returned in TDS_DONE token
-TDS_DONE_FINAL = 0
-TDS_DONE_MORE_RESULTS = 0x01  # more results follow
-TDS_DONE_ERROR = 0x02  # error occurred
-TDS_DONE_INXACT = 0x04  # transaction in progress
-TDS_DONE_PROC = 0x08  # results are from a stored procedure
-TDS_DONE_COUNT = 0x10  # count field in packet is valid
-TDS_DONE_CANCELLED = 0x20  # acknowledging an attention command (usually a cancel)
-TDS_DONE_EVENT = 0x40  # part of an event notification.
-TDS_DONE_SRVERROR = 0x100  # SQL server server error
-
-
-SYBVOID = 31  # 0x1F
-IMAGETYPE = SYBIMAGE = 34  # 0x22
-TEXTTYPE = SYBTEXT = 35  # 0x23
-SYBVARBINARY = 37  # 0x25
-INTNTYPE = SYBINTN = 38  # 0x26
-SYBVARCHAR = 39         # 0x27
-BINARYTYPE = SYBBINARY = 45  # 0x2D
-SYBCHAR = 47  # 0x2F
-INT1TYPE = SYBINT1 = 48  # 0x30
-BITTYPE = SYBBIT = 50  # 0x32
-INT2TYPE = SYBINT2 = 52  # 0x34
-INT4TYPE = SYBINT4 = 56  # 0x38
-DATETIM4TYPE = SYBDATETIME4 = 58  # 0x3A
-FLT4TYPE = SYBREAL = 59  # 0x3B
-MONEYTYPE = SYBMONEY = 60  # 0x3C
-DATETIMETYPE = SYBDATETIME = 61  # 0x3D
-FLT8TYPE = SYBFLT8 = 62  # 0x3E
-NTEXTTYPE = SYBNTEXT = 99  # 0x63
-SYBNVARCHAR = 103  # 0x67
-BITNTYPE = SYBBITN = 104  # 0x68
-NUMERICNTYPE = SYBNUMERIC = 108  # 0x6C
-DECIMALNTYPE = SYBDECIMAL = 106  # 0x6A
-FLTNTYPE = SYBFLTN = 109  # 0x6D
-MONEYNTYPE = SYBMONEYN = 110  # 0x6E
-DATETIMNTYPE = SYBDATETIMN = 111  # 0x6F
-MONEY4TYPE = SYBMONEY4 = 122  # 0x7A
-
-INT8TYPE = SYBINT8 = 127  # 0x7F
-BIGCHARTYPE = XSYBCHAR = 175  # 0xAF
-BIGVARCHRTYPE = XSYBVARCHAR = 167  # 0xA7
-NVARCHARTYPE = XSYBNVARCHAR = 231  # 0xE7
-NCHARTYPE = XSYBNCHAR = 239  # 0xEF
-BIGVARBINTYPE = XSYBVARBINARY = 165  # 0xA5
-BIGBINARYTYPE = XSYBBINARY = 173  # 0xAD
-GUIDTYPE = SYBUNIQUE = 36  # 0x24
-SSVARIANTTYPE = SYBVARIANT = 98  # 0x62
-UDTTYPE = SYBMSUDT = 240  # 0xF0
-XMLTYPE = SYBMSXML = 241  # 0xF1
-TVPTYPE = 243  # 0xF3
-DATENTYPE = SYBMSDATE = 40  # 0x28
-TIMENTYPE = SYBMSTIME = 41  # 0x29
-DATETIME2NTYPE = SYBMSDATETIME2 = 42  # 0x2a
-DATETIMEOFFSETNTYPE = SYBMSDATETIMEOFFSET = 43  # 0x2b
-
-#
-# Sybase only types
-#
-SYBLONGBINARY = 225  # 0xE1
-SYBUINT1 = 64  # 0x40
-SYBUINT2 = 65  # 0x41
-SYBUINT4 = 66  # 0x42
-SYBUINT8 = 67  # 0x43
-SYBBLOB = 36  # 0x24
-SYBBOUNDARY = 104  # 0x68
-SYBDATE = 49  # 0x31
-SYBDATEN = 123  # 0x7B
-SYB5INT8 = 191  # 0xBF
-SYBINTERVAL = 46  # 0x2E
-SYBLONGCHAR = 175  # 0xAF
-SYBSENSITIVITY = 103  # 0x67
-SYBSINT1 = 176  # 0xB0
-SYBTIME = 51  # 0x33
-SYBTIMEN = 147  # 0x93
-SYBUINTN = 68  # 0x44
-SYBUNITEXT = 174  # 0xAE
-SYBXML = 163  # 0xA3
-
-TDS_UT_TIMESTAMP = 80
-
-# compute operator
-SYBAOPCNT = 0x4b
-SYBAOPCNTU = 0x4c
-SYBAOPSUM = 0x4d
-SYBAOPSUMU = 0x4e
-SYBAOPAVG = 0x4f
-SYBAOPAVGU = 0x50
-SYBAOPMIN = 0x51
-SYBAOPMAX = 0x52
-
-# mssql2k compute operator
-SYBAOPCNT_BIG = 0x09
-SYBAOPSTDEV = 0x30
-SYBAOPSTDEVP = 0x31
-SYBAOPVAR = 0x32
-SYBAOPVARP = 0x33
-SYBAOPCHECKSUM_AGG = 0x72
-
-# param flags
-fByRefValue = 1
-fDefaultValue = 2
-
-TDS_IDLE = 0
-TDS_QUERYING = 1
-TDS_PENDING = 2
-TDS_READING = 3
-TDS_DEAD = 4
-state_names = ['IDLE', 'QUERYING', 'PENDING', 'READING', 'DEAD']
-
-TDS_ENCRYPTION_OFF = 0
-TDS_ENCRYPTION_REQUEST = 1
-TDS_ENCRYPTION_REQUIRE = 2
-
-class PreLoginEnc:
-    ENCRYPT_OFF = 0  # Encryption available but off
-    ENCRYPT_ON = 1  # Encryption available and on
-    ENCRYPT_NOT_SUP = 2  # Encryption not available
-    ENCRYPT_REQ = 3  # Encryption required
-
-PLP_MARKER = 0xffff
-PLP_NULL = 0xffffffffffffffff
-PLP_UNKNOWN = 0xfffffffffffffffe
-
-TDS_NO_COUNT = -1
-
-TVP_NULL_TOKEN = 0xffff
-
-# TVP COLUMN FLAGS
-TVP_COLUMN_DEFAULT_FLAG = 0x200
-
-TVP_END_TOKEN = 0x00
-TVP_ROW_TOKEN = 0x01
-TVP_ORDER_UNIQUE_TOKEN = 0x10
-TVP_COLUMN_ORDERING_TOKEN = 0x11
-
-
-class CommonEqualityMixin(object):
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-
-def iterdecode(iterable, codec):
-    """ Uses an incremental decoder to decode each chunk in iterable.
-    This function is a generator.
-
-    :param iterable: Iterable object which yields raw data to be decoded
-    :param codec: An instance of codec
-    """
-    decoder = codec.incrementaldecoder()
-    for chunk in iterable:
-        yield decoder.decode(chunk)
-    yield decoder.decode(b'', True)
-
-
-def force_unicode(s):
-    if isinstance(s, bytes):
-        try:
-            return s.decode('utf8')
-        except UnicodeDecodeError as e:
-            raise DatabaseError(e)
-    elif isinstance(s, six.text_type):
-        return s
-    else:
-        return six.text_type(s)
-
-
-def tds_quote_id(ident):
-    """ Quote an identifier
-
-    :param ident: id to quote
-    :returns: Quoted identifier
-    """
-    return '[{0}]'.format(ident.replace(']', ']]'))
-
-
-# store a tuple of programming error codes
-prog_errors = (
-    102,    # syntax error
-    207,    # invalid column name
-    208,    # invalid object name
-    2812,   # unknown procedure
-    4104    # multi-part identifier could not be bound
-)
-
-# store a tuple of integrity error codes
-integrity_errors = (
-    515,    # NULL insert
-    547,    # FK related
-    2601,   # violate unique index
-    2627,   # violate UNIQUE KEY constraint
-)
-
-
-if sys.version_info[0] >= 3:
-    exc_base_class = Exception
-
-    def my_ord(val):
-        return val
-
-else:
-    exc_base_class = StandardError
-    my_ord = ord
-
-
-# exception hierarchy
-class Warning(exc_base_class):
-    pass
-
-
-class Error(exc_base_class):
-    pass
-
-
-TimeoutError = socket.timeout
-
-
-class InterfaceError(Error):
-    pass
-
-
-class DatabaseError(Error):
-    @property
-    def message(self):
-        if self.procname:
-            return 'SQL Server message %d, severity %d, state %d, ' \
-                   'procedure %s, line %d:\n%s' % (self.number,
-                                                   self.severity, self.state, self.procname,
-                                                   self.line, self.text)
-        else:
-            return 'SQL Server message %d, severity %d, state %d, ' \
-                   'line %d:\n%s' % (self.number, self.severity,
-                                     self.state, self.line, self.text)
-
-
-class ClosedConnectionError(InterfaceError):
-    def __init__(self):
-        super(ClosedConnectionError, self).__init__('Server closed connection')
-
-
-class DataError(Error):
-    pass
-
-
-class OperationalError(DatabaseError):
-    pass
-
-
-class LoginError(OperationalError):
-    pass
-
-
-class IntegrityError(DatabaseError):
-    pass
-
-
-class InternalError(DatabaseError):
-    pass
-
-
-class ProgrammingError(DatabaseError):
-    pass
-
-
-class NotSupportedError(DatabaseError):
-    pass
-
-
-# DB-API type definitions
-class DBAPITypeObject:
-    def __init__(self, *values):
-        self.values = set(values)
-
-    def __eq__(self, other):
-        return other in self.values
-
-    def __cmp__(self, other):
-        if other in self.values:
-            return 0
-        if other < self.values:
-            return 1
-        else:
-            return -1
-
-
-# standard dbapi type objects
-STRING = DBAPITypeObject(SYBVARCHAR, SYBCHAR, SYBTEXT,
-                         XSYBNVARCHAR, XSYBNCHAR, SYBNTEXT,
-                         XSYBVARCHAR, XSYBCHAR, SYBMSXML)
-BINARY = DBAPITypeObject(SYBIMAGE, SYBBINARY, SYBVARBINARY, XSYBVARBINARY, XSYBBINARY)
-NUMBER = DBAPITypeObject(SYBBIT, SYBBITN, SYBINT1, SYBINT2, SYBINT4, SYBINT8, SYBINTN,
-                         SYBREAL, SYBFLT8, SYBFLTN)
-DATETIME = DBAPITypeObject(SYBDATETIME, SYBDATETIME4, SYBDATETIMN)
-DECIMAL = DBAPITypeObject(SYBMONEY, SYBMONEY4, SYBMONEYN, SYBNUMERIC,
-                          SYBDECIMAL)
-ROWID = DBAPITypeObject()
-
-# non-standard, but useful type objects
-INTEGER = DBAPITypeObject(SYBBIT, SYBBITN, SYBINT1, SYBINT2, SYBINT4, SYBINT8, SYBINTN)
-REAL = DBAPITypeObject(SYBREAL, SYBFLT8, SYBFLTN)
-XML = DBAPITypeObject(SYBMSXML)
-
-
-class InternalProc(object):
-    def __init__(self, proc_id, name):
-        self.proc_id = proc_id
-        self.name = name
-
-    def __unicode__(self):
-        return self.name
-
-SP_EXECUTESQL = InternalProc(TDS_SP_EXECUTESQL, 'sp_executesql')
-
-
-def skipall(stm, size):
-    """ Skips exactly size bytes in stm
-
-    If EOF is reached before size bytes are skipped
-    will raise :class:`ClosedConnectionError`
-
-    :param stm: Stream to skip bytes in, should have read method
-                this read method can return less than requested
-                number of bytes.
-    :param size: Number of bytes to skip.
-    """
-    res = stm.read(size)
-    if len(res) == size:
-        return
-    elif len(res) == 0:
-        raise ClosedConnectionError()
-    left = size - len(res)
-    while left:
-        buf = stm.read(left)
-        if len(buf) == 0:
-            raise ClosedConnectionError()
-        left -= len(buf)
-
-
-def read_chunks(stm, size):
-    """ Reads exactly size bytes from stm and produces chunks
-
-    May call stm.read multiple times until required
-    number of bytes is read.
-    If EOF is reached before size bytes are read
-    will raise :class:`ClosedConnectionError`
-
-    :param stm: Stream to read bytes from, should have read method,
-                this read method can return less than requested
-                number of bytes.
-    :param size: Number of bytes to read.
-    """
-    if size == 0:
-        yield b''
-        return
-
-    res = stm.read(size)
-    if len(res) == 0:
-        raise ClosedConnectionError()
-    yield res
-    left = size - len(res)
-    while left:
-        buf = stm.read(left)
-        if len(buf) == 0:
-            raise ClosedConnectionError()
-        yield buf
-        left -= len(buf)
-
-
-def readall(stm, size):
-    """ Reads exactly size bytes from stm
-
-    May call stm.read multiple times until required
-    number of bytes read.
-    If EOF is reached before size bytes are read
-    will raise :class:`ClosedConnectionError`
-
-    :param stm: Stream to read bytes from, should have read method
-                this read method can return less than requested
-                number of bytes.
-    :param size: Number of bytes to read.
-    :returns: Bytes buffer of exactly given size.
-    """
-    return b''.join(read_chunks(stm, size))
-
-
-def readall_fast(stm, size):
-    """
-    Slightly faster version of readall, it reads no more than two chunks.
-    Meaning that it can only be used to read small data that doesn't span
-    more that two packets.
-
-    :param stm: Stream to read from, should have read method.
-    :param size: Number of bytes to read.
-    :return:
-    """
-    buf, offset = stm.read_fast(size)
-    if len(buf) - offset < size:
-        # slow case
-        buf = buf[offset:]
-        buf += stm.read(size - len(buf))
-        return buf, 0
-    return buf, offset
-
-
-def total_seconds(td):
-    """ Total number of seconds in timedelta object
-
-    Python 2.6 doesn't have total_seconds method, this function
-    provides a backport
-    """
-    return td.days * 24 * 60 * 60 + td.seconds
-
-
-class Column(CommonEqualityMixin):
-    fNullable = 1
-    fCaseSen = 2
-    fReadWrite = 8
-    fIdentity = 0x10
-    fComputed = 0x20
-
-    def __init__(self, name='', type=None, flags=0, value=None):
-        self.char_codec = None
-        self.column_name = name
-        self.column_usertype = 0
-        self.flags = flags
-        self.type = type
-        self.value = value
-        self.serializer = None
-
-    def __repr__(self):
-        return '<Column(name={},value={},type={},flags={},user_type={},codec={})>'.format(
-            repr(self.column_name),
-            repr(self.value),
-            repr(self.type),
-            repr(self.flags),
-            repr(self.column_usertype),
-            repr(self.char_codec),
-        )
-
-    def choose_serializer(self, type_factory, collation):
-        return type_factory.serializer_by_type(sql_type=self.type, collation=collation)
+import socket
+import sys
+
+import six
+
+# tds protocol versions
+TDS70 = 0x70000000
+TDS71 = 0x71000000
+TDS71rev1 = 0x71000001
+TDS72 = 0x72090002
+TDS73A = 0x730A0003
+TDS73 = TDS73A
+TDS73B = 0x730B0003
+TDS74 = 0x74000004
+
+IS_TDS7_PLUS = lambda x: x.tds_version >= TDS70
+IS_TDS71_PLUS = lambda x: x.tds_version >= TDS71
+IS_TDS72_PLUS = lambda x: x.tds_version >= TDS72
+IS_TDS73_PLUS = lambda x: x.tds_version >= TDS73A
+
+# packet types
+TDS_QUERY = 1
+TDS_LOGIN = 2
+TDS_RPC = 3
+TDS_REPLY = 4
+TDS_CANCEL = 6
+TDS_BULK = 7
+TDS7_TRANS = 14  # transaction management
+TDS_NORMAL = 15
+TDS7_LOGIN = 16
+TDS7_AUTH = 17
+TDS71_PRELOGIN = 18
+
+# mssql login options flags
+# option_flag1_values
+TDS_BYTE_ORDER_X86 = 0
+TDS_CHARSET_ASCII = 0
+TDS_DUMPLOAD_ON = 0
+TDS_FLOAT_IEEE_754 = 0
+TDS_INIT_DB_WARN = 0
+TDS_SET_LANG_OFF = 0
+TDS_USE_DB_SILENT = 0
+TDS_BYTE_ORDER_68000 = 0x01
+TDS_CHARSET_EBDDIC = 0x02
+TDS_FLOAT_VAX = 0x04
+TDS_FLOAT_ND5000 = 0x08
+TDS_DUMPLOAD_OFF = 0x10  # prevent BCP
+TDS_USE_DB_NOTIFY = 0x20
+TDS_INIT_DB_FATAL = 0x40
+TDS_SET_LANG_ON = 0x80
+
+# enum option_flag2_values
+TDS_INIT_LANG_WARN = 0
+TDS_INTEGRATED_SECURTY_OFF = 0
+TDS_ODBC_OFF = 0
+TDS_USER_NORMAL = 0  # SQL Server login
+TDS_INIT_LANG_REQUIRED = 0x01
+TDS_ODBC_ON = 0x02
+TDS_TRANSACTION_BOUNDARY71 = 0x04  # removed in TDS 7.2
+TDS_CACHE_CONNECT71 = 0x08  # removed in TDS 7.2
+TDS_USER_SERVER = 0x10  # reserved
+TDS_USER_REMUSER = 0x20  # DQ login
+TDS_USER_SQLREPL = 0x40  # replication login
+TDS_INTEGRATED_SECURITY_ON = 0x80
+
+# enum option_flag3_values TDS 7.3+
+TDS_RESTRICTED_COLLATION = 0
+TDS_CHANGE_PASSWORD = 0x01
+TDS_SEND_YUKON_BINARY_XML = 0x02
+TDS_REQUEST_USER_INSTANCE = 0x04
+TDS_UNKNOWN_COLLATION_HANDLING = 0x08
+TDS_ANY_COLLATION = 0x10
+
+TDS5_PARAMFMT2_TOKEN = 32  # 0x20
+TDS_LANGUAGE_TOKEN = 33  # 0x20    TDS 5.0 only
+TDS_ORDERBY2_TOKEN = 34  # 0x22
+TDS_ROWFMT2_TOKEN = 97  # 0x61    TDS 5.0 only
+TDS_LOGOUT_TOKEN = 113  # 0x71    TDS 5.0 only?
+TDS_RETURNSTATUS_TOKEN = 121  # 0x79
+TDS_PROCID_TOKEN = 124  # 0x7C    TDS 4.2 only
+TDS7_RESULT_TOKEN = 129  # 0x81    TDS 7.0 only
+TDS7_COMPUTE_RESULT_TOKEN = 136  # 0x88    TDS 7.0 only
+TDS_COLNAME_TOKEN = 160  # 0xA0    TDS 4.2 only
+TDS_COLFMT_TOKEN = 161  # 0xA1    TDS 4.2 only
+TDS_DYNAMIC2_TOKEN = 163  # 0xA3
+TDS_TABNAME_TOKEN = 164  # 0xA4
+TDS_COLINFO_TOKEN = 165  # 0xA5
+TDS_OPTIONCMD_TOKEN = 166  # 0xA6
+TDS_COMPUTE_NAMES_TOKEN = 167  # 0xA7
+TDS_COMPUTE_RESULT_TOKEN = 168  # 0xA8
+TDS_ORDERBY_TOKEN = 169  # 0xA9
+TDS_ERROR_TOKEN = 170  # 0xAA
+TDS_INFO_TOKEN = 171  # 0xAB
+TDS_PARAM_TOKEN = 172  # 0xAC
+TDS_LOGINACK_TOKEN = 173  # 0xAD
+TDS_CONTROL_TOKEN = 174  # 0xAE
+TDS_ROW_TOKEN = 209  # 0xD1
+TDS_NBC_ROW_TOKEN = 210  # 0xD2    as of TDS 7.3.B
+TDS_CMP_ROW_TOKEN = 211  # 0xD3
+TDS5_PARAMS_TOKEN = 215  # 0xD7    TDS 5.0 only
+TDS_CAPABILITY_TOKEN = 226  # 0xE2
+TDS_ENVCHANGE_TOKEN = 227  # 0xE3
+TDS_EED_TOKEN = 229  # 0xE5
+TDS_DBRPC_TOKEN = 230  # 0xE6
+TDS5_DYNAMIC_TOKEN = 231  # 0xE7    TDS 5.0 only
+TDS5_PARAMFMT_TOKEN = 236  # 0xEC    TDS 5.0 only
+TDS_AUTH_TOKEN = 237  # 0xED    TDS 7.0 only
+TDS_RESULT_TOKEN = 238  # 0xEE
+TDS_DONE_TOKEN = 253  # 0xFD
+TDS_DONEPROC_TOKEN = 254  # 0xFE
+TDS_DONEINPROC_TOKEN = 255  # 0xFF
+
+# CURSOR support: TDS 5.0 only
+TDS_CURCLOSE_TOKEN = 128  # 0x80    TDS 5.0 only
+TDS_CURDELETE_TOKEN = 129  # 0x81    TDS 5.0 only
+TDS_CURFETCH_TOKEN = 130  # 0x82    TDS 5.0 only
+TDS_CURINFO_TOKEN = 131  # 0x83    TDS 5.0 only
+TDS_CUROPEN_TOKEN = 132  # 0x84    TDS 5.0 only
+TDS_CURDECLARE_TOKEN = 134  # 0x86    TDS 5.0 only
+
+# environment type field
+TDS_ENV_DATABASE = 1
+TDS_ENV_LANG = 2
+TDS_ENV_CHARSET = 3
+TDS_ENV_PACKSIZE = 4
+TDS_ENV_LCID = 5
+TDS_ENV_SQLCOLLATION = 7
+TDS_ENV_BEGINTRANS = 8
+TDS_ENV_COMMITTRANS = 9
+TDS_ENV_ROLLBACKTRANS = 10
+TDS_ENV_ENLIST_DTC_TRANS = 11
+TDS_ENV_DEFECT_TRANS = 12
+TDS_ENV_DB_MIRRORING_PARTNER = 13
+TDS_ENV_PROMOTE_TRANS = 15
+TDS_ENV_TRANS_MANAGER_ADDR = 16
+TDS_ENV_TRANS_ENDED = 17
+TDS_ENV_RESET_COMPLETION_ACK = 18
+TDS_ENV_INSTANCE_INFO = 19
+TDS_ENV_ROUTING = 20
+
+# Microsoft internal stored procedure id's
+TDS_SP_CURSOR = 1
+TDS_SP_CURSOROPEN = 2
+TDS_SP_CURSORPREPARE = 3
+TDS_SP_CURSOREXECUTE = 4
+TDS_SP_CURSORPREPEXEC = 5
+TDS_SP_CURSORUNPREPARE = 6
+TDS_SP_CURSORFETCH = 7
+TDS_SP_CURSOROPTION = 8
+TDS_SP_CURSORCLOSE = 9
+TDS_SP_EXECUTESQL = 10
+TDS_SP_PREPARE = 11
+TDS_SP_EXECUTE = 12
+TDS_SP_PREPEXEC = 13
+TDS_SP_PREPEXECRPC = 14
+TDS_SP_UNPREPARE = 15
+
+# Flags returned in TDS_DONE token
+TDS_DONE_FINAL = 0
+TDS_DONE_MORE_RESULTS = 0x01  # more results follow
+TDS_DONE_ERROR = 0x02  # error occurred
+TDS_DONE_INXACT = 0x04  # transaction in progress
+TDS_DONE_PROC = 0x08  # results are from a stored procedure
+TDS_DONE_COUNT = 0x10  # count field in packet is valid
+TDS_DONE_CANCELLED = 0x20  # acknowledging an attention command (usually a cancel)
+TDS_DONE_EVENT = 0x40  # part of an event notification.
+TDS_DONE_SRVERROR = 0x100  # SQL server server error
+
+
+SYBVOID = 31  # 0x1F
+IMAGETYPE = SYBIMAGE = 34  # 0x22
+TEXTTYPE = SYBTEXT = 35  # 0x23
+SYBVARBINARY = 37  # 0x25
+INTNTYPE = SYBINTN = 38  # 0x26
+SYBVARCHAR = 39         # 0x27
+BINARYTYPE = SYBBINARY = 45  # 0x2D
+SYBCHAR = 47  # 0x2F
+INT1TYPE = SYBINT1 = 48  # 0x30
+BITTYPE = SYBBIT = 50  # 0x32
+INT2TYPE = SYBINT2 = 52  # 0x34
+INT4TYPE = SYBINT4 = 56  # 0x38
+DATETIM4TYPE = SYBDATETIME4 = 58  # 0x3A
+FLT4TYPE = SYBREAL = 59  # 0x3B
+MONEYTYPE = SYBMONEY = 60  # 0x3C
+DATETIMETYPE = SYBDATETIME = 61  # 0x3D
+FLT8TYPE = SYBFLT8 = 62  # 0x3E
+NTEXTTYPE = SYBNTEXT = 99  # 0x63
+SYBNVARCHAR = 103  # 0x67
+BITNTYPE = SYBBITN = 104  # 0x68
+NUMERICNTYPE = SYBNUMERIC = 108  # 0x6C
+DECIMALNTYPE = SYBDECIMAL = 106  # 0x6A
+FLTNTYPE = SYBFLTN = 109  # 0x6D
+MONEYNTYPE = SYBMONEYN = 110  # 0x6E
+DATETIMNTYPE = SYBDATETIMN = 111  # 0x6F
+MONEY4TYPE = SYBMONEY4 = 122  # 0x7A
+
+INT8TYPE = SYBINT8 = 127  # 0x7F
+BIGCHARTYPE = XSYBCHAR = 175  # 0xAF
+BIGVARCHRTYPE = XSYBVARCHAR = 167  # 0xA7
+NVARCHARTYPE = XSYBNVARCHAR = 231  # 0xE7
+NCHARTYPE = XSYBNCHAR = 239  # 0xEF
+BIGVARBINTYPE = XSYBVARBINARY = 165  # 0xA5
+BIGBINARYTYPE = XSYBBINARY = 173  # 0xAD
+GUIDTYPE = SYBUNIQUE = 36  # 0x24
+SSVARIANTTYPE = SYBVARIANT = 98  # 0x62
+UDTTYPE = SYBMSUDT = 240  # 0xF0
+XMLTYPE = SYBMSXML = 241  # 0xF1
+TVPTYPE = 243  # 0xF3
+DATENTYPE = SYBMSDATE = 40  # 0x28
+TIMENTYPE = SYBMSTIME = 41  # 0x29
+DATETIME2NTYPE = SYBMSDATETIME2 = 42  # 0x2a
+DATETIMEOFFSETNTYPE = SYBMSDATETIMEOFFSET = 43  # 0x2b
+
+#
+# Sybase only types
+#
+SYBLONGBINARY = 225  # 0xE1
+SYBUINT1 = 64  # 0x40
+SYBUINT2 = 65  # 0x41
+SYBUINT4 = 66  # 0x42
+SYBUINT8 = 67  # 0x43
+SYBBLOB = 36  # 0x24
+SYBBOUNDARY = 104  # 0x68
+SYBDATE = 49  # 0x31
+SYBDATEN = 123  # 0x7B
+SYB5INT8 = 191  # 0xBF
+SYBINTERVAL = 46  # 0x2E
+SYBLONGCHAR = 175  # 0xAF
+SYBSENSITIVITY = 103  # 0x67
+SYBSINT1 = 176  # 0xB0
+SYBTIME = 51  # 0x33
+SYBTIMEN = 147  # 0x93
+SYBUINTN = 68  # 0x44
+SYBUNITEXT = 174  # 0xAE
+SYBXML = 163  # 0xA3
+
+TDS_UT_TIMESTAMP = 80
+
+# compute operator
+SYBAOPCNT = 0x4b
+SYBAOPCNTU = 0x4c
+SYBAOPSUM = 0x4d
+SYBAOPSUMU = 0x4e
+SYBAOPAVG = 0x4f
+SYBAOPAVGU = 0x50
+SYBAOPMIN = 0x51
+SYBAOPMAX = 0x52
+
+# mssql2k compute operator
+SYBAOPCNT_BIG = 0x09
+SYBAOPSTDEV = 0x30
+SYBAOPSTDEVP = 0x31
+SYBAOPVAR = 0x32
+SYBAOPVARP = 0x33
+SYBAOPCHECKSUM_AGG = 0x72
+
+# param flags
+fByRefValue = 1
+fDefaultValue = 2
+
+TDS_IDLE = 0
+TDS_QUERYING = 1
+TDS_PENDING = 2
+TDS_READING = 3
+TDS_DEAD = 4
+state_names = ['IDLE', 'QUERYING', 'PENDING', 'READING', 'DEAD']
+
+TDS_ENCRYPTION_OFF = 0
+TDS_ENCRYPTION_REQUEST = 1
+TDS_ENCRYPTION_REQUIRE = 2
+
+class PreLoginEnc:
+    ENCRYPT_OFF = 0  # Encryption available but off
+    ENCRYPT_ON = 1  # Encryption available and on
+    ENCRYPT_NOT_SUP = 2  # Encryption not available
+    ENCRYPT_REQ = 3  # Encryption required
+
+PLP_MARKER = 0xffff
+PLP_NULL = 0xffffffffffffffff
+PLP_UNKNOWN = 0xfffffffffffffffe
+
+TDS_NO_COUNT = -1
+
+TVP_NULL_TOKEN = 0xffff
+
+# TVP COLUMN FLAGS
+TVP_COLUMN_DEFAULT_FLAG = 0x200
+
+TVP_END_TOKEN = 0x00
+TVP_ROW_TOKEN = 0x01
+TVP_ORDER_UNIQUE_TOKEN = 0x10
+TVP_COLUMN_ORDERING_TOKEN = 0x11
+
+
+class CommonEqualityMixin(object):
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+
+def iterdecode(iterable, codec):
+    """ Uses an incremental decoder to decode each chunk in iterable.
+    This function is a generator.
+
+    :param iterable: Iterable object which yields raw data to be decoded
+    :param codec: An instance of codec
+    """
+    decoder = codec.incrementaldecoder()
+    for chunk in iterable:
+        yield decoder.decode(chunk)
+    yield decoder.decode(b'', True)
+
+
+def force_unicode(s):
+    if isinstance(s, bytes):
+        try:
+            return s.decode('utf8')
+        except UnicodeDecodeError as e:
+            raise DatabaseError(e)
+    elif isinstance(s, six.text_type):
+        return s
+    else:
+        return six.text_type(s)
+
+
+def tds_quote_id(ident):
+    """ Quote an identifier
+
+    :param ident: id to quote
+    :returns: Quoted identifier
+    """
+    return '[{0}]'.format(ident.replace(']', ']]'))
+
+
+# store a tuple of programming error codes
+prog_errors = (
+    102,    # syntax error
+    207,    # invalid column name
+    208,    # invalid object name
+    2812,   # unknown procedure
+    4104    # multi-part identifier could not be bound
+)
+
+# store a tuple of integrity error codes
+integrity_errors = (
+    515,    # NULL insert
+    547,    # FK related
+    2601,   # violate unique index
+    2627,   # violate UNIQUE KEY constraint
+)
+
+
+if sys.version_info[0] >= 3:
+    exc_base_class = Exception
+
+    def my_ord(val):
+        return val
+
+else:
+    exc_base_class = StandardError
+    my_ord = ord
+
+
+# exception hierarchy
+class Warning(exc_base_class):
+    pass
+
+
+class Error(exc_base_class):
+    pass
+
+
+TimeoutError = socket.timeout
+
+
+class InterfaceError(Error):
+    pass
+
+
+class DatabaseError(Error):
+    @property
+    def message(self):
+        if self.procname:
+            return 'SQL Server message %d, severity %d, state %d, ' \
+                   'procedure %s, line %d:\n%s' % (self.number,
+                                                   self.severity, self.state, self.procname,
+                                                   self.line, self.text)
+        else:
+            return 'SQL Server message %d, severity %d, state %d, ' \
+                   'line %d:\n%s' % (self.number, self.severity,
+                                     self.state, self.line, self.text)
+
+
+class ClosedConnectionError(InterfaceError):
+    def __init__(self):
+        super(ClosedConnectionError, self).__init__('Server closed connection')
+
+
+class DataError(Error):
+    pass
+
+
+class OperationalError(DatabaseError):
+    pass
+
+
+class LoginError(OperationalError):
+    pass
+
+
+class IntegrityError(DatabaseError):
+    pass
+
+
+class InternalError(DatabaseError):
+    pass
+
+
+class ProgrammingError(DatabaseError):
+    pass
+
+
+class NotSupportedError(DatabaseError):
+    pass
+
+
+# DB-API type definitions
+class DBAPITypeObject:
+    def __init__(self, *values):
+        self.values = set(values)
+
+    def __eq__(self, other):
+        return other in self.values
+
+    def __cmp__(self, other):
+        if other in self.values:
+            return 0
+        if other < self.values:
+            return 1
+        else:
+            return -1
+
+
+# standard dbapi type objects
+STRING = DBAPITypeObject(SYBVARCHAR, SYBCHAR, SYBTEXT,
+                         XSYBNVARCHAR, XSYBNCHAR, SYBNTEXT,
+                         XSYBVARCHAR, XSYBCHAR, SYBMSXML)
+BINARY = DBAPITypeObject(SYBIMAGE, SYBBINARY, SYBVARBINARY, XSYBVARBINARY, XSYBBINARY)
+NUMBER = DBAPITypeObject(SYBBIT, SYBBITN, SYBINT1, SYBINT2, SYBINT4, SYBINT8, SYBINTN,
+                         SYBREAL, SYBFLT8, SYBFLTN)
+DATETIME = DBAPITypeObject(SYBDATETIME, SYBDATETIME4, SYBDATETIMN)
+DECIMAL = DBAPITypeObject(SYBMONEY, SYBMONEY4, SYBMONEYN, SYBNUMERIC,
+                          SYBDECIMAL)
+ROWID = DBAPITypeObject()
+
+# non-standard, but useful type objects
+INTEGER = DBAPITypeObject(SYBBIT, SYBBITN, SYBINT1, SYBINT2, SYBINT4, SYBINT8, SYBINTN)
+REAL = DBAPITypeObject(SYBREAL, SYBFLT8, SYBFLTN)
+XML = DBAPITypeObject(SYBMSXML)
+
+
+class InternalProc(object):
+    def __init__(self, proc_id, name):
+        self.proc_id = proc_id
+        self.name = name
+
+    def __unicode__(self):
+        return self.name
+
+SP_EXECUTESQL = InternalProc(TDS_SP_EXECUTESQL, 'sp_executesql')
+
+
+def skipall(stm, size):
+    """ Skips exactly size bytes in stm
+
+    If EOF is reached before size bytes are skipped
+    will raise :class:`ClosedConnectionError`
+
+    :param stm: Stream to skip bytes in, should have read method
+                this read method can return less than requested
+                number of bytes.
+    :param size: Number of bytes to skip.
+    """
+    res = stm.read(size)
+    if len(res) == size:
+        return
+    elif len(res) == 0:
+        raise ClosedConnectionError()
+    left = size - len(res)
+    while left:
+        buf = stm.read(left)
+        if len(buf) == 0:
+            raise ClosedConnectionError()
+        left -= len(buf)
+
+
+def read_chunks(stm, size):
+    """ Reads exactly size bytes from stm and produces chunks
+
+    May call stm.read multiple times until required
+    number of bytes is read.
+    If EOF is reached before size bytes are read
+    will raise :class:`ClosedConnectionError`
+
+    :param stm: Stream to read bytes from, should have read method,
+                this read method can return less than requested
+                number of bytes.
+    :param size: Number of bytes to read.
+    """
+    if size == 0:
+        yield b''
+        return
+
+    res = stm.read(size)
+    if len(res) == 0:
+        raise ClosedConnectionError()
+    yield res
+    left = size - len(res)
+    while left:
+        buf = stm.read(left)
+        if len(buf) == 0:
+            raise ClosedConnectionError()
+        yield buf
+        left -= len(buf)
+
+
+def readall(stm, size):
+    """ Reads exactly size bytes from stm
+
+    May call stm.read multiple times until required
+    number of bytes read.
+    If EOF is reached before size bytes are read
+    will raise :class:`ClosedConnectionError`
+
+    :param stm: Stream to read bytes from, should have read method
+                this read method can return less than requested
+                number of bytes.
+    :param size: Number of bytes to read.
+    :returns: Bytes buffer of exactly given size.
+    """
+    return b''.join(read_chunks(stm, size))
+
+
+def readall_fast(stm, size):
+    """
+    Slightly faster version of readall, it reads no more than two chunks.
+    Meaning that it can only be used to read small data that doesn't span
+    more that two packets.
+
+    :param stm: Stream to read from, should have read method.
+    :param size: Number of bytes to read.
+    :return:
+    """
+    buf, offset = stm.read_fast(size)
+    if len(buf) - offset < size:
+        # slow case
+        buf = buf[offset:]
+        buf += stm.read(size - len(buf))
+        return buf, 0
+    return buf, offset
+
+
+def total_seconds(td):
+    """ Total number of seconds in timedelta object
+
+    Python 2.6 doesn't have total_seconds method, this function
+    provides a backport
+    """
+    return td.days * 24 * 60 * 60 + td.seconds
+
+
+class Column(CommonEqualityMixin):
+    fNullable = 1
+    fCaseSen = 2
+    fReadWrite = 8
+    fIdentity = 0x10
+    fComputed = 0x20
+
+    def __init__(self, name='', type=None, flags=0, value=None):
+        self.char_codec = None
+        self.column_name = name
+        self.column_usertype = 0
+        self.flags = flags
+        self.type = type
+        self.value = value
+        self.serializer = None
+
+    def __repr__(self):
+        return '<Column(name={},value={},type={},flags={},user_type={},codec={})>'.format(
+            repr(self.column_name),
+            repr(self.value),
+            repr(self.type),
+            repr(self.flags),
+            repr(self.column_usertype),
+            repr(self.char_codec),
+        )
+
+    def choose_serializer(self, type_factory, collation):
+        return type_factory.serializer_by_type(sql_type=self.type, collation=collation)
```

### Comparing `python-tds-1.9.0/python_tds.egg-info/PKG-INFO` & `python-tds-1.9.1/python_tds.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 1.1
-Name: python-tds
-Version: 1.9.0
-Summary: Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation
-Home-page: https://github.com/denisenkom/pytds
-Author: Mikhail Denisenko
-Author-email: denisenkom@gmail.com
-License: MIT
-Description-Content-Type: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Metadata-Version: 1.1
+Name: python-tds
+Version: 1.9.1
+Summary: Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation
+Home-page: https://github.com/denisenkom/pytds
+Author: Mikhail Denisenko
+Author-email: denisenkom@gmail.com
+License: MIT
+Description-Content-Type: UNKNOWN
+Description: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
```

