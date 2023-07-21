# Comparing `tmp/trapi_predict_kit-0.1.0.tar.gz` & `tmp/trapi_predict_kit-0.1.2.tar.gz`

## Comparing `trapi_predict_kit-0.1.0.tar` & `trapi_predict_kit-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,42 @@
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/CITATION.cff
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/config.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/decorators.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/loaded_model.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/predict_output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/py.typed
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/rdf_utils.py
--rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/trapi.py
--rw-r--r--   0        0        0    20125 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/trapi_parser.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/src/trapi_predict_kit/utils.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/tests/dev.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/tests/test_decorator.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/README.md
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/CITATION.cff
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0    62025 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/OpenPREDICT_datamodel.jpg
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/README.md
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/index.md
+-rw-r--r--   0        0        0    27224 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/openpredict-examples.ipynb
+-rw-r--r--   0        0        0   156773 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/openpredict-pyrdf2vec-embeddings.ipynb
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/query-ars.ipynb
+-rw-r--r--   0        0        0   326036 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/assets/FAIR_data_principles.png
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/assets/custom.css
+-rw-r--r--   0        0        0    54454 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/assets/fontawesome.min.js
+-rw-r--r--   0        0        0    27832 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/assets/icon.png
+-rw-r--r--   0        0        0  1065598 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/assets/solid.min.js
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/getting-started/create-model.md
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/getting-started/create-project.md
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/getting-started/deploy-api.md
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/getting-started/development.md
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/openpredict-api/deploy.md
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/openpredict-api/introduction.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/docs/reference/trapi.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/config.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/decorators.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/loaded_model.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/normalize.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/predict_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/py.typed
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/rdf_utils.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/trapi.py
+-rw-r--r--   0        0        0    20309 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/trapi_parser.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/src/trapi_predict_kit/utils.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/tests/dev.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/tests/test_decorator.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/README.md
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 trapi_predict_kit-0.1.2/PKG-INFO
```

### Comparing `trapi_predict_kit-0.1.0/.github/workflows/publish.yml` & `trapi_predict_kit-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/decorators.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import functools
-from typing import Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 
 from reasoner_pydantic import MetaEdge, MetaNode
 
 from trapi_predict_kit.predict_output import PredictOptions
 
 
 def trapi_predict(
     path: str,
     edges: List[MetaEdge],
     nodes: Dict[str, MetaNode],
     name: Optional[str] = None,
     description: Optional[str] = "",
     default_input: Optional[str] = "drugbank:DB00394",
     default_model: Optional[str] = "openpredict_baseline",
-):
+) -> Callable:
     """A decorator to indicate a function is a function to generate prediction that can be integrated to TRAPI.
     The function needs to take an input_id and returns a list of predicted entities related to the input entity
     """
     if not name:
         name = path
 
-    def decorator(func):
+    def decorator(func: Callable) -> Any:
         @functools.wraps(func)
-        def wrapper(input_id: str, options: Optional[PredictOptions] = None):
+        def wrapper(input_id: str, options: Optional[PredictOptions] = None) -> Callable:
             options = PredictOptions.parse_obj(options) if options else PredictOptions()
             return func(input_id, options)
 
         wrapper._trapi_predict = {
             "edges": edges,
             "nodes": nodes,
             "path": path,
```

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/loaded_model.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/loaded_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,14 @@
     mlem.save(model, path, sample_data=sample_data)
 
     g = get_run_metadata(scores, sample_data, hyper_params, model_name)
     g.serialize(f"{path}.ttl", format="ttl")
     # os.chmod(f"{path}.ttl", 0o644)
     # os.chmod(f"{path}.mlem", 0o644)
 
-    # TODO: generate and store RDF metadata
-    # return path
     return LoadedModel(
         path=path,
         model=model,
         metadata=g,
         hyper_params=hyper_params,
         scores=scores,
     )
```

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/predict_output.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/predict_output.py`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/rdf_utils.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/trapi.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/trapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import time
 from typing import Any, Callable, Dict, List, Optional
 
 from fastapi import Body, FastAPI, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import JSONResponse, RedirectResponse
@@ -23,15 +24,17 @@
 class TRAPI(FastAPI):
     """Translator Reasoner API - wrapper for FastAPI."""
 
     def __init__(
         self,
         *args: Any,
         predict_endpoints: List[Callable],
-        servers: Optional[List[Dict[str, str]]] = None,
+        ordered_servers: Optional[List[Dict[str, str]]] = None,
+        itrb_url_prefix: Optional[str] = None,
+        dev_server_url: Optional[str] = None,
         info: Optional[Dict[str, Any]] = None,
         title="Translator Reasoner API",
         version="1.0.0",
         openapi_version="3.0.1",
         description="""Get predicted targets for a given entity
 \n\nService supported by the [NCATS Translator project](https://ncats.nih.gov/translator/about)""",
         **kwargs: Any,
@@ -41,18 +44,61 @@
             title=title,
             version=version,
             openapi_version=openapi_version,
             description=description,
             root_path_in_servers=False,
             **kwargs,
         )
-        self.servers = servers
         self.predict_endpoints = predict_endpoints
         self.info = info
 
+        # On ITRB deployment and local dev we directly use the current server
+        self.servers = []
+
+        # For the API deployed on our server and registered to SmartAPI we provide the complete list
+        if os.getenv("VIRTUAL_HOST"):
+            if itrb_url_prefix:
+                self.servers.append(
+                    {
+                        "url": f"https://{itrb_url_prefix}.transltr.io",
+                        "description": "TRAPI ITRB Production Server",
+                        "x-maturity": "production",
+                    }
+                )
+                self.servers.append(
+                    {
+                        "url": f"https://{itrb_url_prefix}.test.transltr.io",
+                        "description": "TRAPI ITRB Test Server",
+                        "x-maturity": "testing",
+                    }
+                )
+                self.servers.append(
+                    {
+                        "url": f"https://{itrb_url_prefix}.ci.transltr.io",
+                        "description": "TRAPI ITRB CI Server",
+                        "x-maturity": "staging",
+                    }
+                )
+            if dev_server_url:
+                self.servers.append(
+                    {"url": dev_server_url, "description": "TRAPI Dev Server", "x-maturity": "development"}
+                )
+
+            ordered_servers = []
+            # Add the current server as 1st server in the list
+            for server in self.servers:
+                if os.getenv("VIRTUAL_HOST") in server["url"]:
+                    ordered_servers.append(server)
+                    break
+            # Add other servers
+            for server in self.servers:
+                if os.getenv("VIRTUAL_HOST") not in server["url"]:
+                    ordered_servers.append(server)
+            self.servers = ordered_servers
+
         self.add_middleware(
             CORSMiddleware,
             allow_origins=["*"],
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
         )
@@ -108,15 +154,15 @@
     "query_options": { "n_results": 5 }
 }
 ```
         """,
             response_model=Query,
             tags=["reasoner"],
         )
-        def post_reasoner_predict(request_body: Query = Body(..., example=trapi_example)) -> Query:
+        def post_reasoner_predict(request_body: Query = Body(..., examples=[trapi_example])) -> Query:
             """Get predicted associations for a given ReasonerAPI query.
 
             :param request_body: The ReasonerStdAPI query in JSON
             :return: Predictions as a ReasonerStdAPI Message
             """
             query_graph = request_body.message.query_graph.dict(exclude_none=True)
```

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/trapi_parser.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/trapi_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,21 +260,21 @@
                                     ],
                                     "attributes": [
                                         {
                                             "description": "model_id",
                                             "attribute_type_id": "EDAM:data_1048",
                                             "value": model_id_label,
                                         },
-                                        {
-                                            # TODO: use has_confidence_level?
-                                            "description": "score",
-                                            "attribute_type_id": "EDAM:data_1772",
-                                            "value": association_score
-                                            # https://www.ebi.ac.uk/ols/ontologies/edam/terms?iri=http%3A%2F%2Fedamontology.org%2Fdata_1772&viewMode=All&siblings=false
-                                        },
+                                        # {
+                                        #     # TODO: use has_confidence_level?
+                                        #     "description": "score",
+                                        #     "attribute_type_id": "EDAM:data_1772",
+                                        #     "value": association_score
+                                        #     # https://www.ebi.ac.uk/ols/ontologies/edam/terms?iri=http%3A%2F%2Fedamontology.org%2Fdata_1772&viewMode=All&siblings=false
+                                        # },
                                         # https://github.com/NCATSTranslator/ReasonerAPI/blob/1.4/ImplementationGuidance/Specifications/knowledge_level_agent_type_specification.md
                                         {
                                             "attribute_type_id": "biolink:agent_type",
                                             "value": "computational_model",
                                             "attribute_source": "infores:openpredict",
                                         },
                                         {
@@ -302,14 +302,16 @@
 
                                 # Add the bindings to the results object
                                 result = {
                                     "node_bindings": {},
                                     "analyses": [
                                         {
                                             "resource_id": "infores:openpredict",
+                                            "score": association_score,
+                                            "scoring_method": "Model confidence between 0 and 1",
                                             "edge_bindings": {edge_qg_id: [{"id": edge_kg_id}]},
                                         }
                                     ],
                                     # 'edge_bindings': {},
                                 }
                                 # result['edge_bindings'][edge_qg_id] = [
                                 #     {
```

### Comparing `trapi_predict_kit-0.1.0/src/trapi_predict_kit/utils.py` & `trapi_predict_kit-0.1.2/src/trapi_predict_kit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 log.setLevel(log_level)
 console_handler = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s %(levelname)s: [%(module)s:%(funcName)s] %(message)s")
 console_handler.setFormatter(formatter)
 log.addHandler(console_handler)
 
 
-def get_openpredict_dir(subfolder=""):
+def get_openpredict_dir(subfolder: str = "") -> str:
     """Return the full path to the provided files in the OpenPredict data folder
     Where models and features for runs are stored
     """
     if not settings.OPENPREDICT_DATA_DIR.endswith("/"):
         settings.OPENPREDICT_DATA_DIR += "/"
     return settings.OPENPREDICT_DATA_DIR + subfolder
 
 
-def init_openpredict_dir():
+def init_openpredict_dir() -> None:
     """Create OpenPredict folder and initiate files if necessary."""
     if not os.path.exists(get_openpredict_dir("input/drugbank-drug-goa.csv")):
         raise ValueError(
             "❌ The data required to run the prediction models could not be found in the `data` folder"
             "i️ Use `pip install dvc` and `dvc pull` to pull the data easily"
         )
```

### Comparing `trapi_predict_kit-0.1.0/tests/dev.py` & `trapi_predict_kit-0.1.2/tests/dev.py`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/tests/test_decorator.py` & `trapi_predict_kit-0.1.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/LICENSE.txt` & `trapi_predict_kit-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trapi_predict_kit-0.1.0/README.md` & `trapi_predict_kit-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 <div align="center">
 
 # 🪄 TRAPI Predict Kit
 
-<!--
-
 [![PyPI - Version](https://img.shields.io/pypi/v/trapi-predict-kit.svg?logo=pypi&label=PyPI&logoColor=silver)](https://pypi.org/project/trapi-predict-kit/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/trapi-predict-kit.svg?logo=python&label=Python&logoColor=silver)](https://pypi.org/project/trapi-predict-kit/)
 [![license](https://img.shields.io/pypi/l/trapi-predict-kit.svg?color=%2334D058)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/blob/main/LICENSE.txt)
 [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
--->
 
 [![Test package](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/test.yml/badge.svg)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/test.yml)
 [![Publish package](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/publish.yml/badge.svg)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/publish.yml)
 
 </div>
 
 A package to help create and deploy Translator Reasoner APIs (TRAPI) from any prediction model exposed as a regular python function.
 
+The **TRAPI Predict Kit** helps data scientists to build, and **publish prediction models** in a [FAIR](https://www.go-fair.org/fair-principles/) and reproducible manner. It provides helpers for various steps of the process:
+
+* A template to help user quickly bootstrap a new prediction project with the recommended structure ([MaastrichtU-IDS/cookiecutter-trapi-predict-kit](https://github.com/MaastrichtU-IDS/cookiecutter-trapi-predict-kit/))
+* Helper function to easily save a generated model, its metadata, and the data used to generate it. It uses tools such as [`dvc`](https://dvc.org/) and [`mlem`](https://mlem.ai/) to store large model outside of the git repository.
+* Deploy API endpoints for retrieving predictions, which comply with the NCATS Biomedical Data Translator standards ([Translator Reasoner API](https://github.com/NCATSTranslator/ReasonerAPI) and [BioLink model](https://github.com/biolink/biolink-model)), using a decorator `@trapi_predict` to simply annotate the function that produces predicted associations for a given input entity
+
+Predictions are usually generated from machine learning models (e.g. predict disease treated by drug), but it can adapt to generic python function, as long as the input params and return object follow the expected structure.
+
+Checkout the documentation website at **[maastrichtu-ids.github.io/trapi-predict-kit](https://maastrichtu-ids.github.io/trapi-predict-kit)** for more details.
+
 ## 📦️ Installation
 
 This package requires Python >=3.7, simply install it with:
 
 ```shell
 pip install trapi-predict-kit
 ```
@@ -29,15 +36,26 @@
 
 ```bash
 pip install trapi-predict-kit[web]
 ```
 
 ## 🪄 Usage
 
-### 🔮 Define the prediction endpoint
+### 🍪 Start a new prediction project
+
+A template to help user quickly bootstrap a new prediction project with the recommended structure ([MaastrichtU-IDS/cookiecutter-openpredict-api](https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api/))
+
+You can use [**our cookiecutter template**](https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api/) to quickly bootstrap a repository with everything ready to start developing your prediction models, to then easily publish, and integrate them in the Translator ecosystem
+
+```bash
+pip install cookiecutter
+cookiecutter https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api
+```
+
+### 🔮 Define the prediction endpoint(s)
 
 The `trapi_predict_kit` package provides a decorator `@trapi_predict` to annotate your functions that generate predictions. Predictions generated from functions decorated with `@trapi_predict` can easily be imported in the Translator OpenPredict API, exposed as an API endpoint to get predictions from the web, and queried through the  Translator Reasoner API (TRAPI).
 
 The annotated predict functions are expected to take 2 input  arguments: the input ID (string) and options for the prediction (dictionary). And it should return a dictionary with a list of predicted associated entities hits. Here is an example:
 
  ```python
 from trapi_predict_kit import trapi_predict, PredictOptions, PredictOutput
@@ -84,15 +102,15 @@
             }
         ],
         "count": 1,
     }
     return predictions
  ```
 
-### Define the API
+### Define the TRAPI object
 
 You will need to instantiate a `TRAPI` class to deploy a Translator Reasoner API serving a list of prediction functions that have been decorated with `@trapi_predict`. For example:
 
 ```python
 import logging
 
 from trapi_predict_kit.config import settings
@@ -101,16 +119,14 @@
 from my_model.predict import get_predictions
 
 log_level = logging.ERROR
 if settings.DEV_MODE:
     log_level = logging.INFO
 logging.basicConfig(level=log_level)
 
-predict_endpoints = [ get_predictions ]
-
 openapi_info = {
     "contact": {
         "name": "Firstname Lastname",
         "email": "email@example.com",
         # "x-id": "https://orcid.org/0000-0000-0000-0000",
         "x-role": "responsible developer",
     },
@@ -140,45 +156,59 @@
         "externalDocs": {
             "description": "The values for version are restricted according to the regex in this external JSON schema. See schema and examples at url",
             "url": "https://github.com/NCATSTranslator/translator_extensions/blob/production/x-trapi/",
         },
     }
 }
 
-servers = []
-if settings.VIRTUAL_HOST:
-    servers = [
-        {
-            "url": f"https://{settings.VIRTUAL_HOST}",
-            "description": 'TRAPI ITRB Production Server',
-            "x-maturity": 'production'
-        },
-    ]
-
 app = TRAPI(
-    predict_endpoints=predict_endpoints,
-    servers=servers,
+    predict_endpoints=[ get_predictions ],
     info=openapi_info,
-    title='My model TRAPI',
+    title='OpenPredict TRAPI',
     version='1.0.0',
     openapi_version='3.0.1',
     description="""Machine learning models to produce predictions that can be integrated to Translator Reasoner APIs.
 \n\nService supported by the [NCATS Translator project](https://ncats.nih.gov/translator/about)""",
-    dev_mode=True,
+    itrb_url_prefix="openpredict",
+    dev_server_url="https://openpredict.semanticscience.org",
 )
 ```
 
 ### Deploy the API
 
 Change `trapi.main` to your module path in the command before running it:
 
 ```bash
 uvicorn trapi.main:app --port 8808 --reload
 ```
 
+### 💾 Save a generated model
+
+Helper function to easily save a generated model, its metadata, and the data used to generate it. It uses tools such as [`dvc`](https://dvc.org/) and [`mlem`](https://mlem.ai/) to store large model outside of the git repository.
+
+```python
+from trapi_predict_kit import save
+
+hyper_params = {
+    'penalty': 'l2',
+    'dual': False,
+    'tol': 0.0001,
+    'C': 1.0,
+    'random_state': 100
+}
+
+saved_model = save(
+    model=clf,
+    path="models/my_model",
+    sample_data=sample_data,
+    hyper_params=hyper_params,
+    scores=scores,
+)
+```
+
 ## 🧑‍💻 Development setup
 
 The final section of the README is for if you want to run the package in development, and get involved by making a code contribution.
 
 ### 📥️ Clone
 
 Clone the repository:
@@ -234,19 +264,23 @@
 
 The code will be automatically formatted when you commit your changes using `pre-commit`. But you can also run the script to format the code yourself:
 
 ```
 hatch run fmt
 ```
 
-Check the code for errors, and if it is in accordance with the PEP8 style guide, by running `flake8` and `mypy`:
+### 📖 Update docs
 
+Serve docs locally with `mkdocs`:
+
+```bash
+hatch run docs
 ```
-hatch run check
-```
+
+The documentation website is automatically updated by a GitHub action workflow.
 
 ### ♻️ Reset the environment
 
 In case you are facing issues with dependencies not updating properly you can easily reset the virtual environment with:
 
 ```bash
 hatch env prune
```

### Comparing `trapi_predict_kit-0.1.0/pyproject.toml` & `trapi_predict_kit-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -32,37 +32,39 @@
 dependencies = [
     "requests >=2.23.0",
     "pydantic >=1.9",
     "fastapi >=0.68.1",
     "rdflib >=6.1.1",
     "SPARQLWrapper >=2.0.0,<3.0.0",
     "reasoner-pydantic >=3.0.1",
-    # "fairworkflows",
-    # "fairworkflows@git+https://github.com/vemonet/fairworkflows.git",
-    # "yatiml >=0.10.0",
+    "mlem",
+    # "fairworkflows @ git+https://github.com/vemonet/fairworkflows.git",
 ]
 
 
 
 
 [project.optional-dependencies]
 web = [
     "uvicorn >=0.15.0",
     "gunicorn >=20.0.4",
 ]
-train = [
-    # "mlem >=0.4.0",
-    "mlem"
-]
 test = [
     "pytest >=7.1.3",
     "pytest-cov >=3.0.0",
-    "ruff >=0.0.219",
+    "pre-commit",
     "mypy >=0.991",
-    "black >= 22.8.0",
+    "types-requests",
+]
+doc = [
+    "mkdocs >=1.4.2",
+    "mkdocs-material >=8.2.7",
+    "mkdocstrings[python] >=0.19.1",
+    "mdx-include >=1.4.1",
+    "mkdocs-markdownextradata-plugin >=0.2.5",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/MaastrichtU-IDS/trapi-predict-kit"
 Documentation = "https://github.com/MaastrichtU-IDS/trapi-predict-kit"
 History = "https://github.com/MaastrichtU-IDS/trapi-predict-kit/releases"
@@ -71,84 +73,93 @@
 
 
 # ENVIRONMENTS AND SCRIPTS
 [tool.hatch.envs.default]
 features = [
     "test",
     "web",
-    "train",
+    "doc",
 ]
 post-install-commands = [
+    "pre-commit install",
 ]
 
 [tool.hatch.envs.default.scripts]
-test = "pytest {args}"
-cov = "test --cov src {args}"
 dev = "python tests/dev.py {args}"
 api = "uvicorn tests.dev:app --reload {args}"
 fmt = [
-    "black src tests",
-    "ruff src tests --fix",
+    "pre-commit run --all --all-files",
 ]
-check = [
-    "ruff src tests",
-    "black src tests --check",
-    # "mypy src",
-]
-all = [
+test = [
     "fmt",
-    "check",
-    "cov",
+    "pytest {args}",
+    # "mypy",
 ]
+cov = [
+    "pytest --cov-report html {args}",
+    "python -c 'import webbrowser; webbrowser.open(\"http://0.0.0.0:3000\")'",
+    "python -m http.server 3000 --directory ./htmlcov",
+]
+docs = "mkdocs serve -a localhost:8001 {args}"
 
 # TOOLS
 [tool.hatch.version]
 path = "src/trapi_predict_kit/__init__.py"
 
+# [tool.hatch.metadata]
+# allow-direct-references = true
+
 
 [tool.coverage.run]
 source = ["src"]
 branch = true
 
 [tool.coverage.report]
 omit = ["tests/*"]
 
 
 [tool.mypy]
+files = ["src/"]
 strict = true
 implicit_reexport = true
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 warn_no_return = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
-disallow_any_generics = true
+disallow_any_generics = false
 
 
 [tool.pytest.ini_options]
+addopts = [
+    "-vvv",
+    "--cov=src",
+    "--color=yes",
+    "--cov-report=term-missing",
+]
 filterwarnings = [
     "ignore::DeprecationWarning:httpx.*:"
 ]
 
 
 [tool.black]
 color = true
 line-length = 120
-target-version = ['py37']
+target-version = ['py38']
 skip-string-normalization = false
 
 
 # https://github.com/charliermarsh/ruff#supported-rules
 [tool.ruff]
 src = ["src", "tests"]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
     "A",
     "B",   # flake8-bugbear
     "C",   # flake8-comprehensions
     "E",   # pycodestyle errors
     "F",   # pyflakes
```

### Comparing `trapi_predict_kit-0.1.0/PKG-INFO` & `trapi_predict_kit-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trapi-predict-kit
-Version: 0.1.0
+Version: 0.1.2
 Summary: A package to help create and deploy Translator Reasoner APIs (TRAPI) from any prediction model exposed as a regular python function.
 Project-URL: Homepage, https://github.com/MaastrichtU-IDS/trapi-predict-kit
 Project-URL: Documentation, https://github.com/MaastrichtU-IDS/trapi-predict-kit
 Project-URL: History, https://github.com/MaastrichtU-IDS/trapi-predict-kit/releases
 Project-URL: Tracker, https://github.com/MaastrichtU-IDS/trapi-predict-kit/issues
 Project-URL: Source, https://github.com/MaastrichtU-IDS/trapi-predict-kit
 Author-email: Vincent Emonet <vincent.emonet@gmail.com>
@@ -38,51 +38,63 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: fastapi>=0.68.1
+Requires-Dist: mlem
 Requires-Dist: pydantic>=1.9
 Requires-Dist: rdflib>=6.1.1
 Requires-Dist: reasoner-pydantic>=3.0.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: sparqlwrapper<3.0.0,>=2.0.0
+Provides-Extra: doc
+Requires-Dist: mdx-include>=1.4.1; extra == 'doc'
+Requires-Dist: mkdocs-markdownextradata-plugin>=0.2.5; extra == 'doc'
+Requires-Dist: mkdocs-material>=8.2.7; extra == 'doc'
+Requires-Dist: mkdocs>=1.4.2; extra == 'doc'
+Requires-Dist: mkdocstrings[python]>=0.19.1; extra == 'doc'
 Provides-Extra: test
-Requires-Dist: black>=22.8.0; extra == 'test'
 Requires-Dist: mypy>=0.991; extra == 'test'
+Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'test'
 Requires-Dist: pytest>=7.1.3; extra == 'test'
-Requires-Dist: ruff>=0.0.219; extra == 'test'
-Provides-Extra: train
-Requires-Dist: mlem; extra == 'train'
+Requires-Dist: types-requests; extra == 'test'
 Provides-Extra: web
 Requires-Dist: gunicorn>=20.0.4; extra == 'web'
 Requires-Dist: uvicorn>=0.15.0; extra == 'web'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # 🪄 TRAPI Predict Kit
 
-<!--
-
 [![PyPI - Version](https://img.shields.io/pypi/v/trapi-predict-kit.svg?logo=pypi&label=PyPI&logoColor=silver)](https://pypi.org/project/trapi-predict-kit/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/trapi-predict-kit.svg?logo=python&label=Python&logoColor=silver)](https://pypi.org/project/trapi-predict-kit/)
 [![license](https://img.shields.io/pypi/l/trapi-predict-kit.svg?color=%2334D058)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/blob/main/LICENSE.txt)
 [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
--->
 
 [![Test package](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/test.yml/badge.svg)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/test.yml)
 [![Publish package](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/publish.yml/badge.svg)](https://github.com/MaastrichtU-IDS/trapi-predict-kit/actions/workflows/publish.yml)
 
 </div>
 
 A package to help create and deploy Translator Reasoner APIs (TRAPI) from any prediction model exposed as a regular python function.
 
+The **TRAPI Predict Kit** helps data scientists to build, and **publish prediction models** in a [FAIR](https://www.go-fair.org/fair-principles/) and reproducible manner. It provides helpers for various steps of the process:
+
+* A template to help user quickly bootstrap a new prediction project with the recommended structure ([MaastrichtU-IDS/cookiecutter-trapi-predict-kit](https://github.com/MaastrichtU-IDS/cookiecutter-trapi-predict-kit/))
+* Helper function to easily save a generated model, its metadata, and the data used to generate it. It uses tools such as [`dvc`](https://dvc.org/) and [`mlem`](https://mlem.ai/) to store large model outside of the git repository.
+* Deploy API endpoints for retrieving predictions, which comply with the NCATS Biomedical Data Translator standards ([Translator Reasoner API](https://github.com/NCATSTranslator/ReasonerAPI) and [BioLink model](https://github.com/biolink/biolink-model)), using a decorator `@trapi_predict` to simply annotate the function that produces predicted associations for a given input entity
+
+Predictions are usually generated from machine learning models (e.g. predict disease treated by drug), but it can adapt to generic python function, as long as the input params and return object follow the expected structure.
+
+Checkout the documentation website at **[maastrichtu-ids.github.io/trapi-predict-kit](https://maastrichtu-ids.github.io/trapi-predict-kit)** for more details.
+
 ## 📦️ Installation
 
 This package requires Python >=3.7, simply install it with:
 
 ```shell
 pip install trapi-predict-kit
 ```
@@ -91,15 +103,26 @@
 
 ```bash
 pip install trapi-predict-kit[web]
 ```
 
 ## 🪄 Usage
 
-### 🔮 Define the prediction endpoint
+### 🍪 Start a new prediction project
+
+A template to help user quickly bootstrap a new prediction project with the recommended structure ([MaastrichtU-IDS/cookiecutter-openpredict-api](https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api/))
+
+You can use [**our cookiecutter template**](https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api/) to quickly bootstrap a repository with everything ready to start developing your prediction models, to then easily publish, and integrate them in the Translator ecosystem
+
+```bash
+pip install cookiecutter
+cookiecutter https://github.com/MaastrichtU-IDS/cookiecutter-openpredict-api
+```
+
+### 🔮 Define the prediction endpoint(s)
 
 The `trapi_predict_kit` package provides a decorator `@trapi_predict` to annotate your functions that generate predictions. Predictions generated from functions decorated with `@trapi_predict` can easily be imported in the Translator OpenPredict API, exposed as an API endpoint to get predictions from the web, and queried through the  Translator Reasoner API (TRAPI).
 
 The annotated predict functions are expected to take 2 input  arguments: the input ID (string) and options for the prediction (dictionary). And it should return a dictionary with a list of predicted associated entities hits. Here is an example:
 
  ```python
 from trapi_predict_kit import trapi_predict, PredictOptions, PredictOutput
@@ -146,15 +169,15 @@
             }
         ],
         "count": 1,
     }
     return predictions
  ```
 
-### Define the API
+### Define the TRAPI object
 
 You will need to instantiate a `TRAPI` class to deploy a Translator Reasoner API serving a list of prediction functions that have been decorated with `@trapi_predict`. For example:
 
 ```python
 import logging
 
 from trapi_predict_kit.config import settings
@@ -163,16 +186,14 @@
 from my_model.predict import get_predictions
 
 log_level = logging.ERROR
 if settings.DEV_MODE:
     log_level = logging.INFO
 logging.basicConfig(level=log_level)
 
-predict_endpoints = [ get_predictions ]
-
 openapi_info = {
     "contact": {
         "name": "Firstname Lastname",
         "email": "email@example.com",
         # "x-id": "https://orcid.org/0000-0000-0000-0000",
         "x-role": "responsible developer",
     },
@@ -202,45 +223,59 @@
         "externalDocs": {
             "description": "The values for version are restricted according to the regex in this external JSON schema. See schema and examples at url",
             "url": "https://github.com/NCATSTranslator/translator_extensions/blob/production/x-trapi/",
         },
     }
 }
 
-servers = []
-if settings.VIRTUAL_HOST:
-    servers = [
-        {
-            "url": f"https://{settings.VIRTUAL_HOST}",
-            "description": 'TRAPI ITRB Production Server',
-            "x-maturity": 'production'
-        },
-    ]
-
 app = TRAPI(
-    predict_endpoints=predict_endpoints,
-    servers=servers,
+    predict_endpoints=[ get_predictions ],
     info=openapi_info,
-    title='My model TRAPI',
+    title='OpenPredict TRAPI',
     version='1.0.0',
     openapi_version='3.0.1',
     description="""Machine learning models to produce predictions that can be integrated to Translator Reasoner APIs.
 \n\nService supported by the [NCATS Translator project](https://ncats.nih.gov/translator/about)""",
-    dev_mode=True,
+    itrb_url_prefix="openpredict",
+    dev_server_url="https://openpredict.semanticscience.org",
 )
 ```
 
 ### Deploy the API
 
 Change `trapi.main` to your module path in the command before running it:
 
 ```bash
 uvicorn trapi.main:app --port 8808 --reload
 ```
 
+### 💾 Save a generated model
+
+Helper function to easily save a generated model, its metadata, and the data used to generate it. It uses tools such as [`dvc`](https://dvc.org/) and [`mlem`](https://mlem.ai/) to store large model outside of the git repository.
+
+```python
+from trapi_predict_kit import save
+
+hyper_params = {
+    'penalty': 'l2',
+    'dual': False,
+    'tol': 0.0001,
+    'C': 1.0,
+    'random_state': 100
+}
+
+saved_model = save(
+    model=clf,
+    path="models/my_model",
+    sample_data=sample_data,
+    hyper_params=hyper_params,
+    scores=scores,
+)
+```
+
 ## 🧑‍💻 Development setup
 
 The final section of the README is for if you want to run the package in development, and get involved by making a code contribution.
 
 ### 📥️ Clone
 
 Clone the repository:
@@ -296,19 +331,23 @@
 
 The code will be automatically formatted when you commit your changes using `pre-commit`. But you can also run the script to format the code yourself:
 
 ```
 hatch run fmt
 ```
 
-Check the code for errors, and if it is in accordance with the PEP8 style guide, by running `flake8` and `mypy`:
+### 📖 Update docs
 
+Serve docs locally with `mkdocs`:
+
+```bash
+hatch run docs
 ```
-hatch run check
-```
+
+The documentation website is automatically updated by a GitHub action workflow.
 
 ### ♻️ Reset the environment
 
 In case you are facing issues with dependencies not updating properly you can easily reset the virtual environment with:
 
 ```bash
 hatch env prune
```

