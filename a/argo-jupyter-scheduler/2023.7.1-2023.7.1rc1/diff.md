# Comparing `tmp/argo_jupyter_scheduler-2023.7.1.tar.gz` & `tmp/argo_jupyter_scheduler-2023.7.1rc1.tar.gz`

## Comparing `argo_jupyter_scheduler-2023.7.1.tar` & `argo_jupyter_scheduler-2023.7.1rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/_version.py
--rw-r--r--   0        0        0    18851 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/executor.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/tests/test_scheduler.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/tests/test_utils.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/LICENSE.txt
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/README.md
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0    18851 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/executor.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/tests/test_scheduler.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/tests/test_utils.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/LICENSE.txt
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/README.md
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-2023.7.1rc1/PKG-INFO
```

### Comparing `argo_jupyter_scheduler-2023.7.1/.github/workflows/release.yml` & `argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/.github/workflows/tests.yml` & `argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/executor.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/executor.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/scheduler.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/task_runner.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/argo_jupyter_scheduler/utils.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/tests/conftest.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/tests/test_scheduler.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/tests/test_utils.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/.gitignore` & `argo_jupyter_scheduler-2023.7.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/LICENSE.txt` & `argo_jupyter_scheduler-2023.7.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/README.md` & `argo_jupyter_scheduler-2023.7.1rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   - [Installation](#installation)
   - [What is it?](#what-is-it)
   - [A deeper dive](#a-deeper-dive)
     - [`Job`](#job)
     - [`Job Definition`](#job-definition)
     - [Internals](#internals)
   - [Additional thoughts](#additional-thoughts)
-  - [Known issues](#known-issues)
   - [License](#license)
 
 **Argo-Jupyter-Scheduler**
 
 Submit longing running notebooks to run without the need to keep your JupyterLab server running. And submit a notebook to run on a specified schedule.
 
 ## Installation
@@ -91,14 +90,11 @@
 And when a job definition is created, a corresponding cron-workflow is created. To ensure the database is properly updated, the workflow that the cron-workflow creates has three steps. First, create a job record in the database with a status of `IN PROGRESS`. Second, run the notebook, again using `papermill` and the conda environment specified. And third, update the newly created job record with the status of the notebook run.
 
 
 ## Additional Thoughts
 
 At the moment, Argo-Jupyter-Scheduler is closely coupled with Nebari (via the Nebari-Workflow-Controller) which doesn't make it very useable for other projects. There's no need for this to necessarily be the case. By leveraging Traitlets, we can include other ways of modifying the pod spec for the running workflow and enable it to be used by other projects. If you're interested in this project and would like to see it extended, feel free to open an issue to discuss your ideas. Thank you :)
 
-## Known Issues
-
-All of the core features of Jupyter-Scheduler have been mapped over to Argo-Jupyter-Scheduler. Unfortunately, there is currently a limitation with `Update Job Definition` and with `Pause`/`Resume` for Job Definitions. Although the `Pause` works, the `Resume` fails for the same reason `Update Job Definition` does and this is because the upstream Nebari-Workflow-Controller (see [Known Limitations](https://github.com/nebari-dev/nebari-workflow-controller#known-limitations)) has a limitation whereby it can't resubmit workflows/cron-workflows; there are more details in [this issue](https://github.com/nebari-dev/nebari-workflow-controller/issues/18).
 
 ## License
 
 `argo-jupyter-scheduler` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `argo_jupyter_scheduler-2023.7.1/pyproject.toml` & `argo_jupyter_scheduler-2023.7.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-2023.7.1/PKG-INFO` & `argo_jupyter_scheduler-2023.7.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argo-jupyter-scheduler
-Version: 2023.7.1
+Version: 2023.7.1rc1
 Summary: Argo-Workflow backend extension for Jupyter-Scheduler.
 Project-URL: Documentation, https://github.com/nebari-dev/argo-jupyter-scheduler#readme
 Project-URL: Issues, https://github.com/nebari-dev/argo-jupyter-scheduler/issues
 Project-URL: Source, https://github.com/nebari-dev/argo-jupyter-scheduler
 Author-email: iameskild <eeriksen@quansight.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -45,15 +45,14 @@
   - [Installation](#installation)
   - [What is it?](#what-is-it)
   - [A deeper dive](#a-deeper-dive)
     - [`Job`](#job)
     - [`Job Definition`](#job-definition)
     - [Internals](#internals)
   - [Additional thoughts](#additional-thoughts)
-  - [Known issues](#known-issues)
   - [License](#license)
 
 **Argo-Jupyter-Scheduler**
 
 Submit longing running notebooks to run without the need to keep your JupyterLab server running. And submit a notebook to run on a specified schedule.
 
 ## Installation
@@ -125,14 +124,11 @@
 And when a job definition is created, a corresponding cron-workflow is created. To ensure the database is properly updated, the workflow that the cron-workflow creates has three steps. First, create a job record in the database with a status of `IN PROGRESS`. Second, run the notebook, again using `papermill` and the conda environment specified. And third, update the newly created job record with the status of the notebook run.
 
 
 ## Additional Thoughts
 
 At the moment, Argo-Jupyter-Scheduler is closely coupled with Nebari (via the Nebari-Workflow-Controller) which doesn't make it very useable for other projects. There's no need for this to necessarily be the case. By leveraging Traitlets, we can include other ways of modifying the pod spec for the running workflow and enable it to be used by other projects. If you're interested in this project and would like to see it extended, feel free to open an issue to discuss your ideas. Thank you :)
 
-## Known Issues
-
-All of the core features of Jupyter-Scheduler have been mapped over to Argo-Jupyter-Scheduler. Unfortunately, there is currently a limitation with `Update Job Definition` and with `Pause`/`Resume` for Job Definitions. Although the `Pause` works, the `Resume` fails for the same reason `Update Job Definition` does and this is because the upstream Nebari-Workflow-Controller (see [Known Limitations](https://github.com/nebari-dev/nebari-workflow-controller#known-limitations)) has a limitation whereby it can't resubmit workflows/cron-workflows; there are more details in [this issue](https://github.com/nebari-dev/nebari-workflow-controller/issues/18).
 
 ## License
 
 `argo-jupyter-scheduler` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

