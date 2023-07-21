# Comparing `tmp/promptquality-0.2.0.tar.gz` & `tmp/promptquality-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.2.0.tar", max compression
+gzip compressed data, was "promptquality-0.2.1.tar", max compression
```

## Comparing `promptquality-0.2.0.tar` & `promptquality-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10946 2023-07-18 19:54:59.658617 promptquality-0.2.0/LICENSE
--rw-r--r--   0        0        0      157 2023-07-18 19:54:59.658617 promptquality-0.2.0/README.md
--rw-r--r--   0        0        0     1463 2023-07-18 19:54:59.658617 promptquality-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      394 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/__init__.py
--rw-r--r--   0        0        0      545 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/config.py
--rw-r--r--   0        0        0        0 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/__init__.py
--rw-r--r--   0        0        0      353 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/config.py
--rw-r--r--   0        0        0       80 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/integrations.py
--rw-r--r--   0        0        0      172 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/job.py
--rw-r--r--   0        0        0      618 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/routes.py
--rw-r--r--   0        0        0      150 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/constants/run.py
--rw-r--r--   0        0        0     1836 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/get_metrics.py
--rw-r--r--   0        0        0     4584 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/helpers.py
--rw-r--r--   0        0        0      539 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/integrations.py
--rw-r--r--   0        0        0     1060 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/job_progress.py
--rw-r--r--   0        0        0      462 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/login.py
--rw-r--r--   0        0        0     1515 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/run.py
--rw-r--r--   0        0        0        0 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/types/__init__.py
--rw-r--r--   0        0        0     7068 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/types/config.py
--rw-r--r--   0        0        0     3619 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/types/run.py
--rw-r--r--   0        0        0      474 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/types/settings.py
--rw-r--r--   0        0        0        0 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/__init__.py
--rw-r--r--   0        0        0     4460 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/api_client.py
--rw-r--r--   0        0        0      911 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/config.py
--rw-r--r--   0        0        0       60 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/logger.py
--rw-r--r--   0        0        0    24261 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/name.py
--rw-r--r--   0        0        0     1625 2023-07-18 19:54:59.658617 promptquality-0.2.0/src/promptquality/utils/request.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-07-21 00:13:07.454901 promptquality-0.2.1/LICENSE
+-rw-r--r--   0        0        0      157 2023-07-21 00:13:07.454901 promptquality-0.2.1/README.md
+-rw-r--r--   0        0        0     1543 2023-07-21 00:13:07.454901 promptquality-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      398 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0       80 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/integrations.py
+-rw-r--r--   0        0        0      172 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/job.py
+-rw-r--r--   0        0        0      618 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      150 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0     1840 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0     4588 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/helpers.py
+-rw-r--r--   0        0        0      543 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/integrations.py
+-rw-r--r--   0        0        0     1060 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      466 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/login.py
+-rw-r--r--   0        0        0     1603 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/run.py
+-rw-r--r--   0        0        0     1019 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/set_config.py
+-rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7781 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/config.py
+-rw-r--r--   0        0        0     3619 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/run.py
+-rw-r--r--   0        0        0      474 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/settings.py
+-rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     4460 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0      838 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/config.py
+-rw-r--r--   0        0        0       60 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24261 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.1/PKG-INFO
```

### Comparing `promptquality-0.2.0/LICENSE` & `promptquality-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/pyproject.toml` & `promptquality-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptquality"
-version = "0.2.0"
+version = "0.2.1"
 description = "🦸 Supercharge your prompts with Galileo's Prompt Inspector!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 requests = "^2.31.0"
@@ -22,14 +22,15 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 types-requests = "^2.31.0.1"
 pydantic = {extras = ["mypy"], version = "^2.0.2"}
 types-tqdm = "^4.65.0.1"
+pytest-socket = "^0.6.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Test.
@@ -42,14 +43,16 @@
     "--showlocals",
     # Show extra test summary info as specified by chars.
     "-o", "console_output_style=progress",
     # Disable warnings.
     "--disable-warnings",
     # Show slowest 10 test durations.
     "--durations=10",
+    # Disable internet access.
+    "--disable-socket",
 ]
 
 # Formatters.
 [tool.black]
 line-length = 88
 
 [tool.isort]
```

### Comparing `promptquality-0.2.0/src/promptquality/constants/routes.py` & `promptquality-0.2.1/src/promptquality/constants/routes.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/src/promptquality/get_metrics.py` & `promptquality-0.2.1/src/promptquality/get_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from pydantic import UUID4
 
-from promptquality.config import set_config
 from promptquality.constants.job import JobStatus
 from promptquality.helpers import get_job_status
+from promptquality.set_config import set_config
 from promptquality.types.config import Config
 from promptquality.types.run import GetMetricsRequest, PromptMetrics
 
 
 def get_metrics(
     project_id: Optional[UUID4] = None,
     run_id: Optional[UUID4] = None,
```

### Comparing `promptquality-0.2.0/src/promptquality/helpers.py` & `promptquality-0.2.1/src/promptquality/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import UUID4
 
-from promptquality.config import set_config
+from promptquality.set_config import set_config
 from promptquality.types.config import Config
 from promptquality.types.run import (
     CreateJobRequest,
     CreateJobResponse,
     CreateProjectRequest,
     CreateProjectResponse,
     CreateRunRequest,
```

### Comparing `promptquality-0.2.0/src/promptquality/integrations.py` & `promptquality-0.2.1/src/promptquality/integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from pydantic import SecretStr
 
-from promptquality.config import set_config
+from promptquality.set_config import set_config
 from promptquality.types.config import Config
 from promptquality.types.run import CreateIntegrationRequest
 
 
 def add_openai_integration(
     api_key: str, organization_id: Optional[str] = None, config: Optional[Config] = None
 ) -> None:
```

### Comparing `promptquality-0.2.0/src/promptquality/job_progress.py` & `promptquality-0.2.1/src/promptquality/job_progress.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     job_progress_bar = tqdm(
         total=job_status.steps_total,
         position=0,
         leave=True,
         desc=job_status.progress_message,
     )
     while job_status.status in [JobStatus.unstarted, JobStatus.in_progress]:
+        sleep(backoff)
         job_status = get_job_status(job_id, config)
         job_progress_bar.set_description(job_status.progress_message)
         job_progress_bar.update(job_status.steps_completed - job_progress_bar.n)
-        sleep(backoff)
         backoff *= 2
     job_progress_bar.close()
     logger.debug(f"Job {job_id} status: {job_status.status}.")
     return job_status.id
```

### Comparing `promptquality-0.2.0/src/promptquality/run.py` & `promptquality-0.2.1/src/promptquality/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 from typing import Optional
 
-from promptquality.config import set_config
 from promptquality.get_metrics import get_metrics
 from promptquality.helpers import (
     create_job,
     create_project,
     create_run,
     create_template,
     upload_dataset,
 )
 from promptquality.job_progress import job_progress
+from promptquality.set_config import set_config
 from promptquality.types.run import PromptMetrics
 from promptquality.types.settings import Settings
 
 
 def run(
     template: str,
     dataset: Path,
@@ -53,11 +53,12 @@
         dataset_id,
         template_version_id,
         settings,
         config,
     )
     if wait:
         job_progress(job_id, config)
+    print(f"🔭 View your prompt run on the Galileo console at: {config.run_url}")
     metrics = get_metrics(
         project_id=project_id, run_id=run_id, job_id=job_id, config=config
     )
     return metrics
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `promptquality-0.2.0/src/promptquality/types/config.py` & `promptquality-0.2.1/src/promptquality/types/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from getpass import getpass
 from pathlib import Path
+from posixpath import join
 from typing import Optional
-from urllib.parse import urljoin
+from urllib.parse import urlencode, urljoin
 from webbrowser import open_new_tab
 
 from pydantic import (
     UUID4,
     HttpUrl,
     SecretStr,
     ValidationError,
@@ -14,14 +15,15 @@
     field_validator,
     model_validator,
 )
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from promptquality.constants.config import ConfigDefaults
 from promptquality.constants.routes import Routes
+from promptquality.constants.run import RunDefaults
 from promptquality.types.run import (
     CreateJobResponse,
     CreateProjectResponse,
     CreatePromptTemplateVersionResponse,
     CreateRunResponse,
     CreateTemplateResponse,
     UploadDatasetResponse,
@@ -102,14 +104,34 @@
         return cls.model_validate_json(_config_location().read_text())
 
     def write(self) -> None:
         self.config_file.parent.mkdir(exist_ok=True)
         self.config_file.write_text(self.model_dump_json(exclude_none=True))
 
     @property
+    def run_url(self) -> str:
+        if not self.current_project_id:
+            raise ValueError("No project set.")
+        if not self.current_run_id:
+            raise ValueError("No run set.")
+        query_params = urlencode(
+            {
+                "projectId": self.current_project_id,
+                "runId": self.current_run_id,
+                "taskType": RunDefaults.task_type,
+            }
+        )
+        return join(
+            self.console_url.unicode_string(),
+            "prompt-evaluation",
+            # Open the prompts page.
+            f"prompts?{query_params}",
+        )
+
+    @property
     def api_client(self) -> ApiClient:
         if not self.token:
             raise ValueError("No token set.")
         return ApiClient(api_url=self.api_url, token=self.token)
 
     def token_login(self) -> str:
         token_url = urljoin(str(self.console_url), Routes.get_token)
```

### Comparing `promptquality-0.2.0/src/promptquality/types/run.py` & `promptquality-0.2.1/src/promptquality/types/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/src/promptquality/utils/api_client.py` & `promptquality-0.2.1/src/promptquality/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/src/promptquality/utils/config.py` & `promptquality-0.2.1/src/promptquality/utils/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,11 +15,9 @@
 
     You can also set GALILEO_CONSOLE_URL before importing promptquality to bypass this
 
     :param console_url: If set, that will be used. Otherwise, if an environment variable
     GALILEO_CONSOLE_URL is set, that will be used. Otherwise, you will be prompted for
     a url.
     """
-    if not console_url:
-        console_url = ConfigDefaults.console_url
     if getenv(ConfigEnvironmentVariables.console_url, None) is None:
         environ[ConfigEnvironmentVariables.console_url] = console_url
```

### Comparing `promptquality-0.2.0/src/promptquality/utils/name.py` & `promptquality-0.2.1/src/promptquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/src/promptquality/utils/request.py` & `promptquality-0.2.1/src/promptquality/utils/request.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.0/PKG-INFO` & `promptquality-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptquality
-Version: 0.2.0
+Version: 0.2.1
 Summary: 🦸 Supercharge your prompts with Galileo's Prompt Inspector!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

