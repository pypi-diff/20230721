# Comparing `tmp/mppm-2.0.1.tar.gz` & `tmp/mppm-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mppm-2.0.1.tar", last modified: Thu Jul 20 08:35:27 2023, max compression
+gzip compressed data, was "mppm-3.0.1.tar", last modified: Fri Jul 21 07:51:11 2023, max compression
```

## Comparing `mppm-2.0.1.tar` & `mppm-3.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.038592 mppm-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-19 13:19:06.000000 mppm-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2773 2023-07-20 08:35:27.038592 mppm-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-20 08:31:28.000000 mppm-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.036592 mppm-2.0.1/mppm/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-19 13:19:06.000000 mppm-2.0.1/mppm/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.037593 mppm-2.0.1/mppm/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:19:06.000000 mppm-2.0.1/mppm/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.037593 mppm-2.0.1/mppm/src/command/
--rw-r--r--   0 root         (0) root         (0)     2429 2023-07-20 08:22:26.000000 mppm-2.0.1/mppm/src/command/argpass.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-19 13:19:06.000000 mppm-2.0.1/mppm/src/command/cmd_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     1403 2023-07-20 07:48:16.000000 mppm-2.0.1/mppm/src/command/download.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-07-20 08:09:36.000000 mppm-2.0.1/mppm/src/command/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.037593 mppm-2.0.1/mppm/src/common/
--rw-r--r--   0 root         (0) root         (0)     1272 2023-07-20 06:59:57.000000 mppm-2.0.1/mppm/src/common/const.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-20 08:07:46.000000 mppm-2.0.1/mppm/src/common/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.038592 mppm-2.0.1/mppm/src/config/
--rw-r--r--   0 root         (0) root         (0)     1479 2023-07-19 13:19:06.000000 mppm-2.0.1/mppm/src/config/pip_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:35:27.037593 mppm-2.0.1/mppm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2773 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      429 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-20 08:35:27.000000 mppm-2.0.1/mppm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 08:35:27.038592 mppm-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-20 08:26:31.000000 mppm-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-19 13:19:06.000000 mppm-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-21 07:51:11.828369 mppm-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-21 07:49:27.000000 mppm-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.826369 mppm-3.0.1/mppm/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-19 13:19:06.000000 mppm-3.0.1/mppm/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:19:06.000000 mppm-3.0.1/mppm/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm/src/command/
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-07-21 07:46:34.000000 mppm-3.0.1/mppm/src/command/argpass.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-21 07:25:09.000000 mppm-3.0.1/mppm/src/command/cmd_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-21 07:25:09.000000 mppm-3.0.1/mppm/src/command/download.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-21 07:34:19.000000 mppm-3.0.1/mppm/src/command/rewrite.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-07-20 08:09:36.000000 mppm-3.0.1/mppm/src/command/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/mppm/src/common/
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-21 07:49:27.000000 mppm-3.0.1/mppm/src/common/const.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-20 08:07:46.000000 mppm-3.0.1/mppm/src/common/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.828369 mppm-3.0.1/mppm/src/config/
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-21 07:34:19.000000 mppm-3.0.1/mppm/src/config/pip_conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:51:11.827370 mppm-3.0.1/mppm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-21 07:51:11.000000 mppm-3.0.1/mppm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 07:51:11.828369 mppm-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-21 07:49:27.000000 mppm-3.0.1/setup.py
```

### Comparing `mppm-2.0.1/LICENSE` & `mppm-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mppm-2.0.1/PKG-INFO` & `mppm-3.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 2.0.1
+Version: 3.0.1
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
 Classifier: Development Status :: 4 - Beta
@@ -34,40 +34,52 @@
     pip install mppm
 
 ## Usage
 
     usage: mppm  <sub-commands>  [<args>] 
 
     mppm Manage pip sources and dependent packages
-
+    
     positional arguments:
-      {download,uninstall}
+      {download,uninstall,config}
         download            download modules
         uninstall           uninstall modules
-
+        config              rewrite pip configuration
+    
     options:
       -h, --help            show this help message and exit
+      -v, --version         show program's version number and exit
+
+### SubCommand: config
+    usage: mppm  <sub-commands>  [<args>] config [-h] [-y]
+
+    options:
+      -h, --help  show this help message and exit
+      -y, --yes   force rewrite pip configuration
+
+#### examples
 
+    mppm config
 
 ### SubCommand: download
 
     usage: mppm  <sub-commands>  [<args>] download [-h] (-m MODULE | -r REQUIREMENT) [-y]
-
+    
     options:
       -h, --help            show this help message and exit
       -m MODULE, --module MODULE
                             download specified modules and dependencies
       -r REQUIREMENT, --requirement REQUIREMENT
                             download the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             rewrite the pip configuration
 
+
   #### examples
     mppm download -m flask  
-    mppm download -r /tmp/requiremen.txt -y
-
+    mppm download -r /tmp/requiremen.txt
 
 ### SubCommand: uninstall
 
     usage: mppm  <sub-commands>  [<args>] uninstall [-h] (-m MODULE | -r REQUIREMENT) [-y]
 
     options:
       -h, --help            show this help message and exit
@@ -77,17 +89,16 @@
                             uninstall the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             interactive
 
   #### examples
     mppm uninstall -m flask
     mppm download -r /tmp/requiremen.txt -y
 
+## Configuration
 
-#### Configuration
-
-You can add package indexes to your `pip.conf` file. Example:
+You can add package indexes to your `~/.pip/pip.conf` file. Example:
 
     [global]
     timeout = 120
     index-url = https://pypi.org/simple/
     trusted-host = pypi.org
```

### Comparing `mppm-2.0.1/README.md` & `mppm-3.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -14,40 +14,52 @@
     pip install mppm
 
 ## Usage
 
     usage: mppm  <sub-commands>  [<args>] 
 
     mppm Manage pip sources and dependent packages
-
+    
     positional arguments:
-      {download,uninstall}
+      {download,uninstall,config}
         download            download modules
         uninstall           uninstall modules
-
+        config              rewrite pip configuration
+    
     options:
       -h, --help            show this help message and exit
+      -v, --version         show program's version number and exit
+
+### SubCommand: config
+    usage: mppm  <sub-commands>  [<args>] config [-h] [-y]
+
+    options:
+      -h, --help  show this help message and exit
+      -y, --yes   force rewrite pip configuration
+
+#### examples
 
+    mppm config
 
 ### SubCommand: download
 
     usage: mppm  <sub-commands>  [<args>] download [-h] (-m MODULE | -r REQUIREMENT) [-y]
-
+    
     options:
       -h, --help            show this help message and exit
       -m MODULE, --module MODULE
                             download specified modules and dependencies
       -r REQUIREMENT, --requirement REQUIREMENT
                             download the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             rewrite the pip configuration
 
+
   #### examples
     mppm download -m flask  
-    mppm download -r /tmp/requiremen.txt -y
-
+    mppm download -r /tmp/requiremen.txt
 
 ### SubCommand: uninstall
 
     usage: mppm  <sub-commands>  [<args>] uninstall [-h] (-m MODULE | -r REQUIREMENT) [-y]
 
     options:
       -h, --help            show this help message and exit
@@ -57,17 +69,16 @@
                             uninstall the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             interactive
 
   #### examples
     mppm uninstall -m flask
     mppm download -r /tmp/requiremen.txt -y
 
+## Configuration
 
-#### Configuration
-
-You can add package indexes to your `pip.conf` file. Example:
+You can add package indexes to your `~/.pip/pip.conf` file. Example:
 
     [global]
     timeout = 120
     index-url = https://pypi.org/simple/
     trusted-host = pypi.org
```

### Comparing `mppm-2.0.1/mppm/src/command/download.py` & `mppm-3.0.1/mppm/src/command/download.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,27 +2,16 @@
 from src.config.pip_conf import *
 import os
 
 
 class DownloadCmd():
     def __init__(self, args):
         self.args = args
-        self.rewrite_config = args.yes
-
-    def confirmation_prompt(self):
-        yes_list = ["yes", "y"]
-        prompt = "Are you sure want to continue rewrite the pip configuration: (yes/y/no)? "
-        if self.rewrite_config:
-            if input(prompt).lower().strip() not in yes_list:
-                print_colored("cancel rewrite the pip configuration", "yellow")
-            else:
-                verification_pypi_url()
 
     def exec(self, pip_path):
-        self.confirmation_prompt()
         if self.args.module:
             create_dir(self.args.module)
             download_pip_pkg_cmd = "{} download {} -d {}".format(pip_path, self.args.module, self.args.module)
         else:
             create_dir(ARG_DOWNLOAD_REQUIREMENT)
             download_pip_pkg_cmd = "{} download -r {} -d {}".format(pip_path, self.args.requirement,
                                                                     ARG_DOWNLOAD_REQUIREMENT)
```

### Comparing `mppm-2.0.1/mppm/src/command/uninstall.py` & `mppm-3.0.1/mppm/src/command/uninstall.py`

 * *Files identical despite different names*

### Comparing `mppm-2.0.1/mppm/src/common/const.py` & `mppm-3.0.1/mppm/src/common/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 APP_NAME = 'mppm'  # 程序名称
+APP_VERSION_MAJOR = "3.0"
+APP_VERSION_MINOR = "1"
 EXIT_WITH_ERROR = 9999  # 错误退出码12 为用户自定义信号
 
 pypi_configuration_sources = [
     {"name": "pypi", "url": "https://pypi.org/simple/", "timeout": "120"},
     {"name": "tuna", "url": "https://pypi.tuna.tsinghua.edu.cn/simple/", "timeout": "60"},
     {"name": "aliyun", "url": "https://mirrors.aliyun.com/pypi/simple/", "timeout": "60"},
     {"name": "douban", "url": "http://pypi.douban.com/simple/", "timeout": "60"},
@@ -12,14 +14,19 @@
 pip_configuration_name = "pip.conf"
 
 ignore_errors = {
     "download": "You should consider upgrading",
     "uninstall": "not an installed pip module"
 }
 
+# rewrite pip configuration
+SUB_CMD_REWRITE = "config"
+ARG_CONFIG_REWRITE_FORCE = "yes"
+ARG_CONFIG_REWRITE_FORCE_SHORT = "y"
+
 # Download specified modules and dependencies
 SUB_CMD_DOWNLOAD = "download"
 ARG_DOWNLOAD_MODULE = "module"
 ARG_DOWNLOAD_MODULE_SHORT = "m"
 ARG_DOWNLOAD_REQUIREMENT = "requirement"
 ARG_DOWNLOAD_REQUIREMENT_SHORT = "r"
 ARG_DOWNLOAD_REWRITE_PIP_CONFIG = "yes"
@@ -29,7 +36,11 @@
 SUB_CMD_UNINSTALL = "uninstall"
 ARG_UNINSTALL_MODULE = "module"
 ARG_UNINSTALL_MODULE_SHORT = "m"
 ARG_UNINSTALL_REQUIREMENT = "requirement"
 ARG_UNINSTALL_REQUIREMENT_SHORT = "r"
 ARG_UNINSTALL_FORCE = "yes"
 ARG_UNINSTALL_FORCE_SHORT = "y"
+
+# get version
+ARG_VERSION = "version"
+ARG_VERSION_SHORT = "v"
```

### Comparing `mppm-2.0.1/mppm/src/common/utility.py` & `mppm-3.0.1/mppm/src/common/utility.py`

 * *Files identical despite different names*

### Comparing `mppm-2.0.1/mppm/src/config/pip_conf.py` & `mppm-3.0.1/mppm/src/config/pip_conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 from src.common.utility import *
 from pick import pick
 import os
 import configparser
 
 
 def choice_pipy_source():
-    """
+	"""
     :return: choose pypi source url
     """
-    title = "Please choose a PyPI Configuration Source: "
-    options = [f"{source['name']: <20}{source['url']}" for source in pypi_configuration_sources]
-    option, index = pick(options, title, indicator="=>")
-    url = pypi_configuration_sources[index]["url"]
-    timeout = pypi_configuration_sources[index]["timeout"]
-    return url, timeout
+	title = "Please choose a PyPI Configuration Source: "
+	options = [f"{source['name']: <20}{source['url']}" for source in pypi_configuration_sources]
+	option, index = pick(options, title, indicator="=>")
+	url = pypi_configuration_sources[index]["url"]
+	timeout = pypi_configuration_sources[index]["timeout"]
+	return url, timeout
 
 
 def rewrite_pypi_config(url, timeout):
-    """
+	"""
     :param url: pip source url
     :return: configparser obj
     """
-    config = configparser.ConfigParser(allow_no_value=True)
+	config = configparser.ConfigParser(allow_no_value=True)
 
-    config.add_section("global")
-    config.set('global', 'timeout', timeout)
-    config.set('global', 'index-url', url)
-    config.set('global', 'trusted-host', url.split("/")[2])
-    return config
+	config.add_section("global")
+	config.set('global', 'timeout', timeout)
+	config.set('global', 'index-url', url)
+	config.set('global', 'trusted-host', url.split("/")[2])
+	return config
 
 
 def verification_pypi_url():
-    pypi_source_url, timeout = choice_pipy_source()
-    if pypi_source_url == "None":
-        print_colored("Skip pip repositories configuration.", "yellow")
-    else:
-        config = rewrite_pypi_config(pypi_source_url, timeout)
-        home = os.path.expanduser("~")
-        config_file = os.path.join(home, ".pip", "pip.conf")
-        with open(config_file, "w", encoding="utf8") as f:
-            config.write(f)
-        print_colored("Successfully updated pip repositories configuration[{}]".format(config_file), "green")
+	pypi_source_url, timeout = choice_pipy_source()
+	if pypi_source_url == "None":
+		print_colored("Skip pip repositories configuration.", "yellow")
+	else:
+		config = rewrite_pypi_config(pypi_source_url, timeout)
+		home = os.path.expanduser("~")
+		config_file = os.path.join(home, ".pip", "pip.conf")
+		with open(config_file, "w", encoding="utf8") as f:
+			config.write(f)
+		print_colored("Successfully updated pip repositories configuration[{}]".format(config_file), "green")
```

### Comparing `mppm-2.0.1/mppm.egg-info/PKG-INFO` & `mppm-3.0.1/mppm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppm
-Version: 2.0.1
+Version: 3.0.1
 Summary: Manager Pypi Package & Mirror
 Home-page: https://gitee.com/TianCiwang/mppm.git
 Author: TianCiwang
 Author-email: 13623650548@163.com
 License: MIT
 Keywords: pypi,mirror,package
 Classifier: Development Status :: 4 - Beta
@@ -34,40 +34,52 @@
     pip install mppm
 
 ## Usage
 
     usage: mppm  <sub-commands>  [<args>] 
 
     mppm Manage pip sources and dependent packages
-
+    
     positional arguments:
-      {download,uninstall}
+      {download,uninstall,config}
         download            download modules
         uninstall           uninstall modules
-
+        config              rewrite pip configuration
+    
     options:
       -h, --help            show this help message and exit
+      -v, --version         show program's version number and exit
+
+### SubCommand: config
+    usage: mppm  <sub-commands>  [<args>] config [-h] [-y]
+
+    options:
+      -h, --help  show this help message and exit
+      -y, --yes   force rewrite pip configuration
+
+#### examples
 
+    mppm config
 
 ### SubCommand: download
 
     usage: mppm  <sub-commands>  [<args>] download [-h] (-m MODULE | -r REQUIREMENT) [-y]
-
+    
     options:
       -h, --help            show this help message and exit
       -m MODULE, --module MODULE
                             download specified modules and dependencies
       -r REQUIREMENT, --requirement REQUIREMENT
                             download the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             rewrite the pip configuration
 
+
   #### examples
     mppm download -m flask  
-    mppm download -r /tmp/requiremen.txt -y
-
+    mppm download -r /tmp/requiremen.txt
 
 ### SubCommand: uninstall
 
     usage: mppm  <sub-commands>  [<args>] uninstall [-h] (-m MODULE | -r REQUIREMENT) [-y]
 
     options:
       -h, --help            show this help message and exit
@@ -77,17 +89,16 @@
                             uninstall the modules and dependencies specified in the file. like requirements.txt
       -y, --yes             interactive
 
   #### examples
     mppm uninstall -m flask
     mppm download -r /tmp/requiremen.txt -y
 
+## Configuration
 
-#### Configuration
-
-You can add package indexes to your `pip.conf` file. Example:
+You can add package indexes to your `~/.pip/pip.conf` file. Example:
 
     [global]
     timeout = 120
     index-url = https://pypi.org/simple/
     trusted-host = pypi.org
```

### Comparing `mppm-2.0.1/setup.py` & `mppm-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'pick',
     'configparser',
     'pip-autoremove',
 ]
 
 setup(
     name='mppm',
-    version='2.0.1',
+    version='3.0.1',
     description='Manager Pypi Package & Mirror',
     keywords='pypi,mirror,package',
     url='https://gitee.com/TianCiwang/mppm.git',
     long_description=fread('README.md'),
     long_description_content_type='text/markdown',
     author='TianCiwang',
     author_email='13623650548@163.com',
```

