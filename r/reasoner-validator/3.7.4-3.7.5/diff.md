# Comparing `tmp/reasoner_validator-3.7.4.tar.gz` & `tmp/reasoner_validator-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.4.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.5.tar", max compression
```

## Comparing `reasoner_validator-3.7.4.tar` & `reasoner_validator-3.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1153 2023-07-13 23:22:36.908379 reasoner_validator-3.7.4/LICENSE
--rw-r--r--   0        0        0    12703 2023-07-13 23:22:36.908379 reasoner_validator-3.7.4/README.md
--rw-r--r--   0        0        0      131 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/conf.py
--rw-r--r--   0        0        0    19869 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36836 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2177 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/pyproject.toml
--rw-r--r--   0        0        0    38452 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    77837 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    40078 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/message.py
--rw-r--r--   0        0        0    29568 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11622 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    12532 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      774 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/tests/conftest.py
--rw-r--r--   0        0        0   119662 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    40085 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26808 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_validate.py
--rw-r--r--   0        0        0    21570 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_workflows.py
--rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/LICENSE
+-rw-r--r--   0        0        0    12920 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/README.md
+-rw-r--r--   0        0        0      131 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/conf.py
+-rw-r--r--   0        0        0    19963 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    37242 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2177 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/pyproject.toml
+-rw-r--r--   0        0        0    38452 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    78585 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    40494 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/message.py
+-rw-r--r--   0        0        0    29675 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11622 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    12532 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0     1499 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/conftest.py
+-rw-r--r--   0        0        0   114915 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    39404 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26808 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_validate.py
+-rw-r--r--   0        0        0    21570 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_workflows.py
+-rw-r--r--   0        0        0    14907 1970-01-01 00:00:00.000000 reasoner_validator-3.7.5/PKG-INFO
```

### Comparing `reasoner_validator-3.7.4/LICENSE` & `reasoner_validator-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/README.md` & `reasoner_validator-3.7.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
 First install the documentation-specific dependencies.
 
 ```bash
-poetry install --extras docs
+poetry install --extras docs  # or poetry install --all-extras
 ```
 
 The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
 
 ```bash
 cd reasoner_validator
 python ./validation_codes.py
@@ -163,15 +163,15 @@
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
 First install the web-specific dependencies.
 
 ```bash
-poetry install --extras web
+poetry install --extras web  # or poetry install --all-extras
 ```
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
@@ -291,14 +291,15 @@
 
 ## Change Log
 
 Summary of earlier releases and current Change Log is [here](CHANGELOG.md).
 
 ## Code Limitations (implied Future Work?)
 
+- The release of the reasoner-validator after v2.2.0 will not likely be able to (reliably, if at all) validate TRAPI JSON data models prior to 1.3.0
 - Biolink Model release <= 2.4.8 versus 3.0.0 validation: the reasoner-validator uses the Biolink Model Toolkit. As it happens, the toolkit is not backwards compatible with at least one Biolink Model structural change from release 2.#.# to 3.#.#: the tagging of 'canonical' predicates. That is, the 0.8.10++ toolkit reports canonical <= 2.4.8 model predicates as 'non-canonical'.
 - This release of the Reasoner Validator Web Service will detect TRAPI 1.0.* releases but doesn't strive to be completely backwards compatible with them (considering that TRAPI 1.0.* is totally irrelevant now). 
 - The web service validation doesn't do deep validation of the Results part of a TRAPI Message
 - The validation is only run on the first 1000 nodes and 100 edges of graphs, to keep the validation time tractable (this risks not having complete coverage of the graph)
 - Biolink Model toolkit is not (yet) cached so changing the model version during use will result in some latency in results
 - The validator service doesn't (yet) deeply validate non-core node and edge slot contents of Message Knowledge Graphs
 - The validator service doesn't (yet) attempt validation of Query Graph nodes and edges 'constraints' (e.g. `biolink:Association` etc. `domain` and `range` constraints)
```

### Comparing `reasoner_validator-3.7.4/docs/Makefile` & `reasoner_validator-3.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/docs/conf.py` & `reasoner_validator-3.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/docs/index.rst` & `reasoner_validator-3.7.5/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -181,23 +181,28 @@
                 }
             },
             # other 'critical' code-indexed messages
         }
     }
 
 
-Every message has a 'code' and optional context-specific parameters which correspond to
+
+Every message has a 'code', message scope and optional context-specific parameters which correspond to
 named fields in the Python string templates found in the `reasoner_validator package 'codes.yaml' file <https://github.com/NCATSTranslator/reasoner-validator/blob/master/reasoner_validator/codes.yaml>`_.
 
+A human readable page with the codes is `here <validation_codes_dictionary.html>`_.
+
 Note that the trapi_version parameter to the TRAPIResponseValidator can also be a local path to a .yaml TRAPI schema file, which is read in and used as the validation standard. In such a case, though, it is necessary to encode the TRAPI version as a suffix to the root filename, e.g. my_trapi_schema_1.4.0-beta5.yaml. Note that the TRAPI version suffix to the root file name is assumed to be delimited by a leading underscore character. The simplistic parsing of this version is as follows:
 
 .. code-block:: python
+
     root_path: str = string.replace(".yaml", "")
     semver_string = root_path.split("_")[-1]
 
+
 Python API
 ----------
 .. toctree::
    :maxdepth: 2
 
    TRAPI Response Validation <reasoner_validator>
    TRAPI Schema Validation <reasoner_validator.trapi>
@@ -213,15 +218,15 @@
 
 
 Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 =====================================================================================
 
 A local script trapi_validator.py is available to run TRAPI Response validation against either a PK (UUID)
 indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
-text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
+text file or a locally triggered query Request against an directly specified TRAPI endpoint.
 
 Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
 
 For script usage, type:
 
 .. code-block:: bash
```

### Comparing `reasoner_validator-3.7.4/docs/make.bat` & `reasoner_validator-3.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.5/docs/validation_codes_dictionary.md`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,22 @@
 
 ### error.knowledge_graph.edges.empty
 
 **Message:** No edges found!
 
 **Description:** Knowledge graph in TRAPI messages must have a 'edges' key and non-empty associated value!
 
+### error.knowledge_graph.node.id.missing
+
+**Message:** Node identifier is missing for node
+
+**Context:** identifier
+
+**Description:** Knowledge graph node must have a 'id' key with a non-empty associated value!
+
 ### error.knowledge_graph.node.category.missing
 
 **Message:** Category is missing for node
 
 **Context:** identifier
 
 **Description:** Category value must be specified in an knowledge graph edge!
@@ -380,22 +388,14 @@
 
 **Message:** Node has unknown category
 
 **Context:** node_id, identifier
 
 **Description:** Category specified in knowledge graph edge node is not a model element recorded in specified version of Biolink. Replace with a known category!
 
-### error.knowledge_graph.node.id.missing
-
-**Message:** Node identifier is missing for node
-
-**Context:** identifier
-
-**Description:** Knowledge graph node must have a 'id' key with a non-empty associated value!
-
 ### error.knowledge_graph.node.missing_categories
 
 **Message:** Categories are missing for node
 
 **Context:** identifier
 
 **Description:** Knowledge graph node must have a 'categories' key with a non-empty associated value!
@@ -798,14 +798,26 @@
 
 **Message:** TRAPI Response has unrecognized status code
 
 **Context:** identifier
 
 **Description:** The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable
 
+### warning.trapi.response.schema_version.missing
+
+**Message:** TRAPI Response is missing its TRAPI schema version
+
+**Description:** The TRAPI Response should specify its TRAPI version compliance.
+
+### warning.trapi.response.biolink_version.missing
+
+**Message:** TRAPI Response is missing its Biolink Model version
+
+**Description:** The TRAPI Response should specify its Biolink Model version compliance.
+
 ### warning.trapi.response.knowledge_graph.empty
 
 **Message:** Response returned an empty Message Knowledge Graph?
 
 **Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
 
 ### warning.trapi.response.results.empty
```

### Comparing `reasoner_validator-3.7.4/pyproject.toml` & `reasoner_validator-3.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.4"
+version = "3.7.5"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.7.4/reasoner_validator/__init__.py` & `reasoner_validator-3.7.5/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.5/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Version-specific Biolink Model semantic validation of knowledge graph components.
 """
 from typing import Optional, Any, Dict, List, Tuple, Set
+from sys import stderr
 from enum import Enum
 from functools import lru_cache
 from urllib.error import HTTPError
 from pprint import PrettyPrinter
 
 
 from bmt import Toolkit, utils
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
+from reasoner_validator.message import MESSAGE_CATALOG
 from reasoner_validator.sri.util import is_curie
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.versioning import SemVer, SemVerError
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -88,14 +90,15 @@
         self.bmt: Optional[Toolkit] = None
         if biolink_version != "suppress":
             # Here, the Biolink Model version is validated, and the relevant Toolkit pulled.
             self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
             self.resolved_biolink_version = self.bmt.get_model_version()
         else:
             self.resolved_biolink_version = "suppress"
+        print(f"\nBiolink Model Toolkit Wrapper set to TRAPI Version: '{self.resolved_biolink_version}'", file=stderr)
 
     def get_resolved_biolink_version(self) -> Optional[str]:
         return self.resolved_biolink_version
 
     def get_bmt(self) -> Optional[Toolkit]:
         return self.bmt
 
@@ -153,15 +156,15 @@
 
         :param graph_type: type of graph data being validated
         :type graph_type: TRAPIGraphType
         :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
         :type trapi_version: Optional[str] or None
         :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
         :type biolink_version: Optional[str] or None
-        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :param target_provenance: Dictionary of context identifying the ARA and KP for provenance attribute validation
         :type target_provenance: Optional[Dict[str,str]]
         """
         BMTWrapper.__init__(self, biolink_version=biolink_version)
         ValidationReporter.__init__(
             self,
             prefix=f"Biolink Validation of {graph_type.value}",
             trapi_version=trapi_version,
@@ -181,15 +184,15 @@
             current: SemVer = SemVer.from_string(self.biolink_version)
             target: SemVer = SemVer.from_string(version)
             return current >= target
         except SemVerError as sve:
             logger.error(f"minimum_required_biolink_version() error: {str(sve)}")
             return False
 
-    def get_result(self) -> Tuple[str, Optional[Dict[str, Dict[str, Optional[List[Dict[str, str]]]]]]]:
+    def get_result(self) -> Tuple[str, MESSAGE_CATALOG]:
         """
         Get result of validation.
 
         :return: model version of the validation and dictionary of reported validation messages.
         :rtype Tuple[str, Optional[Dict[str, Set[str]]]]
         """
         return self.bmt.get_model_version(), self.get_messages()
@@ -202,65 +205,80 @@
         :type node_id: str, node identifier
         :param slots: properties of the node
         :type slots: Dict
         """
         logger.debug(f"{node_id}: {str(slots)}")
 
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
-            # TODO: this will fail for an earlier TRAPI data schema version
-            #       which didn't use the tag 'categories' for nodes...
-            #       probably no longer relevant to the community?
-            if 'categories' in slots:
-                if not isinstance(slots["categories"], List):
-                    self.report(code="error.knowledge_graph.node.categories.not_array", identifier=node_id)
-                else:
-                    if self.validate_biolink():
+            if self.validate_biolink():
+                # TODO: this will fail for an earlier TRAPI data schema version
+                #       which didn't use the tag 'categories' for nodes...
+                #       But this earlier TRAPI release is no longer relevant to the community?
+                if 'categories' in slots:
+                    if not isinstance(slots["categories"], List):
+                        self.report(code="error.knowledge_graph.node.categories.not_array", identifier=node_id)
+                    else:
                         # Biolink Validation of node, if not suppressed
                         categories = slots["categories"]
                         node_prefix_mapped: bool = False
                         concrete_category_found: bool = False
+                        included_category: Optional[str] = None
                         for category in categories:
-                            category: Optional[ClassDefinition] = \
+                            concrete_category: Optional[ClassDefinition] = \
                                 self.validate_category(
                                     context="knowledge_graph",
                                     node_id=node_id,
                                     category=category
                                 )
                             # Only 'concrete' (non-abstract, non-mixin, preferably,
                             # non-deprecated) categories are of interest here,
                             # since only they will have associated namespaces
-                            if category:
+                            if concrete_category:
                                 concrete_category_found: bool = True
                                 possible_subject_categories = self.bmt.get_element_by_prefix(node_id)
-                                if possible_subject_categories and category.name in possible_subject_categories:
+                                if possible_subject_categories and \
+                                        concrete_category.name in possible_subject_categories:
                                     node_prefix_mapped = True
                                     # don't need to search any more categories
                                     break
+                            else:
+                                # See above note about CATEGORY_INCLUSIONS
+                                if category in self.CATEGORY_INCLUSIONS:
+                                    included_category = category
 
                         if not concrete_category_found:
-                            self.report(
-                                code="error.knowledge_graph.node.categories.not_concrete",
-                                identifier=node_id,
-                                categories=str(categories)
-                            )
+                            # Although we didn't find any concrete categories, maybe
+                            # we instead saw one of the 'included' abstract/mixin categories
+                            if included_category is not None:
+                                self.report(
+                                    code=f"warning.knowledge_graph.node.category.abstract_or_mixin",
+                                    identifier=concrete_category_found,
+                                    node_id=node_id
+                                )
+                            else:
+                                self.report(
+                                    code="error.knowledge_graph.node.categories.not_concrete",
+                                    identifier=node_id,
+                                    categories=str(categories)
+                                )
 
                         if not node_prefix_mapped:
                             self.report(
                                 code="warning.knowledge_graph.node.id.unmapped_prefix",
                                 identifier=node_id,
                                 categories=str(categories)
                             )
-            else:
-                self.report(
-                    code="error.knowledge_graph.node.category.missing",
-                    context=self.graph_type.value, identifier=node_id
-                )
+                else:
+                    self.report(
+                        code="error.knowledge_graph.node.category.missing",
+                        identifier=node_id
+                    )
 
-            # TODO: Do we need to (or can we) validate here, any other
-            #       Knowledge Graph node fields? Perhaps not yet?
+                # TODO: Do we need to (or can we) validate here, any other
+                #       Knowledge Graph node fields? Perhaps not yet?
 
         else:  # Query Graph node validation
 
             has_node_ids: bool
             if "ids" in slots and slots["ids"]:
                 has_node_ids = True
                 node_ids = slots["ids"]
@@ -417,15 +435,16 @@
                 if not ara_source.startswith("infores:"):
                     ara_source = f"infores:{ara_source}"
             if 'kp_source' in self.target_provenance and self.target_provenance['kp_source']:
                 kp_source: str = self.target_provenance['kp_source']
                 if not kp_source.startswith("infores:"):
                     kp_source = f"infores:{kp_source}"
             kp_source_type = self.target_provenance['kp_source_type'] \
-                if 'kp_source_type' in self.target_provenance and self.target_provenance['kp_source_type'] else 'aggregator'
+                if 'kp_source_type' in self.target_provenance and self.target_provenance['kp_source_type'] \
+                else 'aggregator'
             kp_source_type = f"biolink:{kp_source_type}_knowledge_source"
 
         return ara_source, kp_source, kp_source_type
 
     def validate_provenance(
             self,
             edge_id,
@@ -508,15 +527,15 @@
         # the source_trail is already known and given to this method for reporting purposes here
 
         # Otherwise, in TRAPI 1.3.0, the 'sources' may be compiled here, in this method, from the attributes
         # themselves, then a newly generated 'source_trail', returned for use by the rest of the application
         sources: Dict[str, List[str]] = dict()
 
         # we only report errors about missing or empty edge attributes if TRAPI 1.3.0 or earlier,
-        # and Biolink Validation is not suppressed, since we can't fully validate provenance)
+        # and Biolink Validation is not suppressed, since we can't fully validate provenance and
         # since earlier TRAPI releases are minimally expected to record provenance attributes
         # we only report this for TRAPI < 1.4 when Biolink Validation is done given that
         # without Biolink validation, provenance cannot be reliably assessed
 
         # We can already use 'source_trail' here in the report in case it was
         # already pre-computed by the validate_sources parsing of TRAPI 1.4.0;
         # if TRAPI 1.3.0 is the validation standard, the 'source_trail' would
@@ -837,15 +856,15 @@
                         qualifiers=qualifier_set
                     )
 
     def validate_infores(self, context: str, edge_id: str, identifier: str) -> bool:
         """
         Validate that the specified identifier is a well-formed Infores CURIE.
         Note that here we also now accept that the identifier can
-        be a semi-colon delimited list of such infores.
+        be a semicolon delimited list of such infores.
 
         :param context: reporting context as specified by a validation code prefix
         :param edge_id: specific edge validated, for the purpose of reporting validation context
         :param identifier: candidate (list of) infores curie(s) to be validated.
         :return:
         """
         code_prefix: str = f"error.knowledge_graph.edge.sources.retrieval_source.{context}.infores"
@@ -859,15 +878,15 @@
             )
             return False
 
         # For uniform processing here, we treat every identifier
         # as a potential list (even if only a list of one entry),
         ids: list[str] = [token.strip() for token in identifier.split(";")]
         if not all([i for i in ids]):
-            # if the identifier is a semi-colon delimited array,
+            # if the identifier is a semicolon delimited array,
             # then at least one of the entries is None or empty...
             self.report(
                 code=f"{code_prefix}.missing",
                 identifier=identifier,
                 edge_id=edge_id
             )
             return False
@@ -1323,23 +1342,15 @@
                 if biolink_class.deprecated:
                     self.report(
                         code=f"warning.{context}.node.category.deprecated",
                         identifier=category,
                         node_id=node_id
                     )
                 if biolink_class.abstract or self.bmt.is_mixin(category):
-                    # See above note about CATEGORY_INCLUSIONS
-                    if context == "knowledge_graph" and category in self.CATEGORY_INCLUSIONS:
-                        self.report(
-                            code=f"warning.{context}.node.category.abstract_or_mixin",
-                            identifier=category,
-                            node_id=node_id
-                        )
-                    else:
-                        biolink_class = None
+                    biolink_class = None
                 elif not self.bmt.is_category(category):
                     self.report(
                         code=f"error.{context}.node.category.not_a_category",
                         identifier=category,
                         node_id=node_id
                     )
                     biolink_class = None
```

### Comparing `reasoner_validator-3.7.4/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.5/reasoner_validator/codes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,20 @@
         $message: "No nodes found!"
         $description: "Knowledge graph in TRAPI messages must have a 'nodes' key and non-empty associated value!"
     edges:
       empty:
         $message: "No edges found!"
         $description: "Knowledge graph in TRAPI messages must have a 'edges' key and non-empty associated value!"
     node:
+      id:
+        missing:
+          $message: "Node identifier is missing for node"
+          $context:
+            - identifier
+          $description: "Knowledge graph node must have a 'id' key with a non-empty associated value!"
       category:
         missing:
           $message: "Category is missing for node"
           $context:
             - identifier
           $description: "Category value must be specified in an knowledge graph edge!"
         not_a_category:
@@ -298,20 +304,14 @@
           $description: "Category specified in knowledge graph edge node is not recorded as a category term in specified version of Biolink. Replace with a known category!"
         unknown:
           $message: "Node has unknown category"
           $context:
             - node_id
             - identifier
           $description: "Category specified in knowledge graph edge node is not a model element recorded in specified version of Biolink. Replace with a known category!"
-      id:
-        missing:
-          $message: "Node identifier is missing for node"
-          $context:
-            - identifier
-          $description: "Knowledge graph node must have a 'id' key with a non-empty associated value!"
       missing_categories:
         $message: "Categories are missing for node"
         $context:
           - identifier
         $description: "Knowledge graph node must have a 'categories' key with a non-empty associated value!"
       ids:
         not_array:
@@ -611,14 +611,22 @@
     response:
       status:
         unknown:
           $message: "TRAPI Response has unrecognized status code"
           $context:
             - identifier
           $description:  "The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable"
+      schema_version:
+        missing:
+          $message: "TRAPI Response is missing its TRAPI schema version"
+          $description:  "The TRAPI Response should specify its TRAPI version compliance."
+      biolink_version:
+        missing:
+          $message: "TRAPI Response is missing its Biolink Model version"
+          $description:  "The TRAPI Response should specify its Biolink Model version compliance."
       knowledge_graph:
         empty:
           $message: "Response returned an empty Message Knowledge Graph?"
           $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
       results:
         empty:
           $message: "Response returned empty Message.results?"
```

### Comparing `reasoner_validator-3.7.4/reasoner_validator/message.py` & `reasoner_validator-3.7.5/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/report.py` & `reasoner_validator-3.7.5/reasoner_validator/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Error and Warning Reporting Module"""
 from typing import Optional, Dict, List
-from sys import stdout
+from sys import stdout, stderr
 from importlib import metadata
 from io import StringIO
 import copy
 
 from json import dumps, JSONEncoder
 
 from reasoner_validator.message import (
@@ -72,16 +72,19 @@
                                 validated (Default: if None, use the Biolink Model Toolkit default version).
         :type biolink_version: Optional[str] = None
         :param strict_validation: if True, abstract and mixin elements validate as 'error';
                                   if None or False, just issue a 'warning'
         :type strict_validation: Optional[bool] = None
         """
         self.prefix: str = prefix if prefix else ""
+
         self.trapi_version = get_latest_version(trapi_version) \
             if trapi_version else get_latest_version(self.DEFAULT_TRAPI_VERSION)
+        print(f"\nValidationReporter set to TRAPI Version: '{self.trapi_version}'", file=stderr)
+
         self.biolink_version = biolink_version
         self.strict_validation: Optional[bool] = strict_validation
         self.messages: MESSAGE_CATALOG = {
             "critical": dict(),
             "errors": dict(),
             "warnings": dict(),
             "information": dict()
```

### Comparing `reasoner_validator-3.7.4/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.5/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.5/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.5/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.5/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/reasoner_validator/versioning.py` & `reasoner_validator-3.7.5/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.5/tests/test_biolink_compliance_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,27 @@
     TRAPIGraphType,
     BiolinkValidator,
     get_biolink_model_toolkit,
     check_biolink_model_compliance_of_input_edge,
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph
 )
+from tests import SIMPLE_SAMPLE_NODES, SAMPLE_NODES_WITH_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 pp = PrettyPrinter(indent=4)
 
 # January 25, 2023 - as of reasoner-validator 3.1.0,
 # we don't pretend to totally support Biolink Models any earlier than 3.1.1.
 # If earlier biolink model compliance testing is desired,
 # then perhaps reasoner-validator version 3.0.5 or earlier can be used.
-LATEST_BIOLINK_MODEL_VERSION = "3.2.0"
+LATEST_BIOLINK_MODEL_VERSION = "3.5.2"
 
 # special case of signalling suppression of validation
 SUPPRESS_BIOLINK_MODEL_VALIDATION = "suppress"
 
 
 def test_set_default_biolink_versioned_global_environment():
     validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
@@ -1211,72 +1212,34 @@
                     },
                 ]
             },
             get_ara_test_case(),
             "error.knowledge_graph.edge.attribute.value.empty"
         ),
         (
-            # Query 7. KP provenance value is not a well-formed InfoRes CURIE? Should fail?
+            # Query 7. An attribute_type_id is not a well-formed CURIE? Should fail?
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": "infores:aragorn"
                     },
                     {
-                        "attribute_type_id": "biolink:primary_knowledge_source",
-                        "value": "infores:panther"
+                        "attribute_type_id": "biolink:stoichiometry",
+                        "value": 2
                     },
                     {
                         "attribute_type_id": "non_a_curie",
                         "value": "something"
                     }
                 ]
             },
             get_ara_test_case(),
             # "is not a well-formed CURIE!"
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
-        ),
-        (
-            # Query 8. kp type is 'primary'. Should pass?
-            {
-                "attributes": [
-                    {
-                        "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": "infores:aragorn"
-                    },
-                    {
-                        "attribute_type_id": "biolink:primary_knowledge_source",
-                        "value": "infores:panther"
-                    }
-                ]
-            },
-            get_ara_test_case(),
-            ""
-        ),
-        (
-            # Query 9. Is complete and should pass?
-            {
-                "attributes": [
-                    {
-                        "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": "infores:aragorn"
-                    },
-                    {
-                        "attribute_type_id": "biolink:aggregator_knowledge_source",
-                        "value": "infores:panther"
-                    },
-                    {
-                        "attribute_type_id": "biolink:primary_knowledge_source",
-                        "value": "infores:my-primary-ks"
-                    }
-                ]
-            },
-            get_ara_test_case({"kp_source_type": "aggregator"}),
-            ""
         )
     ]
 )
 def test_latest_validate_attributes(query: Tuple):
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         # trapi_version="latest",
@@ -1880,61 +1843,27 @@
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
 
             # Query 0: Sample full valid TRAPI Knowledge Graph
             {
                 # Sample nodes
-                'nodes': {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                        "attributes": [
-                            {
-                                "attribute_source": "infores:chembl",
-                                "attribute_type_id": "biolink:highest_FDA_approval_status",
-                                "attributes": [],
-                                "original_attribute_name": "max_phase",
-                                "value": "FDA Clinical Research Phase 2",
-                                "value_type_id": "biolink:FDA_approval_status_enum"
-                            }
-                        ]
-                    }
-                },
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
                 # Sample edge
                 'edges': {
                    "edge_1": {
                        "subject": "NCBIGene:29974",
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                        "attributes": [
                            {
                                "attribute_source": "infores:hmdb",
-                               "attribute_type_id": "biolink:primary_knowledge_source",
-                               "attributes": [],
-                               "description": "MolePro's HMDB target transformer",
-                               "original_attribute_name": "biolink:primary_knowledge_source",
-                               "value": "infores:hmdb",
-                               "value_type_id": "biolink:InformationResource"
-                           },
-                           {
-                               "attribute_source": "infores:hmdb",
-                               "attribute_type_id": "biolink:aggregator_knowledge_source",
+                               "attribute_type_id": "biolink:stoichiometry",
+                               "value": 2,
                                "attributes": [],
-                               "description": "Molecular Data Provider",
-                               "original_attribute_name": "biolink:aggregator_knowledge_source",
-                               "value": "infores:molepro",
-                               "value_type_id": "biolink:InformationResource"
                            }
                         ],
                        "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
@@ -1960,36 +1889,24 @@
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - No nodes found!"
             "error.knowledge_graph.nodes.empty"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 3: Empty edges - caught by missing 'edges' dictionary
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    }
-                }
+                "nodes": SIMPLE_SAMPLE_NODES
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - No edges found!"
             "error.knowledge_graph.edges.empty"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 4 Empty edges dictionary
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {}
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - No edges found!"
             "error.knowledge_graph.edges.empty"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
@@ -1999,15 +1916,20 @@
                     "NCBIGene:29974": {}
                 },
                 "edges": {
                    "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2018,23 +1940,28 @@
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 6: 'categories' tag value is ill-formed: should be a list
             {
                 "nodes": {
                     "NCBIGene:29974": {
-                       "categories": "biolink:Gene"
+                        "categories": "biolink:Gene"
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2046,27 +1973,32 @@
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 7: Knowledge Graph 'categories' list values should include
             #          at least one (non-abstract, non-mixin) category term
             {
                 "nodes": {
                     "UniProtKB:Q14191": {
-                       "categories": ["biolink:GeneProductMixin"]
+                        "categories": ["biolink:GeneProductMixin"]
                     },
                     "CHEBI:18420": {
                         "name": "Magnesium",
                         "categories": ["biolink:SmallMolecule"]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "UniProtKB:Q14191",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "CHEBI:18420",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2077,89 +2009,135 @@
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 8: unknown category specified
             {
                 "nodes": {
                     "NCBIGene:29974": {
-                       "categories": [
+                        "categories": [
                            "biolink:NonsenseCategory"
-                       ]
+                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Knowledge Graph Node element 'biolink:NonsenseCategory' is unknown!"
             "error.knowledge_graph.node.category.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 9: unknown category specified
+            # Query 9: issue a warning about an 'inclusion list' abstract or mixin category
+            #          iff they are specified as the only (most specific) category
             {
                 "nodes": {
                     "NCBIGene:29974": {
-                       "categories": [
+                        "categories": [
                            "biolink:BiologicalEntity"
-                       ]
+                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node has deprecated category!"
+            # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node has an abstract or mixin category!"
             "warning.knowledge_graph.node.category.abstract_or_mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 10: abstract category in Knowledge Graphs? Itself ignored now during validation,
+            # Query 10: ignore 'included' abstract or mixin categories which are
+            #           only specified as parents to concrete child instances
+            {
+                "nodes": {
+                    "NCBIGene:29974": {
+                        "categories": [
+                            "biolink:BiologicalEntity",
+                            "biolink:Gene"
+                        ]
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "NCBIGene:29974",
+                        "predicate": "biolink:physically_interacts_with",
+                        "object": "NCBIGene:29974",
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            ""  # this should pass without error?
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+            # Query 11: abstract category in Knowledge Graphs? Itself ignored now during validation,
             #          although if at least one 'concrete' class is not given, other related
             #          validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
-                       "categories": [
+                        "categories": [
                            "biolink:Entity",
                            "biolink:Gene"
-                       ]
+                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
-                                "attribute_type_id": "biolink:primary_knowledge_source",
-                                "value": "infores:my-kp"
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
                             }
                         ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
@@ -2167,35 +2145,35 @@
                     }
                 }
             },
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 11: mixin category in Knowledge Graphs? Itself ignored now during validation,
+            # Query 12: mixin category in Knowledge Graphs? Itself ignored now during validation,
             #          although if at least one 'concrete' class is not given with id_prefix mappings,
             #          other related validation errors (e.g. 'unmapped_prefix'?) may be reported?
             {
                 "nodes": {
                     "NCBIGene:29974": {
-                       "categories": [
+                        "categories": [
                            "biolink:GeneOrGeneProduct",
                            "biolink:Gene"
-                       ]
+                        ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
-                                "attribute_type_id": "biolink:primary_knowledge_source",
-                                "value": "infores:my-kp"
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
                             }
                         ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
@@ -2210,20 +2188,22 @@
         #     LATEST_BIOLINK_MODEL,
         #     # Query xx: deprecated category triggers a warning in Knowledge Graphs
         #     {
         #         "nodes": {
         #             "CHEBI:27300": {  # Vitamin D
         #                "categories": [
         #                    "biolink:Nutrient"
-        #                ]
+        #                ],
+        #                "description": "Vitamin D"
         #             },
         #             "Orphanet:120464": {  # Vitamin D Receptor
         #                "categories": [
         #                    "biolink:Protein"
-        #                ]
+        #                ],
+        #                "description": "Vitamin D Receptor"
         #             }
         #         },
         #         "edges": {
         #             "edge_1": {
         #                 "subject": "CHEBI:27300",
         #                 "predicate": "biolink:physically_interacts_with",
         #                 "object": "Orphanet:120464",
@@ -2232,37 +2212,38 @@
         #         }
         #     },
         #  f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Knowledge Graph Node element 'biolink:OntologyClass' is deprecated!"
         #     "warning.knowledge_graph.node.category.deprecated"
         # ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 12: invalid node CURIE prefix namespace, for specified category
+            # Query 13: invalid node CURIE prefix namespace, for specified category
             {
                 "nodes": {
                     "FOO:1234": {
-                       "categories": [
+                        "categories": [
                            "biolink:Gene"
-                       ],
+                        ],
+                        "description": "Hong Kong Fooey"
                     },
                     "NCBIGene:29974": {
                         "categories": [
                             "biolink:Gene"
                         ]
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "FOO:1234",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
-                                "attribute_type_id": "biolink:primary_knowledge_source",
-                                "value": "infores:my-kp"
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
                             }
                         ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
@@ -2272,29 +2253,28 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Node 'FOO:1234' " +
             # "is unmapped to the target categories: ['biolink:Gene']?"
             "warning.knowledge_graph.node.id.unmapped_prefix"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 13: missing or empty subject, predicate, object values
+            # Query 14 missing or empty subject, predicate, object values
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         # "subject": "",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2303,245 +2283,224 @@
             # ditto for predicate and object... but identical code pattern thus we only test missing subject id here
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'None--biolink:interacts_with->NCBIGene:29974' " +
             # "has a missing or empty 'subject' slot value!"
             "error.knowledge_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 14: 'subject' id is missing from the nodes catalog
+            # Query 15: 'subject' id is missing from the nodes catalog
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:12345",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'subject' id 'NCBIGene:12345' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.subject.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 15: predicate is unknown
+            # Query 16: predicate is unknown
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:unknown_predicate",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:unknown_predicate' is unknown!"
             "error.knowledge_graph.edge.predicate.unknown"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 16: predicate is invalid - may be a valid Biolink element but is not a predicate
+            # Query 17: predicate is invalid - may be a valid Biolink element but is not a predicate
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:has_unit",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:has_unit' is invalid!"
             "error.knowledge_graph.edge.predicate.invalid"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 17: predicate is a mixin - not allowed in Knowledge Graphs
+            # Query 18: predicate is a mixin - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "HGNC:3059": {
-                       "categories": [
+                        "categories": [
                            "biolink:Gene"
-                       ]
+                        ],
+                        "description": "heparin binding EGF like growth factor"
                     },
                     "HGNC:391": {
                         "name": "AKT serine/threonine kinase 1",
                         "categories": [
                             "biolink:Gene"
                         ],
+                        "description": "AKT serine/threonine kinase 1"
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "HGNC:3059",
                         "predicate": "biolink:increases_amount_or_activity_of",
                         "object": "HGNC:391",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # "{KNOWLEDGE_GRAPH_PREFIX}: ERROR -Predicate element 'biolink:increases_amount_or_activity of' is a mixin!"
             "error.knowledge_graph.edge.predicate.mixin"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 18: predicate is abstract - not allowed in Knowledge Graphs
+            # Query 19: predicate is abstract - not allowed in Knowledge Graphs
             {
                 "nodes": {
                     "PMID:1234": {
-                       "categories": [
+                        "categories": [
                            "biolink:InformationContentEntity"
-                       ]
+                        ],
+                        "description": "Some kind of journal article"
                     },
                     "ORCID:56789": {
-                        "name": "cytosine",
+                        "name": "Somebody Great!",
                         "categories": [
                             "biolink:Agent"
                         ],
+                        "description": "a great person"
                     }
                 },
                 "edges": {
                     "edge_1": {
                         "subject": "PMID:1234",
                         "predicate": "biolink:contributor",
                         "object": "ORCID:56789",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Predicate element 'biolink:contributor' is abstract!"
             "error.knowledge_graph.edge.predicate.abstract"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 19: predicate is non-canonical
+            # Query 20: predicate is non-canonical
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:affected_by",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge predicate 'biolink:affected_by' is non-canonical?"
             "warning.knowledge_graph.edge.predicate.non_canonical"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 20: 'object' id is missing from the nodes catalog
+            # Query 21: 'object' id is missing from the nodes catalog
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:678",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2549,29 +2508,17 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'object' id " +
             # f"'PUBCHEM.COMPOUND:678' is missing from the nodes catalog!"
             "error.knowledge_graph.edge.object.missing_from_nodes"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 21: attribute 'attribute_type_id' is missing
+            # Query 22: attribute 'attribute_type_id' is missing
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"value": "some value"}],
                         "sources": [
@@ -2584,64 +2531,45 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'attribute_type_id' key!"
             "error.knowledge_graph.edge.attribute.type_id.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 22: attribute 'value' is missing?
+            # Query 23: attribute 'value' is missing?
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
-                        "attributes": [{"attribute_type_id": "biolink:knowledge_source"}],
+                        "attributes": [
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                # "value": 2
+                            }
+                        ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute is missing its 'value' key!"
             "error.knowledge_graph.edge.attribute.value.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 23: 'attribute_type_id' is not a CURIE
+            # Query 24: 'attribute_type_id' is not a CURIE
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"attribute_type_id": "not_a_curie", "value": "some value"}],
                         "sources": [
@@ -2654,29 +2582,17 @@
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge attribute_type_id 'not_a_curie' is not a CURIE!"
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 24: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
+            # Query 25: 'attribute_type_id' is not a 'biolink:association_slot' (biolink:synonym is a node property)
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"attribute_type_id": "biolink:synonym", "value": "some synonym"}],
                         "sources": [
@@ -2690,66 +2606,48 @@
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id "
             # "'biolink:synonym' is not a biolink:association_slot?"
             "warning.knowledge_graph.edge.attribute.type_id.not_association_slot"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 25: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
+            # Query 26: 'attribute_type_id' has a 'biolink' CURIE prefix and is an association_slot, so it should pass
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
-                            {"attribute_type_id": "biolink:negated", "value": "some value"},
-                            {"attribute_type_id": "biolink:primary_knowledge_source", "value": "infores:hmdb"}
+                            {
+                                "attribute_type_id": "biolink:negated",
+                                "value": "some value"
+                            },
+                            {
+                                "attribute_type_id": "biolink:stoichiometry",
+                                "value": 2
+                            }
                         ],
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             ""  # this should recognize the 'attribute_type_id' as a Biolink CURIE
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
-            # Query 26: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
+            # Query 27: 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink?
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"attribute_type_id": "foo:bar", "value": "some value"}],
                         "sources": [
@@ -2761,58 +2659,47 @@
                     }
                 }
             },
             # f"{KNOWLEDGE_GRAPH_PREFIX}: WARNING - Edge attribute_type_id 'foo:bar' " +
             # f"has a CURIE prefix namespace unknown to Biolink!"
             "warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix"
         ),
-        (   # Query 27:  # An earlier Biolink Model won't recognize a category not found in its specified release
+        (   # Query 28:  # An earlier Biolink Model won't recognize a category not found in its specified release
             "1.8.2",
             {
                 # Sample nodes
                 'nodes': {
                     "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
+                        "categories": [
+                            "biolink:Gene"
+                        ]
                     },
                     "PUBCHEM.COMPOUND:597": {
                         "name": "cytosine",
                         "categories": [
-                            "biolink:SmallMolecule"  # Not valid in the latest model?
+                            "biolink:SmallMolecule"   # Not valid in the latest model?
                         ],
+                        "description": "Cytosine nucleotide"
                     }
                 },
                 # Sample edge
                 'edges': {
                    "edge_1": {
                        "subject": "NCBIGene:29974",
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                     }
                 }
             },
             "error.knowledge_graph.node.category.unknown"
         ),
-        (   # Query 28:  #'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
+        (   # Query 29:  # 'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"attribute_type_id": "foo:bar", "value": "some value"}],
                         "sources": [
@@ -2826,30 +2713,18 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 29: 'attribute_type_id' is not a 'biolink:association_slot'
+            # Query 30: 'attribute_type_id' is not a 'biolink:association_slot'
             #           (biolink:synonym is a node property) but...
             {
-                "nodes": {
-                    "NCBIGene:29974": {
-                       "categories": [
-                           "biolink:Gene"
-                       ]
-                    },
-                    "PUBCHEM.COMPOUND:597": {
-                        "name": "cytosine",
-                        "categories": [
-                            "biolink:SmallMolecule"
-                        ],
-                    }
-                },
+                "nodes": SIMPLE_SAMPLE_NODES,
                 "edges": {
                     "edge_1": {
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [{"attribute_type_id": "biolink:synonym", "value": "some synonym"}],
                         "sources": [
@@ -2864,35 +2739,24 @@
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         )
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(
-        biolink_version: str, graph_data: Dict, validation_code: str):
+        biolink_version: str, graph_data: Dict, validation_code: str
+):
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=graph_data, biolink_version=biolink_version
     )
     check_messages(validator, validation_code)
 
 
 MESSAGE_EDGE_WITHOUT_ATTRIBUTES = {
-    "nodes": {
-        "NCBIGene:29974": {
-            "categories": [
-                "biolink:Gene"
-            ]
-        },
-        "PUBCHEM.COMPOUND:597": {
-            "name": "cytosine",
-            "categories": [
-                "biolink:SmallMolecule"
-            ],
-        }
-    },
+    "nodes": SIMPLE_SAMPLE_NODES,
     "edges": {
         "edge_1": {
             "subject": "NCBIGene:29974",
             "predicate": "biolink:physically_interacts_with",
             "object": "PUBCHEM.COMPOUND:597",
             # "attributes": [{"attribute_type_id": "biolink:knowledge_source"}]
         }
```

### Comparing `reasoner_validator-3.7.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_response_validator.py` & `reasoner_validator-3.7.5/tests/test_response_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from copy import deepcopy
 
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
 from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
 
-from tests import PATCHED_140_SCHEMA_FILEPATH
+from tests import PATCHED_140_SCHEMA_FILEPATH, SAMPLE_NODES_WITH_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 _TEST_QG_1 = {
@@ -34,39 +34,14 @@
             "subject": "drug",
             "predicates": ["biolink:treats"],
             "object": "type-2 diabetes"
         }
     }
 }
 
-# Sample nodes
-_TEST_NODES_1 = {
-        "NCBIGene:29974": {
-           "categories": [
-               "biolink:Gene"
-           ]
-        },
-        "PUBCHEM.COMPOUND:597": {
-            "name": "cytosine",
-            "categories": [
-                "biolink:SmallMolecule"
-            ],
-            "attributes": [
-                {
-                    "attribute_source": "infores:chembl",
-                    "attribute_type_id": "biolink:highest_FDA_approval_status",
-                    "attributes": [],
-                    "original_attribute_name": "max_phase",
-                    "value": "FDA Clinical Research Phase 2",
-                    "value_type_id": "biolink:FDA_approval_status_enum"
-                }
-            ]
-        }
-    }
-
 # Sample edge 1
 _TEST_EDGES_1 = {
        "edge_1": {
            "subject": "NCBIGene:29974",
            "predicate": "biolink:physically_interacts_with",
            "object": "PUBCHEM.COMPOUND:597",
            "attributes": [
@@ -89,15 +64,15 @@
                    "value_type_id": "biolink:InformationResource"
                }
             ],
         }
     }
 
 _TEST_KG_1 = {
-    "nodes": _TEST_NODES_1,
+    "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_1
 }
 
 _TEST_RESULTS_1 = [
         {
             "node_bindings": {
                 "type-2 diabetes": [{"id": "MONDO:0005148"}],
@@ -126,15 +101,15 @@
                    "value_type_id": "biolink:InformationResource"
                }
            ],
         }
     }
 
 _TEST_KG_2 = {
-    "nodes": _TEST_NODES_1,
+    "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_2
 }
 
 _TEST_QG_2 = {
     "nodes": {
         "paper": {
             "categories": ["biolink:InformationContentEntity"]
@@ -221,15 +196,15 @@
                }
            ],
         }
     }
 
 
 _TEST_KG_4 = {
-    "nodes": _TEST_NODES_1,
+    "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_4
 }
 
 # From Implementation Guidlines circa June 2023
 _TEST_TRAPI_1_4_2_FULL_SAMPLE = {
     "message": {
         "query_graph": {
```

### Comparing `reasoner_validator-3.7.4/tests/test_semver.py` & `reasoner_validator-3.7.5/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.5/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_validate.py` & `reasoner_validator-3.7.5/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_validation_report.py` & `reasoner_validator-3.7.5/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/tests/test_workflows.py` & `reasoner_validator-3.7.5/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.4/PKG-INFO` & `reasoner_validator-3.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.4
+Version: 3.7.5
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -151,15 +151,15 @@
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
 First install the documentation-specific dependencies.
 
 ```bash
-poetry install --extras docs
+poetry install --extras docs  # or poetry install --all-extras
 ```
 
 The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
 
 ```bash
 cd reasoner_validator
 python ./validation_codes.py
@@ -205,15 +205,15 @@
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
 First install the web-specific dependencies.
 
 ```bash
-poetry install --extras web
+poetry install --extras web  # or poetry install --all-extras
 ```
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
@@ -333,14 +333,15 @@
 
 ## Change Log
 
 Summary of earlier releases and current Change Log is [here](CHANGELOG.md).
 
 ## Code Limitations (implied Future Work?)
 
+- The release of the reasoner-validator after v2.2.0 will not likely be able to (reliably, if at all) validate TRAPI JSON data models prior to 1.3.0
 - Biolink Model release <= 2.4.8 versus 3.0.0 validation: the reasoner-validator uses the Biolink Model Toolkit. As it happens, the toolkit is not backwards compatible with at least one Biolink Model structural change from release 2.#.# to 3.#.#: the tagging of 'canonical' predicates. That is, the 0.8.10++ toolkit reports canonical <= 2.4.8 model predicates as 'non-canonical'.
 - This release of the Reasoner Validator Web Service will detect TRAPI 1.0.* releases but doesn't strive to be completely backwards compatible with them (considering that TRAPI 1.0.* is totally irrelevant now). 
 - The web service validation doesn't do deep validation of the Results part of a TRAPI Message
 - The validation is only run on the first 1000 nodes and 100 edges of graphs, to keep the validation time tractable (this risks not having complete coverage of the graph)
 - Biolink Model toolkit is not (yet) cached so changing the model version during use will result in some latency in results
 - The validator service doesn't (yet) deeply validate non-core node and edge slot contents of Message Knowledge Graphs
 - The validator service doesn't (yet) attempt validation of Query Graph nodes and edges 'constraints' (e.g. `biolink:Association` etc. `domain` and `range` constraints)
```

