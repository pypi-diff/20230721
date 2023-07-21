# Comparing `tmp/openfoodfacts-0.1.4.tar.gz` & `tmp/openfoodfacts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfoodfacts-0.1.4.tar", max compression
+gzip compressed data, was "openfoodfacts-0.1.5.tar", max compression
```

## Comparing `openfoodfacts-0.1.4.tar` & `openfoodfacts-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1182 2023-06-16 15:29:56.860611 openfoodfacts-0.1.4/LICENSE
--rw-r--r--   0        0        0     2727 2023-06-26 14:44:02.790553 openfoodfacts-0.1.4/README.md
--rw-r--r--   0        0        0      390 2023-07-19 15:55:22.032433 openfoodfacts-0.1.4/openfoodfacts/__init__.py
--rw-r--r--   0        0        0     5559 2023-06-26 14:44:02.790553 openfoodfacts-0.1.4/openfoodfacts/api.py
--rw-r--r--   0        0        0     2891 2023-06-27 08:50:51.170311 openfoodfacts-0.1.4/openfoodfacts/dataset.py
--rw-r--r--   0        0        0     4937 2023-06-26 16:02:20.944920 openfoodfacts-0.1.4/openfoodfacts/images.py
--rw-r--r--   0        0        0    36245 2023-07-19 15:16:54.735185 openfoodfacts-0.1.4/openfoodfacts/ocr.py
--rw-r--r--   0        0        0    10318 2023-07-19 15:14:53.587274 openfoodfacts-0.1.4/openfoodfacts/taxonomy.py
--rw-r--r--   0        0        0    10328 2023-06-26 16:32:09.276745 openfoodfacts-0.1.4/openfoodfacts/types.py
--rw-r--r--   0        0        0     7195 2023-07-19 15:13:28.619361 openfoodfacts-0.1.4/openfoodfacts/utils.py
--rw-r--r--   0        0        0      657 2023-07-19 16:03:48.732958 openfoodfacts-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 openfoodfacts-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1182 2023-06-16 15:29:56.860611 openfoodfacts-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2727 2023-06-26 14:44:02.790553 openfoodfacts-0.1.5/README.md
+-rw-r--r--   0        0        0      390 2023-07-21 09:57:01.715127 openfoodfacts-0.1.5/openfoodfacts/__init__.py
+-rw-r--r--   0        0        0     5559 2023-06-26 14:44:02.790553 openfoodfacts-0.1.5/openfoodfacts/api.py
+-rw-r--r--   0        0        0     2891 2023-07-20 16:21:20.006091 openfoodfacts-0.1.5/openfoodfacts/dataset.py
+-rw-r--r--   0        0        0     4937 2023-06-26 16:02:20.944920 openfoodfacts-0.1.5/openfoodfacts/images.py
+-rw-r--r--   0        0        0    36245 2023-07-19 15:16:54.735185 openfoodfacts-0.1.5/openfoodfacts/ocr.py
+-rw-r--r--   0        0        0    12671 2023-07-20 16:21:20.098092 openfoodfacts-0.1.5/openfoodfacts/taxonomy.py
+-rw-r--r--   0        0        0    10328 2023-06-26 16:32:09.276745 openfoodfacts-0.1.5/openfoodfacts/types.py
+-rw-r--r--   0        0        0     7195 2023-07-19 15:13:28.619361 openfoodfacts-0.1.5/openfoodfacts/utils.py
+-rw-r--r--   0        0        0      936 2023-07-21 09:57:01.715127 openfoodfacts-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 openfoodfacts-0.1.5/PKG-INFO
```

### Comparing `openfoodfacts-0.1.4/LICENSE` & `openfoodfacts-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/README.md` & `openfoodfacts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/api.py` & `openfoodfacts-0.1.5/openfoodfacts/api.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/dataset.py` & `openfoodfacts-0.1.5/openfoodfacts/dataset.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/images.py` & `openfoodfacts-0.1.5/openfoodfacts/images.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/ocr.py` & `openfoodfacts-0.1.5/openfoodfacts/ocr.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/taxonomy.py` & `openfoodfacts-0.1.5/openfoodfacts/taxonomy.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,14 +35,29 @@
     + "/data/taxonomies/packaging_materials.full.json",
     TaxonomyType.packaging_recycling: URLBuilder.static(Flavor.off, Environment.org)
     + "/data/taxonomies/packaging_recycling.full.json",
 }
 
 
 class TaxonomyNode:
+    """A taxonomy element.
+
+    Each node has 0+ parents and 0+ children. Each node has the following
+    attributes:
+
+    - `id`: the node identifier, it starts with a language prefix (ex: `en:`)
+    - `names`: a dict mapping language 2-letter code to the node name for this
+      language
+    - `parents`: the list of the node parents
+    - `children`: the list of the node children
+    - `properties`: additional properties of the node (taxonomy-dependent)
+    - `synonyms`: a dict mapping language 2-letter code to a list of synonyms
+      for this language
+    """
+
     __slots__ = ("id", "names", "parents", "children", "synonyms", "properties")
 
     def __init__(
         self,
         identifier: str,
         names: Dict[str, str],
         synonyms: Optional[Dict[str, List[str]]],
@@ -146,34 +161,52 @@
         return {"name": self.names, "parents": [p.id for p in self.parents]}
 
     def __repr__(self):
         return "<TaxonomyNode %s>" % self.id
 
 
 class Taxonomy:
+    """A class representing a taxonomy.
+
+    For more information about taxonomy, see
+    https://wiki.openfoodfacts.org/Global_taxonomies.
+
+    A Taxonomy instance has only a single `nodes` attribute, that maps the
+    node identifier to a `TaxonomyNode`.
+    """
+
     def __init__(self) -> None:
         self.nodes: Dict[str, TaxonomyNode] = {}
 
     def add(self, key: str, node: TaxonomyNode) -> None:
+        """Add a node to the taxonomy under the id `key`.
+
+        :param key: The node id
+        :param node: the TaxonomyNode
+        """
         self.nodes[key] = node
 
     def __contains__(self, item: str):
+        """Return True if `item` (a taxonomy id) is in the taxonomy, False
+        otherwise."""
         return item in self.nodes
 
     def __getitem__(self, item: str):
         return self.nodes.get(item)
 
-    def __len__(self):
+    def __len__(self) -> int:
+        """Return the number of items in the taxonomy."""
         return len(self.nodes)
 
     def iter_nodes(self) -> Iterable[TaxonomyNode]:
         """Iterate over the nodes of the taxonomy."""
         return iter(self.nodes.values())
 
-    def keys(self):
+    def keys(self) -> Iterable[str]:
+        """Return all node IDs from the taxonomy."""
         return self.nodes.keys()
 
     def find_deepest_nodes(self, nodes: List[TaxonomyNode]) -> List[TaxonomyNode]:
         """Given a list of nodes, returns the list of nodes where all the
         parents within the list have been removed.
 
         For example, for a taxonomy, 'fish' -> 'salmon' -> 'smoked-salmon':
@@ -219,29 +252,44 @@
 
             if candidate_node is not None:
                 to_check_nodes.add(candidate_node)
 
         return node.is_parent_of_any(to_check_nodes)
 
     def get_localized_name(self, key: str, lang: str) -> str:
+        """Return the name of a taxonomy element in a given language.
+
+        If `key` is not in the taxonomy or if no name is available for the
+        requested language, return `key`.
+
+        :param key: the taxonomy element id
+        :param lang: the 2-letter language code
+        :return: the localized name
+        """
         if key not in self.nodes:
             return key
 
         return self.nodes[key].get_localized_name(lang)
 
     def to_dict(self) -> JSONType:
+        """Generate a dict from the Taxonomy."""
         export = {}
 
         for key, node in self.nodes.items():
             export[key] = node.to_dict()
 
         return export
 
     @classmethod
     def from_dict(cls, data: JSONType) -> "Taxonomy":
+        """Create a Taxonomy from `data`.
+
+        :param data: the taxonomy as a dict
+        :return: a Taxonomy
+        """
         taxonomy = Taxonomy()
 
         for key, key_data in data.items():
             if key not in taxonomy:
                 node = TaxonomyNode(
                     identifier=key,
                     names=key_data.get("name", {}),
@@ -259,27 +307,45 @@
             parents = [taxonomy[ref] for ref in key_data.get("parents", [])]
             node.add_parents(parents)
 
         return taxonomy
 
     @classmethod
     def from_path(cls, file_path: Union[str, Path]) -> "Taxonomy":
+        """Create a Taxonomy from a JSON file.
+
+        :param file_path: a JSON file, gzipped (.json.gz) files are supported
+        :return: a Taxonomy
+        """
         return cls.from_dict(load_json(file_path))  # type: ignore
 
     @classmethod
     def from_url(
         cls, url: str, session: Optional[requests.Session] = None, timeout: int = 120
     ) -> "Taxonomy":
+        """Create a Taxonomy from a taxonomy file hosted at `url`.
+
+        :param url: the URL of the taxonomy
+        :param session: the requests session, use a default session if None
+        :param timeout: the request timeout, defaults to 120
+        :return: a Taxonomy
+        """
         session = http_session if session is None else session
         r = session.get(url, timeout=timeout)
         data = r.json()
         return cls.from_dict(data)
 
     @classmethod
     def from_type(cls, taxonomy_type: TaxonomyType) -> "Taxonomy":
+        """Create a Taxonomy from a taxonomy file hosted online from a
+        taxonomy type.
+
+        :param taxonomy_type: the taxonomy type
+        :return: a Taxonomy
+        """
         url = TAXONOMY_URLS[TaxonomyType[taxonomy_type]]
         return cls.from_url(url)
 
 
 def get_taxonomy(
     taxonomy_type: Union[TaxonomyType, str],
     force_download: bool = False,
```

### Comparing `openfoodfacts-0.1.4/openfoodfacts/types.py` & `openfoodfacts-0.1.5/openfoodfacts/types.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/openfoodfacts/utils.py` & `openfoodfacts-0.1.5/openfoodfacts/utils.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.1.4/pyproject.toml` & `openfoodfacts-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 [tool.poetry]
 name = "openfoodfacts"
-version = "0.1.4"
+version = "0.1.5"
 description = "Official Python SDK of Open Food Facts"
 authors = ["The Open Food Facts team"]
 license = "Apache 2.0"
 readme = "README.md"
 
+[tool.mypy]
+ignore_missing_imports = true
+
+[tool.isort] # From https://black.readthedocs.io/en/stable/compatible_configs.html#isort
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 88
+
 [tool.poetry.dependencies]
-python = ">=3.8.1,<=3.10"
+python = ">=3.8.1,<4.0"
 requests = ">=2.20.0"
 pydantic = ">=1.10.0,<2.0.0"
 tqdm = ">=4.0.0,<5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "1.11.0"
 flake8 = "6.0.0"
 black = "23.3.0"
 mypy = "1.3.0"
 isort = "5.12.0"
 coverage = {version = "7.2.7", extras = ["toml"]}
 pytest = "7.3.2"
-types-requests = "2.31.0.1" 
-types-tqdm = "4.65.0.1" 
+types-requests = "2.31.0.1"
+types-tqdm = "4.65.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openfoodfacts-0.1.4/PKG-INFO` & `openfoodfacts-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: openfoodfacts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Official Python SDK of Open Food Facts
 License: Apache 2.0
 Author: The Open Food Facts team
-Requires-Python: >=3.8.1,<=3.10
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.20.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Open Food Facts Python SDK
```

