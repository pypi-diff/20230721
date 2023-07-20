# Comparing `tmp/ignition-gemini-0.1.8.tar.gz` & `tmp/ignition_gemini-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignition-gemini-0.1.8.tar", last modified: Fri Aug 13 00:31:53 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ignition-gemini-0.1.8.tar` & `ignition_gemini-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.591373 ignition-gemini-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10150 2021-08-13 00:31:53.591373 ignition-gemini-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8186 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_7/Lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_7/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_7/Lib/urllib/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_7/Lib/urllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38855 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_7/Lib/urllib/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_8/Lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_8/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_8/Lib/urllib/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_8/Lib/urllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41761 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_8/Lib/urllib/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_9/Lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_9/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.587373 ignition-gemini-0.1.8/ignition/python/python3_9/Lib/urllib/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_9/Lib/urllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41776 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_9/Lib/urllib/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/python/python3_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10834 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     7344 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.591373 ignition-gemini-0.1.8/ignition/ssl/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/ssl/cert_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/ssl/cert_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/ssl/cert_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/ignition/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-13 00:31:53.591373 ignition-gemini-0.1.8/ignition_gemini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10150 2021-08-13 00:31:53.000000 ignition-gemini-0.1.8/ignition_gemini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-08-13 00:31:53.000000 ignition-gemini-0.1.8/ignition_gemini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-13 00:31:53.000000 ignition-gemini-0.1.8/ignition_gemini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-13 00:31:53.000000 ignition-gemini-0.1.8/ignition_gemini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-13 00:31:53.000000 ignition-gemini-0.1.8/ignition_gemini.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2021-08-13 00:31:53.591373 ignition-gemini-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-08-13 00:31:40.000000 ignition-gemini-0.1.8/setup.py
+-rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/__main__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/exceptions.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/globals.py
+-rw-r--r--   0        0        0    14119 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/request.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/response.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/url.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/util.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_10/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_10/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_10/Lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_10/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    42343 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_10/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_11/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_11/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_11/Lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_11/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    42612 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_11/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_7/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_7/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_7/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_7/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    38817 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_7/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_8/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_8/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_8/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_8/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    41749 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_8/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_9/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_9/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_9/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    41748 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/python/python3_9/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/ssl/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/ssl/cert_record.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/ssl/cert_store.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/ignition/ssl/cert_wrapper.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/README.md
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 ignition_gemini-0.2.0/PKG-INFO
```

### Comparing `ignition-gemini-0.1.8/LICENSE` & `ignition_gemini-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ignition-gemini-0.1.8/README.md` & `ignition_gemini-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 If you're building a Python3 application that uses Gemini, Ignition is your gateway to the stars, in very much the same way that [requests](https://requests.readthedocs.io/en/master/) is for HTTP and **gopherlib** is for Gopher.
 
 In order to provide a best-in-class interface, this library does not implement the other parts of a typical client (including user interface and/or command line interface), and instead focuses on providing a robust programmatic API interface.  This project also assumes that different user interfaces will have different requirements for their display of text/gemini files (.gmi), and/or other mime-types, and as such considers this portion of the specification beyond the scope of this project.
 
 In addition, in order to provide stability and simplicity, minimal third-party dependencies are required for Ignition.
 
 ## Project Status
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/cbrews/ignition?label=ignition)
 [![CI v2](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml/badge.svg)](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ignition-gemini)
+![PyPI - License](https://img.shields.io/pypi/l/ignition-gemini)
 
 ![The status is good to go.  This is Gemini Control.](docs/img/transcript-2.png)
 
 Ignition is currently in prerelease.  You can use Ignition today at your own risk, please monitor this repository for changes until version 1.0 is released.  Please be advised that there may be breaking changes in the API until that time.
 
 You can see ignition in action at [gemini.cbrews.xyz](https://gemini.cbrews.xyz).
 
 ## Installation
-⚠ Ignition currently supports Python versions 3.7 - 3.9.
+⚠ Ignition currently supports Python versions 3.7 - 3.11.
 
 Ignition can be installed via [PIP](https://pypi.org/project/ignition-gemini/).  You should install it in alignment with your current development process; if you do not have a build process yet, I recommend you install within a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)
 
 ```bash
 pip install ignition-gemini
 ```
 
 If you prefer to install from source, you can clone and install the repository:
 
 ```bash
 git clone https://github.com/cbrews/ignition.git
 cd ignition
-python3 setup.py install
+pip install .
 ```
 
 ## Simple Usage
 The most basic usage of Ignition allows the user to create a request and get a response back from a remote Gemini capsule:
 ```python
 import ignition
 
@@ -46,43 +49,44 @@
 
 # Get status from remote capsule
 print(response.status)
 
 # Get response information from remote capsule
 print(response.data())
 ```
-[source](examples/simple-usage.py)
+[source](examples/simple_usage.py)
 
 In **all** cases, Ignition assumes that the specified endpoint and protocol will respond over the Gemini protocol, so even if you provide a different protocol or port, it will assume that the endpoint is a Gemini capsule.
 
 ## Key Features
 
 ![This is Gemini Control.  The conversation between pilot and ground so far in this filght has largely been confined to the normal type of test pilot talk that you would expect.](docs/img/transcript-3.png)
 
 ✅ Ignition currently supports the following features:
 * Basic request/response connectivity to a Gemini-enabled server.
 * Basic URL parsing mechanics to allow for specifying protocol, host, port, path, and query params, as per [RFC-3986](https://tools.ietf.org/html/rfc3986)
 * Optional referer URL handling.  Ignition allows the user to pass a path & referer URL and can construct the new path, to simplifying the resolution of links on a Gemini capsule page.
-* Decoding of body responses on successful (20) response from Gemini servers.
-* Trust-on-first-use certificate verification handling scheme.
+* Basic decoding of body responses on successful (20) response from Gemini servers.
+* Trust-on-first-use certificate verification handling scheme using key signatures.
 * Fully-featured response objects for each response type.
-* Robust, human-readable error management and custom error handling for failure cases beyond the scope of the protocol.
+* Standardized & robust, human-readable error management.
+* Custom error handling for networking failure cases beyond the scope of the protocol.
 
 ❌ The following Gemini features will *not* be supported by Ignition:
 * Behavioral processing/handling of specific response types from Gemini capsules, including:
   * Generation of client certificates & automatic resubmission.
   * Automatic redirection following on 3x responses.
-* Body parsing & display of text/gemini mime types
-* Command line interface
-* Advanced session & history management
-* Support for other protocols
+* Advanced body response rendering and/or display of text/gemini mime types.
+* Command line or GUI interface.
+* Advanced session & history management.
+* Support for other protocols.
 
 ⚠ These features are not currently supported but may be supported in the future:
-* Alternative certificate verification schemes
-* Titan protocol
+* Non-verified certificate scheme
+* Improved TOFU scenarios
 
 ## Advanced Usage
 More advanced request usage:
 
 ```python
 import ignition
 
@@ -102,15 +106,15 @@
 import ignition
 
 response1 = ignition.request('//gemini.circumlunar.space')
 response2 = ignition.request('software', referer=response1.url)
 
 print(response2)
 ```
-[source](examples/using-referer.py)
+[source](examples/using_referer.py)
 
 More advanced response validation:
 ```python
 import ignition
 
 url = '//gemini.circumlunar.space'
 response = ignition.request(url)
@@ -133,15 +137,15 @@
 
 elif response.is_a(ignition.ClientCertRequiredResponse):
   print('Client certificate required. %s' % (response.data()))
 
 elif response.is_a(ignition.ErrorResponse):
   print('There was an error on the request: %s' % (response.data()))
 ```
-[source](examples/advanced-usage.py)
+[source](examples/advanced_usage.py)
 
 Finally, the module exposes `DEBUG` level logging via standard python capabilities.  If you are having trouble with the requests, enable debug-level logging with:
 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
@@ -156,13 +160,15 @@
 Want to help contribute to Ignition?  See the [developer documentation](./docs/developer.md) for contribution guidelines, build processes, and testing.
 
 The developer documentation is still being completed, if you have specific questions, please open tickets within this project.
 
 ## License
 Ignition is licensed under [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/).
 
+Copyright 2020-2022 by [Chris Brousseau](https://github.com/cbrews).
+
 ## Thank you
 * *solderpunk* for leading the design of the [Gemini protocol](https://gemini.circumlunar.space/docs/specification.html), without which this project would not have been possible.
 * *Sean Conman* for writing the [Gemini torture tests](gemini://gemini.conman.org/test/torture), which were instrumental in initial client testing.
 * *Michael Lazar* for his work on [Jetforce](https://github.com/michael-lazar/jetforce), which helped testing along the way.
 
 🔭 Happy exploring!
```

### Comparing `ignition-gemini-0.1.8/ignition/exceptions.py` & `ignition_gemini-0.2.0/ignition/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 
 class RemoteCertificateExpired(Exception):
-  '''
-  An exception type to handle expired certificates from the remote server.
-  This should throw if the remote certificate expiration date
-  '''
+    """
+    An exception type to handle expired certificates from the remote server.
+    This should throw if the remote certificate expiration date
+    """
 
 
 class TofuCertificateRejection(Exception):
-  '''
-  An exception type handle TOFU (trust-on-first-use rejection).
-  '''
+    """
+    An exception type handle TOFU (trust-on-first-use rejection).
+    """
 
 
 class CertRecordParseException(Exception):
-  '''
-  An exception triggered on cert record parsing.
-  '''
+    """
+    An exception triggered on cert record parsing.
+    """
 
 
 class GeminiResponseParseError(Exception):
-  '''
-  Raised when the gemini protocol data response cannot be parsed.
-  '''
+    """
+    Raised when the gemini protocol data response cannot be parsed.
+    """
```

### Comparing `ignition-gemini-0.1.8/ignition/globals.py` & `ignition_gemini-0.2.0/ignition/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 CRLF = "\r\n"
 EOL = "\n"
 
 # Gemini-Protocol Mechanical Constants
-GEMINI_SCHEME = 'gemini'
+GEMINI_SCHEME = "gemini"
 GEMINI_PORT = 1965
-GEMINI_DEFAULT_MIME_TYPE = 'text/gemini; charset=utf-8'
-GEMINI_DEFAULT_ENCODING = 'utf-8'
+GEMINI_DEFAULT_MIME_TYPE = "text/gemini; charset=utf-8"
+GEMINI_DEFAULT_ENCODING = "utf-8"
 GEMINI_RESPONSE_HEADER_SEPARATOR = "\\s+"
 GEMINI_URL_MAXLENGTH = 1024
 GEMINI_RESPONSE_HEADER_META_MAXLENGTH = 1024
 
 # One-character response codes
 RESPONSE_STATUS_ERROR = "0"
 RESPONSE_STATUS_INPUT = "1"
@@ -49,8 +49,8 @@
 RESPONSE_STATUSDETAIL_PERM_FAILURE_BAD_REQUEST = "59"
 RESPONSE_STATUSDETAIL_CLIENTCERT_REQUIRED = "60"
 RESPONSE_STATUSDETAIL_CLIENTCERT_REQUIRED_NOT_AUTHORIZED = "61"
 RESPONSE_STATUSDETAIL_CLIENTCERT_REQUIRED_NOT_VALID = "62"
 
 # ignition application defaults
 DEFAULT_REQUEST_TIMEOUT = 30
-DEFAULT_HOSTS_FILE = '.known_hosts'
+DEFAULT_HOSTS_FILE = ".known_hosts"
```

### Comparing `ignition-gemini-0.1.8/ignition/python/__init__.py` & `ignition_gemini-0.2.0/ignition/python/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
-was not distributed with this file, You can obtain one 
+was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import sys
 
 # Polyfill to include gemini in urllib parsing
+if sys.version_info > (3, 12):
+    raise Exception("Python versions > 3.11.x are not supported at this time.")
+if sys.version_info > (3, 11):
+    from .python3_10.Lib import urllib
 if sys.version_info > (3, 10):
-  raise Exception("Python versions > 3.9.x are not supported at this time.")
-
+    from .python3_10.Lib import urllib
 if sys.version_info > (3, 9):
-  from .python3_9.Lib import urllib
+    from .python3_9.Lib import urllib
 elif sys.version_info > (3, 8):
-  from .python3_8.Lib import urllib
+    from .python3_8.Lib import urllib
 elif sys.version_info > (3, 7):
-  from .python3_7.Lib import urllib
+    from .python3_7.Lib import urllib
 else:
-  raise Exception("Python versions < 3.7 are not supported at this time.")
+    raise Exception("Python versions < 3.7 are not supported at this time.")
```

### Comparing `ignition-gemini-0.1.8/ignition/python/python3_7/Lib/urllib/parse.py` & `ignition_gemini-0.2.0/ignition/python/python3_10/Lib/urllib/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,92 +23,206 @@
 urlparse module should conform with it.  The urlparse module is
 currently not entirely compliant with this RFC due to defacto
 scenarios for parsing, and for backward compatibility purposes, some
 parsing quirks from older RFCs are retained. The testcases in
 test_urlparse.py provides a good indicator of parsing behavior.
 """
 
+import collections
 import re
 import sys
-import collections
+import types
+import warnings
 
-__all__ = ["urlparse", "urlunparse", "urljoin", "urldefrag",
-           "urlsplit", "urlunsplit", "urlencode", "parse_qs",
-           "parse_qsl", "quote", "quote_plus", "quote_from_bytes",
-           "unquote", "unquote_plus", "unquote_to_bytes",
-           "DefragResult", "ParseResult", "SplitResult",
-           "DefragResultBytes", "ParseResultBytes", "SplitResultBytes"]
+__all__ = [
+    "urlparse",
+    "urlunparse",
+    "urljoin",
+    "urldefrag",
+    "urlsplit",
+    "urlunsplit",
+    "urlencode",
+    "parse_qs",
+    "parse_qsl",
+    "quote",
+    "quote_plus",
+    "quote_from_bytes",
+    "unquote",
+    "unquote_plus",
+    "unquote_to_bytes",
+    "DefragResult",
+    "ParseResult",
+    "SplitResult",
+    "DefragResultBytes",
+    "ParseResultBytes",
+    "SplitResultBytes",
+]
 
 # A classification of schemes.
 # The empty string classifies URLs with no scheme specified,
 # being the default value returned by “urlsplit” and “urlparse”.
 
-uses_relative = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'imap',  # PATCH added gemini
-                 'wais', 'file', 'https', 'shttp', 'mms',
-                 'prospero', 'rtsp', 'rtspu', 'sftp',
-                 'svn', 'svn+ssh', 'ws', 'wss']
-
-uses_netloc = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'telnet',  # PATCH added gemini
-               'imap', 'wais', 'file', 'mms', 'https', 'shttp',
-               'snews', 'prospero', 'rtsp', 'rtspu', 'rsync',
-               'svn', 'svn+ssh', 'sftp', 'nfs', 'git', 'git+ssh',
-               'ws', 'wss']
-
-uses_params = ['', 'ftp', 'gemini', 'hdl', 'prospero', 'http', 'imap',  # PATCH added gemini
-               'https', 'shttp', 'rtsp', 'rtspu', 'sip', 'sips',
-               'mms', 'sftp', 'tel']
+uses_relative = [
+    "",
+    "ftp",
+    "gemini",
+    "http",
+    "gopher",
+    "nntp",
+    "imap",  # PATCH added gemini
+    "wais",
+    "file",
+    "https",
+    "shttp",
+    "mms",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "sftp",
+    "svn",
+    "svn+ssh",
+    "ws",
+    "wss",
+]
+
+uses_netloc = [
+    "",
+    "ftp",
+    "gemini",
+    "http",
+    "gopher",
+    "nntp",
+    "telnet",  # PATCH added gemini
+    "imap",
+    "wais",
+    "file",
+    "mms",
+    "https",
+    "shttp",
+    "snews",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "rsync",
+    "svn",
+    "svn+ssh",
+    "sftp",
+    "nfs",
+    "git",
+    "git+ssh",
+    "ws",
+    "wss",
+]
+
+uses_params = [
+    "",
+    "ftp",
+    "gemini",
+    "hdl",
+    "prospero",
+    "http",
+    "imap",  # PATCH added gemini
+    "https",
+    "shttp",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+    "mms",
+    "sftp",
+    "tel",
+]
 
 # These are not actually used anymore, but should stay for backwards
 # compatibility.  (They are undocumented, but have a public-looking name.)
 
-non_hierarchical = ['gopher', 'hdl', 'mailto', 'news',
-                    'telnet', 'wais', 'imap', 'snews', 'sip', 'sips']
-
-uses_query = ['', 'http', 'wais', 'imap', 'https', 'shttp', 'mms',
-              'gopher', 'rtsp', 'rtspu', 'sip', 'sips']
-
-uses_fragment = ['', 'ftp', 'hdl', 'http', 'gopher', 'news',
-                 'nntp', 'wais', 'https', 'shttp', 'snews',
-                 'file', 'prospero']
+non_hierarchical = [
+    "gopher",
+    "hdl",
+    "mailto",
+    "news",
+    "telnet",
+    "wais",
+    "imap",
+    "snews",
+    "sip",
+    "sips",
+]
+
+uses_query = [
+    "",
+    "http",
+    "wais",
+    "imap",
+    "https",
+    "shttp",
+    "mms",
+    "gopher",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+]
+
+uses_fragment = [
+    "",
+    "ftp",
+    "hdl",
+    "http",
+    "gopher",
+    "news",
+    "nntp",
+    "wais",
+    "https",
+    "shttp",
+    "snews",
+    "file",
+    "prospero",
+]
 
 # Characters valid in scheme names
-scheme_chars = ('abcdefghijklmnopqrstuvwxyz'
-                'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                '0123456789'
-                '+-.')
+scheme_chars = (
+    "abcdefghijklmnopqrstuvwxyz" "ABCDEFGHIJKLMNOPQRSTUVWXYZ" "0123456789" "+-."
+)
+
+# Unsafe bytes to be removed per WHATWG spec
+_UNSAFE_URL_BYTES_TO_REMOVE = ["\t", "\r", "\n"]
 
 # XXX: Consider replacing with functools.lru_cache
 MAX_CACHE_SIZE = 20
 _parse_cache = {}
 
+
 def clear_cache():
     """Clear the parse cache and the quoters cache."""
     _parse_cache.clear()
     _safe_quoters.clear()
 
 
 # Helpers for bytes handling
 # For 3.2, we deliberately require applications that
 # handle improperly quoted URLs to do their own
 # decoding and encoding. If valid use cases are
 # presented, we may relax this by using latin-1
 # decoding internally for 3.3
-_implicit_encoding = 'ascii'
-_implicit_errors = 'strict'
+_implicit_encoding = "ascii"
+_implicit_errors = "strict"
+
 
 def _noop(obj):
     return obj
 
-def _encode_result(obj, encoding=_implicit_encoding,
-                        errors=_implicit_errors):
+
+def _encode_result(obj, encoding=_implicit_encoding, errors=_implicit_errors):
     return obj.encode(encoding, errors)
 
-def _decode_args(args, encoding=_implicit_encoding,
-                       errors=_implicit_errors):
-    return tuple(x.decode(encoding, errors) if x else '' for x in args)
+
+def _decode_args(args, encoding=_implicit_encoding, errors=_implicit_errors):
+    return tuple(x.decode(encoding, errors) if x else "" for x in args)
+
 
 def _coerce_args(*args):
     # Invokes decode if necessary to create str args
     # and returns the coerced inputs along with
     # an appropriate result coercion function
     #   - noop for str inputs
     #   - encoding function otherwise
@@ -118,33 +232,37 @@
         # "scheme=''" default argument to some functions
         if arg and isinstance(arg, str) != str_input:
             raise TypeError("Cannot mix str and non-str arguments")
     if str_input:
         return args + (_noop,)
     return _decode_args(args) + (_encode_result,)
 
+
 # Result objects are more helpful than simple tuples
 class _ResultMixinStr(object):
     """Standard approach to encoding parsed results from str to bytes"""
+
     __slots__ = ()
 
-    def encode(self, encoding='ascii', errors='strict'):
+    def encode(self, encoding="ascii", errors="strict"):
         return self._encoded_counterpart(*(x.encode(encoding, errors) for x in self))
 
 
 class _ResultMixinBytes(object):
     """Standard approach to decoding parsed results from bytes to str"""
+
     __slots__ = ()
 
-    def decode(self, encoding='ascii', errors='strict'):
+    def decode(self, encoding="ascii", errors="strict"):
         return self._decoded_counterpart(*(x.decode(encoding, errors) for x in self))
 
 
 class _NetlocResultMixinBase(object):
     """Shared methods for the parsed result objects containing a netloc element"""
+
     __slots__ = ()
 
     @property
     def username(self):
         return self._userinfo[0]
 
     @property
@@ -154,95 +272,99 @@
     @property
     def hostname(self):
         hostname = self._hostinfo[0]
         if not hostname:
             return None
         # Scoped IPv6 address may have zone info, which must not be lowercased
         # like http://[fe80::822a:a8ff:fe49:470c%tESt]:1234/keys
-        separator = '%' if isinstance(hostname, str) else b'%'
+        separator = "%" if isinstance(hostname, str) else b"%"
         hostname, percent, zone = hostname.partition(separator)
         return hostname.lower() + percent + zone
 
     @property
     def port(self):
         port = self._hostinfo[1]
         if port is not None:
-            port = int(port, 10)
-            if not ( 0 <= port <= 65535):
+            try:
+                port = int(port, 10)
+            except ValueError:
+                message = f"Port could not be cast to integer value as {port!r}"
+                raise ValueError(message) from None
+            if not (0 <= port <= 65535):
                 raise ValueError("Port out of range 0-65535")
         return port
 
+    __class_getitem__ = classmethod(types.GenericAlias)
+
 
 class _NetlocResultMixinStr(_NetlocResultMixinBase, _ResultMixinStr):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition('@')
+        userinfo, have_info, hostinfo = netloc.rpartition("@")
         if have_info:
-            username, have_password, password = userinfo.partition(':')
+            username, have_password, password = userinfo.partition(":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition('@')
-        _, have_open_br, bracketed = hostinfo.partition('[')
+        _, _, hostinfo = netloc.rpartition("@")
+        _, have_open_br, bracketed = hostinfo.partition("[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(']')
-            _, _, port = port.partition(':')
+            hostname, _, port = bracketed.partition("]")
+            _, _, port = port.partition(":")
         else:
-            hostname, _, port = hostinfo.partition(':')
+            hostname, _, port = hostinfo.partition(":")
         if not port:
             port = None
         return hostname, port
 
 
 class _NetlocResultMixinBytes(_NetlocResultMixinBase, _ResultMixinBytes):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition(b'@')
+        userinfo, have_info, hostinfo = netloc.rpartition(b"@")
         if have_info:
-            username, have_password, password = userinfo.partition(b':')
+            username, have_password, password = userinfo.partition(b":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition(b'@')
-        _, have_open_br, bracketed = hostinfo.partition(b'[')
+        _, _, hostinfo = netloc.rpartition(b"@")
+        _, have_open_br, bracketed = hostinfo.partition(b"[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(b']')
-            _, _, port = port.partition(b':')
+            hostname, _, port = bracketed.partition(b"]")
+            _, _, port = port.partition(b":")
         else:
-            hostname, _, port = hostinfo.partition(b':')
+            hostname, _, port = hostinfo.partition(b":")
         if not port:
             port = None
         return hostname, port
 
 
 from collections import namedtuple
 
-_DefragResultBase = namedtuple('DefragResult', 'url fragment')
-_SplitResultBase = namedtuple(
-    'SplitResult', 'scheme netloc path query fragment')
-_ParseResultBase = namedtuple(
-    'ParseResult', 'scheme netloc path params query fragment')
+_DefragResultBase = namedtuple("DefragResult", "url fragment")
+_SplitResultBase = namedtuple("SplitResult", "scheme netloc path query fragment")
+_ParseResultBase = namedtuple("ParseResult", "scheme netloc path params query fragment")
 
 _DefragResultBase.__doc__ = """
 DefragResult(url, fragment)
 
 A 2-tuple that contains the url without fragment identifier and the fragment
 identifier as a separate argument.
 """
@@ -280,15 +402,15 @@
 
 _SplitResultBase.fragment.__doc__ = """
 Fragment identifier, that allows indirect identification of a secondary resource
 by reference to a primary resource and additional identifying information.
 """
 
 _ParseResultBase.__doc__ = """
-ParseResult(scheme, netloc, path, params,  query, fragment)
+ParseResult(scheme, netloc, path, params, query, fragment)
 
 A 6-tuple that contains components of a parsed URL.
 """
 
 _ParseResultBase.scheme.__doc__ = _SplitResultBase.scheme.__doc__
 _ParseResultBase.netloc.__doc__ = _SplitResultBase.netloc.__doc__
 _ParseResultBase.path.__doc__ = _SplitResultBase.path.__doc__
@@ -305,485 +427,574 @@
 # ResultBase is no longer part of the documented API, but it is
 # retained since deprecating it isn't worth the hassle
 ResultBase = _NetlocResultMixinStr
 
 # Structured result objects for string data
 class DefragResult(_DefragResultBase, _ResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + '#' + self.fragment
+            return self.url + "#" + self.fragment
         else:
             return self.url
 
+
 class SplitResult(_SplitResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResult(_ParseResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Structured result objects for bytes data
 class DefragResultBytes(_DefragResultBase, _ResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + b'#' + self.fragment
+            return self.url + b"#" + self.fragment
         else:
             return self.url
 
+
 class SplitResultBytes(_SplitResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResultBytes(_ParseResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Set up the encode/decode result pairs
 def _fix_result_transcoding():
     _result_pairs = (
         (DefragResult, DefragResultBytes),
         (SplitResult, SplitResultBytes),
         (ParseResult, ParseResultBytes),
     )
     for _decoded, _encoded in _result_pairs:
         _decoded._encoded_counterpart = _encoded
         _encoded._decoded_counterpart = _decoded
 
+
 _fix_result_transcoding()
 del _fix_result_transcoding
 
-def urlparse(url, scheme='', allow_fragments=True):
+
+def urlparse(url, scheme="", allow_fragments=True):
     """Parse a URL into 6 components:
     <scheme>://<netloc>/<path>;<params>?<query>#<fragment>
-    Return a 6-tuple: (scheme, netloc, path, params, query, fragment).
-    Note that we don't break the components up in smaller bits
-    (e.g. netloc is a single string) and we don't expand % escapes."""
+
+    The result is a named 6-tuple with fields corresponding to the
+    above. It is either a ParseResult or ParseResultBytes object,
+    depending on the type of the url parameter.
+
+    The username, password, hostname, and port sub-components of netloc
+    can also be accessed as attributes of the returned object.
+
+    The scheme argument provides the default value of the scheme
+    component when no scheme is found in url.
+
+    If allow_fragments is False, no attempt is made to separate the
+    fragment component from the previous component, which can be either
+    path or query.
+
+    Note that % escapes are not expanded.
+    """
     url, scheme, _coerce_result = _coerce_args(url, scheme)
     splitresult = urlsplit(url, scheme, allow_fragments)
     scheme, netloc, url, query, fragment = splitresult
-    if scheme in uses_params and ';' in url:
+    if scheme in uses_params and ";" in url:
         url, params = _splitparams(url)
     else:
-        params = ''
+        params = ""
     result = ParseResult(scheme, netloc, url, params, query, fragment)
     return _coerce_result(result)
 
+
 def _splitparams(url):
-    if '/'  in url:
-        i = url.find(';', url.rfind('/'))
+    if "/" in url:
+        i = url.find(";", url.rfind("/"))
         if i < 0:
-            return url, ''
+            return url, ""
     else:
-        i = url.find(';')
-    return url[:i], url[i+1:]
+        i = url.find(";")
+    return url[:i], url[i + 1 :]
+
 
 def _splitnetloc(url, start=0):
-    delim = len(url)   # position of end of domain part of url, default is end
-    for c in '/?#':    # look for delimiters; the order is NOT important
-        wdelim = url.find(c, start)        # find first of this delim
-        if wdelim >= 0:                    # if found
-            delim = min(delim, wdelim)     # use earliest delim position
-    return url[start:delim], url[delim:]   # return (domain, rest)
+    delim = len(url)  # position of end of domain part of url, default is end
+    for c in "/?#":  # look for delimiters; the order is NOT important
+        wdelim = url.find(c, start)  # find first of this delim
+        if wdelim >= 0:  # if found
+            delim = min(delim, wdelim)  # use earliest delim position
+    return url[start:delim], url[delim:]  # return (domain, rest)
+
 
 def _checknetloc(netloc):
     if not netloc or netloc.isascii():
         return
     # looking for characters like \u2100 that expand to 'a/c'
     # IDNA uses NFKC equivalence, so normalize for this check
     import unicodedata
-    n = netloc.replace('@', '')   # ignore characters already included
-    n = n.replace(':', '')        # but not the surrounding text
-    n = n.replace('#', '')
-    n = n.replace('?', '')
-    netloc2 = unicodedata.normalize('NFKC', n)
+
+    n = netloc.replace("@", "")  # ignore characters already included
+    n = n.replace(":", "")  # but not the surrounding text
+    n = n.replace("#", "")
+    n = n.replace("?", "")
+    netloc2 = unicodedata.normalize("NFKC", n)
     if n == netloc2:
         return
-    for c in '/?#@:':
+    for c in "/?#@:":
         if c in netloc2:
-            raise ValueError("netloc '" + netloc + "' contains invalid " +
-                             "characters under NFKC normalization")
+            raise ValueError(
+                "netloc '"
+                + netloc
+                + "' contains invalid "
+                + "characters under NFKC normalization"
+            )
 
-def urlsplit(url, scheme='', allow_fragments=True):
+
+def urlsplit(url, scheme="", allow_fragments=True):
     """Parse a URL into 5 components:
     <scheme>://<netloc>/<path>?<query>#<fragment>
-    Return a 5-tuple: (scheme, netloc, path, query, fragment).
-    Note that we don't break the components up in smaller bits
-    (e.g. netloc is a single string) and we don't expand % escapes."""
+
+    The result is a named 5-tuple with fields corresponding to the
+    above. It is either a SplitResult or SplitResultBytes object,
+    depending on the type of the url parameter.
+
+    The username, password, hostname, and port sub-components of netloc
+    can also be accessed as attributes of the returned object.
+
+    The scheme argument provides the default value of the scheme
+    component when no scheme is found in url.
+
+    If allow_fragments is False, no attempt is made to separate the
+    fragment component from the previous component, which can be either
+    path or query.
+
+    Note that % escapes are not expanded.
+    """
+
     url, scheme, _coerce_result = _coerce_args(url, scheme)
+
+    for b in _UNSAFE_URL_BYTES_TO_REMOVE:
+        url = url.replace(b, "")
+        scheme = scheme.replace(b, "")
+
     allow_fragments = bool(allow_fragments)
     key = url, scheme, allow_fragments, type(url), type(scheme)
     cached = _parse_cache.get(key, None)
     if cached:
         return _coerce_result(cached)
-    if len(_parse_cache) >= MAX_CACHE_SIZE: # avoid runaway growth
+    if len(_parse_cache) >= MAX_CACHE_SIZE:  # avoid runaway growth
         clear_cache()
-    netloc = query = fragment = ''
-    i = url.find(':')
+    netloc = query = fragment = ""
+    i = url.find(":")
     if i > 0:
-        if url[:i] == 'http': # optimize the common case
-            url = url[i+1:]
-            if url[:2] == '//':
-                netloc, url = _splitnetloc(url, 2)
-                if (('[' in netloc and ']' not in netloc) or
-                        (']' in netloc and '[' not in netloc)):
-                    raise ValueError("Invalid IPv6 URL")
-            if allow_fragments and '#' in url:
-                url, fragment = url.split('#', 1)
-            if '?' in url:
-                url, query = url.split('?', 1)
-            _checknetloc(netloc)
-            v = SplitResult('http', netloc, url, query, fragment)
-            _parse_cache[key] = v
-            return _coerce_result(v)
         for c in url[:i]:
             if c not in scheme_chars:
                 break
         else:
-            # make sure "url" is not actually a port number (in which case
-            # "scheme" is really part of the path)
-            rest = url[i+1:]
-            if not rest or any(c not in '0123456789' for c in rest):
-                # not a port number
-                scheme, url = url[:i].lower(), rest
+            scheme, url = url[:i].lower(), url[i + 1 :]
 
-    if url[:2] == '//':
+    if url[:2] == "//":
         netloc, url = _splitnetloc(url, 2)
-        if (('[' in netloc and ']' not in netloc) or
-                (']' in netloc and '[' not in netloc)):
+        if ("[" in netloc and "]" not in netloc) or (
+            "]" in netloc and "[" not in netloc
+        ):
             raise ValueError("Invalid IPv6 URL")
-    if allow_fragments and '#' in url:
-        url, fragment = url.split('#', 1)
-    if '?' in url:
-        url, query = url.split('?', 1)
+    if allow_fragments and "#" in url:
+        url, fragment = url.split("#", 1)
+    if "?" in url:
+        url, query = url.split("?", 1)
     _checknetloc(netloc)
     v = SplitResult(scheme, netloc, url, query, fragment)
     _parse_cache[key] = v
     return _coerce_result(v)
 
+
 def urlunparse(components):
     """Put a parsed URL back together again.  This may result in a
     slightly different, but equivalent URL, if the URL that was parsed
     originally had redundant delimiters, e.g. a ? with an empty query
     (the draft states that these are equivalent)."""
-    scheme, netloc, url, params, query, fragment, _coerce_result = (
-                                                  _coerce_args(*components))
+    scheme, netloc, url, params, query, fragment, _coerce_result = _coerce_args(
+        *components
+    )
     if params:
         url = "%s;%s" % (url, params)
     return _coerce_result(urlunsplit((scheme, netloc, url, query, fragment)))
 
+
 def urlunsplit(components):
     """Combine the elements of a tuple as returned by urlsplit() into a
     complete URL as a string. The data argument can be any five-item iterable.
     This may result in a slightly different, but equivalent URL, if the URL that
     was parsed originally had unnecessary delimiters (for example, a ? with an
     empty query; the RFC states that these are equivalent)."""
-    scheme, netloc, url, query, fragment, _coerce_result = (
-                                          _coerce_args(*components))
-    if netloc or (scheme and scheme in uses_netloc and url[:2] != '//'):
-        if url and url[:1] != '/': url = '/' + url
-        url = '//' + (netloc or '') + url
+    scheme, netloc, url, query, fragment, _coerce_result = _coerce_args(*components)
+    if netloc or (scheme and scheme in uses_netloc and url[:2] != "//"):
+        if url and url[:1] != "/":
+            url = "/" + url
+        url = "//" + (netloc or "") + url
     if scheme:
-        url = scheme + ':' + url
+        url = scheme + ":" + url
     if query:
-        url = url + '?' + query
+        url = url + "?" + query
     if fragment:
-        url = url + '#' + fragment
+        url = url + "#" + fragment
     return _coerce_result(url)
 
+
 def urljoin(base, url, allow_fragments=True):
     """Join a base URL and a possibly relative URL to form an absolute
     interpretation of the latter."""
     if not base:
         return url
     if not url:
         return base
 
     base, url, _coerce_result = _coerce_args(base, url)
-    bscheme, bnetloc, bpath, bparams, bquery, bfragment = \
-            urlparse(base, '', allow_fragments)
-    scheme, netloc, path, params, query, fragment = \
-            urlparse(url, bscheme, allow_fragments)
+    bscheme, bnetloc, bpath, bparams, bquery, bfragment = urlparse(
+        base, "", allow_fragments
+    )
+    scheme, netloc, path, params, query, fragment = urlparse(
+        url, bscheme, allow_fragments
+    )
 
     if scheme != bscheme or scheme not in uses_relative:
         return _coerce_result(url)
     if scheme in uses_netloc:
         if netloc:
-            return _coerce_result(urlunparse((scheme, netloc, path,
-                                              params, query, fragment)))
+            return _coerce_result(
+                urlunparse((scheme, netloc, path, params, query, fragment))
+            )
         netloc = bnetloc
 
     if not path and not params:
         path = bpath
         params = bparams
         if not query:
             query = bquery
-        return _coerce_result(urlunparse((scheme, netloc, path,
-                                          params, query, fragment)))
+        return _coerce_result(
+            urlunparse((scheme, netloc, path, params, query, fragment))
+        )
 
-    base_parts = bpath.split('/')
-    if base_parts[-1] != '':
+    base_parts = bpath.split("/")
+    if base_parts[-1] != "":
         # the last item is not a directory, so will not be taken into account
         # in resolving the relative path
         del base_parts[-1]
 
     # for rfc3986, ignore all base path should the first character be root.
-    if path[:1] == '/':
-        segments = path.split('/')
+    if path[:1] == "/":
+        segments = path.split("/")
     else:
-        segments = base_parts + path.split('/')
+        segments = base_parts + path.split("/")
         # filter out elements that would cause redundant slashes on re-joining
         # the resolved_path
         segments[1:-1] = filter(None, segments[1:-1])
 
     resolved_path = []
 
     for seg in segments:
-        if seg == '..':
+        if seg == "..":
             try:
                 resolved_path.pop()
             except IndexError:
                 # ignore any .. segments that would otherwise cause an IndexError
                 # when popped from resolved_path if resolving for rfc3986
                 pass
-        elif seg == '.':
+        elif seg == ".":
             continue
         else:
             resolved_path.append(seg)
 
-    if segments[-1] in ('.', '..'):
+    if segments[-1] in (".", ".."):
         # do some post-processing here. if the last segment was a relative dir,
         # then we need to append the trailing '/'
-        resolved_path.append('')
+        resolved_path.append("")
 
-    return _coerce_result(urlunparse((scheme, netloc, '/'.join(
-        resolved_path) or '/', params, query, fragment)))
+    return _coerce_result(
+        urlunparse(
+            (scheme, netloc, "/".join(resolved_path) or "/", params, query, fragment)
+        )
+    )
 
 
 def urldefrag(url):
     """Removes any existing fragment from URL.
 
     Returns a tuple of the defragmented URL and the fragment.  If
     the URL contained no fragments, the second element is the
     empty string.
     """
     url, _coerce_result = _coerce_args(url)
-    if '#' in url:
+    if "#" in url:
         s, n, p, a, q, frag = urlparse(url)
-        defrag = urlunparse((s, n, p, a, q, ''))
+        defrag = urlunparse((s, n, p, a, q, ""))
     else:
-        frag = ''
+        frag = ""
         defrag = url
     return _coerce_result(DefragResult(defrag, frag))
 
-_hexdig = '0123456789ABCDEFabcdef'
+
+_hexdig = "0123456789ABCDEFabcdef"
 _hextobyte = None
 
+
 def unquote_to_bytes(string):
     """unquote_to_bytes('abc%20def') -> b'abc def'."""
     # Note: strings are encoded as UTF-8. This is only an issue if it contains
     # unescaped non-ASCII characters, which URIs should not.
     if not string:
         # Is it a string-like object?
         string.split
-        return b''
+        return b""
     if isinstance(string, str):
-        string = string.encode('utf-8')
-    bits = string.split(b'%')
+        string = string.encode("utf-8")
+    bits = string.split(b"%")
     if len(bits) == 1:
         return string
     res = [bits[0]]
     append = res.append
     # Delay the initialization of the table to not waste memory
     # if the function is never called
     global _hextobyte
     if _hextobyte is None:
-        _hextobyte = {(a + b).encode(): bytes.fromhex(a + b)
-                      for a in _hexdig for b in _hexdig}
+        _hextobyte = {
+            (a + b).encode(): bytes.fromhex(a + b) for a in _hexdig for b in _hexdig
+        }
     for item in bits[1:]:
         try:
             append(_hextobyte[item[:2]])
             append(item[2:])
         except KeyError:
-            append(b'%')
+            append(b"%")
             append(item)
-    return b''.join(res)
+    return b"".join(res)
+
 
-_asciire = re.compile('([\x00-\x7f]+)')
+_asciire = re.compile("([\x00-\x7f]+)")
 
-def unquote(string, encoding='utf-8', errors='replace'):
+
+def unquote(string, encoding="utf-8", errors="replace"):
     """Replace %xx escapes by their single-character equivalent. The optional
     encoding and errors parameters specify how to decode percent-encoded
     sequences into Unicode characters, as accepted by the bytes.decode()
     method.
     By default, percent-encoded sequences are decoded with UTF-8, and invalid
     sequences are replaced by a placeholder character.
 
     unquote('abc%20def') -> 'abc def'.
     """
-    if '%' not in string:
+    if isinstance(string, bytes):
+        return unquote_to_bytes(string).decode(encoding, errors)
+    if "%" not in string:
         string.split
         return string
     if encoding is None:
-        encoding = 'utf-8'
+        encoding = "utf-8"
     if errors is None:
-        errors = 'replace'
+        errors = "replace"
     bits = _asciire.split(string)
     res = [bits[0]]
     append = res.append
     for i in range(1, len(bits), 2):
         append(unquote_to_bytes(bits[i]).decode(encoding, errors))
         append(bits[i + 1])
-    return ''.join(res)
+    return "".join(res)
 
 
-def parse_qs(qs, keep_blank_values=False, strict_parsing=False,
-             encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qs(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+    separator="&",
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
+
+    qs: percent-encoded query string to be parsed
 
-        qs: percent-encoded query string to be parsed
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as
+        blank strings.  The default false value indicates that
+        blank values are to be ignored and treated as if they were
+        not included.
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as
-            blank strings.  The default false value indicates that
-            blank values are to be ignored and treated as if they were
-            not included.
+    strict_parsing: flag indicating what to do with parsing errors.
+        If false (the default), errors are silently ignored.
+        If true, errors raise a ValueError exception.
 
-        strict_parsing: flag indicating what to do with parsing errors.
-            If false (the default), errors are silently ignored.
-            If true, errors raise a ValueError exception.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    max_num_fields: int. If set, then throws a ValueError if there
+        are more than n fields read by parse_qsl().
 
-        max_num_fields: int. If set, then throws a ValueError if there
-            are more than n fields read by parse_qsl().
+    separator: str. The symbol to use for separating the query arguments.
+        Defaults to &.
 
-        Returns a dictionary.
+    Returns a dictionary.
     """
     parsed_result = {}
-    pairs = parse_qsl(qs, keep_blank_values, strict_parsing,
-                      encoding=encoding, errors=errors,
-                      max_num_fields=max_num_fields)
+    pairs = parse_qsl(
+        qs,
+        keep_blank_values,
+        strict_parsing,
+        encoding=encoding,
+        errors=errors,
+        max_num_fields=max_num_fields,
+        separator=separator,
+    )
     for name, value in pairs:
         if name in parsed_result:
             parsed_result[name].append(value)
         else:
             parsed_result[name] = [value]
     return parsed_result
 
 
-def parse_qsl(qs, keep_blank_values=False, strict_parsing=False,
-              encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qsl(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+    separator="&",
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
+
+    qs: percent-encoded query string to be parsed
 
-        qs: percent-encoded query string to be parsed
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as blank
+        strings.  The default false value indicates that blank values
+        are to be ignored and treated as if they were  not included.
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as blank
-            strings.  The default false value indicates that blank values
-            are to be ignored and treated as if they were  not included.
+    strict_parsing: flag indicating what to do with parsing errors. If
+        false (the default), errors are silently ignored. If true,
+        errors raise a ValueError exception.
 
-        strict_parsing: flag indicating what to do with parsing errors. If
-            false (the default), errors are silently ignored. If true,
-            errors raise a ValueError exception.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    max_num_fields: int. If set, then throws a ValueError
+        if there are more than n fields read by parse_qsl().
 
-        max_num_fields: int. If set, then throws a ValueError
-            if there are more than n fields read by parse_qsl().
+    separator: str. The symbol to use for separating the query arguments.
+        Defaults to &.
 
-        Returns a list, as G-d intended.
+    Returns a list, as G-d intended.
     """
     qs, _coerce_result = _coerce_args(qs)
+    separator, _ = _coerce_args(separator)
+
+    if not separator or (not isinstance(separator, (str, bytes))):
+        raise ValueError("Separator must be of type string or bytes.")
 
     # If max_num_fields is defined then check that the number of fields
     # is less than max_num_fields. This prevents a memory exhaustion DOS
     # attack via post bodies with many fields.
     if max_num_fields is not None:
-        num_fields = 1 + qs.count('&') + qs.count(';')
+        num_fields = 1 + qs.count(separator)
         if max_num_fields < num_fields:
-            raise ValueError('Max number of fields exceeded')
+            raise ValueError("Max number of fields exceeded")
 
-    pairs = [s2 for s1 in qs.split('&') for s2 in s1.split(';')]
     r = []
-    for name_value in pairs:
+    for name_value in qs.split(separator):
         if not name_value and not strict_parsing:
             continue
-        nv = name_value.split('=', 1)
+        nv = name_value.split("=", 1)
         if len(nv) != 2:
             if strict_parsing:
                 raise ValueError("bad query field: %r" % (name_value,))
             # Handle case of a control-name with no equal sign
             if keep_blank_values:
-                nv.append('')
+                nv.append("")
             else:
                 continue
         if len(nv[1]) or keep_blank_values:
-            name = nv[0].replace('+', ' ')
+            name = nv[0].replace("+", " ")
             name = unquote(name, encoding=encoding, errors=errors)
             name = _coerce_result(name)
-            value = nv[1].replace('+', ' ')
+            value = nv[1].replace("+", " ")
             value = unquote(value, encoding=encoding, errors=errors)
             value = _coerce_result(value)
             r.append((name, value))
     return r
 
-def unquote_plus(string, encoding='utf-8', errors='replace'):
+
+def unquote_plus(string, encoding="utf-8", errors="replace"):
     """Like unquote(), but also replace plus signs by spaces, as required for
     unquoting HTML form values.
 
     unquote_plus('%7e/abc+def') -> '~/abc def'
     """
-    string = string.replace('+', ' ')
+    string = string.replace("+", " ")
     return unquote(string, encoding, errors)
 
-_ALWAYS_SAFE = frozenset(b'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                         b'abcdefghijklmnopqrstuvwxyz'
-                         b'0123456789'
-                         b'_.-~')
+
+_ALWAYS_SAFE = frozenset(
+    b"ABCDEFGHIJKLMNOPQRSTUVWXYZ" b"abcdefghijklmnopqrstuvwxyz" b"0123456789" b"_.-~"
+)
 _ALWAYS_SAFE_BYTES = bytes(_ALWAYS_SAFE)
 _safe_quoters = {}
 
+
 class Quoter(collections.defaultdict):
     """A mapping from bytes (in range(0,256)) to strings.
 
     String values are percent-encoded byte values, unless the key < 128, and
     in the "safe" set (either the specified safe set, or default set).
     """
+
     # Keeps a cache internally, using defaultdict, for efficiency (lookups
     # of cached keys don't call Python code at all).
     def __init__(self, safe):
         """safe: bytes object."""
         self.safe = _ALWAYS_SAFE.union(safe)
 
     def __repr__(self):
         # Without this, will just display as a defaultdict
         return "<%s %r>" % (self.__class__.__name__, dict(self))
 
     def __missing__(self, b):
         # Handle a cache miss. Store quoted string in cache and return.
-        res = chr(b) if b in self.safe else '%{:02X}'.format(b)
+        res = chr(b) if b in self.safe else "%{:02X}".format(b)
         self[b] = res
         return res
 
-def quote(string, safe='/', encoding=None, errors=None):
+
+def quote(string, safe="/", encoding=None, errors=None):
     """quote('abc def') -> 'abc%20def'
 
     Each part of a URL, e.g. the path info, the query, etc., has a
     different set of reserved characters that must be quoted. The
     quote function offers a cautious (not minimal) way to quote a
     string for most of these parts.
 
@@ -818,66 +1029,71 @@
     By default, encoding='utf-8' (characters are encoded with UTF-8), and
     errors='strict' (unsupported characters raise a UnicodeEncodeError).
     """
     if isinstance(string, str):
         if not string:
             return string
         if encoding is None:
-            encoding = 'utf-8'
+            encoding = "utf-8"
         if errors is None:
-            errors = 'strict'
+            errors = "strict"
         string = string.encode(encoding, errors)
     else:
         if encoding is not None:
             raise TypeError("quote() doesn't support 'encoding' for bytes")
         if errors is not None:
             raise TypeError("quote() doesn't support 'errors' for bytes")
     return quote_from_bytes(string, safe)
 
-def quote_plus(string, safe='', encoding=None, errors=None):
+
+def quote_plus(string, safe="", encoding=None, errors=None):
     """Like quote(), but also replace ' ' with '+', as required for quoting
     HTML form values. Plus signs in the original string are escaped unless
     they are included in safe. It also does not have safe default to '/'.
     """
     # Check if ' ' in string, where string may either be a str or bytes.  If
     # there are no spaces, the regular quote will produce the right answer.
-    if ((isinstance(string, str) and ' ' not in string) or
-        (isinstance(string, bytes) and b' ' not in string)):
+    if (isinstance(string, str) and " " not in string) or (
+        isinstance(string, bytes) and b" " not in string
+    ):
         return quote(string, safe, encoding, errors)
     if isinstance(safe, str):
-        space = ' '
+        space = " "
     else:
-        space = b' '
+        space = b" "
     string = quote(string, safe + space, encoding, errors)
-    return string.replace(' ', '+')
+    return string.replace(" ", "+")
 
-def quote_from_bytes(bs, safe='/'):
+
+def quote_from_bytes(bs, safe="/"):
     """Like quote(), but accepts a bytes object rather than a str, and does
     not perform string-to-bytes encoding.  It always returns an ASCII string.
     quote_from_bytes(b'abc def\x3f') -> 'abc%20def%3f'
     """
     if not isinstance(bs, (bytes, bytearray)):
         raise TypeError("quote_from_bytes() expected bytes")
     if not bs:
-        return ''
+        return ""
     if isinstance(safe, str):
         # Normalize 'safe' by converting to bytes and removing non-ASCII chars
-        safe = safe.encode('ascii', 'ignore')
+        safe = safe.encode("ascii", "ignore")
     else:
         safe = bytes([c for c in safe if c < 128])
     if not bs.rstrip(_ALWAYS_SAFE_BYTES + safe):
         return bs.decode()
     try:
         quoter = _safe_quoters[safe]
     except KeyError:
         _safe_quoters[safe] = quoter = Quoter(safe).__getitem__
-    return ''.join([quoter(char) for char in bs])
+    return "".join([quoter(char) for char in bs])
+
 
-def urlencode(query, doseq=False, safe='', encoding=None, errors=None,
-              quote_via=quote_plus):
+def urlencode(
+    query, doseq=False, safe="", encoding=None, errors=None, quote_via=quote_plus
+):
     """Encode a dict or sequence of two-element tuples into a URL query string.
 
     If any values in the query arg are sequences and doseq is true, each
     sequence element is converted to a separate parameter.
 
     If the query arg is a sequence of two-element tuples, the order of the
     parameters in the output will match the order of parameters in the
@@ -901,168 +1117,299 @@
                 raise TypeError
             # Zero-length sequences of all types will get here and succeed,
             # but that's a minor nit.  Since the original implementation
             # allowed empty dicts that type of behavior probably should be
             # preserved for consistency
         except TypeError:
             ty, va, tb = sys.exc_info()
-            raise TypeError("not a valid non-string sequence "
-                            "or mapping object").with_traceback(tb)
+            raise TypeError(
+                "not a valid non-string sequence " "or mapping object"
+            ).with_traceback(tb)
 
     l = []
     if not doseq:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
             else:
                 v = quote_via(str(v), safe, encoding, errors)
-            l.append(k + '=' + v)
+            l.append(k + "=" + v)
     else:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             elif isinstance(v, str):
                 v = quote_via(v, safe, encoding, errors)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             else:
                 try:
                     # Is this a sufficient test for sequence-ness?
                     x = len(v)
                 except TypeError:
                     # not a sequence
                     v = quote_via(str(v), safe, encoding, errors)
-                    l.append(k + '=' + v)
+                    l.append(k + "=" + v)
                 else:
                     # loop over the sequence
                     for elt in v:
                         if isinstance(elt, bytes):
                             elt = quote_via(elt, safe)
                         else:
                             elt = quote_via(str(elt), safe, encoding, errors)
-                        l.append(k + '=' + elt)
-    return '&'.join(l)
+                        l.append(k + "=" + elt)
+    return "&".join(l)
+
 
 def to_bytes(url):
+    warnings.warn(
+        "urllib.parse.to_bytes() is deprecated as of 3.8",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _to_bytes(url)
+
+
+def _to_bytes(url):
     """to_bytes(u"URL") --> 'URL'."""
     # Most URL schemes require ASCII. If that changes, the conversion
     # can be relaxed.
     # XXX get rid of to_bytes()
     if isinstance(url, str):
         try:
             url = url.encode("ASCII").decode()
         except UnicodeError:
-            raise UnicodeError("URL " + repr(url) +
-                               " contains non-ASCII characters")
+            raise UnicodeError("URL " + repr(url) + " contains non-ASCII characters")
     return url
 
+
 def unwrap(url):
-    """unwrap('<URL:type://host/path>') --> 'type://host/path'."""
+    """Transform a string like '<URL:scheme://host/path>' into 'scheme://host/path'.
+
+    The string is returned unchanged if it's not a wrapped URL.
+    """
     url = str(url).strip()
-    if url[:1] == '<' and url[-1:] == '>':
+    if url[:1] == "<" and url[-1:] == ">":
         url = url[1:-1].strip()
-    if url[:4] == 'URL:': url = url[4:].strip()
+    if url[:4] == "URL:":
+        url = url[4:].strip()
     return url
 
-_typeprog = None
+
 def splittype(url):
+    warnings.warn(
+        "urllib.parse.splittype() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splittype(url)
+
+
+_typeprog = None
+
+
+def _splittype(url):
     """splittype('type:opaquestring') --> 'type', 'opaquestring'."""
     global _typeprog
     if _typeprog is None:
-        _typeprog = re.compile('([^/:]+):(.*)', re.DOTALL)
+        _typeprog = re.compile("([^/:]+):(.*)", re.DOTALL)
 
     match = _typeprog.match(url)
     if match:
         scheme, data = match.groups()
         return scheme.lower(), data
     return None, url
 
-_hostprog = None
+
 def splithost(url):
+    warnings.warn(
+        "urllib.parse.splithost() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splithost(url)
+
+
+_hostprog = None
+
+
+def _splithost(url):
     """splithost('//host[:port]/path') --> 'host[:port]', '/path'."""
     global _hostprog
     if _hostprog is None:
-        _hostprog = re.compile('//([^/#?]*)(.*)', re.DOTALL)
+        _hostprog = re.compile("//([^/#?]*)(.*)", re.DOTALL)
 
     match = _hostprog.match(url)
     if match:
         host_port, path = match.groups()
-        if path and path[0] != '/':
-            path = '/' + path
+        if path and path[0] != "/":
+            path = "/" + path
         return host_port, path
     return None, url
 
+
 def splituser(host):
+    warnings.warn(
+        "urllib.parse.splituser() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splituser(host)
+
+
+def _splituser(host):
     """splituser('user[:passwd]@host[:port]') --> 'user[:passwd]', 'host[:port]'."""
-    user, delim, host = host.rpartition('@')
+    user, delim, host = host.rpartition("@")
     return (user if delim else None), host
 
+
 def splitpasswd(user):
+    warnings.warn(
+        "urllib.parse.splitpasswd() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitpasswd(user)
+
+
+def _splitpasswd(user):
     """splitpasswd('user:passwd') -> 'user', 'passwd'."""
-    user, delim, passwd = user.partition(':')
+    user, delim, passwd = user.partition(":")
     return user, (passwd if delim else None)
 
+
+def splitport(host):
+    warnings.warn(
+        "urllib.parse.splitport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitport(host)
+
+
 # splittag('/path#tag') --> '/path', 'tag'
 _portprog = None
-def splitport(host):
+
+
+def _splitport(host):
     """splitport('host:port') --> 'host', 'port'."""
     global _portprog
     if _portprog is None:
-        _portprog = re.compile('(.*):([0-9]*)', re.DOTALL)
+        _portprog = re.compile("(.*):([0-9]*)", re.DOTALL)
 
     match = _portprog.fullmatch(host)
     if match:
         host, port = match.groups()
         if port:
             return host, port
     return host, None
 
+
 def splitnport(host, defport=-1):
+    warnings.warn(
+        "urllib.parse.splitnport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitnport(host, defport)
+
+
+def _splitnport(host, defport=-1):
     """Split host and port, returning numeric port.
     Return given default port if no ':' found; defaults to -1.
     Return numerical port if a valid number are found after ':'.
     Return None if ':' but not a valid number."""
-    host, delim, port = host.rpartition(':')
+    host, delim, port = host.rpartition(":")
     if not delim:
         host = port
     elif port:
         try:
             nport = int(port)
         except ValueError:
             nport = None
         return host, nport
     return host, defport
 
+
 def splitquery(url):
+    warnings.warn(
+        "urllib.parse.splitquery() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitquery(url)
+
+
+def _splitquery(url):
     """splitquery('/path?query') --> '/path', 'query'."""
-    path, delim, query = url.rpartition('?')
+    path, delim, query = url.rpartition("?")
     if delim:
         return path, query
     return url, None
 
+
 def splittag(url):
+    warnings.warn(
+        "urllib.parse.splittag() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splittag(url)
+
+
+def _splittag(url):
     """splittag('/path#tag') --> '/path', 'tag'."""
-    path, delim, tag = url.rpartition('#')
+    path, delim, tag = url.rpartition("#")
     if delim:
         return path, tag
     return url, None
 
+
 def splitattr(url):
+    warnings.warn(
+        "urllib.parse.splitattr() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitattr(url)
+
+
+def _splitattr(url):
     """splitattr('/path;attr1=value1;attr2=value2;...') ->
-        '/path', ['attr1=value1', 'attr2=value2', ...]."""
-    words = url.split(';')
+    '/path', ['attr1=value1', 'attr2=value2', ...]."""
+    words = url.split(";")
     return words[0], words[1:]
 
+
 def splitvalue(attr):
+    warnings.warn(
+        "urllib.parse.splitvalue() is deprecated as of 3.8, "
+        "use urllib.parse.parse_qsl() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return _splitvalue(attr)
+
+
+def _splitvalue(attr):
     """splitvalue('attr=value') --> 'attr', 'value'."""
-    attr, delim, value = attr.partition('=')
+    attr, delim, value = attr.partition("=")
     return attr, (value if delim else None)
```

### Comparing `ignition-gemini-0.1.8/ignition/python/python3_8/Lib/urllib/parse.py` & `ignition_gemini-0.2.0/ignition/python/python3_8/Lib/urllib/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,93 +23,202 @@
 urlparse module should conform with it.  The urlparse module is
 currently not entirely compliant with this RFC due to defacto
 scenarios for parsing, and for backward compatibility purposes, some
 parsing quirks from older RFCs are retained. The testcases in
 test_urlparse.py provides a good indicator of parsing behavior.
 """
 
+import collections
 import re
 import sys
-import collections
 import warnings
 
-__all__ = ["urlparse", "urlunparse", "urljoin", "urldefrag",
-           "urlsplit", "urlunsplit", "urlencode", "parse_qs",
-           "parse_qsl", "quote", "quote_plus", "quote_from_bytes",
-           "unquote", "unquote_plus", "unquote_to_bytes",
-           "DefragResult", "ParseResult", "SplitResult",
-           "DefragResultBytes", "ParseResultBytes", "SplitResultBytes"]
+__all__ = [
+    "urlparse",
+    "urlunparse",
+    "urljoin",
+    "urldefrag",
+    "urlsplit",
+    "urlunsplit",
+    "urlencode",
+    "parse_qs",
+    "parse_qsl",
+    "quote",
+    "quote_plus",
+    "quote_from_bytes",
+    "unquote",
+    "unquote_plus",
+    "unquote_to_bytes",
+    "DefragResult",
+    "ParseResult",
+    "SplitResult",
+    "DefragResultBytes",
+    "ParseResultBytes",
+    "SplitResultBytes",
+]
 
 # A classification of schemes.
 # The empty string classifies URLs with no scheme specified,
 # being the default value returned by “urlsplit” and “urlparse”.
 
-uses_relative = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'imap', # PATCH added gemini
-                 'wais', 'file', 'https', 'shttp', 'mms',
-                 'prospero', 'rtsp', 'rtspu', 'sftp',
-                 'svn', 'svn+ssh', 'ws', 'wss']
-
-uses_netloc = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'telnet', # PATCH added gemini
-               'imap', 'wais', 'file', 'mms', 'https', 'shttp',
-               'snews', 'prospero', 'rtsp', 'rtspu', 'rsync',
-               'svn', 'svn+ssh', 'sftp', 'nfs', 'git', 'git+ssh',
-               'ws', 'wss']
-
-uses_params = ['', 'ftp', 'gemini', 'hdl', 'prospero', 'http', 'imap', # PATCH added gemini
-               'https', 'shttp', 'rtsp', 'rtspu', 'sip', 'sips',
-               'mms', 'sftp', 'tel']
+uses_relative = [
+    "",
+    "ftp",
+    "http",
+    "gemini",
+    "gopher",
+    "nntp",
+    "imap",  # PATCH added gemini
+    "wais",
+    "file",
+    "https",
+    "shttp",
+    "mms",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "sftp",
+    "svn",
+    "svn+ssh",
+    "ws",
+    "wss",
+]
+
+uses_netloc = [
+    "",
+    "ftp",
+    "http",
+    "gemini",
+    "gopher",
+    "nntp",
+    "telnet",  # PATCH added gemini
+    "imap",
+    "wais",
+    "file",
+    "mms",
+    "https",
+    "shttp",
+    "snews",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "rsync",
+    "svn",
+    "svn+ssh",
+    "sftp",
+    "nfs",
+    "git",
+    "git+ssh",
+    "ws",
+    "wss",
+]
+
+uses_params = [
+    "",
+    "ftp",
+    "gemini",
+    "hdl",
+    "prospero",
+    "http",
+    "imap",  # PATCH added gemini
+    "https",
+    "shttp",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+    "mms",
+    "sftp",
+    "tel",
+]
 
 # These are not actually used anymore, but should stay for backwards
 # compatibility.  (They are undocumented, but have a public-looking name.)
 
-non_hierarchical = ['gopher', 'hdl', 'mailto', 'news',
-                    'telnet', 'wais', 'imap', 'snews', 'sip', 'sips']
-
-uses_query = ['', 'http', 'wais', 'imap', 'https', 'shttp', 'mms',
-              'gopher', 'rtsp', 'rtspu', 'sip', 'sips']
-
-uses_fragment = ['', 'ftp', 'hdl', 'http', 'gopher', 'news',
-                 'nntp', 'wais', 'https', 'shttp', 'snews',
-                 'file', 'prospero']
+non_hierarchical = [
+    "gopher",
+    "hdl",
+    "mailto",
+    "news",
+    "telnet",
+    "wais",
+    "imap",
+    "snews",
+    "sip",
+    "sips",
+]
+
+uses_query = [
+    "",
+    "http",
+    "wais",
+    "imap",
+    "https",
+    "shttp",
+    "mms",
+    "gopher",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+]
+
+uses_fragment = [
+    "",
+    "ftp",
+    "hdl",
+    "http",
+    "gopher",
+    "news",
+    "nntp",
+    "wais",
+    "https",
+    "shttp",
+    "snews",
+    "file",
+    "prospero",
+]
 
 # Characters valid in scheme names
-scheme_chars = ('abcdefghijklmnopqrstuvwxyz'
-                'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                '0123456789'
-                '+-.')
+scheme_chars = (
+    "abcdefghijklmnopqrstuvwxyz" "ABCDEFGHIJKLMNOPQRSTUVWXYZ" "0123456789" "+-."
+)
 
 # XXX: Consider replacing with functools.lru_cache
 MAX_CACHE_SIZE = 20
 _parse_cache = {}
 
+
 def clear_cache():
     """Clear the parse cache and the quoters cache."""
     _parse_cache.clear()
     _safe_quoters.clear()
 
 
 # Helpers for bytes handling
 # For 3.2, we deliberately require applications that
 # handle improperly quoted URLs to do their own
 # decoding and encoding. If valid use cases are
 # presented, we may relax this by using latin-1
 # decoding internally for 3.3
-_implicit_encoding = 'ascii'
-_implicit_errors = 'strict'
+_implicit_encoding = "ascii"
+_implicit_errors = "strict"
+
 
 def _noop(obj):
     return obj
 
-def _encode_result(obj, encoding=_implicit_encoding,
-                        errors=_implicit_errors):
+
+def _encode_result(obj, encoding=_implicit_encoding, errors=_implicit_errors):
     return obj.encode(encoding, errors)
 
-def _decode_args(args, encoding=_implicit_encoding,
-                       errors=_implicit_errors):
-    return tuple(x.decode(encoding, errors) if x else '' for x in args)
+
+def _decode_args(args, encoding=_implicit_encoding, errors=_implicit_errors):
+    return tuple(x.decode(encoding, errors) if x else "" for x in args)
+
 
 def _coerce_args(*args):
     # Invokes decode if necessary to create str args
     # and returns the coerced inputs along with
     # an appropriate result coercion function
     #   - noop for str inputs
     #   - encoding function otherwise
@@ -119,33 +228,37 @@
         # "scheme=''" default argument to some functions
         if arg and isinstance(arg, str) != str_input:
             raise TypeError("Cannot mix str and non-str arguments")
     if str_input:
         return args + (_noop,)
     return _decode_args(args) + (_encode_result,)
 
+
 # Result objects are more helpful than simple tuples
 class _ResultMixinStr(object):
     """Standard approach to encoding parsed results from str to bytes"""
+
     __slots__ = ()
 
-    def encode(self, encoding='ascii', errors='strict'):
+    def encode(self, encoding="ascii", errors="strict"):
         return self._encoded_counterpart(*(x.encode(encoding, errors) for x in self))
 
 
 class _ResultMixinBytes(object):
     """Standard approach to decoding parsed results from bytes to str"""
+
     __slots__ = ()
 
-    def decode(self, encoding='ascii', errors='strict'):
+    def decode(self, encoding="ascii", errors="strict"):
         return self._decoded_counterpart(*(x.decode(encoding, errors) for x in self))
 
 
 class _NetlocResultMixinBase(object):
     """Shared methods for the parsed result objects containing a netloc element"""
+
     __slots__ = ()
 
     @property
     def username(self):
         return self._userinfo[0]
 
     @property
@@ -155,99 +268,97 @@
     @property
     def hostname(self):
         hostname = self._hostinfo[0]
         if not hostname:
             return None
         # Scoped IPv6 address may have zone info, which must not be lowercased
         # like http://[fe80::822a:a8ff:fe49:470c%tESt]:1234/keys
-        separator = '%' if isinstance(hostname, str) else b'%'
+        separator = "%" if isinstance(hostname, str) else b"%"
         hostname, percent, zone = hostname.partition(separator)
         return hostname.lower() + percent + zone
 
     @property
     def port(self):
         port = self._hostinfo[1]
         if port is not None:
             try:
                 port = int(port, 10)
             except ValueError:
-                message = f'Port could not be cast to integer value as {port!r}'
+                message = f"Port could not be cast to integer value as {port!r}"
                 raise ValueError(message) from None
-            if not ( 0 <= port <= 65535):
+            if not (0 <= port <= 65535):
                 raise ValueError("Port out of range 0-65535")
         return port
 
 
 class _NetlocResultMixinStr(_NetlocResultMixinBase, _ResultMixinStr):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition('@')
+        userinfo, have_info, hostinfo = netloc.rpartition("@")
         if have_info:
-            username, have_password, password = userinfo.partition(':')
+            username, have_password, password = userinfo.partition(":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition('@')
-        _, have_open_br, bracketed = hostinfo.partition('[')
+        _, _, hostinfo = netloc.rpartition("@")
+        _, have_open_br, bracketed = hostinfo.partition("[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(']')
-            _, _, port = port.partition(':')
+            hostname, _, port = bracketed.partition("]")
+            _, _, port = port.partition(":")
         else:
-            hostname, _, port = hostinfo.partition(':')
+            hostname, _, port = hostinfo.partition(":")
         if not port:
             port = None
         return hostname, port
 
 
 class _NetlocResultMixinBytes(_NetlocResultMixinBase, _ResultMixinBytes):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition(b'@')
+        userinfo, have_info, hostinfo = netloc.rpartition(b"@")
         if have_info:
-            username, have_password, password = userinfo.partition(b':')
+            username, have_password, password = userinfo.partition(b":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition(b'@')
-        _, have_open_br, bracketed = hostinfo.partition(b'[')
+        _, _, hostinfo = netloc.rpartition(b"@")
+        _, have_open_br, bracketed = hostinfo.partition(b"[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(b']')
-            _, _, port = port.partition(b':')
+            hostname, _, port = bracketed.partition(b"]")
+            _, _, port = port.partition(b":")
         else:
-            hostname, _, port = hostinfo.partition(b':')
+            hostname, _, port = hostinfo.partition(b":")
         if not port:
             port = None
         return hostname, port
 
 
 from collections import namedtuple
 
-_DefragResultBase = namedtuple('DefragResult', 'url fragment')
-_SplitResultBase = namedtuple(
-    'SplitResult', 'scheme netloc path query fragment')
-_ParseResultBase = namedtuple(
-    'ParseResult', 'scheme netloc path params query fragment')
+_DefragResultBase = namedtuple("DefragResult", "url fragment")
+_SplitResultBase = namedtuple("SplitResult", "scheme netloc path query fragment")
+_ParseResultBase = namedtuple("ParseResult", "scheme netloc path params query fragment")
 
 _DefragResultBase.__doc__ = """
 DefragResult(url, fragment)
 
 A 2-tuple that contains the url without fragment identifier and the fragment
 identifier as a separate argument.
 """
@@ -310,487 +421,549 @@
 # ResultBase is no longer part of the documented API, but it is
 # retained since deprecating it isn't worth the hassle
 ResultBase = _NetlocResultMixinStr
 
 # Structured result objects for string data
 class DefragResult(_DefragResultBase, _ResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + '#' + self.fragment
+            return self.url + "#" + self.fragment
         else:
             return self.url
 
+
 class SplitResult(_SplitResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResult(_ParseResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Structured result objects for bytes data
 class DefragResultBytes(_DefragResultBase, _ResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + b'#' + self.fragment
+            return self.url + b"#" + self.fragment
         else:
             return self.url
 
+
 class SplitResultBytes(_SplitResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResultBytes(_ParseResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Set up the encode/decode result pairs
 def _fix_result_transcoding():
     _result_pairs = (
         (DefragResult, DefragResultBytes),
         (SplitResult, SplitResultBytes),
         (ParseResult, ParseResultBytes),
     )
     for _decoded, _encoded in _result_pairs:
         _decoded._encoded_counterpart = _encoded
         _encoded._decoded_counterpart = _decoded
 
+
 _fix_result_transcoding()
 del _fix_result_transcoding
 
-def urlparse(url, scheme='', allow_fragments=True):
+
+def urlparse(url, scheme="", allow_fragments=True):
     """Parse a URL into 6 components:
     <scheme>://<netloc>/<path>;<params>?<query>#<fragment>
     Return a 6-tuple: (scheme, netloc, path, params, query, fragment).
     Note that we don't break the components up in smaller bits
     (e.g. netloc is a single string) and we don't expand % escapes."""
     url, scheme, _coerce_result = _coerce_args(url, scheme)
     splitresult = urlsplit(url, scheme, allow_fragments)
     scheme, netloc, url, query, fragment = splitresult
-    if scheme in uses_params and ';' in url:
+    if scheme in uses_params and ";" in url:
         url, params = _splitparams(url)
     else:
-        params = ''
+        params = ""
     result = ParseResult(scheme, netloc, url, params, query, fragment)
     return _coerce_result(result)
 
+
 def _splitparams(url):
-    if '/'  in url:
-        i = url.find(';', url.rfind('/'))
+    if "/" in url:
+        i = url.find(";", url.rfind("/"))
         if i < 0:
-            return url, ''
+            return url, ""
     else:
-        i = url.find(';')
-    return url[:i], url[i+1:]
+        i = url.find(";")
+    return url[:i], url[i + 1 :]
+
 
 def _splitnetloc(url, start=0):
-    delim = len(url)   # position of end of domain part of url, default is end
-    for c in '/?#':    # look for delimiters; the order is NOT important
-        wdelim = url.find(c, start)        # find first of this delim
-        if wdelim >= 0:                    # if found
-            delim = min(delim, wdelim)     # use earliest delim position
-    return url[start:delim], url[delim:]   # return (domain, rest)
+    delim = len(url)  # position of end of domain part of url, default is end
+    for c in "/?#":  # look for delimiters; the order is NOT important
+        wdelim = url.find(c, start)  # find first of this delim
+        if wdelim >= 0:  # if found
+            delim = min(delim, wdelim)  # use earliest delim position
+    return url[start:delim], url[delim:]  # return (domain, rest)
+
 
 def _checknetloc(netloc):
     if not netloc or netloc.isascii():
         return
     # looking for characters like \u2100 that expand to 'a/c'
     # IDNA uses NFKC equivalence, so normalize for this check
     import unicodedata
-    n = netloc.replace('@', '')   # ignore characters already included
-    n = n.replace(':', '')        # but not the surrounding text
-    n = n.replace('#', '')
-    n = n.replace('?', '')
-    netloc2 = unicodedata.normalize('NFKC', n)
+
+    n = netloc.replace("@", "")  # ignore characters already included
+    n = n.replace(":", "")  # but not the surrounding text
+    n = n.replace("#", "")
+    n = n.replace("?", "")
+    netloc2 = unicodedata.normalize("NFKC", n)
     if n == netloc2:
         return
-    for c in '/?#@:':
+    for c in "/?#@:":
         if c in netloc2:
-            raise ValueError("netloc '" + netloc + "' contains invalid " +
-                             "characters under NFKC normalization")
+            raise ValueError(
+                "netloc '"
+                + netloc
+                + "' contains invalid "
+                + "characters under NFKC normalization"
+            )
 
-def urlsplit(url, scheme='', allow_fragments=True):
+
+def urlsplit(url, scheme="", allow_fragments=True):
     """Parse a URL into 5 components:
     <scheme>://<netloc>/<path>?<query>#<fragment>
     Return a 5-tuple: (scheme, netloc, path, query, fragment).
     Note that we don't break the components up in smaller bits
     (e.g. netloc is a single string) and we don't expand % escapes."""
     url, scheme, _coerce_result = _coerce_args(url, scheme)
     allow_fragments = bool(allow_fragments)
     key = url, scheme, allow_fragments, type(url), type(scheme)
     cached = _parse_cache.get(key, None)
     if cached:
         return _coerce_result(cached)
-    if len(_parse_cache) >= MAX_CACHE_SIZE: # avoid runaway growth
+    if len(_parse_cache) >= MAX_CACHE_SIZE:  # avoid runaway growth
         clear_cache()
-    netloc = query = fragment = ''
-    i = url.find(':')
+    netloc = query = fragment = ""
+    i = url.find(":")
     if i > 0:
-        if url[:i] == 'http': # optimize the common case
-            url = url[i+1:]
-            if url[:2] == '//':
+        if url[:i] == "http":  # optimize the common case
+            url = url[i + 1 :]
+            if url[:2] == "//":
                 netloc, url = _splitnetloc(url, 2)
-                if (('[' in netloc and ']' not in netloc) or
-                        (']' in netloc and '[' not in netloc)):
+                if ("[" in netloc and "]" not in netloc) or (
+                    "]" in netloc and "[" not in netloc
+                ):
                     raise ValueError("Invalid IPv6 URL")
-            if allow_fragments and '#' in url:
-                url, fragment = url.split('#', 1)
-            if '?' in url:
-                url, query = url.split('?', 1)
+            if allow_fragments and "#" in url:
+                url, fragment = url.split("#", 1)
+            if "?" in url:
+                url, query = url.split("?", 1)
             _checknetloc(netloc)
-            v = SplitResult('http', netloc, url, query, fragment)
+            v = SplitResult("http", netloc, url, query, fragment)
             _parse_cache[key] = v
             return _coerce_result(v)
         for c in url[:i]:
             if c not in scheme_chars:
                 break
         else:
             # make sure "url" is not actually a port number (in which case
             # "scheme" is really part of the path)
-            rest = url[i+1:]
-            if not rest or any(c not in '0123456789' for c in rest):
+            rest = url[i + 1 :]
+            if not rest or any(c not in "0123456789" for c in rest):
                 # not a port number
                 scheme, url = url[:i].lower(), rest
 
-    if url[:2] == '//':
+    if url[:2] == "//":
         netloc, url = _splitnetloc(url, 2)
-        if (('[' in netloc and ']' not in netloc) or
-                (']' in netloc and '[' not in netloc)):
+        if ("[" in netloc and "]" not in netloc) or (
+            "]" in netloc and "[" not in netloc
+        ):
             raise ValueError("Invalid IPv6 URL")
-    if allow_fragments and '#' in url:
-        url, fragment = url.split('#', 1)
-    if '?' in url:
-        url, query = url.split('?', 1)
+    if allow_fragments and "#" in url:
+        url, fragment = url.split("#", 1)
+    if "?" in url:
+        url, query = url.split("?", 1)
     _checknetloc(netloc)
     v = SplitResult(scheme, netloc, url, query, fragment)
     _parse_cache[key] = v
     return _coerce_result(v)
 
+
 def urlunparse(components):
     """Put a parsed URL back together again.  This may result in a
     slightly different, but equivalent URL, if the URL that was parsed
     originally had redundant delimiters, e.g. a ? with an empty query
     (the draft states that these are equivalent)."""
-    scheme, netloc, url, params, query, fragment, _coerce_result = (
-                                                  _coerce_args(*components))
+    scheme, netloc, url, params, query, fragment, _coerce_result = _coerce_args(
+        *components
+    )
     if params:
         url = "%s;%s" % (url, params)
     return _coerce_result(urlunsplit((scheme, netloc, url, query, fragment)))
 
+
 def urlunsplit(components):
     """Combine the elements of a tuple as returned by urlsplit() into a
     complete URL as a string. The data argument can be any five-item iterable.
     This may result in a slightly different, but equivalent URL, if the URL that
     was parsed originally had unnecessary delimiters (for example, a ? with an
     empty query; the RFC states that these are equivalent)."""
-    scheme, netloc, url, query, fragment, _coerce_result = (
-                                          _coerce_args(*components))
-    if netloc or (scheme and scheme in uses_netloc and url[:2] != '//'):
-        if url and url[:1] != '/': url = '/' + url
-        url = '//' + (netloc or '') + url
+    scheme, netloc, url, query, fragment, _coerce_result = _coerce_args(*components)
+    if netloc or (scheme and scheme in uses_netloc and url[:2] != "//"):
+        if url and url[:1] != "/":
+            url = "/" + url
+        url = "//" + (netloc or "") + url
     if scheme:
-        url = scheme + ':' + url
+        url = scheme + ":" + url
     if query:
-        url = url + '?' + query
+        url = url + "?" + query
     if fragment:
-        url = url + '#' + fragment
+        url = url + "#" + fragment
     return _coerce_result(url)
 
+
 def urljoin(base, url, allow_fragments=True):
     """Join a base URL and a possibly relative URL to form an absolute
     interpretation of the latter."""
     if not base:
         return url
     if not url:
         return base
 
     base, url, _coerce_result = _coerce_args(base, url)
-    bscheme, bnetloc, bpath, bparams, bquery, bfragment = \
-            urlparse(base, '', allow_fragments)
-    scheme, netloc, path, params, query, fragment = \
-            urlparse(url, bscheme, allow_fragments)
+    bscheme, bnetloc, bpath, bparams, bquery, bfragment = urlparse(
+        base, "", allow_fragments
+    )
+    scheme, netloc, path, params, query, fragment = urlparse(
+        url, bscheme, allow_fragments
+    )
 
     if scheme != bscheme or scheme not in uses_relative:
         return _coerce_result(url)
     if scheme in uses_netloc:
         if netloc:
-            return _coerce_result(urlunparse((scheme, netloc, path,
-                                              params, query, fragment)))
+            return _coerce_result(
+                urlunparse((scheme, netloc, path, params, query, fragment))
+            )
         netloc = bnetloc
 
     if not path and not params:
         path = bpath
         params = bparams
         if not query:
             query = bquery
-        return _coerce_result(urlunparse((scheme, netloc, path,
-                                          params, query, fragment)))
+        return _coerce_result(
+            urlunparse((scheme, netloc, path, params, query, fragment))
+        )
 
-    base_parts = bpath.split('/')
-    if base_parts[-1] != '':
+    base_parts = bpath.split("/")
+    if base_parts[-1] != "":
         # the last item is not a directory, so will not be taken into account
         # in resolving the relative path
         del base_parts[-1]
 
     # for rfc3986, ignore all base path should the first character be root.
-    if path[:1] == '/':
-        segments = path.split('/')
+    if path[:1] == "/":
+        segments = path.split("/")
     else:
-        segments = base_parts + path.split('/')
+        segments = base_parts + path.split("/")
         # filter out elements that would cause redundant slashes on re-joining
         # the resolved_path
         segments[1:-1] = filter(None, segments[1:-1])
 
     resolved_path = []
 
     for seg in segments:
-        if seg == '..':
+        if seg == "..":
             try:
                 resolved_path.pop()
             except IndexError:
                 # ignore any .. segments that would otherwise cause an IndexError
                 # when popped from resolved_path if resolving for rfc3986
                 pass
-        elif seg == '.':
+        elif seg == ".":
             continue
         else:
             resolved_path.append(seg)
 
-    if segments[-1] in ('.', '..'):
+    if segments[-1] in (".", ".."):
         # do some post-processing here. if the last segment was a relative dir,
         # then we need to append the trailing '/'
-        resolved_path.append('')
+        resolved_path.append("")
 
-    return _coerce_result(urlunparse((scheme, netloc, '/'.join(
-        resolved_path) or '/', params, query, fragment)))
+    return _coerce_result(
+        urlunparse(
+            (scheme, netloc, "/".join(resolved_path) or "/", params, query, fragment)
+        )
+    )
 
 
 def urldefrag(url):
     """Removes any existing fragment from URL.
 
     Returns a tuple of the defragmented URL and the fragment.  If
     the URL contained no fragments, the second element is the
     empty string.
     """
     url, _coerce_result = _coerce_args(url)
-    if '#' in url:
+    if "#" in url:
         s, n, p, a, q, frag = urlparse(url)
-        defrag = urlunparse((s, n, p, a, q, ''))
+        defrag = urlunparse((s, n, p, a, q, ""))
     else:
-        frag = ''
+        frag = ""
         defrag = url
     return _coerce_result(DefragResult(defrag, frag))
 
-_hexdig = '0123456789ABCDEFabcdef'
+
+_hexdig = "0123456789ABCDEFabcdef"
 _hextobyte = None
 
+
 def unquote_to_bytes(string):
     """unquote_to_bytes('abc%20def') -> b'abc def'."""
     # Note: strings are encoded as UTF-8. This is only an issue if it contains
     # unescaped non-ASCII characters, which URIs should not.
     if not string:
         # Is it a string-like object?
         string.split
-        return b''
+        return b""
     if isinstance(string, str):
-        string = string.encode('utf-8')
-    bits = string.split(b'%')
+        string = string.encode("utf-8")
+    bits = string.split(b"%")
     if len(bits) == 1:
         return string
     res = [bits[0]]
     append = res.append
     # Delay the initialization of the table to not waste memory
     # if the function is never called
     global _hextobyte
     if _hextobyte is None:
-        _hextobyte = {(a + b).encode(): bytes.fromhex(a + b)
-                      for a in _hexdig for b in _hexdig}
+        _hextobyte = {
+            (a + b).encode(): bytes.fromhex(a + b) for a in _hexdig for b in _hexdig
+        }
     for item in bits[1:]:
         try:
             append(_hextobyte[item[:2]])
             append(item[2:])
         except KeyError:
-            append(b'%')
+            append(b"%")
             append(item)
-    return b''.join(res)
+    return b"".join(res)
+
 
-_asciire = re.compile('([\x00-\x7f]+)')
+_asciire = re.compile("([\x00-\x7f]+)")
 
-def unquote(string, encoding='utf-8', errors='replace'):
+
+def unquote(string, encoding="utf-8", errors="replace"):
     """Replace %xx escapes by their single-character equivalent. The optional
     encoding and errors parameters specify how to decode percent-encoded
     sequences into Unicode characters, as accepted by the bytes.decode()
     method.
     By default, percent-encoded sequences are decoded with UTF-8, and invalid
     sequences are replaced by a placeholder character.
 
     unquote('abc%20def') -> 'abc def'.
     """
     if isinstance(string, bytes):
-        raise TypeError('Expected str, got bytes')
-    if '%' not in string:
+        raise TypeError("Expected str, got bytes")
+    if "%" not in string:
         string.split
         return string
     if encoding is None:
-        encoding = 'utf-8'
+        encoding = "utf-8"
     if errors is None:
-        errors = 'replace'
+        errors = "replace"
     bits = _asciire.split(string)
     res = [bits[0]]
     append = res.append
     for i in range(1, len(bits), 2):
         append(unquote_to_bytes(bits[i]).decode(encoding, errors))
         append(bits[i + 1])
-    return ''.join(res)
+    return "".join(res)
 
 
-def parse_qs(qs, keep_blank_values=False, strict_parsing=False,
-             encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qs(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
 
-        qs: percent-encoded query string to be parsed
+    qs: percent-encoded query string to be parsed
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as
-            blank strings.  The default false value indicates that
-            blank values are to be ignored and treated as if they were
-            not included.
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as
+        blank strings.  The default false value indicates that
+        blank values are to be ignored and treated as if they were
+        not included.
 
-        strict_parsing: flag indicating what to do with parsing errors.
-            If false (the default), errors are silently ignored.
-            If true, errors raise a ValueError exception.
+    strict_parsing: flag indicating what to do with parsing errors.
+        If false (the default), errors are silently ignored.
+        If true, errors raise a ValueError exception.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        max_num_fields: int. If set, then throws a ValueError if there
-            are more than n fields read by parse_qsl().
+    max_num_fields: int. If set, then throws a ValueError if there
+        are more than n fields read by parse_qsl().
 
-        Returns a dictionary.
+    Returns a dictionary.
     """
     parsed_result = {}
-    pairs = parse_qsl(qs, keep_blank_values, strict_parsing,
-                      encoding=encoding, errors=errors,
-                      max_num_fields=max_num_fields)
+    pairs = parse_qsl(
+        qs,
+        keep_blank_values,
+        strict_parsing,
+        encoding=encoding,
+        errors=errors,
+        max_num_fields=max_num_fields,
+    )
     for name, value in pairs:
         if name in parsed_result:
             parsed_result[name].append(value)
         else:
             parsed_result[name] = [value]
     return parsed_result
 
 
-def parse_qsl(qs, keep_blank_values=False, strict_parsing=False,
-              encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qsl(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
 
-        qs: percent-encoded query string to be parsed
+    qs: percent-encoded query string to be parsed
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as blank
-            strings.  The default false value indicates that blank values
-            are to be ignored and treated as if they were  not included.
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as blank
+        strings.  The default false value indicates that blank values
+        are to be ignored and treated as if they were  not included.
 
-        strict_parsing: flag indicating what to do with parsing errors. If
-            false (the default), errors are silently ignored. If true,
-            errors raise a ValueError exception.
+    strict_parsing: flag indicating what to do with parsing errors. If
+        false (the default), errors are silently ignored. If true,
+        errors raise a ValueError exception.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        max_num_fields: int. If set, then throws a ValueError
-            if there are more than n fields read by parse_qsl().
+    max_num_fields: int. If set, then throws a ValueError
+        if there are more than n fields read by parse_qsl().
 
-        Returns a list, as G-d intended.
+    Returns a list, as G-d intended.
     """
     qs, _coerce_result = _coerce_args(qs)
 
     # If max_num_fields is defined then check that the number of fields
     # is less than max_num_fields. This prevents a memory exhaustion DOS
     # attack via post bodies with many fields.
     if max_num_fields is not None:
-        num_fields = 1 + qs.count('&') + qs.count(';')
+        num_fields = 1 + qs.count("&") + qs.count(";")
         if max_num_fields < num_fields:
-            raise ValueError('Max number of fields exceeded')
+            raise ValueError("Max number of fields exceeded")
 
-    pairs = [s2 for s1 in qs.split('&') for s2 in s1.split(';')]
+    pairs = [s2 for s1 in qs.split("&") for s2 in s1.split(";")]
     r = []
     for name_value in pairs:
         if not name_value and not strict_parsing:
             continue
-        nv = name_value.split('=', 1)
+        nv = name_value.split("=", 1)
         if len(nv) != 2:
             if strict_parsing:
                 raise ValueError("bad query field: %r" % (name_value,))
             # Handle case of a control-name with no equal sign
             if keep_blank_values:
-                nv.append('')
+                nv.append("")
             else:
                 continue
         if len(nv[1]) or keep_blank_values:
-            name = nv[0].replace('+', ' ')
+            name = nv[0].replace("+", " ")
             name = unquote(name, encoding=encoding, errors=errors)
             name = _coerce_result(name)
-            value = nv[1].replace('+', ' ')
+            value = nv[1].replace("+", " ")
             value = unquote(value, encoding=encoding, errors=errors)
             value = _coerce_result(value)
             r.append((name, value))
     return r
 
-def unquote_plus(string, encoding='utf-8', errors='replace'):
+
+def unquote_plus(string, encoding="utf-8", errors="replace"):
     """Like unquote(), but also replace plus signs by spaces, as required for
     unquoting HTML form values.
 
     unquote_plus('%7e/abc+def') -> '~/abc def'
     """
-    string = string.replace('+', ' ')
+    string = string.replace("+", " ")
     return unquote(string, encoding, errors)
 
-_ALWAYS_SAFE = frozenset(b'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                         b'abcdefghijklmnopqrstuvwxyz'
-                         b'0123456789'
-                         b'_.-~')
+
+_ALWAYS_SAFE = frozenset(
+    b"ABCDEFGHIJKLMNOPQRSTUVWXYZ" b"abcdefghijklmnopqrstuvwxyz" b"0123456789" b"_.-~"
+)
 _ALWAYS_SAFE_BYTES = bytes(_ALWAYS_SAFE)
 _safe_quoters = {}
 
+
 class Quoter(collections.defaultdict):
     """A mapping from bytes (in range(0,256)) to strings.
 
     String values are percent-encoded byte values, unless the key < 128, and
     in the "safe" set (either the specified safe set, or default set).
     """
+
     # Keeps a cache internally, using defaultdict, for efficiency (lookups
     # of cached keys don't call Python code at all).
     def __init__(self, safe):
         """safe: bytes object."""
         self.safe = _ALWAYS_SAFE.union(safe)
 
     def __repr__(self):
         # Without this, will just display as a defaultdict
         return "<%s %r>" % (self.__class__.__name__, dict(self))
 
     def __missing__(self, b):
         # Handle a cache miss. Store quoted string in cache and return.
-        res = chr(b) if b in self.safe else '%{:02X}'.format(b)
+        res = chr(b) if b in self.safe else "%{:02X}".format(b)
         self[b] = res
         return res
 
-def quote(string, safe='/', encoding=None, errors=None):
+
+def quote(string, safe="/", encoding=None, errors=None):
     """quote('abc def') -> 'abc%20def'
 
     Each part of a URL, e.g. the path info, the query, etc., has a
     different set of reserved characters that must be quoted. The
     quote function offers a cautious (not minimal) way to quote a
     string for most of these parts.
 
@@ -825,66 +998,71 @@
     By default, encoding='utf-8' (characters are encoded with UTF-8), and
     errors='strict' (unsupported characters raise a UnicodeEncodeError).
     """
     if isinstance(string, str):
         if not string:
             return string
         if encoding is None:
-            encoding = 'utf-8'
+            encoding = "utf-8"
         if errors is None:
-            errors = 'strict'
+            errors = "strict"
         string = string.encode(encoding, errors)
     else:
         if encoding is not None:
             raise TypeError("quote() doesn't support 'encoding' for bytes")
         if errors is not None:
             raise TypeError("quote() doesn't support 'errors' for bytes")
     return quote_from_bytes(string, safe)
 
-def quote_plus(string, safe='', encoding=None, errors=None):
+
+def quote_plus(string, safe="", encoding=None, errors=None):
     """Like quote(), but also replace ' ' with '+', as required for quoting
     HTML form values. Plus signs in the original string are escaped unless
     they are included in safe. It also does not have safe default to '/'.
     """
     # Check if ' ' in string, where string may either be a str or bytes.  If
     # there are no spaces, the regular quote will produce the right answer.
-    if ((isinstance(string, str) and ' ' not in string) or
-        (isinstance(string, bytes) and b' ' not in string)):
+    if (isinstance(string, str) and " " not in string) or (
+        isinstance(string, bytes) and b" " not in string
+    ):
         return quote(string, safe, encoding, errors)
     if isinstance(safe, str):
-        space = ' '
+        space = " "
     else:
-        space = b' '
+        space = b" "
     string = quote(string, safe + space, encoding, errors)
-    return string.replace(' ', '+')
+    return string.replace(" ", "+")
 
-def quote_from_bytes(bs, safe='/'):
+
+def quote_from_bytes(bs, safe="/"):
     """Like quote(), but accepts a bytes object rather than a str, and does
     not perform string-to-bytes encoding.  It always returns an ASCII string.
     quote_from_bytes(b'abc def\x3f') -> 'abc%20def%3f'
     """
     if not isinstance(bs, (bytes, bytearray)):
         raise TypeError("quote_from_bytes() expected bytes")
     if not bs:
-        return ''
+        return ""
     if isinstance(safe, str):
         # Normalize 'safe' by converting to bytes and removing non-ASCII chars
-        safe = safe.encode('ascii', 'ignore')
+        safe = safe.encode("ascii", "ignore")
     else:
         safe = bytes([c for c in safe if c < 128])
     if not bs.rstrip(_ALWAYS_SAFE_BYTES + safe):
         return bs.decode()
     try:
         quoter = _safe_quoters[safe]
     except KeyError:
         _safe_quoters[safe] = quoter = Quoter(safe).__getitem__
-    return ''.join([quoter(char) for char in bs])
+    return "".join([quoter(char) for char in bs])
+
 
-def urlencode(query, doseq=False, safe='', encoding=None, errors=None,
-              quote_via=quote_plus):
+def urlencode(
+    query, doseq=False, safe="", encoding=None, errors=None, quote_via=quote_plus
+):
     """Encode a dict or sequence of two-element tuples into a URL query string.
 
     If any values in the query arg are sequences and doseq is true, each
     sequence element is converted to a separate parameter.
 
     If the query arg is a sequence of two-element tuples, the order of the
     parameters in the output will match the order of parameters in the
@@ -908,260 +1086,299 @@
                 raise TypeError
             # Zero-length sequences of all types will get here and succeed,
             # but that's a minor nit.  Since the original implementation
             # allowed empty dicts that type of behavior probably should be
             # preserved for consistency
         except TypeError:
             ty, va, tb = sys.exc_info()
-            raise TypeError("not a valid non-string sequence "
-                            "or mapping object").with_traceback(tb)
+            raise TypeError(
+                "not a valid non-string sequence " "or mapping object"
+            ).with_traceback(tb)
 
     l = []
     if not doseq:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
             else:
                 v = quote_via(str(v), safe, encoding, errors)
-            l.append(k + '=' + v)
+            l.append(k + "=" + v)
     else:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             elif isinstance(v, str):
                 v = quote_via(v, safe, encoding, errors)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             else:
                 try:
                     # Is this a sufficient test for sequence-ness?
                     x = len(v)
                 except TypeError:
                     # not a sequence
                     v = quote_via(str(v), safe, encoding, errors)
-                    l.append(k + '=' + v)
+                    l.append(k + "=" + v)
                 else:
                     # loop over the sequence
                     for elt in v:
                         if isinstance(elt, bytes):
                             elt = quote_via(elt, safe)
                         else:
                             elt = quote_via(str(elt), safe, encoding, errors)
-                        l.append(k + '=' + elt)
-    return '&'.join(l)
+                        l.append(k + "=" + elt)
+    return "&".join(l)
 
 
 def to_bytes(url):
-    warnings.warn("urllib.parse.to_bytes() is deprecated as of 3.8",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.to_bytes() is deprecated as of 3.8",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _to_bytes(url)
 
 
 def _to_bytes(url):
     """to_bytes(u"URL") --> 'URL'."""
     # Most URL schemes require ASCII. If that changes, the conversion
     # can be relaxed.
     # XXX get rid of to_bytes()
     if isinstance(url, str):
         try:
             url = url.encode("ASCII").decode()
         except UnicodeError:
-            raise UnicodeError("URL " + repr(url) +
-                               " contains non-ASCII characters")
+            raise UnicodeError("URL " + repr(url) + " contains non-ASCII characters")
     return url
 
 
 def unwrap(url):
     """Transform a string like '<URL:scheme://host/path>' into 'scheme://host/path'.
 
     The string is returned unchanged if it's not a wrapped URL.
     """
     url = str(url).strip()
-    if url[:1] == '<' and url[-1:] == '>':
+    if url[:1] == "<" and url[-1:] == ">":
         url = url[1:-1].strip()
-    if url[:4] == 'URL:':
+    if url[:4] == "URL:":
         url = url[4:].strip()
     return url
 
 
 def splittype(url):
-    warnings.warn("urllib.parse.splittype() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splittype() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splittype(url)
 
 
 _typeprog = None
+
+
 def _splittype(url):
     """splittype('type:opaquestring') --> 'type', 'opaquestring'."""
     global _typeprog
     if _typeprog is None:
-        _typeprog = re.compile('([^/:]+):(.*)', re.DOTALL)
+        _typeprog = re.compile("([^/:]+):(.*)", re.DOTALL)
 
     match = _typeprog.match(url)
     if match:
         scheme, data = match.groups()
         return scheme.lower(), data
     return None, url
 
 
 def splithost(url):
-    warnings.warn("urllib.parse.splithost() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splithost() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splithost(url)
 
 
 _hostprog = None
+
+
 def _splithost(url):
     """splithost('//host[:port]/path') --> 'host[:port]', '/path'."""
     global _hostprog
     if _hostprog is None:
-        _hostprog = re.compile('//([^/#?]*)(.*)', re.DOTALL)
+        _hostprog = re.compile("//([^/#?]*)(.*)", re.DOTALL)
 
     match = _hostprog.match(url)
     if match:
         host_port, path = match.groups()
-        if path and path[0] != '/':
-            path = '/' + path
+        if path and path[0] != "/":
+            path = "/" + path
         return host_port, path
     return None, url
 
 
 def splituser(host):
-    warnings.warn("urllib.parse.splituser() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splituser() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splituser(host)
 
 
 def _splituser(host):
     """splituser('user[:passwd]@host[:port]') --> 'user[:passwd]', 'host[:port]'."""
-    user, delim, host = host.rpartition('@')
+    user, delim, host = host.rpartition("@")
     return (user if delim else None), host
 
 
 def splitpasswd(user):
-    warnings.warn("urllib.parse.splitpasswd() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitpasswd() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitpasswd(user)
 
 
 def _splitpasswd(user):
     """splitpasswd('user:passwd') -> 'user', 'passwd'."""
-    user, delim, passwd = user.partition(':')
+    user, delim, passwd = user.partition(":")
     return user, (passwd if delim else None)
 
 
 def splitport(host):
-    warnings.warn("urllib.parse.splitport() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitport(host)
 
 
 # splittag('/path#tag') --> '/path', 'tag'
 _portprog = None
+
+
 def _splitport(host):
     """splitport('host:port') --> 'host', 'port'."""
     global _portprog
     if _portprog is None:
-        _portprog = re.compile('(.*):([0-9]*)', re.DOTALL)
+        _portprog = re.compile("(.*):([0-9]*)", re.DOTALL)
 
     match = _portprog.fullmatch(host)
     if match:
         host, port = match.groups()
         if port:
             return host, port
     return host, None
 
 
 def splitnport(host, defport=-1):
-    warnings.warn("urllib.parse.splitnport() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitnport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitnport(host, defport)
 
 
 def _splitnport(host, defport=-1):
     """Split host and port, returning numeric port.
     Return given default port if no ':' found; defaults to -1.
     Return numerical port if a valid number are found after ':'.
     Return None if ':' but not a valid number."""
-    host, delim, port = host.rpartition(':')
+    host, delim, port = host.rpartition(":")
     if not delim:
         host = port
     elif port:
         try:
             nport = int(port)
         except ValueError:
             nport = None
         return host, nport
     return host, defport
 
 
 def splitquery(url):
-    warnings.warn("urllib.parse.splitquery() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitquery() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitquery(url)
 
 
 def _splitquery(url):
     """splitquery('/path?query') --> '/path', 'query'."""
-    path, delim, query = url.rpartition('?')
+    path, delim, query = url.rpartition("?")
     if delim:
         return path, query
     return url, None
 
 
 def splittag(url):
-    warnings.warn("urllib.parse.splittag() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splittag() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splittag(url)
 
 
 def _splittag(url):
     """splittag('/path#tag') --> '/path', 'tag'."""
-    path, delim, tag = url.rpartition('#')
+    path, delim, tag = url.rpartition("#")
     if delim:
         return path, tag
     return url, None
 
 
 def splitattr(url):
-    warnings.warn("urllib.parse.splitattr() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitattr() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitattr(url)
 
 
 def _splitattr(url):
     """splitattr('/path;attr1=value1;attr2=value2;...') ->
-        '/path', ['attr1=value1', 'attr2=value2', ...]."""
-    words = url.split(';')
+    '/path', ['attr1=value1', 'attr2=value2', ...]."""
+    words = url.split(";")
     return words[0], words[1:]
 
 
 def splitvalue(attr):
-    warnings.warn("urllib.parse.splitvalue() is deprecated as of 3.8, "
-                  "use urllib.parse.parse_qsl() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitvalue() is deprecated as of 3.8, "
+        "use urllib.parse.parse_qsl() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitvalue(attr)
 
 
 def _splitvalue(attr):
     """splitvalue('attr=value') --> 'attr', 'value'."""
-    attr, delim, value = attr.partition('=')
+    attr, delim, value = attr.partition("=")
     return attr, (value if delim else None)
```

### Comparing `ignition-gemini-0.1.8/ignition/python/python3_9/Lib/urllib/parse.py` & `ignition_gemini-0.2.0/ignition/python/python3_11/Lib/urllib/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,94 +23,203 @@
 urlparse module should conform with it.  The urlparse module is
 currently not entirely compliant with this RFC due to defacto
 scenarios for parsing, and for backward compatibility purposes, some
 parsing quirks from older RFCs are retained. The testcases in
 test_urlparse.py provides a good indicator of parsing behavior.
 """
 
+import functools
 import re
 import sys
 import types
-import collections
 import warnings
+from collections import namedtuple
 
-__all__ = ["urlparse", "urlunparse", "urljoin", "urldefrag",
-           "urlsplit", "urlunsplit", "urlencode", "parse_qs",
-           "parse_qsl", "quote", "quote_plus", "quote_from_bytes",
-           "unquote", "unquote_plus", "unquote_to_bytes",
-           "DefragResult", "ParseResult", "SplitResult",
-           "DefragResultBytes", "ParseResultBytes", "SplitResultBytes"]
+__all__ = [
+    "urlparse",
+    "urlunparse",
+    "urljoin",
+    "urldefrag",
+    "urlsplit",
+    "urlunsplit",
+    "urlencode",
+    "parse_qs",
+    "parse_qsl",
+    "quote",
+    "quote_plus",
+    "quote_from_bytes",
+    "unquote",
+    "unquote_plus",
+    "unquote_to_bytes",
+    "DefragResult",
+    "ParseResult",
+    "SplitResult",
+    "DefragResultBytes",
+    "ParseResultBytes",
+    "SplitResultBytes",
+]
 
 # A classification of schemes.
 # The empty string classifies URLs with no scheme specified,
 # being the default value returned by “urlsplit” and “urlparse”.
 
-uses_relative = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'imap', # PATCH added gemini
-                 'wais', 'file', 'https', 'shttp', 'mms',
-                 'prospero', 'rtsp', 'rtspu', 'sftp',
-                 'svn', 'svn+ssh', 'ws', 'wss']
-
-uses_netloc = ['', 'ftp', 'http', 'gemini', 'gopher', 'nntp', 'telnet', # PATCH added gemini
-               'imap', 'wais', 'file', 'mms', 'https', 'shttp',
-               'snews', 'prospero', 'rtsp', 'rtspu', 'rsync',
-               'svn', 'svn+ssh', 'sftp', 'nfs', 'git', 'git+ssh',
-               'ws', 'wss']
-
-uses_params = ['', 'ftp', 'gemini', 'hdl', 'prospero', 'http', 'imap', # PATCH added gemini
-               'https', 'shttp', 'rtsp', 'rtspu', 'sip', 'sips',
-               'mms', 'sftp', 'tel']
+uses_relative = [
+    "",
+    "ftp",
+    "http",
+    "gemini",
+    "gopher",
+    "nntp",
+    "imap",  # PATCH added gemini
+    "wais",
+    "file",
+    "https",
+    "shttp",
+    "mms",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "sftp",
+    "svn",
+    "svn+ssh",
+    "ws",
+    "wss",
+]
+
+uses_netloc = [
+    "",
+    "ftp",
+    "http",
+    "gemini",
+    "gopher",
+    "nntp",
+    "telnet",  # PATCH added gemini
+    "imap",
+    "wais",
+    "file",
+    "mms",
+    "https",
+    "shttp",
+    "snews",
+    "prospero",
+    "rtsp",
+    "rtspu",
+    "rsync",
+    "svn",
+    "svn+ssh",
+    "sftp",
+    "nfs",
+    "git",
+    "git+ssh",
+    "ws",
+    "wss",
+]
+
+uses_params = [
+    "",
+    "ftp",
+    "gemini",
+    "hdl",
+    "prospero",
+    "http",
+    "imap",  # PATCH added gemini
+    "https",
+    "shttp",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+    "mms",
+    "sftp",
+    "tel",
+]
 
 # These are not actually used anymore, but should stay for backwards
 # compatibility.  (They are undocumented, but have a public-looking name.)
 
-non_hierarchical = ['gopher', 'hdl', 'mailto', 'news',
-                    'telnet', 'wais', 'imap', 'snews', 'sip', 'sips']
+non_hierarchical = [
+    "gopher",
+    "hdl",
+    "mailto",
+    "news",
+    "telnet",
+    "wais",
+    "imap",
+    "snews",
+    "sip",
+    "sips",
+]
+
+uses_query = [
+    "",
+    "http",
+    "wais",
+    "imap",
+    "https",
+    "shttp",
+    "mms",
+    "gopher",
+    "rtsp",
+    "rtspu",
+    "sip",
+    "sips",
+]
+
+uses_fragment = [
+    "",
+    "ftp",
+    "hdl",
+    "http",
+    "gopher",
+    "news",
+    "nntp",
+    "wais",
+    "https",
+    "shttp",
+    "snews",
+    "file",
+    "prospero",
+]
 
-uses_query = ['', 'http', 'wais', 'imap', 'https', 'shttp', 'mms',
-              'gopher', 'rtsp', 'rtspu', 'sip', 'sips']
+# Characters valid in scheme names
+scheme_chars = (
+    "abcdefghijklmnopqrstuvwxyz" "ABCDEFGHIJKLMNOPQRSTUVWXYZ" "0123456789" "+-."
+)
 
-uses_fragment = ['', 'ftp', 'hdl', 'http', 'gopher', 'news',
-                 'nntp', 'wais', 'https', 'shttp', 'snews',
-                 'file', 'prospero']
+# Unsafe bytes to be removed per WHATWG spec
+_UNSAFE_URL_BYTES_TO_REMOVE = ["\t", "\r", "\n"]
 
-# Characters valid in scheme names
-scheme_chars = ('abcdefghijklmnopqrstuvwxyz'
-                'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                '0123456789'
-                '+-.')
-
-# XXX: Consider replacing with functools.lru_cache
-MAX_CACHE_SIZE = 20
-_parse_cache = {}
 
 def clear_cache():
-    """Clear the parse cache and the quoters cache."""
-    _parse_cache.clear()
-    _safe_quoters.clear()
+    """Clear internal performance caches. Undocumented; some tests want it."""
+    urlsplit.cache_clear()
+    _byte_quoter_factory.cache_clear()
 
 
 # Helpers for bytes handling
 # For 3.2, we deliberately require applications that
 # handle improperly quoted URLs to do their own
 # decoding and encoding. If valid use cases are
 # presented, we may relax this by using latin-1
 # decoding internally for 3.3
-_implicit_encoding = 'ascii'
-_implicit_errors = 'strict'
+_implicit_encoding = "ascii"
+_implicit_errors = "strict"
+
 
 def _noop(obj):
     return obj
 
-def _encode_result(obj, encoding=_implicit_encoding,
-                        errors=_implicit_errors):
+
+def _encode_result(obj, encoding=_implicit_encoding, errors=_implicit_errors):
     return obj.encode(encoding, errors)
 
-def _decode_args(args, encoding=_implicit_encoding,
-                       errors=_implicit_errors):
-    return tuple(x.decode(encoding, errors) if x else '' for x in args)
+
+def _decode_args(args, encoding=_implicit_encoding, errors=_implicit_errors):
+    return tuple(x.decode(encoding, errors) if x else "" for x in args)
+
 
 def _coerce_args(*args):
     # Invokes decode if necessary to create str args
     # and returns the coerced inputs along with
     # an appropriate result coercion function
     #   - noop for str inputs
     #   - encoding function otherwise
@@ -120,33 +229,37 @@
         # "scheme=''" default argument to some functions
         if arg and isinstance(arg, str) != str_input:
             raise TypeError("Cannot mix str and non-str arguments")
     if str_input:
         return args + (_noop,)
     return _decode_args(args) + (_encode_result,)
 
+
 # Result objects are more helpful than simple tuples
 class _ResultMixinStr(object):
     """Standard approach to encoding parsed results from str to bytes"""
+
     __slots__ = ()
 
-    def encode(self, encoding='ascii', errors='strict'):
+    def encode(self, encoding="ascii", errors="strict"):
         return self._encoded_counterpart(*(x.encode(encoding, errors) for x in self))
 
 
 class _ResultMixinBytes(object):
     """Standard approach to decoding parsed results from bytes to str"""
+
     __slots__ = ()
 
-    def decode(self, encoding='ascii', errors='strict'):
+    def decode(self, encoding="ascii", errors="strict"):
         return self._decoded_counterpart(*(x.decode(encoding, errors) for x in self))
 
 
 class _NetlocResultMixinBase(object):
     """Shared methods for the parsed result objects containing a netloc element"""
+
     __slots__ = ()
 
     @property
     def username(self):
         return self._userinfo[0]
 
     @property
@@ -156,101 +269,97 @@
     @property
     def hostname(self):
         hostname = self._hostinfo[0]
         if not hostname:
             return None
         # Scoped IPv6 address may have zone info, which must not be lowercased
         # like http://[fe80::822a:a8ff:fe49:470c%tESt]:1234/keys
-        separator = '%' if isinstance(hostname, str) else b'%'
+        separator = "%" if isinstance(hostname, str) else b"%"
         hostname, percent, zone = hostname.partition(separator)
         return hostname.lower() + percent + zone
 
     @property
     def port(self):
         port = self._hostinfo[1]
         if port is not None:
             try:
                 port = int(port, 10)
             except ValueError:
-                message = f'Port could not be cast to integer value as {port!r}'
+                message = f"Port could not be cast to integer value as {port!r}"
                 raise ValueError(message) from None
-            if not ( 0 <= port <= 65535):
+            if not (0 <= port <= 65535):
                 raise ValueError("Port out of range 0-65535")
         return port
 
     __class_getitem__ = classmethod(types.GenericAlias)
 
 
 class _NetlocResultMixinStr(_NetlocResultMixinBase, _ResultMixinStr):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition('@')
+        userinfo, have_info, hostinfo = netloc.rpartition("@")
         if have_info:
-            username, have_password, password = userinfo.partition(':')
+            username, have_password, password = userinfo.partition(":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition('@')
-        _, have_open_br, bracketed = hostinfo.partition('[')
+        _, _, hostinfo = netloc.rpartition("@")
+        _, have_open_br, bracketed = hostinfo.partition("[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(']')
-            _, _, port = port.partition(':')
+            hostname, _, port = bracketed.partition("]")
+            _, _, port = port.partition(":")
         else:
-            hostname, _, port = hostinfo.partition(':')
+            hostname, _, port = hostinfo.partition(":")
         if not port:
             port = None
         return hostname, port
 
 
 class _NetlocResultMixinBytes(_NetlocResultMixinBase, _ResultMixinBytes):
     __slots__ = ()
 
     @property
     def _userinfo(self):
         netloc = self.netloc
-        userinfo, have_info, hostinfo = netloc.rpartition(b'@')
+        userinfo, have_info, hostinfo = netloc.rpartition(b"@")
         if have_info:
-            username, have_password, password = userinfo.partition(b':')
+            username, have_password, password = userinfo.partition(b":")
             if not have_password:
                 password = None
         else:
             username = password = None
         return username, password
 
     @property
     def _hostinfo(self):
         netloc = self.netloc
-        _, _, hostinfo = netloc.rpartition(b'@')
-        _, have_open_br, bracketed = hostinfo.partition(b'[')
+        _, _, hostinfo = netloc.rpartition(b"@")
+        _, have_open_br, bracketed = hostinfo.partition(b"[")
         if have_open_br:
-            hostname, _, port = bracketed.partition(b']')
-            _, _, port = port.partition(b':')
+            hostname, _, port = bracketed.partition(b"]")
+            _, _, port = port.partition(b":")
         else:
-            hostname, _, port = hostinfo.partition(b':')
+            hostname, _, port = hostinfo.partition(b":")
         if not port:
             port = None
         return hostname, port
 
 
-from collections import namedtuple
-
-_DefragResultBase = namedtuple('DefragResult', 'url fragment')
-_SplitResultBase = namedtuple(
-    'SplitResult', 'scheme netloc path query fragment')
-_ParseResultBase = namedtuple(
-    'ParseResult', 'scheme netloc path params query fragment')
+_DefragResultBase = namedtuple("DefragResult", "url fragment")
+_SplitResultBase = namedtuple("SplitResult", "scheme netloc path query fragment")
+_ParseResultBase = namedtuple("ParseResult", "scheme netloc path params query fragment")
 
 _DefragResultBase.__doc__ = """
 DefragResult(url, fragment)
 
 A 2-tuple that contains the url without fragment identifier and the fragment
 identifier as a separate argument.
 """
@@ -304,73 +413,87 @@
 Parameters for last path element used to dereference the URI in order to provide
 access to perform some operation on the resource.
 """
 
 _ParseResultBase.query.__doc__ = _SplitResultBase.query.__doc__
 _ParseResultBase.fragment.__doc__ = _SplitResultBase.fragment.__doc__
 
-
 # For backwards compatibility, alias _NetlocResultMixinStr
 # ResultBase is no longer part of the documented API, but it is
 # retained since deprecating it isn't worth the hassle
 ResultBase = _NetlocResultMixinStr
 
+
 # Structured result objects for string data
 class DefragResult(_DefragResultBase, _ResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + '#' + self.fragment
+            return self.url + "#" + self.fragment
         else:
             return self.url
 
+
 class SplitResult(_SplitResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResult(_ParseResultBase, _NetlocResultMixinStr):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Structured result objects for bytes data
 class DefragResultBytes(_DefragResultBase, _ResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         if self.fragment:
-            return self.url + b'#' + self.fragment
+            return self.url + b"#" + self.fragment
         else:
             return self.url
 
+
 class SplitResultBytes(_SplitResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunsplit(self)
 
+
 class ParseResultBytes(_ParseResultBase, _NetlocResultMixinBytes):
     __slots__ = ()
+
     def geturl(self):
         return urlunparse(self)
 
+
 # Set up the encode/decode result pairs
 def _fix_result_transcoding():
     _result_pairs = (
         (DefragResult, DefragResultBytes),
         (SplitResult, SplitResultBytes),
         (ParseResult, ParseResultBytes),
     )
     for _decoded, _encoded in _result_pairs:
         _decoded._encoded_counterpart = _encoded
         _encoded._decoded_counterpart = _decoded
 
+
 _fix_result_transcoding()
 del _fix_result_transcoding
 
-def urlparse(url, scheme='', allow_fragments=True):
+
+def urlparse(url, scheme="", allow_fragments=True):
     """Parse a URL into 6 components:
     <scheme>://<netloc>/<path>;<params>?<query>#<fragment>
 
     The result is a named 6-tuple with fields corresponding to the
     above. It is either a ParseResult or ParseResultBytes object,
     depending on the type of the url parameter.
 
@@ -385,57 +508,69 @@
     path or query.
 
     Note that % escapes are not expanded.
     """
     url, scheme, _coerce_result = _coerce_args(url, scheme)
     splitresult = urlsplit(url, scheme, allow_fragments)
     scheme, netloc, url, query, fragment = splitresult
-    if scheme in uses_params and ';' in url:
+    if scheme in uses_params and ";" in url:
         url, params = _splitparams(url)
     else:
-        params = ''
+        params = ""
     result = ParseResult(scheme, netloc, url, params, query, fragment)
     return _coerce_result(result)
 
+
 def _splitparams(url):
-    if '/'  in url:
-        i = url.find(';', url.rfind('/'))
+    if "/" in url:
+        i = url.find(";", url.rfind("/"))
         if i < 0:
-            return url, ''
+            return url, ""
     else:
-        i = url.find(';')
-    return url[:i], url[i+1:]
+        i = url.find(";")
+    return url[:i], url[i + 1 :]
+
 
 def _splitnetloc(url, start=0):
-    delim = len(url)   # position of end of domain part of url, default is end
-    for c in '/?#':    # look for delimiters; the order is NOT important
-        wdelim = url.find(c, start)        # find first of this delim
-        if wdelim >= 0:                    # if found
-            delim = min(delim, wdelim)     # use earliest delim position
-    return url[start:delim], url[delim:]   # return (domain, rest)
+    delim = len(url)  # position of end of domain part of url, default is end
+    for c in "/?#":  # look for delimiters; the order is NOT important
+        wdelim = url.find(c, start)  # find first of this delim
+        if wdelim >= 0:  # if found
+            delim = min(delim, wdelim)  # use earliest delim position
+    return url[start:delim], url[delim:]  # return (domain, rest)
+
 
 def _checknetloc(netloc):
     if not netloc or netloc.isascii():
         return
     # looking for characters like \u2100 that expand to 'a/c'
     # IDNA uses NFKC equivalence, so normalize for this check
     import unicodedata
-    n = netloc.replace('@', '')   # ignore characters already included
-    n = n.replace(':', '')        # but not the surrounding text
-    n = n.replace('#', '')
-    n = n.replace('?', '')
-    netloc2 = unicodedata.normalize('NFKC', n)
+
+    n = netloc.replace("@", "")  # ignore characters already included
+    n = n.replace(":", "")  # but not the surrounding text
+    n = n.replace("#", "")
+    n = n.replace("?", "")
+    netloc2 = unicodedata.normalize("NFKC", n)
     if n == netloc2:
         return
-    for c in '/?#@:':
+    for c in "/?#@:":
         if c in netloc2:
-            raise ValueError("netloc '" + netloc + "' contains invalid " +
-                             "characters under NFKC normalization")
+            raise ValueError(
+                "netloc '"
+                + netloc
+                + "' contains invalid "
+                + "characters under NFKC normalization"
+            )
 
-def urlsplit(url, scheme='', allow_fragments=True):
+
+# typed=True avoids BytesWarnings being emitted during cache key
+# comparison since this API supports both bytes and str input.
+@functools.lru_cache(typed=True)
+def urlsplit(url, scheme="", allow_fragments=True):
     """Parse a URL into 5 components:
     <scheme>://<netloc>/<path>?<query>#<fragment>
 
     The result is a named 5-tuple with fields corresponding to the
     above. It is either a SplitResult or SplitResultBytes object,
     depending on the type of the url parameter.
 
@@ -449,360 +584,420 @@
     fragment component from the previous component, which can be either
     path or query.
 
     Note that % escapes are not expanded.
     """
 
     url, scheme, _coerce_result = _coerce_args(url, scheme)
+
+    for b in _UNSAFE_URL_BYTES_TO_REMOVE:
+        url = url.replace(b, "")
+        scheme = scheme.replace(b, "")
+
     allow_fragments = bool(allow_fragments)
-    key = url, scheme, allow_fragments, type(url), type(scheme)
-    cached = _parse_cache.get(key, None)
-    if cached:
-        return _coerce_result(cached)
-    if len(_parse_cache) >= MAX_CACHE_SIZE: # avoid runaway growth
-        clear_cache()
-    netloc = query = fragment = ''
-    i = url.find(':')
+    netloc = query = fragment = ""
+    i = url.find(":")
     if i > 0:
         for c in url[:i]:
             if c not in scheme_chars:
                 break
         else:
-            scheme, url = url[:i].lower(), url[i+1:]
+            scheme, url = url[:i].lower(), url[i + 1 :]
 
-    if url[:2] == '//':
+    if url[:2] == "//":
         netloc, url = _splitnetloc(url, 2)
-        if (('[' in netloc and ']' not in netloc) or
-                (']' in netloc and '[' not in netloc)):
+        if ("[" in netloc and "]" not in netloc) or (
+            "]" in netloc and "[" not in netloc
+        ):
             raise ValueError("Invalid IPv6 URL")
-    if allow_fragments and '#' in url:
-        url, fragment = url.split('#', 1)
-    if '?' in url:
-        url, query = url.split('?', 1)
+    if allow_fragments and "#" in url:
+        url, fragment = url.split("#", 1)
+    if "?" in url:
+        url, query = url.split("?", 1)
     _checknetloc(netloc)
     v = SplitResult(scheme, netloc, url, query, fragment)
-    _parse_cache[key] = v
     return _coerce_result(v)
 
+
 def urlunparse(components):
     """Put a parsed URL back together again.  This may result in a
     slightly different, but equivalent URL, if the URL that was parsed
     originally had redundant delimiters, e.g. a ? with an empty query
     (the draft states that these are equivalent)."""
-    scheme, netloc, url, params, query, fragment, _coerce_result = (
-                                                  _coerce_args(*components))
+    scheme, netloc, url, params, query, fragment, _coerce_result = _coerce_args(
+        *components
+    )
     if params:
         url = "%s;%s" % (url, params)
     return _coerce_result(urlunsplit((scheme, netloc, url, query, fragment)))
 
+
 def urlunsplit(components):
     """Combine the elements of a tuple as returned by urlsplit() into a
     complete URL as a string. The data argument can be any five-item iterable.
     This may result in a slightly different, but equivalent URL, if the URL that
     was parsed originally had unnecessary delimiters (for example, a ? with an
     empty query; the RFC states that these are equivalent)."""
-    scheme, netloc, url, query, fragment, _coerce_result = (
-                                          _coerce_args(*components))
-    if netloc or (scheme and scheme in uses_netloc and url[:2] != '//'):
-        if url and url[:1] != '/': url = '/' + url
-        url = '//' + (netloc or '') + url
+    scheme, netloc, url, query, fragment, _coerce_result = _coerce_args(*components)
+    if netloc or (scheme and scheme in uses_netloc and url[:2] != "//"):
+        if url and url[:1] != "/":
+            url = "/" + url
+        url = "//" + (netloc or "") + url
     if scheme:
-        url = scheme + ':' + url
+        url = scheme + ":" + url
     if query:
-        url = url + '?' + query
+        url = url + "?" + query
     if fragment:
-        url = url + '#' + fragment
+        url = url + "#" + fragment
     return _coerce_result(url)
 
+
 def urljoin(base, url, allow_fragments=True):
     """Join a base URL and a possibly relative URL to form an absolute
     interpretation of the latter."""
     if not base:
         return url
     if not url:
         return base
 
     base, url, _coerce_result = _coerce_args(base, url)
-    bscheme, bnetloc, bpath, bparams, bquery, bfragment = \
-            urlparse(base, '', allow_fragments)
-    scheme, netloc, path, params, query, fragment = \
-            urlparse(url, bscheme, allow_fragments)
+    bscheme, bnetloc, bpath, bparams, bquery, bfragment = urlparse(
+        base, "", allow_fragments
+    )
+    scheme, netloc, path, params, query, fragment = urlparse(
+        url, bscheme, allow_fragments
+    )
 
     if scheme != bscheme or scheme not in uses_relative:
         return _coerce_result(url)
     if scheme in uses_netloc:
         if netloc:
-            return _coerce_result(urlunparse((scheme, netloc, path,
-                                              params, query, fragment)))
+            return _coerce_result(
+                urlunparse((scheme, netloc, path, params, query, fragment))
+            )
         netloc = bnetloc
 
     if not path and not params:
         path = bpath
         params = bparams
         if not query:
             query = bquery
-        return _coerce_result(urlunparse((scheme, netloc, path,
-                                          params, query, fragment)))
+        return _coerce_result(
+            urlunparse((scheme, netloc, path, params, query, fragment))
+        )
 
-    base_parts = bpath.split('/')
-    if base_parts[-1] != '':
+    base_parts = bpath.split("/")
+    if base_parts[-1] != "":
         # the last item is not a directory, so will not be taken into account
         # in resolving the relative path
         del base_parts[-1]
 
     # for rfc3986, ignore all base path should the first character be root.
-    if path[:1] == '/':
-        segments = path.split('/')
+    if path[:1] == "/":
+        segments = path.split("/")
     else:
-        segments = base_parts + path.split('/')
+        segments = base_parts + path.split("/")
         # filter out elements that would cause redundant slashes on re-joining
         # the resolved_path
         segments[1:-1] = filter(None, segments[1:-1])
 
     resolved_path = []
 
     for seg in segments:
-        if seg == '..':
+        if seg == "..":
             try:
                 resolved_path.pop()
             except IndexError:
                 # ignore any .. segments that would otherwise cause an IndexError
                 # when popped from resolved_path if resolving for rfc3986
                 pass
-        elif seg == '.':
+        elif seg == ".":
             continue
         else:
             resolved_path.append(seg)
 
-    if segments[-1] in ('.', '..'):
+    if segments[-1] in (".", ".."):
         # do some post-processing here. if the last segment was a relative dir,
         # then we need to append the trailing '/'
-        resolved_path.append('')
+        resolved_path.append("")
 
-    return _coerce_result(urlunparse((scheme, netloc, '/'.join(
-        resolved_path) or '/', params, query, fragment)))
+    return _coerce_result(
+        urlunparse(
+            (scheme, netloc, "/".join(resolved_path) or "/", params, query, fragment)
+        )
+    )
 
 
 def urldefrag(url):
     """Removes any existing fragment from URL.
 
     Returns a tuple of the defragmented URL and the fragment.  If
     the URL contained no fragments, the second element is the
     empty string.
     """
     url, _coerce_result = _coerce_args(url)
-    if '#' in url:
+    if "#" in url:
         s, n, p, a, q, frag = urlparse(url)
-        defrag = urlunparse((s, n, p, a, q, ''))
+        defrag = urlunparse((s, n, p, a, q, ""))
     else:
-        frag = ''
+        frag = ""
         defrag = url
     return _coerce_result(DefragResult(defrag, frag))
 
-_hexdig = '0123456789ABCDEFabcdef'
+
+_hexdig = "0123456789ABCDEFabcdef"
 _hextobyte = None
 
+
 def unquote_to_bytes(string):
     """unquote_to_bytes('abc%20def') -> b'abc def'."""
     # Note: strings are encoded as UTF-8. This is only an issue if it contains
     # unescaped non-ASCII characters, which URIs should not.
     if not string:
         # Is it a string-like object?
         string.split
-        return b''
+        return b""
     if isinstance(string, str):
-        string = string.encode('utf-8')
-    bits = string.split(b'%')
+        string = string.encode("utf-8")
+    bits = string.split(b"%")
     if len(bits) == 1:
         return string
     res = [bits[0]]
     append = res.append
     # Delay the initialization of the table to not waste memory
     # if the function is never called
     global _hextobyte
     if _hextobyte is None:
-        _hextobyte = {(a + b).encode(): bytes.fromhex(a + b)
-                      for a in _hexdig for b in _hexdig}
+        _hextobyte = {
+            (a + b).encode(): bytes.fromhex(a + b) for a in _hexdig for b in _hexdig
+        }
     for item in bits[1:]:
         try:
             append(_hextobyte[item[:2]])
             append(item[2:])
         except KeyError:
-            append(b'%')
+            append(b"%")
             append(item)
-    return b''.join(res)
+    return b"".join(res)
 
-_asciire = re.compile('([\x00-\x7f]+)')
 
-def unquote(string, encoding='utf-8', errors='replace'):
+_asciire = re.compile("([\x00-\x7f]+)")
+
+
+def unquote(string, encoding="utf-8", errors="replace"):
     """Replace %xx escapes by their single-character equivalent. The optional
     encoding and errors parameters specify how to decode percent-encoded
     sequences into Unicode characters, as accepted by the bytes.decode()
     method.
     By default, percent-encoded sequences are decoded with UTF-8, and invalid
     sequences are replaced by a placeholder character.
 
     unquote('abc%20def') -> 'abc def'.
     """
     if isinstance(string, bytes):
         return unquote_to_bytes(string).decode(encoding, errors)
-    if '%' not in string:
+    if "%" not in string:
         string.split
         return string
     if encoding is None:
-        encoding = 'utf-8'
+        encoding = "utf-8"
     if errors is None:
-        errors = 'replace'
+        errors = "replace"
     bits = _asciire.split(string)
     res = [bits[0]]
     append = res.append
     for i in range(1, len(bits), 2):
         append(unquote_to_bytes(bits[i]).decode(encoding, errors))
         append(bits[i + 1])
-    return ''.join(res)
+    return "".join(res)
 
 
-def parse_qs(qs, keep_blank_values=False, strict_parsing=False,
-             encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qs(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+    separator="&",
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
+
+    qs: percent-encoded query string to be parsed
 
-        qs: percent-encoded query string to be parsed
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as
+        blank strings.  The default false value indicates that
+        blank values are to be ignored and treated as if they were
+        not included.
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as
-            blank strings.  The default false value indicates that
-            blank values are to be ignored and treated as if they were
-            not included.
+    strict_parsing: flag indicating what to do with parsing errors.
+        If false (the default), errors are silently ignored.
+        If true, errors raise a ValueError exception.
 
-        strict_parsing: flag indicating what to do with parsing errors.
-            If false (the default), errors are silently ignored.
-            If true, errors raise a ValueError exception.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    max_num_fields: int. If set, then throws a ValueError if there
+        are more than n fields read by parse_qsl().
 
-        max_num_fields: int. If set, then throws a ValueError if there
-            are more than n fields read by parse_qsl().
+    separator: str. The symbol to use for separating the query arguments.
+        Defaults to &.
 
-        Returns a dictionary.
+    Returns a dictionary.
     """
     parsed_result = {}
-    pairs = parse_qsl(qs, keep_blank_values, strict_parsing,
-                      encoding=encoding, errors=errors,
-                      max_num_fields=max_num_fields)
+    pairs = parse_qsl(
+        qs,
+        keep_blank_values,
+        strict_parsing,
+        encoding=encoding,
+        errors=errors,
+        max_num_fields=max_num_fields,
+        separator=separator,
+    )
     for name, value in pairs:
         if name in parsed_result:
             parsed_result[name].append(value)
         else:
             parsed_result[name] = [value]
     return parsed_result
 
 
-def parse_qsl(qs, keep_blank_values=False, strict_parsing=False,
-              encoding='utf-8', errors='replace', max_num_fields=None):
+def parse_qsl(
+    qs,
+    keep_blank_values=False,
+    strict_parsing=False,
+    encoding="utf-8",
+    errors="replace",
+    max_num_fields=None,
+    separator="&",
+):
     """Parse a query given as a string argument.
 
-        Arguments:
+    Arguments:
+
+    qs: percent-encoded query string to be parsed
 
-        qs: percent-encoded query string to be parsed
+    keep_blank_values: flag indicating whether blank values in
+        percent-encoded queries should be treated as blank strings.
+        A true value indicates that blanks should be retained as blank
+        strings.  The default false value indicates that blank values
+        are to be ignored and treated as if they were  not included.
 
-        keep_blank_values: flag indicating whether blank values in
-            percent-encoded queries should be treated as blank strings.
-            A true value indicates that blanks should be retained as blank
-            strings.  The default false value indicates that blank values
-            are to be ignored and treated as if they were  not included.
+    strict_parsing: flag indicating what to do with parsing errors. If
+        false (the default), errors are silently ignored. If true,
+        errors raise a ValueError exception.
 
-        strict_parsing: flag indicating what to do with parsing errors. If
-            false (the default), errors are silently ignored. If true,
-            errors raise a ValueError exception.
+    encoding and errors: specify how to decode percent-encoded sequences
+        into Unicode characters, as accepted by the bytes.decode() method.
 
-        encoding and errors: specify how to decode percent-encoded sequences
-            into Unicode characters, as accepted by the bytes.decode() method.
+    max_num_fields: int. If set, then throws a ValueError
+        if there are more than n fields read by parse_qsl().
 
-        max_num_fields: int. If set, then throws a ValueError
-            if there are more than n fields read by parse_qsl().
+    separator: str. The symbol to use for separating the query arguments.
+        Defaults to &.
 
-        Returns a list, as G-d intended.
+    Returns a list, as G-d intended.
     """
     qs, _coerce_result = _coerce_args(qs)
+    separator, _ = _coerce_args(separator)
+
+    if not separator or (not isinstance(separator, (str, bytes))):
+        raise ValueError("Separator must be of type string or bytes.")
 
     # If max_num_fields is defined then check that the number of fields
     # is less than max_num_fields. This prevents a memory exhaustion DOS
     # attack via post bodies with many fields.
     if max_num_fields is not None:
-        num_fields = 1 + qs.count('&') + qs.count(';')
+        num_fields = 1 + qs.count(separator) if qs else 0
         if max_num_fields < num_fields:
-            raise ValueError('Max number of fields exceeded')
+            raise ValueError("Max number of fields exceeded")
 
-    pairs = [s2 for s1 in qs.split('&') for s2 in s1.split(';')]
     r = []
-    for name_value in pairs:
+    query_args = qs.split(separator) if qs else []
+    for name_value in query_args:
         if not name_value and not strict_parsing:
             continue
-        nv = name_value.split('=', 1)
+        nv = name_value.split("=", 1)
         if len(nv) != 2:
             if strict_parsing:
                 raise ValueError("bad query field: %r" % (name_value,))
             # Handle case of a control-name with no equal sign
             if keep_blank_values:
-                nv.append('')
+                nv.append("")
             else:
                 continue
         if len(nv[1]) or keep_blank_values:
-            name = nv[0].replace('+', ' ')
+            name = nv[0].replace("+", " ")
             name = unquote(name, encoding=encoding, errors=errors)
             name = _coerce_result(name)
-            value = nv[1].replace('+', ' ')
+            value = nv[1].replace("+", " ")
             value = unquote(value, encoding=encoding, errors=errors)
             value = _coerce_result(value)
             r.append((name, value))
     return r
 
-def unquote_plus(string, encoding='utf-8', errors='replace'):
+
+def unquote_plus(string, encoding="utf-8", errors="replace"):
     """Like unquote(), but also replace plus signs by spaces, as required for
     unquoting HTML form values.
 
     unquote_plus('%7e/abc+def') -> '~/abc def'
     """
-    string = string.replace('+', ' ')
+    string = string.replace("+", " ")
     return unquote(string, encoding, errors)
 
-_ALWAYS_SAFE = frozenset(b'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                         b'abcdefghijklmnopqrstuvwxyz'
-                         b'0123456789'
-                         b'_.-~')
+
+_ALWAYS_SAFE = frozenset(
+    b"ABCDEFGHIJKLMNOPQRSTUVWXYZ" b"abcdefghijklmnopqrstuvwxyz" b"0123456789" b"_.-~"
+)
 _ALWAYS_SAFE_BYTES = bytes(_ALWAYS_SAFE)
-_safe_quoters = {}
 
-class Quoter(collections.defaultdict):
-    """A mapping from bytes (in range(0,256)) to strings.
+
+def __getattr__(name):
+    if name == "Quoter":
+        warnings.warn(
+            "Deprecated in 3.11. "
+            "urllib.parse.Quoter will be removed in Python 3.14. "
+            "It was not intended to be a public API.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return _Quoter
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
+
+
+class _Quoter(dict):
+    """A mapping from bytes numbers (in range(0,256)) to strings.
 
     String values are percent-encoded byte values, unless the key < 128, and
-    in the "safe" set (either the specified safe set, or default set).
+    in either of the specified safe set, or the always safe set.
     """
-    # Keeps a cache internally, using defaultdict, for efficiency (lookups
+
+    # Keeps a cache internally, via __missing__, for efficiency (lookups
     # of cached keys don't call Python code at all).
     def __init__(self, safe):
         """safe: bytes object."""
         self.safe = _ALWAYS_SAFE.union(safe)
 
     def __repr__(self):
-        # Without this, will just display as a defaultdict
-        return "<%s %r>" % (self.__class__.__name__, dict(self))
+        return f"<Quoter {dict(self)!r}>"
 
     def __missing__(self, b):
         # Handle a cache miss. Store quoted string in cache and return.
-        res = chr(b) if b in self.safe else '%{:02X}'.format(b)
+        res = chr(b) if b in self.safe else "%{:02X}".format(b)
         self[b] = res
         return res
 
-def quote(string, safe='/', encoding=None, errors=None):
+
+def quote(string, safe="/", encoding=None, errors=None):
     """quote('abc def') -> 'abc%20def'
 
     Each part of a URL, e.g. the path info, the query, etc., has a
     different set of reserved characters that must be quoted. The
     quote function offers a cautious (not minimal) way to quote a
     string for most of these parts.
 
@@ -837,66 +1032,75 @@
     By default, encoding='utf-8' (characters are encoded with UTF-8), and
     errors='strict' (unsupported characters raise a UnicodeEncodeError).
     """
     if isinstance(string, str):
         if not string:
             return string
         if encoding is None:
-            encoding = 'utf-8'
+            encoding = "utf-8"
         if errors is None:
-            errors = 'strict'
+            errors = "strict"
         string = string.encode(encoding, errors)
     else:
         if encoding is not None:
             raise TypeError("quote() doesn't support 'encoding' for bytes")
         if errors is not None:
             raise TypeError("quote() doesn't support 'errors' for bytes")
     return quote_from_bytes(string, safe)
 
-def quote_plus(string, safe='', encoding=None, errors=None):
+
+def quote_plus(string, safe="", encoding=None, errors=None):
     """Like quote(), but also replace ' ' with '+', as required for quoting
     HTML form values. Plus signs in the original string are escaped unless
     they are included in safe. It also does not have safe default to '/'.
     """
     # Check if ' ' in string, where string may either be a str or bytes.  If
     # there are no spaces, the regular quote will produce the right answer.
-    if ((isinstance(string, str) and ' ' not in string) or
-        (isinstance(string, bytes) and b' ' not in string)):
+    if (isinstance(string, str) and " " not in string) or (
+        isinstance(string, bytes) and b" " not in string
+    ):
         return quote(string, safe, encoding, errors)
     if isinstance(safe, str):
-        space = ' '
+        space = " "
     else:
-        space = b' '
+        space = b" "
     string = quote(string, safe + space, encoding, errors)
-    return string.replace(' ', '+')
+    return string.replace(" ", "+")
+
 
-def quote_from_bytes(bs, safe='/'):
+# Expectation: A typical program is unlikely to create more than 5 of these.
+@functools.lru_cache
+def _byte_quoter_factory(safe):
+    return _Quoter(safe).__getitem__
+
+
+def quote_from_bytes(bs, safe="/"):
     """Like quote(), but accepts a bytes object rather than a str, and does
     not perform string-to-bytes encoding.  It always returns an ASCII string.
     quote_from_bytes(b'abc def\x3f') -> 'abc%20def%3f'
     """
     if not isinstance(bs, (bytes, bytearray)):
         raise TypeError("quote_from_bytes() expected bytes")
     if not bs:
-        return ''
+        return ""
     if isinstance(safe, str):
         # Normalize 'safe' by converting to bytes and removing non-ASCII chars
-        safe = safe.encode('ascii', 'ignore')
+        safe = safe.encode("ascii", "ignore")
     else:
+        # List comprehensions are faster than generator expressions.
         safe = bytes([c for c in safe if c < 128])
     if not bs.rstrip(_ALWAYS_SAFE_BYTES + safe):
         return bs.decode()
-    try:
-        quoter = _safe_quoters[safe]
-    except KeyError:
-        _safe_quoters[safe] = quoter = Quoter(safe).__getitem__
-    return ''.join([quoter(char) for char in bs])
+    quoter = _byte_quoter_factory(safe)
+    return "".join([quoter(char) for char in bs])
+
 
-def urlencode(query, doseq=False, safe='', encoding=None, errors=None,
-              quote_via=quote_plus):
+def urlencode(
+    query, doseq=False, safe="", encoding=None, errors=None, quote_via=quote_plus
+):
     """Encode a dict or sequence of two-element tuples into a URL query string.
 
     If any values in the query arg are sequences and doseq is true, each
     sequence element is converted to a separate parameter.
 
     If the query arg is a sequence of two-element tuples, the order of the
     parameters in the output will match the order of parameters in the
@@ -918,262 +1122,300 @@
             # non-empty strings will fail this
             if len(query) and not isinstance(query[0], tuple):
                 raise TypeError
             # Zero-length sequences of all types will get here and succeed,
             # but that's a minor nit.  Since the original implementation
             # allowed empty dicts that type of behavior probably should be
             # preserved for consistency
-        except TypeError:
-            ty, va, tb = sys.exc_info()
-            raise TypeError("not a valid non-string sequence "
-                            "or mapping object").with_traceback(tb)
+        except TypeError as err:
+            raise TypeError(
+                "not a valid non-string sequence " "or mapping object"
+            ) from err
 
     l = []
     if not doseq:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
             else:
                 v = quote_via(str(v), safe, encoding, errors)
-            l.append(k + '=' + v)
+            l.append(k + "=" + v)
     else:
         for k, v in query:
             if isinstance(k, bytes):
                 k = quote_via(k, safe)
             else:
                 k = quote_via(str(k), safe, encoding, errors)
 
             if isinstance(v, bytes):
                 v = quote_via(v, safe)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             elif isinstance(v, str):
                 v = quote_via(v, safe, encoding, errors)
-                l.append(k + '=' + v)
+                l.append(k + "=" + v)
             else:
                 try:
                     # Is this a sufficient test for sequence-ness?
                     x = len(v)
                 except TypeError:
                     # not a sequence
                     v = quote_via(str(v), safe, encoding, errors)
-                    l.append(k + '=' + v)
+                    l.append(k + "=" + v)
                 else:
                     # loop over the sequence
                     for elt in v:
                         if isinstance(elt, bytes):
                             elt = quote_via(elt, safe)
                         else:
                             elt = quote_via(str(elt), safe, encoding, errors)
-                        l.append(k + '=' + elt)
-    return '&'.join(l)
+                        l.append(k + "=" + elt)
+    return "&".join(l)
 
 
 def to_bytes(url):
-    warnings.warn("urllib.parse.to_bytes() is deprecated as of 3.8",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.to_bytes() is deprecated as of 3.8",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _to_bytes(url)
 
 
 def _to_bytes(url):
     """to_bytes(u"URL") --> 'URL'."""
     # Most URL schemes require ASCII. If that changes, the conversion
     # can be relaxed.
     # XXX get rid of to_bytes()
     if isinstance(url, str):
         try:
             url = url.encode("ASCII").decode()
         except UnicodeError:
-            raise UnicodeError("URL " + repr(url) +
-                               " contains non-ASCII characters")
+            raise UnicodeError("URL " + repr(url) + " contains non-ASCII characters")
     return url
 
 
 def unwrap(url):
     """Transform a string like '<URL:scheme://host/path>' into 'scheme://host/path'.
 
     The string is returned unchanged if it's not a wrapped URL.
     """
     url = str(url).strip()
-    if url[:1] == '<' and url[-1:] == '>':
+    if url[:1] == "<" and url[-1:] == ">":
         url = url[1:-1].strip()
-    if url[:4] == 'URL:':
+    if url[:4] == "URL:":
         url = url[4:].strip()
     return url
 
 
 def splittype(url):
-    warnings.warn("urllib.parse.splittype() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splittype() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splittype(url)
 
 
 _typeprog = None
+
+
 def _splittype(url):
     """splittype('type:opaquestring') --> 'type', 'opaquestring'."""
     global _typeprog
     if _typeprog is None:
-        _typeprog = re.compile('([^/:]+):(.*)', re.DOTALL)
+        _typeprog = re.compile("([^/:]+):(.*)", re.DOTALL)
 
     match = _typeprog.match(url)
     if match:
         scheme, data = match.groups()
         return scheme.lower(), data
     return None, url
 
 
 def splithost(url):
-    warnings.warn("urllib.parse.splithost() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splithost() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splithost(url)
 
 
 _hostprog = None
+
+
 def _splithost(url):
     """splithost('//host[:port]/path') --> 'host[:port]', '/path'."""
     global _hostprog
     if _hostprog is None:
-        _hostprog = re.compile('//([^/#?]*)(.*)', re.DOTALL)
+        _hostprog = re.compile("//([^/#?]*)(.*)", re.DOTALL)
 
     match = _hostprog.match(url)
     if match:
         host_port, path = match.groups()
-        if path and path[0] != '/':
-            path = '/' + path
+        if path and path[0] != "/":
+            path = "/" + path
         return host_port, path
     return None, url
 
 
 def splituser(host):
-    warnings.warn("urllib.parse.splituser() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splituser() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splituser(host)
 
 
 def _splituser(host):
     """splituser('user[:passwd]@host[:port]') --> 'user[:passwd]', 'host[:port]'."""
-    user, delim, host = host.rpartition('@')
+    user, delim, host = host.rpartition("@")
     return (user if delim else None), host
 
 
 def splitpasswd(user):
-    warnings.warn("urllib.parse.splitpasswd() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitpasswd() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitpasswd(user)
 
 
 def _splitpasswd(user):
     """splitpasswd('user:passwd') -> 'user', 'passwd'."""
-    user, delim, passwd = user.partition(':')
+    user, delim, passwd = user.partition(":")
     return user, (passwd if delim else None)
 
 
 def splitport(host):
-    warnings.warn("urllib.parse.splitport() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitport(host)
 
 
 # splittag('/path#tag') --> '/path', 'tag'
 _portprog = None
+
+
 def _splitport(host):
     """splitport('host:port') --> 'host', 'port'."""
     global _portprog
     if _portprog is None:
-        _portprog = re.compile('(.*):([0-9]*)', re.DOTALL)
+        _portprog = re.compile("(.*):([0-9]*)", re.DOTALL)
 
     match = _portprog.fullmatch(host)
     if match:
         host, port = match.groups()
         if port:
             return host, port
     return host, None
 
 
 def splitnport(host, defport=-1):
-    warnings.warn("urllib.parse.splitnport() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitnport() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitnport(host, defport)
 
 
 def _splitnport(host, defport=-1):
     """Split host and port, returning numeric port.
     Return given default port if no ':' found; defaults to -1.
     Return numerical port if a valid number are found after ':'.
     Return None if ':' but not a valid number."""
-    host, delim, port = host.rpartition(':')
+    host, delim, port = host.rpartition(":")
     if not delim:
         host = port
     elif port:
         try:
             nport = int(port)
         except ValueError:
             nport = None
         return host, nport
     return host, defport
 
 
 def splitquery(url):
-    warnings.warn("urllib.parse.splitquery() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitquery() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitquery(url)
 
 
 def _splitquery(url):
     """splitquery('/path?query') --> '/path', 'query'."""
-    path, delim, query = url.rpartition('?')
+    path, delim, query = url.rpartition("?")
     if delim:
         return path, query
     return url, None
 
 
 def splittag(url):
-    warnings.warn("urllib.parse.splittag() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splittag() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splittag(url)
 
 
 def _splittag(url):
     """splittag('/path#tag') --> '/path', 'tag'."""
-    path, delim, tag = url.rpartition('#')
+    path, delim, tag = url.rpartition("#")
     if delim:
         return path, tag
     return url, None
 
 
 def splitattr(url):
-    warnings.warn("urllib.parse.splitattr() is deprecated as of 3.8, "
-                  "use urllib.parse.urlparse() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitattr() is deprecated as of 3.8, "
+        "use urllib.parse.urlparse() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitattr(url)
 
 
 def _splitattr(url):
     """splitattr('/path;attr1=value1;attr2=value2;...') ->
-        '/path', ['attr1=value1', 'attr2=value2', ...]."""
-    words = url.split(';')
+    '/path', ['attr1=value1', 'attr2=value2', ...]."""
+    words = url.split(";")
     return words[0], words[1:]
 
 
 def splitvalue(attr):
-    warnings.warn("urllib.parse.splitvalue() is deprecated as of 3.8, "
-                  "use urllib.parse.parse_qsl() instead",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "urllib.parse.splitvalue() is deprecated as of 3.8, "
+        "use urllib.parse.parse_qsl() instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _splitvalue(attr)
 
 
 def _splitvalue(attr):
     """splitvalue('attr=value') --> 'attr', 'value'."""
-    attr, delim, value = attr.partition('=')
+    attr, delim, value = attr.partition("=")
     return attr, (value if delim else None)
```

### Comparing `ignition-gemini-0.1.8/ignition/request.py` & `ignition_gemini-0.2.0/ignition/request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,240 +1,381 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import logging
 import re
 import socket
 import ssl
-from socket import gaierror as SocketGaiErrorException  # pylint:disable=no-name-in-module
-from socket import herror as SocketHErrorException  # pylint:disable=no-name-in-module
-from socket import timeout as SocketTimeoutException  # pylint:disable=no-name-in-module
+from socket import gaierror as SocketGaiErrorException
+from socket import herror as SocketHErrorException
+from socket import timeout as SocketTimeoutException
 
 import cryptography
 
-from .exceptions import GeminiResponseParseError, RemoteCertificateExpired, TofuCertificateRejection
-from .globals import *
+from .exceptions import (
+    GeminiResponseParseError,
+    RemoteCertificateExpired,
+    TofuCertificateRejection,
+)
+from .globals import (
+    CRLF,
+    GEMINI_DEFAULT_ENCODING,
+    GEMINI_RESPONSE_HEADER_META_MAXLENGTH,
+    GEMINI_RESPONSE_HEADER_SEPARATOR,
+    RESPONSE_STATUSDETAIL_ERROR_DNS,
+    RESPONSE_STATUSDETAIL_ERROR_HOST,
+    RESPONSE_STATUSDETAIL_ERROR_PROTOCOL,
+    RESPONSE_STATUSDETAIL_ERROR_TLS,
+)
 from .response import BaseResponse, ResponseFactory
 from .ssl.cert_wrapper import CertWrapper
 from .url import URL
 
 logger = logging.getLogger(__name__)
 
 
 class Request:
-  '''
-  Handles a single request to a Gemini Server.
+    """
+    Handles a single request to a Gemini Server.
 
-  The request handler has four key responsibilities:
+    The request handler has four key responsibilities:
 
-  1. It manages resolution of the requested URL for
-     the remote server, by invoking underlying URL parse
-     logic
-  2. It manages transmission of the request via TLS over a
-     socket connection to the remote server.
-  3. It validates SSL certificate response using a TOFU
-     (trust-on-first-use) validation paradigm
-  4. It manages raw response handling and designation to
-     the Response object
-  '''
-  def __init__(self, url: str, referer=None, request_timeout=None, cert_store=None, ca_cert=None):
-    '''
-    Initializes Response with a url, referer, and timeout
-    '''
-
-    self.__url = URL(url, referer_url=referer)
-    self.__timeout = request_timeout
-    self.__cert_store = cert_store
-    self.__ca_cert = ca_cert  # This should be a tuple
-
-  def get_url(self):
-    '''
-    Fetch the generated URL for the request (based on referer, if present)
-    '''
-
-    return str(self.__url)
-
-  def send(self):
-    '''
-    Performes network communication and returns a Response object
-    '''
-
-    logger.debug(f"Attempting to create a connection to {self.__url.netloc()}")
-    socket_result = self.__get_socket()
-    if isinstance(socket_result, BaseResponse):
-      return socket_result
-
-    logger.debug(f"Attempting to negotiate SSL handshake with {self.__url.netloc()}")
-    secure_socket_result = self.__negotiate_ssl(socket_result)
-    if isinstance(secure_socket_result, BaseResponse):
-      return secure_socket_result
-
-    logger.debug(f"Validating server certificate to {self.__url.netloc()}")
-    ssl_certificate_result = self.__validate_ssl_certificate(secure_socket_result)
-    if isinstance(ssl_certificate_result, BaseResponse):
-      return ssl_certificate_result
-
-    logger.debug(f"Sending request header: {self.__url}")
-    transport_result = self.__transport_payload(secure_socket_result, self.__url)
-    if isinstance(transport_result, BaseResponse):
-      return transport_result
-
-    header, raw_body = transport_result
-    logger.debug(f"Received response header: [{header}] and payload of length {len(raw_body)} bytes")
-    return self.__handle_response(header, raw_body, ssl_certificate_result.certificate)
-
-  def __get_socket(self):
-    '''
-    Creates a socket connection and manages exceptions.
-    '''
-
-    try:
-      sock = socket.create_connection((self.__url.host(), self.__url.port()), timeout=self.__timeout)
-      logger.debug(f"Created socket connection: {sock}")
-      return sock
-    except ConnectionRefusedError as err:
-      logger.debug(f"ConnectionRefusedError: Connection to {self.__url.netloc()} was refused. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Connection refused")
-    except ConnectionResetError as err:
-      logger.debug(f"ConnectionResetError: Connection to {self.__url.netloc()} was reset. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Connection reset")
-    except SocketHErrorException as err:
-      logger.debug(f"socket.herror: socket.gethostbyaddr returned for {self.__url.host()}. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Host error")
-    except SocketGaiErrorException as err:
-      logger.debug(f"socket.gaierror: socket.getaddrinfo returned unknown host for {self.__url.host()}. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_DNS, "Unknown host")
-    except SocketTimeoutException as err:
-      logger.debug(f"socket.timeout: socket timed out connecting to {self.__url.host()}. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout")
-    except Exception as err:
-      logger.error(f"Unknown exception encountered when connecting to {self.__url.netloc()} - {err}")
-      raise err
-
-  def __negotiate_ssl(self, socket_obj) -> ssl.SSLSocket:
-    '''
-    Negotiates a SSL handshake on the passed socket connection and returns the secure socket
-    '''
-
-    try:
-      context = self.__setup_ssl_default_context()
-
-      if self.is_using_ca_cert():
-        self.__setup_ssl_client_certificate_context(context)
-
-      secure_socket_result = context.wrap_socket(socket_obj, server_hostname=self.__url.host())
-      return secure_socket_result
-    except ssl.SSLError as err:
-      logger.debug(f"ssl.SSLError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "Generic SSL Error")
-    except ssl.SSLZeroReturnError as err:
-      logger.debug(f"ssl.SSLZeroReturnError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Zero Return Error")
-    except ssl.SSLWantReadError as err:
-      logger.debug(f"ssl.SSLWantReadError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Read Error")
-    except ssl.SSLWantWriteError as err:
-      logger.debug(f"ssl.SSLWantWriteError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Write Error")
-    except ssl.SSLSyscallError as err:
-      logger.debug(f"ssl.SSLSyscallError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Syscall Error")
-    except ssl.SSLEOFError as err:
-      logger.debug(f"ssl.SSLEOFError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL EOF Error")
-    except ssl.SSLCertVerificationError as err:
-      logger.debug(f"ssl.SSLCertVerificationError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Certificate Verification Error")
-    except ssl.CertificateError as err:
-      logger.debug(f"ssl.CertificateError for {self.__url.host()} - {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Certificate Error")
-    except SocketTimeoutException:
-      logger.debug(f"socket.timeout: socket timed out connecting to {self.__url.host()}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout")
-    except Exception as err:
-      logger.error(f"Unknown exception encountered when completing SSL handshake for {self.__url.host()} - {err}")
-      raise err
-
-  def __validate_ssl_certificate(self, secure_socket) -> CertWrapper:
-    '''
-    Trust-on-first-use (TOFU) validation on SSL certificate or throws exception
-    '''
-
-    try:
-      certificate_wrapper = CertWrapper.parse(secure_socket.getpeercert(True))
-      self.__cert_store.validate_tofu_or_add(secure_socket.server_hostname, certificate_wrapper)
-      return certificate_wrapper
-    except ValueError as err:
-      logger.debug(f"ValueError: {self.__url.netloc()}. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, err)
-    except RemoteCertificateExpired as err:
-      logger.debug(f"RemoteCertificateExpired: {self.__url.netloc()} has an expired certificate. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "Certificate expired")
-    except TofuCertificateRejection as err:
-      logger.debug(f"TofuCertificateRejection: {self.__url.netloc()} has an untrusted, unknown certificate. {err}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "Untrusted certificate (TOFU rejection)")
-    except Exception as err:
-      logger.error(f"Unknown exception encountered when validating ssl certificate on {self.__url.netloc()} - {err}")
-      raise err
-
-  def is_using_ca_cert(self):
-    '''
-    Returns if the request is using ca_cert
-    '''
-    return self.__ca_cert is not None
-
-  def __setup_ssl_default_context(self):
-    '''
-    Setup an SSL default context (without a client certificate)
-    This will bypass certificate validation against a CA.
-    TOFU validation will be completed after the request is completed.
-    '''
-
-    context = ssl.create_default_context()
-    context.check_hostname = False
-    context.verify_mode = ssl.CERT_NONE
-    return context
-
-  def __setup_ssl_client_certificate_context(self, context):
-    '''
-    Load cert chain for client certificate
-    TODO: Better error handling here?
-    '''
-    cert, key = self.__ca_cert
-    context.load_cert_chain(cert, key)
-
-  def __transport_payload(self, socket_obj, payload):
-    '''
-    Handles Gemini protocol negotiation over the socket
-    '''
-
-    try:
-      socket_obj.sendall((f"{payload}{CRLF}").encode(GEMINI_DEFAULT_ENCODING))
-      fd = socket_obj.makefile('rb')
-      return fd.readline().decode(GEMINI_DEFAULT_ENCODING).strip(), fd.read()
-    except SocketTimeoutException:
-      logger.debug(f"socket.timeout: socket timed out connecting to {self.__url.host()}")
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout")
-    except Exception as err:
-      logger.error(f"Unknown exception encountered when transporting data to {self.__url.netloc()} - {err}")
-      raise err
-
-  def __handle_response(self, header, raw_body, certificate: cryptography.x509.Certificate):
-    '''
-    Handles basic response data from the remote server and hands off to the Response object
-    '''
-    try:
-      status, meta = re.split(GEMINI_RESPONSE_HEADER_SEPARATOR, header, maxsplit=1)
-
-      if not re.match(r"^\d{2}$", status):
-        raise GeminiResponseParseError("Response status is not a two-digit code")
-
-      if len(meta) > GEMINI_RESPONSE_HEADER_META_MAXLENGTH:
-        raise GeminiResponseParseError("Header meta text is too long")
-
-      return ResponseFactory.create(self.__url, status, meta.strip(), raw_body, certificate)
-    except GeminiResponseParseError as err:
-      return ResponseFactory.create(self.__url, RESPONSE_STATUSDETAIL_ERROR_PROTOCOL, err)
+    1. It manages resolution of the requested URL for
+       the remote server, by invoking underlying URL parse
+       logic
+    2. It manages transmission of the request via TLS over a
+       socket connection to the remote server.
+    3. It validates SSL certificate response using a TOFU
+       (trust-on-first-use) validation paradigm
+    4. It manages raw response handling and designation to
+       the Response object (or exception raising, if indicated)
+    """
+
+    def __init__(
+        self,
+        url: str,
+        raise_errors=False,
+        referer=None,
+        request_timeout=None,
+        cert_store=None,
+        ca_cert=None,
+    ):
+        """
+        Initializes Response with a url, referer, and timeout
+        """
+
+        self.__url = URL(url, referer_url=referer)
+        self.__raise_errors = raise_errors
+        self.__timeout = request_timeout
+        self.__cert_store = cert_store
+        self.__ca_cert = ca_cert  # This should be a tuple
+
+    def get_url(self):
+        """
+        Fetch the generated URL for the request (based on referer, if present)
+        """
+
+        return str(self.__url)
+
+    def send(self):
+        """
+        Performes network communication and returns a Response object
+        """
+
+        logger.debug(f"Attempting to create a connection to {self.__url.netloc()}")
+        socket_result = self.__get_socket()
+        if isinstance(socket_result, BaseResponse):
+            return socket_result
+
+        logger.debug(
+            f"Attempting to negotiate SSL handshake with {self.__url.netloc()}"
+        )
+        secure_socket_result = self.__negotiate_ssl(socket_result)
+        if isinstance(secure_socket_result, BaseResponse):
+            return secure_socket_result
+
+        logger.debug(f"Validating server certificate to {self.__url.netloc()}")
+        ssl_certificate_result = self.__validate_ssl_certificate(secure_socket_result)
+        if isinstance(ssl_certificate_result, BaseResponse):
+            return ssl_certificate_result
+
+        logger.debug(f"Sending request header: {self.__url}")
+        transport_result = self.__transport_payload(secure_socket_result, self.__url)
+        if isinstance(transport_result, BaseResponse):
+            return transport_result
+
+        header, raw_body = transport_result
+        logger.debug(
+            f"Received response header: [{header}] and payload of length {len(raw_body)} bytes"
+        )
+        return self.__handle_response(
+            header, raw_body, ssl_certificate_result.certificate
+        )
+
+    def __get_socket(self):
+        """
+        Creates a socket connection and manages exceptions.
+        """
+
+        try:
+            sock = socket.create_connection(
+                (self.__url.host(), self.__url.port()), timeout=self.__timeout
+            )
+            logger.debug(f"Created socket connection: {sock}")
+            return sock
+        except ConnectionRefusedError as err:
+            logger.debug(
+                f"ConnectionRefusedError: Connection to {self.__url.netloc()} was refused. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Connection refused"
+            )
+        except ConnectionResetError as err:
+            logger.debug(
+                f"ConnectionResetError: Connection to {self.__url.netloc()} was reset. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Connection reset"
+            )
+        except SocketHErrorException as err:
+            logger.debug(
+                f"socket.herror: socket.gethostbyaddr returned for {self.__url.host()}. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Host error"
+            )
+        except SocketGaiErrorException as err:
+            logger.debug(
+                f"socket.gaierror: socket.getaddrinfo returned unknown host for {self.__url.host()}. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_DNS, "Unknown host"
+            )
+        except SocketTimeoutException as err:
+            logger.debug(
+                f"socket.timeout: socket timed out connecting to {self.__url.host()}. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout"
+            )
+        except Exception as err:
+            logger.error(
+                f"Unknown exception encountered when connecting to {self.__url.netloc()} - {err}"
+            )
+            raise err
+
+    def __negotiate_ssl(self, socket_obj) -> ssl.SSLSocket:
+        """
+        Negotiates a SSL handshake on the passed socket connection and returns the secure socket
+        """
+
+        try:
+            context = self.__setup_ssl_default_context()
+
+            if self.is_using_ca_cert():
+                self.__setup_ssl_client_certificate_context(context)
+
+            secure_socket_result = context.wrap_socket(
+                socket_obj, server_hostname=self.__url.host()
+            )
+            return secure_socket_result
+        except ssl.SSLZeroReturnError as err:
+            logger.debug(f"ssl.SSLZeroReturnError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Zero Return Error"
+            )
+        except ssl.SSLWantReadError as err:
+            logger.debug(f"ssl.SSLWantReadError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Read Error"
+            )
+        except ssl.SSLWantWriteError as err:
+            logger.debug(f"ssl.SSLWantWriteError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Write Error"
+            )
+        except ssl.SSLSyscallError as err:
+            logger.debug(f"ssl.SSLSyscallError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Syscall Error"
+            )
+        except ssl.SSLEOFError as err:
+            logger.debug(f"ssl.SSLEOFError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL EOF Error"
+            )
+        except ssl.SSLCertVerificationError as err:
+            logger.debug(
+                f"ssl.SSLCertVerificationError for {self.__url.host()} - {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url,
+                RESPONSE_STATUSDETAIL_ERROR_TLS,
+                "SSL Certificate Verification Error",
+            )
+        except ssl.SSLError as err:
+            logger.debug(f"ssl.SSLError for {self.__url.host()} - {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "SSL Error"
+            )
+        except SocketTimeoutException as err:
+            logger.debug(
+                f"socket.timeout: socket timed out connecting to {self.__url.host()}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout"
+            )
+        except Exception as err:
+            logger.error(
+                f"Unknown exception encountered when completing SSL handshake for {self.__url.host()} - {err}"
+            )
+            raise err
+
+    def __validate_ssl_certificate(self, secure_socket) -> CertWrapper:
+        """
+        Trust-on-first-use (TOFU) validation on SSL certificate or throws exception
+        """
+
+        try:
+            certificate_wrapper = CertWrapper.parse(secure_socket.getpeercert(True))
+            self.__cert_store.validate_tofu_or_add(
+                secure_socket.server_hostname, certificate_wrapper
+            )
+            return certificate_wrapper
+        except ValueError as err:
+            logger.debug(f"ValueError: {self.__url.netloc()}. {err}")
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, err
+            )
+        except RemoteCertificateExpired as err:
+            logger.debug(
+                f"RemoteCertificateExpired: {self.__url.netloc()} has an expired certificate. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_TLS, "Certificate expired"
+            )
+        except TofuCertificateRejection as err:
+            logger.debug(
+                f"TofuCertificateRejection: {self.__url.netloc()} has an untrusted, unknown certificate. {err}"
+            )
+            if self.__raise_errors:
+                raise err
+            return ResponseFactory.create(
+                self.__url,
+                RESPONSE_STATUSDETAIL_ERROR_TLS,
+                "Untrusted certificate (TOFU rejection)",
+            )
+        except Exception as err:
+            logger.error(
+                f"Unknown exception encountered when validating ssl certificate on {self.__url.netloc()} - {err}"
+            )
+            raise err
+
+    def is_using_ca_cert(self):
+        """
+        Returns if the request is using ca_cert
+        """
+        return self.__ca_cert is not None
+
+    def __setup_ssl_default_context(self):
+        """
+        Setup an SSL default context (without a client certificate)
+        This will bypass certificate validation against a CA.
+        TOFU validation will be completed after the request is completed.
+        """
+
+        context = ssl.create_default_context()
+        context.minimum_version = ssl.TLSVersion.TLSv1_2
+        context.check_hostname = False
+        context.verify_mode = ssl.CERT_NONE
+        return context
+
+    def __setup_ssl_client_certificate_context(self, context):
+        """
+        Load cert chain for client certificate
+        TODO: Better error handling here?
+        """
+        cert, key = self.__ca_cert
+        context.load_cert_chain(cert, key)
+
+    def __transport_payload(self, socket_obj, payload):
+        """
+        Handles Gemini protocol negotiation over the socket
+        """
+
+        try:
+            socket_obj.sendall((f"{payload}{CRLF}").encode(GEMINI_DEFAULT_ENCODING))
+            fd = socket_obj.makefile("rb")
+            return fd.readline().decode(GEMINI_DEFAULT_ENCODING).strip(), fd.read()
+        except SocketTimeoutException:
+            logger.debug(
+                f"socket.timeout: socket timed out connecting to {self.__url.host()}"
+            )
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_HOST, "Socket timeout"
+            )
+        except Exception as err:
+            logger.error(
+                f"Unknown exception encountered when transporting data to {self.__url.netloc()} - {err}"
+            )
+            raise err
+
+    def __handle_response(
+        self, header, raw_body, certificate: cryptography.x509.Certificate
+    ):
+        """
+        Handles basic response data from the remote server and hands off to the Response object
+        """
+        try:
+            status, meta = re.split(
+                GEMINI_RESPONSE_HEADER_SEPARATOR, header, maxsplit=1
+            )
+
+            if not re.match(r"^\d{2}$", status):
+                raise GeminiResponseParseError(
+                    "Response status is not a two-digit code"
+                )
+
+            if len(meta) > GEMINI_RESPONSE_HEADER_META_MAXLENGTH:
+                raise GeminiResponseParseError("Header meta text is too long")
+
+            return ResponseFactory.create(
+                self.__url, status, meta.strip(), raw_body, certificate
+            )
+        except GeminiResponseParseError as err:
+            return ResponseFactory.create(
+                self.__url, RESPONSE_STATUSDETAIL_ERROR_PROTOCOL, err
+            )
```

### Comparing `ignition-gemini-0.1.8/ignition/response.py` & `ignition_gemini-0.2.0/ignition/response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,258 +1,284 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import cgi
 import logging
 
 from cryptography.x509 import Certificate
 
-from .globals import *
+from .globals import (
+    CRLF,
+    GEMINI_DEFAULT_ENCODING,
+    GEMINI_DEFAULT_MIME_TYPE,
+    RESPONSE_STATUSDETAIL_ERROR_PROTOCOL,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class ResponseFactory:
-  '''
-  Wrapper class for factory:
-  Determines the approriate response type based on response status
-  and generates the appropriate response type
-  '''
-  @classmethod
-  def create(cls, url: str, status: str, meta=None, raw_body=None, certificate=None):
-    '''
-    Given a url, status, and response data, generates the appropriate response type
-    '''
-    basic_status_code = status[0]
-    factories = {
-      "0": ErrorResponse,
-      "1": InputResponse,
-      "2": SuccessResponse,
-      "3": RedirectResponse,
-      "4": TempFailureResponse,
-      "5": PermFailureResponse,
-      "6": ClientCertRequiredResponse,
-    }
-
-    factory_class = factories.get(basic_status_code, None)
-
-    if factory_class is None:
-      return ErrorResponse(
-        url,
-        RESPONSE_STATUSDETAIL_ERROR_PROTOCOL,
-        f"Invalid response received from the server, status code: {status}",
-        None,
-        None,
-      )
+    """
+    Wrapper class for factory:
+    Determines the approriate response type based on response status
+    and generates the appropriate response type
+    """
+
+    @classmethod
+    def create(cls, url: str, status: str, meta=None, raw_body=None, certificate=None):
+        """
+        Given a url, status, and response data, generates the appropriate response type
+        """
+        basic_status_code = status[0]
+        factories = {
+            "0": ErrorResponse,
+            "1": InputResponse,
+            "2": SuccessResponse,
+            "3": RedirectResponse,
+            "4": TempFailureResponse,
+            "5": PermFailureResponse,
+            "6": ClientCertRequiredResponse,
+        }
+
+        factory_class = factories.get(basic_status_code, None)
+
+        if factory_class is None:
+            return ErrorResponse(
+                url,
+                RESPONSE_STATUSDETAIL_ERROR_PROTOCOL,
+                f"Invalid response received from the server, status code: {status}",
+                None,
+                None,
+            )
 
-    return factory_class(url, status, meta, raw_body, certificate)
+        return factory_class(url, status, meta, raw_body, certificate)
 
 
 class BaseResponse:
-  '''
-  Abstract Base response type that all response types inherit from.
-  Included public members:
-  * url
-  * basic_status
-  * status
-  * meta
-  * raw_body
-  * certificate
-  '''
-
-  url: str
-  basic_status: str
-  status: str
-  meta: str
-  raw_body: bytes
-  certificate: Certificate
-
-  def __init__(self, url: str, status: str, meta: str, raw_body: bytes, certificate: Certificate):
-    '''
-    Initializes a BaseResponse with the request url, status code, metadata, raw body string, and remote certificate
-    '''
-    self.url = str(url)
-    self.basic_status = status[0]
-    self.status = status
-    self.meta = meta
-    self.raw_body = raw_body
-    self.certificate = certificate
-
-  def is_a(self, response_class_type):
-    '''
-    Returns true if the response class type matches the current class
-    '''
-    return isinstance(self, response_class_type)
-
-  def success(self):
-    '''
-    Returns true if the response is of the type success
-    '''
-    return self.is_a(SuccessResponse)
-
-  def data(self):
-    '''
-    Fetches processed data from the response.  This method should be overloaded in each specific response type.
-    '''
-    return self.raw_body
-
-  def __str__(self):
-    '''
-    Returns a literal string representation of the response, including messageheader
-    '''
-    return f"{self.status} {self.meta}"
-
-  def __repr__(self):
-    '''
-    A representation of the string for developers
-    '''
-    return f'<ignition.response.{self.__class__.__name__}: {self.status} {self.meta} [from {self.url}]>'
+    """
+    Abstract Base response type that all response types inherit from.
+    Included public members:
+    * url
+    * basic_status
+    * status
+    * meta
+    * raw_body
+    * certificate
+    """
+
+    url: str
+    basic_status: str
+    status: str
+    meta: str
+    raw_body: bytes
+    certificate: Certificate
+
+    def __init__(
+        self,
+        url: str,
+        status: str,
+        meta: str,
+        raw_body: bytes,
+        certificate: Certificate,
+    ):
+        """
+        Initializes a BaseResponse with the request url, status code, metadata, raw body string, and remote certificate
+        """
+        self.url = str(url)
+        self.basic_status = status[0]
+        self.status = status
+        self.meta = meta
+        self.raw_body = raw_body
+        self.certificate = certificate
+
+    def is_a(self, response_class_type):
+        """
+        Returns true if the response class type matches the current class
+        """
+        return isinstance(self, response_class_type)
+
+    def success(self):
+        """
+        Returns true if the response is of the type success
+        """
+        return self.is_a(SuccessResponse)
+
+    def data(self):
+        """
+        Fetches processed data from the response.  This method should be overloaded in each specific response type.
+        """
+        return self.raw_body
+
+    def __str__(self):
+        """
+        Returns a literal string representation of the response, including messageheader
+        """
+        return f"{self.status} {self.meta}"
+
+    def __repr__(self):
+        """
+        A representation of the string for developers
+        """
+        return f"<ignition.response.{self.__class__.__name__}: {self.status} {self.meta} [from {self.url}]>"
 
 
 class ErrorResponse(BaseResponse):
-  '''
-  ErrorResponse
-  This is a custom response type for ignition, to handle any responses representing request errors
-  that are outside of the scope of the Gemini protocol.  Included options are:
-
-  00: RESPONSE_STATUSDETAIL_ERROR_NETWORK
-  Any errors that occur at the network level, and prevented the client from making any connection
-  with external services.
-
-  01: RESPONSE_STATUSDETAIL_ERROR_DNS = "01"
-  Any errors at the DNS level.
-
-  02: RESPONSE_STATUSDETAIL_ERROR_HOST
-  Any errors connecting to the host (timeout, refused, etc.).
-
-  03: RESPONSE_STATUSDETAIL_ERROR_TLS
-  Any errors associated with TLS/SSL, including handshake errors, certificate expired errors,
-  and security errors like certificate rejection errors.
-
-  04: RESPONSE_STATUSDETAIL_ERROR_PROTOCOL
-  Any errors where a secure message is received from the server, but it does not conform to the
-  Gemini protocol requirements and cannot be processed.
-  '''
-  def data(self):
-    '''
-    Fetch data relevant to the ErrorResponse; in this case the metadata message from the response
-    '''
-    return self.meta
+    """
+    ErrorResponse
+    This is a custom response type for ignition, to handle any responses representing request errors
+    that are outside of the scope of the Gemini protocol.  Included options are:
+
+    00: RESPONSE_STATUSDETAIL_ERROR_NETWORK
+    Any errors that occur at the network level, and prevented the client from making any connection
+    with external services.
+
+    01: RESPONSE_STATUSDETAIL_ERROR_DNS = "01"
+    Any errors at the DNS level.
+
+    02: RESPONSE_STATUSDETAIL_ERROR_HOST
+    Any errors connecting to the host (timeout, refused, etc.).
+
+    03: RESPONSE_STATUSDETAIL_ERROR_TLS
+    Any errors associated with TLS/SSL, including handshake errors, certificate expired errors,
+    and security errors like certificate rejection errors.
+
+    04: RESPONSE_STATUSDETAIL_ERROR_PROTOCOL
+    Any errors where a secure message is received from the server, but it does not conform to the
+    Gemini protocol requirements and cannot be processed.
+    """
+
+    def data(self):
+        """
+        Fetch data relevant to the ErrorResponse; in this case the metadata message from the response
+        """
+        return self.meta
 
 
 class InputResponse(BaseResponse):
-  '''
-  InputRequest
-  Meets Gemini specification: 3.2.1 1x (INPUT)
-
-  Status codes beginning with 1 are INPUT status codes, meaning that
-  the requested resource accepts a line of textual user input.
-
-  The user should reissue a request to the url with parameters in the form:
-  gemini://hostname/path?query
-  '''
-  def data(self):
-    '''
-    Returns the related instructions for the InputResponse.
-    The <META> line is a prompt which should be displayed to the user.
-    '''
-    return self.meta
+    """
+    InputRequest
+    Meets Gemini specification: 3.2.1 1x (INPUT)
+
+    Status codes beginning with 1 are INPUT status codes, meaning that
+    the requested resource accepts a line of textual user input.
+
+    The user should reissue a request to the url with parameters in the form:
+    gemini://hostname/path?query
+    """
+
+    def data(self):
+        """
+        Returns the related instructions for the InputResponse.
+        The <META> line is a prompt which should be displayed to the user.
+        """
+        return self.meta
 
 
 class SuccessResponse(BaseResponse):
-  '''
-  SuccessResponse
-  Meets Gemini specification: 3.2.2 2x (SUCCESS)
-
-  Status codes beginning with 2 are SUCCESS status codes.
-  '''
-  def data(self):
-    '''
-    Decode the success message body using metadata in the appropriate encoding type
-    '''
-
-    meta = self.meta or GEMINI_DEFAULT_MIME_TYPE
-    _, options = cgi.parse_header(meta)
-    encoding = options['charset'] if 'charset' in options else GEMINI_DEFAULT_ENCODING
-    try:
-      return self.raw_body.decode(encoding)
-    except LookupError:
-      logger.warning(f"Could not decode response body using invalid encoding {encoding}")
-      return self.raw_body
-    except UnicodeDecodeError:
-      logger.warning(f"Could not decode response body via encoding {encoding}, returning raw data")
-      return self.raw_body
-
-  def __str__(self):
-    '''
-    The string representation of the success message should be header + body
-    '''
-    return f"{self.status} {self.meta}{CRLF}{self.data()}"
+    """
+    SuccessResponse
+    Meets Gemini specification: 3.2.2 2x (SUCCESS)
+
+    Status codes beginning with 2 are SUCCESS status codes.
+    """
+
+    def data(self):
+        """
+        Decode the success message body using metadata in the appropriate encoding type
+        """
+
+        meta = self.meta or GEMINI_DEFAULT_MIME_TYPE
+        _, options = cgi.parse_header(meta)
+        encoding = (
+            options["charset"] if "charset" in options else GEMINI_DEFAULT_ENCODING
+        )
+        try:
+            return self.raw_body.decode(encoding)
+        except LookupError:
+            logger.warning(
+                f"Could not decode response body using invalid encoding {encoding}"
+            )
+            return self.raw_body
+        except UnicodeDecodeError:
+            logger.warning(
+                f"Could not decode response body via encoding {encoding}, returning raw data"
+            )
+            return self.raw_body
+
+    def __str__(self):
+        """
+        The string representation of the success message should be header + body
+        """
+        return f"{self.status} {self.meta}{CRLF}{self.data()}"
 
 
 class RedirectResponse(BaseResponse):
-  '''
-  RedirectResponse
-  Meets Gemini specification: 3.2.3 3x (REDIRECT)
-
-  Status codes beginning with 3 are REDIRECT status codes.
-
-  The server is redirecting the client to a new location for the requested resource
-  '''
-  def data(self):
-    '''
-    Returns the new destination for redirection from the server
-    '''
-    return self.meta
+    """
+    RedirectResponse
+    Meets Gemini specification: 3.2.3 3x (REDIRECT)
+
+    Status codes beginning with 3 are REDIRECT status codes.
+
+    The server is redirecting the client to a new location for the requested resource
+    """
+
+    def data(self):
+        """
+        Returns the new destination for redirection from the server
+        """
+        return self.meta
 
 
 class TempFailureResponse(BaseResponse):
-  '''
-  TempFailureResponse
-  Meets Gemini specification: 3.2.4 4x (TEMPORARY FAILURE)
-
-  Status codes beginning with 4 are TEMPORARY FAILURE status codes.
-
-  The request has failed, but an identical request may success in the future.
-  '''
-  def data(self):
-    '''
-    Returns the data from the server in the META field, which may provide additional information to the user.
-    '''
-    return f"{self.status} {self.meta}"
+    """
+    TempFailureResponse
+    Meets Gemini specification: 3.2.4 4x (TEMPORARY FAILURE)
+
+    Status codes beginning with 4 are TEMPORARY FAILURE status codes.
+
+    The request has failed, but an identical request may success in the future.
+    """
+
+    def data(self):
+        """
+        Returns the data from the server in the META field, which may provide additional information to the user.
+        """
+        return f"{self.status} {self.meta}"
 
 
 class PermFailureResponse(BaseResponse):
-  '''
-  PermFailureResponse
-  Meets Gemini specification: 3.2.5 5x (PERMANENT FAILURE)
-
-  Status codes beginning with 5 are PERMANENT FAILURE status codes.
-
-  The request has failed, identical requests will likely fail in the future.
-  '''
-  def data(self):
-    '''
-    Returns the data from the server in the META field, which may provide additional information to the user.
-    '''
-    return f"{self.status} {self.meta}"
+    """
+    PermFailureResponse
+    Meets Gemini specification: 3.2.5 5x (PERMANENT FAILURE)
+
+    Status codes beginning with 5 are PERMANENT FAILURE status codes.
+
+    The request has failed, identical requests will likely fail in the future.
+    """
+
+    def data(self):
+        """
+        Returns the data from the server in the META field, which may provide additional information to the user.
+        """
+        return f"{self.status} {self.meta}"
 
 
 class ClientCertRequiredResponse(BaseResponse):
-  '''
-  ClientCertRequiredResponse
-  Meets Gemini specification: 3.2.6 6x (CLIENT CERTIFICATE REQUIRED)
-
-  Status codes beginning with 6 are CLIENT CERTIFICATE REQUIRED status codes
-
-  The request should be retried with a client certificate.
-  '''
-  def data(self):
-    '''
-    Return additional information from the server on certificate requirements
-    or the reason a certificate was rejected
-    '''
-    return self.meta
+    """
+    ClientCertRequiredResponse
+    Meets Gemini specification: 3.2.6 6x (CLIENT CERTIFICATE REQUIRED)
+
+    Status codes beginning with 6 are CLIENT CERTIFICATE REQUIRED status codes
+
+    The request should be retried with a client certificate.
+    """
+
+    def data(self):
+        """
+        Return additional information from the server on certificate requirements
+        or the reason a certificate was rejected
+        """
+        return self.meta
```

### Comparing `ignition-gemini-0.1.8/ignition/ssl/cert_record.py` & `ignition_gemini-0.2.0/ignition/ssl/cert_record.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,73 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import datetime
 
 from ..exceptions import CertRecordParseException
-from ..globals import *
+from ..globals import EOL
 
 
 class CertRecord:
-  '''
-  Manages a single Certificate Record with a hostfile, signature, and expiration
-  '''
-  hostname: str
-  fingerprint: str
-  expiration: datetime.datetime
-
-  def __init__(self, hostname: str, fingerprint: str, expiration: datetime.datetime):
-    '''
-    Generate a CertRecord from logic; passing in the hostname, fingerprint, and expiration
-    '''
-    self.hostname = hostname
-    self.fingerprint = fingerprint
-    self.expiration = expiration
-
-  @classmethod
-  def from_string(cls, host_string: str):
-    '''
-    Generate a CertRecord from a string in the format:
-    [HOSTNAME] [SSH-ALGORITHM PUBLIC_KEY];EXPIRES=[YYYY-MM-DDTHH:mm:ss.SSSZ]
-    '''
-    try:
-      hostname, fingerprint_with_expiration = host_string.strip().split(' ', maxsplit=1)
-      fingerprint, expiration = fingerprint_with_expiration.split(';EXPIRES=')
-      expiration_datetime = datetime.datetime.fromisoformat(expiration)
-
-      return CertRecord(hostname, fingerprint, expiration_datetime)
-    except Exception as e:
-      raise CertRecordParseException() from e
-
-  def to_string(self):
-    '''
-    Converts a CertRecord to a string in the format:
-    [HOSTNAME] [SSH-ALGORITHM PUBLIC_KEY];EXPIRES=[YYYY-MM-DDTHH:mm:ss.SSSZ]
-    '''
-    return self.hostname + ' ' + self.fingerprint + ';EXPIRES=' + self.expiration.isoformat() + EOL
-
-  def is_expired(self):
-    '''
-    Returns true if the expiration date on the cert record is before now
-    '''
-    return self.expiration < self.now()
-
-  def now(self):
-    '''
-    Utility function to get current datetime, extracted for testing purposes
-    Returns datetime
-    '''
-    return datetime.datetime.now()
+    """
+    Manages a single Certificate Record with a hostfile, signature, and expiration
+    """
+
+    hostname: str
+    fingerprint: str
+    expiration: datetime.datetime
+
+    def __init__(self, hostname: str, fingerprint: str, expiration: datetime.datetime):
+        """
+        Generate a CertRecord from logic; passing in the hostname, fingerprint, and expiration
+        """
+        self.hostname = hostname
+        self.fingerprint = fingerprint
+        self.expiration = expiration
+
+    @classmethod
+    def from_string(cls, host_string: str):
+        """
+        Generate a CertRecord from a string in the format:
+        [HOSTNAME] [SSH-ALGORITHM PUBLIC_KEY];EXPIRES=[YYYY-MM-DDTHH:mm:ss.SSSZ]
+        """
+        try:
+            hostname, fingerprint_with_expiration = host_string.strip().split(
+                " ", maxsplit=1
+            )
+            fingerprint, expiration = fingerprint_with_expiration.split(";EXPIRES=")
+            expiration_datetime = datetime.datetime.fromisoformat(expiration)
+
+            return CertRecord(hostname, fingerprint, expiration_datetime)
+        except Exception as e:
+            raise CertRecordParseException() from e
+
+    def to_string(self):
+        """
+        Converts a CertRecord to a string in the format:
+        [HOSTNAME] [SSH-ALGORITHM PUBLIC_KEY];EXPIRES=[YYYY-MM-DDTHH:mm:ss.SSSZ]
+        """
+        return (
+            self.hostname
+            + " "
+            + self.fingerprint
+            + ";EXPIRES="
+            + self.expiration.isoformat()
+            + EOL
+        )
+
+    def is_expired(self):
+        """
+        Returns true if the expiration date on the cert record is before now
+        """
+        return self.expiration < self.now()
+
+    def now(self):
+        """
+        Utility function to get current datetime, extracted for testing purposes
+        Returns datetime
+        """
+        return datetime.datetime.now()
```

### Comparing `ignition-gemini-0.1.8/ignition/ssl/cert_store.py` & `ignition_gemini-0.2.0/ignition/ssl/cert_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,129 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import logging
 from typing import Dict
 
-from ..exceptions import CertRecordParseException, RemoteCertificateExpired, TofuCertificateRejection
+from ..exceptions import (
+    CertRecordParseException,
+    RemoteCertificateExpired,
+    TofuCertificateRejection,
+)
 from .cert_record import CertRecord
 from .cert_wrapper import CertWrapper
 
 logger = logging.getLogger(__name__)
 
 
 class CertStore:
-  '''
-  Data structure to store the certificates across visited hosts
-  '''
-
-  __hosts_file: str
-  __cert_store_data: Dict[str, CertRecord]
-
-  def __init__(self, hosts_file):
-    '''
-    Initializes a new cert store with a specified file to store the certificate fingerprint & expiration dates
-    '''
-    self.__cert_store_data = {}
-    self.__hosts_file = hosts_file
-
-  def set_hosts_file(self, hosts_file):
-    '''
-    Updates the specified file for certificate fingerprint storage
-    '''
-    self.__hosts_file = hosts_file
-
-  def get_hosts_file(self):
-    '''
-    Returns the currently set hosts file location
-    '''
-    return self.__hosts_file
-
-  def validate_tofu_or_add(self, hostname: str, cert: CertWrapper) -> bool:
-    '''
-    Given the hostname & correspoding certificate, this function:
-    1. Checks to see if the certificate is expired (if so, it throws a RemoteCertificateExpired exception)
-    2. Fetches a corresponding stored certificate record from the client to implement a TOFU check:
-      a. If there is a local cert record, and it's not expired, and it matches the passed certificate, return success
-      b. If there is not a local cert record, save the certificate record locally, and return success
-      c. If there is a local cert record, but it's expired, save the certificate record locally, and return success
-      d. If there is a local cert record, and it's not expired, but it does not match the passed certificate, throw TofuCertificateRejection
-    '''
-    remote_cert_record = CertRecord(hostname, cert.fingerprint(), cert.expiration())
-
-    if remote_cert_record.is_expired():
-      raise RemoteCertificateExpired
-
-    local_cert_record = self.__get_cert_record(hostname)
-
-    if local_cert_record and not local_cert_record.is_expired() and local_cert_record.fingerprint != remote_cert_record.fingerprint:
-      raise TofuCertificateRejection
-
-    self.__add_cert_record(remote_cert_record)
-    return True
-
-  def __get_cert_record(self, hostname: str) -> CertRecord:
-    '''
-    Fetch the corresponding CertRecord for passed hostname from the local storage (file)
-    TODO: smarter loading logic
-    '''
-    self.__load()
-    return self.__cert_store_data.get(hostname, None)
-
-  def __add_cert_record(self, cert_record: CertRecord):
-    '''
-    Add a CertRecord for the corresponding hostname to local storage (file) and save to file
-    TODO: smarter saving logic
-    '''
-    self.__cert_store_data[cert_record.hostname] = cert_record
-    self.__save()
-    return self
-
-  def __load(self):
-    '''
-    Reloads the hosts file from storage and copies that into memory
-    '''
-    file_lines = []
-    try:
-      with open(self.__hosts_file, 'r') as f:
-        file_lines = f.readlines()
-    except FileNotFoundError:
-      file_lines = []
-
-    for file_line in file_lines:
-      cert_record = self.__load_record(file_line)
-      if cert_record is not None:
+    """
+    Data structure to store the certificates across visited hosts
+    """
+
+    __hosts_file: str
+    __cert_store_data: Dict[str, CertRecord]
+
+    def __init__(self, hosts_file):
+        """
+        Initializes a new cert store with a specified file to store the certificate fingerprint & expiration dates
+        """
+        self.__cert_store_data = {}
+        self.__hosts_file = hosts_file
+
+    def set_hosts_file(self, hosts_file):
+        """
+        Updates the specified file for certificate fingerprint storage
+        """
+        self.__hosts_file = hosts_file
+
+    def get_hosts_file(self):
+        """
+        Returns the currently set hosts file location
+        """
+        return self.__hosts_file
+
+    def validate_tofu_or_add(self, hostname: str, cert: CertWrapper) -> bool:
+        """
+        Given the hostname & correspoding certificate, this function:
+        1. Checks to see if the certificate is expired (if so, it throws a RemoteCertificateExpired exception)
+        2. Fetches a corresponding stored certificate record from the client to implement a TOFU check:
+          a. If there is a local cert record, and it's not expired, and it matches the passed certificate, return success
+          b. If there is not a local cert record, save the certificate record locally, and return success
+          c. If there is a local cert record, but it's expired, save the certificate record locally, and return success
+          d. If there is a local cert record, and it's not expired, but it does not match the passed certificate,
+             throw TofuCertificateRejection
+        """
+        remote_cert_record = CertRecord(hostname, cert.fingerprint(), cert.expiration())
+
+        if remote_cert_record.is_expired():
+            raise RemoteCertificateExpired
+
+        local_cert_record = self.__get_cert_record(hostname)
+
+        if (
+            local_cert_record
+            and not local_cert_record.is_expired()
+            and local_cert_record.fingerprint != remote_cert_record.fingerprint
+        ):
+            raise TofuCertificateRejection
+
+        self.__add_cert_record(remote_cert_record)
+        return True
+
+    def __get_cert_record(self, hostname: str) -> CertRecord:
+        """
+        Fetch the corresponding CertRecord for passed hostname from the local storage (file)
+        TODO: smarter loading logic
+        """
+        self.__load()
+        return self.__cert_store_data.get(hostname, None)
+
+    def __add_cert_record(self, cert_record: CertRecord):
+        """
+        Add a CertRecord for the corresponding hostname to local storage (file) and save to file
+        TODO: smarter saving logic
+        """
         self.__cert_store_data[cert_record.hostname] = cert_record
+        self.__save()
+        return self
 
-    return self
+    def __load(self):
+        """
+        Reloads the hosts file from storage and copies that into memory
+        """
+        file_lines = []
+        try:
+            with open(self.__hosts_file, "r", encoding="utf-8") as f:
+                file_lines = f.readlines()
+        except FileNotFoundError:
+            file_lines = []
+
+        for file_line in file_lines:
+            cert_record = self.__load_record(file_line)
+            if cert_record is not None:
+                self.__cert_store_data[cert_record.hostname] = cert_record
+
+        return self
+
+    def __load_record(self, file_line):
+        try:
+            return CertRecord.from_string(file_line)
+        except CertRecordParseException:
+            logger.warning(
+                f"Invalid TOFU record encountered: '{file_line.strip()}'. This record has been skipped."
+            )
+            return None
+
+    def __save(self):
+        """
+        Saves the full set of host records back to file
+        """
+        with open(self.__hosts_file, "w", encoding="utf-8") as f:
+            for c in self.__cert_store_data.values():
+                f.write(c.to_string())
 
-  def __load_record(self, file_line):
-    try:
-      return CertRecord.from_string(file_line)
-    except CertRecordParseException:
-      logger.warning(f"Invalid TOFU record encountered: '{file_line.strip()}'. This record has been skipped.")
-      return None
-
-  def __save(self):
-    '''
-    Saves the full set of host records back to file
-    '''
-    with open(self.__hosts_file, 'w') as f:
-      for c in self.__cert_store_data.values():
-        f.write(c.to_string())
-
-    return self
+        return self
```

### Comparing `ignition-gemini-0.1.8/ignition/ssl/cert_wrapper.py` & `ignition_gemini-0.2.0/ignition/ssl/cert_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import cryptography
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 
 
 class CertWrapper:
-  '''
-  Certificate as defined by x509
-  '''
-  certificate: cryptography.x509.Certificate
-  '''
+    """
+    Certificate as defined by x509
+    """
+
+    certificate: cryptography.x509.Certificate
+    """
   Certificate fingerprint, to be used in TOFU handling and response
-  '''
-  public_key_fingerprint: str
+  """
+    public_key_fingerprint: str
 
-  def __init__(self, certificate: cryptography.x509.Certificate):
-    '''
-    Constructor
-    '''
-    self.certificate = certificate
-
-  def expiration(self) -> str:
-    '''
-    Access function for certificate expiration date
-    '''
-    return self.certificate.not_valid_after
-
-  def fingerprint(self) -> str:
-    '''
-    Extracts the public key & expiration date from the cert,
-    and returns the public key openssh fingerprint
-    '''
-    return self.certificate.public_key().public_bytes(
-      cryptography.hazmat.primitives.serialization.Encoding.OpenSSH,
-      cryptography.hazmat.primitives.serialization.PublicFormat.OpenSSH
-    ).decode('utf-8')
-
-  @classmethod
-  def parse(cls, raw_certificate: bytes):
-    '''
-    Takes as input the raw certificate (originally from the TCP socket)
-    Returns a certificate wrapper
-    '''
-    x509_certificate = x509.load_der_x509_certificate(raw_certificate, default_backend())
-    return CertWrapper(x509_certificate)
+    def __init__(self, certificate: cryptography.x509.Certificate):
+        """
+        Constructor
+        """
+        self.certificate = certificate
+
+    def expiration(self) -> str:
+        """
+        Access function for certificate expiration date
+        """
+        return self.certificate.not_valid_after
+
+    def fingerprint(self) -> str:
+        """
+        Extracts the public key & expiration date from the cert,
+        and returns the public key openssh fingerprint
+        """
+        return (
+            self.certificate.public_key()
+            .public_bytes(
+                cryptography.hazmat.primitives.serialization.Encoding.OpenSSH,
+                cryptography.hazmat.primitives.serialization.PublicFormat.OpenSSH,
+            )
+            .decode("utf-8")
+        )
+
+    @classmethod
+    def parse(cls, raw_certificate: bytes):
+        """
+        Takes as input the raw certificate (originally from the TCP socket)
+        Returns a certificate wrapper
+        """
+        x509_certificate = x509.load_der_x509_certificate(
+            raw_certificate, default_backend()
+        )
+        return CertWrapper(x509_certificate)
```

### Comparing `ignition-gemini-0.1.8/ignition/url.py` & `ignition_gemini-0.2.0/ignition/url.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,122 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import logging
 
-from .globals import *
+from .globals import GEMINI_PORT, GEMINI_SCHEME
 from .python import urllib
 from .util import normalize_path
 
 logger = logging.getLogger(__name__)
 
 
 class URL:
-  '''
-  The URL class negotiates the correct URL based on passed in URL.
+    """
+    The URL class negotiates the correct URL based on passed in URL.
 
-  This logic prepares the URL to be passed via the socket connector,
-  as well as for the data payload for Gemini.
-  '''
-  def __init__(self, url, referer_url=None):
-    '''
-    Construct a protocool-safe URL based on the passed string.
-    '''
-    self.__parsed_url = self.__url_constructor(url, referer_url)
-
-    logger.debug((f"Recieved url {url} for parsing, {f'with referer {referer_url}, ' if referer_url else ''} generated gemini url: {self}"))
-
-  def __url_constructor(self, url, referer_url):
-    '''
-    Constructs a protocol-safe URL based on the passed string.
-
-    If referer_url is included (which should be the constructed
-    URL from the last time this ran), the new url is joined onto
-    the referer.  This allows the user to pass in paths without a
-    hostname.
-    '''
-
-    url = url.lstrip()
-    base_url = url
-    if referer_url:
-      base_url = urllib.parse.urljoin(referer_url, url, False)
-
-    return urllib.parse.urlsplit(base_url, GEMINI_SCHEME, False)
-
-  def __str__(self):
-    '''
-    Custom logic to re-join the URL into a string
-    TODO url = 'about:blank', 'example:test' RFC-6694 and RFC-7585
-    '''
-
-    return ''.join([
-      self.protocol(),
-      self.host(),
-      (f":{self.port()}" if self.port() != GEMINI_PORT else ''),
-      self.path(),
-      (f"?{self.query()}" if self.query() else '')
-    ])
-
-  def path(self):
-    '''
-    Returns path portion of the url
-    URL Schema: scheme://host:port/path?query
-    '''
-
-    return normalize_path(self.__parsed_url.path or '')
-
-  def host(self):
-    '''
-    Returns host portion of the url
-    URL Schema: scheme://host:port/path?query
-    '''
-
-    return self.__parsed_url.hostname or ''
-
-  def port(self):
-    '''
-    Returns port portion of the url
-    URL Schema: scheme://host:port/path?query
-    '''
-
-    try:
-      return self.__parsed_url.port or GEMINI_PORT
-    except ValueError:
-      # https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlsplit
-      logger.warning(f"There was an error reading the port from the url. Defaulting to {GEMINI_PORT}")
-      return GEMINI_PORT
-
-  def netloc(self):
-    '''
-    Returns netloc portion of the url, which is the host:port
-    URL Schema: scheme://host:port/path?query
-    '''
-
-    return self.__parsed_url.netloc
-
-  def protocol(self):
-    '''
-    Returns scheme portion of the url with the protocol designator "://"
-    URL Schema: scheme://host:port/path?query
-    '''
-
-    return f"{self.__parsed_url.scheme}://"
-
-  def query(self):
-    '''
-    Returns query portion of the url
-    URL Schema: scheme://host:port/path?query
-    '''
-    return self.__parsed_url.query
+    This logic prepares the URL to be passed via the socket connector,
+    as well as for the data payload for Gemini.
+    """
+
+    def __init__(self, url, referer_url=None):
+        """
+        Construct a protocool-safe URL based on the passed string.
+        """
+        self.__parsed_url = self.__url_constructor(url, referer_url)
+
+        logger.debug(
+            (
+                f"Recieved url {url} for parsing, {f'with referer {referer_url}, ' if referer_url else ''} generated gemini url: {self}"
+            )
+        )
+
+    def __url_constructor(self, url, referer_url):
+        """
+        Constructs a protocol-safe URL based on the passed string.
+
+        If referer_url is included (which should be the constructed
+        URL from the last time this ran), the new url is joined onto
+        the referer.  This allows the user to pass in paths without a
+        hostname.
+        """
+
+        url = url.lstrip()
+        base_url = url
+        if referer_url:
+            base_url = urllib.parse.urljoin(referer_url, url, False)
+
+        return urllib.parse.urlsplit(base_url, GEMINI_SCHEME, False)
+
+    def __str__(self):
+        """
+        Custom logic to re-join the URL into a string
+        TODO url = 'about:blank', 'example:test' RFC-6694 and RFC-7585
+        """
+
+        return "".join(
+            [
+                self.protocol(),
+                self.host(),
+                (f":{self.port()}" if self.port() != GEMINI_PORT else ""),
+                self.path(),
+                (f"?{self.query()}" if self.query() else ""),
+            ]
+        )
+
+    def path(self):
+        """
+        Returns path portion of the url
+        URL Schema: scheme://host:port/path?query
+        """
+
+        return normalize_path(self.__parsed_url.path or "")
+
+    def host(self):
+        """
+        Returns host portion of the url
+        URL Schema: scheme://host:port/path?query
+        """
+
+        return self.__parsed_url.hostname or ""
+
+    def port(self):
+        """
+        Returns port portion of the url
+        URL Schema: scheme://host:port/path?query
+        """
+
+        try:
+            return self.__parsed_url.port or GEMINI_PORT
+        except ValueError:
+            # https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlsplit
+            logger.warning(
+                f"There was an error reading the port from the url. Defaulting to {GEMINI_PORT}"
+            )
+            return GEMINI_PORT
+
+    def netloc(self):
+        """
+        Returns netloc portion of the url, which is the host:port
+        URL Schema: scheme://host:port/path?query
+        """
+
+        return self.__parsed_url.netloc
+
+    def protocol(self):
+        """
+        Returns scheme portion of the url with the protocol designator "://"
+        URL Schema: scheme://host:port/path?query
+        """
+
+        return f"{self.__parsed_url.scheme}://"
+
+    def query(self):
+        """
+        Returns query portion of the url
+        URL Schema: scheme://host:port/path?query
+        """
+        return self.__parsed_url.query
```

### Comparing `ignition-gemini-0.1.8/ignition/util.py` & `ignition_gemini-0.2.0/ignition/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-'''
+"""
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL
 was not distributed with this file, You can obtain one
 at http://mozilla.org/MPL/2.0/.
-'''
+"""
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def normalize_path(path: str) -> str:
-  '''
-  Implements a normalized path for a string
-  See RFC-3986 https://tools.ietf.org/html/rfc3986#section-5.2.4
-  5.2.4.  Remove Dot Segments
-
-  Example:
-    STEP   OUTPUT BUFFER         INPUT BUFFER
-
-      1 :                         /a/b/c/./../../g
-      2E:   /a                    /b/c/./../../g
-      2E:   /a/b                  /c/./../../g
-      2E:   /a/b/c                /./../../g
-      2B:   /a/b/c                /../../g
-      2C:   /a/b                  /../g
-      2C:   /a                    /g
-      2E:   /a/g
-  '''
-  result_stack = []
-  for component in path.split('/'):
-    if component in ('.', ''):
-      continue  # Do nothing
-    if component == '..':
-      if len(result_stack) > 0:
-        result_stack.pop()
-    else:
-      result_stack.append(component)
-
-  unescaped_path = ''.join([
-    ('/' if len(path) > 0 and path[0] == '/' else ''),
-    ('/'.join(result_stack)),
-    ('/' if len(path) > 0 and path[len(path) - 1] == '/' else ''),
-  ])
+    """
+    Implements a normalized path for a string
+    See RFC-3986 https://tools.ietf.org/html/rfc3986#section-5.2.4
+    5.2.4.  Remove Dot Segments
+
+    Example:
+      STEP   OUTPUT BUFFER         INPUT BUFFER
+
+        1 :                         /a/b/c/./../../g
+        2E:   /a                    /b/c/./../../g
+        2E:   /a/b                  /c/./../../g
+        2E:   /a/b/c                /./../../g
+        2B:   /a/b/c                /../../g
+        2C:   /a/b                  /../g
+        2C:   /a                    /g
+        2E:   /a/g
+    """
+    result_stack = []
+    for component in path.split("/"):
+        if component in (".", ""):
+            continue  # Do nothing
+        if component == "..":
+            if len(result_stack) > 0:
+                result_stack.pop()
+        else:
+            result_stack.append(component)
+
+    unescaped_path = "".join(
+        [
+            ("/" if len(path) > 0 and path[0] == "/" else ""),
+            ("/".join(result_stack)),
+            ("/" if len(path) > 0 and path[len(path) - 1] == "/" else ""),
+        ]
+    )
 
-  return unescaped_path.replace("//", "/")
+    return unescaped_path.replace("//", "/")
 
 
 class TimeoutManager:
-  '''
-  Timeout Manager for global timeout management at the top-level
-  '''
-  def __init__(self, default_timeout):
-    '''
-    Sets a default timeout on initialization
-    '''
-    self.set_default_timeout(default_timeout)
-
-  def set_default_timeout(self, default_timeout):
-    '''
-    Allow the default timeout to be overwritten
-    '''
-    self.default_timeout = default_timeout
-
-  def get_timeout(self, timeout):
-    '''
-    Takes in a timeout and returns that, or the default timeout
-    '''
-    if timeout is not None:
-      return timeout
-    return self.default_timeout
+    """
+    Timeout Manager for global timeout management at the top-level
+    """
+
+    def __init__(self, default_timeout):
+        """
+        Sets a default timeout on initialization
+        """
+        self.set_default_timeout(default_timeout)
+
+    def set_default_timeout(self, default_timeout):
+        """
+        Allow the default timeout to be overwritten
+        """
+        self.default_timeout = default_timeout
+
+    def get_timeout(self, timeout):
+        """
+        Takes in a timeout and returns that, or the default timeout
+        """
+        if timeout is not None:
+            return timeout
+        return self.default_timeout
```

