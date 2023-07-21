# Comparing `tmp/ox_secrets-0.5.1.tar.gz` & `tmp/ox_secrets-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_secrets-0.5.1.tar", last modified: Fri Jul 21 15:28:44 2023, max compression
+gzip compressed data, was "ox_secrets-0.5.2.tar", last modified: Fri Jul 21 16:11:43 2023, max compression
```

## Comparing `ox_secrets-0.5.1.tar` & `ox_secrets-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/
--rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.1/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.1/LICENSE.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)     6741 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)     5047 2023-07-21 15:28:07.000000 ox_secrets-0.5.1/README.org
--rw-------   0 emin      (1000) emin      (1000)     5165 2023-07-21 15:28:13.000000 ox_secrets-0.5.1/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.1/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.1/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.488852 ox_secrets-0.5.1/ox_secrets/
--rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 15:28:26.000000 ox_secrets-0.5.1/ox_secrets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/ox_secrets/core/
--rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.1/ox_secrets/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2392 2022-02-02 03:56:49.000000 ox_secrets-0.5.1/ox_secrets/core/awp.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.1/ox_secrets/core/aws.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.1/ox_secrets/core/common.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.1/ox_secrets/core/evs.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.1/ox_secrets/core/fss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)      738 2022-02-28 17:21:49.000000 ox_secrets-0.5.1/ox_secrets/core/tss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4422 2023-07-21 15:10:45.000000 ox_secrets-0.5.1/ox_secrets/server.py
--rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.1/ox_secrets/settings.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.488852 ox_secrets-0.5.1/ox_secrets.egg-info/
--rw-------   0 emin      (1000) emin      (1000)     6741 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      533 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       40 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/top_level.txt
--rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.1/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1957 2019-05-25 18:41:30.000000 ox_secrets-0.5.1/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/
+-rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.2/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.2/LICENSE.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)     5775 2023-07-21 16:11:19.000000 ox_secrets-0.5.2/README.org
+-rw-------   0 emin      (1000) emin      (1000)     5811 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.2/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.2/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 16:04:45.000000 ox_secrets-0.5.2/ox_secrets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/core/
+-rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.2/ox_secrets/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2374 2023-07-21 15:59:08.000000 ox_secrets-0.5.2/ox_secrets/core/awp.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.2/ox_secrets/core/aws.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.2/ox_secrets/core/common.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.2/ox_secrets/core/evs.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.2/ox_secrets/core/fss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)      719 2023-07-21 15:59:00.000000 ox_secrets-0.5.2/ox_secrets/core/tss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4457 2023-07-21 15:58:42.000000 ox_secrets-0.5.2/ox_secrets/server.py
+-rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.2/ox_secrets/settings.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       48 2023-07-21 16:09:41.000000 ox_secrets-0.5.2/ox_secrets/ui/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2101 2023-07-21 16:03:05.000000 ox_secrets-0.5.2/ox_secrets/ui/cli.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      580 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       55 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/top_level.txt
+-rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.2/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1974 2023-07-21 16:01:01.000000 ox_secrets-0.5.2/setup.py
```

### Comparing `ox_secrets-0.5.1/.gitignore` & `ox_secrets-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/LICENSE.txt` & `ox_secrets-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/PKG-INFO` & `ox_secrets-0.5.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,159 +1,168 @@
-Metadata-Version: 1.1
-Name: ox_secrets
-Version: 0.5.1
-Summary: Simple secret server for python
-Home-page: http://github.com/emin63/ox_secrets
-Author: Emin Martinian
-Author-email: emin.martinian@gmail.com
-License: custom
-Description: Introduction
-        ============
-        
-        The ``ox_secrets`` package provides a simple secret manager for python.
-        You can think ``ox_secrets`` like an ORM for secrets with the following
-        goals:
-        
-        -  Simple, light-weight management of secrets.
-        -  Handle various back-ends for storing secrets:
-        
-           -  environment variables
-           -  Amazon Web Services (AWS)
-           -  local files
-        
-        -  Easy to switch secrets for dev, testing, or production.
-        
-           -  You can use simple file based secret storage in development and
-              testing and then add more sophisticated secret storage in
-              production. Similarly, you can use it to switch which type of
-              secret manager you are using by changing only the mode for
-              ``ox_secerts`` (e.g., by setting ``OX_SECRETS_MODE`` environment
-              variable or setting the value of
-              ``ox_secrets.settings.OX_SECRETS_MODE`` in python) without having
-              to re-write the rest of your code.
-        
-        Currently, the following back ends are supported:
-        
-        -  ``fss``: File secret server
-        
-           -  Reads secrets from a local file.
-           -  Useful for development and testing.
-        
-        -  ``evs``: Environment variable server.
-        
-           -  While other modes back ends can use environment variables to
-              override, this mode **ONLY** looks at environment variables.
-        
-        -  ``aws``: Uses the AWS Secret Manager or AWS Parameter Store
-        
-           -  By default the ``aws`` back-end will use the AWS Secrets Manager.
-              If you want to use the parameter store instead, provide
-              ``service_name='ssm'``.
-        
-        The main secret server can merge and cache secrets from multiple
-        back-ends in case your secrets are split across various places.
-        
-        Usage
-        =====
-        
-        To get started, you can simply ``pip install ox_secrets`` as usual.
-        
-        The ``ox_secrets`` package provides a simple secret server with various
-        back-ends. The following illustrates example usage.
-        
-        .. code:: python
-        
-        
-           # First we setup an example secrets file:
-        
-           >>> import os, tempfile, csv
-           >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
-           >>> writer = csv.writer(open(fn, 'w')).writerows([
-           ... ['name', 'category', 'value', 'notes'],
-           ... ['example_name', 'root', 'super_secret', 'example secret'],
-           ... ['example_pw', 'prod/data', 'super_secret_pw', 'example secret_pw'],
-           ... ['example_pw', 'test/data', 'unsecret_test_pw', 'example secret test pw'],
-           ... ['example_pw', 'alt', 'alt_unsecret_test_pw', 'alt secret test pw']])
-           >>> print(open(fn).read().strip())
-           name,category,value,notes
-           example_name,root,super_secret,example secret
-           example_pw,prod/data,super_secret_pw,example secret_pw
-           example_pw,test/data,unsecret_test_pw,example secret test pw
-           example_pw,alt,alt_unsecret_test_pw,alt secret test pw
-        
-           >>> from ox_secrets import settings, server as oss
-           >>> oss.settings.OX_SECRETS_FILE = fn # default is ~/.ox_secrets.csv
-           >>> oss.forget_secrets()  # Clear it to make sure we start fresh
-           >>> oss.get_secret('example_name')
-           'super_secret'
-        
-           #  We can also get a dictionary of all the secrets for a given category:
-        
-           >>> oss.get_secret_dict(category='test/data')
-           {'example_pw': 'unsecret_test_pw'}
-        
-        
-        
-           #  Sometimes it is nice to be able to just pass a dictionary of
-           #  credential information to get_secret:
-        
-           >>> creds = {'name': 'example_name', 'category': 'root', 'server': 'fss'}
-           >>> oss.get_secret(**creds)
-           'super_secret'
-        
-           #  You can also puts secrets into the environment variables:
-        
-           >>> os.environ['OX_SECRETS_ROOT_EXAMPLE_NAME'] = 'other'
-           >>> oss.get_secret('example_name')
-           'other'
-        
-           #  You can use the OX_SECRETS_CATEGORY_REGEXP and
-           #  the OX_SECRETS_CATEGORY_REPLACE either in the settings file
-           #  or environment variables (before starting python) to automatically
-           #  switch from production to testing secrets:
-        
-           >>> oss.get_secret('example_pw', 'prod/data')
-           'super_secret_pw'
-           >>> oss.forget_secrets()  # Clear it to make sure we start fresh
-           >>> oss.settings.OX_SECRETS_CATEGORY_REGEXP = '^prod/'
-           >>> oss.settings.OX_SECRETS_CATEGORY_REPLACE = 'test/'
-           >>> oss.get_secret('example_pw', 'prod/data')
-           'unsecret_test_pw'
-        
-        
-           #  If desired, you can also store secrets (assuming
-           #  you have appropriate permissions):
-        
-           >>> oss.store_secrets({'example_pw': 'foobar'}, category='alt')
-           >>> oss.get_secret('example_pw', category='alt')
-           'foobar'
-        
-           #  Now cleanup
-        
-           >>> os.remove(fn)
-        
-        
-           #  If you have an account with the appropriate permissions (e.g.,
-           #  you may need to set the AWS_PROFILE environment variable to
-           #  to such an account), you can also store secrets and parameters
-           #  to aws.
-           #  
-           #  For example, you could do something like:
-           #  
-           #      oss.get_server(mode='aws').store_secrets(
-           #          {'test_storage':'foobar'}, category=AWS_SECRET_ID)
-           #  
-           #  to store a secret to the existing secret with secret ID
-           #  `AWS_SECRET_ID` on Amazon Web Services. You could also proide the
-           #  `service_name='ssm'` argument if you wanted to use the parameter store
-           #  instead of the secret store via something like:
-           #  
-           #      oss.get_server(mode='aws').store_secrets(
-           #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
-           #          service_name='ssm')
-        
-        
-Keywords: secret management
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Introduction
+============
+
+The ``ox_secrets`` package provides a simple secret manager for python.
+You can think ``ox_secrets`` like an ORM for secrets with the following
+goals:
+
+-  Simple, light-weight management of secrets.
+-  Handle various back-ends for storing secrets:
+
+   -  environment variables
+   -  Amazon Web Services (AWS)
+   -  local files
+
+-  Easy to switch secrets for dev, testing, or production.
+
+   -  You can use simple file based secret storage in development and
+      testing and then add more sophisticated secret storage in
+      production. Similarly, you can use it to switch which type of
+      secret manager you are using by changing only the mode for
+      ``ox_secerts`` (e.g., by setting ``OX_SECRETS_MODE`` environment
+      variable or setting the value of
+      ``ox_secrets.settings.OX_SECRETS_MODE`` in python) without having
+      to re-write the rest of your code.
+
+Currently, the following back ends are supported:
+
+-  ``fss``: File secret server
+
+   -  Reads secrets from a local file.
+   -  Useful for development and testing.
+
+-  ``evs``: Environment variable server.
+
+   -  While other modes back ends can use environment variables to
+      override, this mode **ONLY** looks at environment variables.
+
+-  ``aws``: Uses the AWS Secret Manager or AWS Parameter Store
+
+   -  By default the ``aws`` back-end will use the AWS Secrets Manager.
+      If you want to use the parameter store instead, provide
+      ``service_name='ssm'``.
+
+The main secret server can merge and cache secrets from multiple
+back-ends in case your secrets are split across various places.
+
+Usage
+=====
+
+To get started, you can simply ``pip install ox_secrets`` as usual and
+then see either the `Usage in Python <#usage-in-python>`__ section for
+how to use in python or the `Usage in Command
+Line <#usage-in-command-line>`__ for the CLI.
+
+Usage in Python
+---------------
+
+.. code:: python
+
+
+   #The =ox_secrets= package provides a simple secret server with various
+   #back-ends. The following illustrates example usage.
+
+   # First we setup an example secrets file:
+
+   >>> import os, tempfile, csv
+   >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
+   >>> writer = csv.writer(open(fn, 'w')).writerows([
+   ... ['name', 'category', 'value', 'notes'],
+   ... ['example_name', 'root', 'super_secret', 'example secret'],
+   ... ['example_pw', 'prod/data', 'super_secret_pw', 'example secret_pw'],
+   ... ['example_pw', 'test/data', 'unsecret_test_pw', 'example secret test pw'],
+   ... ['example_pw', 'alt', 'alt_unsecret_test_pw', 'alt secret test pw']])
+   >>> print(open(fn).read().strip())
+   name,category,value,notes
+   example_name,root,super_secret,example secret
+   example_pw,prod/data,super_secret_pw,example secret_pw
+   example_pw,test/data,unsecret_test_pw,example secret test pw
+   example_pw,alt,alt_unsecret_test_pw,alt secret test pw
+
+   >>> from ox_secrets import settings, server as oss
+   >>> oss.settings.OX_SECRETS_FILE = fn # default is ~/.ox_secrets.csv
+   >>> oss.forget_secrets()  # Clear it to make sure we start fresh
+   >>> oss.get_secret('example_name')
+   'super_secret'
+
+   #  We can also get a dictionary of all the secrets for a given category:
+
+   >>> oss.get_secret_dict(category='test/data')
+   {'example_pw': 'unsecret_test_pw'}
+
+
+
+   #  Sometimes it is nice to be able to just pass a dictionary of
+   #  credential information to get_secret:
+
+   >>> creds = {'name': 'example_name', 'category': 'root', 'server': 'fss'}
+   >>> oss.get_secret(**creds)
+   'super_secret'
+
+   #  You can also puts secrets into the environment variables:
+
+   >>> os.environ['OX_SECRETS_ROOT_EXAMPLE_NAME'] = 'other'
+   >>> oss.get_secret('example_name')
+   'other'
+
+   #  You can use the OX_SECRETS_CATEGORY_REGEXP and
+   #  the OX_SECRETS_CATEGORY_REPLACE either in the settings file
+   #  or environment variables (before starting python) to automatically
+   #  switch from production to testing secrets:
+
+   >>> oss.get_secret('example_pw', 'prod/data')
+   'super_secret_pw'
+   >>> oss.forget_secrets()  # Clear it to make sure we start fresh
+   >>> oss.settings.OX_SECRETS_CATEGORY_REGEXP = '^prod/'
+   >>> oss.settings.OX_SECRETS_CATEGORY_REPLACE = 'test/'
+   >>> oss.get_secret('example_pw', 'prod/data')
+   'unsecret_test_pw'
+
+
+   #  If desired, you can also store secrets (assuming
+   #  you have appropriate permissions):
+
+   >>> oss.store_secrets({'example_pw': 'foobar'}, category='alt')
+   >>> oss.get_secret('example_pw', category='alt')
+   'foobar'
+
+   #  Now cleanup
+
+   >>> os.remove(fn)
+
+
+   #  If you have an account with the appropriate permissions (e.g.,
+   #  you may need to set the AWS_PROFILE environment variable to
+   #  to such an account), you can also store secrets and parameters
+   #  to aws.
+   #  
+   #  For example, you could do something like:
+   #  
+   #      oss.get_server(mode='aws').store_secrets(
+   #          {'test_storage':'foobar'}, category=AWS_SECRET_ID)
+   #  
+   #  to store a secret to the existing secret with secret ID
+   #  `AWS_SECRET_ID` on Amazon Web Services. You could also proide the
+   #  `service_name='ssm'` argument if you wanted to use the parameter store
+   #  instead of the secret store via something like:
+   #  
+   #      oss.get_server(mode='aws').store_secrets(
+   #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
+   #          service_name='ssm')
+
+Usage in Command Line
+---------------------
+
+You can also use ``ox_secrets`` from the command line.
+
+For example, if you setup a secrets file in ``~/.ox_secrets.csv``
+similar to the example in the `Usage in Python <#usage-in-python>`__
+section, you can do something like
+
+.. code:: shell
+
+   ox_secrets example_name --category root
+
+to extract the desired secret.
+
+You can also pass other parameters (run ``ox_secrets --help`` for
+details).
```

### Comparing `ox_secrets-0.5.1/README.org` & `ox_secrets-0.5.2/README.org`

 * *Files 15% similar despite different names*

```diff
@@ -34,25 +34,32 @@
     you want to use the parameter store instead, provide ~service_name='ssm'~.
 
 The main secret server can merge and cache secrets from multiple
 back-ends in case your secrets are split across various places.
 
 * Usage
 
-To get started, you can simply =pip install ox_secrets= as usual.
+To get started, you can simply =pip install ox_secrets= as usual and
+then see either the [[#usage-in-python][Usage in Python]] section for how to use in python
+or the [[#usage-in-command-line][Usage in Command Line]] for the CLI.
+
+** Usage in Python
+  :PROPERTIES:
+    :CUSTOM_ID: usage-in-python
+  :END:
 
 #+COMMENT: The following is copied from /ox_secrets/__init__.py docs
 #+COMMENT: At some point we should use noweb or tangling to clean
 #+COMMENT: this up.
 
-The =ox_secrets= package provides a simple secret server with various
-back-ends. The following illustrates example usage.
-
 #+BEGIN_SRC python
 
+#The =ox_secrets= package provides a simple secret server with various
+#back-ends. The following illustrates example usage.
+
 # First we setup an example secrets file:
 
 >>> import os, tempfile, csv
 >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
 >>> writer = csv.writer(open(fn, 'w')).writerows([
 ... ['name', 'category', 'value', 'notes'],
 ... ['example_name', 'root', 'super_secret', 'example secret'],
@@ -134,7 +141,28 @@
 #  instead of the secret store via something like:
 #  
 #      oss.get_server(mode='aws').store_secrets(
 #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
 #          service_name='ssm')
 #+END_SRC
 
+** Usage in Command Line
+  :PROPERTIES:
+    :CUSTOM_ID: usage-in-command-line
+  :END:
+
+
+You can also use =ox_secrets= from the command line.
+
+For example, if you setup a secrets file in =~/.ox_secrets.csv=
+similar to the example in the [[#usage-in-python][Usage in Python]] section, you can do
+something like
+
+#+BEGIN_SRC shell
+ox_secrets example_name --category root
+#+END_SRC
+
+to extract the desired secret.
+
+You can also pass other parameters (run =ox_secrets --help= for details).
+
+
```

### Comparing `ox_secrets-0.5.1/README.rst` & `ox_secrets-0.5.2/ox_secrets.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,182 @@
-Introduction
-============
-
-The ``ox_secrets`` package provides a simple secret manager for python.
-You can think ``ox_secrets`` like an ORM for secrets with the following
-goals:
-
--  Simple, light-weight management of secrets.
--  Handle various back-ends for storing secrets:
-
-   -  environment variables
-   -  Amazon Web Services (AWS)
-   -  local files
-
--  Easy to switch secrets for dev, testing, or production.
-
-   -  You can use simple file based secret storage in development and
-      testing and then add more sophisticated secret storage in
-      production. Similarly, you can use it to switch which type of
-      secret manager you are using by changing only the mode for
-      ``ox_secerts`` (e.g., by setting ``OX_SECRETS_MODE`` environment
-      variable or setting the value of
-      ``ox_secrets.settings.OX_SECRETS_MODE`` in python) without having
-      to re-write the rest of your code.
-
-Currently, the following back ends are supported:
-
--  ``fss``: File secret server
-
-   -  Reads secrets from a local file.
-   -  Useful for development and testing.
-
--  ``evs``: Environment variable server.
-
-   -  While other modes back ends can use environment variables to
-      override, this mode **ONLY** looks at environment variables.
-
--  ``aws``: Uses the AWS Secret Manager or AWS Parameter Store
-
-   -  By default the ``aws`` back-end will use the AWS Secrets Manager.
-      If you want to use the parameter store instead, provide
-      ``service_name='ssm'``.
-
-The main secret server can merge and cache secrets from multiple
-back-ends in case your secrets are split across various places.
-
-Usage
-=====
-
-To get started, you can simply ``pip install ox_secrets`` as usual.
-
-The ``ox_secrets`` package provides a simple secret server with various
-back-ends. The following illustrates example usage.
-
-.. code:: python
-
-
-   # First we setup an example secrets file:
-
-   >>> import os, tempfile, csv
-   >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
-   >>> writer = csv.writer(open(fn, 'w')).writerows([
-   ... ['name', 'category', 'value', 'notes'],
-   ... ['example_name', 'root', 'super_secret', 'example secret'],
-   ... ['example_pw', 'prod/data', 'super_secret_pw', 'example secret_pw'],
-   ... ['example_pw', 'test/data', 'unsecret_test_pw', 'example secret test pw'],
-   ... ['example_pw', 'alt', 'alt_unsecret_test_pw', 'alt secret test pw']])
-   >>> print(open(fn).read().strip())
-   name,category,value,notes
-   example_name,root,super_secret,example secret
-   example_pw,prod/data,super_secret_pw,example secret_pw
-   example_pw,test/data,unsecret_test_pw,example secret test pw
-   example_pw,alt,alt_unsecret_test_pw,alt secret test pw
-
-   >>> from ox_secrets import settings, server as oss
-   >>> oss.settings.OX_SECRETS_FILE = fn # default is ~/.ox_secrets.csv
-   >>> oss.forget_secrets()  # Clear it to make sure we start fresh
-   >>> oss.get_secret('example_name')
-   'super_secret'
-
-   #  We can also get a dictionary of all the secrets for a given category:
-
-   >>> oss.get_secret_dict(category='test/data')
-   {'example_pw': 'unsecret_test_pw'}
-
-
-
-   #  Sometimes it is nice to be able to just pass a dictionary of
-   #  credential information to get_secret:
-
-   >>> creds = {'name': 'example_name', 'category': 'root', 'server': 'fss'}
-   >>> oss.get_secret(**creds)
-   'super_secret'
-
-   #  You can also puts secrets into the environment variables:
-
-   >>> os.environ['OX_SECRETS_ROOT_EXAMPLE_NAME'] = 'other'
-   >>> oss.get_secret('example_name')
-   'other'
-
-   #  You can use the OX_SECRETS_CATEGORY_REGEXP and
-   #  the OX_SECRETS_CATEGORY_REPLACE either in the settings file
-   #  or environment variables (before starting python) to automatically
-   #  switch from production to testing secrets:
-
-   >>> oss.get_secret('example_pw', 'prod/data')
-   'super_secret_pw'
-   >>> oss.forget_secrets()  # Clear it to make sure we start fresh
-   >>> oss.settings.OX_SECRETS_CATEGORY_REGEXP = '^prod/'
-   >>> oss.settings.OX_SECRETS_CATEGORY_REPLACE = 'test/'
-   >>> oss.get_secret('example_pw', 'prod/data')
-   'unsecret_test_pw'
-
-
-   #  If desired, you can also store secrets (assuming
-   #  you have appropriate permissions):
-
-   >>> oss.store_secrets({'example_pw': 'foobar'}, category='alt')
-   >>> oss.get_secret('example_pw', category='alt')
-   'foobar'
-
-   #  Now cleanup
-
-   >>> os.remove(fn)
-
-
-   #  If you have an account with the appropriate permissions (e.g.,
-   #  you may need to set the AWS_PROFILE environment variable to
-   #  to such an account), you can also store secrets and parameters
-   #  to aws.
-   #  
-   #  For example, you could do something like:
-   #  
-   #      oss.get_server(mode='aws').store_secrets(
-   #          {'test_storage':'foobar'}, category=AWS_SECRET_ID)
-   #  
-   #  to store a secret to the existing secret with secret ID
-   #  `AWS_SECRET_ID` on Amazon Web Services. You could also proide the
-   #  `service_name='ssm'` argument if you wanted to use the parameter store
-   #  instead of the secret store via something like:
-   #  
-   #      oss.get_server(mode='aws').store_secrets(
-   #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
-   #          service_name='ssm')
-
+Metadata-Version: 1.1
+Name: ox-secrets
+Version: 0.5.2
+Summary: Simple secret server for python
+Home-page: http://github.com/emin63/ox_secrets
+Author: Emin Martinian
+Author-email: emin.martinian@gmail.com
+License: custom
+Description: Introduction
+        ============
+        
+        The ``ox_secrets`` package provides a simple secret manager for python.
+        You can think ``ox_secrets`` like an ORM for secrets with the following
+        goals:
+        
+        -  Simple, light-weight management of secrets.
+        -  Handle various back-ends for storing secrets:
+        
+           -  environment variables
+           -  Amazon Web Services (AWS)
+           -  local files
+        
+        -  Easy to switch secrets for dev, testing, or production.
+        
+           -  You can use simple file based secret storage in development and
+              testing and then add more sophisticated secret storage in
+              production. Similarly, you can use it to switch which type of
+              secret manager you are using by changing only the mode for
+              ``ox_secerts`` (e.g., by setting ``OX_SECRETS_MODE`` environment
+              variable or setting the value of
+              ``ox_secrets.settings.OX_SECRETS_MODE`` in python) without having
+              to re-write the rest of your code.
+        
+        Currently, the following back ends are supported:
+        
+        -  ``fss``: File secret server
+        
+           -  Reads secrets from a local file.
+           -  Useful for development and testing.
+        
+        -  ``evs``: Environment variable server.
+        
+           -  While other modes back ends can use environment variables to
+              override, this mode **ONLY** looks at environment variables.
+        
+        -  ``aws``: Uses the AWS Secret Manager or AWS Parameter Store
+        
+           -  By default the ``aws`` back-end will use the AWS Secrets Manager.
+              If you want to use the parameter store instead, provide
+              ``service_name='ssm'``.
+        
+        The main secret server can merge and cache secrets from multiple
+        back-ends in case your secrets are split across various places.
+        
+        Usage
+        =====
+        
+        To get started, you can simply ``pip install ox_secrets`` as usual and
+        then see either the `Usage in Python <#usage-in-python>`__ section for
+        how to use in python or the `Usage in Command
+        Line <#usage-in-command-line>`__ for the CLI.
+        
+        Usage in Python
+        ---------------
+        
+        .. code:: python
+        
+        
+           #The =ox_secrets= package provides a simple secret server with various
+           #back-ends. The following illustrates example usage.
+        
+           # First we setup an example secrets file:
+        
+           >>> import os, tempfile, csv
+           >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
+           >>> writer = csv.writer(open(fn, 'w')).writerows([
+           ... ['name', 'category', 'value', 'notes'],
+           ... ['example_name', 'root', 'super_secret', 'example secret'],
+           ... ['example_pw', 'prod/data', 'super_secret_pw', 'example secret_pw'],
+           ... ['example_pw', 'test/data', 'unsecret_test_pw', 'example secret test pw'],
+           ... ['example_pw', 'alt', 'alt_unsecret_test_pw', 'alt secret test pw']])
+           >>> print(open(fn).read().strip())
+           name,category,value,notes
+           example_name,root,super_secret,example secret
+           example_pw,prod/data,super_secret_pw,example secret_pw
+           example_pw,test/data,unsecret_test_pw,example secret test pw
+           example_pw,alt,alt_unsecret_test_pw,alt secret test pw
+        
+           >>> from ox_secrets import settings, server as oss
+           >>> oss.settings.OX_SECRETS_FILE = fn # default is ~/.ox_secrets.csv
+           >>> oss.forget_secrets()  # Clear it to make sure we start fresh
+           >>> oss.get_secret('example_name')
+           'super_secret'
+        
+           #  We can also get a dictionary of all the secrets for a given category:
+        
+           >>> oss.get_secret_dict(category='test/data')
+           {'example_pw': 'unsecret_test_pw'}
+        
+        
+        
+           #  Sometimes it is nice to be able to just pass a dictionary of
+           #  credential information to get_secret:
+        
+           >>> creds = {'name': 'example_name', 'category': 'root', 'server': 'fss'}
+           >>> oss.get_secret(**creds)
+           'super_secret'
+        
+           #  You can also puts secrets into the environment variables:
+        
+           >>> os.environ['OX_SECRETS_ROOT_EXAMPLE_NAME'] = 'other'
+           >>> oss.get_secret('example_name')
+           'other'
+        
+           #  You can use the OX_SECRETS_CATEGORY_REGEXP and
+           #  the OX_SECRETS_CATEGORY_REPLACE either in the settings file
+           #  or environment variables (before starting python) to automatically
+           #  switch from production to testing secrets:
+        
+           >>> oss.get_secret('example_pw', 'prod/data')
+           'super_secret_pw'
+           >>> oss.forget_secrets()  # Clear it to make sure we start fresh
+           >>> oss.settings.OX_SECRETS_CATEGORY_REGEXP = '^prod/'
+           >>> oss.settings.OX_SECRETS_CATEGORY_REPLACE = 'test/'
+           >>> oss.get_secret('example_pw', 'prod/data')
+           'unsecret_test_pw'
+        
+        
+           #  If desired, you can also store secrets (assuming
+           #  you have appropriate permissions):
+        
+           >>> oss.store_secrets({'example_pw': 'foobar'}, category='alt')
+           >>> oss.get_secret('example_pw', category='alt')
+           'foobar'
+        
+           #  Now cleanup
+        
+           >>> os.remove(fn)
+        
+        
+           #  If you have an account with the appropriate permissions (e.g.,
+           #  you may need to set the AWS_PROFILE environment variable to
+           #  to such an account), you can also store secrets and parameters
+           #  to aws.
+           #  
+           #  For example, you could do something like:
+           #  
+           #      oss.get_server(mode='aws').store_secrets(
+           #          {'test_storage':'foobar'}, category=AWS_SECRET_ID)
+           #  
+           #  to store a secret to the existing secret with secret ID
+           #  `AWS_SECRET_ID` on Amazon Web Services. You could also proide the
+           #  `service_name='ssm'` argument if you wanted to use the parameter store
+           #  instead of the secret store via something like:
+           #  
+           #      oss.get_server(mode='aws').store_secrets(
+           #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
+           #          service_name='ssm')
+        
+        Usage in Command Line
+        ---------------------
+        
+        You can also use ``ox_secrets`` from the command line.
+        
+        For example, if you setup a secrets file in ``~/.ox_secrets.csv``
+        similar to the example in the `Usage in Python <#usage-in-python>`__
+        section, you can do something like
+        
+        .. code:: shell
+        
+           ox_secrets example_name --category root
+        
+        to extract the desired secret.
+        
+        You can also pass other parameters (run ``ox_secrets --help`` for
+        details).
+        
+Keywords: secret management
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
```

### Comparing `ox_secrets-0.5.1/ox_secrets/__init__.py` & `ox_secrets-0.5.2/ox_secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 __version__ = VERSION
```

### Comparing `ox_secrets-0.5.1/ox_secrets/core/awp.py` & `ox_secrets-0.5.2/ox_secrets/core/awp.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             profile_name = settings.OX_SECRETS_AWS_PROFILE_NAME
         logging.warning(
             'Connecting to boto3 for profile %s to read parameters for %s',
             profile_name, parameter_id)
         session = boto3.Session(profile_name=profile_name)
         FIXME
         return secret_dict
-        
+
     @classmethod
     def load_cache(cls, name: typing.Optional[str] = None,
                    category: typing.Optional[str] = None,
                    loader_params: typing.Optional[dict] = None):
         """Load parameters and cache them from back-end store.
 
         :param name:  String name of parameter desired. If this is None, then
@@ -68,9 +68,7 @@
         data = cls.load_parameter_from_aws(parameter_id=category, **loader_params)
         assert isinstance(data, dict)
         with cls._lock:
             cdict = cls._cache.get(category, {})
             if not cdict:
                 cls._cache[category] = cdict
             cdict.update(data)
-
-
```

### Comparing `ox_secrets-0.5.1/ox_secrets/core/aws.py` & `ox_secrets-0.5.2/ox_secrets/core/aws.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/ox_secrets/core/common.py` & `ox_secrets-0.5.2/ox_secrets/core/common.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/ox_secrets/core/evs.py` & `ox_secrets-0.5.2/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/ox_secrets/core/fss.py` & `ox_secrets-0.5.2/ox_secrets/core/fss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/ox_secrets/core/tss.py` & `ox_secrets-0.5.2/ox_secrets/core/tss.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 """
 
 import typing
 import logging
 import csv
 import os
 
+
 from ox_secrets import settings
 from ox_secrets.core import common
 
 
 class TelegramSecretServer(common.SecretServer):
     """Class to handle getting secrets from telegram.
     """
 
     @classmethod
     def one_time_secret(cls, tuser, name, category='root'):
         FIXME
-        
-            
+
+
     @classmethod
     @classmethod
     def load_cache(cls, name: typing.Optional[str] = None,
                    category: typing.Optional[str] = None):
         "Implement loading cache from a file."
         return cls.load_secrets_file()
```

### Comparing `ox_secrets-0.5.1/ox_secrets/server.py` & `ox_secrets-0.5.2/ox_secrets/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     if mode in ['fss', 'file']:
         return fss.FileSecretServer
     if mode in ['evs', 'env']:
         return evs.EnvVarSecretServer
     if mode == 'aws':
         # delayed import so boto3 does not need to be installed if
         # the aws secret server is never used
-        from ox_secrets.core import aws
+        from ox_secrets.core import aws  \
+            # pylint:disable=import-outside-toplevel
         return aws.AWSSecretServer
-    raise ValueError('Invalid secret server mode "{mode}"')
+    raise ValueError(f'Invalid secret server mode "{mode}"')
 
 
 def get_secret(name: str, category: str = 'root',
                server: typing.Optional[
                    typing.Union[str, common.SecretServer]] = None) -> str:
     """Return desired secret.
 
@@ -66,15 +67,15 @@
         allow_update: bool = True,
         loader_params: typing.Optional[dict] = None,
         service_name: typing.Optional[str] = None) -> typing.Dict[
             str, typing.Any]:
     """Lookup secret with given name and return it.
 
     :param mode=None:  Optional string mode for calling get_server.
-                      
+
     :param category='root':  Optional string category for secret
 
     :param allow_update=True:  Whether to loading cache if secret not
                                found.
 
     :param loader_params: Optional dict of parameters which gets
                           passed to load_cache for back-end. This allows
```

### Comparing `ox_secrets-0.5.1/ox_secrets/settings.py` & `ox_secrets-0.5.2/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.1/ox_secrets.egg-info/PKG-INFO` & `ox_secrets-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: ox-secrets
-Version: 0.5.1
+Name: ox_secrets
+Version: 0.5.2
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
@@ -51,22 +51,28 @@
         
         The main secret server can merge and cache secrets from multiple
         back-ends in case your secrets are split across various places.
         
         Usage
         =====
         
-        To get started, you can simply ``pip install ox_secrets`` as usual.
+        To get started, you can simply ``pip install ox_secrets`` as usual and
+        then see either the `Usage in Python <#usage-in-python>`__ section for
+        how to use in python or the `Usage in Command
+        Line <#usage-in-command-line>`__ for the CLI.
         
-        The ``ox_secrets`` package provides a simple secret server with various
-        back-ends. The following illustrates example usage.
+        Usage in Python
+        ---------------
         
         .. code:: python
         
         
+           #The =ox_secrets= package provides a simple secret server with various
+           #back-ends. The following illustrates example usage.
+        
            # First we setup an example secrets file:
         
            >>> import os, tempfile, csv
            >>> fn = tempfile.mktemp(suffix='_ox_secrets.csv')
            >>> writer = csv.writer(open(fn, 'w')).writerows([
            ... ['name', 'category', 'value', 'notes'],
            ... ['example_name', 'root', 'super_secret', 'example secret'],
@@ -147,13 +153,30 @@
            #  `service_name='ssm'` argument if you wanted to use the parameter store
            #  instead of the secret store via something like:
            #  
            #      oss.get_server(mode='aws').store_secrets(
            #          {'test_storage':'foobar', category=AWS_PARAM_NAME,
            #          service_name='ssm')
         
+        Usage in Command Line
+        ---------------------
+        
+        You can also use ``ox_secrets`` from the command line.
+        
+        For example, if you setup a secrets file in ``~/.ox_secrets.csv``
+        similar to the example in the `Usage in Python <#usage-in-python>`__
+        section, you can do something like
+        
+        .. code:: shell
+        
+           ox_secrets example_name --category root
+        
+        to extract the desired secret.
+        
+        You can also pass other parameters (run ``ox_secrets --help`` for
+        details).
         
 Keywords: secret management
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ox_secrets-0.5.1/ox_secrets.egg-info/SOURCES.txt` & `ox_secrets-0.5.2/ox_secrets.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 ox_secrets.egg-info/top_level.txt
 ox_secrets/core/__init__.py
 ox_secrets/core/awp.py
 ox_secrets/core/aws.py
 ox_secrets/core/common.py
 ox_secrets/core/evs.py
 ox_secrets/core/fss.py
-ox_secrets/core/tss.py
+ox_secrets/core/tss.py
+ox_secrets/ui/__init__.py
+ox_secrets/ui/cli.py
```

### Comparing `ox_secrets-0.5.1/setup.py` & `ox_secrets-0.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,11 +53,11 @@
         'sample': ['package_data.dat'],
     },
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points={
         'console_scripts': [
-            'sample=sample:main',
+            'ox_secrets = ox_secrets.ui.cli:main',
         ],
     },
 )
```

