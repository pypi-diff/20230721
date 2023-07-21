# Comparing `tmp/webpagebp-0.1.0.tar.gz` & `tmp/webpagebp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpagebp-0.1.0.tar", max compression
+gzip compressed data, was "webpagebp-0.1.2.tar", max compression
```

## Comparing `webpagebp-0.1.0.tar` & `webpagebp-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1096 2022-10-14 16:09:17.578653 webpagebp-0.1.0/LICENSE
--rw-r--r--   0        0        0      423 2023-07-18 22:53:41.523321 webpagebp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       12 2022-10-14 16:09:17.579153 webpagebp-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-03 20:49:12.324736 webpagebp-0.1.0/webpagebp/__init__.py
--rw-r--r--   0        0        0      929 2023-07-18 22:56:00.042430 webpagebp-0.1.0/webpagebp/browsers.py
--rw-r--r--   0        0        0        0 2022-12-30 22:04:46.955478 webpagebp-0.1.0/webpagebp/generic_browser/__init__.py
--rw-r--r--   0        0        0     2495 2023-07-18 22:56:00.042430 webpagebp-0.1.0/webpagebp/generic_browser/browser.py
--rw-r--r--   0        0        0     2090 2023-01-03 15:44:39.083890 webpagebp-0.1.0/webpagebp/generic_browser/old_browser.py
--rw-r--r--   0        0        0     2120 2023-07-18 22:53:32.465808 webpagebp-0.1.0/webpagebp/job.py
--rw-r--r--   0        0        0        0 2022-12-30 22:27:06.400627 webpagebp-0.1.0/webpagebp/scrapers/__init__.py
--rw-r--r--   0        0        0      945 2023-07-18 17:39:41.933029 webpagebp-0.1.0/webpagebp/scrapers/soup.py
--rw-r--r--   0        0        0        0 2022-12-30 21:41:00.943036 webpagebp-0.1.0/webpagebp/selenium_driver/__init__.py
--rw-r--r--   0        0        0     2577 2023-07-18 22:56:00.041931 webpagebp-0.1.0/webpagebp/selenium_driver/drivers.py
--rw-r--r--   0        0        0     1555 2023-07-18 22:56:00.041931 webpagebp-0.1.0/webpagebp/selenium_driver/generic_driver.py
--rw-r--r--   0        0        0      325 2023-01-03 15:56:55.419546 webpagebp-0.1.0/webpagebp/utils.py
--rw-r--r--   0        0        0     2640 2023-07-14 22:21:22.225050 webpagebp-0.1.0/webpagebp/webpage.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 webpagebp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-10-14 16:09:17.578653 webpagebp-0.1.2/LICENSE
+-rw-r--r--   0        0        0      423 2023-07-21 21:14:45.172112 webpagebp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       12 2022-10-14 16:09:17.579153 webpagebp-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-01-03 20:49:12.324736 webpagebp-0.1.2/webpagebp/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-18 22:56:00.042430 webpagebp-0.1.2/webpagebp/browsers.py
+-rw-r--r--   0        0        0        0 2022-12-30 22:04:46.955478 webpagebp-0.1.2/webpagebp/generic_browser/__init__.py
+-rw-r--r--   0        0        0     2431 2023-07-19 15:14:40.063332 webpagebp-0.1.2/webpagebp/generic_browser/browser.py
+-rw-r--r--   0        0        0     2090 2023-01-03 15:44:39.083890 webpagebp-0.1.2/webpagebp/generic_browser/old_browser.py
+-rw-r--r--   0        0        0     2356 2023-07-19 15:15:49.321020 webpagebp-0.1.2/webpagebp/job.py
+-rw-r--r--   0        0        0        0 2022-12-30 22:27:06.400627 webpagebp-0.1.2/webpagebp/scrapers/__init__.py
+-rw-r--r--   0        0        0      945 2023-07-18 17:39:41.933029 webpagebp-0.1.2/webpagebp/scrapers/soup.py
+-rw-r--r--   0        0        0        0 2022-12-30 21:41:00.943036 webpagebp-0.1.2/webpagebp/selenium_driver/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-18 23:39:38.797351 webpagebp-0.1.2/webpagebp/selenium_driver/drivers.py
+-rw-r--r--   0        0        0     1555 2023-07-18 22:56:00.041931 webpagebp-0.1.2/webpagebp/selenium_driver/generic_driver.py
+-rw-r--r--   0        0        0      950 2023-07-19 14:50:18.873842 webpagebp-0.1.2/webpagebp/utils.py
+-rw-r--r--   0        0        0     2640 2023-07-14 22:21:22.225050 webpagebp-0.1.2/webpagebp/webpage.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 webpagebp-0.1.2/PKG-INFO
```

### Comparing `webpagebp-0.1.0/LICENSE` & `webpagebp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.0/webpagebp/browsers.py` & `webpagebp-0.1.2/webpagebp/browsers.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.0/webpagebp/generic_browser/browser.py` & `webpagebp-0.1.2/webpagebp/generic_browser/old_browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from datetime import datetime
 import re
 import time
 
-from webpagebp.utils import make_dir
-from webpagebp.scrapers.soup import Soup
+from utils import make_dir
+from scrapers.soup import Soup
 
 
 class _Browser:
     def __init__(
                     self, 
                     url = '', 
-                    dir = 'data',
-                    file = 'webpage.html',
                     action = '',
                     browser_driver = None,
+                    dir = 'data', 
+                    filename = 'webpage.html',
+                    headless = False, 
                     load_page_delay = 10, 
                     date = datetime.now().strftime('%Y-%m-%d_%H-%M-%S'),
-                    *args,
-                    **kwargs
                 ) -> None:
         self.url = url
+        self.filename = filename
         self.dir = dir
-        self.file = file
         self.date = date
         self.load_page_delay = load_page_delay
         if browser_driver is None:
             raise NotImplementedError("You're not supposed to use this class directly")
-        self.browser = browser_driver(*args, **kwargs)
+        self.browser = browser_driver(dir=self.dir, headless=headless)
         self.soup = None
 
         self.start()
 
         if action == 'auto_download_and_exit':
             self.auto_download_and_exit()
         elif self.url != '':
@@ -45,36 +44,27 @@
     def start_headless(self):
         self.browser.start_headless()
 
     def quit(self):
         if self.browser.driver.service.is_connectable():
             self.browser.quit()
 
-    def open(self, url, soup: Soup = Soup):
+    def open(self, url):
         self.browser.driver.get(self.fix_url(url))
-        self.soup = soup(self.browser.driver.page_source)
+        self.soup = Soup(self.browser.driver.page_source)
 
     def wait(self):
         time.sleep(self.load_page_delay)
 
-    # def save(self):
-    #     make_dir(dir_name=self.dir)
-    #     with open(f'{self.dir}/{self.filename}', 'w', encoding="utf-8") as file:
-    #         file.write(self.browser.driver.page_source)
-
-    def save(self, file=None, dir=None):
-        dir = dir if dir else self.dir
-        filename = file if file else self.file
-        make_dir(dir_name=dir)
-        with open(f'{dir}/{filename}', 'w', encoding="utf-8") as file:
+    def save(self):
+        make_dir(dir_name=self.dir)
+        with open(f'{self.dir}/{self.filename}', 'w', encoding="utf-8") as file:
             file.write(self.browser.driver.page_source)
-        print(f"Saving to ./{dir}/{filename}..")
 
     def find(self, method, args):
         self.browser.driver.find(method, args)
 
     def auto_download_and_exit(self):
         self.open(self.url)
         self.wait()
         self.save()
-        # super().save()
         self.quit()
```

### Comparing `webpagebp-0.1.0/webpagebp/generic_browser/old_browser.py` & `webpagebp-0.1.2/webpagebp/generic_browser/browser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from datetime import datetime
 import re
 import time
 
-from utils import make_dir
-from scrapers.soup import Soup
+from webpagebp.utils import make_dir, html_from_file
+from webpagebp.scrapers.soup import Soup
 
 
 class _Browser:
     def __init__(
                     self, 
                     url = '', 
+                    dir = 'data',
+                    file = 'webpage.html',
                     action = '',
                     browser_driver = None,
-                    dir = 'data', 
-                    filename = 'webpage.html',
-                    headless = False, 
                     load_page_delay = 10, 
                     date = datetime.now().strftime('%Y-%m-%d_%H-%M-%S'),
+                    *args,
+                    **kwargs
                 ) -> None:
         self.url = url
-        self.filename = filename
         self.dir = dir
+        self.file = file
         self.date = date
         self.load_page_delay = load_page_delay
         if browser_driver is None:
             raise NotImplementedError("You're not supposed to use this class directly")
-        self.browser = browser_driver(dir=self.dir, headless=headless)
+        self.browser = browser_driver(*args, **kwargs)
         self.soup = None
 
         self.start()
 
         if action == 'auto_download_and_exit':
             self.auto_download_and_exit()
+            self.quit()
+        elif action == 'exit':
+            self.quit()
         elif self.url != '':
             self.open(url)
 
     def fix_url(self, url):
         return 'https://' + url if not re.search('http(s|)://', url) else url
 
     def start(self):
@@ -44,25 +48,31 @@
     def start_headless(self):
         self.browser.start_headless()
 
     def quit(self):
         if self.browser.driver.service.is_connectable():
             self.browser.quit()
 
-    def open(self, url):
+    def open(self, url, soup: Soup = Soup):
         self.browser.driver.get(self.fix_url(url))
-        self.soup = Soup(self.browser.driver.page_source)
+        self.soup = soup(self.browser.driver.page_source)
+
+    def open_file(self, file):
+        return html_from_file(file)
 
     def wait(self):
         time.sleep(self.load_page_delay)
 
-    def save(self):
-        make_dir(dir_name=self.dir)
-        with open(f'{self.dir}/{self.filename}', 'w', encoding="utf-8") as file:
+    def save(self, file=None, dir=None):
+        dir = dir if dir else self.dir
+        filename = file if file else self.file
+        make_dir(dir_name=dir)
+        with open(f'{dir}/{filename}', 'w', encoding="utf-8") as file:
             file.write(self.browser.driver.page_source)
+        print(f"Saving to ./{dir}/{filename}..")
 
     def find(self, method, args):
         self.browser.driver.find(method, args)
 
     def auto_download_and_exit(self):
         self.open(self.url)
         self.wait()
```

### Comparing `webpagebp-0.1.0/webpagebp/job.py` & `webpagebp-0.1.2/webpagebp/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 
 class FindAll(DefaultJob):
     def __init__(self, url: str, find_all: List, *args, **kwargs) -> None:
         super().__init__(url, browser=ChromeHBrowser, *args, **kwargs)
         self.result = self.browser.soup.find_all(find_all)
 
 
+class ReadFile(DefaultJob):
+    def __init__(self, file: str, *args, **kwargs) -> None:
+        super().__init__(url='', browser=ChromeHBrowser, action='exit', *args, **kwargs)
+        self.result = self.browser.open_file(file)
+
+
 class Download(DefaultJob):
     def __init__(self, url: str, *args, **kwargs) -> None:
         super().__init__(url, browser=ChromeHBrowser, action='auto_download_and_exit', *args, **kwargs)
 
 
 class Chrome(DefaultJob):
     def __init__(self, url: str, *args, **kwargs) -> None:
```

### Comparing `webpagebp-0.1.0/webpagebp/scrapers/soup.py` & `webpagebp-0.1.2/webpagebp/scrapers/soup.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.0/webpagebp/selenium_driver/drivers.py` & `webpagebp-0.1.2/webpagebp/selenium_driver/drivers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
 
 from webpagebp.selenium_driver.generic_driver import _Driver
 
 
 class ChromeDriver(_Driver):
-    # def __init__(
-    #     self, 
-    #     service: Service(ChromeDriverManager().install()), 
-    #     webdriver: webdriver.Chrome, 
-    #     name = 'chrome', 
-    #     *args, 
-    #     **kwargs):
     def __init__(
         self, 
         service: Service = Service(ChromeDriverManager().install()), 
         webdriver: webdriver = webdriver.Chrome, 
         name = 'chrome', 
         *args, 
         **kwargs):
```

### Comparing `webpagebp-0.1.0/webpagebp/selenium_driver/generic_driver.py` & `webpagebp-0.1.2/webpagebp/selenium_driver/generic_driver.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.0/webpagebp/webpage.py` & `webpagebp-0.1.2/webpagebp/webpage.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.0/PKG-INFO` & `webpagebp-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpagebp
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
 Author: Sergio Schmilovich
 Author-email: sergio.schmilovich@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

