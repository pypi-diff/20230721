# Comparing `tmp/iitkgp_erp_login-2.0.1.tar.gz` & `tmp/iitkgp_erp_login-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-2.0.1.tar", last modified: Thu Jul 20 10:13:30 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-2.1.0.tar", last modified: Fri Jul 21 18:50:11 2023, max compression
```

## Comparing `iitkgp_erp_login-2.0.1.tar` & `iitkgp_erp_login-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.803556 iitkgp_erp_login-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-20 10:13:21.000000 iitkgp_erp_login-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:13:30.803556 iitkgp_erp_login-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-20 10:11:48.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/read_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:13:30.799556 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 10:13:30.000000 iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:50:11.491102 iitkgp_erp_login-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-07-21 18:50:11.491102 iitkgp_erp_login-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 18:49:46.000000 iitkgp_erp_login-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:50:11.491102 iitkgp_erp_login-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:50:11.487102 iitkgp_erp_login-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:50:11.487102 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/read_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-21 18:49:16.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:50:11.491102 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-07-21 18:50:11.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 18:50:11.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:50:11.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-21 18:50:11.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 18:50:11.000000 iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/top_level.txt
```

### Comparing `iitkgp_erp_login-2.0.1/LICENSE` & `iitkgp_erp_login-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.0.1/PKG-INFO` & `iitkgp_erp_login-2.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,156 @@
-Metadata-Version: 2.1
-Name: iitkgp_erp_login
-Version: 2.0.1
-Summary: A package to automate login process in ERP for IIT-KGP
-Author-email: Arpit Bhardwaj <proffapt@pm.me>
-Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
-Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ERP Login Module
 
-A python package/module to automate login process in ERP for IIT-KGP.
+Introducing <b>iitkgp-erp-login</b>: Your Ultimate ERP Login Automation Module for IIT-KGP!
+
+Tired of the tedious ERP login process at IIT-Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say goodbye to all of these problems with iitkgp-erp-login, the all-in-one Python package designed to streamline your ERP login experience!
+
+Key Features:
+
+- Seamless OTP & Credentials Handling
+- Effortless Session & ssoToken Management
+- Smart Token Storage for Efficiency
+
+> **Note** This package is not officially affiliated with IIT Kharagpur.
 
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
+	- <a href="#utility-functions">Utility Functions</a>
+		- <a href="#get-import-location">Get import location</a>
+		- <a href="#generate-token">Generate Token</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
+   - <a href="#ssotoken-alive">ssoToken status check</a>
+      - <a href="#ssotoken-alive-input">Input</a>
+      - <a href="#ssotoken-alive-output">Output</a>
+      - <a href="#ssotoken-alive-usage">Usage</a>
 - <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
-   └── read_mail.py
+   ├── read_mail.py
+   └── utils.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+The [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+
+<div id="utility-functions"></div>
+
+### Utility Functions
+
+In the [utility.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some helper functions that are utilized in the module and made available for _you_ to use.
+
+<div id="generate-token"></div>
+
+#### Generate Token
+
+| Input | None |
+|---|---|
+| Output | Generates the `token.json` file from `credentials.json` file for Gmail enabled Google API |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.generate_token()` |
+
+<div id="get-import-locatioin"></div>
+
+#### Get Import Location
+
+| Input | None |
+|---|---|
+| Output | The full path to the directory where the Python file exists in which this module is imported |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.get_import_location()` |
+
+> This is useful when one wants to make a script that can be called from _anywhere_ in the system.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
+
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
 - `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
+
 ```python
 from iitkgp_erp_login.endpoints import *
 
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False, SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
+
 The function requires following _compulsory_ arguments:
+
 1. `headers`: Headers for the post requests.
-    ```python
-    headers = {
-       'timeout': '20',
-       'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
-    }
-    ``` 
-2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+   ```python
+   headers = {
+      'timeout': '20',
+      'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+   }
+   ```
+2. `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+
+   ```python
+   import requests
 
-    session = requests.Session()
-    ```
+   session = requests.Session()
+   ```
 
 The function can also be provided with these _optional_ arguments:
 
 <div id="erpcreds"></div>
 
 1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user is prompted to enter their credentials manually |
     | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
 
     > **Note** Here, `credentials` refer to the roll number, password, and security question.
+
     <details>
       <summary><b>Prerequisites - ERP credentials file</b></summary>
       
     - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
     - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
       - You can choose any valid name for the file, adhering to Python's naming conventions.
       - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
@@ -126,75 +162,85 @@
             "Q1" : "A1",
             "Q2" : "A2",
             "Q3" : "A3",
         }
         ```
       
     </details>
-    
+
 <div id="token"></div>
     
-2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+2.  `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API continuously checks for new OTP emails.
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user will be prompted to manually enter the received OTP |
     | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
   
     <details>
       <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
 
     The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
 
     1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
        > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
     2. To generate the `token.json` file, follow the steps below:
-        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-        - Import the required module, `google-auth-oauthlib`
-      
+        - Import this module
+
           ```bash
-          pip install google-auth-oauthlib
+          pip install iitkgp-erp-login
           ```
-        - Execute `gentokenjson.py` with the `readonly` argument
-   
+        - Execute following command:
+
           ```bash
-          python3 gentokenjson.py readonly
+          python3 -c "from iitkgp_erp_login.utils import generate_token; generate_token()"	
           ```
         - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
         - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
            - Click on `Continue` instead of __Back To Safety__
            - Then, press `Continue` again
         - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
+
         > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 3.  `LOGGING`: Toggles **comprehensive logging**.
     | Default value | `False` |
     |---|---|
     | NOT Specified | No Logging |
     | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
-    
+
+4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and `ssoToken` -  collectively referred to as "session tokens" here  - are stored for direct usage.
+    | Default value | `None` |
+    |---|---|
+    | NOT Specified | The session tokens will not be stored in a file |
+    | Specified (`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in `.session` file for later direct usage |
+
+    > **Note** The approximate expiry time for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
+
 <div id="login-output"></div>
 
 #### Output
+
 1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
 2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
+
 It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -204,61 +250,77 @@
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, session)
-# Credentials: Manual | OTP: Manual | Logging: No
+# Credentials: Manual | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
-# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
-# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
-# Credentials: Manual | OTP: Manual | Logging: Yes
+# Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: in .session file
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in .session file
 ```
 
+
+> **Note** These are just examples of how to use the _login_ function.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
 <div id="session-alive"></div>
 
 ### Session status check
+
 The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
+
 The function requires following argument:
 
- -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+- `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+  ```python
+  import requests
+
+  session = requests.Session()
+  ```
 
-    session = requests.Session()
-     ```
 <div id="session-alive-output"></div>
 
 #### Output
+
 The `session_alive(session)` function returns the status of the session as a boolean value:
 | Status | Return Value |
 | ------ | :------------: |
-| Valid (`Alive`)  | `True` |
+| Valid (`Alive`) | `True` |
 | Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
+
 It is recommended to use the `session_alive` function in the following manner:
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
@@ -281,32 +343,117 @@
 
 session = requests.Session()
 
 print("Logging into ERP for:", creds.ROLL_NUMBER)
 
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** This is just a sample code demonstrating the usage of `session_alive` along with other _variables_ to get the function working.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
+<div id="ssotoken-alive"></div>
+
+### ssoToken status check
+
+The logic for checking the validity of the ssoToken is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+
+<div id="ssotoken-alive-input"></div>
+
+#### Input
+
+The function requires following argument:
+
+- `ssoToken`: The second returned value from the `login` function.
+  ```python # Importing the erp.py file
+  import iitkgp_erp_login.erp as erp
+
+  # Using the login function inside erp.py - all others are optional arguments
+  _, ssoToken = erp.login(headers, session)
+  ```
+
+<div id="ssotoken-alive-output"></div>
+
+#### Output
+
+The `ssotoken_valid(ssoToken)` function returns the validity status of the ssotoken as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid | `True` |
+| Not Valid | `False` |
+
+<div id="ssotoken-alive-usage"></div>
+
+#### Usage
+
+It is recommended to use the `ssotoken_valid` function in the following manner:
+
+```python
+# Importing the erp.py file
+import iitkgp_erp_login.erp as erp
+
+# Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken))
+```
+
+Here's an example combining all the aspects we have discussed so far about the `login` function and `ssotoken_valid` function. <br>
+This code can be used to log in to the ERP system while storing the ssoToken. If the ssoToken remains valid, it can be used directly for subsequent logins, eliminating the need to re-authenticate each time:
+
+```python
+import webbrowser
+import requests
+import time
+
+import creds
+# Importing creds.py, which contains ERP credentials
+
+import iitkgp_erp_login.erp as erp
+
+headers = {
+    'timeout': '20',
+    'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+}
+session = requests.Session()
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
+if os.path.exists(".session"):
+    with open(".session", "r") as file:
+        ssoToken = file.read()
+    if not erp.ssotoken_valid(ssoToken):
+        _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+        with open(".session", "w") as file:
+            file.write(ssoToken)
+else:
+    _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+    with open(".session", "w") as file:
+        file.write(ssoToken)
+
+logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
+webbrowser.open(logged_in_url)
+```
+> **Note** This is merely a Proof of Concept example; this exact functionality has been integrated into the login function itself from version **2.1.0** onwards.
+
 <div id="example"></div>
 
 ## Example
 
 Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
-   pip install iitkgp_erp_login
-   ````
+   pip install iitkgp-erp-login
+   ```
+
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
 3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
@@ -317,16 +464,17 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=".session")
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
+
 4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,47 +1,61 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.0.1 Summary: A package
-to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
-pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
-Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # ERP Login Module A python package/module to automate login process in
-ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
-Login - Input - Output - Usage - Session_status_check - Input - Output - Usage
-- Example
+# ERP Login Module Introducing iitkgp-erp-login: Your Ultimate ERP Login
+Automation Module for IIT-KGP! Tired of the tedious ERP login process at IIT-
+Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say goodbye
+to all of these problems with iitkgp-erp-login, the all-in-one Python package
+designed to streamline your ERP login experience! Key Features: - Seamless OTP
+& Credentials Handling - Effortless Session & ssoToken Management - Smart Token
+Storage for Efficiency > **Note** This package is not officially affiliated
+with IIT Kharagpur.  Table of Contents - Description - Utility_Functions - Get
+import_location - Generate_Token - Endpoints - About - Usage - Login - Input -
+Output - Usage - Session_status_check - Input - Output - Usage - ssoToken
+status_check - Input - Output - Usage - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
-erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
-helper functions. These functions are not intended to be used by _you_, the
-user. The only case where OTP is required is during the login process, which is
-handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
-abstraction for general users. If you want to modify the OTP fetching process,
-feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+erp.py âââ read_mail.py âââ utils.py ``` The [read_mail.py](https:/
+/github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)`
+function, along with various helper functions. These functions are not intended
+to be used by _you_, the user. The only case where OTP is required is during
+the login process, which is handled by function in [erp.py](https://github.com/
+proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence,
+let this script serve as an abstraction for general users. If you want to
+modify the OTP fetching process, feel free to refer to the [read_mail.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/read_mail.py) script.
+### Utility Functions In the [utility.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some
+helper functions that are utilized in the module and made available for _you_
+to use.
+#### Generate Token | Input | None | |---|---| | Output | Generates the
+`token.json` file from `credentials.json` file for Gmail enabled Google API | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.generate_token()` |
+#### Get Import Location | Input | None | |---|---| | Output | The full path to
+the directory where the Python file exists in which this module is imported | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.get_import_location()` | > This is useful when one wants to make a
+script that can be called from _anywhere_ in the system.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
 ### Login ERP login workflow is implemented in `login(headers, session,
-ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/erp.py). The input and output specifications for the function
-are mentioned below.
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False,
+SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following _compulsory_ arguments: 1.
 `headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 ``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) object, to persist the session parameters
 throughout the workflow. ```python import requests session = requests.Session()
@@ -57,69 +71,85 @@
 - Create a `.py` file with your ERP credentials stored in it. Please follow the
 instructions below to create this file: - You can choose any valid name for the
 file, adhering to Python's naming conventions. - **Do not change the variable
 names**. Copy the format provided below & update the values inside the `double
 quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
 "**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
 "A3", } ```
-2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+2. `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API
 continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
 NOT Specified | The user will be prompted to manually enter the received OTP |
 | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
 checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
 The token file **MUST** be present in the same directory as the script where
 `iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
 API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
 python) guide to obtain `credentials.json` file. > **Note** The
 `credentials.json` file is permanent unless you manually delete its reference
 in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
-logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
-| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+steps below: - Import this module ```bash pip install iitkgp-erp-login ``` -
+Execute following command: ```bash python3 -c "from iitkgp_erp_login.utils
+import generate_token; generate_token()" ``` - A browser window will open,
+prompting you to select the Google account associated with receiving OTP for
+login. - Grant permission to the selected email address to utilize the newly
+enabled **Gmail API**. - Click on `Continue` instead of __Back To Safety__ -
+Then, press `Continue` again - The `token.json` file will be generated in the
+same folder as the `credentials.json` file > **Warning** The `token.json` file
+has an expiration time, so it's important to periodically check and refresh it
+in your projects to ensure uninterrupted access. 3. `LOGGING`: Toggles
+**comprehensive logging**. | Default value | `False` | |---|---| | NOT
+Specified | No Logging | | Specified (`LOGGING=True`) | Logs every step in an
+exhaustive manner | 4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and
+`ssoToken` - collectively referred to as "session tokens" here - are stored for
+direct usage. | Default value | `None` | |---|---| | NOT Specified | The
+session tokens will not be stored in a file | | Specified
+(`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in
+`.session` file for later direct usage | > **Note** The approximate expiry time
+for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
 #### Output 1. The function returns the following, in the order of occurrence
 as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
 en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
 Single_sign-on) 2. It also modifies the `session` object, which now includes
 parameters for the logged-in session. This `session` object can be utilized for
 further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
 manner (optional arguments are _your_ choice): ```python # Importing the erp.py
 file import iitkgp_erp_login.erp as erp # Using the login function inside
 erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
-OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
-aspects we have discussed so far about the `login` function: ```python import
-requests import erpcreds import iitkgp_erp_login.erp as erp headers =
-{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
-537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
-Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
-erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
-Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
-Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
-Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
-erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
-Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
-seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
-- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
-```
+OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None) ``` Here's an
+example combining all the aspects we have discussed so far about the `login`
+function: ```python import requests import erpcreds import iitkgp_erp_login.erp
+as erp headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux
+x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79
+Chrome/51.0.2704.79 Safari/537.36', } session = requests.Session()
+sessionToken, ssoToken = erp.login(headers, session) # Credentials: Manual |
+OTP: Manual | Logging: No | TokenStorage: No sessionToken, ssoToken = erp.login
+(headers, session, ERPCREDS=erpcreds) # Credentials: Automatic - from
+erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No sessionToken,
+ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) # Credentials:
+Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage:
+No sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=5) # Credentials: Automatic - from erpcreds.py | OTP:
+Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic - from erpcreds.py
+| OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session') # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No |
+TokenStorage: in .session file sessionToken, ssoToken = erp.login(headers,
+session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE='.session') # Credentials: Automatic - from erpcreds.py |
+OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in
+.session file ``` > **Note** These are just examples of how to use the _login_
+function. >> Some arguments of `login()` have their own prerequisites that must
+be satisfied in order to use them. See "Input"_section_of_login for complete
+details.
 ### Session status check The logic for checking the status of the session is
 implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
@@ -135,22 +165,63 @@
 aspects we have discussed so far about the `login` function and `session_alive`
 function: ```python import requests import time import creds # Importing
 creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
 headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
 AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
 51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
 ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
-erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
-else: print("Session is alive.") time.sleep(2) ```
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ``` > **Note** This is just a
+sample code demonstrating the usage of `session_alive` along with other
+_variables_ to get the function working. >> Some arguments of `login()` have
+their own prerequisites that must be satisfied in order to use them. See
+"Input"_section_of_login for complete details.
+### ssoToken status check The logic for checking the validity of the ssoToken
+is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). The input and output specifications for the function are mentioned
+below.
+#### Input The function requires following argument: - `ssoToken`: The second
+returned value from the `login` function. ```python # Importing the erp.py file
+import iitkgp_erp_login.erp as erp # Using the login function inside erp.py -
+all others are optional arguments _, ssoToken = erp.login(headers, session) ```
+#### Output The `ssotoken_valid(ssoToken)` function returns the validity status
+of the ssotoken as a boolean value: | Status | Return Value | | ------ | :-----
+-------: | | Valid | `True` | | Not Valid | `False` |
+#### Usage It is recommended to use the `ssotoken_valid` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and
+`ssotoken_valid` function.
+This code can be used to log in to the ERP system while storing the ssoToken.
+If the ssoToken remains valid, it can be used directly for subsequent logins,
+eliminating the need to re-authenticate each time: ```python import webbrowser
+import requests import time import creds # Importing creds.py, which contains
+ERP credentials import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() print("Logging into ERP for:", creds.ROLL_NUMBER)
+if os.path.exists(".session"): with open(".session", "r") as file: ssoToken =
+file.read() if not erp.ssotoken_valid(ssoToken): _, ssoToken = erp.login
+(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True) with
+open(".session", "w") as file: file.write(ssoToken) else: _, ssoToken =
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+with open(".session", "w") as file: file.write(ssoToken) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` >
+**Note** This is merely a Proof of Concept example; this exact functionality
+has been integrated into the login function itself from version **2.1.0**
+onwards.
 ## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
-install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+install iitkgp-erp-login ``` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
-{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
-the script. ```bash python3 open_erp.py ```
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE=".session") logged_in_url = f"{HOMEPAGE_URL}?ssoToken=
+{ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run the script. ```bash
+python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-2.0.1/README.md` & `iitkgp_erp_login-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,170 @@
+Metadata-Version: 2.1
+Name: iitkgp_erp_login
+Version: 2.1.0
+Summary: A package to automate login process in ERP for IIT-KGP
+Author-email: Arpit Bhardwaj <proffapt@pm.me>
+Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
+Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ERP Login Module
 
-A python package/module to automate login process in ERP for IIT-KGP.
+Introducing <b>iitkgp-erp-login</b>: Your Ultimate ERP Login Automation Module for IIT-KGP!
+
+Tired of the tedious ERP login process at IIT-Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say goodbye to all of these problems with iitkgp-erp-login, the all-in-one Python package designed to streamline your ERP login experience!
+
+Key Features:
+
+- Seamless OTP & Credentials Handling
+- Effortless Session & ssoToken Management
+- Smart Token Storage for Efficiency
+
+> **Note** This package is not officially affiliated with IIT Kharagpur.
 
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
+	- <a href="#utility-functions">Utility Functions</a>
+		- <a href="#get-import-location">Get import location</a>
+		- <a href="#generate-token">Generate Token</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
+   - <a href="#ssotoken-alive">ssoToken status check</a>
+      - <a href="#ssotoken-alive-input">Input</a>
+      - <a href="#ssotoken-alive-output">Output</a>
+      - <a href="#ssotoken-alive-usage">Usage</a>
 - <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
-   └── read_mail.py
+   ├── read_mail.py
+   └── utils.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+The [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+
+<div id="utility-functions"></div>
+
+### Utility Functions
+
+In the [utility.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some helper functions that are utilized in the module and made available for _you_ to use.
+
+<div id="generate-token"></div>
+
+#### Generate Token
+
+| Input | None |
+|---|---|
+| Output | Generates the `token.json` file from `credentials.json` file for Gmail enabled Google API |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.generate_token()` |
+
+<div id="get-import-locatioin"></div>
+
+#### Get Import Location
+
+| Input | None |
+|---|---|
+| Output | The full path to the directory where the Python file exists in which this module is imported |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.get_import_location()` |
+
+> This is useful when one wants to make a script that can be called from _anywhere_ in the system.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
+
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
 - `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
+
 ```python
 from iitkgp_erp_login.endpoints import *
 
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False, SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
+
 The function requires following _compulsory_ arguments:
+
 1. `headers`: Headers for the post requests.
-    ```python
-    headers = {
-       'timeout': '20',
-       'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
-    }
-    ``` 
-2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+   ```python
+   headers = {
+      'timeout': '20',
+      'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+   }
+   ```
+2. `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+
+   ```python
+   import requests
 
-    session = requests.Session()
-    ```
+   session = requests.Session()
+   ```
 
 The function can also be provided with these _optional_ arguments:
 
 <div id="erpcreds"></div>
 
 1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user is prompted to enter their credentials manually |
     | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
 
     > **Note** Here, `credentials` refer to the roll number, password, and security question.
+
     <details>
       <summary><b>Prerequisites - ERP credentials file</b></summary>
       
     - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
     - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
       - You can choose any valid name for the file, adhering to Python's naming conventions.
       - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
@@ -112,75 +176,85 @@
             "Q1" : "A1",
             "Q2" : "A2",
             "Q3" : "A3",
         }
         ```
       
     </details>
-    
+
 <div id="token"></div>
     
-2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+2.  `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API continuously checks for new OTP emails.
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user will be prompted to manually enter the received OTP |
     | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
   
     <details>
       <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
 
     The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
 
     1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
        > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
     2. To generate the `token.json` file, follow the steps below:
-        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-        - Import the required module, `google-auth-oauthlib`
-      
+        - Import this module
+
           ```bash
-          pip install google-auth-oauthlib
+          pip install iitkgp-erp-login
           ```
-        - Execute `gentokenjson.py` with the `readonly` argument
-   
+        - Execute following command:
+
           ```bash
-          python3 gentokenjson.py readonly
+          python3 -c "from iitkgp_erp_login.utils import generate_token; generate_token()"	
           ```
         - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
         - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
            - Click on `Continue` instead of __Back To Safety__
            - Then, press `Continue` again
         - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
+
         > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 3.  `LOGGING`: Toggles **comprehensive logging**.
     | Default value | `False` |
     |---|---|
     | NOT Specified | No Logging |
     | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
-    
+
+4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and `ssoToken` -  collectively referred to as "session tokens" here  - are stored for direct usage.
+    | Default value | `None` |
+    |---|---|
+    | NOT Specified | The session tokens will not be stored in a file |
+    | Specified (`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in `.session` file for later direct usage |
+
+    > **Note** The approximate expiry time for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
+
 <div id="login-output"></div>
 
 #### Output
+
 1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
 2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
+
 It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -190,61 +264,77 @@
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, session)
-# Credentials: Manual | OTP: Manual | Logging: No
+# Credentials: Manual | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
-# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
-# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
-# Credentials: Manual | OTP: Manual | Logging: Yes
+# Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: in .session file
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in .session file
 ```
 
+
+> **Note** These are just examples of how to use the _login_ function.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
 <div id="session-alive"></div>
 
 ### Session status check
+
 The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
+
 The function requires following argument:
 
- -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+- `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+  ```python
+  import requests
+
+  session = requests.Session()
+  ```
 
-    session = requests.Session()
-     ```
 <div id="session-alive-output"></div>
 
 #### Output
+
 The `session_alive(session)` function returns the status of the session as a boolean value:
 | Status | Return Value |
 | ------ | :------------: |
-| Valid (`Alive`)  | `True` |
+| Valid (`Alive`) | `True` |
 | Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
+
 It is recommended to use the `session_alive` function in the following manner:
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
@@ -267,32 +357,117 @@
 
 session = requests.Session()
 
 print("Logging into ERP for:", creds.ROLL_NUMBER)
 
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** This is just a sample code demonstrating the usage of `session_alive` along with other _variables_ to get the function working.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
+<div id="ssotoken-alive"></div>
+
+### ssoToken status check
+
+The logic for checking the validity of the ssoToken is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+
+<div id="ssotoken-alive-input"></div>
+
+#### Input
+
+The function requires following argument:
+
+- `ssoToken`: The second returned value from the `login` function.
+  ```python # Importing the erp.py file
+  import iitkgp_erp_login.erp as erp
+
+  # Using the login function inside erp.py - all others are optional arguments
+  _, ssoToken = erp.login(headers, session)
+  ```
+
+<div id="ssotoken-alive-output"></div>
+
+#### Output
+
+The `ssotoken_valid(ssoToken)` function returns the validity status of the ssotoken as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid | `True` |
+| Not Valid | `False` |
+
+<div id="ssotoken-alive-usage"></div>
+
+#### Usage
+
+It is recommended to use the `ssotoken_valid` function in the following manner:
+
+```python
+# Importing the erp.py file
+import iitkgp_erp_login.erp as erp
+
+# Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken))
+```
+
+Here's an example combining all the aspects we have discussed so far about the `login` function and `ssotoken_valid` function. <br>
+This code can be used to log in to the ERP system while storing the ssoToken. If the ssoToken remains valid, it can be used directly for subsequent logins, eliminating the need to re-authenticate each time:
+
+```python
+import webbrowser
+import requests
+import time
+
+import creds
+# Importing creds.py, which contains ERP credentials
+
+import iitkgp_erp_login.erp as erp
+
+headers = {
+    'timeout': '20',
+    'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+}
+session = requests.Session()
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
+if os.path.exists(".session"):
+    with open(".session", "r") as file:
+        ssoToken = file.read()
+    if not erp.ssotoken_valid(ssoToken):
+        _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+        with open(".session", "w") as file:
+            file.write(ssoToken)
+else:
+    _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+    with open(".session", "w") as file:
+        file.write(ssoToken)
+
+logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
+webbrowser.open(logged_in_url)
+```
+> **Note** This is merely a Proof of Concept example; this exact functionality has been integrated into the login function itself from version **2.1.0** onwards.
+
 <div id="example"></div>
 
 ## Example
 
 Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
-   pip install iitkgp_erp_login
-   ````
+   pip install iitkgp-erp-login
+   ```
+
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
 3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
@@ -303,16 +478,17 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=".session")
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
+
 4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,40 +1,68 @@
-# ERP Login Module A python package/module to automate login process in ERP for
-IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage - Login -
-Input - Output - Usage - Session_status_check - Input - Output - Usage -
-Example
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.1.0 Summary: A package
+to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
+pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
+Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # ERP Login Module Introducing iitkgp-erp-login: Your Ultimate ERP
+Login Automation Module for IIT-KGP! Tired of the tedious ERP login process at
+IIT-Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say
+goodbye to all of these problems with iitkgp-erp-login, the all-in-one Python
+package designed to streamline your ERP login experience! Key Features: -
+Seamless OTP & Credentials Handling - Effortless Session & ssoToken Management
+- Smart Token Storage for Efficiency > **Note** This package is not officially
+affiliated with IIT Kharagpur.  Table of Contents - Description - Utility
+Functions - Get_import_location - Generate_Token - Endpoints - About - Usage -
+Login - Input - Output - Usage - Session_status_check - Input - Output - Usage
+- ssoToken_status_check - Input - Output - Usage - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
-erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
-helper functions. These functions are not intended to be used by _you_, the
-user. The only case where OTP is required is during the login process, which is
-handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
-abstraction for general users. If you want to modify the OTP fetching process,
-feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+erp.py âââ read_mail.py âââ utils.py ``` The [read_mail.py](https:/
+/github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)`
+function, along with various helper functions. These functions are not intended
+to be used by _you_, the user. The only case where OTP is required is during
+the login process, which is handled by function in [erp.py](https://github.com/
+proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence,
+let this script serve as an abstraction for general users. If you want to
+modify the OTP fetching process, feel free to refer to the [read_mail.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/read_mail.py) script.
+### Utility Functions In the [utility.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some
+helper functions that are utilized in the module and made available for _you_
+to use.
+#### Generate Token | Input | None | |---|---| | Output | Generates the
+`token.json` file from `credentials.json` file for Gmail enabled Google API | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.generate_token()` |
+#### Get Import Location | Input | None | |---|---| | Output | The full path to
+the directory where the Python file exists in which this module is imported | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.get_import_location()` | > This is useful when one wants to make a
+script that can be called from _anywhere_ in the system.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
 ### Login ERP login workflow is implemented in `login(headers, session,
-ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/erp.py). The input and output specifications for the function
-are mentioned below.
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False,
+SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following _compulsory_ arguments: 1.
 `headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 ``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) object, to persist the session parameters
 throughout the workflow. ```python import requests session = requests.Session()
@@ -50,69 +78,85 @@
 - Create a `.py` file with your ERP credentials stored in it. Please follow the
 instructions below to create this file: - You can choose any valid name for the
 file, adhering to Python's naming conventions. - **Do not change the variable
 names**. Copy the format provided below & update the values inside the `double
 quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
 "**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
 "A3", } ```
-2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+2. `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API
 continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
 NOT Specified | The user will be prompted to manually enter the received OTP |
 | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
 checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
 The token file **MUST** be present in the same directory as the script where
 `iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
 API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
 python) guide to obtain `credentials.json` file. > **Note** The
 `credentials.json` file is permanent unless you manually delete its reference
 in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
-logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
-| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+steps below: - Import this module ```bash pip install iitkgp-erp-login ``` -
+Execute following command: ```bash python3 -c "from iitkgp_erp_login.utils
+import generate_token; generate_token()" ``` - A browser window will open,
+prompting you to select the Google account associated with receiving OTP for
+login. - Grant permission to the selected email address to utilize the newly
+enabled **Gmail API**. - Click on `Continue` instead of __Back To Safety__ -
+Then, press `Continue` again - The `token.json` file will be generated in the
+same folder as the `credentials.json` file > **Warning** The `token.json` file
+has an expiration time, so it's important to periodically check and refresh it
+in your projects to ensure uninterrupted access. 3. `LOGGING`: Toggles
+**comprehensive logging**. | Default value | `False` | |---|---| | NOT
+Specified | No Logging | | Specified (`LOGGING=True`) | Logs every step in an
+exhaustive manner | 4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and
+`ssoToken` - collectively referred to as "session tokens" here - are stored for
+direct usage. | Default value | `None` | |---|---| | NOT Specified | The
+session tokens will not be stored in a file | | Specified
+(`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in
+`.session` file for later direct usage | > **Note** The approximate expiry time
+for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
 #### Output 1. The function returns the following, in the order of occurrence
 as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
 en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
 Single_sign-on) 2. It also modifies the `session` object, which now includes
 parameters for the logged-in session. This `session` object can be utilized for
 further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
 manner (optional arguments are _your_ choice): ```python # Importing the erp.py
 file import iitkgp_erp_login.erp as erp # Using the login function inside
 erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
-OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
-aspects we have discussed so far about the `login` function: ```python import
-requests import erpcreds import iitkgp_erp_login.erp as erp headers =
-{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
-537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
-Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
-erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
-Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
-Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
-Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
-erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
-Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
-seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
-- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
-```
+OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None) ``` Here's an
+example combining all the aspects we have discussed so far about the `login`
+function: ```python import requests import erpcreds import iitkgp_erp_login.erp
+as erp headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux
+x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79
+Chrome/51.0.2704.79 Safari/537.36', } session = requests.Session()
+sessionToken, ssoToken = erp.login(headers, session) # Credentials: Manual |
+OTP: Manual | Logging: No | TokenStorage: No sessionToken, ssoToken = erp.login
+(headers, session, ERPCREDS=erpcreds) # Credentials: Automatic - from
+erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No sessionToken,
+ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) # Credentials:
+Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage:
+No sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=5) # Credentials: Automatic - from erpcreds.py | OTP:
+Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic - from erpcreds.py
+| OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session') # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No |
+TokenStorage: in .session file sessionToken, ssoToken = erp.login(headers,
+session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE='.session') # Credentials: Automatic - from erpcreds.py |
+OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in
+.session file ``` > **Note** These are just examples of how to use the _login_
+function. >> Some arguments of `login()` have their own prerequisites that must
+be satisfied in order to use them. See "Input"_section_of_login for complete
+details.
 ### Session status check The logic for checking the status of the session is
 implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
@@ -128,22 +172,63 @@
 aspects we have discussed so far about the `login` function and `session_alive`
 function: ```python import requests import time import creds # Importing
 creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
 headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
 AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
 51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
 ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
-erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
-else: print("Session is alive.") time.sleep(2) ```
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ``` > **Note** This is just a
+sample code demonstrating the usage of `session_alive` along with other
+_variables_ to get the function working. >> Some arguments of `login()` have
+their own prerequisites that must be satisfied in order to use them. See
+"Input"_section_of_login for complete details.
+### ssoToken status check The logic for checking the validity of the ssoToken
+is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). The input and output specifications for the function are mentioned
+below.
+#### Input The function requires following argument: - `ssoToken`: The second
+returned value from the `login` function. ```python # Importing the erp.py file
+import iitkgp_erp_login.erp as erp # Using the login function inside erp.py -
+all others are optional arguments _, ssoToken = erp.login(headers, session) ```
+#### Output The `ssotoken_valid(ssoToken)` function returns the validity status
+of the ssotoken as a boolean value: | Status | Return Value | | ------ | :-----
+-------: | | Valid | `True` | | Not Valid | `False` |
+#### Usage It is recommended to use the `ssotoken_valid` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and
+`ssotoken_valid` function.
+This code can be used to log in to the ERP system while storing the ssoToken.
+If the ssoToken remains valid, it can be used directly for subsequent logins,
+eliminating the need to re-authenticate each time: ```python import webbrowser
+import requests import time import creds # Importing creds.py, which contains
+ERP credentials import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() print("Logging into ERP for:", creds.ROLL_NUMBER)
+if os.path.exists(".session"): with open(".session", "r") as file: ssoToken =
+file.read() if not erp.ssotoken_valid(ssoToken): _, ssoToken = erp.login
+(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True) with
+open(".session", "w") as file: file.write(ssoToken) else: _, ssoToken =
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+with open(".session", "w") as file: file.write(ssoToken) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` >
+**Note** This is merely a Proof of Concept example; this exact functionality
+has been integrated into the login function itself from version **2.1.0**
+onwards.
 ## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
-install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+install iitkgp-erp-login ``` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
-{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
-the script. ```bash python3 open_erp.py ```
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE=".session") logged_in_url = f"{HOMEPAGE_URL}?ssoToken=
+{ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run the script. ```bash
+python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-2.0.1/pyproject.toml` & `iitkgp_erp_login-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "2.0.1"
+version = "2.1.0"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-2.0.1/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.1.0/src/iitkgp_erp_login/erp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,129 @@
+import os
+import re
+import logging
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from bs4 import BeautifulSoup as bs
-import logging
-import re
 from iitkgp_erp_login.read_mail import getOTP
 from iitkgp_erp_login.endpoints import *
+from iitkgp_erp_login.utils import get_import_location
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 logging.basicConfig(level=logging.INFO)
+sessionToken = ""
 
 class ErpLoginError(Exception):
     pass
 
-def login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False):
-    if ERPCREDS != None:
-        ROLL_NUMBER = ERPCREDS.ROLL_NUMBER
-        PASSWORD = ERPCREDS.PASSWORD
-    else:
-        import getpass
-        ROLL_NUMBER = input("Enter you Roll Number: ")
-        PASSWORD = getpass.getpass("Enter your ERP password: ")
-
-    try:
-        r = session.get(HOMEPAGE_URL)
-        soup = bs(r.text, 'html.parser')
-        sessionToken = soup.find(id='sessionToken')['value']
-        logging.info(" Generated session token") if LOGGING else None
-    except (requests.exceptions.RequestException, KeyError) as e:
-        raise ErpLoginError(f"Failed to generate session token: {str(e)}")
-    
-    try:
-        r = session.post(SECRET_QUESTION_URL, data={'user_id': ROLL_NUMBER}, headers=headers)
-        secret_question = r.text
-        logging.info(" Fetched Security Question") if LOGGING else None
 
-        if ERPCREDS != None:
-            secret_answer = ERPCREDS.SECURITY_QUESTIONS_ANSWERS[secret_question]
-        else:
-            print ("Your secret question: " + secret_question)
-            secret_answer = getpass.getpass("Enter the answer to the secret question: ")
-    except (requests.exceptions.RequestException, KeyError) as e:
-        raise ErpLoginError(f"Failed to fetch Security Question: {str(e)}")
-
-    try:
-        r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER, 'pass': PASSWORD}, headers=headers)
-    except requests.exceptions.RequestException as e:
-        raise ErpLoginError(f"Failed to request OTP: {str(e)}")
-    
-    login_details = {
-        'user_id': ROLL_NUMBER,
-        'password': PASSWORD,
-        'answer': secret_answer,
-        'sessionToken': sessionToken,
-        'requestedUrl': HOMEPAGE_URL,
-    }
+def login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False, SESSION_STORAGE_FILE=None):
+    global sessionToken
+    ssoToken = None
+    if SESSION_STORAGE_FILE:
+        token_file = f"{get_import_location()}/{SESSION_STORAGE_FILE}" if SESSION_STORAGE_FILE else None
+        try:
+            with open(token_file, "r") as file:
+                lines = file.readlines()
+                sessionToken = lines[0].strip() if len(lines) > 0 else None
+                ssoToken = lines[1].strip() if len(lines) > 1 else None
+            logging.info(" Retrieved tokens from the file") if LOGGING else None
+        except (FileNotFoundError, IOError):
+            logging.error(f" Token file doesn't exist") if LOGGING else None
 
-    if r.status_code == 200:
-        logging.info(" Requested OTP") if LOGGING else None
+    if ssoToken and ssotoken_valid(ssoToken):
+        logging.info(" [SSOToken STATUS]: Valid!") if LOGGING else None
+    else:
+        if SESSION_STORAGE_FILE:
+            logging.info(" [SSOToken STATUS]: Not Valid!") if LOGGING and os.path.exists(SESSION_STORAGE_FILE) else None
         
-        if OTP_CHECK_INTERVAL != None:
-                try:
-                    logging.info(" Waiting for OTP...") if LOGGING else None
-                    otp = getOTP(OTP_CHECK_INTERVAL)
-                    logging.info(" Received OTP") if LOGGING else None
-                except Exception as e:
-                    raise ErpLoginError(f"Failed to receive OTP: {str(e)}")
+        if ERPCREDS != None:
+            ROLL_NUMBER = ERPCREDS.ROLL_NUMBER
+            PASSWORD = ERPCREDS.PASSWORD
         else:
-            otp = input("Enter the OTP sent to your registered email address: ").strip()
-            
-        login_details['email_otp'] = otp
-    else:
-        logging.info(" OTP is not required :yay") if LOGGING else None
+            import getpass
+            ROLL_NUMBER = input("Enter you Roll Number: ")
+            PASSWORD = getpass.getpass("Enter your ERP password: ")
+
+        try:
+            r = session.get(HOMEPAGE_URL)
+            soup = bs(r.text, 'html.parser')
+            sessionToken = soup.find(id='sessionToken')['value']
+            logging.info(" Generated sessionToken") if LOGGING else None
+        except (requests.exceptions.RequestException, KeyError) as e:
+            raise ErpLoginError(f"Failed to generate session token: {str(e)}")
+        
+        try:
+            r = session.post(SECRET_QUESTION_URL, data={'user_id': ROLL_NUMBER}, headers=headers)
+            secret_question = r.text
+            logging.info(" Fetched Security Question") if LOGGING else None
+
+            if ERPCREDS != None:
+                secret_answer = ERPCREDS.SECURITY_QUESTIONS_ANSWERS[secret_question]
+            else:
+                print ("Your secret question: " + secret_question)
+                secret_answer = getpass.getpass("Enter the answer to the secret question: ")
+        except (requests.exceptions.RequestException, KeyError) as e:
+            raise ErpLoginError(f"Failed to fetch Security Question: {str(e)}")
+
+        try:
+            r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER, 'pass': PASSWORD}, headers=headers)
+        except requests.exceptions.RequestException as e:
+            raise ErpLoginError(f"Failed to request OTP: {str(e)}")
+        
+        login_details = {
+            'user_id': ROLL_NUMBER,
+            'password': PASSWORD,
+            'answer': secret_answer,
+            'sessionToken': sessionToken,
+            'requestedUrl': HOMEPAGE_URL,
+        }
 
-    try:
-        r = session.post(LOGIN_URL, data=login_details, headers=headers)
-        ssoToken = re.search(r'\?ssoToken=(.+)$', r.history[1].headers['Location'])
-        if ssoToken is None:
-            raise ErpLoginError(f"Failed to generate ssoToken: {str(e)}")
-        ssoToken = ssoToken.group(1)
-        logging.info(" Generated ssoToken") if LOGGING else None
-    except (requests.exceptions.RequestException, IndexError) as e:
-        raise ErpLoginError(f"ERP login failed: {str(e)}")
+        if r.status_code == 200:
+            logging.info(" Requested OTP") if LOGGING else None
+            
+            if OTP_CHECK_INTERVAL != None:
+                    try:
+                        logging.info(" Waiting for OTP...") if LOGGING else None
+                        otp = getOTP(OTP_CHECK_INTERVAL)
+                        logging.info(" Received OTP") if LOGGING else None
+                    except Exception as e:
+                        raise ErpLoginError(f"Failed to receive OTP: {str(e)}")
+            else:
+                otp = input("Enter the OTP sent to your registered email address: ").strip()
+                
+            login_details['email_otp'] = otp
+        else:
+            logging.info(" OTP is not required :yay") if LOGGING else None
 
-    logging.info(" ERP login completed!") if LOGGING else None
+        try:
+            r = session.post(LOGIN_URL, data=login_details, headers=headers)
+            ssoToken = re.search(r'\?ssoToken=(.+)$', r.history[1].headers['Location'])
+            if ssoToken is None:
+                raise ErpLoginError(f"Failed to generate ssoToken: {str(e)}")
+            ssoToken = ssoToken.group(1)
+            logging.info(" Generated ssoToken") if LOGGING else None
+        except (requests.exceptions.RequestException, IndexError) as e:
+            raise ErpLoginError(f"ERP login failed: {str(e)}")
+
+        logging.info(" ERP login completed!") if LOGGING else None
+
+        if SESSION_STORAGE_FILE:
+            with open(token_file, "w") as file:
+                if sessionToken:
+                    file.write(sessionToken + "\n")
+                if ssoToken:
+                    file.write(ssoToken + "\n")
+            logging.info(" Stored tokens in the file") if LOGGING else None
 
     return sessionToken, ssoToken
 
 
 def session_alive(session):
     r = session.get(WELCOMEPAGE_URL)
     return r.status_code == 404
+
+
+def ssotoken_valid(ssoToken):
+    response = requests.get(f"{HOMEPAGE_URL}?ssoToken={ssoToken}")
+    content_type = str(response.headers).split(',')[-1].split("'")[-2]
+    return content_type == 'text/html;charset=UTF-8'
```

### Comparing `iitkgp_erp_login-2.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.1.0/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,170 @@
 Metadata-Version: 2.1
 Name: iitkgp-erp-login
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ERP Login Module
 
-A python package/module to automate login process in ERP for IIT-KGP.
+Introducing <b>iitkgp-erp-login</b>: Your Ultimate ERP Login Automation Module for IIT-KGP!
+
+Tired of the tedious ERP login process at IIT-Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say goodbye to all of these problems with iitkgp-erp-login, the all-in-one Python package designed to streamline your ERP login experience!
+
+Key Features:
+
+- Seamless OTP & Credentials Handling
+- Effortless Session & ssoToken Management
+- Smart Token Storage for Efficiency
+
+> **Note** This package is not officially affiliated with IIT Kharagpur.
 
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
+	- <a href="#utility-functions">Utility Functions</a>
+		- <a href="#get-import-location">Get import location</a>
+		- <a href="#generate-token">Generate Token</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
+   - <a href="#ssotoken-alive">ssoToken status check</a>
+      - <a href="#ssotoken-alive-input">Input</a>
+      - <a href="#ssotoken-alive-output">Output</a>
+      - <a href="#ssotoken-alive-usage">Usage</a>
 - <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
-   └── read_mail.py
+   ├── read_mail.py
+   └── utils.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+The [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+
+<div id="utility-functions"></div>
+
+### Utility Functions
+
+In the [utility.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some helper functions that are utilized in the module and made available for _you_ to use.
+
+<div id="generate-token"></div>
+
+#### Generate Token
+
+| Input | None |
+|---|---|
+| Output | Generates the `token.json` file from `credentials.json` file for Gmail enabled Google API |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.generate_token()` |
+
+<div id="get-import-locatioin"></div>
+
+#### Get Import Location
+
+| Input | None |
+|---|---|
+| Output | The full path to the directory where the Python file exists in which this module is imported |
+| Usage | Import: `import iitkgp_erp_login.utils as utils`, call: `utils.get_import_location()` |
+
+> This is useful when one wants to make a script that can be called from _anywhere_ in the system.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
 <div id="endpoints-about"></div>
 
 #### About
+
 - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage.
 - `SECRET_QUESTION_URL`: The URL for retrieving the secret question for authentication.
 - `OTP_URL`: The URL for requesting the OTP (One-Time Password) for authentication.
 - `LOGIN_URL`: The URL for ERP login.
 - `WELCOMEPAGE_URL`: The URL of the welcome page, which is accessible only when the user is **NOT** logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user is logged in, it returns a `404` error.
 
 <div id="endpoints-usage"></div>
 
 #### Usage
+
 ```python
 from iitkgp_erp_login.endpoints import *
 
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False, SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
+
 The function requires following _compulsory_ arguments:
+
 1. `headers`: Headers for the post requests.
-    ```python
-    headers = {
-       'timeout': '20',
-       'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
-    }
-    ``` 
-2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+   ```python
+   headers = {
+      'timeout': '20',
+      'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+   }
+   ```
+2. `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
 
-    session = requests.Session()
-    ```
+   ```python
+   import requests
+
+   session = requests.Session()
+   ```
 
 The function can also be provided with these _optional_ arguments:
 
 <div id="erpcreds"></div>
 
 1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user is prompted to enter their credentials manually |
     | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
 
     > **Note** Here, `credentials` refer to the roll number, password, and security question.
+
     <details>
       <summary><b>Prerequisites - ERP credentials file</b></summary>
       
     - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
     - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
       - You can choose any valid name for the file, adhering to Python's naming conventions.
       - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
@@ -126,75 +176,85 @@
             "Q1" : "A1",
             "Q2" : "A2",
             "Q3" : "A3",
         }
         ```
       
     </details>
-    
+
 <div id="token"></div>
     
-2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+2.  `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API continuously checks for new OTP emails.
     | Default Value | `None` |
     |---|---|
     | NOT Specified | The user will be prompted to manually enter the received OTP |
     | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
   
     <details>
       <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
 
     The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
 
     1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
        > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
 
     2. To generate the `token.json` file, follow the steps below:
-        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-        - Import the required module, `google-auth-oauthlib`
-      
+        - Import this module
+
           ```bash
-          pip install google-auth-oauthlib
+          pip install iitkgp-erp-login
           ```
-        - Execute `gentokenjson.py` with the `readonly` argument
-   
+        - Execute following command:
+
           ```bash
-          python3 gentokenjson.py readonly
+          python3 -c "from iitkgp_erp_login.utils import generate_token; generate_token()"	
           ```
         - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
         - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
            - Click on `Continue` instead of __Back To Safety__
            - Then, press `Continue` again
         - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
+
         > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
 
 3.  `LOGGING`: Toggles **comprehensive logging**.
     | Default value | `False` |
     |---|---|
     | NOT Specified | No Logging |
     | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
-    
+
+4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and `ssoToken` -  collectively referred to as "session tokens" here  - are stored for direct usage.
+    | Default value | `None` |
+    |---|---|
+    | NOT Specified | The session tokens will not be stored in a file |
+    | Specified (`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in `.session` file for later direct usage |
+
+    > **Note** The approximate expiry time for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
+
 <div id="login-output"></div>
 
 #### Output
+
 1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
 2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
+
 It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -204,61 +264,77 @@
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
 sessionToken, ssoToken = erp.login(headers, session)
-# Credentials: Manual | OTP: Manual | Logging: No
+# Credentials: Manual | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
-# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
-# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
-# Credentials: Manual | OTP: Manual | Logging: Yes
+# Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
 
 sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
-# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage: in .session file
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE='.session')
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in .session file
 ```
 
+
+> **Note** These are just examples of how to use the _login_ function.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
 <div id="session-alive"></div>
 
 ### Session status check
+
 The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
+
 The function requires following argument:
 
- -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
-    ```python
-    import requests
+- `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+  ```python
+  import requests
+
+  session = requests.Session()
+  ```
 
-    session = requests.Session()
-     ```
 <div id="session-alive-output"></div>
 
 #### Output
+
 The `session_alive(session)` function returns the status of the session as a boolean value:
 | Status | Return Value |
 | ------ | :------------: |
-| Valid (`Alive`)  | `True` |
+| Valid (`Alive`) | `True` |
 | Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
+
 It is recommended to use the `session_alive` function in the following manner:
+
 ```python
 # Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
 # Using the session_alive function inside erp.py
 print(erp.session_alive(session))
 ```
@@ -281,32 +357,117 @@
 
 session = requests.Session()
 
 print("Logging into ERP for:", creds.ROLL_NUMBER)
 
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
+> **Note** This is just a sample code demonstrating the usage of `session_alive` along with other _variables_ to get the function working.
+>> Some arguments of `login()` have their own prerequisites that must be satisfied in order to use them. See <a href="#login-input">"Input" section of login</a> for complete details.
+
+<div id="ssotoken-alive"></div>
+
+### ssoToken status check
+
+The logic for checking the validity of the ssoToken is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+
+<div id="ssotoken-alive-input"></div>
+
+#### Input
+
+The function requires following argument:
+
+- `ssoToken`: The second returned value from the `login` function.
+  ```python # Importing the erp.py file
+  import iitkgp_erp_login.erp as erp
+
+  # Using the login function inside erp.py - all others are optional arguments
+  _, ssoToken = erp.login(headers, session)
+  ```
+
+<div id="ssotoken-alive-output"></div>
+
+#### Output
+
+The `ssotoken_valid(ssoToken)` function returns the validity status of the ssotoken as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid | `True` |
+| Not Valid | `False` |
+
+<div id="ssotoken-alive-usage"></div>
+
+#### Usage
+
+It is recommended to use the `ssotoken_valid` function in the following manner:
+
+```python
+# Importing the erp.py file
+import iitkgp_erp_login.erp as erp
+
+# Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken))
+```
+
+Here's an example combining all the aspects we have discussed so far about the `login` function and `ssotoken_valid` function. <br>
+This code can be used to log in to the ERP system while storing the ssoToken. If the ssoToken remains valid, it can be used directly for subsequent logins, eliminating the need to re-authenticate each time:
+
+```python
+import webbrowser
+import requests
+import time
+
+import creds
+# Importing creds.py, which contains ERP credentials
+
+import iitkgp_erp_login.erp as erp
+
+headers = {
+    'timeout': '20',
+    'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
+}
+session = requests.Session()
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
+if os.path.exists(".session"):
+    with open(".session", "r") as file:
+        ssoToken = file.read()
+    if not erp.ssotoken_valid(ssoToken):
+        _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+        with open(".session", "w") as file:
+            file.write(ssoToken)
+else:
+    _, ssoToken = erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+    with open(".session", "w") as file:
+        file.write(ssoToken)
+
+logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
+webbrowser.open(logged_in_url)
+```
+> **Note** This is merely a Proof of Concept example; this exact functionality has been integrated into the login function itself from version **2.1.0** onwards.
+
 <div id="example"></div>
 
 ## Example
 
 Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
-   pip install iitkgp_erp_login
-   ````
+   pip install iitkgp-erp-login
+   ```
+
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
 
 3. Create a file named `open_erp.py` and include the following code:
 
    ```python
    import requests
    import webbrowser
@@ -317,16 +478,17 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=".session")
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
+
 4. Run the script.
    ```bash
    python3 open_erp.py
    ```
```

#### html2text {}

```diff
@@ -1,47 +1,68 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.0.1 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.1.0 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # ERP Login Module A python package/module to automate login process in
-ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
+LICENSE # ERP Login Module Introducing iitkgp-erp-login: Your Ultimate ERP
+Login Automation Module for IIT-KGP! Tired of the tedious ERP login process at
+IIT-Kharagpur? Wanted to automate some ERP workflow but stuck at login? Say
+goodbye to all of these problems with iitkgp-erp-login, the all-in-one Python
+package designed to streamline your ERP login experience! Key Features: -
+Seamless OTP & Credentials Handling - Effortless Session & ssoToken Management
+- Smart Token Storage for Efficiency > **Note** This package is not officially
+affiliated with IIT Kharagpur.  Table of Contents - Description - Utility
+Functions - Get_import_location - Generate_Token - Endpoints - About - Usage -
 Login - Input - Output - Usage - Session_status_check - Input - Output - Usage
-- Example
+- ssoToken_status_check - Input - Output - Usage - Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
-erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
-helper functions. These functions are not intended to be used by _you_, the
-user. The only case where OTP is required is during the login process, which is
-handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
-abstraction for general users. If you want to modify the OTP fetching process,
-feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+erp.py âââ read_mail.py âââ utils.py ``` The [read_mail.py](https:/
+/github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)`
+function, along with various helper functions. These functions are not intended
+to be used by _you_, the user. The only case where OTP is required is during
+the login process, which is handled by function in [erp.py](https://github.com/
+proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence,
+let this script serve as an abstraction for general users. If you want to
+modify the OTP fetching process, feel free to refer to the [read_mail.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/read_mail.py) script.
+### Utility Functions In the [utility.py](https://github.com/proffapt/iitkgp-
+erp-login-pypi/blob/main/src/iitkgp_erp_login/utils.py) file, you can find some
+helper functions that are utilized in the module and made available for _you_
+to use.
+#### Generate Token | Input | None | |---|---| | Output | Generates the
+`token.json` file from `credentials.json` file for Gmail enabled Google API | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.generate_token()` |
+#### Get Import Location | Input | None | |---|---| | Output | The full path to
+the directory where the Python file exists in which this module is imported | |
+Usage | Import: `import iitkgp_erp_login.utils as utils`, call:
+`utils.get_import_location()` | > This is useful when one wants to make a
+script that can be called from _anywhere_ in the system.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 #### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
 ### Login ERP login workflow is implemented in `login(headers, session,
-ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
-(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
-iitkgp_erp_login/erp.py). The input and output specifications for the function
-are mentioned below.
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False,
+SESSION_STORAGE_FILE=None)` function in [erp.py](https://github.com/proffapt/
+iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
+output specifications for the function are mentioned below.
 #### Input The function requires following _compulsory_ arguments: 1.
 `headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 ``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
 latest/_modules/requests/sessions/) object, to persist the session parameters
 throughout the workflow. ```python import requests session = requests.Session()
@@ -57,69 +78,85 @@
 - Create a `.py` file with your ERP credentials stored in it. Please follow the
 instructions below to create this file: - You can choose any valid name for the
 file, adhering to Python's naming conventions. - **Do not change the variable
 names**. Copy the format provided below & update the values inside the `double
 quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
 "**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
 "A3", } ```
-2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+2. `OTP_CHECK_INTERVAL`: The interval (in _seconds_) after which the API
 continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
 NOT Specified | The user will be prompted to manually enter the received OTP |
 | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
 checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
 The token file **MUST** be present in the same directory as the script where
 `iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
 API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
 python) guide to obtain `credentials.json` file. > **Note** The
 `credentials.json` file is permanent unless you manually delete its reference
 in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
-logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
-| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+steps below: - Import this module ```bash pip install iitkgp-erp-login ``` -
+Execute following command: ```bash python3 -c "from iitkgp_erp_login.utils
+import generate_token; generate_token()" ``` - A browser window will open,
+prompting you to select the Google account associated with receiving OTP for
+login. - Grant permission to the selected email address to utilize the newly
+enabled **Gmail API**. - Click on `Continue` instead of __Back To Safety__ -
+Then, press `Continue` again - The `token.json` file will be generated in the
+same folder as the `credentials.json` file > **Warning** The `token.json` file
+has an expiration time, so it's important to periodically check and refresh it
+in your projects to ensure uninterrupted access. 3. `LOGGING`: Toggles
+**comprehensive logging**. | Default value | `False` | |---|---| | NOT
+Specified | No Logging | | Specified (`LOGGING=True`) | Logs every step in an
+exhaustive manner | 4. `SESSION_STORAGE_FILE`: A file where `sessionToken` and
+`ssoToken` - collectively referred to as "session tokens" here - are stored for
+direct usage. | Default value | `None` | |---|---| | NOT Specified | The
+session tokens will not be stored in a file | | Specified
+(`SESSION_STORAGE_FILE=".session"`) | The session tokens will be stored in
+`.session` file for later direct usage | > **Note** The approximate expiry time
+for `ssoToken` is _~30 minutes_ and that of `session` object is _~2.5 hours_
 #### Output 1. The function returns the following, in the order of occurrence
 as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
 en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
 Single_sign-on) 2. It also modifies the `session` object, which now includes
 parameters for the logged-in session. This `session` object can be utilized for
 further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
 manner (optional arguments are _your_ choice): ```python # Importing the erp.py
 file import iitkgp_erp_login.erp as erp # Using the login function inside
 erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
-OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
-aspects we have discussed so far about the `login` function: ```python import
-requests import erpcreds import iitkgp_erp_login.erp as erp headers =
-{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
-537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
-Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
-erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
-Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
-Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
-sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
-Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
-erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
-Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
-seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
-- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
-```
+OTP_CHECK_INTERVAL=2, LOGGING=True, SESSION_STORAGE_FILE=None) ``` Here's an
+example combining all the aspects we have discussed so far about the `login`
+function: ```python import requests import erpcreds import iitkgp_erp_login.erp
+as erp headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux
+x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79
+Chrome/51.0.2704.79 Safari/537.36', } session = requests.Session()
+sessionToken, ssoToken = erp.login(headers, session) # Credentials: Manual |
+OTP: Manual | Logging: No | TokenStorage: No sessionToken, ssoToken = erp.login
+(headers, session, ERPCREDS=erpcreds) # Credentials: Automatic - from
+erpcreds.py | OTP: Manual | Logging: No | TokenStorage: No sessionToken,
+ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) # Credentials:
+Manual | OTP: Automatic - checked every 2 seconds | Logging: No | TokenStorage:
+No sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=5) # Credentials: Automatic - from erpcreds.py | OTP:
+Automatic - checked every 5 seconds | Logging: No | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic - from erpcreds.py
+| OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, SESSION_STORAGE_FILE='.session') # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: No |
+TokenStorage: in .session file sessionToken, ssoToken = erp.login(headers,
+session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE='.session') # Credentials: Automatic - from erpcreds.py |
+OTP: Automatic - checked every 2 seconds | Logging: Yes | TokenStorage: in
+.session file ``` > **Note** These are just examples of how to use the _login_
+function. >> Some arguments of `login()` have their own prerequisites that must
+be satisfied in order to use them. See "Input"_section_of_login for complete
+details.
 ### Session status check The logic for checking the status of the session is
 implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
@@ -135,22 +172,63 @@
 aspects we have discussed so far about the `login` function and `session_alive`
 function: ```python import requests import time import creds # Importing
 creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
 headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
 AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
 51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
 ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
-erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
-else: print("Session is alive.") time.sleep(2) ```
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ``` > **Note** This is just a
+sample code demonstrating the usage of `session_alive` along with other
+_variables_ to get the function working. >> Some arguments of `login()` have
+their own prerequisites that must be satisfied in order to use them. See
+"Input"_section_of_login for complete details.
+### ssoToken status check The logic for checking the validity of the ssoToken
+is implemented in the `ssotoken_valid(ssoToken)` function in [erp.py](https://
+github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
+erp.py). The input and output specifications for the function are mentioned
+below.
+#### Input The function requires following argument: - `ssoToken`: The second
+returned value from the `login` function. ```python # Importing the erp.py file
+import iitkgp_erp_login.erp as erp # Using the login function inside erp.py -
+all others are optional arguments _, ssoToken = erp.login(headers, session) ```
+#### Output The `ssotoken_valid(ssoToken)` function returns the validity status
+of the ssotoken as a boolean value: | Status | Return Value | | ------ | :-----
+-------: | | Valid | `True` | | Not Valid | `False` |
+#### Usage It is recommended to use the `ssotoken_valid` function in the
+following manner: ```python # Importing the erp.py file import
+iitkgp_erp_login.erp as erp # Using the ssotoken_valid function inside erp.py
+print(erp.ssotoken_valid(ssoToken)) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function and
+`ssotoken_valid` function.
+This code can be used to log in to the ERP system while storing the ssoToken.
+If the ssoToken remains valid, it can be used directly for subsequent logins,
+eliminating the need to re-authenticate each time: ```python import webbrowser
+import requests import time import creds # Importing creds.py, which contains
+ERP credentials import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
+'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
+Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
+session = requests.Session() print("Logging into ERP for:", creds.ROLL_NUMBER)
+if os.path.exists(".session"): with open(".session", "r") as file: ssoToken =
+file.read() if not erp.ssotoken_valid(ssoToken): _, ssoToken = erp.login
+(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True) with
+open(".session", "w") as file: file.write(ssoToken) else: _, ssoToken =
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+with open(".session", "w") as file: file.write(ssoToken) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` >
+**Note** This is merely a Proof of Concept example; this exact functionality
+has been integrated into the login function itself from version **2.1.0**
+onwards.
 ## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
-install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
+install iitkgp-erp-login ``` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
 session = requests.Session() _, ssoToken = erp.login(headers, session,
-ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
-{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
-the script. ```bash python3 open_erp.py ```
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True,
+SESSION_STORAGE_FILE=".session") logged_in_url = f"{HOMEPAGE_URL}?ssoToken=
+{ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run the script. ```bash
+python3 open_erp.py ```
```

