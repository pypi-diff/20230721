# Comparing `tmp/pip-inside-0.1.8.tar.gz` & `tmp/pip-inside-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-inside-0.1.8.tar", last modified: Thu Mar 16 09:01:16 2023, max compression
+gzip compressed data, was "pip-inside-0.1.9.tar", last modified: Sat Apr  8 23:08:36 2023, max compression
```

## Comparing `pip-inside-0.1.8.tar` & `pip-inside-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0    10174 2023-02-07 04:20:17.227923 pip-inside-0.1.8/LICENSE
--rw-r--r--   0        0        0     1653 2023-02-14 10:16:47.941486 pip-inside-0.1.8/README.md
--rw-r--r--   0        0        0      111 2023-03-01 10:01:34.351874 pip-inside-0.1.8/pip_inside/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 03:11:37.270743 pip-inside-0.1.8/pip_inside/commands/__init__.py
--rw-r--r--   0        0        0     1263 2023-02-20 02:03:19.305612 pip-inside-0.1.8/pip_inside/commands/add.py
--rw-r--r--   0        0        0     5092 2023-02-14 10:16:47.943235 pip-inside-0.1.8/pip_inside/commands/build.py
--rw-r--r--   0        0        0      839 2023-02-14 10:16:47.943379 pip-inside-0.1.8/pip_inside/commands/freeze.py
--rw-r--r--   0        0        0     5988 2023-03-01 07:17:38.028082 pip-inside-0.1.8/pip_inside/commands/init.py
--rw-r--r--   0        0        0     1606 2023-03-01 10:00:14.255252 pip-inside-0.1.8/pip_inside/commands/install.py
--rw-r--r--   0        0        0     5835 2023-02-14 10:16:47.945835 pip-inside-0.1.8/pip_inside/commands/publish.py
--rw-r--r--   0        0        0      714 2023-02-14 10:16:47.946002 pip-inside-0.1.8/pip_inside/commands/remove.py
--rw-r--r--   0        0        0     1709 2023-02-21 08:35:26.105547 pip-inside-0.1.8/pip_inside/commands/shell.py
--rw-r--r--   0        0        0      183 2023-02-14 10:16:47.946176 pip-inside-0.1.8/pip_inside/commands/show.py
--rw-r--r--   0        0        0      949 2023-03-01 10:15:20.879876 pip-inside-0.1.8/pip_inside/commands/version.py
--rw-r--r--   0        0        0     7594 2023-03-01 10:01:20.145422 pip-inside-0.1.8/pip_inside/main.py
--rw-r--r--   0        0        0        0 2023-02-01 06:44:34.894743 pip-inside-0.1.8/pip_inside/utils/__init__.py
--rw-r--r--   0        0        0     8356 2023-02-20 02:03:19.306326 pip-inside-0.1.8/pip_inside/utils/dependencies.py
--rw-r--r--   0        0        0      359 2023-02-07 06:42:08.687419 pip-inside-0.1.8/pip_inside/utils/licenses.py
--rw-r--r--   0        0        0    10174 2023-02-06 03:45:43.826519 pip-inside-0.1.8/pip_inside/utils/licenses/Apache-2.0.txt
--rw-r--r--   0        0        0    35149 2023-02-07 06:36:31.902883 pip-inside-0.1.8/pip_inside/utils/licenses/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     7652 2023-02-06 04:08:59.022825 pip-inside-0.1.8/pip_inside/utils/licenses/LGPL-3.0-or-later.txt
--rw-r--r--   0        0        0     1067 2023-02-06 07:11:54.140706 pip-inside-0.1.8/pip_inside/utils/licenses/MIT.txt
--rw-r--r--   0        0        0     9185 2023-02-07 06:40:50.811920 pip-inside-0.1.8/pip_inside/utils/licenses/MulanPSL-2.0.txt
--rw-r--r--   0        0        0      820 2023-02-21 08:21:03.065011 pip-inside-0.1.8/pip_inside/utils/misc.py
--rw-r--r--   0        0        0     4297 2023-02-14 10:16:47.947914 pip-inside-0.1.8/pip_inside/utils/packages.py
--rw-r--r--   0        0        0     6006 2023-02-14 10:16:47.948122 pip-inside-0.1.8/pip_inside/utils/pyproject.py
--rw-r--r--   0        0        0      752 2023-02-14 10:16:47.948854 pip-inside-0.1.8/pip_inside/utils/spinner.py
--rw-r--r--   0        0        0     1059 2023-02-14 10:16:47.950050 pip-inside-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 pip-inside-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-03-26 01:15:31.222687 pip-inside-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1157 2023-04-08 01:09:57.036765 pip-inside-0.1.9/README.md
+-rw-r--r--   0        0        0      111 2023-03-26 01:15:31.223064 pip-inside-0.1.9/pip_inside/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 01:15:31.223144 pip-inside-0.1.9/pip_inside/commands/__init__.py
+-rw-r--r--   0        0        0      961 2023-03-26 01:15:31.223235 pip-inside-0.1.9/pip_inside/commands/add.py
+-rw-r--r--   0        0        0     5092 2023-03-26 01:15:31.223333 pip-inside-0.1.9/pip_inside/commands/build.py
+-rw-r--r--   0        0        0      859 2023-03-26 01:15:31.223423 pip-inside-0.1.9/pip_inside/commands/freeze.py
+-rw-r--r--   0        0        0     7880 2023-04-08 01:09:57.037099 pip-inside-0.1.9/pip_inside/commands/init.py
+-rw-r--r--   0        0        0     1460 2023-04-08 01:09:57.037301 pip-inside-0.1.9/pip_inside/commands/install.py
+-rw-r--r--   0        0        0     5835 2023-03-26 01:15:31.223727 pip-inside-0.1.9/pip_inside/commands/publish.py
+-rw-r--r--   0        0        0      813 2023-03-26 01:15:31.223814 pip-inside-0.1.9/pip_inside/commands/remove.py
+-rw-r--r--   0        0        0      183 2023-03-26 01:15:31.223934 pip-inside-0.1.9/pip_inside/commands/resources/.dockerignore
+-rw-r--r--   0        0        0      526 2023-03-26 01:15:31.224014 pip-inside-0.1.9/pip_inside/commands/resources/.gitignore
+-rw-r--r--   0        0        0     1709 2023-03-26 01:15:31.224118 pip-inside-0.1.9/pip_inside/commands/shell.py
+-rw-r--r--   0        0        0      183 2023-03-26 01:15:31.224200 pip-inside-0.1.9/pip_inside/commands/show.py
+-rw-r--r--   0        0        0      433 2023-03-26 01:15:31.224280 pip-inside-0.1.9/pip_inside/commands/version.py
+-rw-r--r--   0        0        0     7187 2023-04-08 01:09:57.037506 pip-inside-0.1.9/pip_inside/main.py
+-rw-r--r--   0        0        0        0 2023-03-26 01:15:31.224448 pip-inside-0.1.9/pip_inside/utils/__init__.py
+-rw-r--r--   0        0        0     8422 2023-03-26 01:15:31.224559 pip-inside-0.1.9/pip_inside/utils/dependencies.py
+-rw-r--r--   0        0        0      480 2023-03-26 01:15:31.224652 pip-inside-0.1.9/pip_inside/utils/licenses.py
+-rw-r--r--   0        0        0    10174 2023-03-26 01:15:31.224795 pip-inside-0.1.9/pip_inside/utils/licenses/Apache-2.0.txt
+-rw-r--r--   0        0        0    35149 2023-03-26 01:15:31.225044 pip-inside-0.1.9/pip_inside/utils/licenses/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     7652 2023-03-26 01:15:31.225168 pip-inside-0.1.9/pip_inside/utils/licenses/LGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     1067 2023-03-26 01:15:31.225250 pip-inside-0.1.9/pip_inside/utils/licenses/MIT.txt
+-rw-r--r--   0        0        0     9185 2023-03-26 01:15:31.225361 pip-inside-0.1.9/pip_inside/utils/licenses/MulanPSL-2.0.txt
+-rw-r--r--   0        0        0     2198 2023-03-26 01:15:31.225455 pip-inside-0.1.9/pip_inside/utils/markers.py
+-rw-r--r--   0        0        0      463 2023-03-26 01:15:31.225537 pip-inside-0.1.9/pip_inside/utils/misc.py
+-rw-r--r--   0        0        0     4297 2023-03-26 01:15:31.225631 pip-inside-0.1.9/pip_inside/utils/packages.py
+-rw-r--r--   0        0        0     5624 2023-04-08 01:09:57.038402 pip-inside-0.1.9/pip_inside/utils/pyproject.py
+-rw-r--r--   0        0        0      752 2023-03-26 01:15:31.225846 pip-inside-0.1.9/pip_inside/utils/spinner.py
+-rw-r--r--   0        0        0      710 2023-03-26 01:15:31.225924 pip-inside-0.1.9/pip_inside/utils/versions.py
+-rw-r--r--   0        0        0     1059 2023-03-26 01:15:31.226015 pip-inside-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1895 1970-01-01 00:00:00.000000 pip-inside-0.1.9/PKG-INFO
```

### Comparing `pip-inside-0.1.8/LICENSE` & `pip-inside-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/README.md` & `pip-inside-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 # pip-inside
 
-I use `pip`, so I have `requirements.txt`, and might `requirements-dev.txt` as well.
+Like [poetry](https://python-poetry.org/), but uses `pip` to maintain dependencies.
 
-Later when I started to configure my `black`, `isort`, `pypy`..., I have `pyproject.toml`.
+Uses `flit-core` as the `build-backend`.
 
-Then I  wanted to move `requrements.txt` into `pyproject.toml`, as it's feature-rich, then I saw [poetry](https://python-poetry.org/).
 
-After used poetry for months, I started to missing `pip`, as `poetry`:
- - sometimes slow, and sometimes quite slow
- - hash mismatch, then I have to delete my entire cache, and download everything again
- - when you have huge dependencies like `torch` (~2 GB), too bad to install a general version, then a working version later in `toe` plugin
+**CONVENSIONS**:
 
-So this `pip-inside` comes out. It's just `flit-core` with `pip` as the dependency installer.
-
-
-**NOTICES**:
-
-Only supports:
  - dynamic `version` (`__version__ = 'your version'` in {root_module}/__init__.py)
  - non-dynamic `description` (in `pyproject.toml`)
  - no `src` folder in project root
  - virtualenv folder named `.venv` in project root
  - not checking hashes
 
 
@@ -33,23 +23,26 @@
 
 ## commands
 
  - pip-inside
  - pi
 
 ```shell
-pi
+> pi
 Usage: pi [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -V, --version  show version of this tool
   --help         Show this message and exit.
 
 Commands:
   add      Add a package as project dependency
   build    Build the wheel and sdist
+  freeze   Freeze dependencies into 'pi.lock'
   init     Init project in current directory
   install  Install project dependencies by groups
   publish  Publish the wheel and sdist to remote repository
   remove   Remove a package from project dependencies
+  shell    Ensure '.venv' virtualenv, and new shell into it
+  show     Show dependency tree
   version  Show version of current project
 ```
```

### Comparing `pip-inside-0.1.8/pip_inside/commands/add.py` & `pip-inside-0.1.9/pip_inside/commands/install.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 import os
 import shutil
 import subprocess
 import sys
-from typing import Optional
+from typing import List
 
 import click
-from InquirerPy import inquirer
+import tomlkit
 
-from pip_inside.utils import misc
 from pip_inside.utils.pyproject import PyProject
 
 
-def handle_add(name: str, group: Optional[str]):
+def handle_install(groups: List[str]):
+    _install_from_pi_lock(groups) or _install_from_pyproject_toml(groups)
+
+
+def _install_from_pi_lock(groups: List[str]):
+    if not os.path.exists('pi.lock'):
+        return
+
+    with open('pi.lock', 'r') as f:
+        data = tomlkit.load(f)
+
+    if '_all_' in groups:
+        for group, deps in data.items():
+            _install_group(group, deps)
+    else:
+        for group in groups:
+            _install_group(group, data.get(group, []))
+
+
+def _install_from_pyproject_toml(groups: List[str]):
+    pyproject = PyProject.from_toml()
+
+    if '_all_' in groups:
+        for group, deps in pyproject.get_dependencies_for_install().items():
+            _install_group(group, deps)
+
+    else:
+        for group in groups:
+            deps = pyproject.get_for_install(group)
+            _install_group(group, deps)
+
+
+def _install_group(group: str, dependencies: list):
+    if dependencies is None or len(dependencies) == 0:
+        click.secho(f"Group: {group}, nothing to install", fg='cyan')
+        return
+
+    click.secho(f"Group: {group}", fg='cyan')
     try:
-        if os.environ.get('VIRTUAL_ENV') is None:
-            proceed = inquirer.confirm(message='Not in virutal env, sure to proceed?', default=False).execute()
-            if not proceed:
-                return
-        pyproject = PyProject.from_toml()
-        name = misc.norm_name(name)
-        if pyproject.find_dependency(name, 'main'):
-            click.secho("Skip, already installed as main dependency")
-            return
-        name_installed = pyproject.find_dependency(name, group)
-        if name_installed:
-            if name_installed == name:
-                click.secho("Skip, already installed")
-            else:
-                pyproject.remove_dependency(name_installed, group)
-        cmd = [shutil.which('python'), '-m', 'pip', 'install', name]
-        if subprocess.run(cmd, stderr=sys.stderr, stdout=sys.stdout).returncode == 0:
-            pyproject.add_dependency(name, group)
-            pyproject.flush()
+        cmd = [shutil.which('python'), '-m', 'pip', 'install', *dependencies]
+        subprocess.run(cmd, stderr=sys.stderr, stdout=sys.stdout)
     except subprocess.CalledProcessError:
         pass
```

### Comparing `pip-inside-0.1.8/pip_inside/commands/build.py` & `pip-inside-0.1.9/pip_inside/commands/build.py`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/commands/freeze.py` & `pip-inside-0.1.9/pip_inside/commands/freeze.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from pip_inside.utils.dependencies import Dependencies, Package
 
 
 def handle_freeze():
     dependencies = Dependencies().load_dependencies()
     requirements = collections.defaultdict(list)
     for child in dependencies._root.children:
-        requirements[child.group].append(f"{child.name}=={child.version}")
+        requirements[child.group].append(f"{child.name}=={child.version_installed}")
         for group, dep in _find_installed_child(child):
             requirements[group or child.group].append(dep)
     with open('pi.lock', 'w') as f:
         tomlkit.dump(requirements, f)
     click.secho(f"Generated pi.lock", fg='bright_cyan')
 
 
 def _find_installed_child(pkg: Package):
     for child in pkg.children:
-        yield child.group, f"{child.name}=={child.version}"
+        yield child.group, f"{child.name}=={child.version_installed}"
         for group, dep in _find_installed_child(child):
             yield group or child.group, dep
```

### Comparing `pip-inside-0.1.8/pip_inside/commands/init.py` & `pip-inside-0.1.9/pip_inside/commands/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
-import pathlib
+import shutil
 import subprocess
 from datetime import date
+from pathlib import Path
 from types import SimpleNamespace
 
 import click
 import tomlkit
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 
 from pip_inside import Aborted
-from pip_inside.utils import licenses, misc, packages
+from pip_inside.utils import licenses, misc, packages, versions
 
 
 def handle_init():
     click.echo(f"Initializing project in {os.getcwd()}")
     check_pyproject_toml()
     meta = collect_metadata()
     toml = build_toml(meta)
@@ -23,26 +24,34 @@
     proceed = inquirer.confirm(message="Proceed?", default=True).execute()
     if not proceed:
         return
 
     write_toml(toml)
     write_readme(meta)
     write_license(meta)
+    write_resource('.gitignore')
+    write_resource('.dockerignore')
     write_root_module_with_version(meta)
 
 
 def check_pyproject_toml():
     if not os.path.exists('pyproject.toml'):
         return
 
     try:
         with open('pyproject.toml', 'r') as f:
             data = tomlkit.load(f)
-        if 'build-system' in data:
-            raise Aborted(f"Skip, 'pyproject.toml' file with 'build-system' already exists")
+        build_system = data.get('build_system')
+        if build_system is not None:
+            if build_system.get('build-backend') == 'flit_core.buildapi':
+                raise Aborted(f"Skip, 'pyproject.toml' file already exists")
+            else:
+                raise Aborted(f"Skip, 'pyproject.toml' file already exists with unsupported 'build-system', only supports 'flit_core.buildapi'")
+    except Aborted as e:
+        raise e
     except Exception as e:
         raise Aborted(f"Skip, 'pyproject.toml' already exists, and failed to load: {e}")
 
 
 def collect_metadata():
     defaults = get_defaults()
     name = inquirer.text(message="Name:", default=defaults.name, mandatory=True).execute()
@@ -153,20 +162,75 @@
         f.write(f"# {meta.name}\n\n {meta.description}\n")
         click.secho(f"Added 'README.md'", fg='bright_cyan')
 
 
 def write_license(meta):
     if os.path.exists('LICENSE') or meta.license == 'skip':
         return
-    licenses_dir = pathlib.Path(__file__).parent / 'licenses'
-    with (licenses_dir / f"{meta.license}.txt").open() as f_in, open('LICENSE', 'w') as f_out:
+    license_file = licenses.get_file(meta.license)
+    with license_file.open() as f_in, open('LICENSE', 'w') as f_out:
         year = date.today().year
         f_out.write(f_in.read().format(year=year, author=meta.author))
         click.secho(f"Added 'LICENSE'", fg='bright_cyan')
 
 
+def write_resource(filename: str):
+    target = Path(filename)
+    if target.exists():
+        return
+    src = Path(__file__).parent / 'resources' / filename
+    shutil.copyfile(src, target)
+    click.secho(f"Added '{filename}'", fg='bright_cyan')
+
+
 def write_root_module_with_version(meta):
+
+    version_line = f"__version__ = '{meta.version}'\n"
     module_name = misc.norm_module(meta.name)
     os.makedirs(module_name, exist_ok=True)
-    with open(f"{module_name}/__init__.py", 'w+') as f:
-        f.write(f"__version__ = '{meta.version}'")
+    path = f"{module_name}/__init__.py"
+
+    is_exists = os.path.exists(path)
+    if is_exists:
+        with open(path, 'a+') as f:
+            f.seek(0)
+            lines = f.readlines()
+            add_version_line = True
+            for i, line in enumerate(lines):
+                m = versions.P.search(line)
+                if m is None:
+                    continue
+                add_version_line = False
+                version = m.groups()[0]
+                if version == meta.version:
+                    return
+                lines[i] = version_line
+
+            f.truncate(0)
+            if add_version_line:
+                i = _add_version_position(lines)
+                lines.insert(i, version_line)
+            for line in lines:
+                f.write(line)
+        click.secho(f"Updated '{module_name}/__init__.py'", fg='bright_cyan')
+
+    else:
+        with open(path, 'w') as f:
+            f.write(version_line)
         click.secho(f"Added '{module_name}/__init__.py'", fg='bright_cyan')
+
+
+def _add_version_position(lines: list):
+    saw_contents = False
+    for i, line in enumerate(lines):
+        line = line.strip()
+        if not line:
+            if not saw_contents:
+                continue
+            else:
+                return i
+
+        saw_contents = True
+        if line.startswith('#'):
+            continue
+        return i
+    return len(lines)
```

### Comparing `pip-inside-0.1.8/pip_inside/commands/publish.py` & `pip-inside-0.1.9/pip_inside/commands/publish.py`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/commands/remove.py` & `pip-inside-0.1.9/pip_inside/commands/remove.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import shutil
 import subprocess
 import sys
 
 import click
+from pkg_resources import Requirement
 
 from pip_inside.utils.dependencies import Dependencies
 from pip_inside.utils.pyproject import PyProject
 
 
-def handle_remove(name, group):
+def handle_remove(name: str, group):
     try:
         pyproject = PyProject.from_toml()
-        if pyproject.remove_dependency(name, group):
+        require = Requirement(name)
+        if pyproject.remove_dependency(require, group):
             pyproject.flush()
-            deps = Dependencies().get_unused_dependencies_for(name)
-            cmd = [shutil.which('python'), '-m', 'pip', 'uninstall', name, *deps, '-y']
+            deps = Dependencies().get_unused_dependencies_for(require)
+            cmd = [shutil.which('python'), '-m', 'pip', 'uninstall', require.key, *deps, '-y']
             subprocess.run(cmd, stderr=sys.stderr, stdout=sys.stdout)
         else:
-            click.secho(f"Package: [{name}] not found in group: [{group}]", fg='yellow')
+            click.secho(f"Package: [{require.key}] not found in group: [{group}]", fg='yellow')
     except subprocess.CalledProcessError:
         pass
```

### Comparing `pip-inside-0.1.8/pip_inside/commands/shell.py` & `pip-inside-0.1.9/pip_inside/commands/shell.py`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/main.py` & `pip-inside-0.1.9/pip_inside/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,38 +34,28 @@
             import traceback
             click.secho(traceback.format_exc(), fg='red')
 
 
 @cli.command()
 @click.argument('name', required=False, type=str)
 @click.option('-G', '--group', default='main', help='dependency group')
-@click.option('-i', 'interactive', is_flag=True, default=False, help="interactive mode")
 @click.option('-v', 'v', is_flag=True, default=False, help="verbovse")
-def add(name, group, interactive: bool, v: bool):
+def add(name, group, v: bool):
     """Add a package as project dependency"""
     try:
         from .commands.add import handle_add
-        from .utils.misc import ver_has_spec
         from .utils.packages import prompt_a_package
         click.secho(f"[python] {shutil.which('python')}", fg='cyan')
         if name:
-            if interactive and ver_has_spec(name) :
-                interactive = False
-                click.secho('Off interactive mode, found version specifier in package name', fg='yellow')
-        else:
-            interactive = True
-
-        if not interactive:
             handle_add(name, group)
-            return
-
-        name = prompt_a_package()
-        while name is not None:
-            handle_add(name, group)
-            name = prompt_a_package(True)
+        else:
+            name = prompt_a_package()
+            while name is not None:
+                handle_add(name, group)
+                name = prompt_a_package(True)
     except Aborted as e:
         click.secho(e, fg='yellow')
     except Exception as e:
         click.secho(e, fg='red')
         if v:
             import traceback
             click.secho(traceback.format_exc(), fg='red')
@@ -90,27 +80,27 @@
         if v:
             import traceback
             click.secho(traceback.format_exc(), fg='red')
 
 
 @cli.command()
 @click.option('-G', '--groups', multiple=True, default=['main'], show_default=True, help='dependency groups')
-@click.option('-A', '--all', is_flag=True, default=False, help="verbovse")
+@click.option('-A', '--all', is_flag=True, default=False, help="all groups")
 @click.option('-v', 'v', is_flag=True, default=False, help="verbovse")
 def install(groups: List[str], all: bool, v: bool):
     """Install project dependencies by groups"""
     try:
         from .commands.install import handle_install
         click.secho(f"[python] {shutil.which('python')}", fg='cyan')
         if len(groups) == 1:
             groups = groups[0].split(',')
         elif len(groups) == 0:
             groups = ['main']
         if all:
-            groups = ['all']
+            groups = ['_all_']
         handle_install(groups)
     except Aborted as e:
         click.secho(e, fg='yellow')
     except Exception as e:
         click.secho(e, fg='red')
         if v:
             import traceback
```

### Comparing `pip-inside-0.1.8/pip_inside/utils/dependencies.py` & `pip-inside-0.1.9/pip_inside/utils/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import os
 import shutil
 import site
 from pathlib import Path
 from typing import Dict, List, Optional, Set
 
 import click
-import pkg_resources
+from pkg_resources import Distribution, Requirement, find_distributions
 
 from .misc import norm_name
 from .pyproject import PyProject
 
 ROOT = 'root'
 DEPENDENCIES_COMMON = [
     'pip', 'certifi', 'setuptools', 'ipython', 'poetry',
     'requests', 'urllib3', 'wheel', 'tomlkit', 'pip-inside',
 ]
 COLOR_MAIN = 'blue'
-COLOR_OPTIONAL = 'magenta'
+COLOR_OPTIONAL = 'green'
 COLOR_SUBS = 'white'
 
 
 def get_name_fg_by_group(group):
     if group is None:
         return COLOR_SUBS
     return COLOR_MAIN if group == 'main' else COLOR_OPTIONAL
@@ -37,40 +37,40 @@
     return next((env_root / 'lib').glob('python*')) / 'site-packages'
 
 
 class Distributions:
     def __init__(self) -> None:
         self._distributions = self._find_distributions()
 
-    def _find_distributions(self) -> Dict[str, pkg_resources.Distribution]:
-        distributions: Dict[str, pkg_resources.Distribution] = {}
+    def _find_distributions(self) -> Dict[str, Distribution]:
+        distributions: Dict[str, Distribution] = {}
         site_package_path = get_site_package_path()
-        for dist in pkg_resources.find_distributions(site_package_path):
-            name = norm_name(dist.key)
-            distributions[name] = dist
+        for dist in find_distributions(site_package_path):
+            distributions[dist.key] = dist
         return distributions
 
-    def get_all(self) -> List[pkg_resources.Distribution]:
+    def get_all(self) -> List[Distribution]:
         return list(self._distributions.values())
 
-    def get(self, name) -> pkg_resources.Distribution:
+    def get(self, name) -> Distribution:
         return self._distributions.get(norm_name(name))
 
 
 class TreeEntry:
     def __init__(self, prefix, package: 'Package') -> None:
         self.prefix = prefix
         self.package = package
 
     def __str__(self):
         return f"{self.prefix} {self.package}"
 
     def echo(self):
         name = click.style(self.package.name, fg=get_name_fg_by_group(self.package.group))
-        click.echo(f"{self.prefix} {name} [required: {self.package.specs or '*'}, installed: {self.package.version}]")
+        installed = f"installed: {self.package.version}" if self.package.version else click.style('[not installed]', fg='yellow')
+        click.echo(f"{self.prefix} {name} [required: {self.package.specs or '*'}, {installed}]")
 
 
 class Package:
 
     def __init__(self,name: str, *, specs: str = None, group: str = None, version: str = None, parent: 'Package' = None) -> None:
         self.name = name
         self.specs = specs
@@ -86,15 +86,16 @@
             paths.append(parent.name)
             parent = parent.parent
         paths.reverse()
         return paths
 
     def echo(self):
         name = click.style(self.name, fg=get_name_fg_by_group(self.group))
-        click.echo(f"{name} [required: {self.specs or '*'}, installed: {self.version}]")
+        installed = f"installed: {self.version}" if self.version else click.style('[not installed]', fg='yellow')
+        click.echo(f"{name} [required: {self.specs or '*'}, {installed}]")
 
     def tree_list(self, skip='│', branch='├', last='└', hyphen='─', prefix='') -> str:
         n_children = len(self.children)
         for i, child in enumerate(self.children):
             if i < n_children - 1:
                 next_prefix = ''.join([prefix, skip, '   '])
                 fork = branch
@@ -115,26 +116,25 @@
         return self.__str__()
 
 
 class Dependencies:
     def __init__(self) -> None:
         self._distributions = Distributions()
         self._pyproject = PyProject.from_toml()
-        self._direct_dependencies = {
-            r.name: (str(r.specifier), group)
-            for r, group in self._pyproject.get_dependencies_with_group().items()
-        }
         self._cyclic_dendencies = []
         self._root: Package = Package(ROOT)
         self._root_non_dep: Package = Package(ROOT)
+        self._direct_dependencies = {
+            r.key: Package(r.key, specs=str(r.specifier), group=group, parent=self._root)
+            for r, group in self._pyproject.get_dependencies_with_group().items()
+        }
 
     def load_dependencies(self):
         self._root.children.clear()
-        for name, (specs, group) in self._direct_dependencies.items():
-            child = Package(name, specs=specs, group=group, parent=self._root)
+        for child in self._direct_dependencies.values():
             self._root.children.append(child)
             self._load_children(child)
         return self
 
     def load_non_dependencies(self):
         if len(self._root.children) == 0:
             self.load_dependencies()
@@ -154,15 +154,14 @@
             self._load_children(child, exclusion, parents)
         self._root_non_dep.children = [child for child in self._root_non_dep.children if parents.get(child.name) == {ROOT}]
         return self
 
     def _load_children(self, pkg: Package, exclusion: Optional[Set[str]] = None, parents: Optional[Dict[str, Set[str]]] = None):
         dist = self._distributions.get(pkg.name)
         if dist is None:
-            pkg.version = '[not installed]'
             return
         pkg.version = dist.version
         for r in dist.requires():
             name, specs_r = norm_name(r.name), str(r.specifier)
             if exclusion is not None and name in exclusion:
                 continue
             ref_path = pkg.get_ref_path()
@@ -211,12 +210,12 @@
         key_subs = click.style(COLOR_SUBS, fg=COLOR_SUBS)
         click.secho(f"Dependencies: (main: {key_main}, optional: {key_optional}, sub-dependencies: {key_subs})")
         for child in root.children:
             child.echo()
             for entry in child.tree_list():
                 entry.echo()
 
-    def get_unused_dependencies_for(self, name: str) -> List[str]:
-        name = norm_name(name)
+    def get_unused_dependencies_for(self, require: Requirement) -> List[str]:
+        name = require.key
         other_in_use = set(self._get_all_project_dependencies(exclusions=[name]))
         children = {norm_name(r.name) for r in self._distributions.get(name).requires()}
         return list(children - other_in_use)
```

### Comparing `pip-inside-0.1.8/pip_inside/utils/licenses/Apache-2.0.txt` & `pip-inside-0.1.9/pip_inside/utils/licenses/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/licenses/GPL-3.0-or-later.txt` & `pip-inside-0.1.9/pip_inside/utils/licenses/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/licenses/LGPL-3.0-or-later.txt` & `pip-inside-0.1.9/pip_inside/utils/licenses/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/licenses/MIT.txt` & `pip-inside-0.1.9/pip_inside/utils/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/licenses/MulanPSL-2.0.txt` & `pip-inside-0.1.9/pip_inside/utils/licenses/MulanPSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/packages.py` & `pip-inside-0.1.9/pip_inside/utils/packages.py`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pip_inside/utils/pyproject.py` & `pip-inside-0.1.9/pip_inside/utils/pyproject.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-import itertools
 import os
-from types import SimpleNamespace
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import tomlkit
-from packaging.requirements import Requirement
+from pkg_resources import Requirement
 
 from pip_inside import Aborted
+from pip_inside.utils import markers
 
-from .misc import get_package_name, norm_module
+from .misc import norm_module
 
 
 class PyProject:
     def __init__(self, path='pyproject.toml') -> None:
         self.path = path
         self._meta = {}
+        self._dependencies: Dict[str, List[Requirement]] = {}
 
     @classmethod
     def from_toml(cls, path='pyproject.toml'):
         pyproject = cls(path)
         pyproject.load()
         return pyproject
 
-    def load(self):
-        if not os.path.exists(self.path):
-            raise ValueError(f"'{self.path}' not found")
-
-        with open(self.path, 'r') as f:
-            self._meta = tomlkit.load(f)
-        self.validate()
-
-    def flush(self):
-        with open(self.path, "w") as f:
-            tomlkit.dump(self._meta, f)
+    def _load_dependencies(self):
+        key_main = 'project.dependencies'
+        key_optionals = 'project.optional-dependencies'
+        self._dependencies['main'] = [Requirement(dep) for dep in self.get(key_main, default=[])]
+        for key, deps in self.get(key_optionals, default={}).items():
+            self._dependencies[key] = [Requirement(dep) for dep in deps]
+
+    def _dump_dependencies(self):
+        for key, requires in self._dependencies.items():
+            if key == 'main':
+                self.set('project.dependencies', [str(r) for r in requires])
+            else:
+                self.set(f"project.optional-dependencies.{key}", [str(r) for r in requires])
 
     def validate(self):
         def check_exists(attr: str, msg: Optional[str] = None):
             if self.get(attr) is None:
                 msg = f", {msg}" if msg else ''
                 raise Aborted(f"Unsupported pyproject.toml, expecting: '{attr}' {msg}")
         def check_not_exists(attr: str, msg: Optional[str] = None):
@@ -53,14 +55,28 @@
         check_exists('project.name')
         check_not_exists('project.version', f"should be defined in {norm_module(self.get('project.name'))}/__init__.py")
         check_equals('project.dynamic', ['version'])
         check_exists('project.requires-python')
         check_exists('build-system')
         check_equals('build-system.build-backend', 'flit_core.buildapi', 'only supports `flit_core` backend')
 
+    def load(self):
+        if not os.path.exists(self.path):
+            raise ValueError(f"'{self.path}' not found")
+
+        with open(self.path, 'r') as f:
+            self._meta = tomlkit.load(f)
+        self.validate()
+        self._load_dependencies()
+
+    def flush(self):
+        self._dump_dependencies()
+        with open(self.path, "w") as f:
+            tomlkit.dump(self._meta, f)
+
     def update(self, key: str, value: Union[str, int, float, dict, list]):
         data = self._meta
         attrs = key.split('.')
         for attr in attrs[:-1]:
             data = data.setdefault(attr, {})
         data[attrs[-1]] = value
 
@@ -87,80 +103,51 @@
             else:
                 data = data.get(attr)
                 if data is None:
                     return False
         data[attrs[-1]] = value
         return True
 
-    def add_dependency(self, name: str, group: str = 'main'):
-        if group == 'main':
-            key = 'project.dependencies'
-        else:
-            key = f"project.optional-dependencies.{group}"
-        dependencies = self.get(key, create_if_missing=True, default=[])
-        if name not in dependencies:
-            dependencies.append(name)
-
-    def remove_dependency(self, name: str, group: str = 'main'):
-        if group == 'main':
-            key = 'project.dependencies'
-        else:
-            key = f"project.optional-dependencies.{group}"
-        dependencies = self.get(key, create_if_missing=False)
-        if dependencies is None or len(dependencies) == 0:
+    def add_dependency(self, require: Requirement, group: str = 'main'):
+        do_add = True
+        dependencies = self._dependencies.get(group)
+        if dependencies:
+            for i, dep in enumerate(dependencies):
+                if require.key != dep.key:
+                    continue
+                if str(require) == str(dep):
+                    return False
+                do_add = False
+                dependencies[i] = require
+
+        if do_add:
+            dependencies.append(require)
+        return True
+
+    def remove_dependency(self, require: Requirement, group: str = 'main'):
+        dependencies = self._dependencies.get(group)
+        if not dependencies:
             return False
-        package_name = get_package_name(name)
-        remove_list = [dep for dep in dependencies if get_package_name(dep) == package_name]
-        if len(remove_list) == 0:
+        deps = [dep for dep in dependencies if dep.key != require.key]
+        if len(deps) == len(dependencies):
             return False
-        for dep in remove_list:
-            try:
-                dependencies.remove(dep)
-            except ValueError:
-                pass
+        self._dependencies[group] = deps
         return True
 
-    def find_dependency(self, name: str, group: str = 'main'):
-        package_name = get_package_name(name)
-        for dep in self.get_dependencies(group):
-            pkg_name = get_package_name(dep)
-            if pkg_name == package_name:
-                return dep
-        return None
-
-    @staticmethod
-    def _is_in_dependencies(name: str, dependencies: List[str]) -> bool:
-        if name in dependencies:
-            return True
-        if name in set([get_package_name(dep) for dep in dependencies]):
-            return True
-        return False
-
-    def get_dependencies(self, group: str = 'main'):
-        if group == 'all':
-            key_main = 'project.dependencies'
-            key_optionals = 'project.optional-dependencies'
-            deps_main = self.get(key_main, default=[])
-            deps_optionals = list(itertools.chain(*self.get(key_optionals, default={}).values()))
-            return deps_main + deps_optionals
-
-        if group == 'main':
-            return self.get('project.dependencies', default=[])
-        else:
-            return self.get(f"project.optional-dependencies.{group}", default=[])
-
-    def get_dependencies_with_group(self):
-        dependencies = {}
-        for dep in self.get('project.dependencies', default=[]):
-            dependencies[Requirement(dep)] = 'main'
-
-        for group, deps in self.get('project.optional-dependencies', default={}).items():
+    def get_for_install(self, group: str = 'main'):
+        deps = self._dependencies.get(group)
+        if deps is None:
+            return None
+        return markers.filter_requirements(deps)
+
+    def get_dependencies_for_install(self) -> Dict[str, List[str]]:
+        return {
+            group: markers.filter_requirements(deps)
+            for group, deps in self._dependencies.items()
+        }
+
+    def get_dependencies_with_group(self) -> Dict[Requirement, str]:
+        dependencies: Dict[Requirement, str] = {}
+        for group, deps in self._dependencies.items():
             for dep in deps:
-                dependencies[Requirement(dep)] = group
+                dependencies[dep] = group
         return dependencies
-
-    @staticmethod
-    def get_template():
-        return SimpleNamespace(
-            name=os.path.basename(os.getcwd()),
-            description=''
-        )
```

### Comparing `pip-inside-0.1.8/pip_inside/utils/spinner.py` & `pip-inside-0.1.9/pip_inside/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/pyproject.toml` & `pip-inside-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip-inside-0.1.8/PKG-INFO` & `pip-inside-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-inside
-Version: 0.1.8
+Version: 0.1.9
 Summary: Like poetry, but it's pip
 Home-page: https://github.com/orctom/pip-inside
 License: Apache-2.0
 Author: orctom
 Author-email: orctom <orctom@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -19,31 +19,21 @@
 Requires-Dist: pexpect
 Requires-Dist: packaging
 Project-URL: homepage, https://github.com/orctom/pip-inside
 Project-URL: repository, https://github.com/orctom/pip-inside
 
 # pip-inside
 
-I use `pip`, so I have `requirements.txt`, and might `requirements-dev.txt` as well.
+Like [poetry](https://python-poetry.org/), but uses `pip` to maintain dependencies.
 
-Later when I started to configure my `black`, `isort`, `pypy`..., I have `pyproject.toml`.
+Uses `flit-core` as the `build-backend`.
 
-Then I  wanted to move `requrements.txt` into `pyproject.toml`, as it's feature-rich, then I saw [poetry](https://python-poetry.org/).
 
-After used poetry for months, I started to missing `pip`, as `poetry`:
- - sometimes slow, and sometimes quite slow
- - hash mismatch, then I have to delete my entire cache, and download everything again
- - when you have huge dependencies like `torch` (~2 GB), too bad to install a general version, then a working version later in `toe` plugin
+**CONVENSIONS**:
 
-So this `pip-inside` comes out. It's just `flit-core` with `pip` as the dependency installer.
-
-
-**NOTICES**:
-
-Only supports:
  - dynamic `version` (`__version__ = 'your version'` in {root_module}/__init__.py)
  - non-dynamic `description` (in `pyproject.toml`)
  - no `src` folder in project root
  - virtualenv folder named `.venv` in project root
  - not checking hashes
 
 
@@ -56,24 +46,27 @@
 
 ## commands
 
  - pip-inside
  - pi
 
 ```shell
-pi
+> pi
 Usage: pi [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -V, --version  show version of this tool
   --help         Show this message and exit.
 
 Commands:
   add      Add a package as project dependency
   build    Build the wheel and sdist
+  freeze   Freeze dependencies into 'pi.lock'
   init     Init project in current directory
   install  Install project dependencies by groups
   publish  Publish the wheel and sdist to remote repository
   remove   Remove a package from project dependencies
+  shell    Ensure '.venv' virtualenv, and new shell into it
+  show     Show dependency tree
   version  Show version of current project
 ```
```

