# Comparing `tmp/otter_service-0.2.1.tar.gz` & `tmp/otter_service-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.1.tar", last modified: Fri Jul 21 14:52:20 2023, max compression
+gzip compressed data, was "otter_service-0.2.2.tar", last modified: Fri Jul 21 16:23:39 2023, max compression
```

## Comparing `otter_service-0.2.1.tar` & `otter_service-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.473463 otter_service-0.2.1/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.1/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 14:52:20.473740 otter_service-0.2.1/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2022-07-15 16:10:04.000000 otter_service-0.2.1/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.1/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 14:52:20.474680 otter_service-0.2.1/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.458041 otter_service-0.2.1/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.463875 otter_service-0.2.1/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 14:51:32.000000 otter_service-0.2.1/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 00:46:58.000000 otter_service-0.2.1/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.1/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19879 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.468308 otter_service-0.2.1/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 18:36:10.000000 otter_service-0.2.1/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.1/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.466970 otter_service-0.2.1/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 14:52:20.000000 otter_service-0.2.1/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 14:52:20.472425 otter_service-0.2.1/tests/
--rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.1/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 18:36:10.000000 otter_service-0.2.1/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 18:36:10.000000 otter_service-0.2.1/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.266916 otter_service-0.2.2/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.2/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 16:23:39.267135 otter_service-0.2.2/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 16:21:06.000000 otter_service-0.2.2/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.2/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 16:23:39.268332 otter_service-0.2.2/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.249997 otter_service-0.2.2/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.258501 otter_service-0.2.2/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 16:23:21.000000 otter_service-0.2.2/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 15:08:41.000000 otter_service-0.2.2/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.2/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     4985 2023-07-20 18:36:10.000000 otter_service-0.2.2/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19815 2023-07-21 16:21:06.000000 otter_service-0.2.2/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.263022 otter_service-0.2.2/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-20 18:36:10.000000 otter_service-0.2.2/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.2/src/otter_service/secrets/gke_key.yaml
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.261673 otter_service-0.2.2/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 16:23:39.000000 otter_service-0.2.2/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 16:23:39.266028 otter_service-0.2.2/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.2/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-20 18:36:10.000000 otter_service-0.2.2/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2090 2023-07-20 18:36:10.000000 otter_service-0.2.2/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.1/LICENSE` & `otter_service-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/PKG-INFO` & `otter_service-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.1
+Version: 0.2.2
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # otter-nb service
 
 This repo contains a tornado flask app that accepts .ipynb files and grades them in a dockerized environment. Assuming you are running a Jupyterhub, you can ask Jupyterhub to run this otter-service as a service; you also have the option to run it in a stand alone manner. Grades are saved to a gcloud Cloud Firestore.
 
-A separate Jupyterhub extension, [gofer_submit](https://github.com/data-8/gofer_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
+A separate Jupyterhub extension, [otter_submit](https://github.com/data-8/otter_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
 
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
```

### Comparing `otter_service-0.2.1/README.md` & `otter_service-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # otter-nb service
 
 This repo contains a tornado flask app that accepts .ipynb files and grades them in a dockerized environment. Assuming you are running a Jupyterhub, you can ask Jupyterhub to run this otter-service as a service; you also have the option to run it in a stand alone manner. Grades are saved to a gcloud Cloud Firestore.
 
-A separate Jupyterhub extension, [gofer_submit](https://github.com/data-8/gofer_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
+A separate Jupyterhub extension, [otter_submit](https://github.com/data-8/otter_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
 
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
```

### Comparing `otter_service-0.2.1/setup.cfg` & `otter_service-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service/access_sops_keys.py` & `otter_service-0.2.2/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service/firestore-test.py` & `otter_service-0.2.2/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service/grade_assignment.py` & `otter_service-0.2.2/src/otter_service/grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service/otter_nb.py` & `otter_service-0.2.2/src/otter_service/otter_nb.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     except GradePostException as grade_post_exception:
         raise grade_post_exception
     except Exception as ex:
         raise Exception(f"Problem Posting Grade to LTI:{ex}") from ex
 
 
-class GoferHandler(HubOAuthenticated, tornado.web.RequestHandler):
+class OtterHandler(HubOAuthenticated, tornado.web.RequestHandler):
     """
     This class handles the HTTP requests for this tornado instance
     """
     def data_received(self, chunk):
         """
         abstract methods empty
         :param chunk
@@ -344,16 +344,15 @@
                 raise GradePostException("NOT POSTING Grades on purpose; see deployment-config-encrypted.yaml -- POST_GRADE")
         except GradePostException as gp:
             log_error_csv(name, course, section, assignment, str(gp))
         except Exception as ex:
             log_error_csv(name, course, section, assignment, str(ex))
         finally:
             if os.path.exists(file_path):
-                print("will remove")
-                #os.remove(file_path)
+                os.remove(file_path)
 
 def get_timestamp():
     """
     returns the time stamp in PST Time
     """
     date_format = "%Y-%m-%d %H:%M:%S,%f"
     date = datetime.now(tz=pytz.utc)
@@ -392,32 +391,33 @@
     :param course: the course
     :param section: the section
     :param assignment: the assignment
     :param msg: optional message to logs
     """
     try:
         write_logs(username, course, section, assignment, msg, None, "info", f'{os.environ.get("ENVIRONMENT")}-logs')
-    except:
-        print("here")
+    except Exception as e:
+        raise e
+
 
 def log_error_csv(username, course, section, assignment, msg):
     """
     This logs the errors occurring when posting assignments
 
     :param timestamp: when the error occurred
     :param username: the username
     :param course: the course
     :param section: the section
     :param assignment: the assignment
     :param msg: optional message to logs
     """
     try:
         write_logs(username, course, section, assignment, msg, str(traceback.format_exc()), "error", f'{os.environ.get("ENVIRONMENT")}-logs')
-    except:
-        print("here1")
+    except Exception as e:
+        raise e
 
 def log_tornado_issues(msg, type):
     """
     This logs the errors associated with tornado
 
     :param msg: message about error
     """
@@ -429,16 +429,15 @@
             'message': msg,
             'trace': st,
             'type': type,
             'timestamp': get_timestamp()
         }
         return db.collection(f'{os.environ.get("ENVIRONMENT")}-tornado-logs').add(data)
     except Exception as err:
-        #raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
-        print("here 34")
+        raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
 def save_submission(username, course, section, assignment, notebook):
     """
     This logs the errors associated with tornado
 
     :param msg: message about error
     """
@@ -478,23 +477,23 @@
     start the tornado server listening on port 10101 - I seperated this function from the main()
     in order to make testing easier
     :return: the application tornado object
     """
     tornado.options.parse_command_line()
     app = tornado.web.Application(
         [
-            (PREFIX, GoferHandler),
-            (
-                url_path_join(
-                    os.environ['JUPYTERHUB_SERVICE_PREFIX'], 'oauth_callback'
-                ),
-                HubOAuthCallbackHandler,
-            )
+            (PREFIX, OtterHandler)
+            # (
+            #     url_path_join(
+            #         PREFIX, 'oauth_callback'
+            #     ),
+            #     HubOAuthCallbackHandler,
+            # )
         ],
-        cookie_secret=os.urandom(32),
+        cookie_secret=os.urandom(32)
     )
 
     server = tornado.httpserver.HTTPServer(app)
     server.listen(10101)
 
     signal.signal(signal.SIGTERM, partial(sig_handler, server))
     signal.signal(signal.SIGINT, partial(sig_handler, server))
@@ -504,12 +503,12 @@
 def main():
     """
     start tornado
     """
     try:
         start_server()
         tornado.ioloop.IOLoop.current().start()
-    except Exception:
+    except Exception as e:
         log_tornado_issues("Server start up issues", "error")
 
 if __name__ == '__main__':
     main()
```

### Comparing `otter_service-0.2.1/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.2/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.2/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.2/src/otter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.1
+Version: 0.2.2
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # otter-nb service
 
 This repo contains a tornado flask app that accepts .ipynb files and grades them in a dockerized environment. Assuming you are running a Jupyterhub, you can ask Jupyterhub to run this otter-service as a service; you also have the option to run it in a stand alone manner. Grades are saved to a gcloud Cloud Firestore.
 
-A separate Jupyterhub extension, [gofer_submit](https://github.com/data-8/gofer_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
+A separate Jupyterhub extension, [otter_submit](https://github.com/data-8/otter_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
 
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
```

### Comparing `otter_service-0.2.1/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.2/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/tests/test_access_sops_keys.py` & `otter_service-0.2.2/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/tests/test_grade_assignment.py` & `otter_service-0.2.2/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.1/tests/test_otter_nb.py` & `otter_service-0.2.2/tests/test_otter_nb.py`

 * *Files identical despite different names*

