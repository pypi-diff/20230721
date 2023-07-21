# Comparing `tmp/sphinx_apitree-1.3.0.tar.gz` & `tmp/sphinx_apitree-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.3.0.tar` & `sphinx_apitree-1.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/LICENSE
--rw-r--r--   0        0        0     1980 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/README.md
--rw-r--r--   0        0        0      105 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/__init__.py
--rw-r--r--   0        0        0     2631 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ast_utils.py
--rw-r--r--   0        0        0     4708 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/conf_util.py
--rw-r--r--   0        0        0     1058 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/context.py
--rw-r--r--   0        0        0     1761 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/auto_ref.py
--rw-r--r--   0        0        0      808 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/docstring.py
--rw-r--r--   0        0        0     2908 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/github_link.py
--rw-r--r--   0        0        0     1691 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/html_helper.py
--rw-r--r--   0        0        0       30 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/structs.py
--rw-r--r--   0        0        0    10880 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/symbol_match.py
--rw-r--r--   0        0        0      183 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/api.md
--rw-r--r--   0        0        0       42 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/function.md
--rw-r--r--   0        0        0      154 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/module.md
--rw-r--r--   0        0        0      121 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1728 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/tree_extractor.py
--rw-r--r--   0        0        0      738 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/writer.py
--rw-r--r--   0        0        0     1556 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 sphinx_apitree-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1980 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/README.md
+-rw-r--r--   0        0        0      105 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/__init__.py
+-rw-r--r--   0        0        0     2631 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/ast_utils.py
+-rw-r--r--   0        0        0     4707 2023-07-21 14:17:56.337312 sphinx_apitree-1.3.1/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/context.py
+-rw-r--r--   0        0        0     1761 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      808 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     2908 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/html_helper.py
+-rw-r--r--   0        0        0       30 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/structs.py
+-rw-r--r--   0        0        0    10880 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/symbol_match.py
+-rw-r--r--   0        0        0      183 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/api.md
+-rw-r--r--   0        0        0       42 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/function.md
+-rw-r--r--   0        0        0      154 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/module.md
+-rw-r--r--   0        0        0      121 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-21 14:17:56.341312 sphinx_apitree-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 sphinx_apitree-1.3.1/PKG-INFO
```

### Comparing `sphinx_apitree-1.3.0/LICENSE` & `sphinx_apitree-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/README.md` & `sphinx_apitree-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/ast_utils.py` & `sphinx_apitree-1.3.1/apitree/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/conf_util.py` & `sphinx_apitree-1.3.1/apitree/conf_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     repo_dir: pathlib.Path,
     docs_dir: pathlib.Path,
     includes_paths: dict[str, str],
 ):
   for repo_path, doc_path in includes_paths.items():
     src_path = repo_dir / repo_path
     dst_path = docs_dir / doc_path
-    match repo_path.suffix:
+    match src_path.suffix:
       case '.md':
         # repo_dir.parent / 'etils'
         # Could dynamically compute the `../../../`
         content = epy.dedent(
             f"""
             ```{{include}} ../{repo_path}
             ```
```

### Comparing `sphinx_apitree-1.3.0/apitree/context.py` & `sphinx_apitree-1.3.1/apitree/context.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/ext/auto_ref.py` & `sphinx_apitree-1.3.1/apitree/ext/auto_ref.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/ext/docstring.py` & `sphinx_apitree-1.3.1/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/ext/github_link.py` & `sphinx_apitree-1.3.1/apitree/ext/github_link.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/html_helper.py` & `sphinx_apitree-1.3.1/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/symbol_match.py` & `sphinx_apitree-1.3.1/apitree/symbol_match.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/tree_extractor.py` & `sphinx_apitree-1.3.1/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/apitree/writer.py` & `sphinx_apitree-1.3.1/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/pyproject.toml` & `sphinx_apitree-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.3.0/PKG-INFO` & `sphinx_apitree-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

