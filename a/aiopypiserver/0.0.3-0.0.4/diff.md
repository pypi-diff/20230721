# Comparing `tmp/aiopypiserver-0.0.3.tar.gz` & `tmp/aiopypiserver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopypiserver-0.0.3.tar", last modified: Tue Jul 18 18:53:24 2023, max compression
+gzip compressed data, was "aiopypiserver-0.0.4.tar", last modified: Fri Jul 21 17:09:38 2023, max compression
```

## Comparing `aiopypiserver-0.0.3.tar` & `aiopypiserver-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/
--rw-r--r--   0 mscada    (1000) mscada    (1000)    35149 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/LICENSE
--rw-r--r--   0 mscada    (1000) mscada    (1000)       31 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/MANIFEST.in
--rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/PKG-INFO
--rw-r--r--   0 mscada    (1000) mscada    (1000)     1587 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/README.md
--rw-r--r--   0 mscada    (1000) mscada    (1000)      789 2023-07-18 18:52:18.000000 aiopypiserver-0.0.3/pyproject.toml
--rw-r--r--   0 mscada    (1000) mscada    (1000)       38 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/setup.cfg
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.860734 aiopypiserver-0.0.3/src/
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.860734 aiopypiserver-0.0.3/src/aiopypiserver/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      109 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/__init__.py
--rw-r--r--   0 mscada    (1000) mscada    (1000)      112 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/__main__.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver/assets/
--rw-r--r--   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:32:37.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/__init__.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver/assets/__pycache__/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      154 2023-07-18 00:32:37.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mscada    (1000) mscada    (1000)      505 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/index.html
--rw-r--r--   0 mscada    (1000) mscada    (1000)      169 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/list.html
--rw-r--r--   0 mscada    (1000) mscada    (1000)    10000 2023-07-18 18:41:05.000000 aiopypiserver-0.0.3/src/aiopypiserver/webserver.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/
--rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/PKG-INFO
--rw-r--r--   0 mscada    (1000) mscada    (1000)      573 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/SOURCES.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)        1 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/dependency_links.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       64 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/entry_points.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       15 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/requires.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       14 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/top_level.txt
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/tests/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      941 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/tests/test_server.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.387835 aiopypiserver-0.0.4/
+-rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:09:38.387835 aiopypiserver-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/README.md
+-rw-rw-rw-   0        0        0      789 2023-07-21 17:07:58.000000 aiopypiserver-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:09:38.388836 aiopypiserver-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.331310 aiopypiserver-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.349308 aiopypiserver-0.0.4/src/aiopypiserver/
+-rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.382834 aiopypiserver-0.0.4/src/aiopypiserver/assets/
+-rw-rw-rw-   0        0        0        0 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.384835 aiopypiserver-0.0.4/src/aiopypiserver/assets/__pycache__/
+-rw-rw-rw-   0        0        0      197 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14282 2023-07-21 16:03:22.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/grids-responsive-min.css
+-rw-rw-rw-   0        0        0     2311 2023-07-21 17:02:47.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/index.html
+-rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/list.html
+-rw-rw-rw-   0        0        0    15721 2023-07-21 16:03:28.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/pure-min.css
+-rw-rw-rw-   0        0        0     2192 2023-07-21 17:00:21.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/styles.css
+-rw-rw-rw-   0        0        0    10554 2023-07-21 17:08:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/webserver.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.373826 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.386836 aiopypiserver-0.0.4/tests/
+-rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/tests/test_server.py
```

### Comparing `aiopypiserver-0.0.3/LICENSE` & `aiopypiserver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.3/PKG-INFO` & `aiopypiserver-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: aiopypiserver
-Version: 0.0.3
-Summary: Do what pypiserver does, but with aiohttp.
-Author: Jamie Walton
-Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
-Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # aiopypiserver
 
 A basic PyPi server using aiohttp to serve web pages. Intended to work behind
 an Apache proxy with relative href accessing. Available here of from [PyPI](https://pypi.org/project/aiopypiserver/).
 
 # Motivation
 
@@ -50,10 +34,18 @@
 Browse index at http://localhost:8080/.
 ```
 
 Can also be run as a module as ```python -m aiopypiserver -h```. Using the internal class is probably a bad idea ATM as the API is likely to change.
 
 By default access logs are generated, as I find it useful to see these.
 
+# Apache
+
+Add the following to your Apache config. This is the item for pypiserver that required wsgi.
+```
+ProxyPass /pypi/ http://127.0.0.1:8080/
+ProxyPassReverse /pypi/ http://127.0.0.1:8080/
+```
+
 # Thanks
 
 Please let me know how you get on through the github page.
```

### Comparing `aiopypiserver-0.0.3/README.md` & `aiopypiserver-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,67 @@
-# aiopypiserver
-
-A basic PyPi server using aiohttp to serve web pages. Intended to work behind
-an Apache proxy with relative href accessing. Available here of from [PyPI](https://pypi.org/project/aiopypiserver/).
-
-# Motivation
-
-This is intended to work behind an Apache proxy. This means providing
-href links in the pages as relative links. i.e. ./packages/pkg_name.tar.gz
-and not /packages... .
-
-This is addressed as provided by [WSGI](https://github.com/pypiserver/pypiserver/issues/155).
-Looking at the code I liked the idea of implementing with ```asyncio``` and ```aiohttp```
-in preference to forking the ```pypiserver``` code.
-
-# Usage
-
-```
-usage: aiopypiserver [-h] [-p port] [-i address] [-u username] [-P password] [-v] [-q] [package_path]
-Private PyPi  server.
-
-positional arguments:
-  package_path                       path to packages
-
-options:
-  -h, --help                         show this help message and exit
-  -p port, --port port               Listen on port
-  -i address, --interface address    Listen on address
-  -u username, --username username   For uploading packages
-  -P password, --password password   ...
-  -v, --verbose                      set debug level
-  -q, --quiet                        turn off access logging
-
-Browse index at http://localhost:8080/.
-```
-
-Can also be run as a module as ```python -m aiopypiserver -h```. Using the internal class is probably a bad idea ATM as the API is likely to change.
-
-By default access logs are generated, as I find it useful to see these.
-
-# Thanks
-
-Please let me know how you get on through the github page.
+Metadata-Version: 2.1
+Name: aiopypiserver
+Version: 0.0.4
+Summary: Do what pypiserver does, but with aiohttp.
+Author: Jamie Walton
+Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
+Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Development Status :: 1 - Planning
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aiopypiserver
+
+A basic PyPi server using aiohttp to serve web pages. Intended to work behind
+an Apache proxy with relative href accessing. Available here of from [PyPI](https://pypi.org/project/aiopypiserver/).
+
+# Motivation
+
+This is intended to work behind an Apache proxy. This means providing
+href links in the pages as relative links. i.e. ./packages/pkg_name.tar.gz
+and not /packages... .
+
+This is addressed as provided by [WSGI](https://github.com/pypiserver/pypiserver/issues/155).
+Looking at the code I liked the idea of implementing with ```asyncio``` and ```aiohttp```
+in preference to forking the ```pypiserver``` code.
+
+# Usage
+
+```
+usage: aiopypiserver [-h] [-p port] [-i address] [-u username] [-P password] [-v] [-q] [package_path]
+Private PyPi  server.
+
+positional arguments:
+  package_path                       path to packages
+
+options:
+  -h, --help                         show this help message and exit
+  -p port, --port port               Listen on port
+  -i address, --interface address    Listen on address
+  -u username, --username username   For uploading packages
+  -P password, --password password   ...
+  -v, --verbose                      set debug level
+  -q, --quiet                        turn off access logging
+
+Browse index at http://localhost:8080/.
+```
+
+Can also be run as a module as ```python -m aiopypiserver -h```. Using the internal class is probably a bad idea ATM as the API is likely to change.
+
+By default access logs are generated, as I find it useful to see these.
+
+# Apache
+
+Add the following to your Apache config. This is the item for pypiserver that required wsgi.
+```
+ProxyPass /pypi/ http://127.0.0.1:8080/
+ProxyPassReverse /pypi/ http://127.0.0.1:8080/
+```
+
+# Thanks
+
+Please let me know how you get on through the github page.
```

### Comparing `aiopypiserver-0.0.3/pyproject.toml` & `aiopypiserver-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopypiserver"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name="Jamie Walton"}
 ]
 description = "Do what pypiserver does, but with aiohttp."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `aiopypiserver-0.0.3/src/aiopypiserver/webserver.py` & `aiopypiserver-0.0.4/src/aiopypiserver/webserver.py`

 * *Files 12% similar despite different names*

```diff
@@ -124,37 +124,47 @@
         """Initialise with an argparse NameSpace."""
         self.ip = config.interface
         self.port = config.port
         self.packages = config.package_path
         self.pkg_path = Path('.').joinpath(self.packages).resolve()
         self.username = config.username
         self.password = config.password
+        logging.info(f"Running on {self.ip}:{self.port} "
+                     f"serving {self.packages}")
         self.info = get_package_details(self.pkg_path)
         if not self.pkg_path.is_dir():
             raise RuntimeError(f"{self.pkg_path} bad package directory")
         self.webapp = web.Application()
         routes = [web.get('/', self.index_handler),
                   web.get('/index.html', self.index_handler),
                   web.get('/packages/', self.packages_handler),
                   web.get('/simple/', self.simple_handler),
                   web.get('/simple/{package}/', self.simple_package_handler),
                   web.get('/packages/{file}', self.packages_file_handler),
-                  web.post('', self.post_handler)]
+                  web.post('', self.post_handler),
+                  web.get('/{file}', self.file_handler)]
         self.webapp.add_routes(routes)
         self.webapp.on_response_prepare.append(on_prepare)
         self.runner = web.AppRunner(self.webapp)
 
     def index_handler(self, request: web.Request):
         """Provide the base index.html file."""
         html = open(get('index.html')).read()
         for k, v in [('ip', self.ip),
                      ('port', str(self.port))]:
             html = html.replace(r'{{' + k + r'}}', v)
         return web.Response(body=html, content_type='text/html')
 
+    def file_handler(self, request: web.Request):
+        """Provide the any pages that might be in assets."""
+        try:
+            return web.FileResponse(get(request.match_info['file']))
+        except FileNotFoundError:
+            raise web.HTTPNotFound
+
     def packages_handler(self, request: web.Request):
         """Provide a list of modules or all packages."""
         dirlist = ''
         for file in self.pkg_path.iterdir():
             dirlist += f'\n<a href="{file.name}">{file.name}</a><br>'
         html = open(get('list.html')).read()
         html = html.replace(r'{{title}}', 'Package Index')
@@ -243,14 +253,16 @@
         self.site = web.TCPSite(self.runner, self.ip, self.port)
         await self.site.start()
 
 
 async def main():
     """Read config and run the server."""
     config = args()
+    if config.username is None or config.password is None:
+        logging.warn('empty password/username, uploading disabled')
     ws = WebServer(config)
     if config.verbose:
         logging.basicConfig(level=logging.INFO)
     await ws.run()
     await asyncio.get_running_loop().create_future()
```

### Comparing `aiopypiserver-0.0.3/src/aiopypiserver.egg-info/PKG-INFO` & `aiopypiserver-0.0.4/src/aiopypiserver.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,67 @@
-Metadata-Version: 2.1
-Name: aiopypiserver
-Version: 0.0.3
-Summary: Do what pypiserver does, but with aiohttp.
-Author: Jamie Walton
-Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
-Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# aiopypiserver
-
-A basic PyPi server using aiohttp to serve web pages. Intended to work behind
-an Apache proxy with relative href accessing. Available here of from [PyPI](https://pypi.org/project/aiopypiserver/).
-
-# Motivation
-
-This is intended to work behind an Apache proxy. This means providing
-href links in the pages as relative links. i.e. ./packages/pkg_name.tar.gz
-and not /packages... .
-
-This is addressed as provided by [WSGI](https://github.com/pypiserver/pypiserver/issues/155).
-Looking at the code I liked the idea of implementing with ```asyncio``` and ```aiohttp```
-in preference to forking the ```pypiserver``` code.
-
-# Usage
-
-```
-usage: aiopypiserver [-h] [-p port] [-i address] [-u username] [-P password] [-v] [-q] [package_path]
-Private PyPi  server.
-
-positional arguments:
-  package_path                       path to packages
-
-options:
-  -h, --help                         show this help message and exit
-  -p port, --port port               Listen on port
-  -i address, --interface address    Listen on address
-  -u username, --username username   For uploading packages
-  -P password, --password password   ...
-  -v, --verbose                      set debug level
-  -q, --quiet                        turn off access logging
-
-Browse index at http://localhost:8080/.
-```
-
-Can also be run as a module as ```python -m aiopypiserver -h```. Using the internal class is probably a bad idea ATM as the API is likely to change.
-
-By default access logs are generated, as I find it useful to see these.
-
-# Thanks
-
-Please let me know how you get on through the github page.
+Metadata-Version: 2.1
+Name: aiopypiserver
+Version: 0.0.4
+Summary: Do what pypiserver does, but with aiohttp.
+Author: Jamie Walton
+Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
+Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Development Status :: 1 - Planning
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aiopypiserver
+
+A basic PyPi server using aiohttp to serve web pages. Intended to work behind
+an Apache proxy with relative href accessing. Available here of from [PyPI](https://pypi.org/project/aiopypiserver/).
+
+# Motivation
+
+This is intended to work behind an Apache proxy. This means providing
+href links in the pages as relative links. i.e. ./packages/pkg_name.tar.gz
+and not /packages... .
+
+This is addressed as provided by [WSGI](https://github.com/pypiserver/pypiserver/issues/155).
+Looking at the code I liked the idea of implementing with ```asyncio``` and ```aiohttp```
+in preference to forking the ```pypiserver``` code.
+
+# Usage
+
+```
+usage: aiopypiserver [-h] [-p port] [-i address] [-u username] [-P password] [-v] [-q] [package_path]
+Private PyPi  server.
+
+positional arguments:
+  package_path                       path to packages
+
+options:
+  -h, --help                         show this help message and exit
+  -p port, --port port               Listen on port
+  -i address, --interface address    Listen on address
+  -u username, --username username   For uploading packages
+  -P password, --password password   ...
+  -v, --verbose                      set debug level
+  -q, --quiet                        turn off access logging
+
+Browse index at http://localhost:8080/.
+```
+
+Can also be run as a module as ```python -m aiopypiserver -h```. Using the internal class is probably a bad idea ATM as the API is likely to change.
+
+By default access logs are generated, as I find it useful to see these.
+
+# Apache
+
+Add the following to your Apache config. This is the item for pypiserver that required wsgi.
+```
+ProxyPass /pypi/ http://127.0.0.1:8080/
+ProxyPassReverse /pypi/ http://127.0.0.1:8080/
+```
+
+# Thanks
+
+Please let me know how you get on through the github page.
```

### Comparing `aiopypiserver-0.0.3/src/aiopypiserver.egg-info/SOURCES.txt` & `aiopypiserver-0.0.4/src/aiopypiserver.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,11 +8,14 @@
 src/aiopypiserver.egg-info/PKG-INFO
 src/aiopypiserver.egg-info/SOURCES.txt
 src/aiopypiserver.egg-info/dependency_links.txt
 src/aiopypiserver.egg-info/entry_points.txt
 src/aiopypiserver.egg-info/requires.txt
 src/aiopypiserver.egg-info/top_level.txt
 src/aiopypiserver/assets/__init__.py
+src/aiopypiserver/assets/grids-responsive-min.css
 src/aiopypiserver/assets/index.html
 src/aiopypiserver/assets/list.html
-src/aiopypiserver/assets/__pycache__/__init__.cpython-39.pyc
+src/aiopypiserver/assets/pure-min.css
+src/aiopypiserver/assets/styles.css
+src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
 tests/test_server.py
```

### Comparing `aiopypiserver-0.0.3/tests/test_server.py` & `aiopypiserver-0.0.4/tests/test_server.py`

 * *Files identical despite different names*

