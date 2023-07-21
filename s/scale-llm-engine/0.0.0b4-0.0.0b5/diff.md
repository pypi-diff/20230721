# Comparing `tmp/scale_llm_engine-0.0.0b4.tar.gz` & `tmp/scale_llm_engine-0.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b4.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b5.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b4.tar` & `scale_llm_engine-0.0.0b5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1002 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/README.md
--rw-r--r--   0        0        0     1576 2023-07-20 17:29:36.022438 scale_llm_engine-0.0.0b4/llmengine/__init__.py
--rw-r--r--   0        0        0     6190 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/api_engine.py
--rw-r--r--   0        0        0    13065 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/completion.py
--rw-r--r--   0        0        0    13090 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/errors.py
--rw-r--r--   0        0        0    13905 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/fine_tuning.py
--rw-r--r--   0        0        0    13738 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-20 17:29:35.126426 scale_llm_engine-0.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-19 01:36:28.535119 scale_llm_engine-0.0.0b5/README.md
+-rw-r--r--   0        0        0     1576 2023-07-21 01:19:40.651366 scale_llm_engine-0.0.0b5/llmengine/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-19 23:57:12.780752 scale_llm_engine-0.0.0b5/llmengine/api_engine.py
+-rw-r--r--   0        0        0    13065 2023-07-19 01:36:28.535834 scale_llm_engine-0.0.0b5/llmengine/completion.py
+-rw-r--r--   0        0        0    13457 2023-07-20 18:43:29.437750 scale_llm_engine-0.0.0b5/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-16 23:34:18.820164 scale_llm_engine-0.0.0b5/llmengine/errors.py
+-rw-r--r--   0        0        0    14021 2023-07-20 18:43:29.438456 scale_llm_engine-0.0.0b5/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    13738 2023-07-19 17:53:11.210172 scale_llm_engine-0.0.0b5/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-21 01:19:40.652418 scale_llm_engine-0.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b5/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b4/README.md` & `scale_llm_engine-0.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b4/llmengine/__init__.py` & `scale_llm_engine-0.0.0b5/llmengine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta4"
+__version__ = "0.0.0.beta5"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
```

### Comparing `scale_llm_engine-0.0.0b4/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b5/llmengine/api_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from functools import wraps
 from typing import Any, AsyncIterable, Dict, Iterator, Optional
 
 import requests
 from aiohttp import ClientSession, ClientTimeout
 from llmengine.errors import parse_error
 
-SCALE_API_KEY = os.getenv("SCALE_API_KEY")
 SPELLBOOK_API_URL = "https://api.spellbook.scale.com"
 LLM_ENGINE_BASE_PATH = os.getenv("LLM_ENGINE_BASE_PATH", SPELLBOOK_API_URL)
 DEFAULT_TIMEOUT: int = 10
 
 
 def get_api_key() -> str:
-    return SCALE_API_KEY or "root"
+    env_api_key = os.getenv("SCALE_API_KEY")
+    return env_api_key or "root"
 
 
 def assert_self_hosted(func):
     @wraps(func)
     def inner(*args, **kwargs):
         if SPELLBOOK_API_URL == LLM_ENGINE_BASE_PATH:
             raise ValueError("This feature is only available for self-hosted users.")
@@ -28,15 +28,15 @@
 
     return inner
 
 
 class APIEngine:
     @classmethod
     def validate_api_key(cls):
-        if SPELLBOOK_API_URL == LLM_ENGINE_BASE_PATH and not SCALE_API_KEY:
+        if SPELLBOOK_API_URL == LLM_ENGINE_BASE_PATH and not get_api_key():
             raise ValueError(
                 "You must set SCALE_API_KEY in your environment to to use the LLM Engine API."
             )
 
     @classmethod
     def _get(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
```

### Comparing `scale_llm_engine-0.0.0b4/llmengine/completion.py` & `scale_llm_engine-0.0.0b5/llmengine/completion.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b4/llmengine/data_types.py` & `scale_llm_engine-0.0.0b5/llmengine/data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -377,14 +377,24 @@
     """
 
     fine_tune_id: str = Field(..., description="ID of the requested job.")
     """
     The ID of the FineTune.
     """
 
+    fine_tuned_model: Optional[str] = Field(
+        default=None,
+        description="Name of the resulting fine-tuned model. This can be plugged into the "
+        "Completion API once the fine-tune is complete",
+    )
+    """
+    The name of the resulting fine-tuned model. This can be plugged into the Completion API
+    once the fine-tune is complete.
+    """
+
     status: BatchJobStatus = Field(..., description="Status of the requested job.")
     """
     The status of the FineTune job.
     """
 
 
 class ListFineTunesResponse(BaseModel):
```

### Comparing `scale_llm_engine-0.0.0b4/llmengine/errors.py` & `scale_llm_engine-0.0.0b5/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b4/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b5/llmengine/fine_tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         and several hours for larger ones.
 
         Args:
             model (`str`):
                 The name of the base model to fine-tune. See [Model Zoo](../../model_zoo) for the list of available models to fine-tune.
 
             training_file (`str`):
-                Publicly accessible URL to a CSV file for training.
+                Publicly accessible URL to a CSV file for training. When no validation_file is provided, one will automatically be created using a 10% split of the training_file data.
 
             validation_file (`Optional[str]`):
                 Publicly accessible URL to a CSV file for validation. The validation file is used to compute metrics which let LLM Engine pick the best fine-tuned checkpoint, which will be used for inference when fine-tuning is complete.
 
             hyperparameters (`Optional[Dict[str, str]]`):
                 A dict of hyperparameters to customize fine-tuning behavior.
```

### Comparing `scale_llm_engine-0.0.0b4/llmengine/model.py` & `scale_llm_engine-0.0.0b5/llmengine/model.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b4/pyproject.toml` & `scale_llm_engine-0.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta4"
+version = "0.0.0.beta5"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b4/PKG-INFO` & `scale_llm_engine-0.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b4
+Version: 0.0.0b5
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

