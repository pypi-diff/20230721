# Comparing `tmp/mine-4.0a2.tar.gz` & `tmp/mine-4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-4.0a2.tar", max compression
+gzip compressed data, was "mine-4.0a3.tar", max compression
```

## Comparing `mine-4.0a2.tar` & `mine-4.0a3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.0a2/LICENSE.md
--rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-4.0a2/README.md
--rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-4.0a2/mine/__init__.py
--rw-r--r--   0        0        0     6860 2023-07-19 02:52:07.566131 mine-4.0a2/mine/cli.py
--rw-r--r--   0        0        0     2889 2023-07-19 02:12:18.943946 mine-4.0a2/mine/common.py
--rw-r--r--   0        0        0     6660 2023-07-19 03:21:57.599480 mine-4.0a2/mine/manager.py
--rw-r--r--   0        0        0      217 2023-07-19 02:12:18.944037 mine-4.0a2/mine/models/__init__.py
--rw-r--r--   0        0        0     1095 2023-07-19 03:18:20.515733 mine-4.0a2/mine/models/application.py
--rw-r--r--   0        0        0     2121 2023-07-19 02:18:02.802475 mine-4.0a2/mine/models/computer.py
--rw-r--r--   0        0        0     3721 2023-07-19 02:28:44.644217 mine-4.0a2/mine/models/config.py
--rw-r--r--   0        0        0     5413 2023-07-19 02:28:30.879778 mine-4.0a2/mine/models/data.py
--rw-r--r--   0        0        0     5863 2023-07-19 03:18:32.152880 mine-4.0a2/mine/models/status.py
--rw-r--r--   0        0        0      882 2023-07-19 02:12:18.944631 mine-4.0a2/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2720 2023-07-19 02:46:39.336705 mine-4.0a2/mine/services.py
--rw-r--r--   0        0        0      578 2023-07-19 02:12:18.944827 mine-4.0a2/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.0a2/mine/tests/__init__.py
--rw-r--r--   0        0        0     1043 2023-07-19 02:12:18.944974 mine-4.0a2/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.0a2/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.0a2/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.0a2/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     3994 2023-07-19 02:20:06.563001 mine-4.0a2/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-4.0a2/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.0a2/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     2193 2023-07-19 01:11:50.938810 mine-4.0a2/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0     3086 2023-07-19 02:12:18.936287 mine-4.0a2/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-4.0a2/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-4.0a2/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.0a2/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3226 2023-07-19 02:41:25.796394 mine-4.0a2/mine/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-07-19 19:46:56.656617 mine-4.0a2/pyproject.toml
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 mine-4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.0a3/LICENSE.md
+-rw-r--r--   0        0        0     2841 2023-07-19 21:05:32.369830 mine-4.0a3/README.md
+-rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-4.0a3/mine/__init__.py
+-rw-r--r--   0        0        0     6866 2023-07-19 22:27:02.284270 mine-4.0a3/mine/cli.py
+-rw-r--r--   0        0        0     2889 2023-07-19 02:12:18.943946 mine-4.0a3/mine/common.py
+-rw-r--r--   0        0        0     6665 2023-07-19 22:45:25.548783 mine-4.0a3/mine/manager.py
+-rw-r--r--   0        0        0      217 2023-07-19 02:12:18.944037 mine-4.0a3/mine/models/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-19 03:18:20.515733 mine-4.0a3/mine/models/application.py
+-rw-r--r--   0        0        0     2121 2023-07-19 02:18:02.802475 mine-4.0a3/mine/models/computer.py
+-rw-r--r--   0        0        0     3772 2023-07-19 22:18:01.818807 mine-4.0a3/mine/models/config.py
+-rw-r--r--   0        0        0     5413 2023-07-19 02:28:30.879778 mine-4.0a3/mine/models/data.py
+-rw-r--r--   0        0        0     5878 2023-07-19 22:22:09.135433 mine-4.0a3/mine/models/status.py
+-rw-r--r--   0        0        0      882 2023-07-19 02:12:18.944631 mine-4.0a3/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2720 2023-07-19 02:46:39.336705 mine-4.0a3/mine/services.py
+-rw-r--r--   0        0        0      578 2023-07-19 02:12:18.944827 mine-4.0a3/mine/settings.py
+-rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.0a3/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-19 22:32:22.022967 mine-4.0a3/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     3995 2023-07-19 22:16:31.053982 mine-4.0a3/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3493 2023-07-19 22:51:10.384382 mine-4.0a3/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.0a3/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     2193 2023-07-19 01:11:50.938810 mine-4.0a3/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0     3086 2023-07-19 02:12:18.936287 mine-4.0a3/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0      782 2023-07-19 21:55:07.916719 mine-4.0a3/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-4.0a3/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.0a3/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3226 2023-07-19 02:41:25.796394 mine-4.0a3/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-07-19 22:42:55.992809 mine-4.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 mine-4.0a3/PKG-INFO
```

### Comparing `mine-4.0a2/LICENSE.md` & `mine-4.0a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/README.md` & `mine-4.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
 [![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
 
 ## Setup
 
 ### Requirements
 
-- Python 3.7+
+- Python 3.10+
 
 ### Installation
 
 Install `mine` with [pipx](https://pipxproject.github.io/pipx/installation/) (or pip):
 
 ```sh
 $ pipx install mine
```

### Comparing `mine-4.0a2/mine/cli.py` & `mine-4.0a3/mine/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     manager = get_manager()
     if not manager.is_running(services.APPLICATION):
         manager.start(services.APPLICATION)
 
     root = services.find_root()
     path = path or services.find_config_path(root=root)
 
-    data = create_model(Data, pattern=path, defaults=True)()
+    data: Data = create_model(Data, pattern=path, defaults=True)()
 
     config = data.config
     status = data.status
 
     log.info("Identifying current computer...")
     computer = config.get_current_computer()
     log.info("Current computer: %s", computer)
```

### Comparing `mine-4.0a2/mine/common.py` & `mine-4.0a3/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/manager.py` & `mine-4.0a3/mine/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,23 @@
 
     @abc.abstractmethod
     def stop(self, application):
         """Stop an application on the current computer."""
         raise NotImplementedError
 
     @classmethod
-    def _get_process(cls, name):
+    def _get_process(cls, name: str):
         """Get a process whose executable path contains an app name."""
         log.debug("Searching for exe path containing '%s'...", name)
 
         for process in psutil.process_iter():
+            if process.status() == psutil.STATUS_ZOMBIE:
+                log.debug("Skipped zombie process: %s", process)
+                continue
+
             try:
                 command = " ".join(process.cmdline()).lower()
                 parts = []
                 for arg in process.cmdline():
                     parts.extend([p.lower() for p in arg.split(os.sep)])
             except psutil.AccessDenied:
                 continue  # the process is likely owned by root
@@ -99,18 +103,14 @@
             if name.lower() not in parts:
                 continue
 
             if process.pid == os.getpid():
                 log.debug("Skipped current process: %s", command)
                 continue
 
-            if process.status() == psutil.STATUS_ZOMBIE:
-                log.debug("Skipped zombie process: %s", command)
-                continue
-
             log.debug("Found matching process: %s", command)
             for ignored in cls.IGNORED_APPLICATION_NAMES:
                 if ignored.lower() in parts:
                     log.debug("But skipped due to ignored name")
                     break
             else:
                 return process
```

### Comparing `mine-4.0a2/mine/models/application.py` & `mine-4.0a3/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/models/computer.py` & `mine-4.0a3/mine/models/computer.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/models/config.py` & `mine-4.0a3/mine/models/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         for computer in self.computers:
             if partial.lower() in computer.name.lower():
                 matches.append(computer)
         if matches:
             return min(matches, key=lambda computer: len(computer.name))
         return None
 
-    def get_current_computer(self):
+    def get_current_computer(self, default_name: str = ""):
         """Get the current computer's information."""
-        this = Computer("")
+        this = Computer("?")
         log.debug(f"Comparing information with {this!r}...")
 
         # Search for a matching hostname
         for other in self.computers:
             if this.hostname == other.hostname:
                 log.debug(f"Matched via hostname: {other!r}")
                 other.address = this.address
@@ -72,17 +72,17 @@
                 log.debug(f"Matched via address: {other!r}")
                 other.hostname = this.hostname
                 if this.serial:
                     other.serial = this.serial
                 return other
 
         # Else, this is a new computer
-        this.name = self.generate_computer_name(this)
+        this.name = default_name or self.generate_computer_name(this)
         assert this.name != "localhost"
-        log.debug("New computer: %s", this)
+        log.debug(f"Detected new computer: {this!r}")
         self.computers.append(this)
         return this
 
     def generate_computer_name(self, computer: Computer):
         """Generate a new label for a computer."""
         name = computer.hostname.lower().split(".")[0]
         copy = 1
```

### Comparing `mine-4.0a2/mine/models/data.py` & `mine-4.0a3/mine/models/data.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/models/status.py` & `mine-4.0a3/mine/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                         "%s marked as started on: %s",
                         application,
                         ", ".join(str(s) for s in states),
                     )
                     # TODO: consider returning the computer instance?
                     return states[0].computer
 
-        log.debug("marked as started on: nothing")
+        log.debug(f"{application} marked as started on: nothing")
         return None
 
     @log_running
     def is_running(self, application, computer):
         """Determine if an application is logged as running on a computer."""
         for status in self.applications:
             if status.application == application.name:
```

### Comparing `mine-4.0a2/mine/models/timestamp.py` & `mine-4.0a3/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/services.py` & `mine-4.0a3/mine/services.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/settings.py` & `mine-4.0a3/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/conftest.py` & `mine-4.0a3/mine/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
     terminal = config.pluginmanager.getplugin("terminal")
     terminal.TerminalReporter.showfspath = False
 
 
 def pytest_runtest_setup(item):
     if "linux_only" in item.keywords and platform.system() != "Linux":
-        pytest.skip("test can only be run on Linux")
+        pytest.skip("Test can only be run on Linux")
     if "mac_only" in item.keywords and platform.system() != "Darwin":
-        pytest.skip("test can only be run on OS X")
+        pytest.skip("Test can only be run on macOS")
     if "windows_only" in item.keywords and platform.system() != "Windows":
-        pytest.skip("test can only be run on Windows")
+        pytest.skip("Test can only be run on Windows")
```

### Comparing `mine-4.0a2/mine/tests/files/mine-in.yml` & `mine-4.0a3/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/files/mine-out.yml` & `mine-4.0a3/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_cli.py` & `mine-4.0a3/mine/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         mock_run.assert_called_once_with(path=None, delay=300)
 
     @patch("mine.cli.run")
     def test_daemon_with_specific_delay(self, mock_run):
         cli.main(["--daemon", "42"])
         mock_run.assert_called_once_with(path=None, delay=42)
 
-    @patch("mine.cli.daemon", Application(""))
+    @patch("mine.cli.daemon", Application("?"))
     def test_warning_when_daemon_is_not_running(self, tmp_path):
         with pytest.raises(SystemExit):
             cli.main(["--file", tmp_path])
 
 
 class TestSwitch:
     """Unit tests for the `switch` function."""
```

### Comparing `mine-4.0a2/mine/tests/test_models_application.py` & `mine-4.0a3/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_models_computer.py` & `mine-4.0a3/mine/tests/test_models_computer.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_models_config.py` & `mine-4.0a3/mine/tests/test_models_config.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_models_data.py` & `mine-4.0a3/mine/tests/test_models_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # pylint: disable=unused-variable
 
+import datafiles
 import pytest
 
 from mine.models import Data
 
 
 def describe_data():
     @pytest.fixture
-    def data():
+    def data(monkeypatch):
+        monkeypatch.setattr(datafiles.settings, "HOOKS_ENABLED", False)
         return Data()
 
     def describe_repr():
         def it_should_always_be_a_simple_name(data):
             assert "settings" == repr(data)
 
     def describe_modified():
```

### Comparing `mine-4.0a2/mine/tests/test_models_status.py` & `mine-4.0a3/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_models_timestamp.py` & `mine-4.0a3/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/mine/tests/test_services.py` & `mine-4.0a3/mine/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a2/pyproject.toml` & `mine-4.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "4.0a2"
+version = "4.0a3"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `mine-4.0a2/PKG-INFO` & `mine-4.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 4.0a2
+Version: 4.0a3
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,15 +59,15 @@
 [![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/jacebrowning/mine.svg)](https://scrutinizer-ci.com/g/jacebrowning/mine/?branch=main)
 [![PyPI Version](https://img.shields.io/pypi/v/mine.svg)](https://pypi.org/project/mine)
 
 ## Setup
 
 ### Requirements
 
-- Python 3.7+
+- Python 3.10+
 
 ### Installation
 
 Install `mine` with [pipx](https://pipxproject.github.io/pipx/installation/) (or pip):
 
 ```sh
 $ pipx install mine
```

