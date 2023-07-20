# Comparing `tmp/umapi_client-3.0.tar.gz` & `tmp/umapi_client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umapi_client-3.0.tar", max compression
+gzip compressed data, was "umapi_client-3.0.1.tar", max compression
```

## Comparing `umapi_client-3.0.tar` & `umapi_client-3.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1094 2023-05-18 20:14:47.088379 umapi_client-3.0/LICENSE
--rw-r--r--   0        0        0     2082 2023-05-18 20:14:47.088379 umapi_client-3.0/README.md
--rw-r--r--   0        0        0     1226 2023-05-18 20:14:47.088379 umapi_client-3.0/pyproject.toml
--rw-r--r--   0        0        0     1543 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/__init__.py
--rw-r--r--   0        0        0    12272 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/api.py
--rw-r--r--   0        0        0     4971 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/auth.py
--rw-r--r--   0        0        0    24495 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/connection.py
--rw-r--r--   0        0        0     2606 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/error.py
--rw-r--r--   0        0        0    14377 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/functional.py
--rw-r--r--   0        0        0     1137 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/version.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 umapi_client-3.0/setup.py
--rw-r--r--   0        0        0     3502 1970-01-01 00:00:00.000000 umapi_client-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-20 23:22:58.078339 umapi_client-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2580 2023-07-20 23:22:58.078339 umapi_client-3.0.1/README.md
+-rw-r--r--   0        0        0     1228 2023-07-20 23:22:58.078339 umapi_client-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1644 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/__init__.py
+-rw-r--r--   0        0        0    12272 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/api.py
+-rw-r--r--   0        0        0     4971 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/auth.py
+-rw-r--r--   0        0        0    24495 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/connection.py
+-rw-r--r--   0        0        0     2606 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/error.py
+-rw-r--r--   0        0        0    14377 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/functional.py
+-rw-r--r--   0        0        0     1139 2023-07-20 23:22:58.082339 umapi_client-3.0.1/umapi_client/version.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 umapi_client-3.0.1/setup.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 umapi_client-3.0.1/PKG-INFO
```

### Comparing `umapi_client-3.0/LICENSE` & `umapi_client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/README.md` & `umapi_client-3.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 # umapi-client.py
 
 This is a Python client for the User Management API from Adobe, aka the
 [UMAPI](https://www.adobe.io/products/usermanagement/docs/gettingstarted.html).
 
-The User Management API is an Adobe-hosted network service 
-which provides Adobe Enterprise customers the ability to manage their users.  This
-client makes it easy to access the UMAPI from a local Python application.
+The User Management API is an Adobe-hosted network service which provides Adobe
+Enterprise customers the ability to manage their users. This client makes it
+easy to access the UMAPI from a local Python application.
+
+See the [user guide](https://adobe-apiplatform.github.io/umapi-client.py/) for
+more information.
 
 This client is open source, maintained by Adobe, and distributed under the terms
-of the OSI-approved MIT license.  Copyright (c) 2016-2021 Adobe Inc.
+of the OSI-approved MIT license. Copyright (c) 2016-2023 Adobe Inc.
+
+# Compatibility
+
+The `3.x` release branch is actively maintained. New users of the UMAPI client
+should use the latest 3.x release. The `2.x` branch is still supported, but new
+2.x releases will only contain bug fixes. New features will only be developed
+for 3.x.
+
+Pull requests for 3.x should be made against the `v3` branch (the default
+branch). Anything related to 2.x bugfixes should target `v2`.
 
 # Installation
 
 `umapi-client.py` is published to the Python Packaging Index.
 
 https://pypi.org/project/umapi-client/
 
@@ -26,39 +39,40 @@
 
 ```
 $ poetry add umapi-client
 ```
 
 # Building
 
-[Poetry](https://python-poetry.org/) is required to build the package. Follow the instructions documented on
-Poetry's website to install it on your system.
+[Poetry](https://python-poetry.org/) is required to build the package. Follow
+the instructions documented on Poetry's website to install it on your system.
 
 1. Clone this repository
    ```
    $ git clone https://github.com/adobe-apiplatform/umapi-client.py
    $ cd umapi-client.py
    ```
 
 2. Install dependencies to virtual environment.
    ```
    $ poetry install
    ```
 
-3. The `build` command will create a source package (`.tar.gz`) and a wheel file (`.whl`) in the `dist` directory.
+3. The `build` command will create a source package (`.tar.gz`) and a wheel file
+   (`.whl`) in the `dist` directory.
+
    ```
    $ poetry build
    $ ls dist
-   umapi-client-2.18.tar.gz  umapi_client-2.18-py3-none-any.whl
+   umapi-client-3.0.1.tar.gz  umapi_client-3.0.1-py3-none-any.whl
    ```
 
 4. Some of the packages required by this module use encryption, and so may
-   require you to do local builds of modules that use SSL.  Typically, this
-   will require you to have a python installed that supports compiling
-   extensions.
+   require you to do local builds of modules that use SSL. Typically, this will
+   require you to have a python installed that supports compiling extensions.
 
 5. Run tests with `pytest`.
    ```
    $ poetry run pytest
    ```
 
 # Usage
@@ -66,8 +80,9 @@
 Usage documentation, as well as information about how to get client
 credentials for use of the UMAPI, can be found in the
 [user guide](https://adobe-apiplatform.github.io/umapi-client.py/),
 whose sources are in the `docs` directory of this repository.
 
 # License
 
-This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+This project is licensed under the MIT License. See [LICENSE](LICENSE) for more
+information.
```

### Comparing `umapi_client-3.0/pyproject.toml` & `umapi_client-3.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umapi-client"
-version = "3.0"
+version = "3.0.1"
 description = "Client for the User Management API (UMAPI) from Adobe - see https://adobe.ly/2h1pHgV"
 readme = "README.md"
 authors = ["Andrew Dorton <adorton@adobe.com>", "Dan Brotsky", "Danimae Vossen", "Kevin Bhunut"]
 maintainers = ["Andrew Dorton <adorton@adobe.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.6",
@@ -28,12 +28,12 @@
 requests = "^2.25.1"
 cryptography = "^38.0.4"
 PyJWT = "2.4.0"
 
 [tool.poetry.dev-dependencies]
 mock = "^4.0.3"
 pytest = "^6.2.3"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `umapi_client-3.0/umapi_client/__init__.py` & `umapi_client-3.0.1/umapi_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,7 +22,10 @@
 from .auth import JWTAuth, OAuthS2S
 from .connection import Connection
 from .error import BatchError, ClientError, RequestError, ServerError, UnavailableError, ArgumentError
 from .functional import IdentityType, IfAlreadyExistsOption
 from .functional import UserAction, UserQuery, UsersQuery
 from .functional import GroupAction, GroupsQuery
 from .version import __version__
+import logging
+from logging import NullHandler
+logging.getLogger(__name__).addHandler(NullHandler())
```

### Comparing `umapi_client-3.0/umapi_client/api.py` & `umapi_client-3.0.1/umapi_client/api.py`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/umapi_client/auth.py` & `umapi_client-3.0.1/umapi_client/auth.py`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/umapi_client/connection.py` & `umapi_client-3.0.1/umapi_client/connection.py`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/umapi_client/error.py` & `umapi_client-3.0.1/umapi_client/error.py`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/umapi_client/functional.py` & `umapi_client-3.0.1/umapi_client/functional.py`

 * *Files identical despite different names*

### Comparing `umapi_client-3.0/umapi_client/version.py` & `umapi_client-3.0.1/umapi_client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = "3.0"
+__version__ = "3.0.1"
```

### Comparing `umapi_client-3.0/setup.py` & `umapi_client-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['PyJWT==2.4.0', 'cryptography>=38.0.4,<39.0.0', 'requests>=2.25.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'umapi-client',
-    'version': '3.0',
+    'version': '3.0.1',
     'description': 'Client for the User Management API (UMAPI) from Adobe - see https://adobe.ly/2h1pHgV',
-    'long_description': "# umapi-client.py\n\nThis is a Python client for the User Management API from Adobe, aka the\n[UMAPI](https://www.adobe.io/products/usermanagement/docs/gettingstarted.html).\n\nThe User Management API is an Adobe-hosted network service \nwhich provides Adobe Enterprise customers the ability to manage their users.  This\nclient makes it easy to access the UMAPI from a local Python application.\n\nThis client is open source, maintained by Adobe, and distributed under the terms\nof the OSI-approved MIT license.  Copyright (c) 2016-2021 Adobe Inc.\n\n# Installation\n\n`umapi-client.py` is published to the Python Packaging Index.\n\nhttps://pypi.org/project/umapi-client/\n\nIt can be installed with pip:\n\n```\n$ pip install umapi-client\n```\n\nOr a dependency manager such as Poetry:\n\n```\n$ poetry add umapi-client\n```\n\n# Building\n\n[Poetry](https://python-poetry.org/) is required to build the package. Follow the instructions documented on\nPoetry's website to install it on your system.\n\n1. Clone this repository\n   ```\n   $ git clone https://github.com/adobe-apiplatform/umapi-client.py\n   $ cd umapi-client.py\n   ```\n\n2. Install dependencies to virtual environment.\n   ```\n   $ poetry install\n   ```\n\n3. The `build` command will create a source package (`.tar.gz`) and a wheel file (`.whl`) in the `dist` directory.\n   ```\n   $ poetry build\n   $ ls dist\n   umapi-client-2.18.tar.gz  umapi_client-2.18-py3-none-any.whl\n   ```\n\n4. Some of the packages required by this module use encryption, and so may\n   require you to do local builds of modules that use SSL.  Typically, this\n   will require you to have a python installed that supports compiling\n   extensions.\n\n5. Run tests with `pytest`.\n   ```\n   $ poetry run pytest\n   ```\n\n# Usage\n\nUsage documentation, as well as information about how to get client\ncredentials for use of the UMAPI, can be found in the\n[user guide](https://adobe-apiplatform.github.io/umapi-client.py/),\nwhose sources are in the `docs` directory of this repository.\n\n# License\n\nThis project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.\n",
+    'long_description': "# umapi-client.py\n\nThis is a Python client for the User Management API from Adobe, aka the\n[UMAPI](https://www.adobe.io/products/usermanagement/docs/gettingstarted.html).\n\nThe User Management API is an Adobe-hosted network service which provides Adobe\nEnterprise customers the ability to manage their users. This client makes it\neasy to access the UMAPI from a local Python application.\n\nSee the [user guide](https://adobe-apiplatform.github.io/umapi-client.py/) for\nmore information.\n\nThis client is open source, maintained by Adobe, and distributed under the terms\nof the OSI-approved MIT license. Copyright (c) 2016-2023 Adobe Inc.\n\n# Compatibility\n\nThe `3.x` release branch is actively maintained. New users of the UMAPI client\nshould use the latest 3.x release. The `2.x` branch is still supported, but new\n2.x releases will only contain bug fixes. New features will only be developed\nfor 3.x.\n\nPull requests for 3.x should be made against the `v3` branch (the default\nbranch). Anything related to 2.x bugfixes should target `v2`.\n\n# Installation\n\n`umapi-client.py` is published to the Python Packaging Index.\n\nhttps://pypi.org/project/umapi-client/\n\nIt can be installed with pip:\n\n```\n$ pip install umapi-client\n```\n\nOr a dependency manager such as Poetry:\n\n```\n$ poetry add umapi-client\n```\n\n# Building\n\n[Poetry](https://python-poetry.org/) is required to build the package. Follow\nthe instructions documented on Poetry's website to install it on your system.\n\n1. Clone this repository\n   ```\n   $ git clone https://github.com/adobe-apiplatform/umapi-client.py\n   $ cd umapi-client.py\n   ```\n\n2. Install dependencies to virtual environment.\n   ```\n   $ poetry install\n   ```\n\n3. The `build` command will create a source package (`.tar.gz`) and a wheel file\n   (`.whl`) in the `dist` directory.\n\n   ```\n   $ poetry build\n   $ ls dist\n   umapi-client-3.0.1.tar.gz  umapi_client-3.0.1-py3-none-any.whl\n   ```\n\n4. Some of the packages required by this module use encryption, and so may\n   require you to do local builds of modules that use SSL. Typically, this will\n   require you to have a python installed that supports compiling extensions.\n\n5. Run tests with `pytest`.\n   ```\n   $ poetry run pytest\n   ```\n\n# Usage\n\nUsage documentation, as well as information about how to get client\ncredentials for use of the UMAPI, can be found in the\n[user guide](https://adobe-apiplatform.github.io/umapi-client.py/),\nwhose sources are in the `docs` directory of this repository.\n\n# License\n\nThis project is licensed under the MIT License. See [LICENSE](LICENSE) for more\ninformation.\n",
     'author': 'Andrew Dorton',
     'author_email': 'adorton@adobe.com',
     'maintainer': 'Andrew Dorton',
     'maintainer_email': 'adorton@adobe.com',
     'url': 'https://github.com/adobe-apiplatform/umapi-client.py/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `umapi_client-3.0/PKG-INFO` & `umapi_client-3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umapi-client
-Version: 3.0
+Version: 3.0.1
 Summary: Client for the User Management API (UMAPI) from Adobe - see https://adobe.ly/2h1pHgV
 Home-page: https://github.com/adobe-apiplatform/umapi-client.py/
 License: MIT
 Author: Andrew Dorton
 Author-email: adorton@adobe.com
 Maintainer: Andrew Dorton
 Maintainer-email: adorton@adobe.com
@@ -32,20 +32,33 @@
 Description-Content-Type: text/markdown
 
 # umapi-client.py
 
 This is a Python client for the User Management API from Adobe, aka the
 [UMAPI](https://www.adobe.io/products/usermanagement/docs/gettingstarted.html).
 
-The User Management API is an Adobe-hosted network service 
-which provides Adobe Enterprise customers the ability to manage their users.  This
-client makes it easy to access the UMAPI from a local Python application.
+The User Management API is an Adobe-hosted network service which provides Adobe
+Enterprise customers the ability to manage their users. This client makes it
+easy to access the UMAPI from a local Python application.
+
+See the [user guide](https://adobe-apiplatform.github.io/umapi-client.py/) for
+more information.
 
 This client is open source, maintained by Adobe, and distributed under the terms
-of the OSI-approved MIT license.  Copyright (c) 2016-2021 Adobe Inc.
+of the OSI-approved MIT license. Copyright (c) 2016-2023 Adobe Inc.
+
+# Compatibility
+
+The `3.x` release branch is actively maintained. New users of the UMAPI client
+should use the latest 3.x release. The `2.x` branch is still supported, but new
+2.x releases will only contain bug fixes. New features will only be developed
+for 3.x.
+
+Pull requests for 3.x should be made against the `v3` branch (the default
+branch). Anything related to 2.x bugfixes should target `v2`.
 
 # Installation
 
 `umapi-client.py` is published to the Python Packaging Index.
 
 https://pypi.org/project/umapi-client/
 
@@ -59,39 +72,40 @@
 
 ```
 $ poetry add umapi-client
 ```
 
 # Building
 
-[Poetry](https://python-poetry.org/) is required to build the package. Follow the instructions documented on
-Poetry's website to install it on your system.
+[Poetry](https://python-poetry.org/) is required to build the package. Follow
+the instructions documented on Poetry's website to install it on your system.
 
 1. Clone this repository
    ```
    $ git clone https://github.com/adobe-apiplatform/umapi-client.py
    $ cd umapi-client.py
    ```
 
 2. Install dependencies to virtual environment.
    ```
    $ poetry install
    ```
 
-3. The `build` command will create a source package (`.tar.gz`) and a wheel file (`.whl`) in the `dist` directory.
+3. The `build` command will create a source package (`.tar.gz`) and a wheel file
+   (`.whl`) in the `dist` directory.
+
    ```
    $ poetry build
    $ ls dist
-   umapi-client-2.18.tar.gz  umapi_client-2.18-py3-none-any.whl
+   umapi-client-3.0.1.tar.gz  umapi_client-3.0.1-py3-none-any.whl
    ```
 
 4. Some of the packages required by this module use encryption, and so may
-   require you to do local builds of modules that use SSL.  Typically, this
-   will require you to have a python installed that supports compiling
-   extensions.
+   require you to do local builds of modules that use SSL. Typically, this will
+   require you to have a python installed that supports compiling extensions.
 
 5. Run tests with `pytest`.
    ```
    $ poetry run pytest
    ```
 
 # Usage
@@ -99,9 +113,10 @@
 Usage documentation, as well as information about how to get client
 credentials for use of the UMAPI, can be found in the
 [user guide](https://adobe-apiplatform.github.io/umapi-client.py/),
 whose sources are in the `docs` directory of this repository.
 
 # License
 
-This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
+This project is licensed under the MIT License. See [LICENSE](LICENSE) for more
+information.
```

