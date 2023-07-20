# Comparing `tmp/argo_jupyter_scheduler-0.1.0.dev1.tar.gz` & `tmp/argo_jupyter_scheduler-2023.7.1rc1.tar.gz`

## Comparing `argo_jupyter_scheduler-0.1.0.dev1.tar` & `argo_jupyter_scheduler-2023.7.1rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/.github/workflows/tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/_version.py
--rw-r--r--   0        0        0    18434 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/executor.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/tests/conftest.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/tests/test_scheduler.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/tests/test_utils.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/LICENSE.txt
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 argo_jupyter_scheduler-0.1.0.dev1/PKG-INFO
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

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/.github/workflows/release.yml` & `argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/.github/workflows/tests.yml` & `argo_jupyter_scheduler-2023.7.1rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/executor.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Dict, Union
 
 from hera.workflows import Container, CronWorkflow, Env, Step, Steps, Workflow, script
-from hera.workflows.models import ContinueOn, WorkflowStopRequest
+from hera.workflows.models import ContinueOn, TTLStrategy, WorkflowStopRequest
 from hera.workflows.service import WorkflowsService
 from jupyter_scheduler.executors import ExecutionManager
 from jupyter_scheduler.models import (
     CreateJob,
     DescribeJob,
     DescribeJobDefinition,
     JobFeature,
@@ -23,14 +23,16 @@
     gen_workflow_name,
     sanitize_label,
     setup_logger,
 )
 
 logger = setup_logger(__name__)
 
+DEFAULT_TTL = 600
+
 
 class ArgoExecutor(ExecutionManager):
     def __init__(
         self,
         action: str,
         db_url: str,
         root_dir: Union[str, None] = None,
@@ -85,17 +87,17 @@
 
     def execute(self):
         model = self.model
 
         if self.job_id:
             if self.action == WorkflowActionsEnum.create:
                 self.create_workflow(
-                    model,
-                    self.parameters,
-                    self.staging_paths,
+                    job=model,
+                    parameters=self.parameters,
+                    staging_paths=self.staging_paths,
                     db_url=self.db_url,
                     use_conda_store_env=self.use_conda_store_env,
                 )
 
             elif self.action == WorkflowActionsEnum.delete:
                 self.delete_workflow(self.job_id)
 
@@ -115,20 +117,20 @@
                     schedule=self.schedule,
                     timezone=self.timezone,
                     db_url=self.db_url,
                     use_conda_store_env=self.use_conda_store_env,
                 )
             elif self.action == WorkflowActionsEnum.update:
                 self.update_cron_workflow(
-                    model,
-                    self.staging_paths,
-                    self.job_definition_id,
-                    self.schedule,
-                    self.timezone,
-                    self.active,
+                    job=model,
+                    staging_paths=self.staging_paths,
+                    job_definition_id=self.job_definition_id,
+                    schedule=self.schedule,
+                    timezone=self.timezone,
+                    active=self.active,
                     db_url=self.db_url,
                     use_conda_store_env=self.use_conda_store_env,
                 )
 
             elif self.action == WorkflowActionsEnum.delete:
                 self.delete_cron_workflow(self.job_definition_id)
 
@@ -206,35 +208,41 @@
         main = Container(
             name="main",
             command=["/bin/sh"],
             args=cmd_args,
             env=envs,
         )
 
+        ttl_strategy = TTLStrategy(
+            seconds_after_completion=DEFAULT_TTL,
+            seconds_after_success=DEFAULT_TTL,
+            seconds_after_failure=DEFAULT_TTL,
+        )
+
         failure = "{{steps.main.status}} == Failed"
         successful = "{{steps.main.status}} == Succeeded"
 
         with Workflow(
-            name=gen_workflow_name(job.job_id), entrypoint="steps", labels=labels
+            name=gen_workflow_name(job.job_id),
+            entrypoint="steps",
+            labels=labels,
+            ttl_strategy=ttl_strategy,
         ) as w:
-            main_step = Step(
-                name="main", template=main, continue_on=ContinueOn(failed=True)
-            )
-            failure_script = update_job_status_failure(
-                name="failure",
-                arguments={"db_url": db_url, "job_id": job.job_id},
-                when=failure,
-            )
-            success_script = update_job_status_success(
-                name="success",
-                arguments={"db_url": db_url, "job_id": job.job_id},
-                when=successful,
-            )
-
-            Steps(name="steps", sub_steps=[main_step, failure_script, success_script])
+            with Steps(name="steps"):
+                Step(name="main", template=main, continue_on=ContinueOn(failed=True))
+                update_job_status_failure(
+                    name="failure",
+                    arguments={"db_url": db_url, "job_id": job.job_id},
+                    when=failure,
+                )
+                update_job_status_success(
+                    name="success",
+                    arguments={"db_url": db_url, "job_id": job.job_id},
+                    when=successful,
+                )
 
         w.create()
 
         logger.info("workflow created")
 
     def delete_workflow(self, job_id: str):
         global_config = authenticate()
@@ -319,14 +327,19 @@
 
         main = Container(
             name="main",
             command=["/bin/sh"],
             args=cmd_args,
             env=envs,
         )
+        ttl_strategy = TTLStrategy(
+            seconds_after_completion=DEFAULT_TTL,
+            seconds_after_success=DEFAULT_TTL,
+            seconds_after_failure=DEFAULT_TTL,
+        )
 
         # mimics internals of the `scheduler.create_job_from_definition` method
         attributes = {
             **job.dict(exclude={"schedule", "timezone"}, exclude_none=True),
             "input_uri": staging_paths["input"],
         }
         model = CreateJob(**attributes)
@@ -341,46 +354,42 @@
             timezone=timezone,
             starting_deadline_seconds=0,
             concurrency_policy="Replace",
             successful_jobs_history_limit=4,
             failed_jobs_history_limit=4,
             cron_suspend=suspend,
             labels=labels,
+            ttl_strategy=ttl_strategy,
         ) as cwf:
-            create_job_record_script = create_job_record(
-                name="create-job-id",
-                arguments={
-                    "model": model,
-                    "db_url": db_url,
-                    "job_definition_id": job_definition_id,
-                },
-            )
-            main_step = Step(
-                name="main", template=main, continue_on=ContinueOn(failed=True)
-            )
-            failure_script = update_job_status_failure(
-                name="failure",
-                arguments={"db_url": db_url, "job_definition_id": job_definition_id},
-                when=failure,
-            )
-            success_script = update_job_status_success(
-                name="success",
-                arguments={"db_url": db_url, "job_definition_id": job_definition_id},
-                when=successful,
-            )
-
-            Steps(
-                name="steps",
-                sub_steps=[
-                    create_job_record_script,
-                    main_step,
-                    failure_script,
-                    success_script,
-                ],
-            )
+            with Steps(name="steps"):
+                create_job_record(
+                    name="create-job-id",
+                    arguments={
+                        "model": model,
+                        "db_url": db_url,
+                        "job_definition_id": job_definition_id,
+                    },
+                )
+                Step(name="main", template=main, continue_on=ContinueOn(failed=True))
+                update_job_status_failure(
+                    name="failure",
+                    arguments={
+                        "db_url": db_url,
+                        "job_definition_id": job_definition_id,
+                    },
+                    when=failure,
+                )
+                update_job_status_success(
+                    name="success",
+                    arguments={
+                        "db_url": db_url,
+                        "job_definition_id": job_definition_id,
+                    },
+                    when=successful,
+                )
 
         return cwf
 
     def create_cron_workflow(
         self,
         job: DescribeJobDefinition,
         staging_paths: Dict,
```

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/scheduler.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/task_runner.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/argo_jupyter_scheduler/utils.py` & `argo_jupyter_scheduler-2023.7.1rc1/argo_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/tests/conftest.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/tests/test_scheduler.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/tests/test_utils.py` & `argo_jupyter_scheduler-2023.7.1rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/.gitignore` & `argo_jupyter_scheduler-2023.7.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/LICENSE.txt` & `argo_jupyter_scheduler-2023.7.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/README.md` & `argo_jupyter_scheduler-2023.7.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/pyproject.toml` & `argo_jupyter_scheduler-2023.7.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argo_jupyter_scheduler-0.1.0.dev1/PKG-INFO` & `argo_jupyter_scheduler-2023.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argo-jupyter-scheduler
-Version: 0.1.0.dev1
+Version: 2023.7.1rc1
 Summary: Argo-Workflow backend extension for Jupyter-Scheduler.
 Project-URL: Documentation, https://github.com/nebari-dev/argo-jupyter-scheduler#readme
 Project-URL: Issues, https://github.com/nebari-dev/argo-jupyter-scheduler/issues
 Project-URL: Source, https://github.com/nebari-dev/argo-jupyter-scheduler
 Author-email: iameskild <eeriksen@quansight.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

