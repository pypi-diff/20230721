# Comparing `tmp/processingtools-0.3.2.tar.gz` & `tmp/processingtools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\processingtools-0.3.2.tar", last modified: Mon Jul  3 11:23:32 2023, max compression
+gzip compressed data, was "dist\processingtools-0.3.3.tar", last modified: Fri Jul 21 14:48:54 2023, max compression
```

## Comparing `processingtools-0.3.2.tar` & `processingtools-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.938592 processingtools-0.3.2/
--rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2667 2023-07-03 11:23:32.937593 processingtools-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.928592 processingtools-0.3.2/ProcessingTools/
--rw-rw-rw-   0        0        0     8085 2023-07-03 11:22:43.000000 processingtools-0.3.2/ProcessingTools/EnvReco.py
--rw-rw-rw-   0        0        0     4566 2023-07-03 11:22:43.000000 processingtools-0.3.2/ProcessingTools/PrgressBar.py
--rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.2/ProcessingTools/__init__.py
--rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.2/ProcessingTools/functions.py
--rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.2/ProcessingTools/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.926592 processingtools-0.3.2/ProcessingTools.egg-info/
--rw-rw-rw-   0        0        0     2667 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2190 2023-07-03 11:22:43.000000 processingtools-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 11:23:32.938592 processingtools-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-03 11:22:43.000000 processingtools-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.203144 processingtools-0.3.3/
+-rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2667 2023-07-21 14:48:54.202145 processingtools-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.194143 processingtools-0.3.3/ProcessingTools/
+-rw-rw-rw-   0        0        0     8846 2023-07-21 14:46:58.000000 processingtools-0.3.3/ProcessingTools/EnvReco.py
+-rw-rw-rw-   0        0        0     4829 2023-07-21 14:46:58.000000 processingtools-0.3.3/ProcessingTools/PrgressBar.py
+-rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.3/ProcessingTools/__init__.py
+-rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.3/ProcessingTools/functions.py
+-rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.3/ProcessingTools/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.193143 processingtools-0.3.3/ProcessingTools.egg-info/
+-rw-rw-rw-   0        0        0     2667 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2190 2023-07-03 11:22:43.000000 processingtools-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 14:48:54.203144 processingtools-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-07-21 14:48:28.000000 processingtools-0.3.3/setup.py
```

### Comparing `processingtools-0.3.2/LICENSE` & `processingtools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.2/PKG-INFO` & `processingtools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.2
+Version: 0.3.3
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `processingtools-0.3.2/ProcessingTools/EnvReco.py` & `processingtools-0.3.3/ProcessingTools/EnvReco.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         if not os.path.exists(self.save_path):
             processingtools.functions.create_folder(self.save_path, warning=False)
 
         self.logs = open(f'{save_path}/logs.txt', 'a')
         self.project_root_path = os.path.dirname(os.path.abspath(__file__)) if project_root_path is None else project_root_path
         self.timer = time.time()
         self.present = datetime.datetime
-        self.__start = True
         self.space = space
 
         self.args = None
         self.gpu = None
         self.os = None
 
         print(f'Record in the \"{self.save_path}\".')
@@ -88,114 +87,112 @@
         if save_type not in ['txt', 'text', 'json']:
             raise ValueError('save_type must be \'txt\' or \'text\' or \'json\'')
 
         if save_type == 'json':
             with open(f'{self.save_path}/args.json', 'w') as f:
                 json.dump(args.__dict__, f, indent=4)
         else:
-            self.put_space(print_console)
             self.print_if_true('Args: ', print_console)
             args_dict = args.__dict__
             print('{', file=self.logs)
             for key in args_dict:
                 print(f'    {key}: {args_dict[key]}', file=self.logs)
             print('}', file=self.logs)
+            self.put_space(print_console)
 
         if print_console:
             args_dict = args.__dict__
             print('{')
             for key in args_dict:
                 print(f'    {key}: {args_dict[key]}')
             print('}')
+            self.put_space(print_console)
 
         self.args = args.__dict__
 
         return self.args, args
 
     @file_opener
     def record_os(self, keys: list = None, print_console: bool = True):
         """
         record os environments
         :param keys: if you insert key values, it will record only key environments
         :param print_console: if True you can see logs in the console as well
         :return: os dictionary
         """
 
-        self.put_space(print_console)
         self.print_if_true('OS Env: ', print_console)
 
         os_env = os.environ
         self.log_dict(os_env, keys, print_console)
 
         self.os = os_env
+        self.put_space(print_console)
 
         return self.os
 
     @file_opener
     def record_gpu(self, keys: list = None, print_console: bool = True) -> dict:
         """
         record gpu environments
         :param keys: if you insert key values, it will record only key environments
         :param print_console: if True you can see logs in the console as well
         :return: gpu dictionary
         """
 
-        self.put_space(print_console)
         self.print_if_true('GPU Info: ', print_console)
 
         try:
             import torch
 
             gpu = {'cuda': torch.cuda.is_available(),
                    'num': torch.cuda.device_count(),
                    'names': [torch.cuda.get_device_name(_) for _ in range(torch.cuda.device_count())]}
 
         except Exception:
             raise ImportError('this function is needed pytorch!')
 
         self.log_dict(gpu, keys, print_console)
         self.gpu = gpu
+        self.put_space(print_console)
 
         return self.gpu
 
     @file_opener
-    def print(self, log: str, console: bool = True, file: bool = True) -> None:
+    def print(self, log: str, console: bool = True, file: bool = True, time: bool = True) -> None:
         """
         write and print log with present time
         :param log: log
         :param console: if True, print in the console
         :param file: if True, write in the logs file
+        :param time: if True, write in the present time before the log
         return True
         """
 
         now = self.present.now()
+        time_info = f'[{now.year}-{now.month:02d}-{now.day:02d} {now.hour:02d}:{now.minute:02d}:{now.second:02d}.' \
+                    f'{round(now.microsecond / 10000):02d}]: ' if time else ''
+
         if console:
-            print(f'\033[32m[{now.year}-{now.month}-{now.day} '
-                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]\033[0m: {log}')
+            print(f'\033[32m{time_info}\033[0m{log}')
         if file:
-            print(f'[{now.year}-{now.month}-{now.day} '
-                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]: {log}', file=self.logs)
+            print(f'{time_info}{log}', file=self.logs)
 
     @file_opener
     def put_space(self, print_console: bool = True) -> bool:
         """
         insert space in the logs
         :param print_console: if True you can see logs in the console as well
         :return: True or False
         """
 
         if self.logs.closed:
             self.logs = open(f'{self.save_path}/logs.txt', 'a')
 
-        if self.__start:
-            self.__start = False
-            return False
-
-        else:
-            self.print_if_true(self.space, print_console)
+        self.print_if_true(self.space, print_console)
 
         return True
 
     @file_opener
     def print_if_true(self, contents: str, print_console: bool) -> None:
         """
         if print_console true, print in the console as well
@@ -237,7 +234,30 @@
         self.print_if_true('{', print_console)
 
         for key in keys:
             self.print_if_true(f'    {key}: {input_dict[key]}', print_console)
         self.print_if_true('}', print_console)
 
         return True
+
+    def record_default(self, comment: bool = True, os_key: list = None, gpu: bool = True, args=None) -> True:
+        """
+        write basic environment
+        :param comment: True if you want to write comment
+        :param os_key: insert key for recording os
+        :param gpu: if True, record gpu information
+        :param args: write args information if feed args
+        :return:
+        """
+
+        if comment:
+            self.print(f'Comments: {input("Leave comments for the logs file: ")}', console=False, time=False)
+            self.put_space()
+        if os_key is not None:
+            self.record_os(os_key)
+        if gpu:
+            self.record_gpu()
+        if args:
+            args = self.arg2abs(args)
+            self.record_arg(args)
+
+        return True
```

### Comparing `processingtools-0.3.2/ProcessingTools/PrgressBar.py` & `processingtools-0.3.3/ProcessingTools/PrgressBar.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,32 +11,29 @@
     example:
         for x in ProgressBar(100)
         for x in ProgressBar(range(0, 100))
         for x in ProgressBar([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     """
 
     def __init__(self, in_loop, bar_length: int = 40, start_mark: str = None, finish_mark='progress done!',
-                 max: int = None, total: int = None, detail_func: callable = None, remove_last: bool = False):
+                 max: int = None, total: int = None, detail_func: callable = None, remove_last: bool = False, smoothing: int = None):
         """
         The initial function
         :param in_loop: the input loop
         :param bar_length: bar length
         :param start_mark: print string when the progress start
         :param finish_mark: print string what you want when progress finish
         :param total: total value. If you do not fill this, it will calculate automatically, but it may be slow
         :param detail_func: write detail using detail_func
         :param remove_last: if True, remove progressbar when process is end
+        :param smoothing: make stable when estimate time taking
         """
 
         print(start_mark) if start_mark is not None else None
 
-        self.take = np.zeros(10, float)
-        T = time.time()
-        for i in range(10): self.take[i] = T
-
         self.start = time.time() * 1000  # for the total take time
         self.bar_length = bar_length
         self.finish_mark = finish_mark
         self.index = 0
         self.detail_func = detail_func
         self.remove_last = remove_last
 
@@ -47,14 +44,19 @@
             warnings.warn('parameter max will be deprecated in the next version. Use total instead.')
             self.length = max
         else:
             self.it, copy_it = itertools.tee(self.it)
             self.length = 0
             for _ in iter(copy_it): self.length = self.length + 1
 
+        self.smoothing = self.length // 100 if smoothing is None else smoothing
+        self.take = np.zeros(self.smoothing, float)
+        T = time.time()
+        for i in range(self.smoothing): self.take[i] = T
+
     def __iter__(self):
         return self
 
     def print_info(self, bar, space, progress_per_str, left, out, end=False):
         if self.detail_func and not end:
             print(f'\r\033[2K|{bar}{space}| \033[38;5;208m{progress_per_str}%\033[0m |'
                   f' \033[38;5;177m{self.index}/{self.length}\033[0m | \033[38;5;43m{left}\033[0m\033[0m |'
@@ -86,20 +88,20 @@
             bar = '█' * int(self.bar_length / 100 * progress_per)
             space = '░' * (self.bar_length - int(self.bar_length / 100 * progress_per))
 
             if self.index == 0:
                 # The first loop is not finished yet, so that it cannot be calculated
                 left = '...'
             else:
-                take_temp = np.zeros(10, float)
-                take_temp[:9] = self.take[1:10]
-                take_temp[9] = time.time()
+                take_temp = np.zeros(self.smoothing, float)
+                take_temp[:self.smoothing - 1] = self.take[1:self.smoothing]
+                take_temp[self.smoothing - 1] = time.time()
 
                 # make time smooth
-                if self.index >= 10:
+                if self.index >= self.smoothing:
                     left = np.mean(take_temp - self.take) * (self.length - self.index)
                 else:
                     left = np.sum(take_temp - self.take) * (self.length - self.index) / self.index
 
                 self.take = take_temp
 
                 if left >= 3600:
```

### Comparing `processingtools-0.3.2/ProcessingTools/functions.py` & `processingtools-0.3.3/ProcessingTools/functions.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.2/ProcessingTools/torch_tools.py` & `processingtools-0.3.3/ProcessingTools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.2/ProcessingTools.egg-info/PKG-INFO` & `processingtools-0.3.3/ProcessingTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.2
+Version: 0.3.3
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `processingtools-0.3.2/ProcessingTools.egg-info/SOURCES.txt` & `processingtools-0.3.3/ProcessingTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.2/README.md` & `processingtools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.2/setup.py` & `processingtools-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="processingtools",
-    version="0.3.2",
+    version="0.3.3",
     install_requires=['opencv-python>=4.5.5.62',
                       'numpy>=1.19.4',
                       'matplotlib>=3.3.3'],
     license='MIT',
     author="syy",
     author_email="ysy9997@gmail.com",
     description="https://github.com/ysy9997/ProcessingTools.git",
```

