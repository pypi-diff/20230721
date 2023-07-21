# Comparing `tmp/robotframework-mainframe3270-3.2.tar.gz` & `tmp/robotframework-mainframe3270-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-mainframe3270-3.2.tar", last modified: Sat Apr  1 12:37:43 2023, max compression
+gzip compressed data, was "robotframework-mainframe3270-4.0.tar", last modified: Thu Jun 15 16:57:04 2023, max compression
```

## Comparing `robotframework-mainframe3270-3.2.tar` & `robotframework-mainframe3270-4.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/
--rw-rw-r--   0 robin     (1000) robin     (1000)     1065 2023-02-12 18:46:10.000000 robotframework-mainframe3270-3.2/LICENSE.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.645147 robotframework-mainframe3270-3.2/Mainframe3270/
--rw-rw-r--   0 robin     (1000) robin     (1000)     4830 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/Mainframe3270/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    15590 2023-03-17 04:57:06.000000 robotframework-mainframe3270-3.2/Mainframe3270/py3270.py
--rw-rw-r--   0 robin     (1000) robin     (1000)       16 2023-04-01 12:26:46.000000 robotframework-mainframe3270-3.2/Mainframe3270/version.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    35623 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/Mainframe3270/x3270.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7343 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     6443 2023-04-01 12:22:17.000000 robotframework-mainframe3270-3.2/README.md
--rw-rw-r--   0 robin     (1000) robin     (1000)     2063 2023-03-16 03:55:46.000000 robotframework-mainframe3270-3.2/THIRD-PARTY-NOTICES.txt
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-01 12:37:43.649147 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     7343 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      410 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       44 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       14 2023-04-01 12:37:43.000000 robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-04-01 12:37:43.653147 robotframework-mainframe3270-3.2/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)     1597 2023-03-16 03:55:46.000000 robotframework-mainframe3270-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:04.403576 robotframework-mainframe3270-4.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:04.338830 robotframework-mainframe3270-4.0/Mainframe3270/
+-rw-rw-rw-   0        0        0     9426 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:04.381261 robotframework-mainframe3270-4.0/Mainframe3270/keywords/
+-rw-rw-rw-   0        0        0      483 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/__init__.py
+-rw-rw-rw-   0        0        0    14477 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/assertions.py
+-rw-rw-rw-   0        0        0     2886 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/commands.py
+-rw-rw-rw-   0        0        0     9780 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/connection.py
+-rw-rw-rw-   0        0        0     3074 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/read_write.py
+-rw-rw-rw-   0        0        0     2338 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     3874 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/keywords/wait_and_timeout.py
+-rw-rw-rw-   0        0        0     1870 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/librarycomponent.py
+-rw-rw-rw-   0        0        0    18278 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/py3270.py
+-rw-rw-rw-   0        0        0      230 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/utils.py
+-rw-rw-rw-   0        0        0       17 2023-06-15 16:55:52.000000 robotframework-mainframe3270-4.0/Mainframe3270/version.py
+-rw-rw-rw-   0        0        0     5826 2023-06-15 16:57:04.401560 robotframework-mainframe3270-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4904 2023-06-15 16:56:11.000000 robotframework-mainframe3270-4.0/README.md
+-rw-rw-rw-   0        0        0     2100 2023-04-10 03:39:09.000000 robotframework-mainframe3270-4.0/THIRD-PARTY-NOTICES.txt
+-rw-rw-rw-   0        0        0      225 2023-06-15 16:54:52.000000 robotframework-mainframe3270-4.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:04.395440 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/
+-rw-rw-rw-   0        0        0     5826 2023-06-15 16:57:04.000000 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-06-15 16:57:04.000000 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:57:04.000000 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-15 16:57:04.000000 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 16:57:04.000000 robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:57:04.403576 robotframework-mainframe3270-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1669 2023-06-15 16:55:40.000000 robotframework-mainframe3270-4.0/setup.py
```

### Comparing `robotframework-mainframe3270-3.2/LICENSE.md` & `robotframework-mainframe3270-4.0/LICENSE.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 altranpt
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Altran Portugal
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `robotframework-mainframe3270-3.2/PKG-INFO` & `robotframework-mainframe3270-4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,157 +1,137 @@
-Metadata-Version: 2.1
-Name: robotframework-mainframe3270
-Version: 3.2
-Summary: Mainframe Test library for Robot Framework
-Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
-Author: Altran Portugal
-Author-email: samuca@gmail.com
-License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: THIRD-PARTY-NOTICES.txt
-
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
-
-1. Download the Dockerfile sources
-```sh
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
-
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
-```
-
-2. Build the image:
-```sh
-docker build -t mainframe3270 .
-```
-
-3. Run the container
-```sh
-docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
+Metadata-Version: 2.1
+Name: robotframework-mainframe3270
+Version: 4.0
+Summary: Mainframe Test library for Robot Framework
+Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
+Author: Altran Portugal
+Author-email: samuca@gmail.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: THIRD-PARTY-NOTICES.txt
+
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from [PyPI](https://pypi.org/project/robotframework-mainframe3270/).
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CONTRIBUTING.md) to help you get started.
+
+## Wiki
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Changelog
+For an overview of the (latest) changes see [CHANGELOG](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CHANGELOG.md).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## Maintainers
+   - **Robin Matz**
+
+## License
+This project is licensed under the MIT License - see [LICENSE](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.2/README.md` & `robotframework-mainframe3270-4.0/robotframework_mainframe3270.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,137 @@
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
-
-1. Download the Dockerfile sources
-```sh
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
-
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
-```
-
-2. Build the image:
-```sh
-docker build -t mainframe3270 .
-```
-
-3. Run the container
-```sh
-docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
+Metadata-Version: 2.1
+Name: robotframework-mainframe3270
+Version: 4.0
+Summary: Mainframe Test library for Robot Framework
+Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
+Author: Altran Portugal
+Author-email: samuca@gmail.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: THIRD-PARTY-NOTICES.txt
+
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from [PyPI](https://pypi.org/project/robotframework-mainframe3270/).
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CONTRIBUTING.md) to help you get started.
+
+## Wiki
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Changelog
+For an overview of the (latest) changes see [CHANGELOG](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CHANGELOG.md).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## Maintainers
+   - **Robin Matz**
+
+## License
+This project is licensed under the MIT License - see [LICENSE](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.2/THIRD-PARTY-NOTICES.txt` & `robotframework-mainframe3270-4.0/THIRD-PARTY-NOTICES.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Robot-Framework-Mainframe3270-Library uses third-party libraries or other resources that may be
-distributed under licenses different than the Robot-Framework-Mainframe3270-Library software.
-
-In the event that we accidentally failed to list a required notice, please
-bring it to our attention by posting an issue or making a pull request to our
-GitHub repository:
-
-https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/
-
-The attached notices are provided for information only.
-
-License notice for py3270
--------------------------
-Copyright (c) 2018, Randy Syring and contributors
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the name of the <organization> nor the
-      names of its contributors may be used to endorse or promote products
-      derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
-ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Robot-Framework-Mainframe3270-Library uses third-party libraries or other resources that may be
+distributed under licenses different than the Robot-Framework-Mainframe3270-Library software.
+
+In the event that we accidentally failed to list a required notice, please
+bring it to our attention by posting an issue or making a pull request to our
+GitHub repository:
+
+https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/
+
+The attached notices are provided for information only.
+
+License notice for py3270
+-------------------------
+Copyright (c) 2018, Randy Syring and contributors
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of the <organization> nor the
+      names of its contributors may be used to endorse or promote products
+      derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `robotframework-mainframe3270-3.2/robotframework_mainframe3270.egg-info/PKG-INFO` & `robotframework-mainframe3270-4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,115 @@
-Metadata-Version: 2.1
-Name: robotframework-mainframe3270
-Version: 3.2
-Summary: Mainframe Test library for Robot Framework
-Home-page: https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library
-Author: Altran Portugal
-Author-email: samuca@gmail.com
-License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: THIRD-PARTY-NOTICES.txt
-
-[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
-[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
-[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
-[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
-
-# Mainframe3270Library
-
-## Introduction
-
-Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
-
-## Compatibility
-Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
-
-## Installation
-
-In order to use this library, first install the package from PyPI.
-```commandline
-pip install robotframework-mainframe3270
-```
-
-Or you can upgrade with:
-```commandline
-pip install --upgrade robotframework-mainframe3270
-```
-
-Then, depending on your OS, proceed with the corresponding chapters in this README.
-
-### Windows
-
-You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
-
-The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
-
-### Unix
-
-You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
-```commandline
-sudo apt-get install x3270
-```
-or
-```commandline
-brew install x3270
-```
-
-More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
-
-## Example
-```RobotFramework
-*** Settings ***
-Library    Mainframe3270
-
-*** Test Cases ***
-Example
-    Open Connection    Hostname    LUname
-    Change Wait Time    0.4 seconds
-    Change Wait Time After Write    0.4 seconds
-    Set Screenshot Folder    C:\\Temp\\IMG
-    ${value}    Read    3    10    17
-    Page Should Contain String    ENTER APPLICATION
-    Wait Field Detected
-    Write Bare    applicationname
-    Send Enter
-    Take Screenshot
-    Close Connection
-```
-
-## Keyword Documentation
-
-You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
-
-## Importing
-
-Arguments:
-   - visible = True
-   - timeout = 30
-   - wait_time = 0.5
-   - wait_time_after_write = 0
-   - img_folder = .
-   - run_on_failure_keyword = Take Screenshot
-
-By default the emulator visibility is set to visible=True.
-In this case test cases are executed using wc3270 (Windows) or x3270 (Linux/MacOSX).
-You can change this by setting visible=False. Then test cases are run using ws3720 (Windows) or s3270 (Linux/MacOS).
-This is useful when test cases are run in a CI/CD-pipeline and there is no need for a graphical user interface.
-
-Timeout, waits and screenshot folder are set on library import as shown above. However, they can be changed during runtime. To modify the ``wait_time``, see [Change Wait Time](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Wait%20Time),
-to modify the ``img_folder``, see [Set Screenshot Folder](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Set%20Screenshot%20Folder),
-and to modify the ``timeout``, see the [Change Timeout](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Change%20Timeout) keyword.
-Timeouts support all available Robot Framework [time formats](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#time-format).
-
-By default, Mainframe3270 will take a screenshot on failure. You can overwrite this to run any other keyword by setting the ``run_on_failure_keyword`` option. If you pass ``None`` to this argument, no keyword will be run. To change the ``run_on_failure_keyword`` during runtime, see [Register Run On Failure Keyword](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html#Register%20Run%20On%20Failure%20Keyword).
-
-## Running with Docker
-
-The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
-
-1. Download the Dockerfile sources
-```sh
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
-
-curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
-```
-
-2. Build the image:
-```sh
-docker build -t mainframe3270 .
-```
-
-3. Run the container
-```sh
-docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
-```
-
-## Contributing to Robot-Framework-Mainframe3270-Library
-
-Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](COUNTRIBUTING.md) to help you get started.
-
-## Keyword Tests
-
-To run all the library tests, you will need to create a user on the [pub400](https://www.pub400.com/) website.
-
-## WIKI
-For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
-
-## Authors
-   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
-   - **Samuel Cabral**
-   - **Joao Gomes**
-   - **Bruno Calado**
-   - **Ricardo Morgado**
-
-## License
-This project is licensed under the MIT License - see [LICENSE.md](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
+[![PyPi downloads](https://img.shields.io/pypi/dm/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Total downloads](https://static.pepy.tech/personalized-badge/robotframework-mainframe3270?period=total&units=international_system&left_color=lightgrey&right_color=yellow&left_text=total)](https://pypi.org/project/robotframework-mainframe3270/)
+[![Latest Version](https://img.shields.io/pypi/v/robotframework-mainframe3270.svg)](https://pypi.org/project/robotframework-mainframe3270/)
+[![tests](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/actions/workflows/run-tests.yml)
+[![codecov](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/branch/master/graph/badge.svg?token=N41G62D883)](https://codecov.io/gh/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library)
+
+# Mainframe3270Library
+
+## Introduction
+
+Mainframe3270 is a library for Robot Framework based on the [py3270 project](https://pypi.org/project/py3270/), a Python interface to x3270, an IBM 3270 terminal emulator. It provides an API to a x3270 or s3270 subprocess.
+
+## Compatibility
+Mainframe3270 requires Python 3. It is tested with Python 3.7 and 3.10, but should support all versions in between these.
+
+## Installation
+
+In order to use this library, first install the package from [PyPI](https://pypi.org/project/robotframework-mainframe3270/).
+```commandline
+pip install robotframework-mainframe3270
+```
+
+Or you can upgrade with:
+```commandline
+pip install --upgrade robotframework-mainframe3270
+```
+
+Then, depending on your OS, proceed with the corresponding chapters in this README.
+
+### Windows
+
+You need to install the [x3270 project](http://x3270.bgp.nu/index.html) and put the directory on your PATH.
+
+The default folder is "C:\Program Files\wc3270". This needs to be in the `PATH` environment variable.
+
+### Unix
+
+You can install the x3270 project from [the instructions page](http://x3270.bgp.nu/Build.html#Unix). Or if it is available in your distribution through:
+```commandline
+sudo apt-get install x3270
+```
+or
+```commandline
+brew install x3270
+```
+
+More information can be found on the [Wiki page](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki/Installation) of this project.
+
+## Example
+```RobotFramework
+*** Settings ***
+Library    Mainframe3270
+
+*** Test Cases ***
+Example
+    Open Connection    Hostname    LUname
+    Change Wait Time    0.4 seconds
+    Change Wait Time After Write    0.4 seconds
+    Set Screenshot Folder    C:\\Temp\\IMG
+    ${value}    Read    3    10    17
+    Page Should Contain String    ENTER APPLICATION
+    Wait Field Detected
+    Write Bare    applicationname
+    Send Enter
+    Take Screenshot
+    Close Connection
+```
+
+## Keyword Documentation
+
+You can find the keyword documentation [here](https://raw.githack.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/doc/Mainframe3270.html).
+
+## Running with Docker
+
+The Docker image contains everything that is needed to run Mainframe tests. Currently the image is not published to Docker Hub. In order to use it, perform the following steps.
+
+1. Download the Dockerfile sources
+```sh
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/Dockerfile
+
+curl -O https://raw.githubusercontent.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/master/entrypoint.sh
+```
+
+2. Build the image:
+```sh
+docker build -t mainframe3270 .
+```
+
+3. Run the container
+```sh
+docker run --user mfuser -v /path/to/your/tests:/home/mfuser/tests mainframe3270 robot /home/mfuser/tests
+```
+
+## Contributing to Robot-Framework-Mainframe3270-Library
+
+Interested in contributing to the project? Great to hear! Whether you found a bug, or want to develop a new feature, please refer to our [Contributing Guidelines](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CONTRIBUTING.md) to help you get started.
+
+## Wiki
+For more information visit the repository [Wiki](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/wiki).
+
+## Changelog
+For an overview of the (latest) changes see [CHANGELOG](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/CHANGELOG.md).
+
+## Authors
+   - **Altran -** [Altran Web Site](https://www.altran.com/us/en/)
+   - **Samuel Cabral**
+   - **Joao Gomes**
+   - **Bruno Calado**
+   - **Ricardo Morgado**
+
+## Maintainers
+   - **Robin Matz**
+
+## License
+This project is licensed under the MIT License - see [LICENSE](https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library/blob/master/LICENSE.md) for details.
```

### Comparing `robotframework-mainframe3270-3.2/setup.py` & `robotframework-mainframe3270-4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from os.path import abspath, dirname, join
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-VERSION = None
-version_file = join(dirname(abspath(__file__)), "Mainframe3270", "version.py")
-
-with open(version_file) as file:
-    code = compile(file.read(), version_file, "exec")
-    exec(code)
-
-with open("README.md", encoding="utf-8") as file:
-    long_description = file.read()
-
-
-package_kwargs = {
-    "name": "robotframework-mainframe3270",
-    "version": VERSION,
-    "description": "Mainframe Test library for Robot Framework",
-    "long_description": long_description,
-    "long_description_content_type": "text/markdown",
-    "author": "Altran Portugal",
-    "author_email": "samuca@gmail.com",
-    "license": "MIT License",
-    "license_files": ["LICENSE.md", "THIRD-PARTY-NOTICES.txt"],
-    "url": "https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library",
-    "packages": ["Mainframe3270"],
-    "install_requires": ["robotframework", "robotframework-pythonlibcore"],
-    "classifiers": [
-        "Development Status :: 5 - Production/Stable",
-        "Framework :: Robot Framework",
-        "Framework :: Robot Framework :: Library",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Topic :: Software Development :: Testing",
-        "Topic :: Software Development :: Testing :: Acceptance",
-    ],
-}
-
-setup(**package_kwargs)
+from os.path import abspath, dirname, join
+
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+VERSION = None
+version_file = join(dirname(abspath(__file__)), "Mainframe3270", "version.py")
+
+with open(version_file) as file:
+    code = compile(file.read(), version_file, "exec")
+    exec(code)
+
+with open("README.md", encoding="utf-8") as file:
+    long_description = file.read()
+
+
+package_kwargs = {
+    "name": "robotframework-mainframe3270",
+    "version": VERSION,
+    "description": "Mainframe Test library for Robot Framework",
+    "long_description": long_description,
+    "long_description_content_type": "text/markdown",
+    "author": "Altran Portugal",
+    "author_email": "samuca@gmail.com",
+    "license": "MIT License",
+    "license_files": ["LICENSE.md", "THIRD-PARTY-NOTICES.txt"],
+    "url": "https://github.com/Altran-PT-GDC/Robot-Framework-Mainframe-3270-Library",
+    "packages": ["Mainframe3270", "Mainframe3270.keywords"],
+    "install_requires": ["robotframework", "robotframework-pythonlibcore"],
+    "classifiers": [
+        "Development Status :: 5 - Production/Stable",
+        "Framework :: Robot Framework",
+        "Framework :: Robot Framework :: Library",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Software Development :: Testing :: Acceptance",
+    ],
+}
+
+setup(**package_kwargs)
```

