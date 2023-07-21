# Comparing `tmp/aurornis-1.4.0.tar.gz` & `tmp/aurornis-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurornis-1.4.0.tar", max compression
+gzip compressed data, was "aurornis-1.5.0.tar", max compression
```

## Comparing `aurornis-1.4.0.tar` & `aurornis-1.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32089 2022-05-12 07:29:01.336478 aurornis-1.4.0/LICENSE.md
--rw-r--r--   0        0        0     4396 2022-05-12 07:29:01.336478 aurornis-1.4.0/README.md
--rw-r--r--   0        0        0     7929 2022-05-12 07:29:01.336478 aurornis-1.4.0/aurornis/__init__.py
--rw-r--r--   0        0        0      712 2022-05-12 07:29:01.336478 aurornis-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5070 2022-05-12 07:29:52.392831 aurornis-1.4.0/setup.py
--rw-r--r--   0        0        0     5332 2022-05-12 07:29:52.393222 aurornis-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    32089 2023-07-21 08:10:09.683750 aurornis-1.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4320 2023-07-21 08:10:09.683750 aurornis-1.5.0/README.md
+-rw-r--r--   0        0        0     6037 2023-07-21 08:10:09.683750 aurornis-1.5.0/aurornis/__init__.py
+-rw-r--r--   0        0        0     3438 2023-07-21 08:10:09.683750 aurornis-1.5.0/aurornis/model.py
+-rw-r--r--   0        0        0      735 2023-07-21 08:10:09.683750 aurornis-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5351 1970-01-01 00:00:00.000000 aurornis-1.5.0/PKG-INFO
```

### Comparing `aurornis-1.4.0/LICENSE.md` & `aurornis-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aurornis-1.4.0/README.md` & `aurornis-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Aurornis - A command line program test helper
 
 [![Coverage Status](https://coveralls.io/repos/github/Deuchnord/Aurornis/badge.svg?branch=main)](https://coveralls.io/github/Deuchnord/Aurornis?branch=main)
 
 Aurornis is a small, yet powerful library designed to help testing command line programs.
-The name is a reference to the [_aurornis xui_](https://en.wikipedia.org/wiki/Aurornis), a prehistoric bird that lived 10 millions ago.
+The name is a reference to the [_aurornis xui_](https://en.wikipedia.org/wiki/Aurornis), a prehistoric bird that lived 10 million years ago.
 
 ## Installation
 
 Aurornis is available in PyPI, so all you need is to install it with PIP:
 
 ```bash
 pip install --user aurornis
@@ -60,15 +60,15 @@
 import aurornis
 import unittest
 
 class CommandTest(unittest.TestCase):
     def test_ls_home(self):
         command_result = aurornis.run(["ls", "-l", "$HOME"], environment={"HOME": "/home/deuchnord"})
         # You can check quickly the command was successful:
-        self.assertTrue(command_result.is_successful())
+        self.assertTrue(command_result.successful)
         # Or if you expected a more specific return value:
         self.assertEqual(2, command_result.return_code) # ls returns 2 if the file does not exist
         
         # Then, check the text returned in standard output and standard error:
         self.assertEqual("""total 6
 drwxr-xr-x 1 deuchnord deuchnord 40 27 May 13:19 Desktop
 drwxr-xr-x 1 deuchnord deuchnord 40 14 Oct 18:08 Documents
@@ -89,10 +89,10 @@
 
 This option also automatically sets [the standard `NO_COLOR` environment variable](https://no-color.org). If your application shows colors, you may want to handle this environment variable to facilitate their deactivation by end users.
 
 ## FAQ/Troubleshooting
 
 ### How to handle correctly the return lines when my tests are executed on both Windows and non-Windows systems? 
 
-Since version 1.4, the `run()` function provides a way to handle it for you. To activate it, set the `normalize_carriage_return` argument to `True`.
-
-If you use a previous version, you can reproduce this behavior easily by replacing the `\r\n` characters with `\n` on both `stdout` and `stderr`.
+The `run()` function provides a way to handle it for you.
+Just set the `normalize_carriage_return` argument to `True`, and any `\r\n` will be replaced with `\n`.
+This will become the default behavior in the version 2.0.
```

### Comparing `aurornis-1.4.0/aurornis/__init__.py` & `aurornis-1.5.0/aurornis/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,47 @@
 #!/usr/bin/env python3
 
 import subprocess
+import warnings
+
 from sys import platform
 from os import environ
+from time import perf_counter_ns
 
-from datetime import datetime
+from .model import CommandResult
 
 UNIX_ESC_CHAR = "\33"
 WINDOWS_ESC_CHAR = "\u001b"
 
 
-class CommandResult:
-    """An object containing the result of a command"""
-
-    def __init__(
-        self,
-        command: [str],
-        return_code: int,
-        stdout: str,
-        stderr: str,
-        exec_time_microseconds: int,
-    ):
-        self._command = command
-        self._return_code = return_code
-        self._stdout = stdout
-        self._stderr = stderr
-        self._exec_time_microseconds = exec_time_microseconds
-
-    @property
-    def command(self) -> [str]:
-        """The command that gave this result"""
-        return self._command
-
-    @property
-    def return_code(self) -> int:
-        """The code returned by the command. Usually a number between 0 and 255 (0 meaning successful)"""
-        return self._return_code
-
-    @property
-    def stdout(self) -> str:
-        """The text that has been returned by the command in the standard output"""
-        return self._stdout
-
-    @property
-    def stderr(self) -> str:
-        """The text that has been returned by the command in the error output"""
-        return self._stderr
-
-    @property
-    def exec_time_us(self) -> int:
-        """The time of execution of the command in microseconds
-
-        This can be useful if you have big constraints and want to guaranty the time execution.
-        If you don't need a so precise value, you can use the `exec_time_ms` property instead.
-        """
-        return self._exec_time_microseconds
-
-    @property
-    def exec_time_ms(self) -> int:
-        """The time of execution of the command in milliseconds
-
-        This can be useful if you have big constraints and want to guaranty the time execution.
-        If you need a more precise value, you can use the `exec_time_us` property instead.
-        """
-        return int(self._exec_time_microseconds / 1000)
-
-    def is_successful(self) -> bool:
-        """Return true if and only if the command has been successful (i.e. its return code is zero)
-
-        This is just a facilitator for `return_code == 0`.
-        This does not verify the command has actually correctly done its job, you still need to write your own tests to check this.
-        """
-        return self.return_code == 0
-
-    def __repr__(self) -> str:
-        return (
-            "<CommandResult"
-            f' command="{" ".join(self.command)}"'
-            f" return_code={self.return_code}"
-            f' stdout="{self.stdout}"'
-            f' stderr="{self.stderr}"'
-            ">"
-        )
-
-
 def run(
     command: [str],
     environment: {str: str} = None,
     remove_colors: bool = False,
     stdin: [str] = None,
-    normalize_carriage_return: bool = False,
+    normalize_carriage_return: bool = None,
 ) -> CommandResult:
     """Execute the given command and return an object ready to check its result.
 
     >>> run(["mkdir", "-p", "/tmp/aurornis"])
     <CommandResult command="mkdir -p /tmp/aurornis" return_code=0 stdout="" stderr="">
 
     If you need to run the tests on both UNIX and Windows, it is recommended to set the `normalize_carriage_return` to True.
     This way, all the "\r\n" in standard output and standard error will be converted to "\n".
+    **This will become the default behavior in version 2.0.**
 
-    If the command returns a non-zero code, the is_successful() method returns false:
+    If the command returns a non-zero code, the successful property is false:
     >>> c = run(["python3", "-c", r"import sys; print('Oops, it didn\\'t work!', file=sys.stderr); exit(1)"], normalize_carriage_return=True)
-    >>> c.is_successful()
+    >>> c.successful
     False
 
-    You can also check the execution time of your command.
-    The object provides two values to facilitate your tests, one in milliseconds:
-    >>> assert c.exec_time_ms < 1000
-
-    and one in microseconds:
-    >>> assert c.exec_time_us < 1000000
+    You can also check the execution time of your command thanks to three properties provided by the object:
+    >>> assert c.exec_time_ms < 1000 # in millisecond
+    >>> assert c.exec_time_us < 1000000 # in microseconds
+    >>> assert c.exec_time_ns < 1000000000 # in nanoseconds
 
     You can get the text returned to the standard output and error:
     >>> c.stdout
     ''
     >>> c.stderr
     "Oops, it didn't work!\\n"
 
@@ -135,91 +63,97 @@
     It is recommended to take this environment variable in account, as it is becoming a standard.
     For more information, see https://no-color.org.
 
     If your command reads the standard input, you can give it with the `stdin` argument.
     It is a list of strings, which are joined with the end-of-line character ("\n") at execution.
     Remember that the text written in standard input does not appear in the standard output.
     >>> c = run(["python3", "-c", "who = input('Who are you? '); print(f'Hello {who}!')"], stdin=["World"], normalize_carriage_return=True)
-    >>> c.is_successful()
+    >>> c.successful
     True
     >>> c.stdout
     'Who are you? Hello World!\\n'
 
     The number of elements given in `stdin` is not verified by Aurornis, it is up to you to verify that the command
     has the expected behavior.
     >>> c = run(["python3", "-c", "who = input('Who are you? '); print(f'Hello {who}!')"], normalize_carriage_return=True)
-    >>> c.is_successful()
+    >>> c.successful
     False
     >>> c.stdout
     'Who are you? '
     >>> c.stderr
     'Traceback (most recent call last):\\n  File "<string>", line 1, in <module>\\nEOFError: EOF when reading a line\\n'
     """
+
+    def _remove_colors(from_text: str) -> str:
+        # Remove escape sequences.
+        # They have the "\e[(mode);(ten)(unit)m" form.
+        # On Windows, "\e" is replaced by the Esc character.
+        # See: https://man7.org/linux/man-pages/man5/terminal-colors.d.5.html
+
+        new_str = from_text
+
+        for escape_char in [UNIX_ESC_CHAR, WINDOWS_ESC_CHAR]:
+            for mode in range(6):
+                for ten in [3, 4]:
+                    for unit in range(0, 8):
+                        seq = f"{escape_char}[{mode};{ten}{unit}m"
+                        new_str = new_str.replace(seq, "")
+
+            new_str = new_str.replace(f"{escape_char}[0m", "")
+
+        return new_str
+
+    def _get_execution_environment(
+        user_environment: {str: str}, remove_colors: bool
+    ) -> {str: str}:
+        exec_env = {"LANG": "C"}
+
+        if platform == "win32":
+            exec_env["SystemRoot"] = environ.get("SystemRoot")
+        else:
+            exec_env["PATH"] = environ.get("PATH")
+
+        if user_environment is not None:
+            for key in user_environment:
+                exec_env[key] = user_environment[key]
+
+        if remove_colors:
+            exec_env["NO_COLOR"] = "1"
+
+        return exec_env
+
     if stdin is not None and len(stdin) > 0:
         input = "\n".join(stdin).encode("utf-8")
     else:
         input = None
 
-    start_time = datetime.now()
+    start_time = perf_counter_ns()
 
     process = subprocess.Popen(
         command,
         env=_get_execution_environment(environment, remove_colors),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
     )
     stdout, stderr = process.communicate(input)
+    exec_time = perf_counter_ns() - start_time
 
     stdout = stdout.decode()
     stderr = stderr.decode()
 
+    if normalize_carriage_return is None:
+        normalize_carriage_return = False
+        warnings.warn(
+            "The normalize_carriage_return argument of the run() function the will default to True in version 2.0. "
+            "Set it to False manually to keep the current behavior.",
+            DeprecationWarning,
+        )
+
     if normalize_carriage_return:
         stdout = stdout.replace("\r\n", "\n")
         stderr = stderr.replace("\r\n", "\n")
 
-    exec_time = (datetime.now() - start_time).microseconds
-
     if remove_colors:
         stdout, stderr = _remove_colors(stdout), _remove_colors(stderr)
 
     return CommandResult(command, process.returncode, stdout, stderr, exec_time)
-
-
-def _remove_colors(from_text: str) -> str:
-    # Remove escape sequences.
-    # They have the "\e[(mode);(ten)(unit)m" form.
-    # On Windows, "\e" is replaced by the Esc character.
-    # See: https://man7.org/linux/man-pages/man5/terminal-colors.d.5.html
-
-    new_str = from_text
-
-    for escape_char in [UNIX_ESC_CHAR, WINDOWS_ESC_CHAR]:
-        for mode in range(6):
-            for ten in [3, 4]:
-                for unit in range(0, 8):
-                    seq = f"{escape_char}[{mode};{ten}{unit}m"
-                    new_str = new_str.replace(seq, "")
-
-        new_str = new_str.replace(f"{escape_char}[0m", "")
-
-    return new_str
-
-
-def _get_execution_environment(
-    user_environment: {str: str}, remove_colors: bool
-) -> {str: str}:
-    exec_env = {"LANG": "C"}
-
-    if platform == "win32":
-        exec_env["SystemRoot"] = environ.get("SystemRoot")
-    else:
-        exec_env["PATH"] = environ.get("PATH")
-
-    if user_environment is not None:
-        for key in user_environment:
-            exec_env[key] = user_environment[key]
-
-    if remove_colors:
-        exec_env["NO_COLOR"] = "1"
-
-    return exec_env
```

### Comparing `aurornis-1.4.0/pyproject.toml` & `aurornis-1.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aurornis"
-version = "1.4.0"
+version = "1.5.0"
 description = "A command line program test helper"
 authors = ["Jérôme Deuchnord <jerome@deuchnord.fr>"]
 repository = "https://github.com/Deuchnord/Aurornis"
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 classifiers = [
@@ -12,16 +12,17 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Testing",
     "Intended Audience :: Developers",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
+deprecation = "^2.1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
+black = "^23.1.0"
 coveralls = "^3.3.1"
 coverage = "^6.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aurornis-1.4.0/setup.py` & `aurornis-1.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aurornis
+Version: 1.5.0
+Summary: A command line program test helper
+Home-page: https://github.com/Deuchnord/Aurornis
+License: AGPL-3.0-or-later
+Author: Jérôme Deuchnord
+Author-email: jerome@deuchnord.fr
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Project-URL: Repository, https://github.com/Deuchnord/Aurornis
+Description-Content-Type: text/markdown
 
-packages = \
-['aurornis']
+# Aurornis - A command line program test helper
 
-package_data = \
-{'': ['*']}
+[![Coverage Status](https://coveralls.io/repos/github/Deuchnord/Aurornis/badge.svg?branch=main)](https://coveralls.io/github/Deuchnord/Aurornis?branch=main)
 
-setup_kwargs = {
-    'name': 'aurornis',
-    'version': '1.4.0',
-    'description': 'A command line program test helper',
-    'long_description': '# Aurornis - A command line program test helper\n\n[![Coverage Status](https://coveralls.io/repos/github/Deuchnord/Aurornis/badge.svg?branch=main)](https://coveralls.io/github/Deuchnord/Aurornis?branch=main)\n\nAurornis is a small, yet powerful library designed to help testing command line programs.\nThe name is a reference to the [_aurornis xui_](https://en.wikipedia.org/wiki/Aurornis), a prehistoric bird that lived 10 millions ago.\n\n## Installation\n\nAurornis is available in PyPI, so all you need is to install it with PIP:\n\n```bash\npip install --user aurornis\n```\n\nIf you are using Pipenv or Poetry, it is recommended to install it as a development dependency:\n\n```bash\npipenv install --dev aurornis\npoetry add --dev aurornis\n```\n\n**Important note:** this library has not been tested on a production environment. For security reasons, it recommended to use it for development tests only.\nThis might evolve in the future.\n\n## Main features\n\n- One simple function: give it the command, and it will take care of all the complexity for you\n- Supports the standard input, output and error\n- Computes the execution time of the command, so you can test its global performance directly\n- Provides a way to clean the colors to make testing simpler (with native support of the [`NO_COLOR` standard](https://no-color.org/))\n- Supports Linux, macOS and Windows. Probably also works on FreeBSD.\n\n## Basic usage\n\nAurornis provides a package with only one function to run a command, that returns an object with the result of the command:\n\n```python\nimport aurornis\n\ncommand_result = aurornis.run(["ls", "-la", "/"])\n# <CommandResult command="ls -la /" return_code=0 stdout="total 68 ..." stderr="">\n```\n\nFor better security and reproducibility, the environment variables of your system are not reproduced, with the exception of `$PATH` on UNIX and `SystemRoot` on Windows.\n\nIf you need to specify environment variables (or even overwrite some of them) before you run the command, add them to the `run` function:\n\n```python\nimport aurornis\n\ncommand_result = aurornis.run(["env"], environment={"HOME": "/home/deuchnord"})\n```\n\nBy default, the `LANG` environment variable (used for internationalization) is reset to `C` (default system language, commonly English). You can change it if you want to test with another locale.\n\nOnce you get the result, all you need to do is to use your favorite unit test framework to check it returned what you expected it to return:\n\n```python\nimport aurornis\nimport unittest\n\nclass CommandTest(unittest.TestCase):\n    def test_ls_home(self):\n        command_result = aurornis.run(["ls", "-l", "$HOME"], environment={"HOME": "/home/deuchnord"})\n        # You can check quickly the command was successful:\n        self.assertTrue(command_result.is_successful())\n        # Or if you expected a more specific return value:\n        self.assertEqual(2, command_result.return_code) # ls returns 2 if the file does not exist\n        \n        # Then, check the text returned in standard output and standard error:\n        self.assertEqual("""total 6\ndrwxr-xr-x 1 deuchnord deuchnord 40 27 May 13:19 Desktop\ndrwxr-xr-x 1 deuchnord deuchnord 40 14 Oct 18:08 Documents\ndrwxr-xr-x 1 deuchnord deuchnord 40  1 Sep 16:52 Downloads\ndrwxr-xr-x 1 deuchnord deuchnord 40 29 Sep 09:11 Pictures\ndrwxr-xr-x 1 deuchnord deuchnord 40 11 Jun  2020 Music\ndrwxr-xr-x 1 deuchnord deuchnord 40 10 Nov 11:32 Videos""", command_result.stdout)\n        self.assertEqual("", command_result.stderr)\n```\n\nIf your command returns colors in your standard output or standard error, you can ask Aurornis to automatically remove them:\n\n```python\nimport aurornis\n\naurornis.run(["echo", "-e", r\'\\e[0;32mHello World!\\e[0m\'], remove_colors=True)\n```\n\nThis option also automatically sets [the standard `NO_COLOR` environment variable](https://no-color.org). If your application shows colors, you may want to handle this environment variable to facilitate their deactivation by end users.\n\n## FAQ/Troubleshooting\n\n### How to handle correctly the return lines when my tests are executed on both Windows and non-Windows systems? \n\nSince version 1.4, the `run()` function provides a way to handle it for you. To activate it, set the `normalize_carriage_return` argument to `True`.\n\nIf you use a previous version, you can reproduce this behavior easily by replacing the `\\r\\n` characters with `\\n` on both `stdout` and `stderr`.\n',
-    'author': 'Jérôme Deuchnord',
-    'author_email': 'jerome@deuchnord.fr',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Deuchnord/Aurornis',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
+Aurornis is a small, yet powerful library designed to help testing command line programs.
+The name is a reference to the [_aurornis xui_](https://en.wikipedia.org/wiki/Aurornis), a prehistoric bird that lived 10 million years ago.
 
+## Installation
+
+Aurornis is available in PyPI, so all you need is to install it with PIP:
+
+```bash
+pip install --user aurornis
+```
+
+If you are using Pipenv or Poetry, it is recommended to install it as a development dependency:
+
+```bash
+pipenv install --dev aurornis
+poetry add --dev aurornis
+```
+
+**Important note:** this library has not been tested on a production environment. For security reasons, it recommended to use it for development tests only.
+This might evolve in the future.
+
+## Main features
+
+- One simple function: give it the command, and it will take care of all the complexity for you
+- Supports the standard input, output and error
+- Computes the execution time of the command, so you can test its global performance directly
+- Provides a way to clean the colors to make testing simpler (with native support of the [`NO_COLOR` standard](https://no-color.org/))
+- Supports Linux, macOS and Windows. Probably also works on FreeBSD.
+
+## Basic usage
+
+Aurornis provides a package with only one function to run a command, that returns an object with the result of the command:
+
+```python
+import aurornis
+
+command_result = aurornis.run(["ls", "-la", "/"])
+# <CommandResult command="ls -la /" return_code=0 stdout="total 68 ..." stderr="">
+```
+
+For better security and reproducibility, the environment variables of your system are not reproduced, with the exception of `$PATH` on UNIX and `SystemRoot` on Windows.
+
+If you need to specify environment variables (or even overwrite some of them) before you run the command, add them to the `run` function:
+
+```python
+import aurornis
+
+command_result = aurornis.run(["env"], environment={"HOME": "/home/deuchnord"})
+```
+
+By default, the `LANG` environment variable (used for internationalization) is reset to `C` (default system language, commonly English). You can change it if you want to test with another locale.
+
+Once you get the result, all you need to do is to use your favorite unit test framework to check it returned what you expected it to return:
+
+```python
+import aurornis
+import unittest
+
+class CommandTest(unittest.TestCase):
+    def test_ls_home(self):
+        command_result = aurornis.run(["ls", "-l", "$HOME"], environment={"HOME": "/home/deuchnord"})
+        # You can check quickly the command was successful:
+        self.assertTrue(command_result.successful)
+        # Or if you expected a more specific return value:
+        self.assertEqual(2, command_result.return_code) # ls returns 2 if the file does not exist
+        
+        # Then, check the text returned in standard output and standard error:
+        self.assertEqual("""total 6
+drwxr-xr-x 1 deuchnord deuchnord 40 27 May 13:19 Desktop
+drwxr-xr-x 1 deuchnord deuchnord 40 14 Oct 18:08 Documents
+drwxr-xr-x 1 deuchnord deuchnord 40  1 Sep 16:52 Downloads
+drwxr-xr-x 1 deuchnord deuchnord 40 29 Sep 09:11 Pictures
+drwxr-xr-x 1 deuchnord deuchnord 40 11 Jun  2020 Music
+drwxr-xr-x 1 deuchnord deuchnord 40 10 Nov 11:32 Videos""", command_result.stdout)
+        self.assertEqual("", command_result.stderr)
+```
+
+If your command returns colors in your standard output or standard error, you can ask Aurornis to automatically remove them:
+
+```python
+import aurornis
+
+aurornis.run(["echo", "-e", r'\e[0;32mHello World!\e[0m'], remove_colors=True)
+```
+
+This option also automatically sets [the standard `NO_COLOR` environment variable](https://no-color.org). If your application shows colors, you may want to handle this environment variable to facilitate their deactivation by end users.
+
+## FAQ/Troubleshooting
+
+### How to handle correctly the return lines when my tests are executed on both Windows and non-Windows systems? 
+
+The `run()` function provides a way to handle it for you.
+Just set the `normalize_carriage_return` argument to `True`, and any `\r\n` will be replaced with `\n`.
+This will become the default behavior in the version 2.0.
 
-setup(**setup_kwargs)
```

