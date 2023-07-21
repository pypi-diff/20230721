# Comparing `tmp/sshoot-1.5.1.tar.gz` & `tmp/sshoot-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sshoot-1.5.1.tar", last modified: Fri Dec 18 20:12:32 2020, max compression
+gzip compressed data, was "sshoot-1.6.0.tar", last modified: Fri Jul 21 06:19:43 2023, max compression
```

## Comparing `sshoot-1.5.1.tar` & `sshoot-1.6.0.tar`

### file list

```diff
@@ -1,45 +1,30 @@
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/
--rw-rw-r--   0 ack       (1000) ack       (1000)     2508 2020-12-18 20:10:35.000000 sshoot-1.5.1/CHANGES.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)    35147 2015-05-28 12:53:49.000000 sshoot-1.5.1/LICENSE.txt
--rw-r--r--   0 ack       (1000) ack       (1000)      114 2018-03-18 13:55:57.000000 sshoot-1.5.1/MANIFEST.in
--rw-rw-r--   0 ack       (1000) ack       (1000)     3766 2020-12-18 20:12:32.344650 sshoot-1.5.1/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)     2223 2020-12-17 07:34:58.000000 sshoot-1.5.1/README.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)      209 2020-11-20 14:49:00.000000 sshoot-1.5.1/pyproject.toml
--rw-rw-r--   0 ack       (1000) ack       (1000)     2636 2020-12-18 20:12:32.348650 sshoot-1.5.1/setup.cfg
--rw-r--r--   0 ack       (1000) ack       (1000)       38 2019-12-03 21:26:26.000000 sshoot-1.5.1/setup.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/shell-completion/
--rw-r--r--   0 ack       (1000) ack       (1000)       98 2018-11-12 15:22:07.000000 sshoot-1.5.1/shell-completion/sshoot
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/sshoot/
--rw-r--r--   0 ack       (1000) ack       (1000)      210 2019-12-03 21:26:26.000000 sshoot-1.5.1/sshoot/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      904 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/autocomplete.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2263 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/config.py
--rw-r--r--   0 ack       (1000) ack       (1000)      966 2019-12-03 21:26:26.000000 sshoot-1.5.1/sshoot/conftest.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      547 2020-12-17 17:40:44.000000 sshoot-1.5.1/sshoot/i18n.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     5105 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/listing.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/sshoot/locale/
--rw-r--r--   0 ack       (1000) ack       (1000)     3207 2018-03-18 13:55:57.000000 sshoot-1.5.1/sshoot/locale/argparse.pot
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.340650 sshoot-1.5.1/sshoot/locale/it_IT/
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 ack       (1000) ack       (1000)     3026 2018-03-18 13:55:57.000000 sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/argparse.mo
--rw-r--r--   0 ack       (1000) ack       (1000)     4469 2018-06-29 18:22:00.000000 sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/argparse.po
--rw-rw-r--   0 ack       (1000) ack       (1000)     4682 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/sshoot.mo
--rw-rw-r--   0 ack       (1000) ack       (1000)     6379 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/sshoot.po
--rw-rw-r--   0 ack       (1000) ack       (1000)     4567 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/locale/sshoot.pot
--rw-rw-r--   0 ack       (1000) ack       (1000)     9062 2020-12-17 20:33:43.000000 sshoot-1.5.1/sshoot/main.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     6190 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/manager.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2605 2020-12-16 20:50:00.000000 sshoot-1.5.1/sshoot/profile.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/sshoot/tests/
--rw-r--r--   0 ack       (1000) ack       (1000)        0 2017-03-04 10:37:10.000000 sshoot-1.5.1/sshoot/tests/__init__.py
--rw-r--r--   0 ack       (1000) ack       (1000)     1766 2019-12-03 21:26:26.000000 sshoot-1.5.1/sshoot/tests/test_autocomplete.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     4413 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/tests/test_config.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     5452 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/tests/test_listing.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     4222 2020-12-17 07:25:22.000000 sshoot-1.5.1/sshoot/tests/test_main.py
--rw-rw-r--   0 ack       (1000) ack       (1000)    14509 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/tests/test_manager.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3901 2020-11-20 14:49:00.000000 sshoot-1.5.1/sshoot/tests/test_profile.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2020-12-18 20:12:32.344650 sshoot-1.5.1/sshoot.egg-info/
--rw-rw-r--   0 ack       (1000) ack       (1000)     3766 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)      872 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/SOURCES.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        1 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/dependency_links.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       47 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/entry_points.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       97 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/requires.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        7 2020-12-18 20:12:32.000000 sshoot-1.5.1/sshoot.egg-info/top_level.txt
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2786 2023-07-21 06:08:24.000000 sshoot-1.6.0/CHANGES.rst
+-rw-rw-r--   0 ack       (1000) ack       (1000)    35147 2015-05-28 12:53:49.000000 sshoot-1.6.0/LICENSE.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)    43968 2023-07-21 06:19:43.621205 sshoot-1.6.0/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2221 2023-05-06 21:20:29.000000 sshoot-1.6.0/README.rst
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2249 2023-05-06 21:18:44.000000 sshoot-1.6.0/pyproject.toml
+-rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-07-21 06:19:43.621205 sshoot-1.6.0/setup.cfg
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/sshoot/
+-rw-rw-r--   0 ack       (1000) ack       (1000)       68 2023-05-06 21:18:44.000000 sshoot-1.6.0/sshoot/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)       35 2023-05-06 21:18:44.000000 sshoot-1.6.0/sshoot/__main__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      917 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/autocomplete.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2348 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/config.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      547 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/i18n.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     5378 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/listing.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/sshoot/locale/
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/sshoot/locale/it_IT/
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/sshoot/locale/it_IT/LC_MESSAGES/
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4652 2023-05-10 06:19:16.000000 sshoot-1.6.0/sshoot/locale/it_IT/LC_MESSAGES/sshoot.mo
+-rw-rw-r--   0 ack       (1000) ack       (1000)     6548 2023-05-10 06:19:16.000000 sshoot-1.6.0/sshoot/locale/it_IT/LC_MESSAGES/sshoot.po
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4594 2023-05-10 06:19:16.000000 sshoot-1.6.0/sshoot/locale/sshoot.pot
+-rw-rw-r--   0 ack       (1000) ack       (1000)    10379 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/main.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     7043 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/manager.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2851 2023-07-21 06:02:58.000000 sshoot-1.6.0/sshoot/profile.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-21 06:19:43.621205 sshoot-1.6.0/sshoot.egg-info/
+-rw-rw-r--   0 ack       (1000) ack       (1000)    43968 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)      502 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       46 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/entry_points.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       79 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/requires.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        7 2023-07-21 06:19:43.000000 sshoot-1.6.0/sshoot.egg-info/top_level.txt
```

### Comparing `sshoot-1.5.1/CHANGES.rst` & `sshoot-1.6.0/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+v1.6.0 - 2022-07-21
+===================
+
+- Support defining global extra options to pass to ``sshuttle`` (#14).
+- Add hint to look at syslog log for ``sshuttle`` output (#13).
+- Require Python3.8+.
+- [snap] Rebase snap on core22.
+- Rework project setup.
+- Update i18n setup.
+
+
 v1.5.1 - 2020-12-18
 ===================
 
 - [snap] Ship Python3.8 in the snap not to depend on version from OS.
-- Drop legacy config file path compatiblity.
+- Drop legacy config file path compatibility.
 - Drop Python3.6 support.
-* Add unittests for main script.
-* Only pass action parameters to Manager methods (Fixes: #10).
+- Add unittests for main script.
+- Only pass action parameters to Manager methods (Fixes: #10).
 
 
 v1.5.0 - 2020-11-20
 ===================
 
 - Add ``restart`` option for a profile.
 - Use ``toolrack.script.Script`` as base for main script.
```

### Comparing `sshoot-1.5.1/LICENSE.txt` & `sshoot-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sshoot-1.5.1/README.rst` & `sshoot-1.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/sshoot.svg
    :alt: Latest Version
    :target: https://pypi.python.org/pypi/sshoot
 .. |Build Status| image:: https://github.com/albertodonato/sshoot/workflows/CI/badge.svg
    :alt: Build Status
    :target: https://github.com/albertodonato/sshoot/actions?query=workflow%3ACI
-.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/albertodonato/sshoot/master.svg
+.. |Coverage Status| image:: https://img.shields.io/codecov/c/github/albertodonato/sshoot/main.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/albertodonato/sshoot
 .. |Snap Package| image:: https://snapcraft.io/sshoot/badge.svg
    :alt: Snap Package
    :target: https://snapcraft.io/sshoot
 .. |Get it from the Snap Store| image:: https://snapcraft.io/static/images/badges/en/snap-store-black.svg
    :alt: Get it from the Snap Store
```

### Comparing `sshoot-1.5.1/sshoot/autocomplete.py` & `sshoot-1.6.0/sshoot/autocomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 def complete_argument(argument, completer):
     """wrapper for setting up argument completer."""
     argument.completer = completer
     return argument
 
 
 def profile_completer(
-    prefix: str, parsed_args: Namespace, running: Optional[bool] = None, **kwargs
+    prefix: str,
+    parsed_args: Namespace,
+    running: Optional[bool] = None,
+    **kwargs,
 ):
     """Autocomplete helper for profile names.
 
     Parameters:
         - running: filter profiles that are running or not (by default no
           filter is applied).
```

### Comparing `sshoot-1.5.1/sshoot/config.py` & `sshoot-1.6.0/sshoot/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 import yaml
 
 from .profile import Profile
 
 
 def yaml_dump(data: Dict, fh: Optional[IO] = None):
     """Dump data in YAML format with sane defaults for readability."""
-    return yaml.safe_dump(data, fh, default_flow_style=False, allow_unicode=True)
+    return yaml.safe_dump(
+        data, fh, default_flow_style=False, allow_unicode=True
+    )
 
 
 class Config:
     """Handle configuration file loading/saving."""
 
-    CONFIG_KEYS = frozenset(["executable"])
+    CONFIG_KEYS = frozenset(["executable", "extra-options"])
 
     def __init__(self, path: Path):
         self._config_file = path / "config.yaml"
         self._profiles_file = path / "profiles.yaml"
         self._reset()
 
     def load(self):
@@ -34,15 +36,17 @@
         self._config = self._load_yaml_file(self._config_file)
         profiles = self._load_yaml_file(self._profiles_file)
         for name, conf in profiles.items():
             self._profiles[name] = Profile.from_config(conf)
 
     def save(self):
         """Save profiles configuration to file."""
-        config = {name: profile.config() for name, profile in self._profiles.items()}
+        config = {
+            name: profile.config() for name, profile in self._profiles.items()
+        }
         self._profiles_file.write_text(yaml_dump(config))
 
     def add_profile(self, name: str, profile: Profile):
         """Add a profile to the configuration."""
         if name in self._profiles:
             raise KeyError(name)
         self._profiles[name] = profile
@@ -56,18 +60,20 @@
         """Return a dict with profiles, using names as key."""
         return self._profiles.copy()
 
     @property
     def config(self) -> Dict[str, Any]:
         """Return a dict with the configuration."""
         return {
-            key: value for key, value in self._config.items() if key in self.CONFIG_KEYS
+            key: value
+            for key, value in self._config.items()
+            if key in self.CONFIG_KEYS
         }
 
-    def _reset(self):
+    def _reset(self) -> None:
         """Reset default empty config."""
         self._profiles: Dict[str, Profile] = {}
         self._config = {}
 
     def _load_yaml_file(self, path: Path) -> Dict[str, Any]:
         """Load the specified YAML file."""
         if not path.exists():
```

### Comparing `sshoot-1.5.1/sshoot/i18n.py` & `sshoot-1.6.0/sshoot/i18n.py`

 * *Files identical despite different names*

### Comparing `sshoot-1.5.1/sshoot/listing.py` & `sshoot-1.6.0/sshoot/listing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Helpers for listing output."""
 
 from collections import OrderedDict
 from csv import DictWriter
 from io import StringIO
 import json
 from typing import (
-    Callable,
     cast,
     Iterable,
     List,
+    Optional,
+    Protocol,
     Tuple,
 )
 
 from prettytable import (
     HEADER,
     PrettyTable,
 )
 
 from .config import yaml_dump
 from .i18n import _
 from .manager import Manager
 from .profile import Profile
 
-# Map names to profile fileds
+# Map names to profile fields
 _FIELDS_MAP = OrderedDict(
     [
         (_("Remote host"), "remote"),
         (_("Subnets"), "subnets"),
         (_("Auto hosts"), "auto_hosts"),
         (_("Auto nets"), "auto_nets"),
         (_("DNS forward"), "dns"),
@@ -42,30 +43,40 @@
 
 class InvalidFormat(Exception):
     def __init__(self, name: str):
         super().__init__(_("Invalid output format: {name}").format(name=name))
 
 
 ProfileIterator = Iterable[Tuple[str, Profile]]
-Formatter = Callable[..., str]  # XXX switch to Protocol when only supporting Python3.8
+
+
+class Formatter(Protocol):
+    def __call__(
+        self, profile_iter: ProfileIterator, verbose: bool = False
+    ) -> str:
+        ...  # pragma: nocoverage
 
 
 class ProfileListing:
     """List details for details in the specified format."""
 
     def __init__(self, manager: Manager):
         self.manager = manager
 
     @classmethod
     def supported_formats(cls) -> List[str]:
-        return sorted(attr[8:] for attr in dir(cls) if attr.startswith("_format_"))
+        return sorted(
+            attr[8:] for attr in dir(cls) if attr.startswith("_format_")
+        )
 
     def get_output(self, _format: str, verbose: bool = False) -> str:
         """Return a string with listing in the specified format."""
-        formatter: Formatter = getattr(self, "_format_{}".format(_format), None)
+        formatter: Optional[Formatter] = getattr(
+            self, f"_format_{_format}", None
+        )
         if formatter is None:
             raise InvalidFormat(_format)
         profiles_iter = self.manager.get_profiles().items()
         return formatter(profiles_iter, verbose=verbose)
 
     def _format_table(
         self, profiles_iter: ProfileIterator, verbose: bool = False
@@ -86,31 +97,41 @@
         table.padding_width = 0
         table.left_padding_width = 0
         table.right_padding_width = 1
         table.hrules = HEADER
 
         for name, profile in profiles_iter:
             row = ["*" if self.manager.is_running(name) else "", name]
-            row.extend(_format_value(getattr(profile, column)) for column in columns)
+            row.extend(
+                _format_value(getattr(profile, column)) for column in columns
+            )
             table.add_row(row)
         return cast(str, table.get_string(sortby=NAME_FIELD)) + "\n"
 
-    def _format_csv(self, profiles_iter: ProfileIterator, verbose: bool = False) -> str:
+    def _format_csv(
+        self, profiles_iter: ProfileIterator, verbose: bool = False
+    ) -> str:
         """Format profiles data as CSV."""
         titles = [NAME_FIELD, STATUS_FIELD]
         titles.extend(_FIELDS_MAP)
 
         buf = StringIO()
         writer = DictWriter(buf, fieldnames=titles)
         writer.writeheader()
 
         for name, profile in profiles_iter:
-            row = {NAME_FIELD: name, STATUS_FIELD: _profile_status(self.manager, name)}
+            row = {
+                NAME_FIELD: name,
+                STATUS_FIELD: _profile_status(self.manager, name),
+            }
             row.update(
-                {title: getattr(profile, _FIELDS_MAP[title]) for title in titles[2:]}
+                {
+                    title: getattr(profile, _FIELDS_MAP[title])
+                    for title in titles[2:]
+                }
             )
             writer.writerow(row)
         return buf.getvalue()
 
     def _format_json(
         self, profiles_iter: ProfileIterator, verbose: bool = False
     ) -> str:
@@ -130,20 +151,22 @@
         data = {name: profile.config() for name, profile in profiles_iter}
         return cast(str, yaml_dump(data))
 
 
 def profile_details(manager: Manager, name: str) -> str:
     """Return a string with details about a profile, formatted as a table."""
     profile = manager.get_profile(name)
-    table = PrettyTable(field_names=["key", "value"], header=False, border=False)
+    table = PrettyTable(
+        field_names=["key", "value"], header=False, border=False
+    )
     table.align["key"] = table.align["value"] = "l"
-    table.add_row(("{}:".format(NAME_FIELD), name))
-    table.add_row(("{}:".format(STATUS_FIELD), _profile_status(manager, name)))
+    table.add_row((f"{NAME_FIELD}:", name))
+    table.add_row((f"{STATUS_FIELD}:", _profile_status(manager, name)))
     for name, field in _FIELDS_MAP.items():
-        table.add_row(("{}:".format(name), _format_value(getattr(profile, field))))
+        table.add_row((f"{name}:", _format_value(getattr(profile, field))))
     return cast(str, table.get_string())
 
 
 def _profile_status(manager: Manager, name: str) -> str:
     """Return a string with the status of a profile."""
     return _("ACTIVE") if manager.is_running(name) else _("STOPPED")
```

### Comparing `sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/sshoot.mo` & `sshoot-1.6.0/sshoot/locale/it_IT/LC_MESSAGES/sshoot.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: sshoot 1.3.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-11-15 11:01+0100\n"
+"POT-Creation-Date: 2023-05-10 08:19+0200\n"
 "PO-Revision-Date: 2020-11-15 11:02+0100\n"
 "Last-Translator: Alberto Donato <alberto.donato@gmail.com>\n"
 "Language: it_IT\n"
 "Language-Team: it_IT <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "ACTIVE"
 msgstr "ATTIVO"
 
 msgid "Auto hosts"
 msgstr "Hosts automatici"
 
@@ -42,17 +42,14 @@
 
 msgid "Invalid profile config '{key}'"
 msgstr "Chiave '{key}' non valida nella configurazione del profilo"
 
 msgid "Manage multiple sshuttle VPN sessions"
 msgstr "Gestisci sessioni VPN sshuttle multiple"
 
-msgid "NOTICE: configuration tree moved from {old_path} to {new_path}\n"
-msgstr "NOTA: la configurazione è stata spostata da {old_path} a {new_path}\n"
-
 msgid "Name"
 msgstr "Nome"
 
 msgid "Profile failed to start: {error}"
 msgstr "Attivazione del profilo fallita: {error}"
 
 msgid "Profile is already running"
@@ -114,14 +111,17 @@
 
 msgid "define a new profile"
 msgstr "definisci un nuovo profilo"
 
 msgid "delete an existing profile"
 msgstr "cancella un profilo esistente"
 
+msgid "disable global extra-options set in config.yaml"
+msgstr "disabilita le opzioni globali presenti in config.yaml"
+
 msgid "exclude subnets from VPN forward"
 msgstr "escludi sottoreti dall'invio tramite VPN"
 
 msgid "extra arguments to pass to sshuttle command line"
 msgstr "opzioni aggiuntive da passare alla linea di comando di sshuttle"
 
 msgid "forward DNS queries through the VPN"
```

### Comparing `sshoot-1.5.1/sshoot/locale/it_IT/LC_MESSAGES/sshoot.po` & `sshoot-1.6.0/sshoot/locale/it_IT/LC_MESSAGES/sshoot.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,244 +3,247 @@
 # This file is distributed under the same license as the sshoot project.
 # Alberto Donato <alberto.donato@gmail.com>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: sshoot 1.3.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-11-15 11:01+0100\n"
+"POT-Creation-Date: 2023-05-10 08:19+0200\n"
 "PO-Revision-Date: 2020-11-15 11:02+0100\n"
 "Last-Translator: Alberto Donato <alberto.donato@gmail.com>\n"
 "Language: it_IT\n"
 "Language-Team: it_IT <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: sshoot/listing.py:28
+#: sshoot/listing.py:29
 msgid "Remote host"
 msgstr "Host remoto"
 
-#: sshoot/listing.py:29
+#: sshoot/listing.py:30
 msgid "Subnets"
 msgstr "Sottoreti"
 
-#: sshoot/listing.py:30
+#: sshoot/listing.py:31
 msgid "Auto hosts"
 msgstr "Hosts automatici"
 
-#: sshoot/listing.py:31
+#: sshoot/listing.py:32
 msgid "Auto nets"
 msgstr "Reti automatiche"
 
-#: sshoot/listing.py:32
+#: sshoot/listing.py:33
 msgid "DNS forward"
 msgstr "Invia req. DNS"
 
-#: sshoot/listing.py:33
+#: sshoot/listing.py:34
 msgid "Exclude subnets"
 msgstr "Sottoreti escluse"
 
-#: sshoot/listing.py:34
+#: sshoot/listing.py:35
 msgid "Seed hosts"
 msgstr "Specifica host"
 
-#: sshoot/listing.py:35
+#: sshoot/listing.py:36
 msgid "Extra options"
 msgstr "Opzioni aggiuntive"
 
-#: sshoot/listing.py:39
+#: sshoot/listing.py:40
 msgid "Name"
 msgstr "Nome"
 
-#: sshoot/listing.py:40
+#: sshoot/listing.py:41
 msgid "Status"
 msgstr "Stato"
 
-#: sshoot/listing.py:45
+#: sshoot/listing.py:46
 msgid "Invalid output format: {name}"
 msgstr "Formato di output invalido: {name}"
 
-#: sshoot/listing.py:148
+#: sshoot/listing.py:171
 msgid "ACTIVE"
 msgstr "ATTIVO"
 
-#: sshoot/listing.py:148
+#: sshoot/listing.py:171
 msgid "STOPPED"
 msgstr "INATTIVO"
 
-#: sshoot/main.py:74
+#: sshoot/main.py:88
 msgid "Profile started"
 msgstr "Profilo avviato"
 
-#: sshoot/main.py:79
+#: sshoot/main.py:93
 msgid "Profile stopped"
 msgstr "Profilo disattivato"
 
-#: sshoot/main.py:84
+#: sshoot/main.py:102
 msgid "Profile restarted"
 msgstr "Profilo riavviato"
 
-#: sshoot/main.py:100
+#: sshoot/main.py:123
 msgid "Manage multiple sshuttle VPN sessions"
 msgstr "Gestisci sessioni VPN sshuttle multiple"
 
-#: sshoot/main.py:111
+#: sshoot/main.py:135
 #, python-format
 msgid "configuration directory (default: %(default)s)"
 msgstr "directory di configurazione (predefinita: %(default)s)"
 
-#: sshoot/main.py:114
+#: sshoot/main.py:138
 msgid "action to perform"
 msgstr "azione da effettuare"
 
-#: sshoot/main.py:119
+#: sshoot/main.py:144
 msgid "list defined profiles"
 msgstr "lista profili definiti"
 
-#: sshoot/main.py:121
+#: sshoot/main.py:147
 msgid "verbose listing"
 msgstr "visualizza maggiori dettagli"
 
-#: sshoot/main.py:128
+#: sshoot/main.py:154
 #, python-format
 msgid "listing format (default %(default)s)"
 msgstr "formato lista (predefinito: %(default)s)"
 
-#: sshoot/main.py:133
+#: sshoot/main.py:159
 msgid "show profile configuration"
 msgstr "visualizza configurazione profilo"
 
-#: sshoot/main.py:136 sshoot/main.py:141
+#: sshoot/main.py:162 sshoot/main.py:170
 msgid "profile name"
 msgstr "nome profilo"
 
-#: sshoot/main.py:140
+#: sshoot/main.py:168
 msgid "define a new profile"
 msgstr "definisci un nuovo profilo"
 
-#: sshoot/main.py:143
+#: sshoot/main.py:172
 msgid "subnets to route over the VPN"
 msgstr "sottoreti da ruotare tramite VPN"
 
-#: sshoot/main.py:146
+#: sshoot/main.py:175
 msgid "remote host to connect to"
 msgstr "host remoto a cui connettersi"
 
-#: sshoot/main.py:152
+#: sshoot/main.py:181
 msgid "automatically update /etc/hosts with hosts from VPN"
 msgstr "aggiorna automaticamente /etc/hosts con hosts dalla VPN"
 
-#: sshoot/main.py:158
+#: sshoot/main.py:187
 msgid "automatically route additional nets from server"
 msgstr "ruota automaticamente le reti dal server"
 
-#: sshoot/main.py:164
+#: sshoot/main.py:193
 msgid "forward DNS queries through the VPN"
 msgstr "invia le richieste DNS attraverso la VPN"
 
-#: sshoot/main.py:170
+#: sshoot/main.py:199
 msgid "exclude subnets from VPN forward"
 msgstr "escludi sottoreti dall'invio tramite VPN"
 
-#: sshoot/main.py:176
+#: sshoot/main.py:205
 msgid "comma-separated list of hosts to seed to auto-hosts"
 msgstr "lista (separata da virgole) degli host da specificare ad auto-hosts"
 
-#: sshoot/main.py:181
+#: sshoot/main.py:210
 msgid "extra arguments to pass to sshuttle command line"
 msgstr "opzioni aggiuntive da passare alla linea di comando di sshuttle"
 
-#: sshoot/main.py:186
+#: sshoot/main.py:215
 msgid "delete an existing profile"
 msgstr "cancella un profilo esistente"
 
-#: sshoot/main.py:189
+#: sshoot/main.py:219
 msgid "name of the profile to remove"
 msgstr "nome del profilo da rimuovere"
 
-#: sshoot/main.py:195
+#: sshoot/main.py:226
 msgid "start a VPN session for a profile"
 msgstr "avvia la sessione VPN per un profilo"
 
-#: sshoot/main.py:198
+#: sshoot/main.py:230
 msgid "name of the profile to start"
 msgstr "nome del profilo da attivare"
 
-#: sshoot/main.py:204 sshoot/main.py:229
+#: sshoot/main.py:238 sshoot/main.py:271 sshoot/main.py:304
+msgid "disable global extra-options set in config.yaml"
+msgstr "disabilita le opzioni globali presenti in config.yaml"
+
+#: sshoot/main.py:243 sshoot/main.py:276
 msgid "additional arguments passed to sshuttle command line"
 msgstr "opzioni aggiuntive da passare alla linea di comando di sshuttle"
 
-#: sshoot/main.py:209
+#: sshoot/main.py:248
 msgid "stop a running VPN session for a profile"
 msgstr "disattiva una sessione VPN attiva per un profilo"
 
-#: sshoot/main.py:212
+#: sshoot/main.py:252
 msgid "name of the profile to stop"
 msgstr "nome del profilo da disattivare"
 
-#: sshoot/main.py:218
+#: sshoot/main.py:259
 msgid "restart a VPN session for a profile"
 msgstr "riavvia la sessione VPN per un profilo"
 
-#: sshoot/main.py:222
+#: sshoot/main.py:263
 msgid "name of the profile to restart"
 msgstr "nome del profilo da riavviare"
 
-#: sshoot/main.py:234
+#: sshoot/main.py:281
 msgid "return whether a profile is running"
 msgstr "ritorna se un profilo è attivo"
 
-#: sshoot/main.py:238
+#: sshoot/main.py:285
 msgid "name of the profile to query"
 msgstr "nome del profilo da interrogare"
 
-#: sshoot/main.py:245
+#: sshoot/main.py:292
 msgid "return the sshuttle command for a profile"
 msgstr "ritorna il comando sshuttle per un profilo"
 
-#: sshoot/main.py:248
+#: sshoot/main.py:296
 msgid "name of the profile"
 msgstr "nomde del profilo"
 
-#: sshoot/main.py:268
-msgid "NOTICE: configuration tree moved from {old_path} to {new_path}\n"
-msgstr "NOTA: la configurazione è stata spostata da {old_path} a {new_path}\n"
-
-#: sshoot/manager.py:62
+#: sshoot/manager.py:66
 msgid "Profile name already in use: {name}"
 msgstr "Nome di profilo già in uso: {name}"
 
-#: sshoot/manager.py:73 sshoot/manager.py:86
+#: sshoot/manager.py:78 sshoot/manager.py:93
 msgid "Unknown profile: {name}"
 msgstr "Profilo sconosciuto: {name}"
 
-#: sshoot/manager.py:91
+#: sshoot/manager.py:104
 msgid "Profile is already running"
 msgstr "Il profilo è già attivo"
 
-#: sshoot/manager.py:94
+#: sshoot/manager.py:111
 msgid "Profile failed to start: {error}"
 msgstr "Attivazione del profilo fallita: {error}"
 
-#: sshoot/manager.py:115
+#: sshoot/manager.py:134
 msgid "Profile is not running"
 msgstr "Il profilo non è attivo"
 
-#: sshoot/manager.py:122
+#: sshoot/manager.py:141
 msgid "Failed to stop profile: {error}"
 msgstr "Disattivazione del profilo fallita: {error}"
 
-#: sshoot/manager.py:175
+#: sshoot/manager.py:215
 msgid "Failed to kill process {pid}"
 msgstr "Terminazione del processo {pid} fallita"
 
-#: sshoot/profile.py:39
+#: sshoot/profile.py:38
 msgid "Profile missing 'subnets' config"
 msgstr "Opzione 'subnets' mancante nella configurazione del profilo"
 
 #: sshoot/profile.py:49
 msgid "Invalid profile config '{key}'"
 msgstr "Chiave '{key}' non valida nella configurazione del profilo"
 
+#~ msgid "NOTICE: configuration tree moved from {old_path} to {new_path}\n"
+#~ msgstr "NOTA: la configurazione è stata spostata da {old_path} a {new_path}\n"
+
```

### Comparing `sshoot-1.5.1/sshoot/locale/sshoot.pot` & `sshoot-1.6.0/sshoot/locale/sshoot.pot`

 * *Files 17% similar despite different names*

```diff
@@ -1,245 +1,245 @@
 # Translations template for sshoot.
-# Copyright (C) 2020 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the sshoot project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: sshoot 1.4.2\n"
+"Project-Id-Version: sshoot VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-11-15 11:01+0100\n"
+"POT-Creation-Date: 2023-05-10 08:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: sshoot/listing.py:28
+#: sshoot/listing.py:29
 msgid "Remote host"
 msgstr ""
 
-#: sshoot/listing.py:29
+#: sshoot/listing.py:30
 msgid "Subnets"
 msgstr ""
 
-#: sshoot/listing.py:30
+#: sshoot/listing.py:31
 msgid "Auto hosts"
 msgstr ""
 
-#: sshoot/listing.py:31
+#: sshoot/listing.py:32
 msgid "Auto nets"
 msgstr ""
 
-#: sshoot/listing.py:32
+#: sshoot/listing.py:33
 msgid "DNS forward"
 msgstr ""
 
-#: sshoot/listing.py:33
+#: sshoot/listing.py:34
 msgid "Exclude subnets"
 msgstr ""
 
-#: sshoot/listing.py:34
+#: sshoot/listing.py:35
 msgid "Seed hosts"
 msgstr ""
 
-#: sshoot/listing.py:35
+#: sshoot/listing.py:36
 msgid "Extra options"
 msgstr ""
 
-#: sshoot/listing.py:39
+#: sshoot/listing.py:40
 msgid "Name"
 msgstr ""
 
-#: sshoot/listing.py:40
+#: sshoot/listing.py:41
 msgid "Status"
 msgstr ""
 
-#: sshoot/listing.py:45
+#: sshoot/listing.py:46
 msgid "Invalid output format: {name}"
 msgstr ""
 
-#: sshoot/listing.py:148
+#: sshoot/listing.py:171
 msgid "ACTIVE"
 msgstr ""
 
-#: sshoot/listing.py:148
+#: sshoot/listing.py:171
 msgid "STOPPED"
 msgstr ""
 
-#: sshoot/main.py:74
+#: sshoot/main.py:88
 msgid "Profile started"
 msgstr ""
 
-#: sshoot/main.py:79
+#: sshoot/main.py:93
 msgid "Profile stopped"
 msgstr ""
 
-#: sshoot/main.py:84
+#: sshoot/main.py:102
 msgid "Profile restarted"
 msgstr ""
 
-#: sshoot/main.py:100
+#: sshoot/main.py:123
 msgid "Manage multiple sshuttle VPN sessions"
 msgstr ""
 
-#: sshoot/main.py:111
+#: sshoot/main.py:135
 #, python-format
 msgid "configuration directory (default: %(default)s)"
 msgstr ""
 
-#: sshoot/main.py:114
+#: sshoot/main.py:138
 msgid "action to perform"
 msgstr ""
 
-#: sshoot/main.py:119
+#: sshoot/main.py:144
 msgid "list defined profiles"
 msgstr ""
 
-#: sshoot/main.py:121
+#: sshoot/main.py:147
 msgid "verbose listing"
 msgstr ""
 
-#: sshoot/main.py:128
+#: sshoot/main.py:154
 #, python-format
 msgid "listing format (default %(default)s)"
 msgstr ""
 
-#: sshoot/main.py:133
+#: sshoot/main.py:159
 msgid "show profile configuration"
 msgstr ""
 
-#: sshoot/main.py:136 sshoot/main.py:141
+#: sshoot/main.py:162 sshoot/main.py:170
 msgid "profile name"
 msgstr ""
 
-#: sshoot/main.py:140
+#: sshoot/main.py:168
 msgid "define a new profile"
 msgstr ""
 
-#: sshoot/main.py:143
+#: sshoot/main.py:172
 msgid "subnets to route over the VPN"
 msgstr ""
 
-#: sshoot/main.py:146
+#: sshoot/main.py:175
 msgid "remote host to connect to"
 msgstr ""
 
-#: sshoot/main.py:152
+#: sshoot/main.py:181
 msgid "automatically update /etc/hosts with hosts from VPN"
 msgstr ""
 
-#: sshoot/main.py:158
+#: sshoot/main.py:187
 msgid "automatically route additional nets from server"
 msgstr ""
 
-#: sshoot/main.py:164
+#: sshoot/main.py:193
 msgid "forward DNS queries through the VPN"
 msgstr ""
 
-#: sshoot/main.py:170
+#: sshoot/main.py:199
 msgid "exclude subnets from VPN forward"
 msgstr ""
 
-#: sshoot/main.py:176
+#: sshoot/main.py:205
 msgid "comma-separated list of hosts to seed to auto-hosts"
 msgstr ""
 
-#: sshoot/main.py:181
+#: sshoot/main.py:210
 msgid "extra arguments to pass to sshuttle command line"
 msgstr ""
 
-#: sshoot/main.py:186
+#: sshoot/main.py:215
 msgid "delete an existing profile"
 msgstr ""
 
-#: sshoot/main.py:189
+#: sshoot/main.py:219
 msgid "name of the profile to remove"
 msgstr ""
 
-#: sshoot/main.py:195
+#: sshoot/main.py:226
 msgid "start a VPN session for a profile"
 msgstr ""
 
-#: sshoot/main.py:198
+#: sshoot/main.py:230
 msgid "name of the profile to start"
 msgstr ""
 
-#: sshoot/main.py:204 sshoot/main.py:229
+#: sshoot/main.py:238 sshoot/main.py:271 sshoot/main.py:304
+msgid "disable global extra-options set in config.yaml"
+msgstr ""
+
+#: sshoot/main.py:243 sshoot/main.py:276
 msgid "additional arguments passed to sshuttle command line"
 msgstr ""
 
-#: sshoot/main.py:209
+#: sshoot/main.py:248
 msgid "stop a running VPN session for a profile"
 msgstr ""
 
-#: sshoot/main.py:212
+#: sshoot/main.py:252
 msgid "name of the profile to stop"
 msgstr ""
 
-#: sshoot/main.py:218
+#: sshoot/main.py:259
 msgid "restart a VPN session for a profile"
 msgstr ""
 
-#: sshoot/main.py:222
+#: sshoot/main.py:263
 msgid "name of the profile to restart"
 msgstr ""
 
-#: sshoot/main.py:234
+#: sshoot/main.py:281
 msgid "return whether a profile is running"
 msgstr ""
 
-#: sshoot/main.py:238
+#: sshoot/main.py:285
 msgid "name of the profile to query"
 msgstr ""
 
-#: sshoot/main.py:245
+#: sshoot/main.py:292
 msgid "return the sshuttle command for a profile"
 msgstr ""
 
-#: sshoot/main.py:248
+#: sshoot/main.py:296
 msgid "name of the profile"
 msgstr ""
 
-#: sshoot/main.py:268
-msgid "NOTICE: configuration tree moved from {old_path} to {new_path}\n"
-msgstr ""
-
-#: sshoot/manager.py:62
+#: sshoot/manager.py:66
 msgid "Profile name already in use: {name}"
 msgstr ""
 
-#: sshoot/manager.py:73 sshoot/manager.py:86
+#: sshoot/manager.py:78 sshoot/manager.py:93
 msgid "Unknown profile: {name}"
 msgstr ""
 
-#: sshoot/manager.py:91
+#: sshoot/manager.py:104
 msgid "Profile is already running"
 msgstr ""
 
-#: sshoot/manager.py:94
+#: sshoot/manager.py:111
 msgid "Profile failed to start: {error}"
 msgstr ""
 
-#: sshoot/manager.py:115
+#: sshoot/manager.py:134
 msgid "Profile is not running"
 msgstr ""
 
-#: sshoot/manager.py:122
+#: sshoot/manager.py:141
 msgid "Failed to stop profile: {error}"
 msgstr ""
 
-#: sshoot/manager.py:175
+#: sshoot/manager.py:215
 msgid "Failed to kill process {pid}"
 msgstr ""
 
-#: sshoot/profile.py:39
+#: sshoot/profile.py:38
 msgid "Profile missing 'subnets' config"
 msgstr ""
 
 #: sshoot/profile.py:49
 msgid "Invalid profile config '{key}'"
 msgstr ""
```

### Comparing `sshoot-1.5.1/sshoot/main.py` & `sshoot-1.6.0/sshoot/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class Sshoot(Script):
     """Manage multiple sshuttle VPN sessions."""
 
     def main(self, args: Namespace):
         try:
             manager = Manager(config_path=args.config)
             manager.load_config()
-        except IOError as error:
+        except OSError as error:
             raise ErrorExitMessage(error, code=3)
         action = args.action.replace("-", "_")
         method = getattr(self, "action_" + action)
         action_args = Namespace(
             **{
                 key: value
                 for key, value in args.__dict__.items()
@@ -56,15 +56,17 @@
     def print(self, *args, **kwargs):
         """Print out message."""
         print(*args, **kwargs, file=self._stdout)
 
     def action_list(self, manager: Manager, args: Namespace):
         """Print out the list of profiles as a table."""
         listing = ProfileListing(manager)
-        self.print(listing.get_output(args.format, verbose=args.verbose), end="")
+        self.print(
+            listing.get_output(args.format, verbose=args.verbose), end=""
+        )
 
     def action_show(self, manager: Manager, args: Namespace):
         """Show details on a profile."""
         self.print(profile_details(manager, args.name))
 
     def action_create(self, manager: Manager, args: Namespace):
         """Create a new profile."""
@@ -74,61 +76,77 @@
 
     def action_delete(self, manager: Manager, args: Namespace):
         """Delete profile with the given name."""
         manager.remove_profile(args.name)
 
     def action_start(self, manager: Manager, args: Namespace):
         """Start sshuttle for the specified profile."""
-        manager.start_profile(args.name, extra_args=args.args)
+        manager.start_profile(
+            args.name,
+            extra_args=args.args,
+            disable_global_extra_options=args.disable_global_extra_options,
+        )
         self.print(_("Profile started"))
 
     def action_stop(self, manager: Manager, args: Namespace):
         """Stop sshuttle for the specified profile."""
         manager.stop_profile(args.name)
         self.print(_("Profile stopped"))
 
     def action_restart(self, manager: Manager, args: Namespace):
         """Restart sshuttle for the specified profile."""
-        manager.restart_profile(args.name, extra_args=args.args)
+        manager.restart_profile(
+            args.name,
+            extra_args=args.args,
+            disable_global_extra_options=args.disable_global_extra_options,
+        )
         self.print(_("Profile restarted"))
 
     def action_is_running(self, manager: Manager, args: Namespace):
         """Return whether the specified profile is running."""
         # raise an error if profile is unknown
         manager.get_profile(args.name)
         retval = 0 if manager.is_running(args.name) else 1
         self.exit(retval)
 
     def action_get_command(self, manager: Manager, args: Namespace):
         """Print the sshuttle command for the specified profile."""
-        cmdline = manager.get_cmdline(args.name)
+        cmdline = manager.get_cmdline(
+            args.name,
+            disable_global_extra_options=args.disable_global_extra_options,
+        )
         self.print(" ".join(cmdline))
 
     def get_parser(self) -> ArgumentParser:
         """Return a configured argparse.ArgumentParse instance."""
-        parser = ArgumentParser(description=_("Manage multiple sshuttle VPN sessions"))
+        parser = ArgumentParser(
+            prog="sshoot",
+            description=_("Manage multiple sshuttle VPN sessions"),
+        )
         parser.add_argument(
             "-V",
             "--version",
             action="version",
-            version="%(prog)s {}".format(__version__),
+            version=f"%(prog)s {__version__}",
         )
         parser.add_argument(
             "-C",
             "--config",
             default=DEFAULT_CONFIG_PATH,
             help=_("configuration directory (default: %(default)s)"),
         )
         subparsers = parser.add_subparsers(
             metavar="ACTION", dest="action", help=_("action to perform")
         )
         subparsers.required = True
 
         # List profiles
-        list_parser = subparsers.add_parser("list", help=_("list defined profiles"))
+        list_parser = subparsers.add_parser(
+            "list", help=_("list defined profiles")
+        )
         list_parser.add_argument(
             "-v", "--verbose", action="store_true", help=_("verbose listing")
         )
         list_parser.add_argument(
             "-f",
             "--format",
             choices=ProfileListing.supported_formats(),
@@ -137,19 +155,22 @@
         )
 
         # Show profile
         show_parser = subparsers.add_parser(
             "show", help=_("show profile configuration")
         )
         complete_argument(
-            show_parser.add_argument("name", help=_("profile name")), profile_completer
+            show_parser.add_argument("name", help=_("profile name")),
+            profile_completer,
         )
 
         # Add profile
-        create_parser = subparsers.add_parser("create", help=_("define a new profile"))
+        create_parser = subparsers.add_parser(
+            "create", help=_("define a new profile")
+        )
         create_parser.add_argument("name", help=_("profile name"))
         create_parser.add_argument(
             "subnets", nargs="+", help=_("subnets to route over the VPN")
         )
         create_parser.add_argument(
             "-r", "--remote", help=_("remote host to connect to")
         )
@@ -190,52 +211,70 @@
         )
 
         # Remove profile
         delete_parser = subparsers.add_parser(
             "delete", help=_("delete an existing profile")
         )
         complete_argument(
-            delete_parser.add_argument("name", help=_("name of the profile to remove")),
+            delete_parser.add_argument(
+                "name", help=_("name of the profile to remove")
+            ),
             profile_completer,
         )
 
         # Start profile
         start_parser = subparsers.add_parser(
             "start", help=_("start a VPN session for a profile")
         )
         complete_argument(
-            start_parser.add_argument("name", help=_("name of the profile to start")),
+            start_parser.add_argument(
+                "name", help=_("name of the profile to start")
+            ),
             partial(profile_completer, running=False),
         )
         start_parser.add_argument(
+            "--no-global-extra-options",
+            dest="disable_global_extra_options",
+            action="store_true",
+            help=_("disable global extra-options set in config.yaml"),
+        )
+        start_parser.add_argument(
             "args",
             nargs="*",
             help=_("additional arguments passed to sshuttle command line"),
         )
 
         # Stop profile
         stop_parser = subparsers.add_parser(
             "stop", help=_("stop a running VPN session for a profile")
         )
         complete_argument(
-            stop_parser.add_argument("name", help=_("name of the profile to stop")),
+            stop_parser.add_argument(
+                "name", help=_("name of the profile to stop")
+            ),
             partial(profile_completer, running=True),
         )
 
         # Restart profile
         restart_parser = subparsers.add_parser(
             "restart", help=_("restart a VPN session for a profile")
         )
         complete_argument(
             restart_parser.add_argument(
                 "name", help=_("name of the profile to restart")
             ),
             partial(profile_completer, running=True),
         )
         restart_parser.add_argument(
+            "--no-global-extra-options",
+            dest="disable_global_extra_options",
+            action="store_true",
+            help=_("disable global extra-options set in config.yaml"),
+        )
+        restart_parser.add_argument(
             "args",
             nargs="*",
             help=_("additional arguments passed to sshuttle command line"),
         )
 
         # Return whether profile is running
         is_running_parser = subparsers.add_parser(
@@ -249,22 +288,32 @@
         )
 
         # Get profile command
         get_command_parser = subparsers.add_parser(
             "get-command", help=_("return the sshuttle command for a profile")
         )
         complete_argument(
-            get_command_parser.add_argument("name", help=_("name of the profile")),
+            get_command_parser.add_argument(
+                "name", help=_("name of the profile")
+            ),
             profile_completer,
         )
+        get_command_parser.add_argument(
+            "--no-global-extra-options",
+            dest="disable_global_extra_options",
+            action="store_true",
+            help=_("disable global extra-options set in config.yaml"),
+        )
 
         # track global arguments/options so they can be stripped from action namespace
         self.global_args: Set[str] = set()
         for group in parser._action_groups:
-            self.global_args.update(action.dest for action in group._group_actions)
+            self.global_args.update(
+                action.dest for action in group._group_actions
+            )
 
         # Setup autocompletion
         autocomplete(parser)
         return parser
 
 
 sshoot = Sshoot()
```

### Comparing `sshoot-1.5.1/sshoot/manager.py` & `sshoot-1.6.0/sshoot/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,16 +37,20 @@
 class ManagerProfileError(Exception):
     """Profile operation failed."""
 
 
 class Manager:
     """Profile manager."""
 
-    def __init__(self, config_path: Optional[str] = None, rundir: Optional[str] = None):
-        self.config_path = Path(config_path) if config_path else DEFAULT_CONFIG_PATH
+    def __init__(
+        self, config_path: Optional[str] = None, rundir: Optional[str] = None
+    ):
+        self.config_path = (
+            Path(config_path) if config_path else DEFAULT_CONFIG_PATH
+        )
         self.rundir = Path(rundir) if rundir else get_rundir("sshoot")
         self.sessions_path = self.rundir / "sessions"
         self._config = Config(self.config_path)
 
     def load_config(self):
         """Load configuration from file."""
         self.config_path.mkdir(parents=True, exist_ok=True)
@@ -66,71 +70,95 @@
         self._config.save()
 
     def remove_profile(self, name: str):
         """Remove profile with given name."""
         try:
             self._config.remove_profile(name)
         except KeyError:
-            raise ManagerProfileError(_("Unknown profile: {name}").format(name=name))
+            raise ManagerProfileError(
+                _("Unknown profile: {name}").format(name=name)
+            )
 
         self._config.save()
 
     def get_profiles(self) -> Dict[str, Profile]:
         """Return profiles defined in config."""
         return self._config.profiles
 
     def get_profile(self, name: str) -> Profile:
         """Return profile with given name."""
         try:
             return self._config.profiles[name]
         except KeyError:
-            raise ManagerProfileError(_("Unknown profile: {name}").format(name=name))
+            raise ManagerProfileError(
+                _("Unknown profile: {name}").format(name=name)
+            )
 
-    def start_profile(self, name: str, extra_args: Optional[List[str]] = None):
+    def start_profile(
+        self,
+        name: str,
+        extra_args: Optional[List[str]] = None,
+        disable_global_extra_options: bool = False,
+    ):
         """Start profile with given name."""
         if self.is_running(name):
             raise ManagerProfileError(_("Profile is already running"))
 
-        cmdline = self.get_cmdline(name, extra_args=extra_args)
+        cmdline = self.get_cmdline(
+            name,
+            extra_args=extra_args,
+            disable_global_extra_options=disable_global_extra_options,
+        )
         message = _("Profile failed to start: {error}")
         try:
             process = Popen(cmdline, stderr=PIPE)
             # Wait until process is started (it daemonizes)
             process.wait()
         except OSError as err:
             # To catch file not found errors
             raise ManagerProfileError(message.format(error=str(err)))
 
         stderr = cast(IO[bytes], process.stderr)
         if process.returncode != 0:
             error = stderr.read().decode()
             stderr.close()
+            if not error:
+                error = "Please see the log for more details: 'grep sshuttle /var/log/syslog'"
             raise ManagerProfileError(message.format(error=error))
         stderr.close()
 
     def stop_profile(self, name: str):
         """Stop profile with given name."""
         self.get_profile(name)
 
         if not self.is_running(name):
             raise ManagerProfileError(_("Profile is not running"))
 
         try:
             pid = int(self._get_pidfile(name).read_text())
             kill_and_wait(pid)
-        except (IOError, OSError, PermissionError) as error:
+        except (OSError, PermissionError) as error:
             raise ManagerProfileError(
                 _("Failed to stop profile: {error}").format(error=error)
             )
 
-    def restart_profile(self, name: str, extra_args: Optional[List[str]] = None):
+    def restart_profile(
+        self,
+        name: str,
+        extra_args: Optional[List[str]] = None,
+        disable_global_extra_options: bool = False,
+    ):
         """Restart profile with given name."""
         if self.is_running(name):
             self.stop_profile(name)
-        self.start_profile(name, extra_args=extra_args)
+        self.start_profile(
+            name,
+            extra_args=extra_args,
+            disable_global_extra_options=disable_global_extra_options,
+        )
 
     def is_running(self, name: str) -> bool:
         """Return whether the specified profile is running."""
         pidfile = self._get_pidfile(name)
         try:
             pid = int(pidfile.read_text())
         except Exception:
@@ -143,28 +171,40 @@
         except ProcessLookupError:
             # Delete stale pidfile
             pidfile.unlink()
             return False
         return True
 
     def get_cmdline(
-        self, name: str, extra_args: Optional[List[str]] = None
+        self,
+        name: str,
+        extra_args: Optional[List[str]] = None,
+        disable_global_extra_options: bool = False,
     ) -> List[str]:
         """Return the command line for the specified profile."""
         profile = self.get_profile(name)
 
         executable = self._get_executable()
         extra_opts = ["--daemon", "--pidfile", str(self._get_pidfile(name))]
+        global_extra_options = (
+            self._config.config.get("extra-options", [])
+            if not disable_global_extra_options
+            else []
+        )
         if extra_args:
             extra_opts.extend(extra_args)
-        return profile.cmdline(executable=executable, extra_opts=extra_opts)
+        return profile.cmdline(
+            executable=executable,
+            extra_opts=extra_opts,
+            global_extra_options=global_extra_options,
+        )
 
     def _get_pidfile(self, name: str) -> Path:
         """Return the path of the pidfile for the specified profile."""
-        return self.sessions_path / "{}.pid".format(name)
+        return self.sessions_path / f"{name}.pid"
 
     def _get_executable(self) -> str:
         """Return the shuttle executable from the config."""
         return self._config.config.get("executable", "sshuttle")
 
 
 class ProcessKillFail(Exception):
@@ -186,10 +226,8 @@
             wait -= 0.2
             time.sleep(0.2)
     raise ProcessKillFail(pid)
 
 
 def get_rundir(prefix: str) -> Path:
     """Return the directory holding runtime data."""
-    return Path(gettempdir()) / "{prefix}-{username}".format(
-        prefix=prefix, username=getuser()
-    )
+    return Path(gettempdir()) / f"{prefix}-{getuser()}"
```

### Comparing `sshoot-1.5.1/sshoot/profile.py` & `sshoot-1.6.0/sshoot/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import dataclasses
 from typing import (
     Any,
     Dict,
     List,
     Optional,
-    Set,
 )
 
 from .i18n import _
 
 
 class ProfileError(Exception):
     """Invalid profile configuration."""
@@ -38,49 +37,57 @@
         except KeyError:
             raise ProfileError(_("Profile missing 'subnets' config"))
         profile.update(config)
         return profile
 
     def update(self, config: Dict[str, Any]):
         """Update the profile from the specified config."""
-        field_names = self._field_names()
+        field_names = list(self._fields())
         for key, value in config.items():
             attr = key.replace("-", "_")
             if attr not in field_names:
-                raise ProfileError(_("Invalid profile config '{key}'").format(key=key))
+                raise ProfileError(
+                    _("Invalid profile config '{key}'").format(key=key)
+                )
             setattr(self, attr, value)
 
     def config(self) -> Dict[str, Any]:
         """Return profile configuration as a dict."""
         conf = {}
-        for attr in self._field_names():
+        for attr, default_value in self._fields().items():
             value = getattr(self, attr)
-            if value:
+            if value != default_value:
                 conf[attr.replace("_", "-")] = value
         return dict(conf)
 
     def cmdline(
-        self, executable: str = "sshuttle", extra_opts: Optional[List[str]] = None
+        self,
+        executable: str = "sshuttle",
+        extra_opts: Optional[List[str]] = None,
+        global_extra_options: Optional[List[str]] = None,
     ) -> List[str]:
         """Return a sshuttle cmdline based on the profile."""
         cmd = [executable] + self.subnets
         if self.remote:
-            cmd.append("--remote={}".format(self.remote))
+            cmd.append(f"--remote={self.remote}")
         if self.auto_hosts:
             cmd.append("--auto-hosts")
         if self.auto_nets:
             cmd.append("--auto-nets")
         if self.dns:
             cmd.append("--dns")
         if self.exclude_subnets:
-            cmd.extend("--exclude={}".format(net) for net in self.exclude_subnets)
+            cmd.extend(f"--exclude={net}" for net in self.exclude_subnets)
         if self.seed_hosts:
-            cmd.append("--seed-hosts={}".format(",".join(self.seed_hosts)))
+            seed_hosts = ",".join(self.seed_hosts)
+            cmd.append(f"--seed-hosts={seed_hosts}")
         if self.extra_opts:
             cmd.extend(self.extra_opts)
         if extra_opts:
             cmd.extend(extra_opts)
+        if global_extra_options:
+            cmd.extend(global_extra_options)
         return cmd
 
     @classmethod
-    def _field_names(cls) -> Set[str]:
-        return {field.name for field in dataclasses.fields(cls)}
+    def _fields(cls) -> Dict[str, Any]:
+        return {field.name: field.default for field in dataclasses.fields(cls)}
```

