# Comparing `tmp/volare-0.9.0.tar.gz` & `tmp/volare-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volare-0.9.0.tar", last modified: Thu Jul 20 05:24:22 2023, max compression
+gzip compressed data, was "dist/volare-0.9.1.tar", last modified: Thu Jul 20 23:05:07 2023, max compression
```

## Comparing `volare-0.9.0.tar` & `volare-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:24:22.000000 volare-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 05:24:22.000000 volare-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:24:22.000000 volare-0.9.0/volare/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:24:22.000000 volare-0.9.0/volare/build/
--rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/git_multi_clone.py
--rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)    14117 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/sky130.py
--rw-r--r--   0 runner    (1001) docker     (122)     9206 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-07-20 05:24:05.000000 volare-0.9.0/volare/build/asap7.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-20 05:24:05.000000 volare-0.9.0/volare/families.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-20 05:24:05.000000 volare-0.9.0/volare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 05:24:05.000000 volare-0.9.0/volare/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 05:24:05.000000 volare-0.9.0/volare/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (122)     8783 2023-07-20 05:24:05.000000 volare-0.9.0/volare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-07-20 05:24:05.000000 volare-0.9.0/volare/click_common.py
--rw-r--r--   0 runner    (1001) docker     (122)    10607 2023-07-20 05:24:05.000000 volare-0.9.0/volare/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-07-20 05:24:05.000000 volare-0.9.0/volare/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:24:22.000000 volare-0.9.0/volare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 05:24:21.000000 volare-0.9.0/volare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-07-20 05:24:22.000000 volare-0.9.0/volare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 05:24:21.000000 volare-0.9.0/volare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-20 05:24:21.000000 volare-0.9.0/volare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 05:24:21.000000 volare-0.9.0/volare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-20 05:24:21.000000 volare-0.9.0/volare.egg-info/requires.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-07-20 05:24:05.000000 volare-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 05:24:22.000000 volare-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 23:05:07.000000 volare-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/git_multi_clone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14117 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/sky130.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9206 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/asap7.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-20 23:04:52.000000 volare-0.9.1/volare/families.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 23:04:52.000000 volare-0.9.1/volare/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8810 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-07-20 23:04:52.000000 volare-0.9.1/volare/click_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10607 2023-07-20 23:04:52.000000 volare-0.9.1/volare/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-07-20 23:04:52.000000 volare-0.9.1/volare/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/requires.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-07-20 23:04:52.000000 volare-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 23:05:07.000000 volare-0.9.1/PKG-INFO
```

### Comparing `volare-0.9.0/volare/build/git_multi_clone.py` & `volare-0.9.1/volare/build/git_multi_clone.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/build/__init__.py` & `volare-0.9.1/volare/build/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/build/magic.py` & `volare-0.9.1/volare/build/magic.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/build/sky130.py` & `volare-0.9.1/volare/build/sky130.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/build/gf180mcu.py` & `volare-0.9.1/volare/build/gf180mcu.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/build/asap7.py` & `volare-0.9.1/volare/build/asap7.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/families.py` & `volare-0.9.1/volare/families.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/__init__.py` & `volare-0.9.1/volare/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/__version__.py` & `volare-0.9.1/volare/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `volare-0.9.0/volare/__main__.py` & `volare-0.9.1/volare/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     version = check_version(version, tool_metadata_file_path, console)
     try:
         enable(
             pdk_root=pdk_root,
             pdk=pdk,
             version=version,
             include_libraries=include_libraries,
-            console=console,
+            output=console,
         )
     except Exception as e:
         console.print(f"[red]{e}")
         exit(-1)
 
 
 @click.command("enable_or_build", hidden=True)
@@ -264,14 +264,15 @@
             push_kwargs={
                 "owner": owner,
                 "repository": repository,
                 "token": token,
                 "pre": pre,
             },
             include_libraries=include_libraries,
+            output=console,
         )
     except Exception as e:
         console.print(f"[red]{e}")
         exit(-1)
 
 
 @click.group()
```

### Comparing `volare-0.9.0/volare/click_common.py` & `volare-0.9.1/volare/click_common.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/common.py` & `volare-0.9.1/volare/common.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare/manage.py` & `volare-0.9.1/volare/manage.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/volare.egg-info/PKG-INFO` & `volare-0.9.1/volare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.9.0
+Version: 0.9.1
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.9.0 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.9.1 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

### Comparing `volare-0.9.0/setup.py` & `volare-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.0/PKG-INFO` & `volare-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.9.0
+Version: 0.9.1
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.9.0 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.9.1 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
```

