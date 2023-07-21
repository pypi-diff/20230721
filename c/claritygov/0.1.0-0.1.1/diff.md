# Comparing `tmp/claritygov-0.1.0.tar.gz` & `tmp/claritygov-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claritygov-0.1.0.tar", last modified: Fri Jul 21 21:08:01 2023, max compression
+gzip compressed data, was "claritygov-0.1.1.tar", last modified: Fri Jul 21 21:32:57 2023, max compression
```

## Comparing `claritygov-0.1.0.tar` & `claritygov-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 21:08:01.839931 claritygov-0.1.0/
--rw-rw-rw-   0        0        0    16011 2023-07-21 20:48:18.000000 claritygov-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      815 2023-07-21 21:08:01.839931 claritygov-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-07-21 21:00:01.000000 claritygov-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 21:08:01.829647 claritygov-0.1.0/claritygov/
--rw-rw-rw-   0        0        0        0 2023-07-21 20:54:23.000000 claritygov-0.1.0/claritygov/__init__.py
--rw-rw-rw-   0        0        0      641 2023-07-21 20:36:20.000000 claritygov-0.1.0/claritygov/api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:08:01.838831 claritygov-0.1.0/claritygov/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 20:24:23.000000 claritygov-0.1.0/claritygov/utils/__init__.py
--rw-rw-rw-   0        0        0     1665 2023-07-21 20:27:50.000000 claritygov-0.1.0/claritygov/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:08:01.837657 claritygov-0.1.0/claritygov.egg-info/
--rw-rw-rw-   0        0        0      815 2023-07-21 21:08:01.000000 claritygov-0.1.0/claritygov.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-21 21:08:01.000000 claritygov-0.1.0/claritygov.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:08:01.000000 claritygov-0.1.0/claritygov.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-21 21:08:01.000000 claritygov-0.1.0/claritygov.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-21 21:08:01.000000 claritygov-0.1.0/claritygov.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 21:08:01.841140 claritygov-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-07-21 21:07:58.000000 claritygov-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:32:57.083581 claritygov-0.1.1/
+-rw-rw-rw-   0        0        0    16011 2023-07-21 20:48:18.000000 claritygov-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2102 2023-07-21 21:32:57.083581 claritygov-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2023-07-21 21:14:45.000000 claritygov-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 21:32:57.070385 claritygov-0.1.1/claritygov/
+-rw-rw-rw-   0        0        0        0 2023-07-21 20:54:23.000000 claritygov-0.1.1/claritygov/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:32:57.082210 claritygov-0.1.1/claritygov/api/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:22:39.000000 claritygov-0.1.1/claritygov/api/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-21 21:29:21.000000 claritygov-0.1.1/claritygov/api/house.py
+-rw-rw-rw-   0        0        0      146 2023-07-21 20:23:10.000000 claritygov-0.1.1/claritygov/api/state.py
+-rw-rw-rw-   0        0        0      641 2023-07-21 20:36:20.000000 claritygov-0.1.1/claritygov/api_client.py
+-rw-rw-rw-   0        0        0     1686 2023-07-21 21:29:36.000000 claritygov-0.1.1/claritygov/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:32:57.079486 claritygov-0.1.1/claritygov.egg-info/
+-rw-rw-rw-   0        0        0     2102 2023-07-21 21:32:57.000000 claritygov-0.1.1/claritygov.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-21 21:32:57.000000 claritygov-0.1.1/claritygov.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:32:57.000000 claritygov-0.1.1/claritygov.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-21 21:32:57.000000 claritygov-0.1.1/claritygov.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 21:32:57.000000 claritygov-0.1.1/claritygov.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 21:32:57.084967 claritygov-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-07-21 21:32:50.000000 claritygov-0.1.1/setup.py
```

### Comparing `claritygov-0.1.0/LICENSE.txt` & `claritygov-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `claritygov-0.1.0/claritygov/api_client.py` & `claritygov-0.1.1/claritygov/api_client.py`

 * *Files identical despite different names*

### Comparing `claritygov-0.1.0/claritygov/utils/utils.py` & `claritygov-0.1.1/claritygov/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-us_state_to_abbrev = {
+us_state_to_abbrev_dict = {
     "Alabama": "AL",
     "Alaska": "AK",
     "Arizona": "AZ",
     "Arkansas": "AR",
     "California": "CA",
     "Colorado": "CO",
     "Connecticut": "CT",
@@ -57,11 +56,11 @@
     "Puerto Rico": "PR",
     "United States Minor Outlying Islands": "UM",
     "U.S. Virgin Islands": "VI",
 }
     
 def abbrev_to_us_state(abbrev):
     abbrev = abbrev.upper()
-    return dict(map(reversed, us_state_to_abbrev.items()))[abbrev]
+    return dict(map(reversed, us_state_to_abbrev_dict.items()))[abbrev]
 def us_state_to_abbrev(state):
     state = state.title()
-    return us_state_to_abbrev[state]
+    return us_state_to_abbrev_dict[state].lower()
```

### Comparing `claritygov-0.1.0/setup.py` & `claritygov-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='claritygov',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests==2.31.0',
         'pytest==7.4.0'
     ],
     keywords=['claritygov', 'clarityapi', 'government', 'transparency'],
     license='Creative Commons Attribution 4.0 International Public License',
     description='Python API Client for ClarityGov, a free public developer API for accessing government legislative data in a standardized format.',
+    long_description=open('README.md').read(),
     author='ClarityGov',
-    download_url='https://github.com/ianmcvann/ClarityGovClient/archive/refs/tags/v0.1.0.tar.gz',
+    download_url='https://github.com/ianmcvann/ClarityGovClient/archive/refs/tags/v0.1.1.tar.gz',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3'
```

