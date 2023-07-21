# Comparing `tmp/cylc-rose-1.2.0.tar.gz` & `tmp/cylc-rose-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-rose-1.2.0.tar", last modified: Mon Jan 16 13:09:21 2023, max compression
+gzip compressed data, was "cylc-rose-1.3.0.tar", last modified: Fri Jul 21 10:10:08 2023, max compression
```

## Comparing `cylc-rose-1.2.0.tar` & `cylc-rose-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 13:09:21.885746 cylc-rose-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-01-16 13:09:21.885746 cylc-rose-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 13:09:21.881746 cylc-rose-1.2.0/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 13:09:21.885746 cylc-rose-1.2.0/cylc/rose/
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/jinja2_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/platform_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20809 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/stem.py
--rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/cylc/rose/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 13:09:21.885746 cylc-rose-1.2.0/cylc_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-16 13:09:21.000000 cylc-rose-1.2.0/cylc_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-01-16 13:09:21.885746 cylc-rose-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-01-16 13:09:18.000000 cylc-rose-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:10:08.756784 cylc-rose-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-21 10:10:08.756784 cylc-rose-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:10:08.752784 cylc-rose-1.3.0/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:10:08.756784 cylc-rose-1.3.0/cylc/rose/
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/jinja2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/platform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21140 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/stem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/cylc/rose/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:10:08.756784 cylc-rose-1.3.0/cylc_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 10:10:08.000000 cylc-rose-1.3.0/cylc_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 10:10:08.756784 cylc-rose-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 10:10:03.000000 cylc-rose-1.3.0/setup.py
```

### Comparing `cylc-rose-1.2.0/COPYING` & `cylc-rose-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.2.0/PKG-INFO` & `cylc-rose-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.2.0/README.md` & `cylc-rose-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.2.0/cylc/rose/__init__.py` & `cylc-rose-1.3.0/cylc/rose/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,8 +201,8 @@
    To reinstall a rose stem suite use ``cylc reinstall``.  Cylc can get any
    options you do not change from the ``rose-suite-cylc-install.conf``` file.
    Using ``rose stem`` a second time will attempt install a new copy
    of your rose stem suite.
 
 """
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
```

### Comparing `cylc-rose-1.2.0/cylc/rose/entry_points.py` & `cylc-rose-1.3.0/cylc/rose/entry_points.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.2.0/cylc/rose/jinja2_parser.py` & `cylc-rose-1.3.0/cylc/rose/jinja2_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.2.0/cylc/rose/platform_utils.py` & `cylc-rose-1.3.0/cylc/rose/platform_utils.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.2.0/cylc/rose/stem.py` & `cylc-rose-1.3.0/cylc/rose/stem.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,26 +70,27 @@
 
 from cylc.flow.exceptions import CylcError
 from cylc.flow.scripts.install import (
     get_option_parser,
     install as cylc_install
 )
 
+from cylc.rose.entry_points import get_rose_vars
+
 import metomi.rose.config
 from metomi.rose.fs_util import FileSystemUtil
 from metomi.rose.host_select import HostSelector
 from metomi.rose.popen import RosePopener
 from metomi.rose.reporter import Reporter, Event
 from metomi.rose.resource import ResourceLocator
 
 
 EXC_EXIT = cparse('<red><bold>{name}: </bold>{exc}</red>')
 DEFAULT_TEST_DIR = 'rose-stem'
 ROSE_STEM_VERSION = 1
-SUITE_RC_PREFIX = '[jinja2:suite.rc]'
 
 
 class ConfigVariableSetEvent(Event):
 
     """Event to report a particular variable has been set."""
 
     LEVEL = Event.V
@@ -239,26 +240,27 @@
         if fs_util is None:
             self.fs_util = FileSystemUtil(event_handler=self.reporter)
         else:
             self.fs_util = fs_util
 
         self.host_selector = HostSelector(event_handler=self.reporter,
                                           popen=self.popen)
+        self.template_section = '[template variables]'
 
     def _add_define_option(self, var, val):
         """Add a define option passed to the SuiteRunner.
 
         Args:
             var: Name of variable to set
             val: Value of variable to set
         """
         if self.opts.defines:
-            self.opts.defines.append(SUITE_RC_PREFIX + var + '=' + val)
+            self.opts.defines.append(self.template_section + var + '=' + val)
         else:
-            self.opts.defines = [SUITE_RC_PREFIX + var + '=' + val]
+            self.opts.defines = [self.template_section + var + '=' + val]
         self.reporter(ConfigVariableSetEvent(var, val))
         return
 
     def _get_fcm_loc_layout_info(self, src_tree):
         """Given a source tree return the following from 'fcm loc-layout':
            * url
            * sub_tree
@@ -443,14 +445,20 @@
         self.opts.project = []
 
         for i, url in enumerate(self.opts.stem_sources):
             project, url, base, rev, mirror = self._ascertain_project(url)
             self.opts.stem_sources[i] = url
             self.opts.project.append(project)
 
+            if i == 0:
+                # Get the name of the template section to be used:
+                template_type = get_rose_vars(
+                    Path(url) / "rose-stem")["templating_detected"]
+                self.template_section = f'[{template_type}]'
+
             # Versions of variables with hostname prepended for working copies
             url_host = self._prepend_localhost(url)
             base_host = self._prepend_localhost(base)
 
             if project in repos:
                 repos[project].append(url)
                 repos_with_hosts[project].append(url_host)
@@ -479,16 +487,16 @@
         # Generate the variable containing tasks to run
         if self.opts.stem_groups:
             if not self.opts.defines:
                 self.opts.defines = []
             expanded_groups = []
             for i in self.opts.stem_groups:
                 expanded_groups.extend(i.split(','))
-            self.opts.defines.append(SUITE_RC_PREFIX + 'RUN_NAMES=' +
-                                     str(expanded_groups))
+            self.opts.defines.append(
+                f"{self.template_section}RUN_NAMES={str(expanded_groups)}")
 
         # Load the config file and return any automatic-options
         auto_opts = self._read_auto_opts()
         if auto_opts:
             automatic_options = auto_opts.split()
             for option in automatic_options:
                 elements = option.split("=")
```

### Comparing `cylc-rose-1.2.0/cylc/rose/utilities.py` & `cylc-rose-1.3.0/cylc/rose/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pathlib import Path
 import re
 import shlex
 from typing import TYPE_CHECKING, Union
 
 from cylc.flow.hostuserutil import get_host
 from cylc.flow import LOG
-import cylc.flow.flags as flags
+from cylc.flow.flags import cylc7_back_compat
 from cylc.rose.jinja2_parser import Parser, patch_jinja2_leading_zeros
 from metomi.rose import __version__ as ROSE_VERSION
 from metomi.isodatetime.datetimeoper import DateTimeOperator
 from metomi.rose.config import ConfigDumper, ConfigNodeDiff, ConfigNode
 from metomi.rose.config_processor import ConfigProcessError
 from metomi.rose.env import env_var_process, UnboundEnvironmentVariableError
 
@@ -38,14 +38,16 @@
 
 
 SECTIONS = {'jinja2:suite.rc', 'empy:suite.rc', 'template variables'}
 SET_BY_CYLC = 'set by Cylc'
 ROSE_ORIG_HOST_INSTALLED_OVERRIDE_STRING = (
     ' ROSE_ORIG_HOST set by cylc install.'
 )
+MESSAGE = 'message'
+ALL_MODES = 'all modes'
 
 
 class MultipleTemplatingEnginesError(Exception):
     ...
 
 
 def get_rose_vars_from_config_node(config, config_node, environ):
@@ -262,15 +264,15 @@
     )
 
     # Reload the Config using the suite_ variables.
     # (we can't do this first time around because we have no idea what the
     # templating section is.)
     if getattr(opts, 'rose_template_vars', None):
         template_section = identify_templating_section(config_tree.node)
-        for template_var in opts.rose_template_vars:
+        for template_var in opts.rose_template_vars or []:
             redefinitions.append(f'[{template_section}]{template_var}')
         # Reload the config
         config_tree = ConfigTreeLoader().load(
             str(srcdir),
             'rose-suite.conf',
             opt_keys=opt_conf_keys,
             defines=redefinitions,
@@ -351,36 +353,36 @@
         {'value': 'BAZ', 'state': '', 'comments': []}
     """
     # Unpack info we want from opts:
     opt_conf_keys = []
     defines = []
     rose_template_vars = []
     if opts and 'opt_conf_keys' in dir(opts):
-        opt_conf_keys = opts.opt_conf_keys
+        opt_conf_keys = opts.opt_conf_keys or []
     if opts and 'defines' in dir(opts):
-        defines = opts.defines
+        defines = opts.defines or []
     if opts and 'rose_template_vars' in dir(opts):
-        rose_template_vars = opts.rose_template_vars
+        rose_template_vars = opts.rose_template_vars or []
 
     rose_orig_host = get_host()
     defines.append(f'[env]ROSE_ORIG_HOST={rose_orig_host}')
     rose_template_vars.append(f'ROSE_ORIG_HOST={rose_orig_host}')
 
     # Construct new ouput based on optional Configs:
     newconfig = ConfigNode()
 
     # For each __define__ determine whether it is an env or template define.
     for define in defines:
         match = re.match(
-                (
-                    r'^\[(?P<key1>.*)\](?P<state>!{0,2})'
-                    r'(?P<key2>.*)\s*=\s*(?P<value>.*)'
-                ),
-                define
-            ).groupdict()
+            (
+                r'^\[(?P<key1>.*)\](?P<state>!{0,2})'
+                r'(?P<key2>.*)\s*=\s*(?P<value>.*)'
+            ),
+            define
+        ).groupdict()
         if match['key1'] == '' and match['state'] in ['!', '!!']:
             LOG.warning(
                 'CLI opts set to ignored or trigger-ignored will be ignored.'
             )
         else:
             newconfig.set(
                 keys=[match['key1'], match['key2']],
@@ -652,34 +654,54 @@
 
 def deprecation_warnings(config_tree):
     """Check for deprecated items in config.
     Logs a warning for deprecated items:
         - "root-dir"
         - "jinja2:suite.rc"
         - "empy:suite.rc"
+        - root-dir
 
+    If ALL_MODES is True this deprecation will ignore whether there is a
+    flow.cylc or suite.rc in the workflow directory.
     """
 
     deprecations = {
-        'empy:suite.rc': (
-            "'rose-suite.conf[empy:suite.rc]' is deprecated."
-            " Use [template variables] instead."),
-        'jinja2:suite.rc': (
-            "'rose-suite.conf[jinja2:suite.rc]' is deprecated."
-            " Use [template variables] instead."),
-        'empy:flow.cylc': (
-            "'rose-suite.conf[empy:flow.cylc]' is not used by Cylc."
-            " Use [template variables] instead."),
-        'jinja2:flow.cylc': (
-            "'rose-suite.conf[jinja2:flow.cylc]' is not used by Cylc."
-            " Use [template variables] instead."),
-        'root-dir': (
-            'You have set "rose-suite.conf[root-dir]", '
-            'which is not supported at '
-            'Cylc 8. Use `[install] symlink dirs` in global.cylc '
-            'instead.')
+        'empy:suite.rc': {
+            MESSAGE: (
+                "'rose-suite.conf[empy:suite.rc]' is deprecated."
+                " Use [template variables] instead."),
+            ALL_MODES: False,
+        },
+        'jinja2:suite.rc': {
+            MESSAGE: (
+                "'rose-suite.conf[jinja2:suite.rc]' is deprecated."
+                " Use [template variables] instead."),
+            ALL_MODES: False,
+        },
+        'empy:flow.cylc': {
+            MESSAGE: (
+                "'rose-suite.conf[empy:flow.cylc]' is not used by Cylc."
+                " Use [template variables] instead."),
+            ALL_MODES: False,
+        },
+        'jinja2:flow.cylc': {
+            MESSAGE: (
+                "'rose-suite.conf[jinja2:flow.cylc]' is not used by Cylc."
+                " Use [template variables] instead."),
+            ALL_MODES: False,
+        },
+        'root-dir': {
+            MESSAGE: (
+                'You have set "rose-suite.conf[root-dir]", '
+                'which is not supported at '
+                'Cylc 8. Use `[install] symlink dirs` in global.cylc '
+                'instead.'),
+            ALL_MODES: True,
+        },
     }
-    if not flags.cylc7_back_compat:
-        for string in list(config_tree.node):
-            for deprecation in deprecations.keys():
-                if deprecation in string.lower():
-                    LOG.warning(deprecations[deprecation])
+    for string in list(config_tree.node):
+        for name, info in deprecations.items():
+            if (
+                (info[ALL_MODES] or not cylc7_back_compat)
+                and name in string.lower()
+            ):
+                LOG.warning(info[MESSAGE])
```

### Comparing `cylc-rose-1.2.0/cylc_rose.egg-info/PKG-INFO` & `cylc-rose-1.3.0/cylc_rose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.2.0/cylc_rose.egg-info/requires.txt` & `cylc-rose-1.3.0/cylc_rose.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-metomi-rose==2.0.*
-cylc-flow==8.1.*
+metomi-rose==2.1.*
+cylc-flow==8.2.*
 metomi-isodatetime
 jinja2
 
 [all]
 coverage>=5.0.0
 flake8
 flake8-broken-line>=0.3.0
```

### Comparing `cylc-rose-1.2.0/setup.cfg` & `cylc-rose-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 python_requires = >=3.7
 
 [options]
 packages = find_namespace:
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
-	metomi-rose==2.0.*
-	cylc-flow==8.1.*
+	metomi-rose==2.1.*
+	cylc-flow==8.2.*
 	metomi-isodatetime
 	jinja2
 
 [options.packages.find]
 include = cylc*
 
 [options.extras_require]
```

### Comparing `cylc-rose-1.2.0/setup.py` & `cylc-rose-1.3.0/setup.py`

 * *Files identical despite different names*

