# Comparing `tmp/robotframework-reportportal_updated-1.1.8.tar.gz` & `tmp/robotframework-reportportal_updated-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal_updated-1.1.8.tar", last modified: Thu Jul 20 11:55:20 2023, max compression
+gzip compressed data, was "robotframework-reportportal_updated-1.1.9.tar", last modified: Thu Jul 20 19:13:11 2023, max compression
```

## Comparing `robotframework-reportportal_updated-1.1.8.tar` & `robotframework-reportportal_updated-1.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:55:20.195517 robotframework-reportportal_updated-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-20 11:55:20.195517 robotframework-reportportal_updated-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:55:20.195517 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/result_visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/variables.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:55:20.195517 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 11:55:20.000000 robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 11:55:20.195517 robotframework-reportportal_updated-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-20 11:55:15.000000 robotframework-reportportal_updated-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:13:11.718611 robotframework-reportportal_updated-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-20 19:13:11.718611 robotframework-reportportal_updated-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:13:11.714611 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/variables.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:13:11.714611 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 19:13:11.000000 robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 19:13:11.718611 robotframework-reportportal_updated-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-20 19:13:06.000000 robotframework-reportportal_updated-1.1.9/setup.py
```

### Comparing `robotframework-reportportal_updated-1.1.8/CONTRIBUTING.rst` & `robotframework-reportportal_updated-1.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/LICENSE.txt` & `robotframework-reportportal_updated-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/PKG-INFO` & `robotframework-reportportal_updated-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal_updated
-Version: 1.1.8
+Version: 1.1.9
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.8
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.9
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotframework-reportportal_updated-1.1.8/README.md` & `robotframework-reportportal_updated-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/__init__.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/exception.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/exception.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/listener.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/listener.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/listener.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/listener.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/logger.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/model.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/model.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/model.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/post_report.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/post_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/result_visitor.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/result_visitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
+import traceback
 import string
 from datetime import datetime
 
 from robot.api import ResultVisitor
 from six.moves.urllib.parse import unquote
 
 from . import listener
@@ -114,43 +115,61 @@
             'source': test.source,
             'status': test.status,
             'message': test.message,
         }
         listener.end_test(test.name, attrs, ts)
 
     def start_keyword(self, kw):
-        ts = to_timestamp(kw.starttime if kw.id not in corrections else corrections[kw.id][0])
-        attrs = {
-            'type': string.capwords(kw.type),
-            'kwname': kw.kwname,
-            'libname': kw.libname,
-            'doc': kw.doc,
-            'args': kw.args,
-            'assign': kw.assign,
-            'tags': kw.tags,
-            'starttime': ts,
-        }
-        listener.start_keyword(kw.name, attrs, ts)
+        try:
+            keyword_status = 'PASS' if kw.assign else kw.status
+            empty_arguments = bool('${' in str(kw.args))
+            keywords_as_library = '_keywords' in '' if kw.libname is None else kw.libname
+
+            if (keyword_status == 'FAIL') or (keyword_status == 'PASS' and not empty_arguments and not keywords_as_library):
+                print("suite ID {} {}.{} - {}".format(kw.id, getattr(kw, 'libname', 'none'),kw.kwname, getattr(kw, 'args', ())))
+                ts = to_timestamp(kw.starttime if kw.id not in corrections else corrections[kw.id][0])
+                attrs = {
+                    'type': string.capwords(kw.type),
+                    'kwname': kw.kwname,
+                    'libname': kw.libname,
+                    'doc': kw.doc,
+                    'args': kw.args,
+                    'assign': kw.assign,
+                    'tags': kw.tags,
+                    'starttime': ts,
+                }
+                listener.start_keyword(kw.name, attrs, ts)
+        except Exception as e:
+            traceback.print_exc()
 
     def end_keyword(self, kw):
-        ts = to_timestamp(kw.endtime if kw.id not in corrections else corrections[kw.id][1])
-        status = 'PASS' if kw.assign else kw.status
-        attrs = {
-            'type': string.capwords(kw.type),
-            'kwname': kw.kwname,
-            'libname': kw.libname,
-            'doc': kw.doc,
-            'args': kw.args,
-            'assign': kw.assign,
-            'tags': kw.tags,
-            'endtime': ts,
-            'elapsedtime': kw.elapsedtime,
-            'status': status,
-        }
-        listener.end_keyword(kw.name, attrs, ts)
+        try:
+            keyword_status = 'PASS' if kw.assign else kw.status
+            empty_arguments = bool('${' in str(kw.args))
+            keywords_as_library = '_keywords' in '' if kw.libname is None else kw.libname
+
+            if (keyword_status == 'FAIL') or (keyword_status == 'PASS' and not empty_arguments and not keywords_as_library):
+                ts = to_timestamp(kw.endtime if kw.id not in corrections else corrections[kw.id][1])
+                status = 'PASS' if kw.assign else kw.status
+                # print("E-suite ID {} {}.{}".format(kw.id, kw.libname, kw.kwname))
+                attrs = {
+                    'type': string.capwords(kw.type),
+                    'kwname': kw.kwname,
+                    'libname': kw.libname,
+                    'doc': kw.doc,
+                    'args': kw.args,
+                    'assign': kw.assign,
+                    'tags': kw.tags,
+                    'endtime': ts,
+                    'elapsedtime': kw.elapsedtime,
+                    'status': status,
+                }
+                listener.end_keyword(kw.name, attrs, ts)
+        except Exception as e:
+            traceback.print_exc()
 
     def start_message(self, msg):
         if msg.parent.status == "FAIL" and msg.message:
             message = {
                 'message': msg.message,
                 'level': msg.level
             }
```

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/result_visitor.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/result_visitor.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/service.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/service.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/service.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/service.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/static.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/static.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/static.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/time_visitor.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/variables.py` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/variables.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated/variables.pyi` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated/variables.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/PKG-INFO` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal-updated
-Version: 1.1.8
+Version: 1.1.9
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.8
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.9
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotframework-reportportal_updated-1.1.8/robotframework_reportportal_updated.egg-info/SOURCES.txt` & `robotframework-reportportal_updated-1.1.9/robotframework_reportportal_updated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.8/setup.py` & `robotframework-reportportal_updated-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup instructions for the package."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
```

