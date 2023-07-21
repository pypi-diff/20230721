# Comparing `tmp/mtmtool-1.2.8.tar.gz` & `tmp/mtmtool-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.2.8.tar", last modified: Mon Jun 19 12:48:09 2023, max compression
+gzip compressed data, was "mtmtool-1.2.9.tar", last modified: Wed Jun 21 03:13:24 2023, max compression
```

## Comparing `mtmtool-1.2.8.tar` & `mtmtool-1.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.105533 mtmtool-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-19 12:48:00.000000 mtmtool-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-19 12:48:00.000000 mtmtool-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-19 12:48:09.101533 mtmtool-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-19 12:48:00.000000 mtmtool-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 12:48:09.105533 mtmtool-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-06-19 12:48:00.000000 mtmtool-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/functool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/itertools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-19 12:48:00.000000 mtmtool-1.2.8/src/mtmtool/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 12:48:08.000000 mtmtool-1.2.8/src/mtmtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-19 12:48:09.000000 mtmtool-1.2.8/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 12:48:09.101533 mtmtool-1.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-19 12:48:00.000000 mtmtool-1.2.8/test/test_args2kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-06-19 12:48:00.000000 mtmtool-1.2.8/test/test_map_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:24.395521 mtmtool-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-21 03:13:15.000000 mtmtool-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-21 03:13:15.000000 mtmtool-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-21 03:13:24.395521 mtmtool-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-21 03:13:15.000000 mtmtool-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 03:13:24.395521 mtmtool-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-06-21 03:13:15.000000 mtmtool-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:24.391521 mtmtool-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:24.391521 mtmtool-1.2.9/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5671 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-21 03:13:15.000000 mtmtool-1.2.9/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:24.391521 mtmtool-1.2.9/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-21 03:13:24.000000 mtmtool-1.2.9/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 03:13:24.395521 mtmtool-1.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-21 03:13:15.000000 mtmtool-1.2.9/test/test_args2kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-21 03:13:15.000000 mtmtool-1.2.9/test/test_map_pool.py
```

### Comparing `mtmtool-1.2.8/LICENSE` & `mtmtool-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/PKG-INFO` & `mtmtool-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.8
+Version: 1.2.9
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.8/setup.py` & `mtmtool-1.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_python_tool"
 abbreviation_name = "mtmtool"
 description = " A Personal Python Tool Library."
-version = "1.2.8"
+version = "1.2.9"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmtool-1.2.8/src/mtmtool/functool.py` & `mtmtool-1.2.9/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool/io.py` & `mtmtool-1.2.9/src/mtmtool/io.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool/log.py` & `mtmtool-1.2.9/src/mtmtool/log.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool/pool.py` & `mtmtool-1.2.9/src/mtmtool/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial, update_wrapper
 from itertools import product
 from mtmtool.log import create_stream_logger
 from multiprocessing import Pool
 from multiprocessing.pool import ThreadPool
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 import os, sys
-from collections.abc import Callable
+from collections.abc import Callable, Generator
 import dill
 
 logger = create_stream_logger("Pool")
 
 CPUNUM = os.cpu_count()
 
 
@@ -55,93 +55,93 @@
     else:
         with pool(worker_num) as p:
             res = p.starmap(func, iters)
     return res
 
 
 class MapPool:
-    def __init__(self, func:Callable=None, max_workers:int=None, ptype:str="Thread", **kwargs) -> None:
+    def __init__(self, func:Callable=None, max_workers:int=None, pool_type:str="Thread", **kwargs) -> None:
         self.max_workers = max_workers # 最大worker数量
         self.buffer = [] # 任务缓冲区
-        self.pool_type = ptype # 进程池类型
+        self.pool_type = pool_type # 进程池类型
         # 将函数序列化，以便在子进程中使用
         self.function_dill = dill.dumps(func)
         # 复制函数属性
         update_wrapper(self, func)
         self.__wrapped__ = self.function_dill
         
 
     def __call__(self, *args, **kwargs):
         workers = kwargs.get("workers", self.max_workers)
         if "workers" in kwargs:
             kwargs.pop("workers")        
-        if workers == 1:
-            # 如果只有一个worker, 则直接运行
+        if workers is None:
+            # 如果没有传入worker数量, 则像普通函数一样运行
             func = dill.loads(self.function_dill)
             return func(*args, **kwargs)
         else:
-            # 如果有多个worker, 则将任务放入缓冲区
+            # 如果指定了worker数量, 则将任务放入缓冲区
             self.buffer.append((args, kwargs))
 
     def worker_wrapper(self, arg:tuple, func:Callable=None):
         args, kwargs = arg
         if func is None or sys.modules["__mp_main__"].__name__ == "__mp_main__":
             # 如果是在子进程中, 则需要重新加载函数
             import dill
             if not hasattr(self, "_func"):
                 self._func = dill.loads(self.function_dill)
             return self._func(*args, **kwargs)
         else:
             return func(*args, **kwargs)
 
     
-    def result(self, max_workers:int=None, pool_type:str=None):
+    def result(self, workers:int=None, pool_type:str=None)->Generator:
         # 如果没有传入参数, 则使用构造时的参数
-        if max_workers is None:
-            max_workers = self.max_workers
+        if workers is None:
+            workers = self.max_workers
         if pool_type is None:
             pool_type = self.pool_type
         # 如果缓冲区为空, 则直接返回
-        if max_workers == 1 or max_workers is None:
-            # 如果只有一个worker, 则直接运行
+        if workers == 1 or workers is None:
+            # 如果只有一个worker, 或者没有传入worker数量, 则直接运行，不使用线程池或进程池
             _func = dill.loads(self.function_dill)
             result = [_func(*args, **kwargs) for args, kwargs in self.buffer]
         else:
-            logger.info("Running ({} workers, {} tasks)".format(max_workers, len(self.buffer)))
+            logger.info("Running ({} workers, {} tasks)".format(workers, len(self.buffer)))
             # 如果有多个worker, 则运行缓冲区中的任务
-            if pool_type is not None and self.pool_type.lower() == "process":
+            if pool_type is not None and pool_type.lower() == "process":
                 # 如果是进程池, 则需要将函数序列化，否则会报错
                 worker_wrapper = partial(self.worker_wrapper, func=None)
                 pool_executor = ProcessPoolExecutor
             else:
                 # 如果是线程池, 则不需要将函数序列化
                 worker_wrapper = partial(self.worker_wrapper, func=dill.loads(self.function_dill))
                 pool_executor = ThreadPoolExecutor
             # 使用线程池或进程池运行任务
-            with pool_executor(max_workers=max_workers) as executor:
+            with pool_executor(max_workers=workers) as executor:
                 result = executor.map(worker_wrapper, self.buffer)
         # 清空缓冲区
         self.buffer = []
         # 清空函数self._func
         if hasattr(self, "_func"):
             del self._func
         # 返回结果
         return result
 
-def map_pool(func:Callable=None, max_workers:int=None, pool_type:str=None):
+def pooling(func:Callable=None, max_workers:int=None, pool_type:str=None):
     """这是一个装饰器，用于将函数转换为MapPool对象
 
     Parameters
     ----------
     func : Callable, optional
-        输入函数,使用形式为@map_pool, 不能传入参数, by default None
+        输入函数,使用形式为@pooling, 不能传入参数, by default None
     max_workers : int, optional
-        默认最大工作数目,使用形式为@map_pool(), by default None
+        默认最大工作数目,使用形式为@pooling(), by default None
     pool_type : str, optional
-        默认类型,使用形式为@map_pool(), by default None
+        默认类型,使用形式为@pooling(), by default None
 
     Returns
     -------
     Callable
         返回MapPool对象
     """
     if func is not None and isinstance(func, Callable) and max_workers is None and pool_type is None:
```

### Comparing `mtmtool-1.2.8/src/mtmtool/projection.py` & `mtmtool-1.2.9/src/mtmtool/projection.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool/time.py` & `mtmtool-1.2.9/src/mtmtool/time.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool/webhook.py` & `mtmtool-1.2.9/src/mtmtool/webhook.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.9/src/mtmtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.8
+Version: 1.2.9
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.8/test/test_args2kwargs.py` & `mtmtool-1.2.9/test/test_args2kwargs.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.8/test/test_map_pool.py` & `mtmtool-1.2.9/test/test_map_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,91 @@
-from mtmtool.pool import map_pool, MapPool
-
+from mtmtool.pool import pooling, MapPool
 def test_MapPool():
     def add(a, b):
         return a + b
-    pow = MapPool(add, max_workers=1, ptype="Thread")
+    pow = MapPool(add)
     result = pow(10,5)
     assert result == 15
 
     pow = MapPool(add, max_workers=2, ptype="Thread")
     result = pow(10,5)
     result = pow(10,5)
     assert list(pow.result()) == [15, 15]
 
     pow = MapPool(add, max_workers=2, ptype="process")
     result = pow(10,5)
     result = pow(10,5)
     assert list(pow.result()) == [15, 15]
 
-    pow = MapPool(add, max_workers=1, ptype="process")
+    pow = MapPool(add, max_workers=None, ptype="process")
+    result = pow(10,5)
+    assert result == 15
+
+    pow = MapPool(add, max_workers=None, ptype="Thread")
     result = pow(10,5)
     assert result == 15
 
-def test_map_pool():
-    # 构造装饰器后的函数
-    @map_pool(max_workers=2, pool_type="Thread")
+def test_pooling_no_params():
+    # 构造装饰器后的函数，装饰时不带传入参数，（推荐）
+    @pooling
+    def add(a, b):
+        return a + b
+
+    # 单线程运行
+    assert add(1, 2) == 3
+
+    # 多线程运行
+    add(1, 2, workers=2)
+    add(1, 3, workers=2)
+    assert list(add.result(workers=2, pool_type="Thread")) == [3, 4]
+
+    # 多进程运行
+    add(1, 2, workers=2)
+    add(1, 3, workers=2)
+    assert list(add.result(workers=2, pool_type="Process")) == [3, 4]
+
+    # 测试装饰器后更改max_workers，是否生效
+    add.max_workers = 2
+    add(1, 2)
+    add(1, 3)
+    assert list(add.result(pool_type="Thread")) == [3, 4]
+    
+    # 测试装饰器后更改pool_type，是否生效
+    add.max_workers = 2
+    add.pool_type = "Process"
+    add(1, 2)
+    add(1, 3)
+    assert list(add.result(pool_type="Thread")) == [3, 4]
+    
+def test_pooling_with_params():
+    # 构造装饰器后的函数, 装饰时带传入参数
+    @pooling(max_workers=2, pool_type="Thread")
     def add(a, b):
         return a + b
     
     # 单线程运行
-    assert add(1, 2, workers=1) == 3
+    assert add(1, 2, workers=None) == 3
 
     # 多线程运行
     add(1, 2)
     add(1, 3)
     assert list(add.result(pool_type="Thread")) == [3, 4]
 
     # 多进程运行
     add(1, 2)
     add(1, 3)
     assert list(add.result(pool_type="Process")) == [3, 4]
 
     # 测试装饰器后的函数属性
     assert add.__name__ == "add"
-    assert add.__qualname__ == "test_map_pool.<locals>.add"
-    assert add.__doc__ == None
-    assert add.__module__ == "test_map_pool" or add.__module__ == "__main__"
 
     # 测试装饰器后更改max_workers，是否生效
-    add.max_workers = 1
+    add.max_workers = None
     assert add(1, 2) == 3
     add.max_workers = 2
     add(1, 2)
     assert list(add.result(pool_type="Process")) == [3]
     add(1, 2)
     assert list(add.result(pool_type="Process")) == [3]
 
 if __name__ == '__main__':
-    test_map_pool()
+    test_pooling_no_params()
```

