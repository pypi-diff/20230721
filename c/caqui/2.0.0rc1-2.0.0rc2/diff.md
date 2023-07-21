# Comparing `tmp/caqui-2.0.0rc1.tar.gz` & `tmp/caqui-2.0.0rc2.tar.gz`

## Comparing `caqui-2.0.0rc1.tar` & `caqui-2.0.0rc2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/sample-appium.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/sample-win-app-driver.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/sample-winium.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/sample.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/test-requirements.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tox.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/__init__.py
--rw-r--r--   0        0        0    26200 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/asynchronous.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/by.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/caqui.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/exceptions.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/helper.py
--rw-r--r--   0        0        0    25459 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/constants.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/fake_responses.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/test_sniffer.py
--rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/apk/app-debug.apk
--rw-r--r--   0        0        0    33529 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/html/iframe.html
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/html/playground.html
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/__initi__.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/test_by.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/test_helper.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/test_objects.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/utils/coverage.sh
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 caqui-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-appium.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-win-app-driver.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-winium.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/test-requirements.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tox.ini
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/__init__.py
+-rw-r--r--   0        0        0    27242 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/asynchronous.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/by.py
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/caqui.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/exceptions.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/helper.py
+-rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/constants.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/fake_responses.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/test_sniffer.py
+-rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/apk/app-debug.apk
+-rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/html/iframe.html
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/html/playground.html
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_by.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/utils/coverage.sh
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/PKG-INFO
```

### Comparing `caqui-2.0.0rc1/CODE_OF_CONDUCT.md` & `caqui-2.0.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/sample-appium.py` & `caqui-2.0.0rc2/sample-appium.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/sample-win-app-driver.py` & `caqui-2.0.0rc2/sample-win-app-driver.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/sample-winium.py` & `caqui-2.0.0rc2/sample-winium.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/sample.py` & `caqui-2.0.0rc2/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/.github/workflows/python-app.yml` & `caqui-2.0.0rc2/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/.github/workflows/python-publish.yml` & `caqui-2.0.0rc2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/caqui/asynchronous.py` & `caqui-2.0.0rc2/caqui/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,45 @@
 
 async def actions(driver_url, session, payload):
     url = f"{driver_url}/session/{session}/actions"
     await __post(url, payload)
     return True
 
 
+async def actions_move_to_element(driver_url, session, element):
+    """Move to an element simulating a mouse movement"""
+    try:
+        payload = {
+            "actions": [
+                {
+                    "type": "pointer",
+                    "parameters": {"pointerType": "mouse"},
+                    "id": "mouse",
+                    "actions": [
+                        {
+                            "type": "pointerMove",
+                            "duration": 250,
+                            "x": 0,
+                            "y": 0,
+                            "origin": {"ELEMENT": element},
+                        }
+                    ],
+                },
+                {
+                    "type": "key",
+                    "id": "key",
+                    "actions": [{"type": "pause", "duration": 0}],
+                },
+            ]
+        }
+        return await actions(driver_url, session, payload)
+    except Exception as error:
+        raise WebDriverError(f"Failed to move to element.") from error
+
+
 async def actions_scroll_to_element(driver_url, session, element):
     """Scroll to an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
                 {
                     "type": "wheel",
```

### Comparing `caqui-2.0.0rc1/caqui/caqui.py` & `caqui-2.0.0rc2/caqui/caqui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,69 @@
+import os
 from caqui import asynchronous, synchronous
 
 
+class ActionChains:
+    def __init__(self, driver) -> None:
+        self.__remote = driver.remote
+        self.__session = driver.session
+        self.__coroutines = []
+        self.__element = None
+
+    def click(self, element=None):
+        if not element:
+            element = self.__element
+        coroutine = asynchronous.click(self.__remote, self.__session, str(element))
+        self.__coroutines.append(coroutine)
+        return self
+
+    def move_to_element(self, element):
+        self.__element = element
+        coroutine = asynchronous.actions_move_to_element(
+            self.__remote, self.__session, str(element)
+        )
+        self.__coroutines.append(coroutine)
+        return self
+
+    def scroll_to_element(self, element):
+        self.__element = element
+        coroutine = asynchronous.actions_scroll_to_element(
+            self.__remote, self.__session, str(element)
+        )
+        self.__coroutines.append(coroutine)
+        return self
+
+    async def perform(self):
+        for coroutine in self.__coroutines:
+            await coroutine
+        return True
+
+
 class Window:
-    def __init__(self, remote, session) -> None:
-        self.__remote = remote
-        self.__session = session
+    def __init__(self, driver) -> None:
+        self.__remote = driver.remote
+        self.__session = driver.session
 
     async def new(self, window_type="tab"):
         """
         Open a new window
 
         :param window_type (str): tab or window
 
         return (str): window handle
         """
         return await asynchronous.new_window(self.__remote, self.__session, window_type)
 
 
 class Element:
-    def __init__(self, element, remote, session) -> None:
+    def __init__(self, element, driver) -> None:
         self.__element = element
-        self.__remote = remote
-        self.__session = session
+        self.__remote = driver.remote
+        self.__session = driver.session
+        self.__driver = driver
 
     def __str__(self) -> str:
         return self.__element
 
     @property
     def text(self):
         return synchronous.get_text(self.__remote, self.__session, self.__element)
@@ -103,66 +141,96 @@
             self.__remote, self.__session, self.__element, text
         )
 
     async def click(self):
         return await asynchronous.click(self.__remote, self.__session, self.__element)
 
     async def find_elements(self, locator, value):
-        return await asynchronous.find_children_elements(
+        result = []
+        elements = await asynchronous.find_children_elements(
             self.__remote, self.__session, self.__element, locator, value
         )
+        for element in elements:
+            result.append(Element(element, self.__driver))
+        return result
 
     async def find_element(self, locator, value):
-        return await asynchronous.find_child_element(
+        element = await asynchronous.find_child_element(
             self.__remote, self.__session, self.__element, locator, value
         )
+        return Element(element, self.__driver)
 
 
 class AsyncDriver:
     def __init__(self, remote, capabilities, url=None) -> None:
         self.__remote = remote
         self.__session = synchronous.get_session(remote, capabilities)
         if url:
+            self.__url = url
             synchronous.get(
                 remote,
                 self.__session,
                 url,
             )
 
     @property
     def remote(self):
         return self.__remote
 
     @property
     def session(self):
         return self.__session
 
+    @property
+    def title(self):
+        return synchronous.get_title(self.__remote, self.__session)
+
+    @property
+    def current_url(self):
+        return synchronous.get_url(self.__remote, self.__session)
+
     def quit(self):
         synchronous.close_session(self.__remote, self.__session)
 
+    def close(self):
+        self.quit()
+
     def window(self):
-        return Window(self.__remote, self.__session)
+        return Window(self)
+
+    def actions(self):
+        return ActionChains(self)
+
+    async def save_screenshot(self, file):
+        path = os.path.dirname(file)
+        if not path:
+            path = "./"
+        file_name = os.path.basename(file)
+        return await asynchronous.take_screenshot(
+            self.__remote, self.__session, path, file_name
+        )
 
     async def maximize_window(self):
         return await asynchronous.maximize_window(self.__remote, self.__session)
 
     async def get(self, url):
+        self.__url = url
         await asynchronous.go_to_page(
             self.__remote,
             self.__session,
             url,
         )
 
     async def find_elements(self, locator, value):
         elements = await asynchronous.find_elements(
             self.__remote, self.__session, locator, value
         )
         result = []
         for element in elements:
-            result.append(Element(element, self.__remote, self.__session))
+            result.append(Element(element, self))
         return result
 
     async def find_element(self, locator, value):
         element = await asynchronous.find_element(
             self.__remote, self.__session, locator, value
         )
-        return Element(element, self.__remote, self.__session)
+        return Element(element, self)
```

### Comparing `caqui-2.0.0rc1/caqui/synchronous.py` & `caqui-2.0.0rc2/caqui/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,28 +295,59 @@
 
 
 def get_shadow_root(driver_url, session, element):
     """Get the shadow root element"""
     try:
         root_element = "shadow-6066-11e4-a52e-4f735466cecf"
         url = f"{driver_url}/session/{session}/element/{element}/shadow"
-        return __get(url).get("value",{}).get(root_element)
+        return __get(url).get("value", {}).get(root_element)
     except Exception as error:
         raise WebDriverError(f"Failed to get the element shadow.") from error
 
 
 def get_rect(driver_url, session, element):
     """Get the element rectangle"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/rect"
         return __get(url).get("value")
     except Exception as error:
         raise WebDriverError(f"Failed to get the element rect.") from error
 
 
+def actions_move_to_element(driver_url, session, element):
+    """Move to an element simulating a mouse movement"""
+    try:
+        payload = {
+            "actions": [
+                {
+                    "type": "pointer",
+                    "parameters": {"pointerType": "mouse"},
+                    "id": "mouse",
+                    "actions": [
+                        {
+                            "type": "pointerMove",
+                            "duration": 250,
+                            "x": 0,
+                            "y": 0,
+                            "origin": {"ELEMENT": element},
+                        }
+                    ],
+                },
+                {
+                    "type": "key",
+                    "id": "key",
+                    "actions": [{"type": "pause", "duration": 0}],
+                },
+            ]
+        }
+        return actions(driver_url, session, payload)
+    except Exception as error:
+        raise WebDriverError(f"Failed to move to element.") from error
+
+
 def actions_scroll_to_element(driver_url, session, element):
     """Scroll to an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
                 {
                     "type": "wheel",
```

### Comparing `caqui-2.0.0rc1/tests/fake_responses.py` & `caqui-2.0.0rc2/tests/fake_responses.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/test_sniffer.py` & `caqui-2.0.0rc2/tests/test_sniffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support import expected_conditions, wait
 from selenium.webdriver.common.alert import Alert
 import os
+from selenium.webdriver.common.action_chains import ActionChains
 
 
 @fixture
 def setup():
     desired_capabilities = {
         # 'deviceName': 'Device',
         "deviceName": "Emulator",
@@ -39,19 +40,47 @@
     service = Service(f"/home/douglas/web_drivers/chromedriver.113")
     options = Options()
     # options.add_argument('--headless')
     options.add_argument("window-size=1920,1080")
     browser = webdriver.Chrome(service=service, options=options)
     browser.get(PAGE_URL)
 
+    browser._shadowroot_cls
+
     yield browser
     # browser.quit()
 
 
 @mark.skip("used just to discover request data")
+def test_action_chains(setup):
+    driver = setup
+
+    resource = driver.find_element("xpath", "//button")
+
+    action = ActionChains(driver)
+    action.move_to_element(resource)
+    action.perform()
+
+
+@mark.skip("used just to discover request data")
+def test_switch_to_frame_sniffer(setup):
+    driver = setup
+    # Click the link to activate the alert
+    import time
+
+    time.sleep(3)
+    element = driver.find_element(By.ID, "my-iframe")
+    driver.switch_to.frame(element)
+
+    element_alert = driver.find_element(By.ID, "alert-button-iframe")
+    element_alert.click()
+    time.sleep(3)
+
+
+@mark.skip("used just to discover request data")
 def test_switch_to_frame_sniffer(setup):
     driver = setup
     # Click the link to activate the alert
     import time
 
     time.sleep(3)
     element = driver.find_element(By.ID, "my-iframe")
```

### Comparing `caqui-2.0.0rc1/tests/apk/app-debug.apk` & `caqui-2.0.0rc2/tests/apk/app-debug.apk`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/feature/test_sync_and_async.py` & `caqui-2.0.0rc2/tests/feature/test_sync_and_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,14 +559,27 @@
 
     assert synchronous.get_rect(driver_url, session, element) == expected
 
     assert await asynchronous.get_rect(driver_url, session, element) == expected
 
 
 @mark.asyncio
+async def test_move_to_element(__setup):
+    driver_url, session = __setup
+    locator_type = By.XPATH
+    locator_value = "//button"
+
+    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
+    assert synchronous.actions_move_to_element(driver_url, session, element) is True
+    assert (
+        await asynchronous.actions_move_to_element(driver_url, session, element) is True
+    )
+
+
+@mark.asyncio
 async def test_actions_scroll_to_element(__setup):
     driver_url, session = __setup
     locator_type = By.XPATH
     locator_value = "//button"
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
     assert synchronous.actions_scroll_to_element(driver_url, session, element) is True
```

### Comparing `caqui-2.0.0rc1/tests/html/playground.html` & `caqui-2.0.0rc2/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/integration/test_async_scenarios.py` & `caqui-2.0.0rc2/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/integration/test_sync_scenarios.py` & `caqui-2.0.0rc2/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/unit/test_async_unit.py` & `caqui-2.0.0rc2/tests/unit/test_async_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/unit/test_by.py` & `caqui-2.0.0rc2/tests/unit/test_by.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/unit/test_helper.py` & `caqui-2.0.0rc2/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/tests/unit/test_objects.py` & `caqui-2.0.0rc2/tests/unit/test_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from caqui.caqui import AsyncDriver
+from caqui.caqui import AsyncDriver, Element, ActionChains
 from caqui.by import By
 from pytest import mark, fixture
 from tests.constants import PAGE_URL
 from caqui import synchronous
 
 
 class TestObject:
@@ -19,14 +19,42 @@
             }
         }
         driver = AsyncDriver(remote, capabilities, PAGE_URL)
         yield driver
         driver.quit()
 
     @mark.asyncio
+    async def test_action_chains(self, setup: AsyncDriver):
+        driver = setup
+        element = await driver.find_element(By.XPATH, "//button")
+        actions = (
+            await driver.actions()
+            .move_to_element(element)
+            .scroll_to_element(element)
+            .click()
+            .perform()
+        )
+        assert actions is True
+
+        actions = (
+            await ActionChains(driver)
+            .move_to_element(element)
+            .scroll_to_element(element)
+            .click()
+            .perform()
+        )
+        assert actions is True
+
+    @mark.asyncio
+    async def test_save_screenshot(self, setup: AsyncDriver):
+        driver = setup
+
+        assert await driver.save_screenshot("/tmp/test.png") is True
+
+    @mark.asyncio
     async def test_object_to_string(self, setup: AsyncDriver):
         driver = setup
 
         element_string = synchronous.find_element(
             driver.remote, driver.session, By.XPATH, "//button"
         )
         element = await driver.find_element(locator=By.XPATH, value="//button")
@@ -77,20 +105,23 @@
     @mark.asyncio
     async def test_find_elements_from_element(self, setup: AsyncDriver):
         driver = setup
         expected = 1
         element = await driver.find_element(locator=By.XPATH, value="//body")
         actual = await element.find_elements(By.XPATH, "//button")
         assert len(actual) >= expected
+        assert isinstance(actual[0], Element)
 
     @mark.asyncio
     async def test_find_element_from_element(self, setup: AsyncDriver):
         driver = setup
         element = await driver.find_element(locator=By.XPATH, value="//body")
-        assert await element.find_element(By.XPATH, "//button") is not None
+        actual = await element.find_element(By.XPATH, "//button")
+        assert actual is not None
+        assert isinstance(actual, Element)
 
     @mark.asyncio
     async def test_find_elements(self, setup: AsyncDriver):
         driver = setup
         expected = 1
         actual = await driver.find_elements(locator=By.XPATH, value="//button")
         assert len(actual) >= expected
```

### Comparing `caqui-2.0.0rc1/tests/unit/test_sync_unit.py` & `caqui-2.0.0rc2/tests/unit/test_sync_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/.gitignore` & `caqui-2.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/LICENSE` & `caqui-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/README.md` & `caqui-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc1/pyproject.toml` & `caqui-2.0.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "2.0.0-rc1"
+version = "2.0.0-rc2"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `caqui-2.0.0rc1/PKG-INFO` & `caqui-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 2.0.0rc1 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 2.0.0rc2 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.6 Requires-Dist: aiohttp Requires-Dist: requests Description-
```

