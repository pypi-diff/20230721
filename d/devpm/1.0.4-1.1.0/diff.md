# Comparing `tmp/devpm-1.0.4.tar.gz` & `tmp/devpm-1.1.0.tar.gz`

## Comparing `devpm-1.0.4.tar` & `devpm-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 devpm-1.0.4/devpackage.schema.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/cli/base_command.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/cli/main.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/commands/__init__.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/commands/install.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/bash.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/code.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/context.py
--rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/git.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/log.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.4/devpm/_internal/utils/pip.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.4/LICENSE
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 devpm-1.0.4/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 devpm-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     9103 2020-02-02 00:00:00.000000 devpm-1.1.0/devpackage.schema.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/cli/base_command.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/cli/main.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/base_run.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/cr.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/install.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/lint.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/pr.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/restart.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/run.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/start.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/stop.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/test.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/version.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/bash.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/bin.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/code.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/context.py
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/git.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/log.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/pip.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 devpm-1.1.0/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 devpm-1.1.0/PKG-INFO
```

### Comparing `devpm-1.0.4/devpm/__main__.py` & `devpm-1.1.0/devpm/__main__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.4/devpm/_internal/commands/__init__.py` & `devpm-1.1.0/devpm/_internal/commands/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,41 +8,50 @@
 # Package contains all devpm commands.
 
 import importlib
 from collections import namedtuple
 from typing import Any, Dict, Optional
 
 from devpm._internal.cli.base_command import Command
+from devpm._internal.utils.context import Context
 
-CommandInfo = namedtuple("CommandInfo", "module_path, class_name, summary")
+CommandInfo = namedtuple("CommandInfo", "summary")
 
 # This dictionary does a bunch of heavy lifting for help output:
 # - Enables avoiding additional (costly) imports for presenting `--help`.
 # - The ordering matters for help display.
 #
 # Even though the module path starts with the same "devpm._internal.commands"
 # prefix, the full path makes testing easier (specifically when modifying
 # `commands_dict` in test setup / teardown).
 commands_dict: Dict[str, CommandInfo] = {
-  "install": CommandInfo(
-    "devpm._internal.commands.install",
-    "InstallCommand",
-    "Install packages.",
-  )
+    "install": CommandInfo("Install packages from devpackage.json."),
+    "pr": CommandInfo("Create a Pull Request."),
+    "cr": CommandInfo("Create a Code Review, same to pr."),
+    "run": CommandInfo("Run [NAME] script in devpackage.json."),
+    "lint": CommandInfo("Run lint script in devpackage.json."),
+    "test": CommandInfo("Run test script in devpackage.json."),
+    "start": CommandInfo("Run start script in devpackage.json."),
+    "stop": CommandInfo("Run stop script in devpackage.json."),
+    "restart": CommandInfo("Run restart script in devpackage.json."),
+    "version": CommandInfo("Bump a package version and auto-gen CHANGELOG."),
 }
 
 
-def create_command(name: str, **kwargs: Any) -> Command:
+def create_command(context: Context, name: str, **kwargs: Any) -> Command:
     """
     Create an instance of the Command class with the given name.
     """
-    module_path, class_name, summary = commands_dict[name]
+    summary, = commands_dict[name]
+    module_path = f'devpm._internal.commands.{name}'
+    class_name = f'{name.capitalize()}Command'
     module = importlib.import_module(module_path)
     command_class = getattr(module, class_name)
-    command = command_class(name=name, summary=summary, **kwargs)
+    command = command_class(context=context, name=name,
+                            summary=summary, **kwargs)
 
     return command
 
 
 def get_similar_commands(name: str) -> Optional[str]:
     """Command name auto-correct."""
     from difflib import get_close_matches
```

### Comparing `devpm-1.0.4/devpm/_internal/commands/install.py` & `devpm-1.1.0/devpm/_internal/commands/install.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,27 @@
 # This file is part of devpm.
 #
 # Copyright (c) 2023 wequick
 # This software is distributed under the MIT license.
 
 # devpm install
 
+from argparse import _SubParsersAction
 from devpm._internal.cli.base_command import Command
 from devpm._internal.utils.context import Context
 import os
 import sys
 import json
 
 
 class InstallCommand(Command):
     def run(self, args=None):
-        cwd = os.getcwd()
-        config_file = os.path.join(cwd, 'devpackage.json')
-        if not os.path.exists(config_file):
-            sys.stdout.write('devpackage.json no found.')
-            sys.exit(1)
-        sys.stdout.write('Install from %s\n' % config_file)
-        config = {}
-        with open(config_file, 'r', encoding='utf-8') as f:
-            config = json.load(f)
-        
-        context = Context()
-        context.init()
+        config = self.context.load_config()
 
+        context = self.context
         vscode_dependencies = config['vscodeDependencies']
         python_dependencies = config['pythonDependencies']
         bash_dependencies = config['bashDependencies']
         vscode_user_settings = config['vscodeUserSettings']
         git_hooks = config['gitHooks']
 
         # vscode extensions
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/bash.py` & `devpm-1.1.0/devpm/_internal/utils/bash.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 
 # Common bash cli
 
 import sys
 import subprocess
 
 class Bash:
-  def __init__(self):
-    self.is_win32 = sys.platform == 'win32'
-    if self.is_win32:
-      self.bin = r'C:\Program Files\Git\bin\bash.exe'
-    else:
-      self.bin = 'bash'
-
-  def bash_path(self, path):
-    drive, p = path.split(':')
-    return '/%s%s' % (drive.lower(), p.replace('\\', '/'))
-
-  def win32_bin_path(self, path):
-    index = path.find('/', 1)
-    drive = path[1:index].upper()
-    p = path[index:].replace('/', '\\')
-    return drive + ':' + p + '.exe'
-
-  def which(self, bin):
-    args = [self.bin, '-c', 'which ' + bin]
-    try:
-      output = subprocess.check_output(args, shell=False).decode('utf-8')
-      return self.win32_bin_path(output.strip()) if self.is_win32 else output.strip()
-    except:
-      pass
-    return None
-  
-  def check_install(self, bin, script):
-    path = self.which(bin)
-    if path:
-      return path
-    try:
-      args = [self.bin, '-c', script]
-      subprocess.check_call(args)
-    except:
-      return None
-    return self.which(bin)
+    def __init__(self):
+        self.is_win32 = sys.platform == 'win32'
+        if self.is_win32:
+            self.bin = r'C:\Program Files\Git\bin\bash.exe'
+        else:
+            self.bin = 'bash'
+
+    def bash_path(self, path):
+        drive, p = path.split(':')
+        return '/%s%s' % (drive.lower(), p.replace('\\', '/'))
+
+    def win32_bin_path(self, path):
+        index = path.find('/', 1)
+        drive = path[1:index].upper()
+        p = path[index:].replace('/', '\\')
+        return drive + ':' + p + '.exe'
+
+    def which(self, bin):
+        args = [self.bin, '-c', 'which ' + bin]
+        try:
+            output = subprocess.check_output(args, shell=False).decode('utf-8')
+            return self.win32_bin_path(output.strip()) if self.is_win32 else output.strip()
+        except:
+            pass
+        return None
+    
+    def check_install(self, bin, script):
+        path = self.which(bin)
+        if path:
+            return path
+        try:
+            args = [self.bin, '-c', script]
+            subprocess.check_call(args)
+        except:
+            return None
+        return self.which(bin)
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/code.py` & `devpm-1.1.0/devpm/_internal/utils/code.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,90 +5,70 @@
 # Copyright (c) 2023 wequick
 # This software is distributed under the MIT license.
 
 # Visual studio code cli and user settings editor
 
 import json
 import os
-import sys
-import subprocess
 from contextlib import contextmanager
+from devpm._internal.utils.bin import Bin
 
-class Code:
-  def __init__(self):
-    self.bin = None
-    self.shell = False
-    self.settings_root = None
-    self.user_settings_path = None
-
-  def init(self):
-    host_os = sys.platform
-    home = os.path.expanduser("~")
-    # https://code.visualstudio.com/docs/getstarted/settings#_settings-file-locations
-    if host_os == 'win32':
-      self.settings_root = os.getenv('APPDATA')
-    elif host_os == 'darwin':
-      self.settings_root = os.path.join(home, 'Library', 'Application Support')
-    else:
-      self.settings_root = os.path.join(home, '.config')
-    self.user_settings_path = os.path.join(self.settings_root, 'Code', 'User', 'settings.json')
-    self.shell = host_os == 'win32'
-    if os.environ.get('NODE_OPTIONS'):
-      os.environ.pop('NODE_OPTIONS')
-    try:
-      subprocess.check_call(['code', '--version'], shell=self.shell)
-      self.bin = 'code'
-    except:
-      # default path
-      default_path = None
-      if host_os == 'darwin':
-        default_path = "/Applications/Visual Studio Code.app/Contents/Resources/app/bin/code"
-      elif host_os == 'win32':
-        default_path = os.path.join(home, 'AppData', 'Local', 'Programs', 'Microsoft VS Code', 'bin', 'code')
-      if not default_path or not os.path.exists(default_path):
-        return False
-      self.bin = default_path
-      subprocess.check_call([self.bin, '--version'], shell=self.shell)
-    return True
-
-  def install_vsix(self, path, ver):
-    args = [self.bin, '--install-extension']
-    if ver == 'latest':
-      args.append('--force')
-    elif ver:
-      args.append(path + '@' + ver)
-    else:
-      args.append(path)
-    subprocess.call(args, shell=self.shell)
-
-  def check_install_vsix(self, ext, ver):
-    args = [self.bin, '--list-extensions', '--show-versions']
-    installed_ver = None
-    if ver == '':
-      ver = None
-    try:
-      output = subprocess.check_output(args, shell=self.shell).decode('utf-8')
-      for line in output.splitlines():
-        index = line.find('@')
-        if index > 0:
-          if str(line[:index]).lower() == ext:
-            installed_ver = str(line[index+1:])
-    except:
-      pass
-    finally:
-      if not installed_ver or (ver and installed_ver != ver):
-        self.install_vsix(ext, ver)
-      else:
-        print('Version %s installed.' % installed_ver)
-
-  @contextmanager
-  def open_user_settings(self):
-    f = open(self.user_settings_path, 'r')
-    s = f.read()
-    f.close()
-    settings = json.loads(s)
-    yield settings
-    s2 = json.dumps(settings, indent=4)
-    if s != s2:
-      f = open(self.user_settings_path, 'w')
-      f.write(s2)
-      f.close()
+
+class Code(Bin):
+    def __init__(self):
+        super().__init__()
+        self.name = 'code'
+        platform = 'mac' if 'darwin' == self.platform else self.platform
+        self.help_url = f'https://code.visualstudio.com/docs/setup/{platform}#_launching-from-the-command-line'
+        self.shell = self.platform == 'win32'
+        # https://code.visualstudio.com/docs/getstarted/settings#_settings-file-locations
+        if self.platform == 'win32':
+            self.settings_root = os.getenv('APPDATA')
+            self.search_paths = [os.path.join(self.home, 'AppData', 'Local', 'Programs', 'Microsoft VS Code', 'bin', 'code')]
+        elif self.platform == 'darwin':
+            self.settings_root = os.path.join(self.home, 'Library', 'Application Support')
+            self.search_paths = ['/Applications/Visual Studio Code.app/Contents/Resources/app/bin/code']
+        else:
+            self.settings_root = os.path.join(self.home, '.config')
+        self.user_settings_path = os.path.join(self.settings_root, 'Code', 'User', 'settings.json')
+        if os.environ.get('NODE_OPTIONS'):
+            os.environ.pop('NODE_OPTIONS')
+
+    def install_vsix(self, path, ver):
+        args = ['--install-extension']
+        if ver == 'latest':
+            args.append('--force')
+        elif ver:
+            args.append(path + '@' + ver)
+        else:
+            args.append(path)
+        self.call(args)
+
+    def check_install_vsix(self, ext, ver):
+        args = ['--list-extensions', '--show-versions']
+        installed_ver = None
+        if ver == '':
+            ver = None
+        output = self.run(args)
+        if output:
+            for line in output.splitlines():
+                index = line.find('@')
+                if index > 0:
+                    if str(line[:index]).lower() == ext:
+                        installed_ver = str(line[index+1:])
+        if not installed_ver or (ver and installed_ver != ver):
+            self.install_vsix(ext, ver)
+        else:
+            print('Version %s installed.' % installed_ver)
+
+    @contextmanager
+    def open_user_settings(self):
+        f = open(self.user_settings_path, 'r')
+        s = f.read()
+        f.close()
+        settings = json.loads(s)
+        yield settings
+        s2 = json.dumps(settings, indent=4)
+        if s != s2:
+            f = open(self.user_settings_path, 'w')
+            f.write(s2)
+            f.close()
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/context.py` & `devpm-1.1.0/devpm/_internal/utils/context.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,71 +3,69 @@
 # This file is part of devpm.
 #
 # Copyright (c) 2023 wequick
 # This software is distributed under the MIT license.
 
 # System context manager
 
+import json
+import os
 import subprocess
 from devpm._internal.utils.git import Git
 from devpm._internal.utils.bash import Bash
 from devpm._internal.utils.log import Log
 from devpm._internal.utils.code import Code
 from devpm._internal.utils.pip import Pip
 
 
 class Context:
-  def __init__(self):
-    self.log = Log()
-    self.code = Code()
-    self.pip = Pip()
-    self.bash = Bash()
-    self.git = Git()
-  
-  def init(self):
-    self.log.h1('Checking executable [code]')
-    if not self.code.init():
-      self.log.abort('VSCode required. see https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line')
-
-    self.log.h1('Checking executable [pip]')
-    if not self.pip.init():
-      self.log.abort('python3 required. see https://www.python.org/downloads/')
-
-    self.log.h1('Checking executable [git]')
-    if not self.git.init():
-      self.log.abort('git required. see https://git-scm.com/downloads')
-
-  def check_install_exe(self, exe, url):
-    installed_ver = None
-    args = [exe, '-h']
-    try:
-      p = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-      output, error = p.communicate()
-      if p.returncode != 1:
-        if len(output) == 0:
-          output = error.decode('utf-8')
+    def __init__(self):
+        self.cwd = os.getcwd()
+        self.log = Log()
+        self.code = Code()
+        self.pip = Pip()
+        self.bash = Bash()
+        self.git = Git()
+
+    def load_config(self) -> dict:
+        config_file = os.path.join(self.cwd, 'devpackage.json')
+        if not os.path.exists(config_file):
+            print('devpackage.json no found.')
+            exit(1)
+        config = {}
+        with open(config_file, 'r', encoding='utf-8') as file:
+            config = json.load(file)
+        return config
+
+    def check_install_exe(self, exe, url):
+        installed_ver = None
+        args = [exe, '-h']
+        try:
+            p = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            output, error = p.communicate()
+            if p.returncode != 1:
+                if len(output) == 0:
+                    output = error.decode('utf-8')
+                else:
+                    output = output.decode('utf-8')
+                if len(output) > 0:
+                    lines = output.splitlines()
+                    installed_ver = lines[0]
+        except:
+            pass
+        return installed_ver
+
+    def evaluate(self, exp, cwd):
+        if not exp or exp[0] != '$':
+            return exp
+        index = exp.find(':', 1)
+        if index > 0:
+            func = exp[1:index]
+            args = exp[index+1:]
         else:
-          output = output.decode('utf-8')
-        if len(output) > 0:
-          lines = output.splitlines()
-          installed_ver = lines[0]
-    except:
-      pass
-    return installed_ver
-
-  def evaluate(self, exp, cwd):
-    if not exp or exp[0] != '$':
-      return exp
-    index = exp.find(':', 1)
-    if index > 0:
-      func = exp[1:index]
-      args = exp[index+1:]
-    else:
-      func = exp[1:]
-      args = None
-    if func == 'pip.which':
-      return self.pip.which(args)
-    elif func == 'bash.which':
-      return self.bash.which(args)
-    elif func == 'git.install_pre_commit':
-      return self.git.install_pre_commit(args, cwd)
-    return None
+            func = exp[1:]
+            args = None
+        if func == 'pip.which':
+            return self.pip.which(args)
+        elif func == 'bash.which':
+            return self.bash.which(args)
+        return None
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/git.py` & `devpm-1.1.0/devpm/_internal/utils/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,257 +6,243 @@
 # This software is distributed under the MIT license.
 
 import os
 import stat
 import subprocess
 import sys
 from collections import namedtuple
+from devpm._internal.utils.bin import Bin
 
 GitModule = namedtuple('GitModule', field_names=[
-  'host_root_path', 'root_path', 'git_path', 'rel_path', 'is_submodule'])
+    'host_root_path', 'root_path', 'git_path', 'rel_path', 'is_submodule'])
 
 # Git管理
-class Git:
-  def __init__(self):
-    self.bin = 'git'
-    self.shell = False
-    self.cwd = None
-
-  def init(self):
-    try:
-      subprocess.check_call(['git', '--version'], self.shell)
-      return True
-    except:
-      return False
-
-  def run(self, args, cwd):
-    args.insert(0, self.bin)
-    try:
-      return subprocess.check_output(args, shell=self.shell, cwd=cwd).decode('utf-8').strip()
-    except:
-      return None
-
-  def root_path(self, cwd):
-    dir = os.path.join(cwd, '.git')
-    if os.path.exists(dir):
-      return cwd
-    dir = self.run(['rev-parse', '--show-toplevel'], cwd=cwd)
-
-  def git_path(self, cwd = None):
-    cwd = cwd or self.cwd or os.getcwd()
-    path = self.run(['rev-parse', '--git-dir'], cwd=cwd)
-    if not path:
-      return None
-    return os.path.abspath(os.path.join(cwd, path))
-  
-  def create_regexp_hook_script(self, root_path, name, pattern, tips):
-    tips_echo = ''
-    for tip in tips:
-      tips_echo += 'echo "%s"\n' % tip
-    # note: grep -P for posix, which support \d match, compat for windows.
-    grep_mode = 'P' if sys.platform == 'win32' else 'E'
-    s = '''#!/bin/bash
+class Git(Bin):
+    def __init__(self) -> None:
+        super().__init__()
+        self.name = 'git'
+        self.help_url = 'https://git-scm.com/downloads'
+
+    def root_path(self, cwd):
+        dir = os.path.join(cwd, '.git')
+        if os.path.exists(dir):
+            return cwd
+        dir = self.run(['rev-parse', '--show-toplevel'], cwd=cwd)
+
+    def git_path(self, cwd = None):
+        cwd = cwd or self.cwd or os.getcwd()
+        path = self.run(['rev-parse', '--git-dir'], cwd=cwd)
+        if not path:
+            return None
+        return os.path.abspath(os.path.join(cwd, path))
+    
+    def create_regexp_hook_script(self, root_path, name, pattern, tips):
+        tips_echo = ''
+        for tip in tips:
+            tips_echo += 'echo "%s"\n' % tip
+        # note: grep -P for posix, which support \d match, compat for windows.
+        grep_mode = 'P' if sys.platform == 'win32' else 'E'
+        s = '''#!/bin/bash
 # Auto-generated by devpm.
 
 if [ $(grep -%s '%s' "$1" | wc -l) -eq 0 ]; then
 %s
 exit 1
 fi
 ''' % (grep_mode, pattern, tips_echo)
-    script_dir = os.path.join(root_path, 'dev_modules', 'git-hooks')
-    if not os.path.exists(script_dir):
-      os.makedirs(script_dir)
-    script_file = os.path.join(script_dir, name)
-    with open(script_file, 'w', encoding='utf-8') as f:
-      f.write(s)
-    self.make_exec(script_file)
-    return 'dev_modules/git-hooks/%s' % name
-  
-  def append_hook(self, root_path, git_path, name, hook, apply_submodules):
-    t = hook['type'] if 'type' in hook else None
-    if not t:
-      return
-    available_types = ['exec', 'regexp', 'pre-commit']
-    if not t in available_types:
-      return
+        script_dir = os.path.join(root_path, 'dev_modules', 'git-hooks')
+        if not os.path.exists(script_dir):
+            os.makedirs(script_dir)
+        script_file = os.path.join(script_dir, name)
+        with open(script_file, 'w', encoding='utf-8') as f:
+            f.write(s)
+        self.make_exec(script_file)
+        return 'dev_modules/git-hooks/%s' % name
     
-    modules = self.get_modules(root_path)
-    if t == 'exec':
-      self.append_hook_script(modules, name, hook['bin'])
-    elif t == 'regexp':
-      # write git-hook file
-      if not 'pattern' in hook or not 'tips' in hook:
-        print('  pattern, tips required for regexp mode.')
-        return
-      script_bin = self.create_regexp_hook_script(root_path, name, hook['pattern'], hook['tips'])
-      return self.append_hook_script(modules, name, script_bin)
-    elif t == 'pre-commit':
-      self.install_pre_commit(modules, hook['repos'], root_path)
-
-  def make_exec(self, file):
-    st = os.stat(file)
-    mode = st.st_mode & stat.S_IEXEC
-    if mode == 0:
-      os.chmod(file, st.st_mode | stat.S_IEXEC)
-
-  def get_modules(self, host):
-    modules = []
-    git_path = os.path.join(host, '.git')
-    if not os.path.exists(git_path):
-      return modules
-    modules.append(GitModule(host, host, git_path, '.', False))
-    try:
-      output = subprocess.check_output(['git', 'submodule'], cwd=host).decode('utf-8')
-      for line in output.splitlines():
-        arr = line.strip().split(' ')
-        if len(arr) > 1:
-          sub = arr[1]
-          modules.append(GitModule(
-            host,
-            os.path.join(host, sub),
-            os.path.join(git_path, 'modules', sub),
-            os.path.relpath('.', sub).replace('\\', '/'),
-            True))
-    except:
-      pass
-    return modules
-
-  def append_hook_script(self, modules, name, script_file):
-    hook_enabled = len(script_file) > 0
-    if hook_enabled:
-      if not os.path.exists(script_file):
-        print('script file not exists: %s' % script_file)
-        return
-    self.make_exec(script_file)
-    for module in modules:
-      hook_path = os.path.join(module.git_path, 'hooks')
-      self.append_hook_script_sub(hook_enabled, module.host_root_path, hook_path, name, module.rel_path + '/' + script_file)
-
-  def append_hook_script_sub(self, hook_enabled, host, hook_path, name, bin):
-    exec = 'DEVPME=exec;$DEVPME'
-    script = '%s %s $1' % (exec, bin)
-    if os.path.exists(hook_path):
-      hook_file = os.path.join(hook_path, name)
-      new_file_content = None
-      if not os.path.exists(hook_file):
+    def append_hook(self, root_path, git_path, name, hook, apply_submodules):
+        t = hook['type'] if 'type' in hook else None
+        if not t:
+            return
+        available_types = ['exec', 'regexp', 'pre-commit']
+        if not t in available_types:
+            return
+        
+        modules = self.get_modules(root_path)
+        if t == 'exec':
+            self.append_hook_script(modules, name, hook['bin'])
+        elif t == 'regexp':
+            # write git-hook file
+            if not 'pattern' in hook or not 'tips' in hook:
+                print('    pattern, tips required for regexp mode.')
+                return
+            script_bin = self.create_regexp_hook_script(root_path, name, hook['pattern'], hook['tips'])
+            return self.append_hook_script(modules, name, script_bin)
+        elif t == 'pre-commit':
+            self.install_pre_commit(modules, hook['repos'], root_path)
+
+    def make_exec(self, file):
+        st = os.stat(file)
+        mode = st.st_mode & stat.S_IEXEC
+        if mode == 0:
+            os.chmod(file, st.st_mode | stat.S_IEXEC)
+
+    def get_modules(self, host):
+        modules = []
+        git_path = os.path.join(host, '.git')
+        if not os.path.exists(git_path):
+            return modules
+        modules.append(GitModule(host, host, git_path, '.', False))
+        output = self.run(['submodule'], cwd=host)
+        if output:
+            for line in output.splitlines():
+                arr = line.strip().split(' ')
+                if len(arr) > 1:
+                    sub = arr[1]
+                    modules.append(GitModule(
+                        host,
+                        os.path.join(host, sub),
+                        os.path.join(git_path, 'modules', sub),
+                        os.path.relpath('.', sub).replace('\\', '/'),
+                        True))
+        return modules
+
+    def append_hook_script(self, modules, name, script_file):
+        hook_enabled = len(script_file) > 0
         if hook_enabled:
-          new_file_content = '#!/bin/bash\n\n# Auto-generated by devpm.\n' + script + '\n'
-      else:
-        with open(hook_file, 'r', encoding='utf-8') as f:
-          needs_update = False
-          file_content = ''
-          found = False
-          for line in f.readlines():
-            index = line.find(exec)
-            if index < 0:
-              file_content += line
-            else:
-              found = True
-              hook_added = not '#' in line[:index]
-              if hook_added == hook_enabled:
-                if not hook_enabled or script == line.strip():
-                  break
-                needs_update = True
-                file_content += script + '\n'
-              else:
-                needs_update = True
+            if not os.path.exists(script_file):
+                print('script file not exists: %s' % script_file)
+                return
+        self.make_exec(script_file)
+        for module in modules:
+            hook_path = os.path.join(module.git_path, 'hooks')
+            self.append_hook_script_sub(hook_enabled, module.host_root_path, hook_path, name, module.rel_path + '/' + script_file)
+
+    def append_hook_script_sub(self, hook_enabled, host, hook_path, name, bin):
+        exec = 'DEVPME=exec;$DEVPME'
+        script = '%s %s $1' % (exec, bin)
+        if os.path.exists(hook_path):
+            hook_file = os.path.join(hook_path, name)
+            new_file_content = None
+            if not os.path.exists(hook_file):
                 if hook_enabled:
-                  file_content += script + '\n'
-                else:
-                  file_content += '# ' + line
-          if not found and hook_enabled:
-            needs_update = True
-            file_content += script + '\n'
-          if needs_update:
-            new_file_content = file_content
-      result = '%s installed at %s' % (name, os.path.relpath(hook_file, host))
-      if new_file_content:
-        with open(hook_file, 'w', encoding='utf-8') as f:
-          f.write(new_file_content)
-          result += ' [updated]'
-      self.make_exec(hook_file)
-      print(result)
-
-  def update_pre_commit_config_yaml(self, name, cfg_repos, cwd):
-    import yaml
-    target_pre_commit_config = os.path.join(cwd, name)
-    new_file_content = None
-    data = {}
-    if not os.path.exists(target_pre_commit_config):
-      data['repos'] = cfg_repos
-      new_file_content = yaml.dump(data)
-    else:
-      file_content = ''
-      with open(target_pre_commit_config, 'r', encoding='utf-8') as f:
-        file_content = f.read()
-        data = yaml.load(file_content, Loader=yaml.FullLoader)
-      if not 'repos' in data:
-        data['repos'] = cfg_repos
-      else:
-        for cfg_repo in cfg_repos:
-          has_repo = False
-          data['repos'] = [x for x in data['repos'] if 'repo' in x]
-          for repo in data['repos']:
-            if repo['repo'] != cfg_repo['repo']:
-              continue
-            has_repo = True
-            repo['rev'] = cfg_repo['rev']
-            if not 'hooks' in repo:
-              repo['hooks'] = cfg_repo['hooks']
+                    new_file_content = '#!/bin/bash\n\n# Auto-generated by devpm.\n' + script + '\n'
             else:
-              for cfg_hook in cfg_repo['hooks']:
-                id = cfg_hook['id']
-                found = None
-                for hook in repo['hooks']:
-                  if id == hook['id']:
-                    found = True
-                    for key in cfg_hook:
-                      hook[key] = cfg_hook[key]
-                    break
-                if not found:
-                  repo['hooks'].append(cfg_hook)
-          if not has_repo:
-            data['repos'].append(cfg_repo)
-      new_file_content = yaml.dump(data, sort_keys=False)
-      if file_content == new_file_content:
+                with open(hook_file, 'r', encoding='utf-8') as f:
+                    needs_update = False
+                    file_content = ''
+                    found = False
+                    for line in f.readlines():
+                        index = line.find(exec)
+                        if index < 0:
+                            file_content += line
+                        else:
+                            found = True
+                            hook_added = not '#' in line[:index]
+                            if hook_added == hook_enabled:
+                                if not hook_enabled or script == line.strip():
+                                    break
+                                needs_update = True
+                                file_content += script + '\n'
+                            else:
+                                needs_update = True
+                                if hook_enabled:
+                                    file_content += script + '\n'
+                                else:
+                                    file_content += '# ' + line
+                    if not found and hook_enabled:
+                        needs_update = True
+                        file_content += script + '\n'
+                    if needs_update:
+                        new_file_content = file_content
+            result = '%s installed at %s' % (name, os.path.relpath(hook_file, host))
+            if new_file_content:
+                with open(hook_file, 'w', encoding='utf-8') as f:
+                    f.write(new_file_content)
+                    result += ' [updated]'
+            self.make_exec(hook_file)
+            print(result)
+
+    def update_pre_commit_config_yaml(self, name, cfg_repos, cwd):
+        import yaml
+        target_pre_commit_config = os.path.join(cwd, name)
         new_file_content = None
-    if new_file_content:
-      print('update %s' % (name))
-      with open(target_pre_commit_config, 'w', encoding='utf-8') as f:
-        f.write(new_file_content)
-
-  def install_pre_commit(self, modules, repos, host):
-    # Create config yaml from user hook config.
-    host_yaml = '.pre-commit-config.yaml'
-    self.update_pre_commit_config_yaml(host_yaml, repos, host)
-    # Install pre-commit at host module.
-    try:
-      # Exec `pre-commit install` for submodules
-      subprocess.check_call(['pre-commit', 'install'], cwd=host)
-    except:
-      return
-    # Copy pre-commit to submodules.
-    host_pre_commit = os.path.join(host, '.git', 'hooks', 'pre-commit')
-    for module in modules:
-      if module.is_submodule:
-        sub_pre_commit = os.path.join(module.git_path, 'hooks', 'pre-commit')
-        sub_yaml = module.rel_path + '/' + host_yaml
-        self.install_pre_commit_sub(host, host_pre_commit, sub_pre_commit, host_yaml, sub_yaml)
-
-  def install_pre_commit_sub(self, host, host_pre_commit, sub_pre_commit, host_yaml, sub_yaml):
-    s = ''
-    with open(host_pre_commit, 'r') as f:
-      s = f.read()
-    s = s.replace(host_yaml, sub_yaml)
-    with open(sub_pre_commit, 'w') as f:
-      f.write(s)
-      print('pre-commit installed at %s' % os.path.relpath(sub_pre_commit, host))
+        data = {}
+        if not os.path.exists(target_pre_commit_config):
+            data['repos'] = cfg_repos
+            new_file_content = yaml.dump(data)
+        else:
+            file_content = ''
+            with open(target_pre_commit_config, 'r', encoding='utf-8') as f:
+                file_content = f.read()
+                data = yaml.load(file_content, Loader=yaml.FullLoader)
+            if not 'repos' in data:
+                data['repos'] = cfg_repos
+            else:
+                for cfg_repo in cfg_repos:
+                    has_repo = False
+                    data['repos'] = [x for x in data['repos'] if 'repo' in x]
+                    for repo in data['repos']:
+                        if repo['repo'] != cfg_repo['repo']:
+                            continue
+                        has_repo = True
+                        repo['rev'] = cfg_repo['rev']
+                        if not 'hooks' in repo:
+                            repo['hooks'] = cfg_repo['hooks']
+                        else:
+                            for cfg_hook in cfg_repo['hooks']:
+                                id = cfg_hook['id']
+                                found = None
+                                for hook in repo['hooks']:
+                                    if id == hook['id']:
+                                        found = True
+                                        for key in cfg_hook:
+                                            hook[key] = cfg_hook[key]
+                                        break
+                                if not found:
+                                    repo['hooks'].append(cfg_hook)
+                    if not has_repo:
+                        data['repos'].append(cfg_repo)
+            new_file_content = yaml.dump(data, sort_keys=False)
+            if file_content == new_file_content:
+                new_file_content = None
+        if new_file_content:
+            print('update %s' % (name))
+            with open(target_pre_commit_config, 'w', encoding='utf-8') as f:
+                f.write(new_file_content)
+
+    def install_pre_commit(self, modules, repos, host):
+        # Create config yaml from user hook config.
+        host_yaml = '.pre-commit-config.yaml'
+        self.update_pre_commit_config_yaml(host_yaml, repos, host)
+        # Install pre-commit at host module.
+        try:
+            # Exec `pre-commit install` for submodules
+            subprocess.check_call(['pre-commit', 'install'], cwd=host)
+        except:
+            return
+        # Copy pre-commit to submodules.
+        host_pre_commit = os.path.join(host, '.git', 'hooks', 'pre-commit')
+        for module in modules:
+            if module.is_submodule:
+                sub_pre_commit = os.path.join(module.git_path, 'hooks', 'pre-commit')
+                sub_yaml = module.rel_path + '/' + host_yaml
+                self.install_pre_commit_sub(host, host_pre_commit, sub_pre_commit, host_yaml, sub_yaml)
+
+    def install_pre_commit_sub(self, host, host_pre_commit, sub_pre_commit, host_yaml, sub_yaml):
+        s = ''
+        with open(host_pre_commit, 'r') as f:
+            s = f.read()
+        s = s.replace(host_yaml, sub_yaml)
+        with open(sub_pre_commit, 'w') as f:
+            f.write(s)
+            print('pre-commit installed at %s' % os.path.relpath(sub_pre_commit, host))
 
 if __name__ == '__main__':
-  # test
-  git = Git()
-  git.init()
-  # print(os.getcwd())
-  # print(git.root_path(os.getcwd()))
-  # git_path = git.git_path(os.getcwd())
-  # git.append_hook(git_path, 'commit-msg', 'scaffold/git-hooks/commit-msg', '.', True)  # scaffold/git-hooks/commit-msg
-  git.run_all_modules('hello', git.root_path(os.getcwd()))
+    # test
+    # git = Git()
+    # git.init()
+    # print(os.getcwd())
+    # print(git.root_path(os.getcwd()))
+    # git_path = git.git_path(os.getcwd())
+    # git.append_hook(git_path, 'commit-msg', 'scaffold/git-hooks/commit-msg', '.', True)    # scaffold/git-hooks/commit-msg
+    # git.run_all_modules('hello', git.root_path(os.getcwd()))
+    pass
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/log.py` & `devpm-1.1.0/devpm/_internal/utils/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 #
 # Copyright (c) 2023 wequick
 # This software is distributed under the MIT license.
 
 # Common log
 
 class Log:
-  def __init__(self):
-    pass
+    def __init__(self):
+        pass
 
-  def abort(self, msg):
-    print('')
-    print(' [!] Error: %s' % (msg))
-    print('')
-    exit(1)
-
-  def warn(self, msg):
-    print('')
-    print(' [!] Warn: %s' % (msg))
-    print('')
-
-  def info(self, msg):
-    print('')
-    print(' [!] %s' % (msg))
-    print('')
-
-  def h1(self, msg):
-    print('')
-    print('==== %s ====' % (msg))
+    def abort(self, msg):
+        print('')
+        print(' [!] Error: %s' % (msg))
+        print('')
+        exit(1)
+
+    def warn(self, msg):
+        print('')
+        print(' [!] Warn: %s' % (msg))
+        print('')
+
+    def info(self, msg):
+        print('')
+        print(' [!] %s' % (msg))
+        print('')
+
+    def h1(self, msg):
+        print('')
+        print('==== %s ====' % (msg))
```

### Comparing `devpm-1.0.4/devpm/_internal/utils/pip.py` & `devpm-1.1.0/devpm/_internal/utils/pip.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,72 +5,65 @@
 # Copyright (c) 2023 wequick
 # This software is distributed under the MIT license.
 
 # Python pip manager
 
 import os
 import sys
-import subprocess
+from devpm._internal.utils.bin import Bin
 
 
-class Pip:
-  def __init__(self):
-    self.bin = None
-    self.shell = sys.platform == 'win32'
-  
-  def init(self):
-    try:
-      output = subprocess.check_output(['pip', '--version']).decode('utf-8')
-      if 'python 2' in output:
-        return False
-      print(output.strip())
-      self.bin = 'pip'
-      return True
-    except:
-      return False
-
-  def install(self, lib, ver):
-    args = [self.bin, 'install']
-    if ver:
-      args.append('-v')
-      args.append('%s==%s' % (lib, ver))
-    else:
-      args.append(lib)
-    subprocess.call(args, shell=self.shell)
-
-  def show(self, lib):
-    info = {}
-    args = [self.bin, 'show', lib]
-    try:
-      output = subprocess.check_output(args).decode('utf-8')
-      for line in output.splitlines():
-        token = ': '
-        index = line.find(token)
-        if index > 0:
-          info[line[:index]] = line[index+len(token):]
-    except:
-      pass
-    return info
-
-  def check_install(self, lib, ver):
-    installed_ver = None
-    info = self.show(lib)
-    if 'Version' in info:
-      installed_ver = info['Version']
-    if not installed_ver or (ver and installed_ver != ver):
-      self.install(lib, ver)
-    else:
-      print('Version %s installed.' % installed_ver)
-
-  def which(self, lib):
-    info = self.show(lib)
-    bin_name = lib if sys.platform != 'win32' else lib + '.exe'
-    if 'Location' in info:
-      bin_path = info['Location']
-      bin = os.path.join(bin_path, bin_name)
-      if os.path.exists(bin):
-        return bin
-      bin_path = os.path.abspath(os.path.join(bin_path, '..', '..', 'Scripts'))
-      bin = os.path.join(bin_path, bin_name)
-      if os.path.exists(bin):
-        return bin
-    return None
+class Pip(Bin):
+    def __init__(self):
+        super().__init__()
+        self.name = 'pip'
+        self.help_url = 'https://www.python.org/downloads/'
+        self.shell = sys.platform == 'win32'
+
+    def verify_version(self, v) -> str | None:
+        if 'python 2' in v:
+            return 'requires v3+'
+    
+    def install(self, lib, ver):
+        args = ['install']
+        if ver:
+            args.append('-v')
+            args.append('%s==%s' % (lib, ver))
+        else:
+            args.append(lib)
+        self.call(args)
+
+    def show(self, lib):
+        info = {}
+        args = ['show', lib]
+        output = self.run(args)
+        if output:
+            for line in output.splitlines():
+                token = ': '
+                index = line.find(token)
+                if index > 0:
+                    info[line[:index]] = line[index+len(token):]
+        return info
+
+    def check_install(self, lib, ver):
+        installed_ver = None
+        info = self.show(lib)
+        if 'Version' in info:
+            installed_ver = info['Version']
+        if not installed_ver or (ver and installed_ver != ver):
+            self.install(lib, ver)
+        else:
+            print('Version %s installed.' % installed_ver)
+
+    def which(self, lib):
+        info = self.show(lib)
+        bin_name = lib if sys.platform != 'win32' else lib + '.exe'
+        if 'Location' in info:
+            bin_path = info['Location']
+            bin = os.path.join(bin_path, bin_name)
+            if os.path.exists(bin):
+                return bin
+            bin_path = os.path.abspath(os.path.join(bin_path, '..', '..', 'Scripts'))
+            bin = os.path.join(bin_path, bin_name)
+            if os.path.exists(bin):
+                return bin
+        return None
```

### Comparing `devpm-1.0.4/.gitignore` & `devpm-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `devpm-1.0.4/LICENSE` & `devpm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devpm-1.0.4/README.md` & `devpm-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,25 @@
 
 * devpm install - Install packages by devpackage.json in current directory which support config:
   - vscodeDependencies for vscode extensions
   - vscodeUserSettings for edit vscode user settings file
   - pythonDependencies for python modules
   - bashDependencies for custom bash script
   - gitHooks for add git hooks like `pre-commit`, `commit-msg`
+* devpm pr - Create a Pull Request
+* devpm cr - Create a Code Review, same to `devpm pr`
+* devpm run [NAME] - Run [NAME] script in devpackage.json
+* devpm lint - Run lint script in devpackage.json. Equal to `devpm run lint`
+* devpm test - Run test script in devpackage.json. Equal to `devpm run test`
+* devpm start - Run start script in devpackage.json. Equal to `devpm run start`
+* devpm stop - Run stop script in devpackage.json. Equal to `devpm run stop`
+* devpm restart - Run restart script in devpackage.json. Equal to `devpm run restart`
+* devpm version - Bump a package version and auto-gen CHANGELOG. (not yet finished)
+
+`devpm --help` for more details.
 
 ## devpackage.json
 
 ### vscodeDependencies
 Packages installed by visutal studio code.
 Key for vscode extension id, value for `version` (1).
 Version definition:
```

### Comparing `devpm-1.0.4/pyproject.toml` & `devpm-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 sources = ["src"]
 directory = "devpm"
 include = ["**/*.py", "devpackage.schema.json"]
 
 [project]
 name = "devpm"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Galen Lin", email="oolgloo.2012@gmail.com" },
 ]
 description = "Development package manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `devpm-1.0.4/PKG-INFO` & `devpm-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpm
-Version: 1.0.4
+Version: 1.1.0
 Summary: Development package manager
 Project-URL: Homepage, https://github.com/wequick/devpm
 Project-URL: Bug Tracker, https://github.com/wequick/devpm/issues
 Author-email: Galen Lin <oolgloo.2012@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,25 @@
 
 * devpm install - Install packages by devpackage.json in current directory which support config:
   - vscodeDependencies for vscode extensions
   - vscodeUserSettings for edit vscode user settings file
   - pythonDependencies for python modules
   - bashDependencies for custom bash script
   - gitHooks for add git hooks like `pre-commit`, `commit-msg`
+* devpm pr - Create a Pull Request
+* devpm cr - Create a Code Review, same to `devpm pr`
+* devpm run [NAME] - Run [NAME] script in devpackage.json
+* devpm lint - Run lint script in devpackage.json. Equal to `devpm run lint`
+* devpm test - Run test script in devpackage.json. Equal to `devpm run test`
+* devpm start - Run start script in devpackage.json. Equal to `devpm run start`
+* devpm stop - Run stop script in devpackage.json. Equal to `devpm run stop`
+* devpm restart - Run restart script in devpackage.json. Equal to `devpm run restart`
+* devpm version - Bump a package version and auto-gen CHANGELOG. (not yet finished)
+
+`devpm --help` for more details.
 
 ## devpackage.json
 
 ### vscodeDependencies
 Packages installed by visutal studio code.
 Key for vscode extension id, value for `version` (1).
 Version definition:
```

