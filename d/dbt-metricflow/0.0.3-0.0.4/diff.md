# Comparing `tmp/dbt_metricflow-0.0.3.tar.gz` & `tmp/dbt_metricflow-0.0.4.tar.gz`

## Comparing `dbt_metricflow-0.0.3.tar` & `dbt_metricflow-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/.gitignore
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/LICENSE
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/README.md
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.4/.gitignore
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.4/README.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.4/PKG-INFO
```

### Comparing `dbt_metricflow-0.0.3/.gitignore` & `dbt_metricflow-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.3/LICENSE` & `dbt_metricflow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.3/README.md` & `dbt_metricflow-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.3/PKG-INFO` & `dbt_metricflow-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-metricflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: Execute commands against the MetricFlow semantic layer with dbt.
+Project-URL: Source Code, https://github.com/dbt-labs/metricflow/tree/main/dbt-metricflow
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: BUSL-1.1
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: <3.10,>=3.8
+Requires-Python: <3.12,>=3.8
 Requires-Dist: dbt-core~=1.6.0rc1
 Requires-Dist: metricflow==0.200.0.dev13
 Provides-Extra: postgres
 Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres'
 Provides-Extra: snowflake
 Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.0.3 Summary: Execute
-commands against the MetricFlow semantic layer with dbt. Author-email: dbt Labs
+Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.0.4 Summary: Execute
+commands against the MetricFlow semantic layer with dbt. Project-URL: Source
+Code, https://github.com/dbt-labs/metricflow/tree/main/dbt-metricflow Author-
+email: dbt Labs
 dbtlabs.com> License-Expression: BUSL-1.1 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Programming Language :: Python ::
-Implementation :: PyPy Requires-Python: <3.10,>=3.8 Requires-Dist: dbt-
-core~=1.6.0rc1 Requires-Dist: metricflow==0.200.0.dev13 Provides-Extra:
-postgres Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres' Provides-
-Extra: snowflake Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
-Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Python: <3.12,>=3.8
+Requires-Dist: dbt-core~=1.6.0rc1 Requires-Dist: metricflow==0.200.0.dev13
+Provides-Extra: postgres Requires-Dist: dbt-postgres>=1.6.0b6; extra ==
+'postgres' Provides-Extra: snowflake Requires-Dist: dbt-snowflake>=1.6.0b3;
+extra == 'snowflake' Description-Content-Type: text/markdown
                     [https://img.shields.io/twitter/follow/
  dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat] [https://
     img.shields.io/badge/Slack-join-163B36] [https://img.shields.io/badge/
                         code%20style-black-000000.svg]
 # Welcome to dbt-metricflow This repo encapsulates the dbt-core, MetricFlow,
 and supported dbt-adapters packages. This package will manage the versioning
 between these packages such that they are compatible with each other. ## Repo
```

