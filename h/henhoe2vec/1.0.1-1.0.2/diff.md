# Comparing `tmp/henhoe2vec-1.0.1.tar.gz` & `tmp/henhoe2vec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henhoe2vec-1.0.1.tar", last modified: Tue Jun 20 13:35:26 2023, max compression
+gzip compressed data, was "henhoe2vec-1.0.2.tar", last modified: Fri Jul 21 07:56:44 2023, max compression
```

## Comparing `henhoe2vec-1.0.1.tar` & `henhoe2vec-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.502830 henhoe2vec-1.0.1/
--rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.1/LICENSE.txt
--rw-r--r--   0 bob        (501) staff       (20)     7136 2023-06-20 13:35:26.502679 henhoe2vec-1.0.1/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)     4985 2023-06-20 13:30:29.000000 henhoe2vec-1.0.1/README.md
--rw-r--r--   0 bob        (501) staff       (20)     1199 2023-06-20 13:33:41.000000 henhoe2vec-1.0.1/pyproject.toml
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-20 13:35:26.502879 henhoe2vec-1.0.1/setup.cfg
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.1/setup.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.498708 henhoe2vec-1.0.1/src/
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.500370 henhoe2vec-1.0.1/src/henhoe2vec/
--rw-r--r--   0 bob        (501) staff       (20)       78 2023-06-11 08:46:34.000000 henhoe2vec-1.0.1/src/henhoe2vec/__init__.py
--rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.1/src/henhoe2vec/alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)     2109 2023-06-20 13:32:52.000000 henhoe2vec-1.0.1/src/henhoe2vec/embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)    10636 2023-06-20 13:32:52.000000 henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.1/src/henhoe2vec/napkin.py
--rw-r--r--   0 bob        (501) staff       (20)     5262 2023-06-17 08:10:10.000000 henhoe2vec-1.0.1/src/henhoe2vec/utils.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.501401 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/
--rw-r--r--   0 bob        (501) staff       (20)     7136 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)      566 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/SOURCES.txt
--rw-r--r--   0 bob        (501) staff       (20)        1 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/dependency_links.txt
--rw-r--r--   0 bob        (501) staff       (20)       76 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/requires.txt
--rw-r--r--   0 bob        (501) staff       (20)       11 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/top_level.txt
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.502458 henhoe2vec-1.0.1/tests/
--rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.1/tests/test_henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.240456 henhoe2vec-1.0.2/
+-rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.2/LICENSE.txt
+-rw-r--r--   0 bob        (501) staff       (20)     7136 2023-07-21 07:56:44.240249 henhoe2vec-1.0.2/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)     4985 2023-06-20 13:30:29.000000 henhoe2vec-1.0.2/README.md
+-rw-r--r--   0 bob        (501) staff       (20)     1199 2023-07-21 07:56:37.000000 henhoe2vec-1.0.2/pyproject.toml
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-07-21 07:56:44.240519 henhoe2vec-1.0.2/setup.cfg
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.2/setup.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.234847 henhoe2vec-1.0.2/src/
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.237406 henhoe2vec-1.0.2/src/henhoe2vec/
+-rw-r--r--   0 bob        (501) staff       (20)       78 2023-07-21 07:52:37.000000 henhoe2vec-1.0.2/src/henhoe2vec/__init__.py
+-rw-r--r--   0 bob        (501) staff       (20)       37 2023-07-21 07:52:37.000000 henhoe2vec-1.0.2/src/henhoe2vec/__main__.py
+-rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.2/src/henhoe2vec/alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)     2109 2023-06-20 13:32:52.000000 henhoe2vec-1.0.2/src/henhoe2vec/embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)    10540 2023-07-21 07:37:30.000000 henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.2/src/henhoe2vec/napkin.py
+-rw-r--r--   0 bob        (501) staff       (20)     5314 2023-07-02 16:12:23.000000 henhoe2vec-1.0.2/src/henhoe2vec/utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.238544 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/
+-rw-r--r--   0 bob        (501) staff       (20)     7136 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)      593 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 bob        (501) staff       (20)        1 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 bob        (501) staff       (20)       76 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/requires.txt
+-rw-r--r--   0 bob        (501) staff       (20)       11 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/top_level.txt
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.239685 henhoe2vec-1.0.2/tests/
+-rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.2/tests/test_henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.2/tests/test_utils.py
```

### Comparing `henhoe2vec-1.0.1/LICENSE.txt` & `henhoe2vec-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/PKG-INFO` & `henhoe2vec-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `henhoe2vec-1.0.1/README.md` & `henhoe2vec-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/pyproject.toml` & `henhoe2vec-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "henhoe2vec"
-version = "1.0.1"
+version = "1.0.2"
 description = "Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021)."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Robert Giesler", email = "robert.giesler@rwth-aachen.de"}
 ]
```

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/alias_sampling.py` & `henhoe2vec-1.0.2/src/henhoe2vec/alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/embeddings.py` & `henhoe2vec-1.0.2/src/henhoe2vec/embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec.py` & `henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,64 +22,64 @@
 
     parser.add_argument(
         "--sep", type=str, help=("Delimiter of the input csv edge list."), default="\t"
     )
 
     parser.add_argument(
         "--header",
-        type="store_true",
+        action="store_true",
         help=("Pass this argument if the input csv edge list has a header."),
     )
 
     parser.add_argument(
-        "--output-name",
+        "--output_name",
         type=str,
         help=(
             "Name of the output .csv file (without suffix). Default is 'embeddings'."
         ),
         default="embeddings",
     )
 
     parser.add_argument(
-        "--is-directed",
+        "--is_directed",
         action="store_true",
         help="Pass this argument if the network is directed.",
     )
 
     parser.add_argument(
-        "--edges-are-distance",
+        "--edges_are_distance",
         action="store_true",
         help=(
             "Pass this argument if edge weights indicate distance between nodes"
             " (opposed to weight/similarity)."
         ),
     )
 
     parser.add_argument(
-        "--output-dir",
+        "--output_dir",
         type=str,
         help="Path of the output directory where the embedding files will be saved.",
     )
 
     parser.add_argument(
         "--dimensions",
         type=int,
         default=128,
         help="The dimensionality of the embeddings. Default is 128.",
     )
 
     parser.add_argument(
-        "--walk-length",
+        "--walk_length",
         type=int,
         default=20,
         help="Length of each random walk. Default is 20.",
     )
 
     parser.add_argument(
-        "--num-walks",
+        "--num_walks",
         type=int,
         default=10,
         help="Number of random walks to simulate for each node. Default is 10.",
     )
 
     parser.add_argument(
         "--p",
@@ -102,30 +102,30 @@
         help=(
             "Default switching parameter for layer pairs which are not specified"
             " in the --s-dict argument. Default is 1."
         ),
     )
 
     parser.add_argument(
-        "--s-dict",
+        "--s_dict",
         nargs="*",
         default=[],
         help=(
             "Switching parameters for specific layer"
             " pairs in a dict-like manner. Pass the names of layer pairs followed by"
             " their switching parameters, separated by whitespaces. E.g., if the"
             " switching parameter from layer1 to layer2 is 0.5 and the switching"
             " parameter from layer2 to layer1 is 0.7, you would pass 'layer1 layer2"
             " 0.5 layer2 layer1 0.7'. Note that layer pairs are directed. For all layer"
             " pairs which are not specified here, the default parameter --s is adopted."
         ),
     )
 
     parser.add_argument(
-        "--window-size",
+        "--window_size",
         type=int,
         default=10,
         help="Context size for the word2vec optimization. Default is 10.",
     )
 
     parser.add_argument(
         "--epochs", default=1, type=int, help="Number of epochs in SGD. Default is 1."
@@ -319,36 +319,35 @@
             workers,
             verbose,
         )
 
     finish = time.time()
     if verbose:
         print(
-            f"Completed multilayer network embedding in {finish - start} seconds."
-            f" See results in {output_dir}."
+            f"[STATUS] Completed multilayer network embedding in"
+            f" {round((finish - start), 1)} seconds. See results in {output_dir}."
         )
 
 
 def main():
-    if __name__ == "__main__":
-        args = parse_args()
-        # Parse arguments s and s-dict
-        s = parse_switching_param(args.s, args.s_dict)
-        run(
-            input_csv=args.input,
-            output_dir=args.output_dir,
-            sep=args.sep,
-            header=args.header,
-            output_name=args.output_name,
-            is_directed=args.is_directed,
-            edges_are_distance=args.edges_are_distance,
-            dims=args.dimensions,
-            walk_length=args.walk_length,
-            num_walks=args.num_walks,
-            p=args.p,
-            q=args.q,
-            s=s,
-            window_size=args.window_size,
-            epochs=args.epochs,
-            workers=args.workers,
-            verbose=True,
-        )
+    args = parse_args()
+    # Parse arguments s and s-dict
+    s = parse_switching_param(args.s, args.s_dict)
+    run(
+        input_csv=args.input,
+        output_dir=args.output_dir,
+        sep=args.sep,
+        header=args.header,
+        output_name=args.output_name,
+        is_directed=args.is_directed,
+        edges_are_distance=args.edges_are_distance,
+        dims=args.dimensions,
+        walk_length=args.walk_length,
+        num_walks=args.num_walks,
+        p=args.p,
+        q=args.q,
+        s=s,
+        window_size=args.window_size,
+        epochs=args.epochs,
+        workers=args.workers,
+        verbose=True,
+    )
```

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec_walks.py` & `henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/napkin.py` & `henhoe2vec-1.0.2/src/henhoe2vec/napkin.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec/utils.py` & `henhoe2vec-1.0.2/src/henhoe2vec/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,20 +93,23 @@
     object
         The return object of the method.
     """
     print(f"[STATUS] Started {action_desc}...")
     start = time.time()
     try:
         output = method()
-        print(f"[STATUS] Finished {action_desc} in {int(time.time() - start)} seconds")
+        print(
+            f"[STATUS] Finished {action_desc} in {round((time.time() - start), 1)}"
+            f" seconds"
+        )
         return output
     except Exception:
         print(
-            f"[ERROR] Exception while {action_desc} after {int(time.time() - start)}"
-            f" seconds"
+            f"[ERROR] Exception while {action_desc} after"
+            f" {round((time.time() - start), 1)} seconds"
         )
         raise
 
 
 def emb_to_dataframe(emb_file):
     """
     Convert an embedding file, as output from a trained word2vec model, to a pandas
```

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec.egg-info/PKG-INFO` & `henhoe2vec-1.0.2/src/henhoe2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `henhoe2vec-1.0.1/src/henhoe2vec.egg-info/SOURCES.txt` & `henhoe2vec-1.0.2/src/henhoe2vec.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 src/henhoe2vec/__init__.py
+src/henhoe2vec/__main__.py
 src/henhoe2vec/alias_sampling.py
 src/henhoe2vec/embeddings.py
 src/henhoe2vec/henhoe2vec.py
 src/henhoe2vec/henhoe2vec_walks.py
 src/henhoe2vec/napkin.py
 src/henhoe2vec/utils.py
 src/henhoe2vec.egg-info/PKG-INFO
```

### Comparing `henhoe2vec-1.0.1/tests/test_alias_sampling.py` & `henhoe2vec-1.0.2/tests/test_alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/tests/test_embeddings.py` & `henhoe2vec-1.0.2/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/tests/test_henhoe2vec.py` & `henhoe2vec-1.0.2/tests/test_henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/tests/test_henhoe2vec_walks.py` & `henhoe2vec-1.0.2/tests/test_henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.1/tests/test_utils.py` & `henhoe2vec-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

