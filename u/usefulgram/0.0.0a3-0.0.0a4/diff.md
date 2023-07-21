# Comparing `tmp/usefulgram-0.0.0a3.tar.gz` & `tmp/usefulgram-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a3.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0a4.tar", max compression
```

## Comparing `usefulgram-0.0.0a3.tar` & `usefulgram-0.0.0a4.tar`

### file list

```diff
@@ -1,56 +1,28 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a3/LICENSE
--rw-r--r--   0        0        0      735 2023-07-12 23:25:02.804630 usefulgram-0.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     2252 2023-07-07 21:36:03.207522 usefulgram-0.0.0a3/README.md
--rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a3/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a3/usefulgram/enums/__init__.py
--rw-r--r--   0        0        0      192 2023-06-18 20:21:06.663801 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      207 2023-07-12 20:52:05.669860 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      626 2023-06-25 23:36:03.804852 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-310.pyc
--rw-r--r--   0        0        0      825 2023-07-12 20:52:05.670858 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-311.pyc
--rw-r--r--   0        0        0      300 2023-06-25 20:25:25.579092 usefulgram-0.0.0a3/usefulgram/enums/const.py
--rw-r--r--   0        0        0      170 2023-07-07 21:21:58.932059 usefulgram-0.0.0a3/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      348 2023-06-19 16:50:03.414405 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      412 2023-07-12 20:52:05.683100 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      525 2023-06-19 16:50:03.415402 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      697 2023-07-12 20:52:05.686587 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0      457 2023-06-19 16:49:59.041300 usefulgram-0.0.0a3/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a3/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      400 2023-07-12 20:52:05.690132 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2023-07-12 20:52:05.694121 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/database_filters.cpython-311.pyc
--rw-r--r--   0        0        0     6545 2023-07-12 23:43:20.285814 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/parse_filters.cpython-311.pyc
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a3/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     4056 2023-07-12 23:43:19.426659 usefulgram-0.0.0a3/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0       60 2023-07-07 21:21:58.951007 usefulgram-0.0.0a3/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0      255 2023-07-01 22:52:11.609139 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      285 2023-07-12 20:52:05.671855 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4586 2023-07-01 22:56:43.331106 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0        0        0     8156 2023-07-12 22:54:24.105242 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2023-07-12 22:54:23.162090 usefulgram-0.0.0a3/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a3/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0      203 2023-06-25 23:40:11.949558 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      219 2023-07-12 20:52:04.890650 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5110 2023-06-25 23:40:11.952550 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-310.pyc
--rw-r--r--   0        0        0     9884 2023-07-12 21:45:25.379199 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-311.pyc
--rw-r--r--   0        0        0     9580 2023-07-12 21:45:25.228138 usefulgram-0.0.0a3/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a3/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0      297 2023-07-12 20:52:05.696116 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1802 2023-07-12 20:52:05.697113 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/stacker.cpython-311.pyc
--rw-r--r--   0        0        0     2783 2023-07-12 21:45:26.170753 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/trottling.cpython-311.pyc
--rw-r--r--   0        0        0      847 2023-06-25 23:39:58.644717 usefulgram-0.0.0a3/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1505 2023-07-12 21:45:25.238959 usefulgram-0.0.0a3/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a3/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0      210 2023-07-01 22:52:11.613096 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-07-12 20:52:05.678130 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2658 2023-06-25 23:36:03.801859 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-310.pyc
--rw-r--r--   0        0        0     4860 2023-07-12 23:37:41.723037 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-311.pyc
--rw-r--r--   0        0        0     2676 2023-07-01 22:52:11.616112 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-310.pyc
--rw-r--r--   0        0        0     4281 2023-07-12 21:45:26.163773 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-311.pyc
--rw-r--r--   0        0        0     2803 2023-07-12 23:37:40.829073 usefulgram-0.0.0a3/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2514 2023-07-12 21:45:25.242944 usefulgram-0.0.0a3/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0       52 2023-06-18 09:35:26.952475 usefulgram-0.0.0a3/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0      198 2023-06-18 09:35:27.816247 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      230 2023-07-12 20:52:05.687137 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      559 2023-06-18 09:36:47.317788 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-310.pyc
--rw-r--r--   0        0        0      909 2023-07-12 20:52:05.689134 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-311.pyc
--rw-r--r--   0        0        0      233 2023-06-18 09:36:46.396163 usefulgram-0.0.0a3/usefulgram/utils/autorepr.py
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 usefulgram-0.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a4/LICENSE
+-rw-r--r--   0        0        0      751 2023-07-20 13:00:49.747638 usefulgram-0.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a4/README.md
+-rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a4/usefulgram/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a4/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a4/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a4/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a4/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a4/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a4/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     5991 2023-07-20 23:26:12.344647 usefulgram-0.0.0a4/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a4/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0     3615 2023-07-20 21:15:40.376031 usefulgram-0.0.0a4/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a4/usefulgram/keyboard/buttons.py
+-rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a4/usefulgram/keyboard/rows.py
+-rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a4/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a4/usefulgram/lazy/editor.py
+-rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a4/usefulgram/lazy/lazy_editing.py
+-rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a4/usefulgram/lazy/sender.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a4/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a4/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a4/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a4/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a4/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a4/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0       52 2023-06-18 09:35:26.952475 usefulgram-0.0.0a4/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-18 09:36:46.396163 usefulgram-0.0.0a4/usefulgram/utils/autorepr.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a4/PKG-INFO
```

### Comparing `usefulgram-0.0.0a3/LICENSE` & `usefulgram-0.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a3/pyproject.toml` & `usefulgram-0.0.0a4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a3"
+version = "0.0.0a4"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-aiogram = "^3.0.0b5"
+python = "^3.9"
+aiogram = "^3.0.0b8"
 cachetools ="^4.0.0"
-pydantic ="^1.10.7"
+pydantic ="^2.0.0"
+pytz ="^2020.3"
 
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Sethis/usefulgram/issues"
```

### Comparing `usefulgram-0.0.0a3/README.md` & `usefulgram-0.0.0a4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # Usefulgram
 
+### Как скачать? 
+Всё просто - достаточно ввести `pip install usefulgram`
+
 ### Немного истории 
 aiogram - прекрасный фреймворк. Однако при работе с ним я столкнулся с тем, 
 что переношу многие функции и классы из проекта в проект. Сначала, 
 для удобной транспортировки были созданы общие классы, затем это перосло
 в общую папку, а теперь - в отдельный проект. Надеюсь, что данная
 небольшая надстройка станет полезным инструментом не только мне, но  и вам
 
 ### Какие изменения?
 В целом, usefulgram нельзя расценивать как что-то независимое. Это
 надстройка, собирающая в себя множество маленьких, но полезных утилит.
 Основные измения:
-- lazyediting - класс для удобного изменения сообщений в callback хендлерах
-- Builder, Row, Button и ReplyButton - классы для представления клавиатуры 
+- lazyediting - класс для удобного изменения сообщений в callback хендлерах.
+Настолько удобен, что я считаю его главной киллер-фичей
+- Builder, Row, Button и Reply аналоги - классы для представления клавиатуры 
 в массивно-подобном виде
 - BasePydanticFilter - Базовый класс, несколько развитая версия
 CallbackFactory, способная на type hints и несколько более обширный список
-типов
+типов. Незаменим при использовании вместе с плагином для pydantic подсказок
+в вашу IDE
 - TrottlingMiddleware - Класс, позволяющий не допустить спам. Немного 
 изменённая версия [данного кода](https://github.com/wakaree/simple_echo_bot/blob/main/middlewares/throttling.py)
 - StackerMiddleware - Класс, добавляющий все эти классы в функции
+- И многое, многое другое!
 
 #### Пример использования:
-В разработке
+На данный момент существует единственный, но при этом почти полный пример 
+использования. Найти его можно в **examples -> fully_example**
+
+#### Документация: 
+_В разработке и скоро будет доступна_
 
 ### Roadmap
-- Добавить пример использования
+- Добавить больше примеров использования
 - Перевести все тексты в библиотеке на английский
 - Добавить документацию
 - Добавить больше комментариев в код
-- Улучшить код
+- Улучшить код ✔️ - 80% библиотеки было переписано
```

### Comparing `usefulgram-0.0.0a3/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0a4/usefulgram/filters/database_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a3/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0a4/usefulgram/filters/parse_filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,108 @@
 
 
 from typing import Optional, Union, Dict, Any, Tuple
+from abc import ABC
 
 from pydantic import BaseModel
 
 from aiogram.filters import BaseFilter
 from aiogram.types import CallbackQuery
 
+from aiogram.filters.magic_data import MagicData
+from aiogram.utils.magic_filter import MagicFilter
+
 from usefulgram.parsing.decode import DecodeCallbackData
+from usefulgram.exceptions import UndefinedMagicFilterModel
+
+
+class _BaseMagicFilter(ABC):
+    _magic_filter: Optional[tuple[MagicFilter]] = None
+
+    def filter(self, *args: MagicFilter):
+        self.__setattr__("_magic_filter", args)
+
+        return self
+
+    @staticmethod
+    async def _ckeck_magic_filter(
+            callback: CallbackQuery,
+            magic_filter: tuple[MagicFilter],
+            values: Optional[tuple[Any, ...]] = None,
+            model: Optional[dict[Any, Any]] = None
+    ) -> bool:
+
+        for filter_obj in magic_filter:
+            filter_instance = MagicData(filter_obj)
+
+            if values is not None:
+                result = await filter_instance(callback, *values)
+
+            elif model is not None:
+                result = await filter_instance(callback, **model)
+
+            else:
+                raise UndefinedMagicFilterModel
 
+            if not result:
+                return False
+
+        return True
 
-class BasePydanticFilter(BaseFilter, BaseModel):
-    prefix: Optional[str]
+    def get_magic_filter(self) -> Any:
+        try:
+            return self.__getattribute__("_magic_filter")
 
+        except AttributeError:
+            return None
+
+
+class _BaseDataclassesFilter(_BaseMagicFilter, ABC):
     async def __call__(
-            self, _callback: CallbackQuery,
-            decoder: DecodeCallbackData,
-            united: Optional[bool] = False) -> Union[bool, Dict[str, Any]]:
+            self,
+            callback: CallbackQuery,
+            decoder: DecodeCallbackData) -> Union[bool, Dict[str, Any]]:
 
         try:
-            callback_data = decoder.to_format(type(self), add_prefix=True)
+            callback_data_model = decoder.to_format(type(self), add_prefix=True)
 
         except (AttributeError, ValueError, IndexError):
             return False
 
-        for item_name in self.__fields__.keys():
-            result = self.__getattribute__(item_name)
+        for item_name in self.__annotations__.keys():
+            if item_name == "_magic_filter":
+                continue
+
+            filter_value = self.__getattribute__(item_name)
 
-            if result is None:
+            if filter_value is None:
                 continue
 
-            if callback_data.__getattribute__(item_name) != result:
+            data_value = callback_data_model.__getattribute__(item_name)
+
+            if data_value != filter_value:
                 return False
 
-        if united:
-            return decoder.class_to_dict(callback_data)
+        magic_filter: Optional[tuple[MagicFilter]] = super().get_magic_filter()
 
-        if len(callback_data.__annotations__) == len(decoder.additional):
-            return decoder.class_to_dict(callback_data)
+        if magic_filter is not None:
+            if await self._ckeck_magic_filter(
+                callback=callback,
+                magic_filter=magic_filter,
+                model=decoder.class_to_dict(callback_data_model)
+            ):
+                return decoder.class_to_dict(callback_data_model)
 
-        return False
+            return False
+
+        return decoder.class_to_dict(callback_data_model)
+
+
+class BasePydanticFilter(_BaseDataclassesFilter, BaseModel, BaseFilter):
+    prefix: Optional[str] = None
 
 
 class CallbackPrefixFilter(BaseFilter):
     def __init__(self, prefix: str):
         """
 
         :param prefix: first argument in callback data
@@ -55,101 +114,111 @@
 
         if self.prefix == decoder.prefix:
             return True
 
         return False
 
 
-class ItarationFilter(BaseFilter):
+class ItarationFilter(_BaseMagicFilter):
     def __init__(self, item_number: int = 0):
         self._item_number: int = item_number
         self._operation: Optional[Tuple[str, Any]] = None
         self._error_result: bool = False
 
     def __getitem__(self, item: int):
         self._item_number = item
 
+        return self
+
     @staticmethod
     def _convert(other: str) -> Optional[int]:
         try:
             return int(other)
 
         except ValueError:
             return None
 
     def __eq__(self, other: Any):
         self._operation = ("eq", other)
 
+        return self
+
     def __ne__(self, other: Any):
         self._operation = ("ne", other)
 
-    def __lt__(self, other: Any):
-        int_other = self._convert(other)
-
-        if int_other is None:
-            self._error_result = True
+        return self
 
-            return
+    def __lt__(self, other: Any):
+        self._operation = ("lt", other)
 
-        self._operation = ("lt", int_other)
+        return self
 
     def __gt__(self, other: Any):
-        int_other = self._convert(other)
-
-        if int_other is None:
-            self._error_result = True
+        self._operation = ("gt", other)
 
-            return
-
-        self._operation = ("gt", int_other)
+        return self
 
     def __le__(self, other: Any):
-        int_other = self._convert(other)
-
-        if int_other is None:
-            self._error_result = True
-
-            return
+        self._operation = ("le", other)
 
-        self._operation = ("le", int_other)
+        return self
 
     def __ge__(self, other: Any):
-        int_other = self._convert(other)
-
-        if int_other is None:
-            self._error_result = True
-
-            return
+        self._operation = ("ge", other)
 
-        self._operation = ("ge", int_other)
+        return self
 
     @staticmethod
     def _do_operation(operation: str, first_item: Any, second_item: Any):
         if operation == "eq":
             return first_item == second_item
 
         if operation == "ne":
             return first_item != second_item
 
+        first_item = ItarationFilter._convert(first_item)
+
+        if first_item is False:
+            return False
+
         if operation == "lt":
             return first_item < second_item
 
         if operation == "gt":
             return first_item > second_item
 
         if operation == "le":
             return first_item <= second_item
 
         if operation == "ge":
             return first_item >= second_item
 
-    async def __call__(self, _callback: CallbackQuery,
-                       decoder: DecodeCallbackData):
+    async def __call__(
+            self, callback: CallbackQuery,
+            decoder: DecodeCallbackData
+    ):
+
+        magic_filter: Optional[tuple[MagicFilter]] = super().get_magic_filter()
 
         if self._error_result:
             return False
 
-        first_item = (decoder.prefix, decoder.additional)[self._item_number]
+        values = (decoder.prefix, *decoder.additional)
+
+        first_item = values[self._item_number]
+
+        if magic_filter is not None:
+            if await self._ckeck_magic_filter(
+                    callback=callback,
+                    magic_filter=magic_filter,
+                    values=values
+            ):
+                return True
+
+            return False
+
+        if self._operation is None:
+            return False
 
         operation, second_item = self._operation
 
         return self._do_operation(operation, first_item, second_item)
```

### Comparing `usefulgram-0.0.0a3/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0a4/usefulgram/middlewares/trottling.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if user is not None:
             if user.id in self._cache:
                 self._cache[user.id] = None
 
                 if isinstance(event, CallbackQuery):
                     return await self.trottling_answer(self._answer_text, event)
 
-                return
+                return None
 
             self._cache[user.id] = None
 
         return await handler(event, data)
 
     @staticmethod
     async def trottling_answer(text: str, callback: CallbackQuery):
```

### Comparing `usefulgram-0.0.0a3/usefulgram/parsing/decode.py` & `usefulgram-0.0.0a4/usefulgram/parsing/encode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,116 @@
 
 
-from typing import Union
-from datetime import datetime, date, time
+import sys
 
-from usefulgram.enums import Const
+from typing import Any
+
+from enum import Enum
+from decimal import Decimal
 
-from pydantic import BaseModel
-from dataclasses import dataclass
+from datetime import date, time, datetime
 
+from usefulgram.exceptions import TooMoreCharacters, RecursionObjectParse
+from usefulgram.enums import Const
 
-class DecodeCallbackData:
-    prefix: str
-    additional: list[str]
 
+class _Additional:
     @staticmethod
-    def _parse(callback_data: str, separator: str) -> tuple[str, list[str]]:
-        split_data = callback_data.split(separator)
+    def _add_separator(item: str, separator: str = "&") -> str:
+        return f"{item}{separator}"
 
-        additional = split_data[1].split("&")
+    def _object_to_str(self, item: object) -> str:
+        annotations_keys = list(item.__annotations__.keys())
 
-        return split_data[0], additional
+        result = ""
 
-    def __init__(self, callback_data: str, separator: str = "/"):
-        self.prefix, self.additional = self._parse(callback_data, separator)
+        for key in annotations_keys:
+            if key == "prefix":
+                continue
 
-    def _convert_str_to_type(self, obj_value: str, obj_type: Union[type, object]):
-        if obj_value == "None":
-            return None
+            values = item.__getattribute__(f"{key}")
 
-        if not isinstance(obj_type, type):
-            optional_type = obj_type.__getattribute__("__args__")[0]
+            string_value = self._to_str(values, is_recursion=True)
 
-            return self._convert_str_to_type(obj_value, optional_type)
+            result += self._add_separator(string_value)
 
-        if issubclass(obj_type, datetime):
-            return datetime.strptime(obj_value, Const.DATETIME_FORMAT)
+        return result[:-1]
 
-        if issubclass(obj_type, date):
-            return datetime.strptime(obj_value, Const.DATETIME_FORMAT).date()
+    def _to_str(self, item: Any, is_recursion: bool = False) -> str:
+        if item is None:
+            return ""
 
-        if issubclass(obj_type, time):
-            return datetime.strptime(obj_value, Const.DATETIME_FORMAT).time()
+        if isinstance(item, bool):
+            return str(int(item))
 
-        if issubclass(obj_type, bool):
-            if obj_value == "False":
-                return False
+        if isinstance(item, str):
+            return item
 
-        return obj_type(obj_value)
+        if isinstance(item, (int, float, Decimal)):
+            return str(item)
 
-    def _iter_key_and_type(
-            self, keys: list[str], objects_type: list[type],
-            add_prefix: bool
-    ) -> dict[str, type]:
+        if isinstance(item, (datetime, date, time)):
+            return item.strftime(Const.DATETIME_FORMAT)
 
-        return_param = {}
+        if isinstance(item, Enum):
+            return item.name
 
-        if add_prefix:
-            return_param["prefix"] = self.prefix
+        if is_recursion:
+            raise RecursionObjectParse
 
-        additional_value = 0
+        try:
+            return self._object_to_str(item)
 
-        for key, obj_type in zip(keys, objects_type):
-            if key == "prefix":
-                return_param[key] = self._convert_str_to_type(self.prefix, obj_type)
+        except AttributeError:
+            return f"{item}"
 
-                continue
+    def __call__(self, *args: Any) -> str:
+        if args == ():
+            return ""
 
-            return_param[key] = self._convert_str_to_type(
-                self.additional[additional_value], obj_type
-            )
+        result = ""
 
-            additional_value += 1
+        for item in args:
+            result += self._add_separator(self._to_str(item))
 
-        return return_param
+        result = result[:-1]
 
-    def to_format(self, format_objects: type, add_prefix: bool = False) -> Union[BaseModel, dataclass]:
-        annotations = format_objects.__annotations__
+        return result
 
-        keys = list(annotations.keys())
-        values = list(annotations.values())
 
-        obj_params = self._iter_key_and_type(keys, values, add_prefix)
+class _CallbackData:
+    @staticmethod
+    def _get_str_callback_data(
+            prefix: str, additional: str, separator: str
+    ) -> str:
 
-        return format_objects(**obj_params)
+        return f"{prefix}{separator}{additional}"
 
     @staticmethod
-    def class_to_dict(class_: Union[BaseModel, dataclass]):
-        result_dict = {}
+    def _check_callback_data_bytes(callback_data: str) -> bool:
+        size = sys.getsizeof(callback_data)
+
+        true_size = size - 37  # 37 - is a system empty string lenght
+
+        if true_size < 64:
+            return True
+
+        raise TooMoreCharacters
+
+    def __call__(
+            self, prefix: str,
+            *args: Any,
+            separator: str = "/") -> str:
+
+        additional = AdditionalInstance(*args)
+
+        callback_data = self._get_str_callback_data(
+            prefix, additional, separator
+        )
+
+        self._check_callback_data_bytes(callback_data)
+
+        return callback_data
 
-        for key in class_.__fields__.keys():
-            result_dict[key] = class_.__getattribute__(key)
 
-        return result_dict
+AdditionalInstance = _Additional()
+CallbackData = _CallbackData()
```

### Comparing `usefulgram-0.0.0a3/PKG-INFO` & `usefulgram-0.0.0a4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 Metadata-Version: 2.1
 Name: usefulgram
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: Like aiogram but more easy
 Home-page: https://github.com/Sethis/usefulgram
 License: MIT
 Author: Alexandr Bortnik
 Author-email: sambonsttt@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiogram (>=3.0.0b5,<4.0.0)
+Requires-Dist: aiogram (>=3.0.0b8,<4.0.0)
 Requires-Dist: cachetools (>=4.0.0,<5.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
+Requires-Dist: pytz (>=2020.3,<2021.0)
 Project-URL: Bug Tracker, https://github.com/Sethis/usefulgram/issues
 Description-Content-Type: text/markdown
 
 # Usefulgram
 
+### Как скачать? 
+Всё просто - достаточно ввести `pip install usefulgram`
+
 ### Немного истории 
 aiogram - прекрасный фреймворк. Однако при работе с ним я столкнулся с тем, 
 что переношу многие функции и классы из проекта в проект. Сначала, 
 для удобной транспортировки были созданы общие классы, затем это перосло
 в общую папку, а теперь - в отдельный проект. Надеюсь, что данная
 небольшая надстройка станет полезным инструментом не только мне, но  и вам
 
 ### Какие изменения?
 В целом, usefulgram нельзя расценивать как что-то независимое. Это
 надстройка, собирающая в себя множество маленьких, но полезных утилит.
 Основные измения:
-- lazyediting - класс для удобного изменения сообщений в callback хендлерах
-- Builder, Row, Button и ReplyButton - классы для представления клавиатуры 
+- lazyediting - класс для удобного изменения сообщений в callback хендлерах.
+Настолько удобен, что я считаю его главной киллер-фичей
+- Builder, Row, Button и Reply аналоги - классы для представления клавиатуры 
 в массивно-подобном виде
 - BasePydanticFilter - Базовый класс, несколько развитая версия
 CallbackFactory, способная на type hints и несколько более обширный список
-типов
+типов. Незаменим при использовании вместе с плагином для pydantic подсказок
+в вашу IDE
 - TrottlingMiddleware - Класс, позволяющий не допустить спам. Немного 
 изменённая версия [данного кода](https://github.com/wakaree/simple_echo_bot/blob/main/middlewares/throttling.py)
 - StackerMiddleware - Класс, добавляющий все эти классы в функции
+- И многое, многое другое!
 
 #### Пример использования:
-В разработке
+На данный момент существует единственный, но при этом почти полный пример 
+использования. Найти его можно в **examples -> fully_example**
+
+#### Документация: 
+_В разработке и скоро будет доступна_
 
 ### Roadmap
-- Добавить пример использования
+- Добавить больше примеров использования
 - Перевести все тексты в библиотеке на английский
 - Добавить документацию
 - Добавить больше комментариев в код
-- Улучшить код
+- Улучшить код ✔️ - 80% библиотеки было переписано
```

