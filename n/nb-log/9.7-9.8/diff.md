# Comparing `tmp/nb_log-9.7.tar.gz` & `tmp/nb_log-9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log-9.7.tar", last modified: Sun Jul  9 07:29:18 2023, max compression
+gzip compressed data, was "nb_log-9.8.tar", last modified: Fri Jul 21 14:26:59 2023, max compression
```

## Comparing `nb_log-9.7.tar` & `nb_log-9.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.504090 nb_log-9.7/
--rw-rw-rw-   0        0        0    30393 2023-07-09 07:29:18.502088 nb_log-9.7/PKG-INFO
--rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.481082 nb_log-9.7/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.7/nb_log/__init__.py
--rw-rw-rw-   0        0        0     3423 2023-07-06 13:56:36.000000 nb_log-9.7/nb_log/file_write.py
--rw-rw-rw-   0        0        0    51493 2023-07-09 06:01:38.000000 nb_log-9.7/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.7/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    31273 2023-07-09 05:58:10.000000 nb_log-9.7/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6764 2023-07-09 06:17:13.000000 nb_log-9.7/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.7/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0     2350 2023-07-09 06:34:51.000000 nb_log-9.7/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10816 2023-07-09 07:23:29.000000 nb_log-9.7/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     5127 2023-07-06 13:55:43.000000 nb_log-9.7/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     6260 2023-07-09 07:15:13.000000 nb_log-9.7/nb_log/rotate_file_writter.py
--rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.7/nb_log/set_nb_log_config.py
--rw-rw-rw-   0        0        0     2067 2023-07-09 04:17:03.000000 nb_log-9.7/nb_log/simple_print.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.499089 nb_log-9.7/nb_log.egg-info/
--rw-rw-rw-   0        0        0    30393 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 07:29:18.505088 nb_log-9.7/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-09 07:29:09.000000 nb_log-9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.102989 nb_log-9.8/
+-rw-rw-rw-   0        0        0    30393 2023-07-21 14:26:59.099990 nb_log-9.8/PKG-INFO
+-rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.073990 nb_log-9.8/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.8/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-07-06 13:56:36.000000 nb_log-9.8/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    51517 2023-07-09 11:39:13.000000 nb_log-9.8/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.8/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    31273 2023-07-09 05:58:10.000000 nb_log-9.8/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6841 2023-07-21 14:24:52.000000 nb_log-9.8/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.8/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0     2420 2023-07-21 14:24:52.000000 nb_log-9.8/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10921 2023-07-14 15:43:54.000000 nb_log-9.8/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     5127 2023-07-06 13:55:43.000000 nb_log-9.8/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     6283 2023-07-09 13:55:16.000000 nb_log-9.8/nb_log/rotate_file_writter.py
+-rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.8/nb_log/set_nb_log_config.py
+-rw-rw-rw-   0        0        0     2067 2023-07-09 04:17:03.000000 nb_log-9.8/nb_log/simple_print.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.094987 nb_log-9.8/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    30393 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 14:26:59.102989 nb_log-9.8/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-21 14:26:19.000000 nb_log-9.8/setup.py
```

### Comparing `nb_log-9.7/PKG-INFO` & `nb_log-9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.7
+Version: 9.8
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.7/README.md` & `nb_log-9.8/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/__init__.py` & `nb_log-9.8/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/file_write.py` & `nb_log-9.8/nb_log/file_write.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/handlers.py` & `nb_log-9.8/nb_log/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1187,17 +1187,17 @@
 
 # ConcurrentDayRotatingFileHandler = ConcurrentSecondRotatingFileHandlerLinux
 #
 # print(ConcurrentDayRotatingFileHandler)
 
 
 class BothDayAndSizeRotatingFileHandler(logging.Handler):
+    """
+    自己从头开发的按照时间和大小切割
+    """
     def __init__(self, file_name: typing.Optional[str], log_path='/pythonlogs', max_bytes=1000 * 1000 * 1000, back_count=10):
-        init_kwargs = copy.copy(locals())
-        init_kwargs.pop('self')
-        init_kwargs.pop('__class__')
         super().__init__()
-        self.os_file_writter = OsFileWritter(**init_kwargs)
+        self.os_file_writter = OsFileWritter(file_name=file_name,log_path=log_path,max_bytes=max_bytes,back_count=back_count)
 
     def emit(self, record: logging.LogRecord) -> None:
         msg = self.format(record)
         self.os_file_writter.write_2_file(msg + '\n')
```

### Comparing `nb_log-9.7/nb_log/handlers0000.py` & `nb_log-9.8/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/log_manager.py` & `nb_log-9.8/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/monkey_print.py` & `nb_log-9.8/nb_log/monkey_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 def stderr_write(msg: str):
     sys.stderr.write(msg)
     sys.stderr.flush()
 
 
 print_wrtie_file_name = os.environ.get('PRINT_WRTIE_FILE_NAME', None) or nb_log_config_default.PRINT_WRTIE_FILE_NAME
 
-print_file_writter = OsFileWritter(print_wrtie_file_name, back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT, max_bytes=nb_log_config_default.LOG_FILE_SIZE * 1024 * 1024)
+print_file_writter = OsFileWritter(print_wrtie_file_name, log_path=nb_log_config_default.LOG_PATH,
+                                   back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT, max_bytes=nb_log_config_default.LOG_FILE_SIZE * 1024 * 1024)
 
 
 def _print_with_file_line(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=2):
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
     args_str = sep.join(args) + end
     # stdout_write(f'56:{file}')
     if file == sys.stderr:
```

### Comparing `nb_log-9.7/nb_log/monkey_std_filter_words.py` & `nb_log-9.8/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/monkey_sys_std.py` & `nb_log-9.8/nb_log/monkey_sys_std.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 stdout_raw = sys.stdout.write
 stderr_raw = sys.stderr.write
 
 dele_color_pattern = re.compile('\\033\[.+?m')
 
 sys_std_file_name = os.environ.get('SYS_STD_FILE_NAME', None) or nb_log_config_default.SYS_STD_FILE_NAME
-std_writter = OsFileWritter(sys_std_file_name,back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT,max_bytes=nb_log_config_default.LOG_FILE_SIZE * 1024 * 1024)
+std_writter = OsFileWritter(sys_std_file_name,log_path=nb_log_config_default.LOG_PATH,
+                            back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT,max_bytes=nb_log_config_default.LOG_FILE_SIZE * 1024 * 1024)
 
 is_win = True if os.name == 'nt' else False
 
 
 
 class BulkStdout:
     q = queue.SimpleQueue()
```

### Comparing `nb_log-9.7/nb_log/nb_log_config_default.py` & `nb_log-9.8/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 
 MONGO_URL = 'mongodb://myUserAdmin:mimamiama@127.0.0.1:27016/admin'
 
 # 项目中的print是否自动写入到文件中。值为None则不重定向print到文件中。 自动每天一个文件， 2023-06-30.my_proj.print,生成的文件位置在定义的LOG_PATH
 # 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
 PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print'
 
-# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
+# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件，为None将不把标准输出重定向到文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
 # 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
 SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'
 
-USE_BULK_STDOUT_ON_WINDOWS = True
+USE_BULK_STDOUT_ON_WINDOWS = True # 在win上是否每隔0.1秒批量stdout,win的io太差了
 
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
@@ -143,9 +143,7 @@
     10: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板。
     11: logging.Formatter(
         f'({computer_ip},{computer_name})-[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板以及ip和主机名。
 }
 
 FORMATTER_KIND = 5  # 如果get_logger不指定日志模板，则默认选择第几个模板
-
-
```

### Comparing `nb_log-9.7/nb_log/nb_logger.py` & `nb_log-9.8/nb_log/nb_logger.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/rotate_file_writter.py` & `nb_log-9.8/nb_log/rotate_file_writter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import multiprocessing
 import queue
 import threading
 import typing
 from pathlib import Path
 import time
 import os
+
+
 # from nb_log.simple_print import sprint as print  # 在此模块中不能print，print会写入文件，文件中print又写入文件，无限懵逼死循环。
 
 
 def build_current_date_str():
     return time.strftime('%Y-%m-%d')
 
 
 class FileWritter:
     _lock = threading.RLock()
 
-
     def __init__(self, file_name: str, log_path='/pythonlogs', max_bytes=1000 * 1000 * 1000, back_count=10):
         self._max_bytes = max_bytes
         self._back_count = back_count
         self.need_write_2_file = True if file_name else False
         if self.need_write_2_file:
             self._file_name = file_name
             self.log_path = log_path
@@ -78,15 +79,15 @@
             f_list.append(f)
         # f_list.sort(key=lambda f:f.stat().st_mtime,reverse=True)
         f_list.sort(key=lambda f: f.name, reverse=True)
         for f in f_list[self._back_count:]:
             try:
                 # print(f'删除 {f} ') # 这里不能print， stdout写入文件，写入文件时候print，死循环
                 f.unlink()
-            except FileNotFoundError:
+            except (FileNotFoundError, PermissionError):
                 pass
 
 
 class BulkFileWritter:
     _lock = threading.Lock()
 
     filename__queue_map = {}
@@ -154,14 +155,15 @@
             threading.Thread(target=_bulk_write, daemon=True).start()
 
 
 atexit.register(BulkFileWritter._when_exit)
 
 OsFileWritter = FileWritter if os.name == 'posix' else BulkFileWritter
 
+
 def tt():
     fw = OsFileWritter('test_file6.log', '/test_dir2', max_bytes=1000 * 100)
     t1 = time.time()
     for i in range(10000):
         # time.sleep(0.001)
         msg = f'yyy{str(i).zfill(5)}' * 4
         print(msg)
```

### Comparing `nb_log-9.7/nb_log/set_nb_log_config.py` & `nb_log-9.8/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log/simple_print.py` & `nb_log-9.8/nb_log/simple_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.7/nb_log.egg-info/PKG-INFO` & `nb_log-9.8/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 9.7
+Version: 9.8
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.7/setup.py` & `nb_log-9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.7",
+    version="9.8",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -63,14 +63,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-9.7.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.8.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

