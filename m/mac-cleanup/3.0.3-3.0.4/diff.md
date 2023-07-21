# Comparing `tmp/mac_cleanup-3.0.3.tar.gz` & `tmp/mac_cleanup-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mac_cleanup-3.0.3.tar", max compression
+gzip compressed data, was "mac_cleanup-3.0.4.tar", max compression
```

## Comparing `mac_cleanup-3.0.3.tar` & `mac_cleanup-3.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-11 22:17:44.340035 mac_cleanup-3.0.3/LICENSE
--rw-r--r--   0        0        0     3831 2023-05-20 17:39:59.781578 mac_cleanup-3.0.3/README.md
--rw-r--r--   0        0        0      425 2023-05-11 22:17:44.340449 mac_cleanup-3.0.3/mac_cleanup/__init__.py
--rw-r--r--   0        0        0      181 2023-05-11 22:17:44.340660 mac_cleanup-3.0.3/mac_cleanup/__version__.py
--rw-r--r--   0        0        0     8289 2023-05-20 17:35:49.810064 mac_cleanup-3.0.3/mac_cleanup/config.py
--rw-r--r--   0        0        0      652 2023-05-20 17:35:49.810403 mac_cleanup-3.0.3/mac_cleanup/console.py
--rw-r--r--   0        0        0     7720 2023-05-20 17:35:49.810702 mac_cleanup-3.0.3/mac_cleanup/core.py
--rw-r--r--   0        0        0     4185 2023-05-20 17:35:49.811119 mac_cleanup-3.0.3/mac_cleanup/core_modules.py
--rw-r--r--   0        0        0    14634 2023-05-20 17:36:58.239398 mac_cleanup-3.0.3/mac_cleanup/default_modules.py
--rw-r--r--   0        0        0     3790 2023-05-20 17:35:49.811893 mac_cleanup-3.0.3/mac_cleanup/error_handling.py
--rw-r--r--   0        0        0     2918 2023-05-11 22:17:44.341805 mac_cleanup-3.0.3/mac_cleanup/main.py
--rw-r--r--   0        0        0     1181 2023-05-11 22:17:44.341922 mac_cleanup-3.0.3/mac_cleanup/parser.py
--rw-r--r--   0        0        0     3378 2023-05-20 17:35:49.812177 mac_cleanup-3.0.3/mac_cleanup/progress.py
--rwxr-xr-x   0        0        0     3176 2023-05-20 17:35:49.812475 mac_cleanup-3.0.3/mac_cleanup/utils.py
--rw-r--r--   0        0        0     2946 2023-05-20 17:39:59.756956 mac_cleanup-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     4971 1970-01-01 00:00:00.000000 mac_cleanup-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 22:17:44.340035 mac_cleanup-3.0.4/LICENSE
+-rw-r--r--   0        0        0     4325 2023-07-21 00:13:06.751976 mac_cleanup-3.0.4/README.md
+-rw-r--r--   0        0        0      445 2023-07-21 00:13:06.752878 mac_cleanup-3.0.4/mac_cleanup/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-11 22:17:44.340660 mac_cleanup-3.0.4/mac_cleanup/__version__.py
+-rw-r--r--   0        0        0     8289 2023-07-20 20:59:09.610960 mac_cleanup-3.0.4/mac_cleanup/config.py
+-rw-r--r--   0        0        0      652 2023-05-20 17:35:49.810403 mac_cleanup-3.0.4/mac_cleanup/console.py
+-rw-r--r--   0        0        0     7720 2023-05-20 17:35:49.810702 mac_cleanup-3.0.4/mac_cleanup/core.py
+-rw-r--r--   0        0        0     4574 2023-07-21 00:13:06.753280 mac_cleanup-3.0.4/mac_cleanup/core_modules.py
+-rw-r--r--   0        0        0    15288 2023-07-21 00:13:06.753696 mac_cleanup-3.0.4/mac_cleanup/default_modules.py
+-rw-r--r--   0        0        0     3790 2023-05-20 17:35:49.811893 mac_cleanup-3.0.4/mac_cleanup/error_handling.py
+-rw-r--r--   0        0        0     2918 2023-05-11 22:17:44.341805 mac_cleanup-3.0.4/mac_cleanup/main.py
+-rw-r--r--   0        0        0     1330 2023-07-21 00:13:06.754061 mac_cleanup-3.0.4/mac_cleanup/parser.py
+-rw-r--r--   0        0        0     3486 2023-07-21 00:13:06.754514 mac_cleanup-3.0.4/mac_cleanup/progress.py
+-rwxr-xr-x   0        0        0     3176 2023-05-20 17:35:49.812475 mac_cleanup-3.0.4/mac_cleanup/utils.py
+-rw-r--r--   0        0        0     2946 2023-07-21 00:13:06.756157 mac_cleanup-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 mac_cleanup-3.0.4/PKG-INFO
```

### Comparing `mac_cleanup-3.0.3/LICENSE` & `mac_cleanup-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/README.md` & `mac_cleanup-3.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # mac-cleanup-py
 
 [![PyPI](https://img.shields.io/pypi/v/mac_cleanup)](https://pypi.org/project/mac-cleanup/)
 [![Tests](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml)
 [![CodeQL](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml)
+[![JetBrains](https://img.shields.io/badge/Thanks-JetBrains-green.svg)](https://www.jetbrains.com)
 
 ## 🧹 Python cleanup script for macOS
 
 **mac-cleanup-py** is a powerful cleanup script for macOS.\
 This project is a rewrite of the original [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python. 
 
 
@@ -103,15 +104,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.3
+    3.0.4
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
@@ -122,7 +123,16 @@
 
 ## 🌟 Contributing
 Contributions are always welcome!\
 If you have any ideas, suggestions, or bug reports, feel free to submit an issue or open a pull request.
 
 ## 📝 License
 This project is licensed under the [Apache-2.0 License](https://github.com/mac-cleanup/mac-cleanup-py/blob/main/LICENSE).
+
+## 👏 Acknowledgements
+This project is developed using tools provided by the *JetBrains OSS Development Program*.
+
+> Find out more about their program and how they support open source [here](https://jb.gg/OpenSourceSupport).
+
+<a href="https://www.jetbrains.com">
+  <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.svg" alt="JetBrains" width="80">
+</a>
```

### Comparing `mac_cleanup-3.0.3/mac_cleanup/config.py` & `mac_cleanup-3.0.4/mac_cleanup/config.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/mac_cleanup/console.py` & `mac_cleanup-3.0.4/mac_cleanup/console.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/mac_cleanup/core.py` & `mac_cleanup-3.0.4/mac_cleanup/core.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/mac_cleanup/core_modules.py` & `mac_cleanup-3.0.4/mac_cleanup/core_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """All core modules."""
 from abc import ABC, abstractmethod
 from pathlib import Path as Path_
 from typing import Final, Optional, TypeVar, final
 
 from beartype import beartype  # pyright: ignore [reportUnknownVariableType]
 
+from mac_cleanup import args
 from mac_cleanup.progress import ProgressBar
 from mac_cleanup.utils import check_deletable, check_exists, cmd
 
 T = TypeVar("T")
 
 
 class BaseModule(ABC):
@@ -23,14 +24,17 @@
         Execute command with user prompt.
 
         :param message_: Message to be shown on prompt
         :return: Instance of self from
         :class: `BaseModule`
         """
 
+        if args.force:
+            return self
+
         # Can't be solved without typing.Self
         self.__prompt = True  # pyright: ignore [reportGeneralTypeIssues]
 
         if message_:
             # Can't be solved without typing.Self
             self.__prompt_message = message_  # pyright: ignore [reportGeneralTypeIssues]
 
@@ -69,32 +73,32 @@
     @property
     def get_command(self) -> Optional[str]:
         """Get command specified to the module."""
 
         return self.__command
 
     @abstractmethod
-    def _execute(self, **kwargs: bool) -> Optional[str]:
+    def _execute(self, ignore_errors: bool = True) -> Optional[str]:
         """
         Execute the command specified.
 
-        :param ignore_errors_: Ignore errors during execution
+        :param ignore_errors: Ignore errors during execution
         :return: Command execution results based on specified parameters
         """
 
         # Skip if there is no command
         if not self.__command:
             return
 
         # Skip on negative prompt
         if not super()._execute():
             return
 
         # Execute command
-        return cmd(command=self.__command, ignore_errors=kwargs.get("ignore_errors", True))
+        return cmd(command=self.__command, ignore_errors=ignore_errors)
 
 
 @final
 class Command(_BaseCommand):
     """Collector list unit for command execution."""
 
     __ignore_errors: bool = True
@@ -102,16 +106,23 @@
     def with_errors(self) -> "Command":
         """Return errors in exec output :return: :class:`Command`"""
 
         self.__ignore_errors = False
 
         return self
 
-    def _execute(self) -> Optional[str]:
-        return super()._execute(ignore_errors=self.__ignore_errors)
+    def _execute(self, ignore_errors: Optional[bool] = None) -> Optional[str]:
+        """
+        Execute the command specified.
+
+        :param ignore_errors: Overrides flag `ignore_errors` in class
+        :return: Command execution results based on specified parameters
+        """
+
+        return super()._execute(ignore_errors=self.__ignore_errors if ignore_errors is None else ignore_errors)
 
 
 @final
 class Path(_BaseCommand):
     """Collector list unit for cleaning paths."""
 
     __dry_run_only: bool = False
@@ -133,20 +144,20 @@
     def dry_run_only(self) -> "Path":
         """Set module to only count size in dry runs :return: :class:`Path`"""
 
         self.__dry_run_only = True
 
         return self
 
-    def _execute(self) -> Optional[str]:
+    def _execute(self, ignore_errors: bool = True) -> Optional[str]:
         """Delete specified path :return: Command execution results based on specified
         parameters.
         """
 
         if self.__dry_run_only:
             return
 
         # Skip if path is not deletable or undefined
         if not all([check_deletable(path=self.__path), check_exists(path=self.__path, expand_user=False)]):
             return
 
-        return super()._execute()  # Always ignore errors
+        return super()._execute(ignore_errors=ignore_errors)
```

### Comparing `mac_cleanup-3.0.3/mac_cleanup/default_modules.py` & `mac_cleanup-3.0.4/mac_cleanup/default_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,7 +413,29 @@
         unit.add(Command("sudo killall -HUP mDNSResponder"))
 
 
 def inactive_memory():
     with clc as unit:
         unit.message("Purging inactive memory")
         unit.add(Command("sudo purge"))
+
+
+def telegram():
+    from mac_cleanup.utils import cmd
+
+    with clc as unit:
+        unit.message("Clear old Telegram cache")
+
+        reopen_telegram = False
+
+        if cmd("ps aux | grep '[T]elegram'"):
+            reopen_telegram = True
+            unit.add(Command("killall -KILL Telegram"))
+
+        unit.add(
+            Path("~/Library/Group Containers/*.ru.keepcoder.Telegram/stable/account-*/postbox/db").with_prompt(
+                "Telegram cache will be deleted. Once reopened, cache will be rebuild smaller. Continue?"
+            )
+        )
+
+        if reopen_telegram:
+            unit.add(Command("open /Applications/Telegram.app"))
```

### Comparing `mac_cleanup-3.0.3/mac_cleanup/error_handling.py` & `mac_cleanup-3.0.4/mac_cleanup/error_handling.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/mac_cleanup/main.py` & `mac_cleanup-3.0.4/mac_cleanup/main.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/mac_cleanup/parser.py` & `mac_cleanup-3.0.4/mac_cleanup/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 @final
 @attr.s(slots=True)
 class Args:
     dry_run: bool = attr.ib(default=False)
     update: bool = attr.ib(default=False)
     configure: bool = attr.ib(default=False)
     custom_path: bool = attr.ib(default=False)
+    force: bool = attr.ib(default=False)
 
 
 parser = ArgumentParser(
     description=f"""\
     Python cleanup script for macOS
     Version: {__version__}
     https://github.com/mac-cleanup/mac-cleanup-py\
     """,
     formatter_class=RawTextHelpFormatter,
 )
 
-parser.add_argument("-n", "--dry-run", help="Dry run without deleting stuff", action="store_true")
+parser.add_argument("-n", "--dry-run", help="Run without deleting stuff", action="store_true")
 
-parser.add_argument("-u", "--update", help="Update HomeBrew on cleanup", action="store_true")
+parser.add_argument("-u", "--update", help="Update Homebrew on cleanup", action="store_true")
 
-parser.add_argument("-c", "--configure", help="Configure default and custom modules", action="store_true")
+parser.add_argument("-c", "--configure", help="Open module configuration screen", action="store_true")
 
 parser.add_argument("-p", "--custom-path", help="Specify path for custom modules", action="store_true")
 
+parser.add_argument("-f", "--force", help="Accept all warnings", action="store_true")
+
 args = Args()
 parser.parse_args(namespace=args)
 
 # args.dry_run = True  # debug
 # args.configure = True  # debug
 # args.custom_path = True  # debug
+# args.force = True  # debug
```

### Comparing `mac_cleanup-3.0.3/mac_cleanup/progress.py` & `mac_cleanup-3.0.4/mac_cleanup/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,24 +36,26 @@
         self,
         prompt_text: str,
         prompt_title: str,
         password: bool = False,
         choices: Optional[list[str]] = None,
         show_default: bool = True,
         show_choices: bool = True,
+        default: bool = True,
     ) -> bool:
         """
         Stops progress bar to show prompt to user.
 
         :param prompt_text: Text to be shown in panel
         :param prompt_title: Title of panel to be shown
         :param password: Enable password input. Defaults to False.
         :param choices: A list of valid choices. Defaults to None.
         :param show_default: Show default in prompt. Defaults to True.
         :param show_choices: Show choices in prompt. Defaults to True.
+        :param default: Default value in prompt.
         :return: True on successful prompt
         """
 
         # Stop refreshing progress bar
         self.current_progress.stop()
 
         # Print prompt to user
@@ -63,14 +65,15 @@
         answer = Confirm.ask(
             prompt="Do you want to continue?",
             console=self.current_progress.console,
             password=password,
             choices=choices,
             show_default=show_default,
             show_choices=show_choices,
+            default=default,
         )
 
         # Clear printed stuff
         self.current_progress.console.clear()
         self.current_progress.console.clear_live()
 
         # Resume refreshing progress bar
```

### Comparing `mac_cleanup-3.0.3/mac_cleanup/utils.py` & `mac_cleanup-3.0.4/mac_cleanup/utils.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.3/pyproject.toml` & `mac_cleanup-3.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mac_cleanup"
-version = "3.0.3"
+version = "3.0.4"
 description = "Python cleanup script for macOS"
 license = "Apache-2.0"
 authors = [ "Drugsosos" ]
 readme = "README.md"
 homepage = "https://github.com/mac-cleanup/mac-cleanup-py"
 repository = "https://github.com/mac-cleanup/mac-cleanup-py"
 keywords = [
@@ -26,38 +26,38 @@
 [tool.poetry.urls]
 "Documentation" = "https://github.com/mac-cleanup/mac-cleanup-py#install-automatically"
 "Issue Tracker" = "https://github.com/mac-cleanup/mac-cleanup-py/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-rich = "^13.3.5"
+rich = "^13.4.2"
 attrs = "^23.1.0"
 inquirer = "^3.1.3"
 toml = "^0.10.2"
-beartype = "^0.14.0"
+beartype = "^0.14.1"
 
 [tool.poetry.scripts]
 mac-cleanup = "mac_cleanup:main"
 
 [tool.poetry.group.test.dependencies]
-tox = "^4.5.1"
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
-pyright = "^1.1.309"
-ruff = "^0.0.269"
+tox = "^4.6.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pyright = "^1.1.317"
+ruff = "^0.0.278"
 
 [tool.poetry.group.dev.dependencies]
-commitizen = "^3.2.2"
-pre-commit = "^3.3.2"
+commitizen = "^3.5.3"
+pre-commit = "^3.3.3"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.3.0"
+black = "^23.7.0"
 isort = "^5.12.0"
-docformatter = "^1.7.1"
+docformatter = "^1.7.5"
 
 [build-system]
 requires = [ "poetry-core>=1.0.0" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -126,10 +126,10 @@
 ]
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "double"
 multiline-quotes = "double"
 
 [tool.pytest.ini_options]
-minversion = "7.3.1"
+minversion = "7.4.0"
 addopts = "--cov=mac_cleanup"
 testpaths = [ "tests" ]
```

### Comparing `mac_cleanup-3.0.3/PKG-INFO` & `mac_cleanup-3.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: mac-cleanup
-Version: 3.0.3
+Version: 3.0.4
 Summary: Python cleanup script for macOS
 Home-page: https://github.com/mac-cleanup/mac-cleanup-py
 License: Apache-2.0
 Keywords: macos,script,cleanup,cleaner
 Author: Drugsosos
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: beartype (>=0.14.0,<0.15.0)
+Requires-Dist: beartype (>=0.14.1,<0.15.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/mac-cleanup/mac-cleanup-py#install-automatically
 Project-URL: Issue Tracker, https://github.com/mac-cleanup/mac-cleanup-py/issues
 Project-URL: Repository, https://github.com/mac-cleanup/mac-cleanup-py
 Description-Content-Type: text/markdown
 
 # mac-cleanup-py
 
 [![PyPI](https://img.shields.io/pypi/v/mac_cleanup)](https://pypi.org/project/mac-cleanup/)
 [![Tests](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml)
 [![CodeQL](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml)
+[![JetBrains](https://img.shields.io/badge/Thanks-JetBrains-green.svg)](https://www.jetbrains.com)
 
 ## 🧹 Python cleanup script for macOS
 
 **mac-cleanup-py** is a powerful cleanup script for macOS.\
 This project is a rewrite of the original [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python. 
 
 
@@ -130,15 +129,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.3
+    3.0.4
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
@@ -150,7 +149,16 @@
 ## 🌟 Contributing
 Contributions are always welcome!\
 If you have any ideas, suggestions, or bug reports, feel free to submit an issue or open a pull request.
 
 ## 📝 License
 This project is licensed under the [Apache-2.0 License](https://github.com/mac-cleanup/mac-cleanup-py/blob/main/LICENSE).
 
+## 👏 Acknowledgements
+This project is developed using tools provided by the *JetBrains OSS Development Program*.
+
+> Find out more about their program and how they support open source [here](https://jb.gg/OpenSourceSupport).
+
+<a href="https://www.jetbrains.com">
+  <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.svg" alt="JetBrains" width="80">
+</a>
+
```

