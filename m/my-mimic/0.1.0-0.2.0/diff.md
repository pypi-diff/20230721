# Comparing `tmp/my_mimic-0.1.0.tar.gz` & `tmp/my_mimic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_mimic-0.1.0.tar", max compression
+gzip compressed data, was "my_mimic-0.2.0.tar", max compression
```

## Comparing `my_mimic-0.1.0.tar` & `my_mimic-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-03-29 22:07:22.392076 my_mimic-0.1.0/LICENSE
--rw-r--r--   0        0        0     7984 2023-04-02 10:06:11.666414 my_mimic-0.1.0/README.md
--rw-r--r--   0        0        0      122 2023-04-02 09:59:52.109188 my_mimic-0.1.0/mr/__init__.py
--rw-r--r--   0        0        0      392 2023-04-02 09:59:52.109188 my_mimic-0.1.0/mr/config/__init__.py
--rw-r--r--   0        0        0     2562 2023-04-02 09:59:52.109188 my_mimic-0.1.0/mr/mime.py
--rw-r--r--   0        0        0        0 2023-04-02 09:59:52.109188 my_mimic-0.1.0/mr/states/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 09:59:52.109188 my_mimic-0.1.0/mr/states/implementations/__init__.py
--rw-r--r--   0        0        0     1140 2023-04-02 09:59:52.113188 my_mimic-0.1.0/mr/states/implementations/memory.py
--rw-r--r--   0        0        0     1073 2023-04-02 09:59:52.113188 my_mimic-0.1.0/mr/states/interface.py
--rw-r--r--   0        0        0      594 2023-04-02 10:06:30.919286 my_mimic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8824 1970-01-01 00:00:00.000000 my_mimic-0.1.0/setup.py
--rw-r--r--   0        0        0     8503 1970-01-01 00:00:00.000000 my_mimic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-02 10:14:35.846347 my_mimic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8803 2023-07-21 21:23:17.285047 my_mimic-0.2.0/README.md
+-rw-r--r--   0        0        0      177 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/config/__init__.py
+-rw-r--r--   0        0        0     2425 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/mime.py
+-rw-r--r--   0        0        0      326 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/states/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:50:05.481157 my_mimic-0.2.0/mr/states/implementations/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/states/implementations/memory.py
+-rw-r--r--   0        0        0     1955 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/states/implementations/redis.py
+-rw-r--r--   0        0        0     1141 2023-07-21 21:23:17.285047 my_mimic-0.2.0/mr/states/interface.py
+-rw-r--r--   0        0        0      874 2023-07-21 21:23:17.285047 my_mimic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9775 1970-01-01 00:00:00.000000 my_mimic-0.2.0/setup.py
+-rw-r--r--   0        0        0     9613 1970-01-01 00:00:00.000000 my_mimic-0.2.0/PKG-INFO
```

### Comparing `my_mimic-0.1.0/LICENSE` & `my_mimic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my_mimic-0.1.0/README.md` & `my_mimic-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         :param value: Any
         :param ttl: int. Seconds that the cache will have to live. Set None to never die
         :return:
         """
 
 ```
 
-To configure a new state you need to use `mr.Mime.set_config` function passing a config instance.
+To configure a new state you need to use `mr.Mime.set_config` function passing a config instance. The config accepts a `kwargs: dict` parameter, this parameter will be sent to the state instance. 
 
 ```python
 import mr
 
 class MyState(mr.IState):
     def sync_get(self, key: str):
         pass
@@ -100,17 +100,46 @@
 
     async def async_get(self, key: str):
         pass
 
     async def async_set(self, key: str, value: any, ttl: int = None):
         pass
 
-mr.Mime.set_config(config=mr.Config(state=MyState))
+mr.Mime.set_config(config=mr.Config(state=MyState, kwargs={"KEY": "value"}))
 ```
 
+### Extras
+
+For default a memory-state is allways set. But we also have extras states see below the list:
+
+#### Redis
+
+This extra add the redis [package](https://pypi.org/project/redis/) in version `^4.6.0`. All result will be `serialized` to be stored and `unserialized` to be returned using the [pickle lib](https://docs.python.org/3/library/pickle.html).
+
+How to install extra packages?
+
+```shell
+poetry add my-mimic -E redis_edition
+OR
+pip install 'my-mimic[redis_edition]'
+```
+
+You need pass the `REDIS_URL` parameter on configuration
+
+```python
+import mr
+mr.Mime.set_config(
+    config=mr.Config(
+        state=mr.states.RedisState, 
+        kwargs={"REDIS_URL": "redis://"}
+    )
+)
+```
+
+
 ### How to use
 
 For that we use `mr.Mime` as decorator that receive a ttl as argument. That means the ttl is the seconds that the cache will have to live. Set None to never die.
 
 Mime works fine with sync and async functions too.
 
 ```python
```

### Comparing `my_mimic-0.1.0/mr/mime.py` & `my_mimic-0.2.0/mr/mime.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,83 +6,75 @@
 import inspect
 from typing import TypeVar
 
 import meeseeks
 
 from mr.config import Config
 from mr.states.implementations.memory import MemoryState
-from mr.states.interface import IState
 
 T = TypeVar("T")
 
 
 singleton_container = meeseeks.OnlyOne(by_args_hash=True)
 
 
 @singleton_container
 class Mime:
     """
     Decorator to aplay cache/memoization on your functions
     """
 
     _config: Config = Config(state=MemoryState)
-    _state: IState = None
 
     @classmethod
     def set_config(cls, config: Config):
         """
         Replace the default config
 
         :param config: Config. IS a instance os Config class
         :return: None
         """
         cls._config = config
 
     def __init__(self, ttl: int = None):
         self._ttl = ttl
 
-    @classmethod
-    def _acquire_state(cls) -> IState:
-        if cls._state is None:
-            cls._state = cls._config.state()
-        return cls._state
-
     @staticmethod
     def _hash_args(args: tuple, kwargs: dict) -> str:
         """
         Created for each arg + kwargs hash. The kwargs`s order doesn't have influence
         """
         hash_args = [str(arg) for arg in args]
         hash_kwargs = [f"{str(key)}{str(arg)}" for key, arg in kwargs.items()]
         hash_kwargs.sort()
-        hash_instance = hashlib.sha1(f"{hash_args}{hash_kwargs}".encode())
+        hash_instance = hashlib.sha256(f"{hash_args}{hash_kwargs}".encode())
         return hash_instance.hexdigest()
 
     def __call__(self, function: T) -> T:
         is_async = inspect.iscoroutinefunction(function)
 
         if is_async:
 
             async def async_mimic(*args, **kwargs):
                 args_hash = self._hash_args(args=args, kwargs=kwargs)
-                state = self._acquire_state()
-                if cached_value := await state.async_get(key=args_hash):
-                    return cached_value
-                value = await function(*args, **kwargs)
-                await state.async_set(key=args_hash, value=value, ttl=self._ttl)
-                return value
+                async with self._config.async_acquire_state() as state:
+                    if cached_value := await state.async_get(key=args_hash):
+                        return cached_value
+                    value = await function(*args, **kwargs)
+                    await state.async_set(key=args_hash, value=value, ttl=self._ttl)
+                    return value
 
             mimic = async_mimic
         else:
 
             def sync_mimic(*args, **kwargs):
                 args_hash = self._hash_args(args=args, kwargs=kwargs)
-                state = self._acquire_state()
-                if cached_value := state.sync_get(key=args_hash):
-                    return cached_value
-                value = function(*args, **kwargs)
-                state.sync_set(key=args_hash, value=value, ttl=self._ttl)
-                return value
+                with self._config.sync_acquire_state() as state:
+                    if cached_value := state.sync_get(key=args_hash):
+                        return cached_value
+                    value = function(*args, **kwargs)
+                    state.sync_set(key=args_hash, value=value, ttl=self._ttl)
+                    return value
 
             mimic = sync_mimic
         mimic.__wrapped__ = function
         return mimic
```

### Comparing `my_mimic-0.1.0/mr/states/implementations/memory.py` & `my_mimic-0.2.0/mr/states/implementations/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 
 class MemoryState(IState):
     """
     State that use hash table to save cached returns
     """
 
-    def __init__(self):
+    def __init__(self, **kwargs):
+        self.kwargs = kwargs
         self._state = {}
 
     def sync_get(self, key: str):
         now_timestamp = datetime.utcnow().timestamp()
         if register := self._state.get(key):
             register_timestamp = register.get("created_at")
             ttl = register.get("ttl")
```

### Comparing `my_mimic-0.1.0/mr/states/interface.py` & `my_mimic-0.2.0/mr/states/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 class IState(ABC):
     """
     State interface
     """
 
     @abstractmethod
+    def __init__(self, **kwargs):
+        pass
+
+    @abstractmethod
     def sync_get(self, key: str):
         """
         Sync get implementation
         :param key: Str
         :return:
         """
```

### Comparing `my_mimic-0.1.0/setup.py` & `my_mimic-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['meeseeks-singleton>=0.4.2,<0.5.0']
 
+extras_require = \
+{'redis-edition': ['redis>=4.6.0,<5.0.0']}
+
 setup_kwargs = {
     'name': 'my-mimic',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Cache/Memoization package',
-    'long_description': '# My Mimic\n```\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣶⣶⣦⣄⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⢠⢊⢽⣝⡆⣫⣷⣌⣦⣤⡐⠾⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⣾⣯⣿⣯⣷⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⡠⢤⣜⠺⢟⡩⡇⢹⣉⡟⣰⠻⣯⢇⣿⣿⣿⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣾⣿⣿⣿⣿⣿⣿⣿⠿⠿⠿⠿⠷⠄⠀⠀⠀⠀⠀⠀⠀\n⢸⢰⣻⡟⣄⢈⣖⠹⢺⠰⠷⣏⢱⣾⣿⣿⣿⣿⣾⣿⣷⣶⣶⣤⣤⠠⠐⠂⠀⠀⠐⠒⠠⣄⣤⣤⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠁⠋⠳⣄⠫⡐⣉⠆⡓⢌⢂⢿⢹⣿⡛⢿⣿⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀⠀⠀⢀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠛⠻⠿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠈⡔⣡⠒⣸⠞⡌⢂⢎⣥⣷⣿⢨⣿⣿⣿⣿⡟⠁⡀⠀⠠⠀⡐⠀⠡⠀⠀⠀⢿⣿⣿⣿⣿⣿⣿⣿⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠸⣦⣳⡆⣞⣴⡿⠃⠀⠘⠛⠛⣿⣿⣿⡿⢀⡞⢣⡇⠀⡀⠰⡴⠟⡄⠆⢃⠘⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⢠⢛⢻⠏⠉⠀⠀⠀⠀⠀⠀⠙⠛⡫⢁⠸⡀⠸⠅⢀⠡⢸⡇⠘⡿⠀⠈⠘⡌⠛⠿⢿⡟⠉⠉⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⡜⠀⢸⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣟⡆⢠⠈⠁⢀⠂⠀⡀⠉⢒⠇⠠⢀⣭⣔⡩⢐⠂⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⢇⢀⡦⠀⠀⠀⠀⠀⠀⠀⢀⣀⠀⣯⡇⢀⡘⢷⣶⢶⠶⣶⣚⡟⡄⣴⠻⣭⣟⣷⡈⢒⣃⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⢸⡈⠐⠣⠄⣀⡀⠀⣠⡾⣩⢏⡼⣹⢏⣧⡂⠌⡌⠻⣉⠎⡑⢎⢧⡐⢯⣷⢳⡾⡝⣠⠿⣏⡟⣿⣟⣦⡄⠀⠀⣀⣀⡀⠤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠙⠦⠄⣐⡀⢀⠠⠉⠉⠘⡷⣎⢷⡹⣎⢷⡻⣖⢨⣑⣨⠘⢩⠘⠌⣃⠢⢉⣋⣵⠾⣍⢳⣬⣛⢶⣻⡮⡑⠆⠀⢀⣀⣠⠀⠈⡆⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⢱⣧⣥⣾⢿⡜⣯⢳⣝⢮⣳⡇⠁⠒⠤⢋⢏⢩⡙⢭⢉⠧⡈⣿⡝⣮⢳⢮⡝⣮⢷⣻⢾⡏⠉⠀⠀⠘⡦⠀⢹⡀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⡽⣯⠿⣽⣞⡷⣞⡷⣯⠛⠀⠀⣠⣤⠾⡶⣞⣤⣅⠂⠀⢻⣽⣎⣟⣮⡽⣯⢿⣹⡿⠀⠀⠀⠀⠀⠸⢄⣈⡇⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣽⣻⠷⣾⡽⣯⠟⠃⠀⢠⣾⢻⣬⢛⡵⢫⡞⣭⢻⡄⠀⠙⠾⣽⢾⣽⣳⡯⠛⠀⠀⠀⠀⠀⡠⠊⠉⠀⠈⠑⠢⡀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⣩⠁⠀⠀⠀⠀⣼⣇⡳⣌⠳⣜⢣⡞⣵⣫⢽⠀⠀⢀⠤⡉⠽⠀⠀⠀⠀⡠⠖⠂⠒⠁⠀⡀⠀⡀⠀⠀⣠⠭⡁⠉⡀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡅⡄⠀⠀⠀⢿⡲⣝⡬⣓⢮⡳⣝⢮⣳⢻⠀⡌⢃⢚⢰⠃⠀⠀⠀⠀⢧⢀⡰⠊⠙⣼⠁⡬⡄⢰⠦⢄⡁⠘⢫⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⡾⣻⢟⣿⣴⠠⢌⠻⣧⣻⣝⣮⣳⣏⡷⡽⣣⡵⣞⠿⣯⢿⣄⠀⠀⠀⠀⠀⠀⠀⠀⡠⠃⠀⡇⢸⠀⠑⢤⠐⠴⠞⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⣱⣟⣾⣳⣟⣷⡨⠒⣌⠱⡛⢚⠓⣛⢙⣰⣿⡹⣞⡽⣎⢷⣻⡄⠀⠀⠀⠀⠀⠀⠐⢧⣀⣠⠇⠘⠶⠀⠞⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠽⢷⣻⣞⣧⣟⡾⣽⠧⠣⢄⠣⡘⠤⡉⢤⠃⣼⣷⣻⢾⣵⣻⠞⠉⠓⠤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡄⠊⠁⠀⢀⣿⣞⣷⣫⣽⡞⠐⢣⣬⣆⣁⣢⣑⣢⣵⡞⣷⣯⣟⣾⣽⠂⣤⣀⠀⠀⢉⡔⠒⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⣴⠞⠉⠀⢠⣴⠞⠋⠉⠙⠛⠛⠉⠀⠀⠀⠀⠈⠉⠉⠉⠁⠀⠀⠈⠘⠛⠉⠁⠀⠀⠉⠛⠶⡏⠀⠀⠀⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⣎⠈⠐⠒⡖⣾⡉⢷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⣫⢭⠶⣋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠈⠳⠶⠹⢜⡱⡸⢌⡳⢄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⣈⢦⠓⡼⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣶⣄⡀⠈⠑⣇⡝⣌⣿⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣣⡛⡔⡻⣄⠀⠀⠀⠀⠀⣀⡀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⠛⢻⣷⣤⣾⣿⣿⣿⣿⣿⡿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⣷⣌⣱⣿⣷⣄⡀⣠⣾⣿⢿⣧⡀⠀\n⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠺⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣾⣿⣻⣷⡀\n⠀⠀⠀⠀⠀⠀⠀⠙⠿⣿⣿⣿⣿⣿⣿⡿⠟⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠛⢿⣿⣿⣿⣟⣿⣻⣽⣳⣯⣿⠇\n⠀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠉⠉⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠛⠛⠛⠻⠷⠿⠷⠟⠋⠀\n                                                                            By CenturyBoys\n```\n\n\nMy Mimic is a function decorator for cache/memoization. They use the args and kwargs to create a hash to storage the function call result after the first call all function invoke will use already storage result.  \n\n### Configuration\n\nUsing `mr.Mime` from Mimic allowed you to use the default config or create a self one. By default, an in-memory state are used you can implement your own state resolver using the interface IState.\n\nBelow you can see the interface contract\n```python\nfrom abc import ABC, abstractmethod\n\nclass IState(ABC):\n    """\n    State interface\n    """\n\n    @abstractmethod\n    def sync_get(self, key: str):\n        """\n        Sync get implementation\n        :param key: Str\n        :return:\n        """\n\n    @abstractmethod\n    def sync_set(self, key: str, value: any, ttl: int = None):\n        """\n        Sync set implementation\n        :param key: Str\n        :param value: Any\n        :param ttl: int. Seconds that the cache will have to live. Set None to never die\n        :return:\n        """\n\n    @abstractmethod\n    async def async_get(self, key: str):\n        """\n        Async get implementation\n        :param key: Str\n        :return:\n        """\n\n    @abstractmethod\n    async def async_set(self, key: str, value: any, ttl: int = None):\n        """\n        Async set implementation\n        :param key: Str\n        :param value: Any\n        :param ttl: int. Seconds that the cache will have to live. Set None to never die\n        :return:\n        """\n\n```\n\nTo configure a new state you need to use `mr.Mime.set_config` function passing a config instance.\n\n```python\nimport mr\n\nclass MyState(mr.IState):\n    def sync_get(self, key: str):\n        pass\n\n    def sync_set(self, key: str, value: any, ttl: int = None):\n        pass\n\n    async def async_get(self, key: str):\n        pass\n\n    async def async_set(self, key: str, value: any, ttl: int = None):\n        pass\n\nmr.Mime.set_config(config=mr.Config(state=MyState))\n```\n\n### How to use\n\nFor that we use `mr.Mime` as decorator that receive a ttl as argument. That means the ttl is the seconds that the cache will have to live. Set None to never die.\n\nMime works fine with sync and async functions too.\n\n```python\nimport time\nimport mr\n\n@mr.Mime(ttl=1)\ndef cached_callback(param_a: int, param_b: int):\n    print("Function was called")\n    return param_a + param_b\n\nresult = cached_callback(1, 2)\nprint(result)\nresult = cached_callback(1, 2)\nprint(result)\ntime.sleep(2)\nprint("Await 2 seconds")\nresult = cached_callback(1, 2)\nprint(result)\n```\nThe output will be\n\n```bash\nFunction was called\n3\n3\nAwait 2 seconds\nFunction was called\n3\n```',
+    'long_description': '# My Mimic\n```\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣶⣶⣦⣄⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⢠⢊⢽⣝⡆⣫⣷⣌⣦⣤⡐⠾⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⣾⣯⣿⣯⣷⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⡠⢤⣜⠺⢟⡩⡇⢹⣉⡟⣰⠻⣯⢇⣿⣿⣿⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣾⣿⣿⣿⣿⣿⣿⣿⠿⠿⠿⠿⠷⠄⠀⠀⠀⠀⠀⠀⠀\n⢸⢰⣻⡟⣄⢈⣖⠹⢺⠰⠷⣏⢱⣾⣿⣿⣿⣿⣾⣿⣷⣶⣶⣤⣤⠠⠐⠂⠀⠀⠐⠒⠠⣄⣤⣤⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠁⠋⠳⣄⠫⡐⣉⠆⡓⢌⢂⢿⢹⣿⡛⢿⣿⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀⠀⠀⢀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠛⠻⠿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠈⡔⣡⠒⣸⠞⡌⢂⢎⣥⣷⣿⢨⣿⣿⣿⣿⡟⠁⡀⠀⠠⠀⡐⠀⠡⠀⠀⠀⢿⣿⣿⣿⣿⣿⣿⣿⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠸⣦⣳⡆⣞⣴⡿⠃⠀⠘⠛⠛⣿⣿⣿⡿⢀⡞⢣⡇⠀⡀⠰⡴⠟⡄⠆⢃⠘⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⢠⢛⢻⠏⠉⠀⠀⠀⠀⠀⠀⠙⠛⡫⢁⠸⡀⠸⠅⢀⠡⢸⡇⠘⡿⠀⠈⠘⡌⠛⠿⢿⡟⠉⠉⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⡜⠀⢸⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣟⡆⢠⠈⠁⢀⠂⠀⡀⠉⢒⠇⠠⢀⣭⣔⡩⢐⠂⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⢇⢀⡦⠀⠀⠀⠀⠀⠀⠀⢀⣀⠀⣯⡇⢀⡘⢷⣶⢶⠶⣶⣚⡟⡄⣴⠻⣭⣟⣷⡈⢒⣃⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⢸⡈⠐⠣⠄⣀⡀⠀⣠⡾⣩⢏⡼⣹⢏⣧⡂⠌⡌⠻⣉⠎⡑⢎⢧⡐⢯⣷⢳⡾⡝⣠⠿⣏⡟⣿⣟⣦⡄⠀⠀⣀⣀⡀⠤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠙⠦⠄⣐⡀⢀⠠⠉⠉⠘⡷⣎⢷⡹⣎⢷⡻⣖⢨⣑⣨⠘⢩⠘⠌⣃⠢⢉⣋⣵⠾⣍⢳⣬⣛⢶⣻⡮⡑⠆⠀⢀⣀⣠⠀⠈⡆⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⢱⣧⣥⣾⢿⡜⣯⢳⣝⢮⣳⡇⠁⠒⠤⢋⢏⢩⡙⢭⢉⠧⡈⣿⡝⣮⢳⢮⡝⣮⢷⣻⢾⡏⠉⠀⠀⠘⡦⠀⢹⡀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⡽⣯⠿⣽⣞⡷⣞⡷⣯⠛⠀⠀⣠⣤⠾⡶⣞⣤⣅⠂⠀⢻⣽⣎⣟⣮⡽⣯⢿⣹⡿⠀⠀⠀⠀⠀⠸⢄⣈⡇⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣽⣻⠷⣾⡽⣯⠟⠃⠀⢠⣾⢻⣬⢛⡵⢫⡞⣭⢻⡄⠀⠙⠾⣽⢾⣽⣳⡯⠛⠀⠀⠀⠀⠀⡠⠊⠉⠀⠈⠑⠢⡀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⣩⠁⠀⠀⠀⠀⣼⣇⡳⣌⠳⣜⢣⡞⣵⣫⢽⠀⠀⢀⠤⡉⠽⠀⠀⠀⠀⡠⠖⠂⠒⠁⠀⡀⠀⡀⠀⠀⣠⠭⡁⠉⡀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡅⡄⠀⠀⠀⢿⡲⣝⡬⣓⢮⡳⣝⢮⣳⢻⠀⡌⢃⢚⢰⠃⠀⠀⠀⠀⢧⢀⡰⠊⠙⣼⠁⡬⡄⢰⠦⢄⡁⠘⢫⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⡾⣻⢟⣿⣴⠠⢌⠻⣧⣻⣝⣮⣳⣏⡷⡽⣣⡵⣞⠿⣯⢿⣄⠀⠀⠀⠀⠀⠀⠀⠀⡠⠃⠀⡇⢸⠀⠑⢤⠐⠴⠞⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⣱⣟⣾⣳⣟⣷⡨⠒⣌⠱⡛⢚⠓⣛⢙⣰⣿⡹⣞⡽⣎⢷⣻⡄⠀⠀⠀⠀⠀⠀⠐⢧⣀⣠⠇⠘⠶⠀⠞⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠽⢷⣻⣞⣧⣟⡾⣽⠧⠣⢄⠣⡘⠤⡉⢤⠃⣼⣷⣻⢾⣵⣻⠞⠉⠓⠤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡄⠊⠁⠀⢀⣿⣞⣷⣫⣽⡞⠐⢣⣬⣆⣁⣢⣑⣢⣵⡞⣷⣯⣟⣾⣽⠂⣤⣀⠀⠀⢉⡔⠒⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠀⣴⠞⠉⠀⢠⣴⠞⠋⠉⠙⠛⠛⠉⠀⠀⠀⠀⠈⠉⠉⠉⠁⠀⠀⠈⠘⠛⠉⠁⠀⠀⠉⠛⠶⡏⠀⠀⠀⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⣎⠈⠐⠒⡖⣾⡉⢷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⣫⢭⠶⣋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⠈⠳⠶⠹⢜⡱⡸⢌⡳⢄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⣈⢦⠓⡼⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣶⣄⡀⠈⠑⣇⡝⣌⣿⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣣⡛⡔⡻⣄⠀⠀⠀⠀⠀⣀⡀⠀⠀⠀\n⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⠛⢻⣷⣤⣾⣿⣿⣿⣿⣿⡿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⣷⣌⣱⣿⣷⣄⡀⣠⣾⣿⢿⣧⡀⠀\n⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠺⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣾⣿⣻⣷⡀\n⠀⠀⠀⠀⠀⠀⠀⠙⠿⣿⣿⣿⣿⣿⣿⡿⠟⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠛⢿⣿⣿⣿⣟⣿⣻⣽⣳⣯⣿⠇\n⠀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠉⠉⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠛⠛⠛⠻⠷⠿⠷⠟⠋⠀\n                                                                            By CenturyBoys\n```\n\n\nMy Mimic is a function decorator for cache/memoization. They use the args and kwargs to create a hash to storage the function call result after the first call all function invoke will use already storage result.  \n\n### Configuration\n\nUsing `mr.Mime` from Mimic allowed you to use the default config or create a self one. By default, an in-memory state are used you can implement your own state resolver using the interface IState.\n\nBelow you can see the interface contract\n```python\nfrom abc import ABC, abstractmethod\n\nclass IState(ABC):\n    """\n    State interface\n    """\n\n    @abstractmethod\n    def sync_get(self, key: str):\n        """\n        Sync get implementation\n        :param key: Str\n        :return:\n        """\n\n    @abstractmethod\n    def sync_set(self, key: str, value: any, ttl: int = None):\n        """\n        Sync set implementation\n        :param key: Str\n        :param value: Any\n        :param ttl: int. Seconds that the cache will have to live. Set None to never die\n        :return:\n        """\n\n    @abstractmethod\n    async def async_get(self, key: str):\n        """\n        Async get implementation\n        :param key: Str\n        :return:\n        """\n\n    @abstractmethod\n    async def async_set(self, key: str, value: any, ttl: int = None):\n        """\n        Async set implementation\n        :param key: Str\n        :param value: Any\n        :param ttl: int. Seconds that the cache will have to live. Set None to never die\n        :return:\n        """\n\n```\n\nTo configure a new state you need to use `mr.Mime.set_config` function passing a config instance. The config accepts a `kwargs: dict` parameter, this parameter will be sent to the state instance. \n\n```python\nimport mr\n\nclass MyState(mr.IState):\n    def sync_get(self, key: str):\n        pass\n\n    def sync_set(self, key: str, value: any, ttl: int = None):\n        pass\n\n    async def async_get(self, key: str):\n        pass\n\n    async def async_set(self, key: str, value: any, ttl: int = None):\n        pass\n\nmr.Mime.set_config(config=mr.Config(state=MyState, kwargs={"KEY": "value"}))\n```\n\n### Extras\n\nFor default a memory-state is allways set. But we also have extras states see below the list:\n\n#### Redis\n\nThis extra add the redis [package](https://pypi.org/project/redis/) in version `^4.6.0`. All result will be `serialized` to be stored and `unserialized` to be returned using the [pickle lib](https://docs.python.org/3/library/pickle.html).\n\nHow to install extra packages?\n\n```shell\npoetry add my-mimic -E redis_edition\nOR\npip install \'my-mimic[redis_edition]\'\n```\n\nYou need pass the `REDIS_URL` parameter on configuration\n\n```python\nimport mr\nmr.Mime.set_config(\n    config=mr.Config(\n        state=mr.states.RedisState, \n        kwargs={"REDIS_URL": "redis://"}\n    )\n)\n```\n\n\n### How to use\n\nFor that we use `mr.Mime` as decorator that receive a ttl as argument. That means the ttl is the seconds that the cache will have to live. Set None to never die.\n\nMime works fine with sync and async functions too.\n\n```python\nimport time\nimport mr\n\n@mr.Mime(ttl=1)\ndef cached_callback(param_a: int, param_b: int):\n    print("Function was called")\n    return param_a + param_b\n\nresult = cached_callback(1, 2)\nprint(result)\nresult = cached_callback(1, 2)\nprint(result)\ntime.sleep(2)\nprint("Await 2 seconds")\nresult = cached_callback(1, 2)\nprint(result)\n```\nThe output will be\n\n```bash\nFunction was called\n3\n3\nAwait 2 seconds\nFunction was called\n3\n```',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `my_mimic-0.1.0/PKG-INFO` & `my_mimic-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: my-mimic
-Version: 0.1.0
+Version: 0.2.0
 Summary: Cache/Memoization package
 License: Apache-2.0
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: redis-edition
 Requires-Dist: meeseeks-singleton (>=0.4.2,<0.5.0)
+Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "redis-edition"
+Project-URL: documentation, https://github.com/CenturyBoys/my-mimic
+Project-URL: homepage, https://github.com/CenturyBoys/my-mimic
+Project-URL: repository, https://github.com/CenturyBoys/my-mimic
 Description-Content-Type: text/markdown
 
 # My Mimic
 ```
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣶⣶⣦⣄⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⠀⠀⢠⢊⢽⣝⡆⣫⣷⣌⣦⣤⡐⠾⣿⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⣾⣯⣿⣯⣷⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⡠⢤⣜⠺⢟⡩⡇⢹⣉⡟⣰⠻⣯⢇⣿⣿⣿⣦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣾⣿⣿⣿⣿⣿⣿⣿⠿⠿⠿⠿⠷⠄⠀⠀⠀⠀⠀⠀⠀
@@ -97,15 +102,15 @@
         :param value: Any
         :param ttl: int. Seconds that the cache will have to live. Set None to never die
         :return:
         """
 
 ```
 
-To configure a new state you need to use `mr.Mime.set_config` function passing a config instance.
+To configure a new state you need to use `mr.Mime.set_config` function passing a config instance. The config accepts a `kwargs: dict` parameter, this parameter will be sent to the state instance. 
 
 ```python
 import mr
 
 class MyState(mr.IState):
     def sync_get(self, key: str):
         pass
@@ -115,17 +120,46 @@
 
     async def async_get(self, key: str):
         pass
 
     async def async_set(self, key: str, value: any, ttl: int = None):
         pass
 
-mr.Mime.set_config(config=mr.Config(state=MyState))
+mr.Mime.set_config(config=mr.Config(state=MyState, kwargs={"KEY": "value"}))
 ```
 
+### Extras
+
+For default a memory-state is allways set. But we also have extras states see below the list:
+
+#### Redis
+
+This extra add the redis [package](https://pypi.org/project/redis/) in version `^4.6.0`. All result will be `serialized` to be stored and `unserialized` to be returned using the [pickle lib](https://docs.python.org/3/library/pickle.html).
+
+How to install extra packages?
+
+```shell
+poetry add my-mimic -E redis_edition
+OR
+pip install 'my-mimic[redis_edition]'
+```
+
+You need pass the `REDIS_URL` parameter on configuration
+
+```python
+import mr
+mr.Mime.set_config(
+    config=mr.Config(
+        state=mr.states.RedisState, 
+        kwargs={"REDIS_URL": "redis://"}
+    )
+)
+```
+
+
 ### How to use
 
 For that we use `mr.Mime` as decorator that receive a ttl as argument. That means the ttl is the seconds that the cache will have to live. Set None to never die.
 
 Mime works fine with sync and async functions too.
 
 ```python
```

