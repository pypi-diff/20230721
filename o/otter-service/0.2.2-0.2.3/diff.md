# Comparing `tmp/otter_service-0.2.2.tar.gz` & `tmp/otter_service-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.2.tar", last modified: Fri Jul 21 16:23:39 2023, max compression
+gzip compressed data, was "otter_service-0.2.3.tar", last modified: Fri Jul 21 21:02:28 2023, max compression
```

## Comparing `otter_service-0.2.2.tar` & `otter_service-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.266916 otter_service-0.2.2/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.2/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 16:23:39.267135 otter_service-0.2.2/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 16:21:06.000000 otter_service-0.2.2/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.2/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 16:23:39.268332 otter_service-0.2.2/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.249997 otter_service-0.2.2/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.258501 otter_service-0.2.2/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 16:23:21.000000 otter_service-0.2.2/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 15:08:41.000000 otter_service-0.2.2/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.2/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 18:36:10.000000 otter_service-0.2.2/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19815 2023-07-21 16:21:06.000000 otter_service-0.2.2/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.263022 otter_service-0.2.2/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 18:36:10.000000 otter_service-0.2.2/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.2/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.261673 otter_service-0.2.2/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.266028 otter_service-0.2.2/tests/
--rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.2/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 18:36:10.000000 otter_service-0.2.2/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 18:36:10.000000 otter_service-0.2.2/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.432687 otter_service-0.2.3/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.3/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 21:02:28.432941 otter_service-0.2.3/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 17:54:42.000000 otter_service-0.2.3/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.3/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 21:02:28.434100 otter_service-0.2.3/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.419700 otter_service-0.2.3/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.425184 otter_service-0.2.3/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 21:01:08.000000 otter_service-0.2.3/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 17:51:59.000000 otter_service-0.2.3/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.3/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5059 2023-07-21 21:00:48.000000 otter_service-0.2.3/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19675 2023-07-21 21:01:08.000000 otter_service-0.2.3/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.429137 otter_service-0.2.3/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-21 17:51:59.000000 otter_service-0.2.3/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.3/src/otter_service/secrets/gke_key.yaml
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.428120 otter_service-0.2.3/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.432340 otter_service-0.2.3/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.3/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-21 17:51:59.000000 otter_service-0.2.3/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2094 2023-07-21 21:00:48.000000 otter_service-0.2.3/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.2/LICENSE` & `otter_service-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/PKG-INFO` & `otter_service-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.2
+Version: 0.2.3
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.2/README.md` & `otter_service-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/setup.cfg` & `otter_service-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/src/otter_service/access_sops_keys.py` & `otter_service-0.2.3/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/src/otter_service/firestore-test.py` & `otter_service-0.2.3/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/src/otter_service/grade_assignment.py` & `otter_service-0.2.3/src/otter_service/grade_assignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,24 @@
             shutil.rmtree(storage_path)
         os.rename(extracted_path, storage_path)
         os.remove(download_path)
     else:
         raise Exception(f"Unable to access: {url}")
     return storage_path
 
+
 def remove_notebook():
     files = glob.glob('/tmp/*')
     for f in files:
         if not os.path.isdir(f):
-            os.remove(f)
+            try:
+                os.remove(f)
+            except Exception:
+                pass
+
 
 async def grade_assignment(submission, sec='3', assignment='lab01', solutions_path=None, sops_path=None, secrets_file=None, save_path=None):
     """
     This function spins up a docker instance using otter, grades the submission
     and returns the grade
 
     :param submission: the path to the file you want to grade
```

### Comparing `otter_service-0.2.2/src/otter_service/otter_nb.py` & `otter_service-0.2.3/src/otter_service/otter_nb.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 from datetime import datetime
 import os
 from hashlib import sha1
 from oauthlib.oauth1.rfc5849 import signature, parameters
 import pandas as pd
 import pytz
 from pytz import timezone
-from jupyterhub.services.auth import HubOAuthenticated, HubOAuthCallbackHandler
-from jupyterhub.utils import url_path_join
+from jupyterhub.services.auth import HubOAuthenticated
 from lxml import etree
 import aiohttp
 import async_timeout
 import tornado.web
 import tornado.httpserver
 import tornado.ioloop
 import tornado.escape
 import tornado.options
 import tornado.gen
-from tornado.web import authenticated
 from otter_service import access_sops_keys
 from otter_service.grade_assignment import grade_assignment
 import firebase_admin
 from firebase_admin import credentials, firestore
 import grpc
 from google.cloud.firestore_v1.client import firestore_client
 from google.cloud.firestore_v1.client import firestore_grpc_transport
@@ -36,14 +34,15 @@
 # Use the application default credentials
 cred = credentials.ApplicationDefault()
 firebase_admin.initialize_app(cred, {
     'projectId': os.environ.get("GCP_PROJECT_ID"),
     'storageBucket': 'data8x-scratch.appspot.com/submissions'
 })
 
+
 def write_grade(grade_info):
     """
     write the grade to the database
 
     :param grade_info: the four values in a tuple(userid, grade, section, lab, timestamp)
     :return Google FireStore document id
     """
@@ -172,17 +171,17 @@
         body_hash = base64.b64encode(body_hash_sha.digest()).decode('utf-8')
         args = {
             'oauth_body_hash': body_hash,
             'oauth_consumer_key': consumer_key,
             'oauth_timestamp': str(time.time()),
             'oauth_nonce': str(time.time())
         }
-        base_string = signature.construct_base_string(
+        base_string = signature.signature_base_string(
             'POST',
-            signature.normalize_base_string_uri(outcomes_url),
+            outcomes_url,
             signature.normalize_parameters(
                 signature.collect_parameters(body=args, headers={})
             )
         )
 
         oauth_signature = signature.sign_hmac_sha1(base_string, consumer_secret, None)
         args['oauth_signature'] = oauth_signature
@@ -272,15 +271,15 @@
                 course = notebook['metadata']['course']
 
             if notebook is None or section is None or assignment is None:
                 raise GradeSubmissionException("Notebook does not have required metadata or maybe no notebook in post")
 
             log_info_csv(user["name"], course, section, assignment, f"User logged in -  Using Referrer: {using_test_user}")
             # save notebook submission with user id and time stamp - this will be deleted
-            sub_timestamp = timestamp.replace(" ", "-").replace(",", "-").replace(":","-")
+            sub_timestamp = timestamp.replace(" ", "-").replace(",", "-").replace(":", "-")
             submission_file = f"/tmp/{user['name']}_{section}_{assignment}_{sub_timestamp}.ipynb"
             with open(submission_file, 'w', encoding="utf8") as outfile:
                 json.dump(notebook, outfile)
             save_submission(user['name'], course, section, assignment, notebook)
             log_info_csv(user["name"], course, section, assignment, "user submission saved to logs")
 
             args = {}
@@ -346,23 +345,25 @@
             log_error_csv(name, course, section, assignment, str(gp))
         except Exception as ex:
             log_error_csv(name, course, section, assignment, str(ex))
         finally:
             if os.path.exists(file_path):
                 os.remove(file_path)
 
+
 def get_timestamp():
     """
     returns the time stamp in PST Time
     """
     date_format = "%Y-%m-%d %H:%M:%S,%f"
     date = datetime.now(tz=pytz.utc)
     date = date.astimezone(timezone('US/Pacific'))
     return date.strftime(date_format)[:-3]
 
+
 def write_logs(username, course, section, assignment, msg, trace, type, collection):
     if os.getenv("VERBOSE_LOGGING") == "True" or type == "error":
         try:
             db = firestore.client()
             # this redirects FireStore to local emulator when local testing!
             if os.getenv("ENVIRONMENT") == "otter-docker-local-test":
                 channel = grpc.insecure_channel("host.docker.internal:8080")
@@ -378,14 +379,15 @@
                 'type': type,
                 'timestamp': get_timestamp()
             }
             return db.collection(collection).add(data)
         except Exception as err:
             raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
+
 def log_info_csv(username, course, section, assignment, msg):
     """
     This logs information in the chain of events -- user logs in and submits,
     graded, posted to Edx
 
     :param username: the username
     :param course: the course
@@ -411,34 +413,36 @@
     :param msg: optional message to logs
     """
     try:
         write_logs(username, course, section, assignment, msg, str(traceback.format_exc()), "error", f'{os.environ.get("ENVIRONMENT")}-logs')
     except Exception as e:
         raise e
 
+
 def log_tornado_issues(msg, type):
     """
     This logs the errors associated with tornado
 
     :param msg: message about error
     """
     try:
-        st =  str(traceback.format_exc()) 
-        st =  st if not "None" in st else None
+        st = str(traceback.format_exc())
+        st = st if "None" not in st else None
         db = firestore.client()
         data = {
             'message': msg,
             'trace': st,
             'type': type,
             'timestamp': get_timestamp()
         }
         return db.collection(f'{os.environ.get("ENVIRONMENT")}-tornado-logs').add(data)
     except Exception as err:
         raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
+
 def save_submission(username, course, section, assignment, notebook):
     """
     This logs the errors associated with tornado
 
     :param msg: message about error
     """
     try:
@@ -451,14 +455,15 @@
             'notebook': notebook,
             'timestamp': get_timestamp()
         }
         return db.collection(f'{os.environ.get("ENVIRONMENT")}-submissions').add(data)
     except Exception as err:
         raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
+
 def sig_handler(server, sig, frame):
     io_loop = tornado.ioloop.IOLoop.instance()
     MAX_WAIT_SECONDS_BEFORE_SHUTDOWN = 3
 
     def stop_loop(deadline):
         io_loop.stop()
         log_tornado_issues('Shutdown finally', "info")
@@ -468,14 +473,15 @@
         server.stop()
         log_tornado_issues(f'Will shutdown in {MAX_WAIT_SECONDS_BEFORE_SHUTDOWN} seconds ...', "info")
         stop_loop(time.time() + MAX_WAIT_SECONDS_BEFORE_SHUTDOWN)
 
     log_tornado_issues(f'Caught signal: {sig}', "warning")
     io_loop.add_callback_from_signal(shutdown)
 
+
 def start_server():
     """
     start the tornado server listening on port 10101 - I seperated this function from the main()
     in order to make testing easier
     :return: the application tornado object
     """
     tornado.options.parse_command_line()
@@ -496,19 +502,21 @@
     server.listen(10101)
 
     signal.signal(signal.SIGTERM, partial(sig_handler, server))
     signal.signal(signal.SIGINT, partial(sig_handler, server))
 
     return app
 
+
 def main():
     """
     start tornado
     """
     try:
         start_server()
         tornado.ioloop.IOLoop.current().start()
-    except Exception as e:
+    except Exception:
         log_tornado_issues("Server start up issues", "error")
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `otter_service-0.2.2/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.3/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.3/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.3/src/otter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.2
+Version: 0.2.3
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.2/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.3/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/tests/test_access_sops_keys.py` & `otter_service-0.2.3/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/tests/test_grade_assignment.py` & `otter_service-0.2.3/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.2/tests/test_otter_nb.py` & `otter_service-0.2.3/tests/test_otter_nb.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 import otter_service.otter_nb as gn
 from firebase_admin import firestore
 
 import grpc
 from google.cloud.firestore_v1.client import firestore_client
 from google.cloud.firestore_v1.client import firestore_grpc_transport
 
+
 @pytest.fixture
 def app():
     return gn.start_server()
 
+
 @pytest.fixture
 def firebase_local():
     channel = grpc.insecure_channel("localhost:8080")
     transport = firestore_grpc_transport.FirestoreGrpcTransport(channel=channel)
     db = firestore.client()
     db._firestore_api_internal = firestore_client.FirestoreClient(transport=transport)
     yield db
 
+
 @pytest.mark.skip(reason="test oauth2 now")
 async def test_http_client(http_server_client):
     resp = await http_server_client.fetch('/services/otter_grade/')
     assert resp.code == 302
     http_server_client.close()
 
 
 def test_write_grade(firebase_local):
-    grade_info = {"userid": "WRITE_TEST", "course":"8x-test", "grade": 88.0, "section": "1", "assignment": "lab99"}
+    grade_info = {"userid": "WRITE_TEST", "course": "8x-test", "grade": 88.0, "section": "1", "assignment": "lab99"}
     doc = gn.write_grade(grade_info)[1]
     doc_ref = firebase_local.collection(f'{os.environ.get("ENVIRONMENT")}-grades').document(f'{doc.id}')
     doc_obj = doc_ref.get()
     doc_dict = doc_obj.to_dict()
 
     assert "WRITE_TEST" == doc_dict["user"]
     assert "1" == doc_dict["section"]
```

