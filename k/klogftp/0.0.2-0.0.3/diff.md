# Comparing `tmp/klogftp-0.0.2.tar.gz` & `tmp/klogftp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\klogftp-0.0.2.tar", last modified: Wed Jul 19 10:27:32 2023, max compression
+gzip compressed data, was "dist\klogftp-0.0.3.tar", last modified: Fri Jul 21 05:55:24 2023, max compression
```

## Comparing `klogftp-0.0.2.tar` & `klogftp-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 10:27:32.000000 klogftp-0.0.2/
--rw-rw-rw-   0        0        0      499 2023-07-19 10:27:32.000000 klogftp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-07-18 06:34:03.000000 klogftp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogFTP/
--rw-rw-rw-   0        0        0     2044 2023-07-17 06:08:37.000000 klogftp-0.0.2/klogFTP/HRMISPasswordTool.py
--rw-rw-rw-   0        0        0        0 2023-07-18 06:25:20.000000 klogftp-0.0.2/klogFTP/__init__.py
--rw-rw-rw-   0        0        0     3858 2023-07-17 06:08:37.000000 klogftp-0.0.2/klogFTP/database.py
--rw-rw-rw-   0        0        0      659 2023-07-17 06:08:37.000000 klogftp-0.0.2/klogFTP/dataframe_process.py
--rw-rw-rw-   0        0        0    20911 2023-07-18 05:39:40.000000 klogftp-0.0.2/klogFTP/hrapi.py
--rw-rw-rw-   0        0        0    10624 2023-07-19 08:29:47.000000 klogftp-0.0.2/klogFTP/kid_logger_file_arrange.py
--rw-rw-rw-   0        0        0     3724 2023-07-19 08:29:42.000000 klogftp-0.0.2/klogFTP/log.py
--rw-rw-rw-   0        0        0     1317 2023-07-19 08:29:33.000000 klogftp-0.0.2/klogFTP/portal.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogftp.egg-info/
--rw-rw-rw-   0        0        0      499 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogftp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogftp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogftp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 10:27:32.000000 klogftp-0.0.2/klogftp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 10:27:32.000000 klogftp-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-07-19 10:27:14.000000 klogftp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:55:24.000000 klogftp-0.0.3/
+-rw-rw-rw-   0        0        0      499 2023-07-21 05:55:24.000000 klogftp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-07-18 06:34:03.000000 klogftp-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogFTP/
+-rw-rw-rw-   0        0        0     2044 2023-07-17 06:08:37.000000 klogftp-0.0.3/klogFTP/HRMISPasswordTool.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:25:20.000000 klogftp-0.0.3/klogFTP/__init__.py
+-rw-rw-rw-   0        0        0     3858 2023-07-17 06:08:37.000000 klogftp-0.0.3/klogFTP/database.py
+-rw-rw-rw-   0        0        0      659 2023-07-17 06:08:37.000000 klogftp-0.0.3/klogFTP/dataframe_process.py
+-rw-rw-rw-   0        0        0    20911 2023-07-18 05:39:40.000000 klogftp-0.0.3/klogFTP/hrapi.py
+-rw-rw-rw-   0        0        0    10624 2023-07-19 08:29:47.000000 klogftp-0.0.3/klogFTP/kid_logger_file_arrange.py
+-rw-rw-rw-   0        0        0     3391 2023-07-21 05:54:11.000000 klogftp-0.0.3/klogFTP/log.py
+-rw-rw-rw-   0        0        0     1317 2023-07-19 08:29:33.000000 klogftp-0.0.3/klogFTP/portal.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogftp.egg-info/
+-rw-rw-rw-   0        0        0      499 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogftp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogftp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogftp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 05:55:24.000000 klogftp-0.0.3/klogftp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:55:24.000000 klogftp-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-07-21 05:54:33.000000 klogftp-0.0.3/setup.py
```

### Comparing `klogftp-0.0.2/klogFTP/HRMISPasswordTool.py` & `klogftp-0.0.3/klogFTP/HRMISPasswordTool.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/klogFTP/database.py` & `klogftp-0.0.3/klogFTP/database.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/klogFTP/dataframe_process.py` & `klogftp-0.0.3/klogFTP/dataframe_process.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/klogFTP/hrapi.py` & `klogftp-0.0.3/klogFTP/hrapi.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/klogFTP/kid_logger_file_arrange.py` & `klogftp-0.0.3/klogFTP/kid_logger_file_arrange.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/klogFTP/log.py` & `klogftp-0.0.3/klogFTP/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,99 +4,99 @@
 from pathlib import Path
 from datetime import date
 from datetime import datetime
 
 BASE_DIR = Path(__file__).resolve().parent
 
 class Log_model:
-    def __init__(self, getlogger, log_path) -> None:
-        self.getlogger = getlogger
-        self.__logname = '%s.log' % datetime.strftime(datetime.now(), "%Y-%m-%d")
-        self.logdir = log_path
-        self.path = log_path + self.__logname
-        if not os.path.exists(self.logdir):
-            os.mkdir(self.logdir)
-
-    def settings(self, format="%(asctime)s - [line:%(lineno)d] - %(levelname)s: %(message)s"):
-        os.makedirs(self.logdir, exist_ok=True)
-
-        logging.basicConfig(
-            level=logging.DEBUG,
-            format=format,
-            filename=self.path
-        )
-        Log = logging.getLogger(self.getlogger)
-        Log.setLevel(logging.DEBUG)
-
-        # 待改
-        handler_path = f'{BASE_DIR}/{self.logdir}/{self.__logname}'.replace('\\','').replace('/','')
-        handlers = [handler.baseFilename.replace('\\','').replace('/','') for handler in Log.handlers if len(Log.handlers) > 0]
-
-        if handler_path not in handlers:
-            fileHandler = logging.FileHandler(self.path, mode="a")
-            fileHandler.setLevel(logging.INFO)
-
-            streamHandler = logging.StreamHandler()
-            streamHandler.setLevel(logging.WARNING)
-
-            AllFormatter = logging.Formatter(format)
-            fileHandler.setFormatter(AllFormatter)
-            streamHandler.setFormatter(AllFormatter)
-
-            Log.addHandler(fileHandler)
-            Log.addHandler(streamHandler)
-        return Log
+	def __init__(self, getlogger, log_path) -> None:
+		self.getlogger = getlogger
+		self.__logname = '%s.log' % datetime.strftime(datetime.now(), "%Y-%m-%d")
+		self.logdir = log_path
+		self.path = log_path + self.__logname
+		if not os.path.exists(self.logdir):
+			os.mkdir(self.logdir)
+
+	def settings(self, format="%(asctime)s - %(filename)s - %(funcName)s - [line:%(lineno)d] - %(levelname)s: %(message)s"):
+		os.makedirs(self.logdir, exist_ok=True)
+
+		logging.basicConfig(
+			level=logging.DEBUG,
+			format=format,
+			filename=self.path
+		)
+		Log = logging.getLogger(self.getlogger)
+		Log.setLevel(logging.DEBUG)
+
+		# 待改
+		handler_path = f'{BASE_DIR}/{self.logdir}/{self.__logname}'.replace('\\','').replace('/','')
+		handlers = [handler.baseFilename.replace('\\','').replace('/','') for handler in Log.handlers if len(Log.handlers) > 0]
+
+		if handler_path not in handlers:
+			fileHandler = logging.FileHandler(self.path, mode="a")
+			fileHandler.setLevel(logging.INFO)
+
+			streamHandler = logging.StreamHandler()
+			streamHandler.setLevel(logging.WARNING)
+
+			AllFormatter = logging.Formatter(format)
+			fileHandler.setFormatter(AllFormatter)
+			streamHandler.setFormatter(AllFormatter)
+
+			Log.addHandler(fileHandler)
+			Log.addHandler(streamHandler)
+		return Log
 
 
 def logger(message, log_path):
-    if not os.path.exists(log_path):
-        os.mkdir(log_path)
-    LOG_FILENAME = f'{datetime.strftime(datetime.now(), "%Y-%m-%d")}.log'
-
-    logging.basicConfig(
-        filename = log_path + LOG_FILENAME,
-        level= logging.DEBUG,
-        format='%(asctime)s - {username} - %(filename)s - %(funcName)s - %(lineno)d - %(levelname)s - %(message)s'.format(username = os.environ.get('USERNAME')),
-        datefmt='%Y/%m/%d %I:%M:%S'
-    )
-
-    logging.debug(message)
-    # with open(log_path + LOG_FILENAME, 'a', encoding='utf-8') as file:
-    # 	file.read()
+	if not os.path.exists(log_path):
+		os.mkdir(log_path)
+	LOG_FILENAME = f'{datetime.strftime(datetime.now(), "%Y-%m-%d")}.log'
+
+	logging.basicConfig(
+		filename = log_path + LOG_FILENAME,
+		level= logging.DEBUG,
+		format='%(asctime)s - %(levelname)s - {username} - %(filename)s - %(funcName)s - %(lineno)d - %(message)s'.format(username = os.environ.get('USERNAME')),
+		datefmt='%Y/%m/%d %I:%M:%S'
+	)
+
+	logging.debug(message)
+	# with open(log_path + LOG_FILENAME, 'a', encoding='utf-8') as file:
+	# 	file.read()
 
 
 def logMessage(level:str ,message:str, log_path:str, **kwargs) -> None:
-    if not os.path.exists(log_path):
-        os.mkdir(log_path)
-    logpath = log_path
-    if "logpath" in kwargs:
-        logpath = kwargs['logpath']
-    if not os.path.exists(logpath):
-        os.makedirs(logpath)
-
-    logname = f"{date.today()}.log"
-    if "logname" in kwargs:
-        logname = kwargs["logname"]
-
-    levelMode = ""
-    if level == "debug": levelMode = logging.DEBUG
-    elif level == "info": levelMode = logging.INFO
-    elif level == "warning": levelMode = logging.WARNING
-    elif level == "error": levelMode = logging.ERROR
-    elif level == "critical": levelMode = logging.CRITICAL
-    elif level == "exception": levelMode = logging.ERROR
-
-    logging.basicConfig(
-        filename = os.path.join(logpath, logname),
-        level= levelMode,
-        format='%(asctime)s - {username} - %(funcName)s - %(levelname)s - %(message)s'.format(username = os.environ.get('USERNAME')),
-        datefmt='%Y/%m/%d %I:%M:%S'
-    )
-
-    open(os.path.join(logpath, logname), 'a', encoding='utf-8')
-
-    if level == "debug": logging.debug(message)
-    elif level == "info": logging.info(message)
-    elif level == "warning": logging.warning(message)
-    elif level == "error": logging.error(message)
-    elif level == "critical": logging.critical(message)
-    elif level == "exception": logging.exception(message)
+	if not os.path.exists(log_path):
+		os.mkdir(log_path)
+	logpath = log_path
+	if "logpath" in kwargs:
+		logpath = kwargs['logpath']
+	if not os.path.exists(logpath):
+		os.makedirs(logpath)
+
+	logname = f"{date.today()}.log"
+	if "logname" in kwargs:
+		logname = kwargs["logname"]
+
+	levelMode = ""
+	if level == "debug": levelMode = logging.DEBUG
+	elif level == "info": levelMode = logging.INFO
+	elif level == "warning": levelMode = logging.WARNING
+	elif level == "error": levelMode = logging.ERROR
+	elif level == "critical": levelMode = logging.CRITICAL
+	elif level == "exception": levelMode = logging.ERROR
+
+	logging.basicConfig(
+		filename = os.path.join(logpath, logname),
+		level= levelMode,
+		format='%(asctime)s - %(levelname)s - {username} - %(filename)s - %(funcName)s - %(message)s'.format(username = os.environ.get('USERNAME')),
+		datefmt='%Y/%m/%d %I:%M:%S'
+	)
+
+	open(os.path.join(logpath, logname), 'a', encoding='utf-8')
+
+	if level == "debug": logging.debug(message)
+	elif level == "info": logging.info(message)
+	elif level == "warning": logging.warning(message)
+	elif level == "error": logging.error(message)
+	elif level == "critical": logging.critical(message)
+	elif level == "exception": logging.exception(message)
```

### Comparing `klogftp-0.0.2/klogFTP/portal.py` & `klogftp-0.0.3/klogFTP/portal.py`

 * *Files identical despite different names*

### Comparing `klogftp-0.0.2/setup.py` & `klogftp-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # readme.md = github readme.md, 這裡可接受markdown寫法
 # 如果沒有的話，需要自己打出介紹此專案的檔案，再讓程式知道
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="klogftp", #
-    version="0.0.2",
+    version="0.0.3",
     author="JasonWu",
     author_email="wujason0509@gmail.com",
     description="This is a package for Klog.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

