# Comparing `tmp/envisionriskraas-1.0.8.tar.gz` & `tmp/envisionriskraas-1.0.9.tar.gz`

## Comparing `envisionriskraas-1.0.8.tar` & `envisionriskraas-1.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 envisionriskraas-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/README.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 envisionriskraas-1.0.9/PKG-INFO
```

### Comparing `envisionriskraas-1.0.8/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.0.9/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.8/LICENSE.txt` & `envisionriskraas-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.8/README.md` & `envisionriskraas-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.8/pyproject.toml` & `envisionriskraas-1.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
-  { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
+  { name="EnvisionRisk", email="support@envisionrisk.com" },
 ]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://www.envisionrisk.com/"
-"GitHub profile" = "https://github.com/EnvisionRisk"
+"API webpage" = "https://www.linkedin.com/safety/go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D"
+"Homepage" = "https://www.envisionrisk.com/"
```

### Comparing `envisionriskraas-1.0.8/PKG-INFO` & `envisionriskraas-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.8
+Version: 1.0.9
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
+Project-URL: API webpage, https://www.linkedin.com/safety/go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D
 Project-URL: Homepage, https://www.envisionrisk.com/
-Project-URL: GitHub profile, https://github.com/EnvisionRisk
-Author-email: Jonas Hal <jonas.hal@envisionrisk.com>
+Author-email: EnvisionRisk <support@envisionrisk.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,21 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.9 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
-Project-URL: Homepage, https://www.envisionrisk.com/ Project-URL: GitHub
-profile, https://github.com/EnvisionRisk Author-email: Jonas Hal
-hal@envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Project-URL: API webpage, https://www.linkedin.com/safety/
+go?url=https%3A%2F%2Fenvisionrisk.stoplight.io%2Fdocs%2Fapi-aleadomus-
+documentation%2Fcjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
+risk-management&trk=flagship-messaging-
+web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-
+ZDc1YzY5ODEtYWNkMy00MDUwLThhMGUtN2YxMWZjYTQyNjUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Ad_flagship3_leia_profile_views%3BHqF4fDGaRb6atW5VqsXnFw%3D%3D
+Project-URL: Homepage, https://www.envisionrisk.com/ Author-email: EnvisionRisk
+envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
+Type: text/markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
 without leaving your Python programming environment. Embrace this smarter,
```

