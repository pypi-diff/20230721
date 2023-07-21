# Comparing `tmp/selene-2.0.0rc2.tar.gz` & `tmp/selene-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selene-2.0.0rc2.tar", max compression
+gzip compressed data, was "selene-2.0.0rc3.tar", max compression
```

## Comparing `selene-2.0.0rc2.tar` & `selene-2.0.0rc3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc2/LICENSE
--rw-r--r--   0        0        0    16589 2023-04-10 12:28:03.426931 selene-2.0.0rc2/README.md
--rw-r--r--   0        0        0     7937 2023-04-12 20:12:16.143699 selene-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     6045 2023-04-12 19:26:33.211787 selene-2.0.0rc2/selene/__init__.py
--rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc2/selene/_managed.py
--rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc2/selene/api/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc2/selene/api/base/__init__.py
--rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc2/selene/api/shared/__init__.py
--rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc2/selene/common/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc2/selene/common/data_structures/__init__.py
--rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc2/selene/common/data_structures/persistent.py
--rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc2/selene/common/fp.py
--rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc2/selene/common/helpers.py
--rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc2/selene/common/none_object.py
--rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc2/selene/common/predicate.py
--rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc2/selene/core/__init__.py
--rw-r--r--   0        0        0     8731 2023-04-13 16:15:03.548744 selene-2.0.0rc2/selene/core/command.py
--rw-r--r--   0        0        0     6608 2023-04-10 11:06:23.381272 selene-2.0.0rc2/selene/core/condition.py
--rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc2/selene/core/conditions.py
--rw-r--r--   0        0        0    61013 2023-04-13 13:34:08.396102 selene-2.0.0rc2/selene/core/configuration.py
--rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc2/selene/core/configuration.pyi
--rw-r--r--   0        0        0    44335 2023-04-13 13:44:05.445570 selene-2.0.0rc2/selene/core/entity.py
--rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc2/selene/core/entity.pyi
--rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc2/selene/core/exceptions.py
--rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc2/selene/core/locator.py
--rw-r--r--   0        0        0    17245 2023-04-10 11:06:23.584719 selene-2.0.0rc2/selene/core/match.py
--rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc2/selene/core/query.py
--rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc2/selene/core/wait.py
--rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc2/selene/py.typed
--rw-r--r--   0        0        0      107 2023-04-01 17:58:51.579568 selene-2.0.0rc2/selene/support/__init__.py
--rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc2/selene/support/_logging.py
--rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc2/selene/support/by.py
--rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc2/selene/support/conditions/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc2/selene/support/conditions/be.py
--rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc2/selene/support/conditions/have.py
--rw-r--r--   0        0        0     8989 2023-04-10 11:06:23.509416 selene-2.0.0rc2/selene/support/conditions/not_.py
--rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc2/selene/support/shared/__init__.py
--rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc2/selene/support/shared/browser.py
--rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc2/selene/support/shared/config.py
--rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc2/selene/support/shared/jquery_style.py
--rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc2/selene/support/webdriver.py
--rw-r--r--   0        0        0    18274 1970-01-01 00:00:00.000000 selene-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc3/LICENSE
+-rw-r--r--   0        0        0    16589 2023-07-21 19:40:03.696730 selene-2.0.0rc3/README.md
+-rw-r--r--   0        0        0     7937 2023-07-21 20:19:06.512747 selene-2.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-07-21 20:13:43.937671 selene-2.0.0rc3/selene/__init__.py
+-rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc3/selene/_managed.py
+-rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc3/selene/api/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc3/selene/api/base/__init__.py
+-rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc3/selene/api/shared/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc3/selene/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc3/selene/common/data_structures/__init__.py
+-rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc3/selene/common/data_structures/persistent.py
+-rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc3/selene/common/fp.py
+-rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc3/selene/common/helpers.py
+-rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc3/selene/common/none_object.py
+-rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc3/selene/common/predicate.py
+-rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc3/selene/core/__init__.py
+-rw-r--r--   0        0        0     9379 2023-07-01 11:09:18.988781 selene-2.0.0rc3/selene/core/command.py
+-rw-r--r--   0        0        0     6672 2023-07-01 11:00:30.192218 selene-2.0.0rc3/selene/core/condition.py
+-rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc3/selene/core/conditions.py
+-rw-r--r--   0        0        0    61335 2023-07-21 19:02:34.547994 selene-2.0.0rc3/selene/core/configuration.py
+-rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc3/selene/core/configuration.pyi
+-rw-r--r--   0        0        0    44433 2023-07-01 11:09:18.989737 selene-2.0.0rc3/selene/core/entity.py
+-rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc3/selene/core/entity.pyi
+-rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc3/selene/core/exceptions.py
+-rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc3/selene/core/locator.py
+-rw-r--r--   0        0        0    17246 2023-07-01 11:09:18.990179 selene-2.0.0rc3/selene/core/match.py
+-rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc3/selene/core/query.py
+-rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc3/selene/core/wait.py
+-rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc3/selene/py.typed
+-rw-r--r--   0        0        0      120 2023-07-21 19:00:31.406121 selene-2.0.0rc3/selene/support/__init__.py
+-rw-r--r--   0        0        0       32 2023-07-21 19:00:05.654941 selene-2.0.0rc3/selene/support/_extensions/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-21 19:00:05.662165 selene-2.0.0rc3/selene/support/_extensions/webdriver_manager/__init__.py
+-rw-r--r--   0        0        0     7336 2023-07-21 20:05:15.134209 selene-2.0.0rc3/selene/support/_extensions/webdriver_manager/patch.py
+-rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc3/selene/support/_logging.py
+-rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc3/selene/support/by.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc3/selene/support/conditions/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc3/selene/support/conditions/be.py
+-rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc3/selene/support/conditions/have.py
+-rw-r--r--   0        0        0     9093 2023-07-01 10:59:38.230736 selene-2.0.0rc3/selene/support/conditions/not_.py
+-rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc3/selene/support/shared/__init__.py
+-rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc3/selene/support/shared/browser.py
+-rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc3/selene/support/shared/config.py
+-rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc3/selene/support/shared/jquery_style.py
+-rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc3/selene/support/webdriver.py
+-rw-r--r--   0        0        0    18226 1970-01-01 00:00:00.000000 selene-2.0.0rc3/PKG-INFO
```

### Comparing `selene-2.0.0rc2/LICENSE` & `selene-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/README.md` & `selene-2.0.0rc3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
 
 ## Changelog
 
 [see CHANGELOG.md][changelog]
 
 <!-- References -->
 [selenide]: http://selenide.org/
-[latest-recommended-version]: https://pypi.org/project/selene/2.0.0b17/
+[latest-recommended-version]: https://pypi.org/project/selene/2.0.0rc2/
 [brunch-ver-1]: https://github.com/yashaka/selene/tree/1.x
 [selene-stable]: https://pypi.org/project/selene/1.0.2/
 [python-37]: https://www.python.org/downloads/release/python-370/
 [pyenv]: https://github.com/pyenv/pyenv
 [poetry]: https://python-poetry.org/
 [project-template]: https://github.com/yashaka/python-web-test
 <!-- --8<-- [end:githubSection] -->
```

### Comparing `selene-2.0.0rc2/pyproject.toml` & `selene-2.0.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "selene"
-version = "2.0.0rc2"
+version = "2.0.0rc3"
 description = "User-oriented browser tests in Python (Selenide port)"
 authors = ["Iakiv Kramarenko <yashaka@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
 	"testing",
 	"selenium",
 	"selenide",
 	"browser",
 	"pageobject",
 	"widget",
 	"wrapper"
 ]
 homepage = "https://yashaka.github.io/selene/"
-repository = "http://github.com/yashaka/selene/"
+repository = "https://github.com/yashaka/selene/"
 documentation = "https://yashaka.github.io/selene/"
 classifiers = [
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
-	"Development Status :: 3 - Alpha",
+	"Development Status :: 4 - Beta",
 	"Natural Language :: English",
 	"Environment :: Web Environment",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: Apache Software License",
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 	"Topic :: Software Development :: Libraries :: Application Frameworks",
@@ -45,15 +45,15 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/yashaka/selene/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 selenium = ">=4.4.3"
 future = "*"
-webdriver-manager = ">=3.8.5"
+webdriver-manager = "==3.8.6"
 typing-extensions = "==4.3.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pycodestyle = "*"
 pylint = "^2.7.2"
 pytest = "*"
@@ -64,16 +64,16 @@
 Appium-Python-Client = "^2.9.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.2"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocs-material = "^9.1.6"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mkdocs-redirects = "^1.2.0"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `selene-2.0.0rc2/selene/__init__.py` & `selene-2.0.0rc3/selene/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,8 +223,8 @@
 """
 
 # """
 # Just types...
 # """
 from selene.core.entity import Element, Collection  # noqa
 
-__version__ = '2.0.0rc2'
+__version__ = '2.0.0rc3'
```

### Comparing `selene-2.0.0rc2/selene/api/__init__.py` & `selene-2.0.0rc3/selene/api/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/api/base/__init__.py` & `selene-2.0.0rc3/selene/api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/api/shared/__init__.py` & `selene-2.0.0rc3/selene/api/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/common/data_structures/persistent.py` & `selene-2.0.0rc3/selene/common/data_structures/persistent.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/common/fp.py` & `selene-2.0.0rc3/selene/common/fp.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/common/helpers.py` & `selene-2.0.0rc3/selene/common/helpers.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/common/none_object.py` & `selene-2.0.0rc3/selene/common/none_object.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/common/predicate.py` & `selene-2.0.0rc3/selene/common/predicate.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/__init__.py` & `selene-2.0.0rc3/selene/core/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/command.py` & `selene-2.0.0rc3/selene/core/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,35 @@
     .locate()
     .send_keys(
         (Keys.COMMAND if sys.platform == 'darwin' else Keys.CONTROL) + 'a' + Keys.NULL,
     ),
 )
 
 
+def _drag_to(destination: Element):
+    def func(source: Element):
+        located_source = source.locate()
+        located_destination = destination.locate()
+        driver = source.config.driver
+        actions: ActionChains = ActionChains(driver)
+
+        actions.w3c_actions = ActionBuilder(
+            driver, mouse=PointerInput(interaction.POINTER_MOUSE, 'mouse')
+        )
+        (
+            actions.w3c_actions.pointer_action.move_to(located_source)
+            .pointer_down()
+            .move_to(located_destination)
+            .release()
+        )
+        actions.perform()
+
+    return Command(f'drag to -> {destination}', func)
+
+
 # TODO: can we make it work for both mobile and web?
 #       should we selectively choose proper interaction.POINTER_TOUCH below?
 def _long_press(duration=1.0):
     def func(element: Element):
         located_element = element.locate()
         driver = element.config.driver
         actions: ActionChains = ActionChains(driver)
```

### Comparing `selene-2.0.0rc2/selene/core/condition.py` & `selene-2.0.0rc3/selene/core/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
                 self.call(entity)
                 return True
             except Exception as e:
                 return False
 
         return fn
 
+    # TODO: fix typing issues when passing to should explicitly
     @property
     def not_(self) -> Condition[E]:  # TODO: better name?
         return self.__class__.as_not(self)
 
     def __call__(self, entity: E) -> None:
         return self._fn(entity)
```

### Comparing `selene-2.0.0rc2/selene/core/conditions.py` & `selene-2.0.0rc3/selene/core/conditions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/configuration.py` & `selene-2.0.0rc3/selene/core/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2015-2023 Iakiv Kramarenko
+# Copyright (c) 2015 Iakiv Kramarenko
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -30,27 +30,28 @@
 import typing
 import warnings
 from typing import Callable, Optional, Any
 
 from selenium.webdriver.common.options import BaseOptions
 from selenium.webdriver.common.service import Service
 
+from selene import support
 from selene.common import fp, helpers
 from selene.common.data_structures import persistent
 from selene.common.fp import F
 from selene.common.helpers import on_error_return_false
 
 from selene.core.exceptions import TimeoutException
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from selene.core.wait import Wait, E
 
 
 # TODO: consider moving to support.*
-#       like support._loging.wait_with
+#       like support._logging.wait_with
 def _build_local_driver_by_name_or_remote_by_url_and_options(
     config: Config,
 ) -> WebDriver:
     from selenium.webdriver import (
         ChromeOptions,
         EdgeOptions,
         Chrome,
@@ -68,38 +69,35 @@
 
     from webdriver_manager.core.utils import ChromeType  # type: ignore
 
     def install_and_build_chrome():
         # TODO: consider simplifying the logic... to much of ifs
         #       probably all ifs were already before calling this function
         #       see example of simplification in install_and_build_firefox
-        if config.driver_options:
-            if isinstance(config.driver_options, ChromeOptions):
-                return Chrome(
-                    service=config.driver_service
-                    or ChromeService(
-                        ChromeDriverManager(chrome_type=ChromeType.GOOGLE).install()
-                    ),
-                    options=config.driver_options,
-                )
-            else:
-                raise ValueError(
-                    f'Default config.build_driver_strategy («driver factory»), '
-                    f'if config.driver_name is set to "chrome", - '
-                    f'expects only instance of ChromeOptions or None'
-                    f'in config.driver_options,'
-                    f'but got: {config.driver_options}'
-                )
-        else:
-            return Chrome(
-                service=config.driver_service
-                or ChromeService(
-                    ChromeDriverManager(chrome_type=ChromeType.GOOGLE).install()
-                )
+        if config.driver_options and not isinstance(
+            config.driver_options, ChromeOptions
+        ):
+            raise ValueError(
+                f'Default config.build_driver_strategy ("driver factory"), '
+                f'if config.driver_name is set to "chrome", - '
+                f'expects only instance of ChromeOptions or None'
+                f'in config.driver_options,'
+                f'but got: {config.driver_options}'
+            )
+
+        driver_manager = (
+            support._extensions.webdriver_manager.patch._to_find_chromedrivers_from_115(
+                ChromeDriverManager(chrome_type=ChromeType.GOOGLE)
             )
+        )
+
+        return Chrome(
+            service=config.driver_service or ChromeService(driver_manager.install()),
+            options=config.driver_options,
+        )
 
     def install_and_build_firefox():
         return Firefox(
             service=config.driver_service
             or FirefoxService(GeckoDriverManager().install()),
             options=config.driver_options,
         )
@@ -383,15 +381,15 @@
                     raise TypeError(
                         'Providing custom descriptor objects on init '
                         'to customize driver management is not supported, '
                         'because it would be too limited... '
                         'You would be able to provide it only on init,'
                         'and use it only via attribute access,'
                         'without possibility to override value with `persistent.replace` '
-                        'or `config.with_(**optioins_to_override)`. '
+                        'or `config.with_(**options_to_override)`. '
                         'If you want to use custom descriptor, '
                         'you have to subclass Config and provide your descriptor object'
                         'on class attributes definition level.'
                     )  # TODO: cover with tests
             else:
                 # setting WebDriver instance directly on init
                 driver_box = persistent.Box(value)
@@ -426,23 +424,27 @@
     of Selene commands. And `config.base_url` is used
     in `browser.open(relative_url)` command.
 
     As option, the driver instance is also considered. Moreover, this config
     is not just config, but fully manages the driver lifecycle.
     Actually, the "driver manager" is a part of this config.
 
-    While surfing through all avaialable options, pay attention to terminology:
+    While surfing through all available options, pay attention to terminology:
 
     - all options that have a `driver` word in their name
-      are related to driver management, and they are connected in a specific way:)
-      - read more on this under `config.with_` doc section;)
+    are related to driver management, and they are connected in a specific way:)
+        - read more on this under
+        [`config.with_`][selene.core.configuration.Config.with_] doc section;)
     - all options that have a `strategy` word in their name directly influence
-      the driver lifecycle in context of driver management.
-    - all options that are prefixed with `_` are considered "experimental"
-        - their naming can be changed in the future, or even an option can be removed
+    the driver lifecycle in context of driver management.
+    - !!! warning ""
+
+            all options that are prefixed with `_` are considered "experimental"
+            (their naming can be changed in the future,
+            or even an option can be removed)
 
     Examples:
         Here's how you can build a driver with the instance of this config:
 
         >>> from selene import Config
         >>> config = Config()
         >>> driver = config.driver  # new instance, built on 1st access to `driver`
@@ -497,15 +499,15 @@
         >>> driver = my_config.driver
         >>> assert driver.name == 'firefox'
         >>> # AND...
         >>> assert driver is not browser.config.driver  # ;)
         >>> assert browser.config.driver.name == 'chrome'
 
         As you can see Selene config is closely related to the browser.
-        Moreover, the same type of "declarative config copying" happens implicitely,
+        Moreover, the same type of "declarative config copying" happens implicitly,
         when you apply "copying" to browser:
 
         >>> from selene import browser
         >>> second_browser = browser.with_(driver_name='firefox')
         >>> assert second_browser.config.driver.name == 'firefox'
         >>> # AND...
         >>> assert second_browser.config.driver is not browser.config.driver  # ;)
@@ -632,20 +634,20 @@
         >>>     },
         >>> )
         >>> browser.config.driver_options = options
         >>> browser.config.driver_remote_url = 'http://hub.browserstack.com/wd/hub'
 
     By having config options that influences Selene behavior,
     like `config.timeout` and `config.base_url`,
-    - together with complete "driver management",
+    – together with complete "driver management",
     we definitely break SRP principle... In the name of Good:D. Kind of;).
 
     All this makes it far from being a simple options data class...
-    - yet kept as one «class for everything» to keep things easier to use,
-    especially taking into account some historical reasons of Selenes design,
+    – yet kept as one "class for everything" to keep things easier to use,
+    especially taking into account some historical reasons of Selene design,
     that was influenced a lot by the Selenide from Java world.
     As a result sometimes options are not consistent with each other,
     when we speak about different contexts of their usage.
     For example, this same config,
     once customized with `config.driver_options = UiAutomator2Options()`,
     will result in mobile driver built, but then all other web-related options,
     for example, a `config.base_url` will be not relevant.
@@ -682,16 +684,16 @@
     Hence, you can't use `config.driver` directly inside this factory,
     because it may lead to recursion.
 
     The default factory builds:
 
     - either a local driver by value specified in `config.driver_name`
     - or a local driver by browserName capability specified in `config.driver_options`
-    - or remote driver by value specified in `config.driver_remote_url`.
-    - or mobile driver according to `config.driver_options` capabilities.
+    - or remote driver by value specified in `config.driver_remote_url`
+    - or mobile driver according to `config.driver_options` capabilities
     """
 
     # TODO: isn't this option too much?
     #       having it, we have to keep driver descriptor definition
     #       after this option definition,
     #       that is pretty tightly coupled...
     #       heh, but maybe we definitely have to keep it defined
@@ -761,15 +763,15 @@
         which driver to build, e.g. just specifying
 
         >>> from selene import browser
         >>> from selenium import webdriver
         >>>
         >>> browser.config.driver_options = webdriver.FirefoxOptions()`
 
-        - will tell Selene to build a Firefox driver.
+        – will tell Selene to build a Firefox driver.
 
         But usually you want something more specific,
         like specifying to run a browser in headless more:
 
         >>> from selene import browser
         >>> from selenium import webdriver
         >>>
@@ -958,17 +960,19 @@
 
     Is used inside `browser.open(relative_or_absolute_url)`,
     and defines its behavior correspondingly.
     """
 
     # TODO: should we use `rebuild` term instead of `reset`?
     #       to be consistent with `rebuild_not_alive_driver`...
-    #       Technically, we are not explicitely rebuilding it with this option,
+    #       Technically, we are not explicitly rebuilding it with this option,
     #       we do reset it by setting to `...`. But then in same `get_url`,
     #       on first access it will be rebuilt automatically.
+    #       But shouldn't we use a goal-oriented term, not impl-oriented?
+    #       The goal is actually to rebuild driver on get url!
     _reset_not_alive_driver_on_get_url: bool = True
     """
     Controls whether driver should be automatically reset and, thus,
     forced to be rebuilt, if it was noticed as not alive (e.g. after quit or crash)
     on next call to `config.driver.get(url)`
     (via `config._driver_get_url_strategy`).
 
@@ -1033,15 +1037,15 @@
 
     Once driver-definition-related options are set
     (like `config.driver_options`, `config.driver_remote_url`),
     the driver will be built on first access to this attribute.
     Thus, to build the driver with Selene,
     you simply call `config.driver` for the first time,
     and usually the simplest way to access it
-    - is through either `browser.config.driver` or even `browser.driver` shortcut.
+    – is through either `browser.config.driver` or even `browser.driver` shortcut.
     Moreover, usually you don't do this explicitly,
     but rather use `browser.open(url)` to build a driver and open a page.
 
     Scenarios:
         GIVEN unset, i.e. equals to default `...` or `None`,<br>
         WHEN accessed first time (e.g. via config.driver)<br>
         THEN it will be set to the instance built by `config.build_driver_strategy`.<br>
@@ -1169,14 +1173,17 @@
     """
     click_by_js: bool = False
     """
     A flag to indicate whether to use JavaScript to click on element
     via `element.click()`, usually, as a workaround,
     when default selenium-based implementation does not work.
     """
+    # TODO: consider wait_with_js_for_element_interactable
+    #       should we add also (or instead?)
+    #       config.is_element_interactable_strategy?
     wait_for_no_overlap_found_by_js: bool = False
     """
     A flag to indicate whether to use JavaScript to detect overlapping elements
     and wait for them to disappear, when calling commands like `element.type(text)`.
     It is needed because Selenium does not support overlapping elements detection
     on any command except `click`. Hence, when you call `click` on an element,
     and there is some overlay on top of it
@@ -1188,21 +1195,23 @@
     Selenium will not and so Selene will not wait.
     Hence, if you want to wait in such cases, turn on this option.
     Just keep in mind, that it will work only for web tests, not mobile.
     """
 
     # TODO: better name? now technically it's not a decorator but decorator_builder...
     # or decorator_factory...
-    # yet in python they call it just «decorator with args» or «decorator with params»
+    # yet in python they call it just "decorator with args" or "decorator with params"
     # so technically we are correct naming it simply _wait_decorator
     # by type hint end users yet will see the real signature
-    # and hence guess its «builder-like» nature
+    # and hence guess its "builder-like" nature
     # yet... should we for verbosity distinguish options
     # that a decorator factories from options that are simple decorators?
     # maybe better time to decide on this will be once we have more such options :p
+    # TODO: What about config.wait_decorator_strategy?
+    #       or even config.build_wait_decorator_strategy?
     _wait_decorator: Callable[[Wait[E]], Callable[[F], F]] = lambda w: lambda f: f
     """
     Is used when performing any element command and assertion (i.e. should)
     Hence, can be used to log corresponding commands with waits,
     and integrate with something like allure reporting;)
 
     Yet prefixed with underscore, indicating that method is experimental,
@@ -1225,18 +1234,18 @@
         >>>   context=allure_commons._allure.StepContext
         >>> )
     """
 
     # TODO: why we name it as hook_* why not handle_* ?
     #       what would be proper style?
     hook_wait_failure: Optional[Callable[[TimeoutException], Exception]] = None
-    '''
+    """
     A handler for all exceptions, thrown on failed waiting for timeout.
     Should process the original exception and rethrow it or the modified one.
-    '''
+    """
 
     reports_folder: str = os.path.join(
         os.path.expanduser('~'),
         '.selene',
         'screenshots',
         str(round(time.time() * 1000)),
     )
@@ -1284,16 +1293,16 @@
                     else ...
                 ),
             )
         ),
         fp.do(
             lambda path: (
                 warnings.warn(
-                    "name used for saved screenshot does not match file "
-                    "type. It should end with an `.png` extension",
+                    'name used for saved screenshot does not match file '
+                    'type. It should end with an `.png` extension',
                     UserWarning,
                 )
                 if not path.lower().endswith('.png')
                 else ...
             )
         ),
         lambda path: (path if config.driver.get_screenshot_as_file(path) else None),
@@ -1332,16 +1341,16 @@
                     else ...
                 ),
             )
         ),
         fp.do(
             lambda path: (
                 warnings.warn(
-                    "name used for saved page source does not match file "
-                    "type. It should end with an `.html` extension",
+                    'name used for saved page source does not match file '
+                    'type. It should end with an `.html` extension',
                     UserWarning,
                 )
                 if not path.lower().endswith('.html')
                 else ...
             )
         ),
         lambda path: (path, config.driver.page_source),
```

### Comparing `selene-2.0.0rc2/selene/core/configuration.pyi` & `selene-2.0.0rc3/selene/core/configuration.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/entity.py` & `selene-2.0.0rc3/selene/core/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1036,14 +1036,15 @@
                     typing.Sequence[WebElement],
                     flatten([webelement.find_elements(*by) for webelement in self()]),
                 ),
             ),
             self.config,
         )
 
+    # todo: consider collection.all_first(number, selector) to get e.g. two first td from each tr
     def all_first(self, selector: Union[str, Tuple[str, str]]) -> Collection:
         """
         Returns a collection of each first element found be selector inside each element of self
 
         An alias to ``collection.collected(lambda its: its.element(selector))``.
         Not same as ``collection.all(selector).first`` that is same as ``collection.first.element(selector)``
```

### Comparing `selene-2.0.0rc2/selene/core/entity.pyi` & `selene-2.0.0rc3/selene/core/entity.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/exceptions.py` & `selene-2.0.0rc3/selene/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/locator.py` & `selene-2.0.0rc3/selene/core/locator.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/match.py` & `selene-2.0.0rc3/selene/core/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from selene.core.entity import Collection, Element, Browser
 
 # TODO: consider moving to selene.match.element.is_visible, etc...
 element_is_visible: Condition[Element] = ElementCondition.raise_if_not(
     'is visible', lambda element: element().is_displayed()
 )
 
+
 element_is_hidden: Condition[Element] = ElementCondition.as_not(
     element_is_visible, 'is hidden'
 )
 
 element_is_enabled: Condition[Element] = ElementCondition.raise_if_not(
     'is enabled', lambda element: element().is_enabled()
 )
```

### Comparing `selene-2.0.0rc2/selene/core/query.py` & `selene-2.0.0rc3/selene/core/query.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/core/wait.py` & `selene-2.0.0rc3/selene/core/wait.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/_logging.py` & `selene-2.0.0rc3/selene/support/_logging.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/by.py` & `selene-2.0.0rc3/selene/support/by.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/conditions/be.py` & `selene-2.0.0rc3/selene/support/conditions/be.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/conditions/have.py` & `selene-2.0.0rc3/selene/support/conditions/have.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/conditions/not_.py` & `selene-2.0.0rc3/selene/support/conditions/not_.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 from selene.core import match as _match
 
 # --- be.* conditions --- #
 from selene.core.condition import Condition
 from selene.core.entity import Element, Collection, Browser
 
+# TODO: consider refactoring to class for better extendability
+#       when creating custom conditions
+
 visible: Condition[Element] = _match.element_is_visible.not_
 hidden: Condition[Element] = _match.element_is_hidden.not_
 
 present: Condition[Element] = _match.element_is_present.not_
 in_dom: Condition[Element] = _match.element_is_present.not_
 # TODO: do we need both present and in_dom?
 # TODO: consider deprecating existing
```

### Comparing `selene-2.0.0rc2/selene/support/shared/__init__.py` & `selene-2.0.0rc3/selene/support/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/shared/browser.py` & `selene-2.0.0rc3/selene/support/shared/browser.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/shared/config.py` & `selene-2.0.0rc3/selene/support/shared/config.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/shared/jquery_style.py` & `selene-2.0.0rc3/selene/support/shared/jquery_style.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/selene/support/webdriver.py` & `selene-2.0.0rc3/selene/support/webdriver.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc2/PKG-INFO` & `selene-2.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: selene
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: User-oriented browser tests in Python (Selenide port)
 Home-page: https://yashaka.github.io/selene/
 License: MIT
 Keywords: testing,selenium,selenide,browser,pageobject,widget,wrapper
 Author: Iakiv Kramarenko
 Author-email: yashaka@gmail.com
 Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: future
 Requires-Dist: selenium (>=4.4.3)
 Requires-Dist: typing-extensions (==4.3.0)
-Requires-Dist: webdriver-manager (>=3.8.5)
+Requires-Dist: webdriver-manager (==3.8.6)
 Project-URL: Changelog, https://github.com/yashaka/selene/releases
 Project-URL: Documentation, https://yashaka.github.io/selene/
-Project-URL: Repository, http://github.com/yashaka/selene/
+Project-URL: Repository, https://github.com/yashaka/selene/
 Description-Content-Type: text/markdown
 
 <!-- --8<-- [start:githubSection] -->
 # Selene - User-oriented Web UI browser tests in Python (Selenide port)
 
 ![Pre-release Version](https://img.shields.io/github/v/release/yashaka/selene?label=latest)
 [![tests](https://github.com/yashaka/selene/actions/workflows/tests.yml/badge.svg)](https://github.com/yashaka/selene/actions/workflows/tests.yml)
@@ -583,15 +582,15 @@
 
 ## Changelog
 
 [see CHANGELOG.md][changelog]
 
 <!-- References -->
 [selenide]: http://selenide.org/
-[latest-recommended-version]: https://pypi.org/project/selene/2.0.0b17/
+[latest-recommended-version]: https://pypi.org/project/selene/2.0.0rc2/
 [brunch-ver-1]: https://github.com/yashaka/selene/tree/1.x
 [selene-stable]: https://pypi.org/project/selene/1.0.2/
 [python-37]: https://www.python.org/downloads/release/python-370/
 [pyenv]: https://github.com/pyenv/pyenv
 [poetry]: https://python-poetry.org/
 [project-template]: https://github.com/yashaka/python-web-test
 <!-- --8<-- [end:githubSection] -->
```

