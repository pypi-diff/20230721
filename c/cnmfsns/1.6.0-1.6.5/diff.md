# Comparing `tmp/cnmfsns-1.6.0.tar.gz` & `tmp/cnmfsns-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.6.0.tar", last modified: Mon Jul 10 18:03:45 2023, max compression
+gzip compressed data, was "cnmfsns-1.6.5.tar", last modified: Fri Jul 21 16:11:48 2023, max compression
```

## Comparing `cnmfsns-1.6.0.tar` & `cnmfsns-1.6.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     4320 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3805 2023-07-10 16:56:05.000000 cnmfsns-1.6.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      980 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.447642 cnmfsns-1.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.479030 cnmfsns-1.6.0/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.6.0/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    52096 2023-07-10 16:41:48.000000 cnmfsns-1.6.0/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.6.0/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    36423 2023-07-10 18:02:42.000000 cnmfsns-1.6.0/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.6.0/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    59662 2023-07-10 17:04:09.000000 cnmfsns-1.6.0/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.6.0/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-07-10 02:54:46.000000 cnmfsns-1.6.0/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     4320 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:48.063226 cnmfsns-1.6.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0     4320 2023-07-21 16:11:48.063226 cnmfsns-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2023-07-21 16:02:46.000000 cnmfsns-1.6.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0      980 2023-07-21 16:11:48.063226 cnmfsns-1.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:48.030243 cnmfsns-1.6.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:48.046501 cnmfsns-1.6.5/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.6.5/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    52492 2023-07-21 16:08:05.000000 cnmfsns-1.6.5/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.6.5/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.6.5/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-07-18 03:10:45.000000 cnmfsns-1.6.5/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    36407 2023-07-19 20:10:17.000000 cnmfsns-1.6.5/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.6.5/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    59662 2023-07-10 17:04:09.000000 cnmfsns-1.6.5/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    41881 2023-07-21 16:04:07.000000 cnmfsns-1.6.5/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-07-10 02:54:46.000000 cnmfsns-1.6.5/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:48.063226 cnmfsns-1.6.5/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     4320 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 16:11:48.000000 cnmfsns-1.6.5/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.6.0/LICENSE` & `cnmfsns-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/PKG-INFO` & `cnmfsns-1.6.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.6.0
+Version: 1.6.5
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.6.0-blue)
+![version badge](https://img.shields.io/badge/version-1.6.5-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.6.0/README.md` & `cnmfsns-1.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e36 2e30 2d62 6c75  ersion-1.6.0-blu
+000000b0: 6572 7369 6f6e 2d31 2e36 2e35 2d62 6c75  ersion-1.6.5-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.6.0/setup.cfg` & `cnmfsns-1.6.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 362e 300d 0a61 7574  ion = 1.6.0..aut
+00000020: 696f 6e20 3d20 312e 362e 350d 0a61 7574  ion = 1.6.5..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.6.0/src/cnmfsns/__init__.py` & `cnmfsns-1.6.5/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/cli.py` & `cnmfsns-1.6.5/src/cnmfsns/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,19 @@
     help="Output directory for cNMF-SNS results generated using `cnmfsns integrate`")
 @click.option(
     '-n', '--name', type=str, default=datetime.strftime(datetime.now(), "%Y-%m-%d_%H%M%S"),
     help="Name for this network. Output from this step will be in [output_dir]/sns_networks/[name]/...")
 @click.option(
     '-c', '--config_toml', type=click.Path(exists=True, dir_okay=False), 
     help="TOML config file. Defaults to file output from `cnmfsns integrate` step: [output_dir]/integrate/config.toml")
-def cmd_create_network(output_dir, name, config_toml):
+@click.option(
+    '-m', '--communities_toml', type=click.Path(exists=True, dir_okay=False), 
+    help="TOML file containing communities from a previous run. This file overrides community discovery according to parameters in the config TOML file.")
+
+def cmd_create_network(output_dir, name, config_toml, communities_toml):
     """
     Create network integration.
     """
     utils.start_logging(os.path.join(output_dir, "logfile.txt"))
 
     if config_toml is None:
         config = Config.from_toml(os.path.join(output_dir, "integrate", "config.toml"))
@@ -590,19 +594,25 @@
     if config.sns["subset_nodes"] == "none":
         subset_nodes = None
     else:
         subset_nodes = config.sns["subset_nodes"]
         
     snsmap = SNS(integration=integration, subset_nodes=subset_nodes)
     
-    community_algorithm = config.sns["community_algorithm"]
-    snsmap.community_search(algorithm=community_algorithm,
-                            resolution=config.sns["communities"][community_algorithm]["resolution"])
+
+    if communities_toml is None:
+        community_algorithm = config.sns["community_algorithm"]
+        snsmap.community_search(algorithm=community_algorithm,
+                                resolution=config.sns["communities"][community_algorithm]["resolution"])
+    else:
+        snsmap.read_communities_from_toml(communities_toml)
     nx.write_graphml(snsmap.gep_graph, os.path.join(sns_output_dir, "gep_graph.graphml"))
 
+
+
     snsmap.compute_layout(
         algorithm=config.sns["layout_algorithm"],
         shared_community_weight = config.sns["layouts"]["community_weighted_spring"]["within_community"],
         shared_dataset_weight = config.sns["layouts"]["community_weighted_spring"]["within_dataset"]
     )
     snsmap.compute_community_network_layout()
```

### Comparing `cnmfsns-1.6.0/src/cnmfsns/cnmf.py` & `cnmfsns-1.6.5/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/colors.py` & `cnmfsns-1.6.5/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/config.py` & `cnmfsns-1.6.5/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/dataset.py` & `cnmfsns-1.6.5/src/cnmfsns/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,1629 +649,1628 @@
 00002880: 626f 6f6c 2076 616c 7565 7320 746f 2073  bool values to s
 00002890: 7472 696e 6773 2061 7320 7468 6573 6520  trings as these 
 000028a0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
 000028b0: 6420 6279 2041 6e6e 4461 7461 206f 6e2d  d by AnnData on-
 000028c0: 6469 736b 2066 6f72 6d61 740d 0a20 2020  disk format..   
 000028d0: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
 000028e0: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
-000028f0: 7328 696e 636c 7564 653d 226f 626a 6563  s(include="objec
-00002900: 7422 292e 636f 6c75 6d6e 733a 0d0a 2020  t").columns:..  
-00002910: 2020 2020 2020 2020 2020 6f62 735b 636f            obs[co
-00002920: 6c5d 203d 206f 6273 5b63 6f6c 5d2e 7265  l] = obs[col].re
-00002930: 706c 6163 6528 7b54 7275 653a 2022 5472  place({True: "Tr
-00002940: 7565 222c 2046 616c 7365 3a20 2246 616c  ue", False: "Fal
-00002950: 7365 227d 292e 6173 7479 7065 2822 6361  se"}).astype("ca
-00002960: 7465 676f 7279 2229 0d0a 2020 2020 2020  tegory")..      
-00002970: 2020 6d69 7373 696e 675f 7361 6d70 6c65    missing_sample
-00002980: 735f 696e 5f58 203d 206f 6273 2e69 6e64  s_in_X = obs.ind
-00002990: 6578 2e64 6966 6665 7265 6e63 6528 7365  ex.difference(se
-000029a0: 6c66 2e61 6461 7461 2e6f 6273 2e69 6e64  lf.adata.obs.ind
-000029b0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
-000029c0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
-000029d0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
-000029e0: 6d70 6c65 735f 696e 5f58 3a0d 0a20 2020  mples_in_X:..   
-000029f0: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-00002a00: 2e77 6172 6e69 6e67 2822 5468 6520 666f  .warning("The fo
-00002a10: 6c6c 6f77 696e 6720 7361 6d70 6c65 7320  llowing samples 
-00002a20: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
-00002a30: 7765 7265 206e 6f74 2070 7265 7365 6e74  were not present
-00002a40: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
-00002a50: 6461 7461 2e58 6029 3a5c 6e20 202d 2022  data.X`):\n  - "
-00002a60: 202b 2022 5c6e 2020 2d20 222e 6a6f 696e   + "\n  - ".join
-00002a70: 286d 6973 7369 6e67 5f73 616d 706c 6573  (missing_samples
-00002a80: 5f69 6e5f 5829 290d 0a20 2020 2020 2020  _in_X))..       
-00002a90: 206d 6973 7369 6e67 5f73 616d 706c 6573   missing_samples
-00002aa0: 5f69 6e5f 6d64 203d 2073 656c 662e 6164  _in_md = self.ad
-00002ab0: 6174 612e 6f62 732e 696e 6465 782e 6469  ata.obs.index.di
-00002ac0: 6666 6572 656e 6365 286f 6273 2e69 6e64  fference(obs.ind
-00002ad0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
-00002ae0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
-00002af0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
-00002b00: 6d70 6c65 735f 696e 5f6d 643a 0d0a 2020  mples_in_md:..  
-00002b10: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-00002b20: 672e 7761 726e 696e 6728 2254 6865 2066  g.warning("The f
-00002b30: 6f6c 6c6f 7769 6e67 2073 616d 706c 6573  ollowing samples
-00002b40: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
-00002b50: 6461 7461 2e58 6029 2077 6572 6520 6162  data.X`) were ab
-00002b60: 7365 6e74 2069 6e20 7468 6520 6d65 7461  sent in the meta
-00002b70: 6461 7461 3a5c 6e20 202d 2022 202b 2022  data:\n  - " + "
-00002b80: 5c6e 2020 2d20 222e 6a6f 696e 286d 6973  \n  - ".join(mis
-00002b90: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
-00002ba0: 6d64 2929 0d0a 2020 2020 2020 2020 7365  md))..        se
-00002bb0: 6c66 2e61 6461 7461 2e6f 6273 203d 206f  lf.adata.obs = o
-00002bc0: 6273 2e72 6569 6e64 6578 2873 656c 662e  bs.reindex(self.
-00002bd0: 6164 6174 612e 6f62 732e 696e 6465 7829  adata.obs.index)
-00002be0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00002bf0: 6765 745f 6d65 7461 6461 7461 5f74 7970  get_metadata_typ
-00002c00: 655f 7375 6d6d 6172 7928 7365 6c66 293a  e_summary(self):
-00002c10: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-00002c20: 7572 6e20 6120 7072 696e 7461 626c 6520  urn a printable 
-00002c30: 7375 6d6d 6172 7920 6f66 206d 6574 6164  summary of metad
-00002c40: 6174 6120 616e 6420 7661 6c75 6520 7479  ata and value ty
-00002c50: 7065 7320 666f 7220 6561 6368 206d 6574  pes for each met
-00002c60: 6164 6174 6120 6c61 7965 722e 0d0a 0d0a  adata layer.....
-00002c70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00002c80: 2053 756d 6d61 7279 206f 6620 6d65 7461   Summary of meta
-00002c90: 6461 7461 0d0a 2020 2020 2020 2020 3a72  data..        :r
-00002ca0: 7479 7065 3a20 7374 720d 0a20 2020 2020  type: str..     
-00002cb0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002cc0: 6d73 6720 3d20 2222 0d0a 2020 2020 2020  msg = ""..      
-00002cd0: 2020 666f 7220 636f 6c20 696e 2073 656c    for col in sel
-00002ce0: 662e 6164 6174 612e 6f62 732e 636f 6c75  f.adata.obs.colu
-00002cf0: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
-00002d00: 2020 6d73 6720 2b3d 2022 2020 2020 436f    msg += "    Co
-00002d10: 6c75 6d6e 3a20 2220 2b20 636f 6c20 2b20  lumn: " + col + 
-00002d20: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
-00002d30: 2020 666f 7220 7661 6c75 655f 7479 7065    for value_type
-00002d40: 2c20 636f 756e 7420 696e 2073 656c 662e  , count in self.
-00002d50: 6164 6174 612e 6f62 735b 636f 6c5d 2e64  adata.obs[col].d
-00002d60: 726f 706e 6128 292e 6d61 7028 7479 7065  ropna().map(type
-00002d70: 292e 7661 6c75 655f 636f 756e 7473 2829  ).value_counts()
-00002d80: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00002d90: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
-00002da0: 3d20 6622 2020 2020 2020 2020 7b76 616c  = f"        {val
-00002db0: 7565 5f74 7970 657d 3a20 7b63 6f75 6e74  ue_type}: {count
-00002dc0: 7d5c 6e22 0d0a 2020 2020 2020 2020 7265  }\n"..        re
-00002dd0: 7475 726e 206d 7367 0d0a 2020 2020 0d0a  turn msg..    ..
-00002de0: 2020 2020 6465 6620 7772 6974 655f 6835      def write_h5
-00002df0: 6164 2873 656c 662c 0d0a 2020 2020 2020  ad(self,..      
-00002e00: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00002e10: 656e 616d 653a 2073 7472 293a 0d0a 2020  ename: str):..  
-00002e20: 2020 2020 2020 2222 2257 7269 7465 2064        """Write d
-00002e30: 6174 6173 6574 2074 6f20 2e68 3561 6420  ataset to .h5ad 
-00002e40: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
-00002e50: 203a 7061 7261 6d20 6669 6c65 6e61 6d65   :param filename
-00002e60: 3a20 6669 6c65 7061 7468 0d0a 2020 2020  : filepath..    
-00002e70: 2020 2020 3a74 7970 6520 6669 6c65 6e61      :type filena
-00002e80: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
-00002e90: 2022 2222 0d0a 2020 2020 2020 2020 6669   """..        fi
-00002ea0: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
-00002eb0: 2e61 6273 7061 7468 2866 696c 656e 616d  .abspath(filenam
-00002ec0: 6529 0d0a 2020 2020 2020 2020 6c6f 6767  e)..        logg
-00002ed0: 696e 672e 696e 666f 2866 2257 7269 7469  ing.info(f"Writi
-00002ee0: 6e67 2074 6f20 7b66 696c 656e 616d 657d  ng to {filename}
-00002ef0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00002f00: 2e61 6461 7461 2e77 7269 7465 5f68 3561  .adata.write_h5a
-00002f10: 6428 6669 6c65 6e61 6d65 290d 0a20 2020  d(filename)..   
-00002f20: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
-00002f30: 6f28 6622 446f 6e65 2229 0d0a 2020 2020  o(f"Done")..    
-00002f40: 0d0a 2020 2020 6465 6620 746f 5f64 6628  ..    def to_df(
-00002f50: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00002f60: 2020 2020 206e 6f72 6d61 6c69 7a65 643a       normalized:
-00002f70: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
-00002f80: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-00002f90: 6461 7461 206d 6174 7269 7820 6173 2061  data matrix as a
-00002fa0: 2060 7064 2e44 6174 6146 7261 6d65 600d   `pd.DataFrame`.
-00002fb0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00002fc0: 6d20 6e6f 726d 616c 697a 6564 3a20 5365  m normalized: Se
-00002fd0: 7420 7472 7565 2066 6f72 2054 504d 206e  t true for TPM n
-00002fe0: 6f72 6d61 6c69 7a65 6420 6f75 7470 7574  ormalized output
-00002ff0: 2c20 6465 6661 756c 7473 2074 6f20 4661  , defaults to Fa
-00003000: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
-00003010: 7065 206e 6f72 6d61 6c69 7a65 643a 2062  pe normalized: b
-00003020: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
-00003030: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00003040: 6f62 7365 7276 6174 696f 6e73 20c3 9720  observations .. 
-00003050: 7661 7269 6162 6c65 7320 6461 7461 206d  variables data m
-00003060: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
-00003070: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
-00003080: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
-00003090: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
-000030a0: 656c 662e 6164 6174 612e 746f 5f64 6628  elf.adata.to_df(
-000030b0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-000030c0: 726d 616c 697a 6564 2061 6e64 206e 6f74  rmalized and not
-000030d0: 2073 656c 662e 6973 5f6e 6f72 6d61 6c69   self.is_normali
-000030e0: 7a65 643a 0d0a 2020 2020 2020 2020 2020  zed:..          
-000030f0: 2020 6466 203d 2064 662e 6469 7628 6466    df = df.div(df
-00003100: 2e73 756d 2861 7869 733d 3129 2c20 6178  .sum(axis=1), ax
-00003110: 6973 3d30 2920 2a20 3165 3620 2023 2054  is=0) * 1e6  # T
-00003120: 504d 206e 6f72 6d61 6c69 7a61 7469 6f6e  PM normalization
-00003130: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003140: 2064 660d 0a20 2020 2020 2020 200d 0a20   df..        .. 
-00003150: 2020 2064 6566 2072 656d 6f76 655f 756e     def remove_un
-00003160: 6661 6374 6f72 697a 6162 6c65 5f67 656e  factorizable_gen
-00003170: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
-00003180: 2020 2022 2222 5265 6d6f 7665 7320 6765     """Removes ge
-00003190: 6e65 7320 7769 7468 206d 6973 7369 6e67  nes with missing
-000031a0: 2076 616c 7565 7320 6f72 207a 6572 6f20   values or zero 
-000031b0: 7661 7269 616e 6365 2066 726f 6d20 7468  variance from th
-000031c0: 6520 6461 7461 206d 6174 7269 782e 0d0a  e data matrix...
-000031d0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000031e0: 2020 2020 2064 6620 3d20 7365 6c66 2e74       df = self.t
-000031f0: 6f5f 6466 286e 6f72 6d61 6c69 7a65 643d  o_df(normalized=
-00003200: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-00003210: 2320 4368 6563 6b20 666f 7220 7661 7269  # Check for vari
-00003220: 6162 6c65 7320 7769 7468 206d 6973 7369  ables with missi
-00003230: 6e67 2076 616c 7565 730d 0a20 2020 2020  ng values..     
-00003240: 2020 2067 656e 6573 5f77 6974 685f 6d69     genes_with_mi
-00003250: 7373 696e 6776 616c 7565 7320 3d20 6466  ssingvalues = df
-00003260: 2e69 736e 756c 6c28 292e 616e 7928 290d  .isnull().any().
-00003270: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00003280: 2020 2069 6620 6765 6e65 735f 7769 7468     if genes_with
-00003290: 5f6d 6973 7369 6e67 7661 6c75 6573 2e61  _missingvalues.a
-000032a0: 6e79 2829 3a0d 0a20 2020 2020 2020 2020  ny():..         
-000032b0: 2020 206e 5f6d 6973 7369 6e67 203d 2067     n_missing = g
-000032c0: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
-000032d0: 6776 616c 7565 732e 7375 6d28 290d 0a20  gvalues.sum().. 
-000032e0: 2020 2020 2020 2020 2020 206c 6f67 6769             loggi
-000032f0: 6e67 2e77 6172 6e69 6e67 2866 227b 6e5f  ng.warning(f"{n_
-00003300: 6d69 7373 696e 677d 206f 6620 7b73 656c  missing} of {sel
-00003310: 662e 6164 6174 612e 6e5f 7661 7273 7d20  f.adata.n_vars} 
-00003320: 7661 7269 6162 6c65 7320 6172 6520 6d69  variables are mi
-00003330: 7373 696e 6720 7661 6c75 6573 2028 6061  ssing values (`a
-00003340: 6461 7461 2e58 6029 2e22 290d 0a20 2020  data.X`).")..   
-00003350: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-00003360: 2e77 6172 6e69 6e67 2866 2253 7562 7365  .warning(f"Subse
-00003370: 7474 696e 6720 7661 7269 6162 6c65 7320  tting variables 
-00003380: 746f 2074 686f 7365 2077 6974 6820 6e6f  to those with no
-00003390: 206d 6973 7369 6e67 2076 616c 7565 732e   missing values.
-000033a0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-000033b0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-000033c0: 4368 6563 6b20 666f 7220 6765 6e65 7320  Check for genes 
-000033d0: 7769 7468 207a 6572 6f20 7661 7269 616e  with zero varian
-000033e0: 6365 0d0a 2020 2020 2020 2020 7a65 726f  ce..        zero
-000033f0: 7661 7267 656e 6573 203d 2028 6466 2e76  vargenes = (df.v
-00003400: 6172 2829 203d 3d20 3029 0d0a 2020 2020  ar() == 0)..    
-00003410: 2020 2020 6966 207a 6572 6f76 6172 6765      if zerovarge
-00003420: 6e65 732e 616e 7928 293a 0d0a 2020 2020  nes.any():..    
-00003430: 2020 2020 2020 2020 6e5f 7a65 726f 7661          n_zerova
-00003440: 7220 3d20 7a65 726f 7661 7267 656e 6573  r = zerovargenes
-00003450: 2e73 756d 2829 0d0a 2020 2020 2020 2020  .sum()..        
-00003460: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
-00003470: 696e 6728 6622 7b6e 5f7a 6572 6f76 6172  ing(f"{n_zerovar
-00003480: 7d20 6f66 207b 7365 6c66 2e61 6461 7461  } of {self.adata
-00003490: 2e6e 5f76 6172 737d 2076 6172 6961 626c  .n_vars} variabl
-000034a0: 6573 2068 6176 6520 6120 7661 7269 616e  es have a varian
-000034b0: 6365 206f 6620 7a65 726f 2069 6e20 636f  ce of zero in co
-000034c0: 756e 7473 2064 6174 6120 2860 6164 6174  unts data (`adat
-000034d0: 612e 7261 772e 5860 292e 2229 0d0a 2020  a.raw.X`).")..  
-000034e0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-000034f0: 672e 7761 726e 696e 6728 6622 5375 6273  g.warning(f"Subs
-00003500: 6574 7469 6e67 2076 6172 6961 626c 6573  etting variables
-00003510: 2074 6f20 7468 6f73 6520 7769 7468 206e   to those with n
-00003520: 6f6e 7a65 726f 2076 6172 6961 6e63 652e  onzero variance.
-00003530: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
-00003540: 2020 2020 2020 6765 6e65 735f 746f 5f6b        genes_to_k
-00003550: 6565 7020 3d20 287e 6765 6e65 735f 7769  eep = (~genes_wi
-00003560: 7468 5f6d 6973 7369 6e67 7661 6c75 6573  th_missingvalues
-00003570: 2920 2620 287e 7a65 726f 7661 7267 656e  ) & (~zerovargen
-00003580: 6573 290d 0a20 2020 2020 2020 200d 0a20  es)..        .. 
-00003590: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-000035a0: 6120 3d20 7365 6c66 2e61 6461 7461 5b3a  a = self.adata[:
-000035b0: 2c67 656e 6573 5f74 6f5f 6b65 6570 5d0d  ,genes_to_keep].
-000035c0: 0a0d 0a20 2020 2064 6566 2063 6f6d 7075  ...    def compu
-000035d0: 7465 5f67 656e 655f 7374 6174 7328 7365  te_gene_stats(se
-000035e0: 6c66 2c20 6f64 675f 6465 6661 756c 745f  lf, odg_default_
-000035f0: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
-00003600: 6e74 203d 2033 2c20 6f64 675f 6465 6661  nt = 3, odg_defa
-00003610: 756c 745f 646f 663a 2069 6e74 203d 2038  ult_dof: int = 8
-00003620: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00003630: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
-00003640: 7320 6765 6e65 2073 7461 7469 7374 6963  s gene statistic
-00003650: 7320 616e 6420 6669 7473 2074 776f 206d  s and fits two m
-00003660: 6f64 656c 7320 6f66 206d 6561 6e20 616e  odels of mean an
-00003670: 6420 7661 7269 616e 6365 206f 6620 6765  d variance of ge
-00003680: 6e65 7320 696e 2074 6865 2064 6174 6173  nes in the datas
-00003690: 6574 2e20 5468 6520 6669 7273 7420 6d65  et. The first me
-000036a0: 7468 6f64 2069 7320 7468 650d 0a20 2020  thod is the..   
-000036b0: 2020 2020 2067 656e 6572 616c 697a 6564       generalized
-000036c0: 2061 6464 6974 6976 6520 6d6f 6465 6c20   additive model 
-000036d0: 7769 7468 2073 6d6f 6f74 6820 636f 6d70  with smooth comp
-000036e0: 6f6e 656e 7473 2028 422d 7370 6c69 6e65  onents (B-spline
-000036f0: 7329 2074 6f20 6d6f 6465 6c20 7468 6520  s) to model the 
-00003700: 7265 6c61 7469 6f6e 7368 6970 206f 6620  relationship of 
-00003710: 6d65 616e 2061 6e64 2076 6172 6961 6e63  mean and varianc
-00003720: 650d 0a20 2020 2020 2020 2062 6574 7765  e..        betwe
-00003730: 656e 2067 656e 6573 2069 6e20 7468 6520  en genes in the 
-00003740: 6461 7461 7365 742e 2049 7420 7072 6f64  dataset. It prod
-00003750: 7563 6573 2061 6e20 6f64 7363 6f72 6520  uces an odscore 
-00003760: 6d65 7472 6963 2066 6f72 206f 7665 7264  metric for overd
-00003770: 6973 7065 7273 696f 6e2e 2054 6865 2073  ispersion. The s
-00003780: 6563 6f6e 6420 6973 2074 6865 2063 6f75  econd is the cou
-00003790: 6e74 2d73 7461 7469 7374 6963 730d 0a20  nt-statistics.. 
-000037a0: 2020 2020 2020 206d 6574 686f 6420 666f         method fo
-000037b0: 756e 6420 696e 2074 6865 2063 4e4d 4620  und in the cNMF 
-000037c0: 7061 636b 6167 652c 2077 6869 6368 2070  package, which p
-000037d0: 726f 6475 6365 7320 6120 6d6f 6469 6669  roduces a modifi
-000037e0: 6564 2076 2d73 636f 7265 206d 6574 7269  ed v-score metri
-000037f0: 632e 2041 6c6c 2067 656e 6520 7374 6174  c. All gene stat
-00003800: 6973 7469 6373 2061 7265 2073 746f 7265  istics are store
-00003810: 6420 7769 7468 696e 2074 6865 0d0a 2020  d within the..  
-00003820: 2020 2020 2020 6461 7461 7365 7420 6f62        dataset ob
-00003830: 6a65 6374 2061 6e64 2061 7265 2061 6363  ject and are acc
-00003840: 6573 7369 626c 6520 7573 696e 6720 6064  essible using `d
-00003850: 6174 6173 6574 2e61 6e6e 6461 7461 2e76  ataset.anndata.v
-00003860: 6172 602e 0d0a 0d0a 2020 2020 2020 2020  ar`.....        
-00003870: 3a70 6172 616d 206f 6467 5f64 6566 6175  :param odg_defau
-00003880: 6c74 5f73 706c 696e 655f 6465 6772 6565  lt_spline_degree
-00003890: 3a20 422d 5370 6c69 6e65 2064 6567 7265  : B-Spline degre
-000038a0: 6520 666f 7220 474c 4d2d 4741 4d20 6d6f  e for GLM-GAM mo
-000038b0: 6465 6c6c 696e 6720 6f66 206d 6561 6e2d  delling of mean-
-000038c0: 7661 7269 616e 6365 2072 656c 6174 696f  variance relatio
-000038d0: 6e73 6869 702c 2064 6566 6175 6c74 7320  nship, defaults 
-000038e0: 746f 2033 0d0a 2020 2020 2020 2020 3a74  to 3..        :t
-000038f0: 7970 6520 6f64 675f 6465 6661 756c 745f  ype odg_default_
-00003900: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
-00003910: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
-00003920: 2020 2020 2020 3a70 6172 616d 206f 6467        :param odg
-00003930: 5f64 6566 6175 6c74 5f64 6f66 3a20 4465  _default_dof: De
-00003940: 6772 6565 7320 6f66 2066 7265 6564 6f6d  grees of freedom
-00003950: 2066 6f72 2047 4c4d 2d47 414d 206d 6f64   for GLM-GAM mod
-00003960: 656c 6c69 6e67 206f 6620 6d65 616e 2d76  elling of mean-v
-00003970: 6172 616e 6365 2c20 6465 6661 756c 7473  arance, defaults
-00003980: 2074 6f20 380d 0a20 2020 2020 2020 203a   to 8..        :
-00003990: 7479 7065 206f 6467 5f64 6566 6175 6c74  type odg_default
-000039a0: 5f64 6f66 3a20 696e 742c 206f 7074 696f  _dof: int, optio
-000039b0: 6e61 6c0d 0a20 2020 2020 2020 2022 2222  nal..        """
-000039c0: 0d0a 2020 2020 2020 2020 6461 7461 5f72  ..        data_r
-000039d0: 6177 203d 2073 656c 662e 746f 5f64 6628  aw = self.to_df(
-000039e0: 290d 0a20 2020 2020 2020 2064 6174 615f  )..        data_
-000039f0: 6e6f 726d 616c 697a 6564 203d 2073 656c  normalized = sel
-00003a00: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
-00003a10: 6564 3d54 7275 6529 0d0a 2020 2020 2020  ed=True)..      
-00003a20: 2020 0d0a 2020 2020 2020 2020 2320 6372    ..        # cr
-00003a30: 6561 7465 2064 6174 6166 7261 6d65 206f  eate dataframe o
-00003a40: 6620 7065 722d 6765 6e65 2073 7461 7469  f per-gene stati
-00003a50: 7374 6963 730d 0a20 2020 2020 2020 2073  stics..        s
-00003a60: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
-00003a70: 6561 6e22 5d20 3d20 6461 7461 5f6e 6f72  ean"] = data_nor
-00003a80: 6d61 6c69 7a65 642e 6d65 616e 2829 0d0a  malized.mean()..
-00003a90: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00003aa0: 7461 2e76 6172 5b22 7261 6e6b 5f6d 6561  ta.var["rank_mea
-00003ab0: 6e22 5d20 3d20 7365 6c66 2e61 6461 7461  n"] = self.adata
-00003ac0: 2e76 6172 5b22 6d65 616e 225d 2e72 616e  .var["mean"].ran
-00003ad0: 6b28 290d 0a20 2020 2020 2020 2073 656c  k()..        sel
-00003ae0: 662e 6164 6174 612e 7661 725b 2276 6172  f.adata.var["var
-00003af0: 6961 6e63 6522 5d20 3d20 6461 7461 5f6e  iance"] = data_n
-00003b00: 6f72 6d61 6c69 7a65 642e 7661 7228 290d  ormalized.var().
-00003b10: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00003b20: 6174 612e 7661 725b 2273 6422 5d20 3d20  ata.var["sd"] = 
-00003b30: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
-00003b40: 7374 6428 290d 0a20 2020 2020 2020 2073  std()..        s
-00003b50: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
-00003b60: 6973 7369 6e67 6e65 7373 225d 203d 2064  issingness"] = d
-00003b70: 6174 615f 6e6f 726d 616c 697a 6564 2e69  ata_normalized.i
-00003b80: 736e 756c 6c28 292e 7375 6d28 2920 2f20  snull().sum() / 
-00003b90: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
-00003ba0: 7368 6170 655b 305d 0d0a 2020 2020 2020  shape[0]..      
-00003bb0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
-00003bc0: 5b5b 226c 6f67 5f6d 6561 6e22 2c20 226c  [["log_mean", "l
-00003bd0: 6f67 5f76 6172 6961 6e63 6522 5d5d 203d  og_variance"]] =
-00003be0: 206e 702e 6c6f 6731 3028 7365 6c66 2e61   np.log10(self.a
-00003bf0: 6461 7461 2e76 6172 5b5b 226d 6561 6e22  data.var[["mean"
-00003c00: 2c20 2276 6172 6961 6e63 6522 5d5d 290d  , "variance"]]).
-00003c10: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00003c20: 6174 612e 7661 725b 226d 6561 6e5f 636f  ata.var["mean_co
-00003c30: 756e 7473 225d 203d 2064 6174 615f 7261  unts"] = data_ra
-00003c40: 772e 6d65 616e 2829 0d0a 2020 2020 2020  w.mean()..      
-00003c50: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
-00003c60: 5b22 6f64 7363 6f72 655f 6578 636c 7564  ["odscore_exclud
-00003c70: 6564 225d 203d 2028 2873 656c 662e 6164  ed"] = ((self.ad
-00003c80: 6174 612e 7661 725b 226d 6973 7369 6e67  ata.var["missing
-00003c90: 6e65 7373 225d 203e 2030 2920 7c0d 0a20  ness"] > 0) |.. 
+000028f0: 7328 696e 636c 7564 653d 2822 626f 6f6c  s(include=("bool
+00002900: 222c 2022 6f62 6a65 6374 2229 292e 636f  ", "object")).co
+00002910: 6c75 6d6e 733a 0d0a 2020 2020 2020 2020  lumns:..        
+00002920: 2020 2020 6f62 735b 636f 6c5d 203d 206f      obs[col] = o
+00002930: 6273 5b63 6f6c 5d2e 6173 7479 7065 2822  bs[col].astype("
+00002940: 7374 7222 292e 6173 7479 7065 2822 6361  str").astype("ca
+00002950: 7465 676f 7279 2229 0d0a 2020 2020 2020  tegory")..      
+00002960: 2020 6d69 7373 696e 675f 7361 6d70 6c65    missing_sample
+00002970: 735f 696e 5f58 203d 206f 6273 2e69 6e64  s_in_X = obs.ind
+00002980: 6578 2e64 6966 6665 7265 6e63 6528 7365  ex.difference(se
+00002990: 6c66 2e61 6461 7461 2e6f 6273 2e69 6e64  lf.adata.obs.ind
+000029a0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
+000029b0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
+000029c0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
+000029d0: 6d70 6c65 735f 696e 5f58 3a0d 0a20 2020  mples_in_X:..   
+000029e0: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+000029f0: 2e77 6172 6e69 6e67 2822 5468 6520 666f  .warning("The fo
+00002a00: 6c6c 6f77 696e 6720 7361 6d70 6c65 7320  llowing samples 
+00002a10: 696e 2074 6865 206d 6574 6164 6174 6120  in the metadata 
+00002a20: 7765 7265 206e 6f74 2070 7265 7365 6e74  were not present
+00002a30: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
+00002a40: 6461 7461 2e58 6029 3a5c 6e20 202d 2022  data.X`):\n  - "
+00002a50: 202b 2022 5c6e 2020 2d20 222e 6a6f 696e   + "\n  - ".join
+00002a60: 286d 6973 7369 6e67 5f73 616d 706c 6573  (missing_samples
+00002a70: 5f69 6e5f 5829 290d 0a20 2020 2020 2020  _in_X))..       
+00002a80: 206d 6973 7369 6e67 5f73 616d 706c 6573   missing_samples
+00002a90: 5f69 6e5f 6d64 203d 2073 656c 662e 6164  _in_md = self.ad
+00002aa0: 6174 612e 6f62 732e 696e 6465 782e 6469  ata.obs.index.di
+00002ab0: 6666 6572 656e 6365 286f 6273 2e69 6e64  fference(obs.ind
+00002ac0: 6578 292e 6173 7479 7065 2873 7472 292e  ex).astype(str).
+00002ad0: 746f 5f6c 6973 7428 290d 0a20 2020 2020  to_list()..     
+00002ae0: 2020 2069 6620 6d69 7373 696e 675f 7361     if missing_sa
+00002af0: 6d70 6c65 735f 696e 5f6d 643a 0d0a 2020  mples_in_md:..  
+00002b00: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+00002b10: 672e 7761 726e 696e 6728 2254 6865 2066  g.warning("The f
+00002b20: 6f6c 6c6f 7769 6e67 2073 616d 706c 6573  ollowing samples
+00002b30: 2069 6e20 7468 6520 6461 7461 2028 6061   in the data (`a
+00002b40: 6461 7461 2e58 6029 2077 6572 6520 6162  data.X`) were ab
+00002b50: 7365 6e74 2069 6e20 7468 6520 6d65 7461  sent in the meta
+00002b60: 6461 7461 3a5c 6e20 202d 2022 202b 2022  data:\n  - " + "
+00002b70: 5c6e 2020 2d20 222e 6a6f 696e 286d 6973  \n  - ".join(mis
+00002b80: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
+00002b90: 6d64 2929 0d0a 2020 2020 2020 2020 7365  md))..        se
+00002ba0: 6c66 2e61 6461 7461 2e6f 6273 203d 206f  lf.adata.obs = o
+00002bb0: 6273 2e72 6569 6e64 6578 2873 656c 662e  bs.reindex(self.
+00002bc0: 6164 6174 612e 6f62 732e 696e 6465 7829  adata.obs.index)
+00002bd0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00002be0: 6765 745f 6d65 7461 6461 7461 5f74 7970  get_metadata_typ
+00002bf0: 655f 7375 6d6d 6172 7928 7365 6c66 293a  e_summary(self):
+00002c00: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00002c10: 7572 6e20 6120 7072 696e 7461 626c 6520  urn a printable 
+00002c20: 7375 6d6d 6172 7920 6f66 206d 6574 6164  summary of metad
+00002c30: 6174 6120 616e 6420 7661 6c75 6520 7479  ata and value ty
+00002c40: 7065 7320 666f 7220 6561 6368 206d 6574  pes for each met
+00002c50: 6164 6174 6120 6c61 7965 722e 0d0a 0d0a  adata layer.....
+00002c60: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00002c70: 2053 756d 6d61 7279 206f 6620 6d65 7461   Summary of meta
+00002c80: 6461 7461 0d0a 2020 2020 2020 2020 3a72  data..        :r
+00002c90: 7479 7065 3a20 7374 720d 0a20 2020 2020  type: str..     
+00002ca0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002cb0: 6d73 6720 3d20 2222 0d0a 2020 2020 2020  msg = ""..      
+00002cc0: 2020 666f 7220 636f 6c20 696e 2073 656c    for col in sel
+00002cd0: 662e 6164 6174 612e 6f62 732e 636f 6c75  f.adata.obs.colu
+00002ce0: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
+00002cf0: 2020 6d73 6720 2b3d 2022 2020 2020 436f    msg += "    Co
+00002d00: 6c75 6d6e 3a20 2220 2b20 636f 6c20 2b20  lumn: " + col + 
+00002d10: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
+00002d20: 2020 666f 7220 7661 6c75 655f 7479 7065    for value_type
+00002d30: 2c20 636f 756e 7420 696e 2073 656c 662e  , count in self.
+00002d40: 6164 6174 612e 6f62 735b 636f 6c5d 2e64  adata.obs[col].d
+00002d50: 726f 706e 6128 292e 6d61 7028 7479 7065  ropna().map(type
+00002d60: 292e 7661 6c75 655f 636f 756e 7473 2829  ).value_counts()
+00002d70: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00002d80: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
+00002d90: 3d20 6622 2020 2020 2020 2020 7b76 616c  = f"        {val
+00002da0: 7565 5f74 7970 657d 3a20 7b63 6f75 6e74  ue_type}: {count
+00002db0: 7d5c 6e22 0d0a 2020 2020 2020 2020 7265  }\n"..        re
+00002dc0: 7475 726e 206d 7367 0d0a 2020 2020 0d0a  turn msg..    ..
+00002dd0: 2020 2020 6465 6620 7772 6974 655f 6835      def write_h5
+00002de0: 6164 2873 656c 662c 0d0a 2020 2020 2020  ad(self,..      
+00002df0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00002e00: 656e 616d 653a 2073 7472 293a 0d0a 2020  ename: str):..  
+00002e10: 2020 2020 2020 2222 2257 7269 7465 2064        """Write d
+00002e20: 6174 6173 6574 2074 6f20 2e68 3561 6420  ataset to .h5ad 
+00002e30: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
+00002e40: 203a 7061 7261 6d20 6669 6c65 6e61 6d65   :param filename
+00002e50: 3a20 6669 6c65 7061 7468 0d0a 2020 2020  : filepath..    
+00002e60: 2020 2020 3a74 7970 6520 6669 6c65 6e61      :type filena
+00002e70: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
+00002e80: 2022 2222 0d0a 2020 2020 2020 2020 6669   """..        fi
+00002e90: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
+00002ea0: 2e61 6273 7061 7468 2866 696c 656e 616d  .abspath(filenam
+00002eb0: 6529 0d0a 2020 2020 2020 2020 6c6f 6767  e)..        logg
+00002ec0: 696e 672e 696e 666f 2866 2257 7269 7469  ing.info(f"Writi
+00002ed0: 6e67 2074 6f20 7b66 696c 656e 616d 657d  ng to {filename}
+00002ee0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00002ef0: 2e61 6461 7461 2e77 7269 7465 5f68 3561  .adata.write_h5a
+00002f00: 6428 6669 6c65 6e61 6d65 290d 0a20 2020  d(filename)..   
+00002f10: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
+00002f20: 6f28 6622 446f 6e65 2229 0d0a 2020 2020  o(f"Done")..    
+00002f30: 0d0a 2020 2020 6465 6620 746f 5f64 6628  ..    def to_df(
+00002f40: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00002f50: 2020 2020 206e 6f72 6d61 6c69 7a65 643a       normalized:
+00002f60: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00002f70: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00002f80: 6461 7461 206d 6174 7269 7820 6173 2061  data matrix as a
+00002f90: 2060 7064 2e44 6174 6146 7261 6d65 600d   `pd.DataFrame`.
+00002fa0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00002fb0: 6d20 6e6f 726d 616c 697a 6564 3a20 5365  m normalized: Se
+00002fc0: 7420 7472 7565 2066 6f72 2054 504d 206e  t true for TPM n
+00002fd0: 6f72 6d61 6c69 7a65 6420 6f75 7470 7574  ormalized output
+00002fe0: 2c20 6465 6661 756c 7473 2074 6f20 4661  , defaults to Fa
+00002ff0: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
+00003000: 7065 206e 6f72 6d61 6c69 7a65 643a 2062  pe normalized: b
+00003010: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+00003020: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003030: 6f62 7365 7276 6174 696f 6e73 20c3 9720  observations .. 
+00003040: 7661 7269 6162 6c65 7320 6461 7461 206d  variables data m
+00003050: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
+00003060: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
+00003070: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
+00003080: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
+00003090: 656c 662e 6164 6174 612e 746f 5f64 6628  elf.adata.to_df(
+000030a0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000030b0: 726d 616c 697a 6564 2061 6e64 206e 6f74  rmalized and not
+000030c0: 2073 656c 662e 6973 5f6e 6f72 6d61 6c69   self.is_normali
+000030d0: 7a65 643a 0d0a 2020 2020 2020 2020 2020  zed:..          
+000030e0: 2020 6466 203d 2064 662e 6469 7628 6466    df = df.div(df
+000030f0: 2e73 756d 2861 7869 733d 3129 2c20 6178  .sum(axis=1), ax
+00003100: 6973 3d30 2920 2a20 3165 3620 2023 2054  is=0) * 1e6  # T
+00003110: 504d 206e 6f72 6d61 6c69 7a61 7469 6f6e  PM normalization
+00003120: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003130: 2064 660d 0a20 2020 2020 2020 200d 0a20   df..        .. 
+00003140: 2020 2064 6566 2072 656d 6f76 655f 756e     def remove_un
+00003150: 6661 6374 6f72 697a 6162 6c65 5f67 656e  factorizable_gen
+00003160: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+00003170: 2020 2022 2222 5265 6d6f 7665 7320 6765     """Removes ge
+00003180: 6e65 7320 7769 7468 206d 6973 7369 6e67  nes with missing
+00003190: 2076 616c 7565 7320 6f72 207a 6572 6f20   values or zero 
+000031a0: 7661 7269 616e 6365 2066 726f 6d20 7468  variance from th
+000031b0: 6520 6461 7461 206d 6174 7269 782e 0d0a  e data matrix...
+000031c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000031d0: 2020 2020 2064 6620 3d20 7365 6c66 2e74       df = self.t
+000031e0: 6f5f 6466 286e 6f72 6d61 6c69 7a65 643d  o_df(normalized=
+000031f0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00003200: 2320 4368 6563 6b20 666f 7220 7661 7269  # Check for vari
+00003210: 6162 6c65 7320 7769 7468 206d 6973 7369  ables with missi
+00003220: 6e67 2076 616c 7565 730d 0a20 2020 2020  ng values..     
+00003230: 2020 2067 656e 6573 5f77 6974 685f 6d69     genes_with_mi
+00003240: 7373 696e 6776 616c 7565 7320 3d20 6466  ssingvalues = df
+00003250: 2e69 736e 756c 6c28 292e 616e 7928 290d  .isnull().any().
+00003260: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00003270: 2020 2069 6620 6765 6e65 735f 7769 7468     if genes_with
+00003280: 5f6d 6973 7369 6e67 7661 6c75 6573 2e61  _missingvalues.a
+00003290: 6e79 2829 3a0d 0a20 2020 2020 2020 2020  ny():..         
+000032a0: 2020 206e 5f6d 6973 7369 6e67 203d 2067     n_missing = g
+000032b0: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
+000032c0: 6776 616c 7565 732e 7375 6d28 290d 0a20  gvalues.sum().. 
+000032d0: 2020 2020 2020 2020 2020 206c 6f67 6769             loggi
+000032e0: 6e67 2e77 6172 6e69 6e67 2866 227b 6e5f  ng.warning(f"{n_
+000032f0: 6d69 7373 696e 677d 206f 6620 7b73 656c  missing} of {sel
+00003300: 662e 6164 6174 612e 6e5f 7661 7273 7d20  f.adata.n_vars} 
+00003310: 7661 7269 6162 6c65 7320 6172 6520 6d69  variables are mi
+00003320: 7373 696e 6720 7661 6c75 6573 2028 6061  ssing values (`a
+00003330: 6461 7461 2e58 6029 2e22 290d 0a20 2020  data.X`).")..   
+00003340: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00003350: 2e77 6172 6e69 6e67 2866 2253 7562 7365  .warning(f"Subse
+00003360: 7474 696e 6720 7661 7269 6162 6c65 7320  tting variables 
+00003370: 746f 2074 686f 7365 2077 6974 6820 6e6f  to those with no
+00003380: 206d 6973 7369 6e67 2076 616c 7565 732e   missing values.
+00003390: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000033a0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+000033b0: 4368 6563 6b20 666f 7220 6765 6e65 7320  Check for genes 
+000033c0: 7769 7468 207a 6572 6f20 7661 7269 616e  with zero varian
+000033d0: 6365 0d0a 2020 2020 2020 2020 7a65 726f  ce..        zero
+000033e0: 7661 7267 656e 6573 203d 2028 6466 2e76  vargenes = (df.v
+000033f0: 6172 2829 203d 3d20 3029 0d0a 2020 2020  ar() == 0)..    
+00003400: 2020 2020 6966 207a 6572 6f76 6172 6765      if zerovarge
+00003410: 6e65 732e 616e 7928 293a 0d0a 2020 2020  nes.any():..    
+00003420: 2020 2020 2020 2020 6e5f 7a65 726f 7661          n_zerova
+00003430: 7220 3d20 7a65 726f 7661 7267 656e 6573  r = zerovargenes
+00003440: 2e73 756d 2829 0d0a 2020 2020 2020 2020  .sum()..        
+00003450: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
+00003460: 696e 6728 6622 7b6e 5f7a 6572 6f76 6172  ing(f"{n_zerovar
+00003470: 7d20 6f66 207b 7365 6c66 2e61 6461 7461  } of {self.adata
+00003480: 2e6e 5f76 6172 737d 2076 6172 6961 626c  .n_vars} variabl
+00003490: 6573 2068 6176 6520 6120 7661 7269 616e  es have a varian
+000034a0: 6365 206f 6620 7a65 726f 2069 6e20 636f  ce of zero in co
+000034b0: 756e 7473 2064 6174 6120 2860 6164 6174  unts data (`adat
+000034c0: 612e 7261 772e 5860 292e 2229 0d0a 2020  a.raw.X`).")..  
+000034d0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+000034e0: 672e 7761 726e 696e 6728 6622 5375 6273  g.warning(f"Subs
+000034f0: 6574 7469 6e67 2076 6172 6961 626c 6573  etting variables
+00003500: 2074 6f20 7468 6f73 6520 7769 7468 206e   to those with n
+00003510: 6f6e 7a65 726f 2076 6172 6961 6e63 652e  onzero variance.
+00003520: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
+00003530: 2020 2020 2020 6765 6e65 735f 746f 5f6b        genes_to_k
+00003540: 6565 7020 3d20 287e 6765 6e65 735f 7769  eep = (~genes_wi
+00003550: 7468 5f6d 6973 7369 6e67 7661 6c75 6573  th_missingvalues
+00003560: 2920 2620 287e 7a65 726f 7661 7267 656e  ) & (~zerovargen
+00003570: 6573 290d 0a20 2020 2020 2020 200d 0a20  es)..        .. 
+00003580: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00003590: 6120 3d20 7365 6c66 2e61 6461 7461 5b3a  a = self.adata[:
+000035a0: 2c67 656e 6573 5f74 6f5f 6b65 6570 5d0d  ,genes_to_keep].
+000035b0: 0a0d 0a20 2020 2064 6566 2063 6f6d 7075  ...    def compu
+000035c0: 7465 5f67 656e 655f 7374 6174 7328 7365  te_gene_stats(se
+000035d0: 6c66 2c20 6f64 675f 6465 6661 756c 745f  lf, odg_default_
+000035e0: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
+000035f0: 6e74 203d 2033 2c20 6f64 675f 6465 6661  nt = 3, odg_defa
+00003600: 756c 745f 646f 663a 2069 6e74 203d 2038  ult_dof: int = 8
+00003610: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00003620: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
+00003630: 7320 6765 6e65 2073 7461 7469 7374 6963  s gene statistic
+00003640: 7320 616e 6420 6669 7473 2074 776f 206d  s and fits two m
+00003650: 6f64 656c 7320 6f66 206d 6561 6e20 616e  odels of mean an
+00003660: 6420 7661 7269 616e 6365 206f 6620 6765  d variance of ge
+00003670: 6e65 7320 696e 2074 6865 2064 6174 6173  nes in the datas
+00003680: 6574 2e20 5468 6520 6669 7273 7420 6d65  et. The first me
+00003690: 7468 6f64 2069 7320 7468 650d 0a20 2020  thod is the..   
+000036a0: 2020 2020 2067 656e 6572 616c 697a 6564       generalized
+000036b0: 2061 6464 6974 6976 6520 6d6f 6465 6c20   additive model 
+000036c0: 7769 7468 2073 6d6f 6f74 6820 636f 6d70  with smooth comp
+000036d0: 6f6e 656e 7473 2028 422d 7370 6c69 6e65  onents (B-spline
+000036e0: 7329 2074 6f20 6d6f 6465 6c20 7468 6520  s) to model the 
+000036f0: 7265 6c61 7469 6f6e 7368 6970 206f 6620  relationship of 
+00003700: 6d65 616e 2061 6e64 2076 6172 6961 6e63  mean and varianc
+00003710: 650d 0a20 2020 2020 2020 2062 6574 7765  e..        betwe
+00003720: 656e 2067 656e 6573 2069 6e20 7468 6520  en genes in the 
+00003730: 6461 7461 7365 742e 2049 7420 7072 6f64  dataset. It prod
+00003740: 7563 6573 2061 6e20 6f64 7363 6f72 6520  uces an odscore 
+00003750: 6d65 7472 6963 2066 6f72 206f 7665 7264  metric for overd
+00003760: 6973 7065 7273 696f 6e2e 2054 6865 2073  ispersion. The s
+00003770: 6563 6f6e 6420 6973 2074 6865 2063 6f75  econd is the cou
+00003780: 6e74 2d73 7461 7469 7374 6963 730d 0a20  nt-statistics.. 
+00003790: 2020 2020 2020 206d 6574 686f 6420 666f         method fo
+000037a0: 756e 6420 696e 2074 6865 2063 4e4d 4620  und in the cNMF 
+000037b0: 7061 636b 6167 652c 2077 6869 6368 2070  package, which p
+000037c0: 726f 6475 6365 7320 6120 6d6f 6469 6669  roduces a modifi
+000037d0: 6564 2076 2d73 636f 7265 206d 6574 7269  ed v-score metri
+000037e0: 632e 2041 6c6c 2067 656e 6520 7374 6174  c. All gene stat
+000037f0: 6973 7469 6373 2061 7265 2073 746f 7265  istics are store
+00003800: 6420 7769 7468 696e 2074 6865 0d0a 2020  d within the..  
+00003810: 2020 2020 2020 6461 7461 7365 7420 6f62        dataset ob
+00003820: 6a65 6374 2061 6e64 2061 7265 2061 6363  ject and are acc
+00003830: 6573 7369 626c 6520 7573 696e 6720 6064  essible using `d
+00003840: 6174 6173 6574 2e61 6e6e 6461 7461 2e76  ataset.anndata.v
+00003850: 6172 602e 0d0a 0d0a 2020 2020 2020 2020  ar`.....        
+00003860: 3a70 6172 616d 206f 6467 5f64 6566 6175  :param odg_defau
+00003870: 6c74 5f73 706c 696e 655f 6465 6772 6565  lt_spline_degree
+00003880: 3a20 422d 5370 6c69 6e65 2064 6567 7265  : B-Spline degre
+00003890: 6520 666f 7220 474c 4d2d 4741 4d20 6d6f  e for GLM-GAM mo
+000038a0: 6465 6c6c 696e 6720 6f66 206d 6561 6e2d  delling of mean-
+000038b0: 7661 7269 616e 6365 2072 656c 6174 696f  variance relatio
+000038c0: 6e73 6869 702c 2064 6566 6175 6c74 7320  nship, defaults 
+000038d0: 746f 2033 0d0a 2020 2020 2020 2020 3a74  to 3..        :t
+000038e0: 7970 6520 6f64 675f 6465 6661 756c 745f  ype odg_default_
+000038f0: 7370 6c69 6e65 5f64 6567 7265 653a 2069  spline_degree: i
+00003900: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+00003910: 2020 2020 2020 3a70 6172 616d 206f 6467        :param odg
+00003920: 5f64 6566 6175 6c74 5f64 6f66 3a20 4465  _default_dof: De
+00003930: 6772 6565 7320 6f66 2066 7265 6564 6f6d  grees of freedom
+00003940: 2066 6f72 2047 4c4d 2d47 414d 206d 6f64   for GLM-GAM mod
+00003950: 656c 6c69 6e67 206f 6620 6d65 616e 2d76  elling of mean-v
+00003960: 6172 616e 6365 2c20 6465 6661 756c 7473  arance, defaults
+00003970: 2074 6f20 380d 0a20 2020 2020 2020 203a   to 8..        :
+00003980: 7479 7065 206f 6467 5f64 6566 6175 6c74  type odg_default
+00003990: 5f64 6f66 3a20 696e 742c 206f 7074 696f  _dof: int, optio
+000039a0: 6e61 6c0d 0a20 2020 2020 2020 2022 2222  nal..        """
+000039b0: 0d0a 2020 2020 2020 2020 6461 7461 5f72  ..        data_r
+000039c0: 6177 203d 2073 656c 662e 746f 5f64 6628  aw = self.to_df(
+000039d0: 290d 0a20 2020 2020 2020 2064 6174 615f  )..        data_
+000039e0: 6e6f 726d 616c 697a 6564 203d 2073 656c  normalized = sel
+000039f0: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
+00003a00: 6564 3d54 7275 6529 0d0a 2020 2020 2020  ed=True)..      
+00003a10: 2020 0d0a 2020 2020 2020 2020 2320 6372    ..        # cr
+00003a20: 6561 7465 2064 6174 6166 7261 6d65 206f  eate dataframe o
+00003a30: 6620 7065 722d 6765 6e65 2073 7461 7469  f per-gene stati
+00003a40: 7374 6963 730d 0a20 2020 2020 2020 2073  stics..        s
+00003a50: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
+00003a60: 6561 6e22 5d20 3d20 6461 7461 5f6e 6f72  ean"] = data_nor
+00003a70: 6d61 6c69 7a65 642e 6d65 616e 2829 0d0a  malized.mean()..
+00003a80: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00003a90: 7461 2e76 6172 5b22 7261 6e6b 5f6d 6561  ta.var["rank_mea
+00003aa0: 6e22 5d20 3d20 7365 6c66 2e61 6461 7461  n"] = self.adata
+00003ab0: 2e76 6172 5b22 6d65 616e 225d 2e72 616e  .var["mean"].ran
+00003ac0: 6b28 290d 0a20 2020 2020 2020 2073 656c  k()..        sel
+00003ad0: 662e 6164 6174 612e 7661 725b 2276 6172  f.adata.var["var
+00003ae0: 6961 6e63 6522 5d20 3d20 6461 7461 5f6e  iance"] = data_n
+00003af0: 6f72 6d61 6c69 7a65 642e 7661 7228 290d  ormalized.var().
+00003b00: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00003b10: 6174 612e 7661 725b 2273 6422 5d20 3d20  ata.var["sd"] = 
+00003b20: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
+00003b30: 7374 6428 290d 0a20 2020 2020 2020 2073  std()..        s
+00003b40: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
+00003b50: 6973 7369 6e67 6e65 7373 225d 203d 2064  issingness"] = d
+00003b60: 6174 615f 6e6f 726d 616c 697a 6564 2e69  ata_normalized.i
+00003b70: 736e 756c 6c28 292e 7375 6d28 2920 2f20  snull().sum() / 
+00003b80: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
+00003b90: 7368 6170 655b 305d 0d0a 2020 2020 2020  shape[0]..      
+00003ba0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+00003bb0: 5b5b 226c 6f67 5f6d 6561 6e22 2c20 226c  [["log_mean", "l
+00003bc0: 6f67 5f76 6172 6961 6e63 6522 5d5d 203d  og_variance"]] =
+00003bd0: 206e 702e 6c6f 6731 3028 7365 6c66 2e61   np.log10(self.a
+00003be0: 6461 7461 2e76 6172 5b5b 226d 6561 6e22  data.var[["mean"
+00003bf0: 2c20 2276 6172 6961 6e63 6522 5d5d 290d  , "variance"]]).
+00003c00: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00003c10: 6174 612e 7661 725b 226d 6561 6e5f 636f  ata.var["mean_co
+00003c20: 756e 7473 225d 203d 2064 6174 615f 7261  unts"] = data_ra
+00003c30: 772e 6d65 616e 2829 0d0a 2020 2020 2020  w.mean()..      
+00003c40: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+00003c50: 5b22 6f64 7363 6f72 655f 6578 636c 7564  ["odscore_exclud
+00003c60: 6564 225d 203d 2028 2873 656c 662e 6164  ed"] = ((self.ad
+00003c70: 6174 612e 7661 725b 226d 6973 7369 6e67  ata.var["missing
+00003c80: 6e65 7373 225d 203e 2030 2920 7c0d 0a20  ness"] > 0) |.. 
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003cd0: 662e 6164 6174 612e 7661 725b 226c 6f67  f.adata.var["log
-00003ce0: 5f6d 6561 6e22 5d2e 6973 6e75 6c6c 2829  _mean"].isnull()
-00003cf0: 207c 0d0a 2020 2020 2020 2020 2020 2020   |..            
+00003cb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003cc0: 662e 6164 6174 612e 7661 725b 226c 6f67  f.adata.var["log
+00003cd0: 5f6d 6561 6e22 5d2e 6973 6e75 6c6c 2829  _mean"].isnull()
+00003ce0: 207c 0d0a 2020 2020 2020 2020 2020 2020   |..            
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 2020 2873 656c 662e 6164 6174 612e 7661    (self.adata.va
-00003d30: 725b 226d 6561 6e22 5d20 3d3d 2030 2920  r["mean"] == 0) 
-00003d40: 7c0d 0a20 2020 2020 2020 2020 2020 2020  |..             
+00003d10: 2020 2873 656c 662e 6164 6174 612e 7661    (self.adata.va
+00003d20: 725b 226d 6561 6e22 5d20 3d3d 2030 2920  r["mean"] == 0) 
+00003d30: 7c0d 0a20 2020 2020 2020 2020 2020 2020  |..             
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
-00003d80: 226c 6f67 5f76 6172 6961 6e63 6522 5d2e  "log_variance"].
-00003d90: 6973 6e75 6c6c 2829 290d 0a0d 0a20 2020  isnull())....   
-00003da0: 2020 2020 2023 206d 6f64 656c 206d 6561       # model mea
-00003db0: 6e2d 7661 7269 616e 6365 2072 656c 6174  n-variance relat
-00003dc0: 696f 6e73 6869 7020 7573 696e 6720 6765  ionship using ge
-00003dd0: 6e65 7261 6c69 7a65 6420 6164 6469 7469  neralized additi
-00003de0: 7665 206d 6f64 656c 2077 6974 6820 736d  ve model with sm
-00003df0: 6f6f 7468 2063 6f6d 706f 6e65 6e74 730d  ooth components.
-00003e00: 0a20 2020 2020 2020 2064 665f 6d6f 6465  .        df_mode
-00003e10: 6c20 3d20 7365 6c66 2e61 6461 7461 2e76  l = self.adata.v
-00003e20: 6172 5b7e 7365 6c66 2e61 6461 7461 2e76  ar[~self.adata.v
-00003e30: 6172 5b22 6f64 7363 6f72 655f 6578 636c  ar["odscore_excl
-00003e40: 7564 6564 225d 5d0d 0a20 2020 2020 2020  uded"]]..       
-00003e50: 2062 7320 3d20 4253 706c 696e 6573 2864   bs = BSplines(d
-00003e60: 665f 6d6f 6465 6c5b 226d 6561 6e22 5d2c  f_model["mean"],
-00003e70: 2064 663d 6f64 675f 6465 6661 756c 745f   df=odg_default_
-00003e80: 646f 662c 2064 6567 7265 653d 6f64 675f  dof, degree=odg_
-00003e90: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
-00003ea0: 6567 7265 6529 0d0a 2020 2020 2020 2020  egree)..        
-00003eb0: 6761 6d20 3d20 474c 4d47 616d 2e66 726f  gam = GLMGam.fro
-00003ec0: 6d5f 666f 726d 756c 6128 226c 6f67 5f76  m_formula("log_v
-00003ed0: 6172 6961 6e63 6520 7e20 6c6f 675f 6d65  ariance ~ log_me
-00003ee0: 616e 222c 2064 6174 613d 6466 5f6d 6f64  an", data=df_mod
-00003ef0: 656c 2c20 736d 6f6f 7468 6572 3d62 7329  el, smoother=bs)
-00003f00: 2e66 6974 2829 0d0a 2020 2020 2020 2020  .fit()..        
-00003f10: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
-00003f20: 7265 7369 645f 6c6f 675f 7661 7269 616e  resid_log_varian
-00003f30: 6365 225d 203d 2067 616d 2e72 6573 6964  ce"] = gam.resid
-00003f40: 5f72 6573 706f 6e73 650d 0a20 2020 2020  _response..     
-00003f50: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
-00003f60: 725b 226f 6473 636f 7265 225d 203d 206e  r["odscore"] = n
-00003f70: 702e 7371 7274 2831 3020 2a2a 2073 656c  p.sqrt(10 ** sel
-00003f80: 662e 6164 6174 612e 7661 725b 2272 6573  f.adata.var["res
-00003f90: 6964 5f6c 6f67 5f76 6172 6961 6e63 6522  id_log_variance"
-00003fa0: 5d29 0d0a 2020 2020 2020 2020 7365 6c66  ])..        self
-00003fb0: 2e61 6461 7461 2e76 6172 5b22 6761 6d5f  .adata.var["gam_
-00003fc0: 6669 7474 6564 7661 6c75 6573 225d 203d  fittedvalues"] =
-00003fd0: 2067 616d 2e66 6974 7465 6476 616c 7565   gam.fittedvalue
-00003fe0: 730d 0a0d 0a0d 0a20 2020 2020 2020 2023  s......        #
-00003ff0: 206d 6f64 656c 206d 6561 6e2d 7661 7269   model mean-vari
-00004000: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
-00004010: 7020 7573 696e 6720 634e 4d46 2773 206d  p using cNMF's m
-00004020: 6574 686f 6420 6261 7365 6420 6f6e 2076  ethod based on v
-00004030: 2d73 636f 7265 2061 6e64 206d 696e 696d  -score and minim
-00004040: 756d 2065 7870 7265 7373 696f 6e20 7468  um expression th
-00004050: 7265 7368 6f6c 640d 0a20 2020 2020 2020  reshold..       
-00004060: 2076 7363 6f72 655f 7374 6174 7320 3d20   vscore_stats = 
-00004070: 7064 2e44 6174 6146 7261 6d65 2863 6e6d  pd.DataFrame(cnm
-00004080: 662e 6765 745f 6869 6768 7661 725f 6765  f.get_highvar_ge
-00004090: 6e65 7328 696e 7075 745f 636f 756e 7473  nes(input_counts
-000040a0: 3d64 6174 615f 6e6f 726d 616c 697a 6564  =data_normalized
-000040b0: 2e76 616c 7565 732c 206d 696e 696d 616c  .values, minimal
-000040c0: 5f6d 6561 6e3d 3029 5b30 5d29 0d0a 2020  _mean=0)[0])..  
-000040d0: 2020 2020 2020 7673 636f 7265 5f73 7461        vscore_sta
-000040e0: 7473 2e69 6e64 6578 203d 2064 6174 615f  ts.index = data_
-000040f0: 6e6f 726d 616c 697a 6564 2e63 6f6c 756d  normalized.colum
-00004100: 6e73 0d0a 2020 2020 2020 2020 7365 6c66  ns..        self
-00004110: 2e61 6461 7461 2e76 6172 5b22 7673 636f  .adata.var["vsco
-00004120: 7265 225d 203d 2076 7363 6f72 655f 7374  re"] = vscore_st
-00004130: 6174 735b 2266 616e 6f5f 7261 7469 6f22  ats["fano_ratio"
-00004140: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00004150: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00004160: 5b22 6f64 675f 6465 6661 756c 745f 7370  ["odg_default_sp
-00004170: 6c69 6e65 5f64 6567 7265 6522 5d20 3d20  line_degree"] = 
-00004180: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
-00004190: 6e65 5f64 6567 7265 650d 0a20 2020 2020  ne_degree..     
-000041a0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-000041b0: 735b 226f 6467 225d 5b22 6f64 675f 6465  s["odg"]["odg_de
-000041c0: 6661 756c 745f 646f 6622 5d20 3d20 6f64  fault_dof"] = od
-000041d0: 675f 6465 6661 756c 745f 646f 660d 0a20  g_default_dof.. 
-000041e0: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
-000041f0: 6e64 5f74 6f5f 6869 7374 6f72 7928 2247  nd_to_history("G
-00004200: 656e 652d 6c65 7665 6c20 7374 6174 6973  ene-level statis
-00004210: 7469 6373 2061 6e64 206f 7665 7264 6973  tics and overdis
-00004220: 7065 7273 696f 6e20 6d6f 6465 6c6c 696e  persion modellin
-00004230: 6720 636f 6d70 6c65 7465 642e 2229 0d0a  g completed.")..
-00004240: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00004250: 6620 7365 6c65 6374 5f6f 7665 7264 6973  f select_overdis
-00004260: 7065 7273 6564 5f67 656e 6573 5f66 726f  persed_genes_fro
-00004270: 6d5f 6765 6e65 6c69 7374 2873 656c 662c  m_genelist(self,
-00004280: 2067 656e 6573 3a20 436f 6c6c 6563 7469   genes: Collecti
-00004290: 6f6e 2c20 6d69 6e5f 6d65 616e 3d30 293a  on, min_mean=0):
-000042a0: 0d0a 2020 2020 2020 2020 2222 2253 656c  ..        """Sel
-000042b0: 6563 7420 6f76 6572 6469 7370 6572 7365  ect overdisperse
-000042c0: 6420 6765 6e65 732f 6665 6174 7572 6573  d genes/features
-000042d0: 2075 7369 6e67 2061 2063 7573 746f 6d20   using a custom 
-000042e0: 6c69 7374 2e20 4765 6e65 732f 6665 6174  list. Genes/feat
-000042f0: 7572 6573 206e 6f74 2070 7265 7365 6e74  ures not present
-00004300: 2069 6e20 7468 6520 6461 7461 7365 7420   in the dataset 
-00004310: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
-00004320: 7920 6669 6c74 6572 6564 206f 7574 2e0d  y filtered out..
-00004330: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00004340: 6d20 6765 6e65 733a 2067 656e 6520 6c69  m genes: gene li
-00004350: 7374 0d0a 2020 2020 2020 2020 3a74 7970  st..        :typ
-00004360: 6520 6765 6e65 733a 2043 6f6c 6c65 6374  e genes: Collect
-00004370: 696f 6e0d 0a20 2020 2020 2020 203a 7061  ion..        :pa
-00004380: 7261 6d20 6d69 6e5f 6d65 616e 3a20 6d69  ram min_mean: mi
-00004390: 6e69 6d75 6d20 6765 6e65 2065 7870 7265  nimum gene expre
-000043a0: 7373 696f 6e20 666f 7220 6765 6e65 7320  ssion for genes 
-000043b0: 746f 2062 6520 636f 756e 7465 6420 6173  to be counted as
-000043c0: 206f 7665 7264 6973 7065 7273 6564 2c20   overdispersed, 
-000043d0: 6465 6661 756c 7473 2074 6f20 300d 0a20  defaults to 0.. 
-000043e0: 2020 2020 2020 203a 7479 7065 206d 696e         :type min
-000043f0: 5f6d 6561 6e3a 2069 6e74 2c20 6f70 7469  _mean: int, opti
-00004400: 6f6e 616c 0d0a 2020 2020 2020 2020 2222  onal..        ""
-00004410: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00004420: 6164 6174 612e 7661 725b 2273 656c 6563  adata.var["selec
-00004430: 7465 6422 5d20 3d20 7365 6c66 2e61 6461  ted"] = self.ada
-00004440: 7461 2e76 6172 2e69 6e64 6578 2e69 7369  ta.var.index.isi
-00004450: 6e28 6765 6e65 7329 2026 2073 656c 662e  n(genes) & self.
-00004460: 6164 6174 612e 7661 725b 226d 6561 6e5f  adata.var["mean_
-00004470: 636f 756e 7473 225d 203e 3d20 6d69 6e5f  counts"] >= min_
-00004480: 6d65 616e 0d0a 2020 2020 2020 2020 7365  mean..        se
-00004490: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
-000044a0: 6722 5d5b 226f 7665 7264 6973 7065 7273  g"]["overdispers
-000044b0: 696f 6e5f 6d65 7472 6963 225d 203d 2022  ion_metric"] = "
-000044c0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000044d0: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-000044e0: 5b22 6d69 6e5f 6d65 616e 225d 203d 206d  ["min_mean"] = m
-000044f0: 696e 5f6d 6561 6e0d 0a20 2020 2020 2020  in_mean..       
-00004500: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00004510: 226f 6467 225d 5b22 6d69 6e5f 7363 6f72  "odg"]["min_scor
-00004520: 6522 5d20 3d20 2222 0d0a 2020 2020 2020  e"] = ""..      
-00004530: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
-00004540: 5b22 6f64 6722 5d5b 2274 6f70 5f6e 225d  ["odg"]["top_n"]
-00004550: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
-00004560: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-00004570: 6467 225d 5b22 7175 616e 7469 6c65 225d  dg"]["quantile"]
-00004580: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
-00004590: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
-000045a0: 7374 6f72 7928 224f 7665 7264 6973 7065  story("Overdispe
-000045b0: 7273 6564 2067 656e 6573 2073 656c 6563  rsed genes selec
-000045c0: 7465 6420 6672 6f6d 2063 7573 746f 6d20  ted from custom 
-000045d0: 6765 6e65 206c 6973 7422 290d 0a20 2020  gene list")..   
-000045e0: 2020 2020 200d 0a20 2020 2064 6566 2073       ..    def s
-000045f0: 656c 6563 745f 6f76 6572 6469 7370 6572  elect_overdisper
-00004600: 7365 645f 6765 6e65 7328 7365 6c66 2c0d  sed_genes(self,.
-00004610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 2020 6f76 6572 6469 7370 6572 7369      overdispersi
-00004640: 6f6e 5f6d 6574 7269 633a 2073 7472 203d  on_metric: str =
-00004650: 2022 6f64 7363 6f72 6522 2c0d 0a20 2020   "odscore",..   
+00003d60: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
+00003d70: 226c 6f67 5f76 6172 6961 6e63 6522 5d2e  "log_variance"].
+00003d80: 6973 6e75 6c6c 2829 290d 0a0d 0a20 2020  isnull())....   
+00003d90: 2020 2020 2023 206d 6f64 656c 206d 6561       # model mea
+00003da0: 6e2d 7661 7269 616e 6365 2072 656c 6174  n-variance relat
+00003db0: 696f 6e73 6869 7020 7573 696e 6720 6765  ionship using ge
+00003dc0: 6e65 7261 6c69 7a65 6420 6164 6469 7469  neralized additi
+00003dd0: 7665 206d 6f64 656c 2077 6974 6820 736d  ve model with sm
+00003de0: 6f6f 7468 2063 6f6d 706f 6e65 6e74 730d  ooth components.
+00003df0: 0a20 2020 2020 2020 2064 665f 6d6f 6465  .        df_mode
+00003e00: 6c20 3d20 7365 6c66 2e61 6461 7461 2e76  l = self.adata.v
+00003e10: 6172 5b7e 7365 6c66 2e61 6461 7461 2e76  ar[~self.adata.v
+00003e20: 6172 5b22 6f64 7363 6f72 655f 6578 636c  ar["odscore_excl
+00003e30: 7564 6564 225d 5d0d 0a20 2020 2020 2020  uded"]]..       
+00003e40: 2062 7320 3d20 4253 706c 696e 6573 2864   bs = BSplines(d
+00003e50: 665f 6d6f 6465 6c5b 226d 6561 6e22 5d2c  f_model["mean"],
+00003e60: 2064 663d 6f64 675f 6465 6661 756c 745f   df=odg_default_
+00003e70: 646f 662c 2064 6567 7265 653d 6f64 675f  dof, degree=odg_
+00003e80: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
+00003e90: 6567 7265 6529 0d0a 2020 2020 2020 2020  egree)..        
+00003ea0: 6761 6d20 3d20 474c 4d47 616d 2e66 726f  gam = GLMGam.fro
+00003eb0: 6d5f 666f 726d 756c 6128 226c 6f67 5f76  m_formula("log_v
+00003ec0: 6172 6961 6e63 6520 7e20 6c6f 675f 6d65  ariance ~ log_me
+00003ed0: 616e 222c 2064 6174 613d 6466 5f6d 6f64  an", data=df_mod
+00003ee0: 656c 2c20 736d 6f6f 7468 6572 3d62 7329  el, smoother=bs)
+00003ef0: 2e66 6974 2829 0d0a 2020 2020 2020 2020  .fit()..        
+00003f00: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+00003f10: 7265 7369 645f 6c6f 675f 7661 7269 616e  resid_log_varian
+00003f20: 6365 225d 203d 2067 616d 2e72 6573 6964  ce"] = gam.resid
+00003f30: 5f72 6573 706f 6e73 650d 0a20 2020 2020  _response..     
+00003f40: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
+00003f50: 725b 226f 6473 636f 7265 225d 203d 206e  r["odscore"] = n
+00003f60: 702e 7371 7274 2831 3020 2a2a 2073 656c  p.sqrt(10 ** sel
+00003f70: 662e 6164 6174 612e 7661 725b 2272 6573  f.adata.var["res
+00003f80: 6964 5f6c 6f67 5f76 6172 6961 6e63 6522  id_log_variance"
+00003f90: 5d29 0d0a 2020 2020 2020 2020 7365 6c66  ])..        self
+00003fa0: 2e61 6461 7461 2e76 6172 5b22 6761 6d5f  .adata.var["gam_
+00003fb0: 6669 7474 6564 7661 6c75 6573 225d 203d  fittedvalues"] =
+00003fc0: 2067 616d 2e66 6974 7465 6476 616c 7565   gam.fittedvalue
+00003fd0: 730d 0a0d 0a0d 0a20 2020 2020 2020 2023  s......        #
+00003fe0: 206d 6f64 656c 206d 6561 6e2d 7661 7269   model mean-vari
+00003ff0: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
+00004000: 7020 7573 696e 6720 634e 4d46 2773 206d  p using cNMF's m
+00004010: 6574 686f 6420 6261 7365 6420 6f6e 2076  ethod based on v
+00004020: 2d73 636f 7265 2061 6e64 206d 696e 696d  -score and minim
+00004030: 756d 2065 7870 7265 7373 696f 6e20 7468  um expression th
+00004040: 7265 7368 6f6c 640d 0a20 2020 2020 2020  reshold..       
+00004050: 2076 7363 6f72 655f 7374 6174 7320 3d20   vscore_stats = 
+00004060: 7064 2e44 6174 6146 7261 6d65 2863 6e6d  pd.DataFrame(cnm
+00004070: 662e 6765 745f 6869 6768 7661 725f 6765  f.get_highvar_ge
+00004080: 6e65 7328 696e 7075 745f 636f 756e 7473  nes(input_counts
+00004090: 3d64 6174 615f 6e6f 726d 616c 697a 6564  =data_normalized
+000040a0: 2e76 616c 7565 732c 206d 696e 696d 616c  .values, minimal
+000040b0: 5f6d 6561 6e3d 3029 5b30 5d29 0d0a 2020  _mean=0)[0])..  
+000040c0: 2020 2020 2020 7673 636f 7265 5f73 7461        vscore_sta
+000040d0: 7473 2e69 6e64 6578 203d 2064 6174 615f  ts.index = data_
+000040e0: 6e6f 726d 616c 697a 6564 2e63 6f6c 756d  normalized.colum
+000040f0: 6e73 0d0a 2020 2020 2020 2020 7365 6c66  ns..        self
+00004100: 2e61 6461 7461 2e76 6172 5b22 7673 636f  .adata.var["vsco
+00004110: 7265 225d 203d 2076 7363 6f72 655f 7374  re"] = vscore_st
+00004120: 6174 735b 2266 616e 6f5f 7261 7469 6f22  ats["fano_ratio"
+00004130: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00004140: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00004150: 5b22 6f64 675f 6465 6661 756c 745f 7370  ["odg_default_sp
+00004160: 6c69 6e65 5f64 6567 7265 6522 5d20 3d20  line_degree"] = 
+00004170: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
+00004180: 6e65 5f64 6567 7265 650d 0a20 2020 2020  ne_degree..     
+00004190: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+000041a0: 735b 226f 6467 225d 5b22 6f64 675f 6465  s["odg"]["odg_de
+000041b0: 6661 756c 745f 646f 6622 5d20 3d20 6f64  fault_dof"] = od
+000041c0: 675f 6465 6661 756c 745f 646f 660d 0a20  g_default_dof.. 
+000041d0: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+000041e0: 6e64 5f74 6f5f 6869 7374 6f72 7928 2247  nd_to_history("G
+000041f0: 656e 652d 6c65 7665 6c20 7374 6174 6973  ene-level statis
+00004200: 7469 6373 2061 6e64 206f 7665 7264 6973  tics and overdis
+00004210: 7065 7273 696f 6e20 6d6f 6465 6c6c 696e  persion modellin
+00004220: 6720 636f 6d70 6c65 7465 642e 2229 0d0a  g completed.")..
+00004230: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00004240: 6620 7365 6c65 6374 5f6f 7665 7264 6973  f select_overdis
+00004250: 7065 7273 6564 5f67 656e 6573 5f66 726f  persed_genes_fro
+00004260: 6d5f 6765 6e65 6c69 7374 2873 656c 662c  m_genelist(self,
+00004270: 2067 656e 6573 3a20 436f 6c6c 6563 7469   genes: Collecti
+00004280: 6f6e 2c20 6d69 6e5f 6d65 616e 3d30 293a  on, min_mean=0):
+00004290: 0d0a 2020 2020 2020 2020 2222 2253 656c  ..        """Sel
+000042a0: 6563 7420 6f76 6572 6469 7370 6572 7365  ect overdisperse
+000042b0: 6420 6765 6e65 732f 6665 6174 7572 6573  d genes/features
+000042c0: 2075 7369 6e67 2061 2063 7573 746f 6d20   using a custom 
+000042d0: 6c69 7374 2e20 4765 6e65 732f 6665 6174  list. Genes/feat
+000042e0: 7572 6573 206e 6f74 2070 7265 7365 6e74  ures not present
+000042f0: 2069 6e20 7468 6520 6461 7461 7365 7420   in the dataset 
+00004300: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
+00004310: 7920 6669 6c74 6572 6564 206f 7574 2e0d  y filtered out..
+00004320: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00004330: 6d20 6765 6e65 733a 2067 656e 6520 6c69  m genes: gene li
+00004340: 7374 0d0a 2020 2020 2020 2020 3a74 7970  st..        :typ
+00004350: 6520 6765 6e65 733a 2043 6f6c 6c65 6374  e genes: Collect
+00004360: 696f 6e0d 0a20 2020 2020 2020 203a 7061  ion..        :pa
+00004370: 7261 6d20 6d69 6e5f 6d65 616e 3a20 6d69  ram min_mean: mi
+00004380: 6e69 6d75 6d20 6765 6e65 2065 7870 7265  nimum gene expre
+00004390: 7373 696f 6e20 666f 7220 6765 6e65 7320  ssion for genes 
+000043a0: 746f 2062 6520 636f 756e 7465 6420 6173  to be counted as
+000043b0: 206f 7665 7264 6973 7065 7273 6564 2c20   overdispersed, 
+000043c0: 6465 6661 756c 7473 2074 6f20 300d 0a20  defaults to 0.. 
+000043d0: 2020 2020 2020 203a 7479 7065 206d 696e         :type min
+000043e0: 5f6d 6561 6e3a 2069 6e74 2c20 6f70 7469  _mean: int, opti
+000043f0: 6f6e 616c 0d0a 2020 2020 2020 2020 2222  onal..        ""
+00004400: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00004410: 6164 6174 612e 7661 725b 2273 656c 6563  adata.var["selec
+00004420: 7465 6422 5d20 3d20 7365 6c66 2e61 6461  ted"] = self.ada
+00004430: 7461 2e76 6172 2e69 6e64 6578 2e69 7369  ta.var.index.isi
+00004440: 6e28 6765 6e65 7329 2026 2073 656c 662e  n(genes) & self.
+00004450: 6164 6174 612e 7661 725b 226d 6561 6e5f  adata.var["mean_
+00004460: 636f 756e 7473 225d 203e 3d20 6d69 6e5f  counts"] >= min_
+00004470: 6d65 616e 0d0a 2020 2020 2020 2020 7365  mean..        se
+00004480: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
+00004490: 6722 5d5b 226f 7665 7264 6973 7065 7273  g"]["overdispers
+000044a0: 696f 6e5f 6d65 7472 6963 225d 203d 2022  ion_metric"] = "
+000044b0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+000044c0: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+000044d0: 5b22 6d69 6e5f 6d65 616e 225d 203d 206d  ["min_mean"] = m
+000044e0: 696e 5f6d 6561 6e0d 0a20 2020 2020 2020  in_mean..       
+000044f0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00004500: 226f 6467 225d 5b22 6d69 6e5f 7363 6f72  "odg"]["min_scor
+00004510: 6522 5d20 3d20 2222 0d0a 2020 2020 2020  e"] = ""..      
+00004520: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+00004530: 5b22 6f64 6722 5d5b 2274 6f70 5f6e 225d  ["odg"]["top_n"]
+00004540: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
+00004550: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
+00004560: 6467 225d 5b22 7175 616e 7469 6c65 225d  dg"]["quantile"]
+00004570: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
+00004580: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
+00004590: 7374 6f72 7928 224f 7665 7264 6973 7065  story("Overdispe
+000045a0: 7273 6564 2067 656e 6573 2073 656c 6563  rsed genes selec
+000045b0: 7465 6420 6672 6f6d 2063 7573 746f 6d20  ted from custom 
+000045c0: 6765 6e65 206c 6973 7422 290d 0a20 2020  gene list")..   
+000045d0: 2020 2020 200d 0a20 2020 2064 6566 2073       ..    def s
+000045e0: 656c 6563 745f 6f76 6572 6469 7370 6572  elect_overdisper
+000045f0: 7365 645f 6765 6e65 7328 7365 6c66 2c0d  sed_genes(self,.
+00004600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004620: 2020 2020 6f76 6572 6469 7370 6572 7369      overdispersi
+00004630: 6f6e 5f6d 6574 7269 633a 2073 7472 203d  on_metric: str =
+00004640: 2022 6f64 7363 6f72 6522 2c0d 0a20 2020   "odscore",..   
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 6d69 6e5f 6d65 616e 3a20 666c 6f61 7420  min_mean: float 
-00004690: 3d20 302c 0d0a 2020 2020 2020 2020 2020  = 0,..          
-000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046b0: 2020 2020 2020 2020 206d 696e 5f73 636f           min_sco
-000046c0: 7265 3a20 666c 6f61 7420 3d20 312e 302c  re: float = 1.0,
-000046d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 2074 6f70 5f6e 3a20 696e 7420       top_n: int 
-00004700: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004720: 2020 2020 2020 2020 2020 2020 7175 616e              quan
-00004730: 7469 6c65 3a20 666c 6f61 7420 3d20 4e6f  tile: float = No
-00004740: 6e65 293a 0d0a 2020 2020 2020 2020 2222  ne):..        ""
-00004750: 2253 656c 6563 7420 6f76 6572 6469 7370  "Select overdisp
-00004760: 6572 7365 6420 6765 6e65 732f 6665 6174  ersed genes/feat
-00004770: 7572 6573 2075 7369 6e67 2061 6e20 6f76  ures using an ov
-00004780: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
-00004790: 7269 632e 204f 7074 696f 6e61 6c6c 7920  ric. Optionally 
-000047a0: 7365 7420 6120 6d69 6e69 6d75 6d20 6765  set a minimum ge
-000047b0: 6e65 2065 7870 7265 7373 696f 6e20 6c65  ne expression le
-000047c0: 7665 6c2e 0d0a 2020 2020 2020 2020 5365  vel...        Se
-000047d0: 7420 6120 7468 7265 7368 6f6c 6420 7573  t a threshold us
-000047e0: 696e 6720 7468 6520 746f 7020 4e20 2827  ing the top N ('
-000047f0: 746f 705f 6e27 292c 206d 696e 696d 756d  top_n'), minimum
-00004800: 2073 636f 7265 2028 276d 696e 5f73 636f   score ('min_sco
-00004810: 7265 2729 2c20 6f72 2070 726f 706f 7274  re'), or proport
-00004820: 696f 6e20 6f66 2066 6561 7475 7265 7320  ion of features 
-00004830: 2827 7175 616e 7469 6c65 2729 206d 6574  ('quantile') met
-00004840: 686f 6473 2e0d 0a20 2020 2020 2020 204f  hods...        O
-00004850: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
-00004860: 6520 6c69 7374 2069 7320 7361 7665 6420  e list is saved 
-00004870: 696e 2074 6865 2044 6174 6173 6574 206f  in the Dataset o
-00004880: 626a 6563 742e 0d0a 0d0a 2020 2020 2020  bject.....      
-00004890: 2020 3a70 6172 616d 206f 7665 7264 6973    :param overdis
-000048a0: 7065 7273 696f 6e5f 6d65 7472 6963 3a20  persion_metric: 
-000048b0: 226f 6473 636f 7265 2220 6f72 2022 7673  "odscore" or "vs
-000048c0: 636f 7265 222c 2064 6566 6175 6c74 7320  core", defaults 
-000048d0: 746f 2022 6f64 7363 6f72 6522 0d0a 2020  to "odscore"..  
-000048e0: 2020 2020 2020 3a74 7970 6520 6f76 6572        :type over
-000048f0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
-00004900: 633a 2073 7472 2c20 6f70 7469 6f6e 616c  c: str, optional
-00004910: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00004920: 206d 696e 5f6d 6561 6e3a 206d 696e 696d   min_mean: minim
-00004930: 756d 2067 656e 6520 6578 7072 6573 7369  um gene expressi
-00004940: 6f6e 2066 6f72 2067 656e 6573 2074 6f20  on for genes to 
-00004950: 6265 2063 6f75 6e74 6564 2061 7320 6f76  be counted as ov
-00004960: 6572 6469 7370 6572 7365 642c 2064 6566  erdispersed, def
-00004970: 6175 6c74 7320 746f 2030 0d0a 2020 2020  aults to 0..    
-00004980: 2020 2020 3a74 7970 6520 6d69 6e5f 6d65      :type min_me
-00004990: 616e 3a20 696e 742c 206f 7074 696f 6e61  an: int, optiona
-000049a0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-000049b0: 6d20 6d69 6e5f 7363 6f72 653a 206d 696e  m min_score: min
-000049c0: 696d 756d 2073 636f 7265 2066 6f72 206f  imum score for o
-000049d0: 7665 7264 6973 7065 7273 696f 6e2c 2064  verdispersion, d
-000049e0: 6566 6175 6c74 7320 746f 2031 2e30 0d0a  efaults to 1.0..
-000049f0: 2020 2020 2020 2020 3a74 7970 6520 6d69          :type mi
-00004a00: 6e5f 7363 6f72 653a 2066 6c6f 6174 2c20  n_score: float, 
-00004a10: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00004a20: 2020 3a70 6172 616d 2074 6f70 5f6e 3a20    :param top_n: 
-00004a30: 4368 6f6f 7365 2074 6865 2074 6f70 204e  Choose the top N
-00004a40: 206d 6f73 7420 6f76 6572 6469 7370 6572   most overdisper
-00004a50: 7365 6420 6765 6e65 732c 2064 6566 6175  sed genes, defau
-00004a60: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-00004a70: 2020 2020 203a 7479 7065 2074 6f70 5f6e       :type top_n
-00004a80: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
-00004a90: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00004aa0: 7175 616e 7469 6c65 3a20 4368 6f6f 7365  quantile: Choose
-00004ab0: 2061 2071 7561 6e74 696c 6520 6f66 206f   a quantile of o
-00004ac0: 7665 7264 6973 7065 7273 696f 6e2e 2046  verdispersion. F
-00004ad0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
-00004ae0: 746f 7020 3130 2520 6f66 206f 7665 7264  top 10% of overd
-00004af0: 6973 7065 7273 6564 2067 656e 6573 2077  ispersed genes w
-00004b00: 6f75 6c64 2062 6520 302e 3130 2e20 4465  ould be 0.10. De
-00004b10: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
-00004b20: 2020 2020 2020 2020 3a74 7970 6520 7175          :type qu
-00004b30: 616e 7469 6c65 3a20 666c 6f61 742c 206f  antile: float, o
-00004b40: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00004b50: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
-00004b60: 726f 723a 2045 7272 6f72 2069 6620 696e  ror: Error if in
-00004b70: 7661 6c69 6420 6f76 6572 6469 7370 6572  valid overdisper
-00004b80: 7369 6f6e 206d 6574 7269 6320 6973 2063  sion metric is c
-00004b90: 686f 7365 6e2e 0d0a 2020 2020 2020 2020  hosen...        
-00004ba0: 2222 220d 0a20 2020 2020 2020 200d 0a20  """..        .. 
-00004bb0: 2020 2020 2020 2069 6620 6f76 6572 6469         if overdi
-00004bc0: 7370 6572 7369 6f6e 5f6d 6574 7269 6320  spersion_metric 
-00004bd0: 6e6f 7420 696e 2073 656c 662e 6164 6174  not in self.adat
-00004be0: 612e 7661 722e 636f 6c75 6d6e 733a 0d0a  a.var.columns:..
-00004bf0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00004c00: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
-00004c10: 7472 6963 2069 6e20 2822 6f64 7363 6f72  tric in ("odscor
-00004c20: 6522 2c20 2276 7363 6f72 6522 293a 0d0a  e", "vscore"):..
-00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c40: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00004c50: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00004c60: 2020 2020 2020 2066 227b 6f76 6572 6469         f"{overdi
-00004c70: 7370 6572 7369 6f6e 5f6d 6574 7269 637d  spersion_metric}
-00004c80: 2068 6173 206e 6f74 2062 6565 6e20 6361   has not been ca
-00004c90: 6c63 756c 6174 6564 2066 6f72 2074 6869  lculated for thi
-00004ca0: 7320 6461 7461 7365 742e 2022 0d0a 2020  s dataset. "..  
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2245 6e73 7572 6520 7468 6174 2079    "Ensure that y
-00004cd0: 6f75 2063 616c 6c20 7468 6520 6044 6174  ou call the `Dat
-00004ce0: 6173 6574 2e63 6f6d 7075 7465 5f67 656e  aset.compute_gen
-00004cf0: 655f 7374 6174 7328 2960 2066 6972 7374  e_stats()` first
-00004d00: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-00004d10: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00004d20: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00004d30: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00004d40: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
-00004d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d60: 2020 2020 2066 227b 6f76 6572 6469 7370       f"{overdisp
-00004d70: 6572 7369 6f6e 5f6d 6574 7269 637d 2069  ersion_metric} i
-00004d80: 7320 6e6f 7420 6120 7661 6c69 6420 6f76  s not a valid ov
-00004d90: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
-00004da0: 7269 632e 220d 0a20 2020 2020 2020 2020  ric."..         
-00004db0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00004dc0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00004dd0: 2320 7761 726e 2069 6620 6d75 6c74 6970  # warn if multip
-00004de0: 6c65 206d 6574 686f 6473 2061 7265 2073  le methods are s
-00004df0: 656c 6563 7465 640d 0a20 2020 2020 2020  elected..       
-00004e00: 2073 656c 6563 7465 645f 6d65 7468 6f64   selected_method
-00004e10: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00004e20: 6966 206d 696e 5f73 636f 7265 2069 7320  if min_score is 
-00004e30: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00004e40: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00004e50: 6d65 7468 6f64 732e 6170 7065 6e64 2822  methods.append("
-00004e60: 6d69 6e5f 7363 6f72 6522 290d 0a20 2020  min_score")..   
-00004e70: 2020 2020 2069 6620 746f 705f 6e20 6973       if top_n is
-00004e80: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00004e90: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00004ea0: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
-00004eb0: 2274 6f70 5f6e 2229 0d0a 2020 2020 2020  "top_n")..      
-00004ec0: 2020 6966 2071 7561 6e74 696c 6520 6973    if quantile is
-00004ed0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00004ee0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00004ef0: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
-00004f00: 2271 7561 6e74 696c 6522 290d 0a20 2020  "quantile")..   
-00004f10: 2020 2020 2069 6620 6c65 6e28 7365 6c65       if len(sele
-00004f20: 6374 6564 5f6d 6574 686f 6473 2920 3e20  cted_methods) > 
-00004f30: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00004f40: 6d65 7468 6f64 7761 726e 7374 7220 3d20  methodwarnstr = 
-00004f50: 222c 2022 2e6a 6f69 6e28 7365 6c65 6374  ", ".join(select
-00004f60: 6564 5f6d 6574 686f 6473 290d 0a20 2020  ed_methods)..   
-00004f70: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
-00004f80: 2e77 6172 6e69 6e67 2866 224d 756c 7469  .warning(f"Multi
-00004f90: 706c 6520 636f 6e66 6c69 6374 696e 6720  ple conflicting 
-00004fa0: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
-00004fb0: 6e65 2073 656c 6563 7469 6f6e 2063 7269  ne selection cri
-00004fc0: 7465 7269 6120 6861 7665 2062 6565 6e20  teria have been 
-00004fd0: 7365 6c65 6374 6564 3a20 7b6d 6574 686f  selected: {metho
-00004fe0: 6477 6172 6e73 7472 7d2e 2022 0d0a 2020  dwarnstr}. "..  
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2020 2020 224f 6e6c 7920            "Only 
-00005010: 7468 6520 696e 7465 7273 6563 7469 6f6e  the intersection
-00005020: 206f 6620 7468 6573 6520 6d65 7468 6f64   of these method
-00005030: 7320 7769 6c6c 2062 6520 7365 6c65 6374  s will be select
-00005040: 6564 2e22 290d 0a20 2020 2020 2020 2020  ed.")..         
-00005050: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005060: 2023 206d 696e 5f6d 6561 6e20 6669 6c74   # min_mean filt
-00005070: 6572 0d0a 2020 2020 2020 2020 7365 6c65  er..        sele
-00005080: 6374 6564 5f67 656e 6573 203d 2073 656c  cted_genes = sel
-00005090: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
-000050a0: 6e5f 636f 756e 7473 225d 203e 3d20 6d69  n_counts"] >= mi
-000050b0: 6e5f 6d65 616e 0d0a 2020 2020 2020 2020  n_mean..        
-000050c0: 2320 6d69 6e5f 7363 6f72 6520 6669 6c74  # min_score filt
-000050d0: 6572 0d0a 2020 2020 2020 2020 6966 206d  er..        if m
-000050e0: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
-000050f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00005100: 2020 2073 656c 6563 7465 645f 6765 6e65     selected_gene
-00005110: 7320 3d20 7365 6c65 6374 6564 5f67 656e  s = selected_gen
-00005120: 6573 2026 2028 7365 6c66 2e61 6461 7461  es & (self.adata
-00005130: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
-00005140: 696f 6e5f 6d65 7472 6963 5d20 3e3d 206d  ion_metric] >= m
-00005150: 696e 5f73 636f 7265 290d 0a20 2020 2020  in_score)..     
-00005160: 2020 2023 2074 6f70 5f6e 2066 696c 7465     # top_n filte
-00005170: 720d 0a20 2020 2020 2020 2069 6620 746f  r..        if to
-00005180: 705f 6e20 6973 206e 6f74 204e 6f6e 653a  p_n is not None:
-00005190: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
-000051a0: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
-000051b0: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
-000051c0: 696f 6e5f 6d65 7472 6963 5d2e 736f 7274  ion_metric].sort
-000051d0: 5f76 616c 7565 7328 6173 6365 6e64 696e  _values(ascendin
-000051e0: 673d 4661 6c73 6529 2e68 6561 6428 696e  g=False).head(in
-000051f0: 7428 746f 705f 6e29 292e 696e 6465 780d  t(top_n)).index.
-00005200: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005210: 6563 7465 645f 6765 6e65 7320 3d20 7365  ected_genes = se
-00005220: 6c65 6374 6564 5f67 656e 6573 2026 2073  lected_genes & s
-00005230: 656c 662e 6164 6174 612e 7661 722e 696e  elf.adata.var.in
-00005240: 6465 782e 6973 696e 2867 656e 6573 290d  dex.isin(genes).
-00005250: 0a20 2020 2020 2020 2023 2071 7561 6e74  .        # quant
-00005260: 696c 6520 6669 6c74 6572 0d0a 2020 2020  ile filter..    
-00005270: 2020 2020 6966 2071 7561 6e74 696c 6520      if quantile 
-00005280: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00005290: 2020 2020 2020 2020 2020 6e5f 746f 7461            n_tota
-000052a0: 6c5f 6765 6e65 7320 3d20 7365 6c66 2e61  l_genes = self.a
-000052b0: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
-000052c0: 7065 7273 696f 6e5f 6d65 7472 6963 5d2e  persion_metric].
-000052d0: 6e6f 746e 756c 6c28 292e 7375 6d28 290d  notnull().sum().
-000052e0: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
-000052f0: 6573 203d 2073 656c 662e 6164 6174 612e  es = self.adata.
-00005300: 7661 725b 6f76 6572 6469 7370 6572 7369  var[overdispersi
-00005310: 6f6e 5f6d 6574 7269 635d 2e73 6f72 745f  on_metric].sort_
-00005320: 7661 6c75 6573 2861 7363 656e 6469 6e67  values(ascending
-00005330: 3d46 616c 7365 292e 6865 6164 2869 6e74  =False).head(int
-00005340: 2871 7561 6e74 696c 6520 2a20 6e5f 746f  (quantile * n_to
-00005350: 7461 6c5f 6765 6e65 7329 292e 696e 6465  tal_genes)).inde
-00005360: 780d 0a20 2020 2020 2020 2020 2020 2073  x..            s
-00005370: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
-00005380: 7365 6c65 6374 6564 5f67 656e 6573 2026  selected_genes &
-00005390: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
-000053a0: 696e 6465 782e 6973 696e 2867 656e 6573  index.isin(genes
-000053b0: 290d 0a0d 0a20 2020 2020 2020 206e 5f73  )....        n_s
-000053c0: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
-000053d0: 7365 6c65 6374 6564 5f67 656e 6573 2e73  selected_genes.s
-000053e0: 756d 2829 0d0a 2020 2020 2020 2020 6c6f  um()..        lo
-000053f0: 6767 696e 672e 696e 666f 2866 227b 6e5f  gging.info(f"{n_
-00005400: 7365 6c65 6374 6564 5f67 656e 6573 7d20  selected_genes} 
-00005410: 6765 6e65 7320 7365 6c65 6374 6564 2066  genes selected f
-00005420: 6f72 2066 6163 746f 7269 7a61 7469 6f6e  or factorization
-00005430: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
-00005440: 2020 2020 2020 2320 6d61 6b65 2063 6861        # make cha
-00005450: 6e67 6573 2074 6f20 4461 7461 7365 7420  nges to Dataset 
-00005460: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
-00005470: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
-00005480: 7365 6c65 6374 6564 225d 203d 2073 656c  selected"] = sel
-00005490: 6563 7465 645f 6765 6e65 730d 0a20 2020  ected_genes..   
-000054a0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-000054b0: 756e 735b 226f 6467 225d 5b22 6f76 6572  uns["odg"]["over
-000054c0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
-000054d0: 6322 5d20 3d20 6f76 6572 6469 7370 6572  c"] = overdisper
-000054e0: 7369 6f6e 5f6d 6574 7269 630d 0a20 2020  sion_metric..   
-000054f0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00005500: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
-00005510: 6d65 616e 225d 203d 206d 696e 5f6d 6561  mean"] = min_mea
-00005520: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-00005530: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00005540: 5b22 6d69 6e5f 7363 6f72 6522 5d20 3d20  ["min_score"] = 
-00005550: 6d69 6e5f 7363 6f72 6520 6966 206d 696e  min_score if min
-00005560: 5f73 636f 7265 2069 7320 6e6f 7420 4e6f  _score is not No
-00005570: 6e65 2065 6c73 6520 2222 0d0a 2020 2020  ne else ""..    
-00005580: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-00005590: 6e73 5b22 6f64 6722 5d5b 2274 6f70 5f6e  ns["odg"]["top_n
-000055a0: 225d 203d 2074 6f70 5f6e 2069 6620 746f  "] = top_n if to
-000055b0: 705f 6e20 6973 206e 6f74 204e 6f6e 6520  p_n is not None 
-000055c0: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
-000055d0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-000055e0: 226f 6467 225d 5b22 7175 616e 7469 6c65  "odg"]["quantile
-000055f0: 225d 203d 2071 7561 6e74 696c 6520 6966  "] = quantile if
-00005600: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
-00005610: 204e 6f6e 6520 656c 7365 2022 220d 0a20   None else "".. 
-00005620: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
-00005630: 6e64 5f74 6f5f 6869 7374 6f72 7928 224f  nd_to_history("O
-00005640: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
-00005650: 6573 2073 656c 6563 7465 6422 290d 0a20  es selected").. 
-00005660: 2020 200d 0a20 2020 2064 6566 2069 6e69     ..    def ini
-00005670: 7469 616c 697a 655f 636e 6d66 2873 656c  tialize_cnmf(sel
-00005680: 662c 2063 6e6d 665f 6f75 7470 7574 5f64  f, cnmf_output_d
-00005690: 6972 3a20 7374 722c 0d0a 2020 2020 2020  ir: str,..      
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 636e 6d66 5f6e 616d 653a 2073 7472    cnmf_name: str
-000056c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000056d0: 2020 2020 2020 2020 2020 206b 7661 6c73             kvals
-000056e0: 3a20 436f 6c6c 6563 7469 6f6e 203d 2072  : Collection = r
-000056f0: 616e 6765 2832 2c20 3631 292c 0d0a 2020  ange(2, 61),..  
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 2020 6e5f 6974 6572 3a20 696e        n_iter: in
-00005720: 7420 3d20 3230 302c 0d0a 2020 2020 2020  t = 200,..      
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 6265 7461 5f6c 6f73 733a 2073 7472    beta_loss: str
-00005750: 203d 2022 6b75 6c6c 6261 636b 2d6c 6569   = "kullback-lei
-00005760: 626c 6572 222c 0d0a 2020 2020 2020 2020  bler",..        
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 7365 6564 3a20 4f70 7469 6f6e 616c 5b69  seed: Optional[i
-00005790: 6e74 5d20 3d20 4e6f 6e65 2920 2d3e 2063  nt] = None) -> c
-000057a0: 6e6d 662e 634e 4d46 3a0d 0a20 2020 2020  nmf.cNMF:..     
-000057b0: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
-000057c0: 2061 2063 4e4d 4620 7275 6e20 666f 7220   a cNMF run for 
-000057d0: 7375 6273 6571 7565 6e74 2066 6163 746f  subsequent facto
-000057e0: 7269 7a61 7469 6f6e 2e0d 0a0d 0a20 2020  rization.....   
-000057f0: 2020 2020 203a 7061 7261 6d20 636e 6d66       :param cnmf
-00005800: 5f6f 7574 7075 745f 6469 723a 204f 7574  _output_dir: Out
-00005810: 7075 7420 6469 7265 6374 6f72 7920 666f  put directory fo
-00005820: 7220 634e 4d46 2072 6573 756c 7473 0d0a  r cNMF results..
-00005830: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
-00005840: 6d66 5f6f 7574 7075 745f 6469 723a 2073  mf_output_dir: s
-00005850: 7472 0d0a 2020 2020 2020 2020 3a70 6172  tr..        :par
-00005860: 616d 2063 6e6d 665f 6e61 6d65 3a20 4e61  am cnmf_name: Na
-00005870: 6d65 206f 6620 7468 6520 634e 4d46 2072  me of the cNMF r
-00005880: 6573 756c 7473 2e20 4669 6c65 7320 7769  esults. Files wi
-00005890: 6c6c 2062 6520 6f75 7470 7574 2074 6f20  ll be output to 
-000058a0: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
-000058b0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d2f 0d0a  ]/[cnmf_name]/..
-000058c0: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
-000058d0: 6d66 5f6e 616d 653a 2073 7472 0d0a 2020  mf_name: str..  
-000058e0: 2020 2020 2020 3a70 6172 616d 206b 7661        :param kva
-000058f0: 6c73 3a20 5261 6e6b 7320 666f 7220 634e  ls: Ranks for cN
-00005900: 4d46 2066 6163 746f 7269 7a61 7469 6f6e  MF factorization
-00005910: 2c20 6465 6661 756c 7473 2074 6f20 7261  , defaults to ra
-00005920: 6e67 6528 322c 2036 3129 0d0a 2020 2020  nge(2, 61)..    
-00005930: 2020 2020 3a74 7970 6520 6b76 616c 733a      :type kvals:
-00005940: 2043 6f6c 6c65 6374 696f 6e2c 206f 7074   Collection, opt
-00005950: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
-00005960: 7061 7261 6d20 6e5f 6974 6572 3a20 4e75  param n_iter: Nu
-00005970: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
-00005980: 6e73 2066 726f 6d20 7768 6963 6820 746f  ns from which to
-00005990: 2062 7569 6c64 2061 2063 6f6e 7365 6e73   build a consens
-000059a0: 7573 2073 6f6c 7574 696f 6e2c 2064 6566  us solution, def
-000059b0: 6175 6c74 7320 746f 2032 3030 0d0a 2020  aults to 200..  
-000059c0: 2020 2020 2020 3a74 7970 6520 6e5f 6974        :type n_it
-000059d0: 6572 3a20 696e 742c 206f 7074 696f 6e61  er: int, optiona
-000059e0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-000059f0: 6d20 6265 7461 5f6c 6f73 733a 2062 6574  m beta_loss: bet
-00005a00: 612d 6c6f 7373 2066 756e 6374 696f 6e2c  a-loss function,
-00005a10: 2065 6974 6865 7220 226b 756c 6c62 6163   either "kullbac
-00005a20: 6b2d 6c65 6962 6c65 7222 206f 7220 2266  k-leibler" or "f
-00005a30: 726f 6265 6e69 7573 222e 2044 6566 6175  robenius". Defau
-00005a40: 6c74 7320 746f 2022 6b75 6c6c 6261 636b  lts to "kullback
-00005a50: 2d6c 6569 626c 6572 220d 0a20 2020 2020  -leibler"..     
-00005a60: 2020 203a 7479 7065 2062 6574 615f 6c6f     :type beta_lo
-00005a70: 7373 3a20 7374 722c 206f 7074 696f 6e61  ss: str, optiona
-00005a80: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-00005a90: 6d20 7365 6564 3a20 5261 6e64 6f6d 2073  m seed: Random s
-00005aa0: 6565 6420 666f 7220 7265 7072 6f64 7563  eed for reproduc
-00005ab0: 6962 696c 6974 792c 2064 6566 6175 6c74  ibility, default
-00005ac0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-00005ad0: 2020 203a 7479 7065 2073 6565 643a 204f     :type seed: O
-00005ae0: 7074 696f 6e61 6c5b 696e 745d 2c20 6f70  ptional[int], op
-00005af0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00005b00: 3a72 6574 7572 6e3a 2063 4e4d 4620 6f62  :return: cNMF ob
-00005b10: 6a65 6374 0d0a 2020 2020 2020 2020 3a72  ject..        :r
-00005b20: 7479 7065 3a20 3a63 6c61 7373 3a60 636e  type: :class:`cn
-00005b30: 6d66 736e 732e 636e 6d66 2e63 4e4d 4660  mfsns.cnmf.cNMF`
-00005b40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005b50: 2020 2020 2020 2063 6e6d 665f 6f62 6a20         cnmf_obj 
-00005b60: 3d20 636e 6d66 2e63 4e4d 4628 6f75 7470  = cnmf.cNMF(outp
-00005b70: 7574 5f64 6972 3d63 6e6d 665f 6f75 7470  ut_dir=cnmf_outp
-00005b80: 7574 5f64 6972 2c20 6e61 6d65 3d63 6e6d  ut_dir, name=cnm
-00005b90: 665f 6e61 6d65 290d 0a20 2020 2020 2020  f_name)..       
-00005ba0: 200d 0a20 2020 2020 2020 2023 2077 7269   ..        # wri
-00005bb0: 7465 2054 504d 2028 6e6f 726d 616c 697a  te TPM (normaliz
-00005bc0: 6564 2920 6461 7461 0d0a 2020 2020 2020  ed) data..      
-00005bd0: 2020 7470 6d20 3d20 6164 2e41 6e6e 4461    tpm = ad.AnnDa
-00005be0: 7461 2873 656c 662e 746f 5f64 6628 6e6f  ta(self.to_df(no
-00005bf0: 726d 616c 697a 6564 3d54 7275 6529 290d  rmalized=True)).
-00005c00: 0a20 2020 2020 2020 2074 706d 2e77 7269  .        tpm.wri
-00005c10: 7465 5f68 3561 6428 636e 6d66 5f6f 626a  te_h5ad(cnmf_obj
-00005c20: 2e70 6174 6873 5b22 7470 6d22 5d29 0d0a  .paths["tpm"])..
-00005c30: 0d0a 2020 2020 2020 2020 6765 6e65 5f74  ..        gene_t
-00005c40: 706d 5f6d 6561 6e20 3d20 6e70 2e61 7272  pm_mean = np.arr
-00005c50: 6179 2874 706d 2e58 2e6d 6561 6e28 6178  ay(tpm.X.mean(ax
-00005c60: 6973 3d30 2929 2e72 6573 6861 7065 282d  is=0)).reshape(-
-00005c70: 3129 0d0a 2020 2020 2020 2020 6765 6e65  1)..        gene
-00005c80: 5f74 706d 5f73 7464 6465 7620 3d20 6e70  _tpm_stddev = np
-00005c90: 2e61 7272 6179 2874 706d 2e58 2e73 7464  .array(tpm.X.std
-00005ca0: 2861 7869 733d 302c 2064 646f 663d 3029  (axis=0, ddof=0)
-00005cb0: 292e 7265 7368 6170 6528 2d31 290d 0a20  ).reshape(-1).. 
-00005cc0: 2020 2020 2020 2069 6e70 7574 5f74 706d         input_tpm
-00005cd0: 5f73 7461 7473 203d 2070 642e 4461 7461  _stats = pd.Data
-00005ce0: 4672 616d 6528 5b67 656e 655f 7470 6d5f  Frame([gene_tpm_
-00005cf0: 6d65 616e 2c20 6765 6e65 5f74 706d 5f73  mean, gene_tpm_s
-00005d00: 7464 6465 765d 2c20 696e 6465 7820 3d20  tddev], index = 
-00005d10: 5b27 5f5f 6d65 616e 272c 2027 5f5f 7374  ['__mean', '__st
-00005d20: 6427 5d29 2e54 0d0a 2020 2020 2020 2020  d']).T..        
-00005d30: 7574 696c 732e 7361 7665 5f64 665f 746f  utils.save_df_to
-00005d40: 5f6e 707a 2869 6e70 7574 5f74 706d 5f73  _npz(input_tpm_s
-00005d50: 7461 7473 2c20 636e 6d66 5f6f 626a 2e70  tats, cnmf_obj.p
-00005d60: 6174 6873 5b27 7470 6d5f 7374 6174 7327  aths['tpm_stats'
-00005d70: 5d29 0d0a 2020 2020 2020 2020 6f76 6572  ])..        over
-00005d80: 6469 7370 6572 7365 645f 6765 6e65 7320  dispersed_genes 
-00005d90: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00005da0: 5b22 7365 6c65 6374 6564 225d 5b73 656c  ["selected"][sel
-00005db0: 662e 6164 6174 612e 7661 725b 2273 656c  f.adata.var["sel
-00005dc0: 6563 7465 6422 5d5d 2e69 6e64 6578 0d0a  ected"]].index..
-00005dd0: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
-00005de0: 6e74 7320 3d20 636e 6d66 5f6f 626a 2e67  nts = cnmf_obj.g
-00005df0: 6574 5f6e 6f72 6d5f 636f 756e 7473 2873  et_norm_counts(s
-00005e00: 656c 662e 6164 6174 612c 2074 706d 2c20  elf.adata, tpm, 
-00005e10: 6869 6768 5f76 6172 6961 6e63 655f 6765  high_variance_ge
-00005e20: 6e65 735f 6669 6c74 6572 3d6f 7665 7264  nes_filter=overd
-00005e30: 6973 7065 7273 6564 5f67 656e 6573 290d  ispersed_genes).
-00005e40: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
-00005e50: 5f63 6f75 6e74 732e 582e 6474 7970 6520  _counts.X.dtype 
-00005e60: 213d 206e 702e 666c 6f61 7436 343a 0d0a  != np.float64:..
-00005e70: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-00005e80: 5f63 6f75 6e74 732e 5820 3d20 6e6f 726d  _counts.X = norm
-00005e90: 5f63 6f75 6e74 732e 582e 6173 7479 7065  _counts.X.astype
-00005ea0: 286e 702e 666c 6f61 7436 3429 0d0a 2020  (np.float64)..  
-00005eb0: 2020 2020 2020 636e 6d66 5f6f 626a 2e73        cnmf_obj.s
-00005ec0: 6176 655f 6e6f 726d 5f63 6f75 6e74 7328  ave_norm_counts(
-00005ed0: 6e6f 726d 5f63 6f75 6e74 7329 0d0a 0d0a  norm_counts)....
-00005ee0: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
-00005ef0: 6172 616d 6574 6572 7320 666f 7220 6661  arameters for fa
-00005f00: 6374 6f72 697a 6174 696f 6e20 7374 6570  ctorization step
-00005f10: 0d0a 2020 2020 2020 2020 636e 6d66 5f6f  ..        cnmf_o
-00005f20: 626a 2e73 6176 655f 6e6d 665f 6974 6572  bj.save_nmf_iter
-00005f30: 5f70 6172 616d 7328 2a63 6e6d 665f 6f62  _params(*cnmf_ob
-00005f40: 6a2e 6765 745f 6e6d 665f 6974 6572 5f70  j.get_nmf_iter_p
-00005f50: 6172 616d 7328 6b73 3d6b 7661 6c73 2c20  arams(ks=kvals, 
-00005f60: 6e5f 6974 6572 3d6e 5f69 7465 722c 2072  n_iter=n_iter, r
-00005f70: 616e 646f 6d5f 7374 6174 655f 7365 6564  andom_state_seed
-00005f80: 3d73 6565 642c 2062 6574 615f 6c6f 7373  =seed, beta_loss
-00005f90: 3d62 6574 615f 6c6f 7373 2929 0d0a 0d0a  =beta_loss))....
-00005fa0: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
-00005fb0: 6172 616d 6574 6572 7320 696e 2041 6e6e  arameters in Ann
-00005fc0: 4461 7461 206f 626a 6563 740d 0a20 2020  Data object..   
-00005fd0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00005fe0: 756e 735b 2263 6e6d 6622 5d20 3d20 636e  uns["cnmf"] = cn
-00005ff0: 6d66 5f6f 626a 2e67 6574 5f6e 6d66 5f69  mf_obj.get_nmf_i
-00006000: 7465 725f 7061 7261 6d73 286b 733d 6b76  ter_params(ks=kv
-00006010: 616c 732c 206e 5f69 7465 723d 6e5f 6974  als, n_iter=n_it
-00006020: 6572 2c20 7261 6e64 6f6d 5f73 7461 7465  er, random_state
-00006030: 5f73 6565 643d 7365 6564 2c20 6265 7461  _seed=seed, beta
-00006040: 5f6c 6f73 733d 6265 7461 5f6c 6f73 7329  _loss=beta_loss)
-00006050: 5b31 5d20 2023 2064 6963 7420 6f66 2063  [1]  # dict of c
-00006060: 6e6d 6620 7061 7261 6d65 7465 7273 0d0a  nmf parameters..
-00006070: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00006080: 2020 7365 6c66 2e61 7070 656e 645f 746f    self.append_to
-00006090: 5f68 6973 746f 7279 2866 2263 4e4d 4620  _history(f"cNMF 
-000060a0: 7061 7261 6d65 7465 7273 2061 6464 6564  parameters added
-000060b0: 2e20 634e 4d46 2069 6e70 7574 7320 696e  . cNMF inputs in
-000060c0: 6974 6961 6c69 7a65 6420 696e 207b 636e  itialized in {cn
-000060d0: 6d66 5f6f 7574 7075 745f 6469 727d 2f7b  mf_output_dir}/{
-000060e0: 636e 6d66 5f6e 616d 657d 2229 0d0a 2020  cnmf_name}")..  
-000060f0: 2020 2020 2020 7265 7475 726e 2063 6e6d        return cnm
-00006100: 665f 6f62 6a0d 0a20 2020 200d 0a20 2020  f_obj..    ..   
-00006110: 2064 6566 2061 6464 5f63 6e6d 665f 7265   def add_cnmf_re
-00006120: 7375 6c74 7328 7365 6c66 2c20 636e 6d66  sults(self, cnmf
-00006130: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
-00006140: 665f 6e61 6d65 2c20 6c6f 6361 6c5f 6465  f_name, local_de
-00006150: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
-00006160: 2066 6c6f 6174 203d 204e 6f6e 652c 206c   float = None, l
-00006170: 6f63 616c 5f6e 6569 6768 626f 7268 6f6f  ocal_neighborhoo
-00006180: 645f 7369 7a65 3a20 666c 6f61 7420 3d20  d_size: float = 
-00006190: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-000061a0: 2222 220d 0a20 2020 2020 2020 2041 6674  """..        Aft
-000061b0: 6572 2066 6163 746f 7269 7a61 7469 6f6e  er factorization
-000061c0: 2c20 6164 6420 636f 6d70 6c65 7465 6420  , add completed 
-000061d0: 634e 4d46 2072 6573 756c 7473 2069 6e20  cNMF results in 
-000061e0: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
-000061f0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d20 746f  ]/[cnmf_name] to
-00006200: 2074 6865 2064 6174 6173 6574 206f 626a   the dataset obj
-00006210: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
-00006220: 3a70 6172 616d 2063 6e6d 665f 6f75 7470  :param cnmf_outp
-00006230: 7574 5f64 6972 3a20 4f75 7470 7574 2064  ut_dir: Output d
-00006240: 6972 6563 746f 7279 2066 6f72 2063 4e4d  irectory for cNM
-00006250: 4620 7265 7375 6c74 730d 0a20 2020 2020  F results..     
-00006260: 2020 203a 7479 7065 2063 6e6d 665f 6f75     :type cnmf_ou
-00006270: 7470 7574 5f64 6972 3a20 7374 720d 0a20  tput_dir: str.. 
-00006280: 2020 2020 2020 203a 7061 7261 6d20 636e         :param cn
-00006290: 6d66 5f6e 616d 653a 204e 616d 6520 6f66  mf_name: Name of
-000062a0: 2074 6865 2063 4e4d 4620 7265 7375 6c74   the cNMF result
-000062b0: 732e 2046 696c 6573 2077 696c 6c20 6265  s. Files will be
-000062c0: 206f 7574 7075 7420 746f 205b 636e 6d66   output to [cnmf
-000062d0: 5f6f 7574 7075 745f 6469 725d 2f5b 636e  _output_dir]/[cn
-000062e0: 6d66 5f6e 616d 655d 2f0d 0a20 2020 2020  mf_name]/..     
-000062f0: 2020 203a 7479 7065 2063 6e6d 665f 6e61     :type cnmf_na
-00006300: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
-00006310: 203a 7061 7261 6d20 6c6f 6361 6c5f 6465   :param local_de
-00006320: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
-00006330: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
-00006340: 6865 206c 6f63 616c 2064 656e 7369 7479  he local density
-00006350: 2066 696c 7465 7269 6e67 2070 7269 6f72   filtering prior
-00006360: 2074 6f20 4745 5020 636f 6e73 656e 7375   to GEP consensu
-00006370: 732e 2041 6363 6570 7461 626c 6520 7468  s. Acceptable th
-00006380: 7265 7368 6f6c 6473 2061 7265 203e 2030  resholds are > 0
-00006390: 2061 6e64 203c 3d20 3220 2832 2e30 2069   and <= 2 (2.0 i
-000063a0: 7320 6e6f 2066 696c 7465 7269 6e67 292e  s no filtering).
-000063b0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-000063c0: 652e 0d0a 2020 2020 2020 2020 3a74 7970  e...        :typ
-000063d0: 6520 6c6f 6361 6c5f 6465 6e73 6974 795f  e local_density_
-000063e0: 7468 7265 7368 6f6c 643a 2066 6c6f 6174  threshold: float
-000063f0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00006400: 2020 2020 3a70 6172 616d 206c 6f63 616c      :param local
-00006410: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
-00006420: 7a65 3a20 4672 6163 7469 6f6e 206f 6620  ze: Fraction of 
-00006430: 7468 6520 6e75 6d62 6572 206f 6620 7265  the number of re
-00006440: 706c 6963 6174 6573 2074 6f20 7573 6520  plicates to use 
-00006450: 6173 206e 6561 7265 7374 206e 6569 6768  as nearest neigh
-00006460: 626f 7273 2066 6f72 206c 6f63 616c 2064  bors for local d
-00006470: 656e 7369 7479 2066 696c 7465 7269 6e67  ensity filtering
-00006480: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00006490: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
-000064a0: 6520 6c6f 6361 6c5f 6e65 6967 6862 6f72  e local_neighbor
-000064b0: 686f 6f64 5f73 697a 653a 2066 6c6f 6174  hood_size: float
-000064c0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-000064d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000064e0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-000064f0: 2263 6e6d 665f 6e61 6d65 225d 203d 2063  "cnmf_name"] = c
-00006500: 6e6d 665f 6e61 6d65 0d0a 0d0a 2020 2020  nmf_name....    
-00006510: 2020 2020 2320 696e 6665 7220 6672 6f6d      # infer from
-00006520: 2066 696c 656e 616d 6573 2077 6869 6368   filenames which
-00006530: 206c 6f63 616c 2064 656e 7369 7479 2074   local density t
-00006540: 6872 6573 686f 6c64 2077 6173 2075 7365  hreshold was use
-00006550: 640d 0a20 2020 2020 2020 2073 656e 7365  d..        sense
-00006560: 645f 6c64 7473 203d 2073 6574 2829 0d0a  d_ldts = set()..
-00006570: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-00006580: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
-00006590: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
-000065a0: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
-000065b0: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e2a  f"{cnmf_name}*.*
-000065c0: 7370 6563 7472 612a 2e6b 5f2a 2229 293a  spectra*.k_*")):
-000065d0: 0d0a 2020 2020 2020 2020 2020 2020 6c64  ..            ld
-000065e0: 745f 7374 7220 3d20 6f73 2e70 6174 682e  t_str = os.path.
-000065f0: 6261 7365 6e61 6d65 2866 6e29 2e73 706c  basename(fn).spl
-00006600: 6974 2822 2e22 295b 2d33 5d0d 0a20 2020  it(".")[-3]..   
-00006610: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00006620: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00006630: 6474 203d 2066 6c6f 6174 286c 6474 5f73  dt = float(ldt_s
-00006640: 7472 2e72 6570 6c61 6365 2822 6474 5f22  tr.replace("dt_"
-00006650: 2c20 2222 292e 7265 706c 6163 6528 225f  , "").replace("_
-00006660: 222c 2022 2e22 2929 0d0a 2020 2020 2020  ", "."))..      
-00006670: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-00006680: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
-00006690: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-000066a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000066b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000066c0: 2020 2073 656e 7365 645f 6c64 7473 2e61     sensed_ldts.a
-000066d0: 6464 2828 6c64 745f 7374 722c 206c 6474  dd((ldt_str, ldt
-000066e0: 2929 0d0a 2020 2020 2020 2020 6966 206c  ))..        if l
-000066f0: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
-00006700: 6573 686f 6c64 2069 7320 4e6f 6e65 2061  eshold is None a
-00006710: 6e64 206c 656e 2873 656e 7365 645f 6c64  nd len(sensed_ld
-00006720: 7473 2920 3d3d 2031 3a0d 0a20 2020 2020  ts) == 1:..     
-00006730: 2020 2020 2020 206c 6474 5f73 7472 2c20         ldt_str, 
-00006740: 6c64 7420 3d20 7365 6e73 6564 5f6c 6474  ldt = sensed_ldt
-00006750: 732e 706f 7028 290d 0a20 2020 2020 2020  s.pop()..       
-00006760: 2065 6c69 6620 6c6f 6361 6c5f 6465 6e73   elif local_dens
-00006770: 6974 795f 7468 7265 7368 6f6c 6420 696e  ity_threshold in
-00006780: 2028 6c64 745b 315d 2066 6f72 206c 6474   (ldt[1] for ldt
-00006790: 2069 6e20 7365 6e73 6564 5f6c 6474 7329   in sensed_ldts)
-000067a0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-000067b0: 6474 5f73 7472 2c20 6c64 7420 3d20 5b28  dt_str, ldt = [(
-000067c0: 6c64 745f 7374 722c 206c 6474 2920 666f  ldt_str, ldt) fo
-000067d0: 7220 6c64 745f 7374 722c 206c 6474 2069  r ldt_str, ldt i
-000067e0: 6e20 7365 6e73 6564 5f6c 6474 7320 6966  n sensed_ldts if
-000067f0: 206c 6474 203d 3d20 6c6f 6361 6c5f 6465   ldt == local_de
-00006800: 6e73 6974 795f 7468 7265 7368 6f6c 645d  nsity_threshold]
-00006810: 2e70 6f70 2829 0d0a 2020 2020 2020 2020  .pop()..        
-00006820: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00006830: 2020 206c 6f67 6769 6e67 2e65 7272 6f72     logging.error
-00006840: 2866 226c 6f63 616c 5f64 656e 7369 7479  (f"local_density
-00006850: 5f74 6872 6573 686f 6c64 206f 6620 7b6c  _threshold of {l
-00006860: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
-00006870: 6573 686f 6c64 7d20 646f 6573 206e 6f74  eshold} does not
-00006880: 206d 6174 6368 2077 6861 7420 6973 2069   match what is i
-00006890: 6e20 7468 6520 634e 4d46 2072 6573 756c  n the cNMF resul
-000068a0: 7420 6469 7265 6374 6f72 793a 207b 7365  t directory: {se
-000068b0: 6e73 6564 5f6c 6474 737d 2229 0d0a 2020  nsed_ldts}")..  
-000068c0: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
-000068d0: 6974 2831 290d 0a20 2020 2020 2020 2073  it(1)..        s
-000068e0: 656c 662e 6164 6174 612e 756e 735b 226c  elf.adata.uns["l
-000068f0: 6474 225d 203d 206c 6474 0d0a 2020 2020  dt"] = ldt..    
-00006900: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-00006910: 6e73 5b22 6c6e 7322 5d20 3d20 6c6f 6361  ns["lns"] = loca
-00006920: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
-00006930: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
-00006940: 200d 0a20 2020 2020 2020 2023 2049 6d70   ..        # Imp
-00006950: 6f72 7420 4745 5073 0d0a 2020 2020 2020  ort GEPs..      
-00006960: 2020 7265 7375 6c74 5f74 7970 6573 203d    result_types =
-00006970: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00006980: 2267 656e 655f 7370 6563 7472 615f 7363  "gene_spectra_sc
-00006990: 6f72 6522 3a20 2263 6e6d 665f 6765 705f  ore": "cnmf_gep_
-000069a0: 7363 6f72 6522 2c0d 0a20 2020 2020 2020  score",..       
-000069b0: 2020 2020 2022 6765 6e65 5f73 7065 6374       "gene_spect
-000069c0: 7261 5f74 706d 223a 2022 636e 6d66 5f67  ra_tpm": "cnmf_g
-000069d0: 6570 5f74 706d 222c 0d0a 2020 2020 2020  ep_tpm",..      
-000069e0: 2020 2020 2020 2273 7065 6374 7261 223a        "spectra":
-000069f0: 2022 636e 6d66 5f67 6570 5f72 6177 220d   "cnmf_gep_raw".
-00006a00: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00006a10: 2020 2020 2020 2020 666f 7220 6d61 7463          for matc
-00006a20: 6873 7472 2c20 7265 7375 6c74 5f74 7970  hstr, result_typ
-00006a30: 6520 696e 2072 6573 756c 745f 7479 7065  e in result_type
-00006a40: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-00006a50: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00006a60: 696e 666f 2866 2249 6d70 6f72 7469 6e67  info(f"Importing
-00006a70: 2047 4550 733a 207b 6d61 7463 6873 7472   GEPs: {matchstr
-00006a80: 7d22 2920 200d 0a20 2020 2020 2020 2020  }")  ..         
-00006a90: 2020 206d 6574 615f 7720 3d20 5b5d 0d0a     meta_w = []..
-00006aa0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00006ab0: 666e 2069 6e20 676c 6f62 286f 732e 7061  fn in glob(os.pa
-00006ac0: 7468 2e6a 6f69 6e28 636e 6d66 5f6f 7574  th.join(cnmf_out
-00006ad0: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
-00006ae0: 6d65 2c20 6622 7b63 6e6d 665f 6e61 6d65  me, f"{cnmf_name
-00006af0: 7d2a 2e7b 6d61 7463 6873 7472 7d2e 6b5f  }*.{matchstr}.k_
-00006b00: 2a2e 7b6c 6474 5f73 7472 7d2e 2a74 7874  *.{ldt_str}.*txt
-00006b10: 2229 293a 0d0a 2020 2020 2020 2020 2020  ")):..          
-00006b20: 2020 2020 2020 6b20 3d20 696e 7428 6f73        k = int(os
-00006b30: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
-00006b40: 6e29 2e72 656d 6f76 6570 7265 6669 7828  n).removeprefix(
-00006b50: 6622 7b63 6e6d 665f 6e61 6d65 7d2e 7b6d  f"{cnmf_name}.{m
-00006b60: 6174 6368 7374 727d 2e22 292e 7370 6c69  atchstr}.").spli
-00006b70: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
-00006b80: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
-00006b90: 2020 2020 2020 2020 2020 2020 2020 7720                w 
-00006ba0: 3d20 7064 2e72 6561 645f 7461 626c 6528  = pd.read_table(
-00006bb0: 666e 2c20 696e 6465 785f 636f 6c3d 3029  fn, index_col=0)
-00006bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006bd0: 2020 772e 696e 6465 7820 3d20 7374 7228    w.index = str(
-00006be0: 6b29 202b 2022 2e22 202b 2077 2e69 6e64  k) + "." + w.ind
-00006bf0: 6578 2e61 7374 7970 6528 7374 7229 0d0a  ex.astype(str)..
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 6d65 7461 5f77 2e61 7070 656e 6428 7729  meta_w.append(w)
-00006c20: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
-00006c30: 7461 5f77 203d 2070 642e 636f 6e63 6174  ta_w = pd.concat
-00006c40: 286d 6574 615f 772c 2061 7869 733d 3029  (meta_w, axis=0)
-00006c50: 2e54 2e72 6569 6e64 6578 2873 656c 662e  .T.reindex(self.
-00006c60: 6164 6174 612e 7661 722e 696e 6465 7829  adata.var.index)
-00006c70: 2e72 656e 616d 655f 6178 6973 285b 226b  .rename_axis(["k
-00006c80: 2e67 6570 225d 2c20 6178 6973 3d31 290d  .gep"], axis=1).
-00006c90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006ca0: 662e 6164 6174 612e 7661 726d 5b72 6573  f.adata.varm[res
-00006cb0: 756c 745f 7479 7065 5d20 3d20 6d65 7461  ult_type] = meta
-00006cc0: 5f77 0d0a 0d0a 2020 2020 2020 2020 2320  _w....        # 
-00006cd0: 496d 706f 7274 2055 7361 6765 730d 0a20  Import Usages.. 
-00006ce0: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
-00006cf0: 6e66 6f28 6622 496d 706f 7274 696e 6720  nfo(f"Importing 
-00006d00: 5573 6167 6573 2229 2020 0d0a 2020 2020  Usages")  ..    
-00006d10: 2020 2020 7573 6167 6520 3d20 5b5d 0d0a      usage = []..
-00006d20: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-00006d30: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
-00006d40: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
-00006d50: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
-00006d60: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e75  f"{cnmf_name}*.u
-00006d70: 7361 6765 732e 6b5f 2a2e 7b6c 6474 5f73  sages.k_*.{ldt_s
-00006d80: 7472 7d2e 2a74 7874 2229 293a 0d0a 2020  tr}.*txt")):..  
-00006d90: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-00006da0: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
-00006db0: 6d65 2866 6e29 2e72 656d 6f76 6570 7265  me(fn).removepre
-00006dc0: 6669 7828 6622 7b63 6e6d 665f 6e61 6d65  fix(f"{cnmf_name
-00006dd0: 7d2e 7573 6167 6573 2e22 292e 7370 6c69  }.usages.").spli
-00006de0: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
-00006df0: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
-00006e00: 2020 2020 2020 2020 2020 6820 3d20 7064            h = pd
-00006e10: 2e72 6561 645f 7461 626c 6528 666e 2c20  .read_table(fn, 
-00006e20: 696e 6465 785f 636f 6c3d 3029 0d0a 2020  index_col=0)..  
-00006e30: 2020 2020 2020 2020 2020 682e 636f 6c75            h.colu
-00006e40: 6d6e 7320 3d20 7374 7228 6b29 202b 2022  mns = str(k) + "
-00006e50: 2e22 202b 2068 2e63 6f6c 756d 6e73 2e61  ." + h.columns.a
-00006e60: 7374 7970 6528 7374 7229 0d0a 2020 2020  stype(str)..    
-00006e70: 2020 2020 2020 2020 7573 6167 652e 6170          usage.ap
-00006e80: 7065 6e64 2868 290d 0a20 2020 2020 2020  pend(h)..       
-00006e90: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
-00006ea0: 5b22 636e 6d66 5f75 7361 6765 225d 203d  ["cnmf_usage"] =
-00006eb0: 2070 642e 636f 6e63 6174 2875 7361 6765   pd.concat(usage
-00006ec0: 2c20 6178 6973 3d31 292e 736f 7274 5f69  , axis=1).sort_i
-00006ed0: 6e64 6578 2861 7869 733d 3129 2e72 656e  ndex(axis=1).ren
-00006ee0: 616d 655f 6178 6973 285b 226b 2e67 6570  ame_axis(["k.gep
-00006ef0: 225d 2c20 6178 6973 3d31 290d 0a20 2020  "], axis=1)..   
-00006f00: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00006f10: 2049 6d70 6f72 7420 6765 6e65 206c 6973   Import gene lis
-00006f20: 7420 7573 6564 2066 6f72 2066 6163 746f  t used for facto
-00006f30: 7269 7a61 7469 6f6e 0d0a 2020 2020 2020  rization..      
-00006f40: 2020 7769 7468 206f 7065 6e28 6f73 2e70    with open(os.p
-00006f50: 6174 682e 6a6f 696e 2863 6e6d 665f 6f75  ath.join(cnmf_ou
-00006f60: 7470 7574 5f64 6972 2c20 636e 6d66 5f6e  tput_dir, cnmf_n
-00006f70: 616d 652c 2066 227b 636e 6d66 5f6e 616d  ame, f"{cnmf_nam
-00006f80: 657d 2e6f 7665 7264 6973 7065 7273 6564  e}.overdispersed
-00006f90: 5f67 656e 6573 2e74 7874 2229 2920 6173  _genes.txt")) as
-00006fa0: 2066 3a0d 0a20 2020 2020 2020 2020 2020   f:..           
-00006fb0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00006fc0: 2267 656e 655f 6c69 7374 225d 203d 205b  "gene_list"] = [
-00006fd0: 6c69 6e65 2e73 7472 6970 2829 2066 6f72  line.strip() for
-00006fe0: 206c 696e 6520 696e 2066 2e72 6561 646c   line in f.readl
-00006ff0: 696e 6573 2829 5d0d 0a0d 0a20 2020 2020  ines()]....     
-00007000: 2020 2023 2049 6d70 6f72 7420 4b2d 7365     # Import K-se
-00007010: 6c65 6374 696f 6e20 7374 6174 730d 0a20  lection stats.. 
-00007020: 2020 2020 2020 206b 7661 6c73 203d 2070         kvals = p
-00007030: 642e 4461 7461 4672 616d 6528 2a2a 6e70  d.DataFrame(**np
-00007040: 2e6c 6f61 6428 6f73 2e70 6174 682e 6a6f  .load(os.path.jo
-00007050: 696e 2863 6e6d 665f 6f75 7470 7574 5f64  in(cnmf_output_d
-00007060: 6972 2c20 636e 6d66 5f6e 616d 652c 2066  ir, cnmf_name, f
-00007070: 227b 636e 6d66 5f6e 616d 657d 2e6b 5f73  "{cnmf_name}.k_s
-00007080: 656c 6563 7469 6f6e 5f73 7461 7473 2e64  election_stats.d
-00007090: 662e 6e70 7a22 292c 2061 6c6c 6f77 5f70  f.npz"), allow_p
-000070a0: 6963 6b6c 653d 5472 7565 2929 2e73 6574  ickle=True)).set
-000070b0: 5f69 6e64 6578 2822 6b22 295b 5b22 7374  _index("k")[["st
-000070c0: 6162 696c 6974 7922 2c20 2270 7265 6469  ability", "predi
-000070d0: 6374 696f 6e5f 6572 726f 7222 5d5d 0d0a  ction_error"]]..
-000070e0: 2020 2020 2020 2020 6b76 616c 732e 696e          kvals.in
-000070f0: 6465 7820 3d20 6b76 616c 732e 696e 6465  dex = kvals.inde
-00007100: 782e 6173 7479 7065 2869 6e74 290d 0a20  x.astype(int).. 
-00007110: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00007120: 612e 756e 735b 226b 7661 6c73 225d 203d  a.uns["kvals"] =
-00007130: 206b 7661 6c73 0d0a 2020 2020 2020 2020   kvals..        
-00007140: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
-00007150: 6973 746f 7279 2822 634e 4d46 2072 6573  istory("cNMF res
-00007160: 756c 7473 2061 6464 6564 2066 726f 6d20  ults added from 
-00007170: 6f75 7470 7574 2064 6972 6563 746f 7279  output directory
-00007180: 207b 636e 6d66 5f6f 7574 7075 745f 6469   {cnmf_output_di
-00007190: 727d 2f7b 636e 6d66 5f6e 616d 657d 2229  r}/{cnmf_name}")
-000071a0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-000071b0: 7573 6167 6573 2873 656c 662c 0d0a 2020  usages(self,..  
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 206b 3a20 556e 696f 6e5b 696e 742c 2049   k: Union[int, I
-000071e0: 7465 7261 626c 655d 203d 204e 6f6e 652c  terable] = None,
-000071f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007200: 2020 2020 2064 6973 6372 6574 697a 653a       discretize:
-00007210: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 206e 6f72 6d61 6c69 7a65 3a20 626f     normalize: bo
-00007240: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
-00007250: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007260: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-00007270: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00007280: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-00007290: 6520 7573 6167 6520 6f66 2065 6163 6820  e usage of each 
-000072a0: 4745 5020 696e 2065 6163 6820 7361 6d70  GEP in each samp
-000072b0: 6c65 2f6f 6273 6572 7661 7469 6f6e 2e0d  le/observation..
-000072c0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000072d0: 6d20 6b3a 2049 6620 616e 2069 6e74 6567  m k: If an integ
-000072e0: 6572 206f 7220 6c69 7374 206f 6620 696e  er or list of in
-000072f0: 7465 6765 7273 2c20 7265 7475 726e 7320  tegers, returns 
-00007300: 7573 6167 6573 206f 6e6c 7920 666f 7220  usages only for 
-00007310: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
-00007320: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
-00007330: 726e 7320 7573 6167 6520 6f66 2061 6c6c  rns usage of all
-00007340: 2047 4550 7320 6163 726f 7373 2072 616e   GEPs across ran
-00007350: 6b73 2e20 4465 6661 756c 7473 2074 6f20  ks. Defaults to 
-00007360: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
-00007370: 7970 6520 6b3a 2069 6e74 2c20 6f70 7469  ype k: int, opti
-00007380: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00007390: 6172 616d 2064 6973 6372 6574 697a 653a  aram discretize:
-000073a0: 2044 6973 6372 6574 697a 6573 2074 6865   Discretizes the
-000073b0: 2075 7361 6765 206d 6174 7269 7820 7375   usage matrix su
-000073c0: 6368 2074 6861 7420 666f 7220 6561 6368  ch that for each
-000073d0: 2076 616c 7565 206f 6620 6b2c 2065 6163   value of k, eac
-000073e0: 6820 7361 6d70 6c65 2068 6173 2075 7361  h sample has usa
-000073f0: 6765 206f 6620 6f6e 6c79 2031 2047 4550  ge of only 1 GEP
-00007400: 2028 7468 6520 6f6e 6520 7769 7468 2074   (the one with t
-00007410: 6865 206d 6178 696d 756d 2075 7361 6765  he maximum usage
-00007420: 292e 2044 6566 6175 6c74 7320 746f 2046  ). Defaults to F
-00007430: 616c 7365 0d0a 2020 2020 2020 2020 3a74  alse..        :t
-00007440: 7970 6520 6469 7363 7265 7469 7a65 3a20  ype discretize: 
-00007450: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
-00007460: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
-00007470: 6f72 6d61 6c69 7a65 3a20 4e6f 726d 616c  ormalize: Normal
-00007480: 697a 6520 7468 6520 4745 5020 7573 6167  ize the GEP usag
-00007490: 6520 6d61 7472 6978 2073 7563 6820 7468  e matrix such th
-000074a0: 6174 2066 6f72 2065 6163 6820 7661 6c75  at for each valu
-000074b0: 6520 6f66 206b 2c20 7573 6167 6520 6f66  e of k, usage of
-000074c0: 2061 6c6c 2047 4550 7320 7375 6d73 2074   all GEPs sums t
-000074d0: 6f20 312e 2044 6566 6175 6c74 7320 746f  o 1. Defaults to
-000074e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-000074f0: 3a74 7970 6520 6e6f 726d 616c 697a 653a  :type normalize:
-00007500: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00007510: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00007520: 3a20 6f62 7365 7276 6174 696f 6e20 c397  : observation ..
-00007530: 2047 4550 206d 6174 7269 780d 0a20 2020   GEP matrix..   
-00007540: 2020 2020 203a 7274 7970 653a 2070 642e       :rtype: pd.
-00007550: 4461 7461 4672 616d 650d 0a20 2020 2020  DataFrame..     
-00007560: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00007570: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
-00007580: 6f62 736d 5b22 636e 6d66 5f75 7361 6765  obsm["cnmf_usage
-00007590: 225d 2e63 6f70 7928 290d 0a20 2020 2020  "].copy()..     
-000075a0: 2020 2064 662e 636f 6c75 6d6e 7320 3d20     df.columns = 
-000075b0: 7064 2e4d 756c 7469 496e 6465 782e 6672  pd.MultiIndex.fr
-000075c0: 6f6d 5f74 7570 6c65 7328 6466 2e63 6f6c  om_tuples(df.col
-000075d0: 756d 6e73 2e73 7472 2e73 706c 6974 2822  umns.str.split("
-000075e0: 2e22 292e 746f 5f6c 6973 7428 2929 0d0a  .").to_list())..
-000075f0: 2020 2020 2020 2020 6466 2e63 6f6c 756d          df.colum
-00007600: 6e73 203d 2064 662e 636f 6c75 6d6e 732e  ns = df.columns.
-00007610: 7365 745f 6c65 7665 6c73 285b 6c2e 6173  set_levels([l.as
-00007620: 7479 7065 2822 696e 7422 2920 666f 7220  type("int") for 
-00007630: 6c20 696e 2064 662e 636f 6c75 6d6e 732e  l in df.columns.
-00007640: 6c65 7665 6c73 5d29 0d0a 2020 2020 2020  levels])..      
-00007650: 2020 6966 206e 6f72 6d61 6c69 7a65 3a0d    if normalize:.
-00007660: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
-00007670: 6d61 6c69 7a65 6420 3d20 5b5d 0d0a 2020  malized = []..  
-00007680: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
-00007690: 2073 7562 6466 2069 6e20 6466 2e67 726f   subdf in df.gro
-000076a0: 7570 6279 2861 7869 733d 312c 206c 6576  upby(axis=1, lev
-000076b0: 656c 3d30 293a 0d0a 2020 2020 2020 2020  el=0):..        
-000076c0: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
-000076d0: 6564 2e61 7070 656e 6428 7375 6264 662e  ed.append(subdf.
-000076e0: 6469 7628 7375 6264 662e 7375 6d28 6178  div(subdf.sum(ax
-000076f0: 6973 3d31 292c 2061 7869 733d 3029 290d  is=1), axis=0)).
-00007700: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
-00007710: 3d20 7064 2e63 6f6e 6361 7428 6e6f 726d  = pd.concat(norm
-00007720: 616c 697a 6564 2c20 6178 6973 3d31 290d  alized, axis=1).
-00007730: 0a20 2020 2020 2020 2069 6620 6469 7363  .        if disc
-00007740: 7265 7469 7a65 3a0d 0a20 2020 2020 2020  retize:..       
-00007750: 2020 2020 2064 6973 6372 6574 697a 6564       discretized
-00007760: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00007770: 2020 2066 6f72 205f 2c20 7375 6264 6620     for _, subdf 
-00007780: 696e 2064 662e 6772 6f75 7062 7928 6178  in df.groupby(ax
-00007790: 6973 3d31 2c20 6c65 7665 6c3d 3029 3a0d  is=1, level=0):.
-000077a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077b0: 2064 6973 6372 6574 697a 6564 2e61 7070   discretized.app
-000077c0: 656e 6428 7375 6264 662e 6571 2873 7562  end(subdf.eq(sub
-000077d0: 6466 2e6d 6178 2861 7869 733d 3129 2c20  df.max(axis=1), 
-000077e0: 6178 6973 3d30 292e 6173 7479 7065 2869  axis=0).astype(i
-000077f0: 6e74 2929 0d0a 2020 2020 2020 2020 2020  nt))..          
-00007800: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
-00007810: 2864 6973 6372 6574 697a 6564 2c20 6178  (discretized, ax
-00007820: 6973 3d31 2920 2020 2020 2020 200d 0a20  is=1)        .. 
-00007830: 2020 2020 2020 2069 6620 6b20 6973 206e         if k is n
-00007840: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00007850: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
-00007860: 635b 3a2c 206b 5d0d 0a20 2020 2020 2020  c[:, k]..       
-00007870: 2064 6620 3d20 6466 2e73 6f72 745f 696e   df = df.sort_in
-00007880: 6465 7828 6178 6973 3d30 292e 736f 7274  dex(axis=0).sort
-00007890: 5f69 6e64 6578 2861 7869 733d 3129 2020  _index(axis=1)  
-000078a0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-000078b0: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
-000078c0: 6465 6620 6765 745f 6765 7073 2873 656c  def get_geps(sel
-000078d0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-000078e0: 2020 2020 206b 3a20 556e 696f 6e5b 696e       k: Union[in
-000078f0: 742c 2049 7465 7261 626c 655d 203d 204e  t, Iterable] = N
-00007900: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00007910: 2020 2020 2020 2074 7970 653d 2263 6e6d         type="cnm
-00007920: 665f 6765 705f 7363 6f72 6522 0d0a 2020  f_gep_score"..  
-00007930: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007940: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-00007950: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00007960: 2020 2020 2020 2020 4765 7420 4745 5073          Get GEPs
-00007970: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
-00007980: 7261 6d20 6b3a 2049 6620 616e 2069 6e74  ram k: If an int
-00007990: 6567 6572 206f 7220 6c69 7374 206f 6620  eger or list of 
-000079a0: 696e 7465 6765 7273 2c20 7265 7475 726e  integers, return
-000079b0: 7320 4745 5073 206f 6e6c 7920 666f 7220  s GEPs only for 
-000079c0: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
-000079d0: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
-000079e0: 726e 7320 4745 5073 2066 726f 6d20 616c  rns GEPs from al
-000079f0: 6c20 7261 6e6b 732e 2044 6566 6175 6c74  l ranks. Default
-00007a00: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-00007a10: 2020 203a 7479 7065 206b 3a20 556e 696f     :type k: Unio
-00007a20: 6e5b 696e 742c 2049 7465 7261 626c 655d  n[int, Iterable]
-00007a30: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00007a40: 2020 2020 3a70 6172 616d 2074 7970 653a      :param type:
-00007a50: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
-00007a60: 2220 6f72 2022 636e 6d66 5f67 6570 5f74  " or "cnmf_gep_t
-00007a70: 706d 222c 2064 6566 6175 6c74 7320 746f  pm", defaults to
-00007a80: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
-00007a90: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
-00007aa0: 2074 7970 653a 2073 7472 2c20 6f70 7469   type: str, opti
-00007ab0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-00007ac0: 6574 7572 6e3a 2066 6561 7475 7265 7320  eturn: features 
-00007ad0: c397 2047 4550 206d 6174 7269 780d 0a20  .. GEP matrix.. 
-00007ae0: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
-00007af0: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
-00007b00: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00007b10: 2020 6466 203d 2073 656c 662e 6164 6174    df = self.adat
-00007b20: 612e 7661 726d 5b74 7970 655d 2e63 6f70  a.varm[type].cop
-00007b30: 7928 290d 0a20 2020 2020 2020 2064 662e  y()..        df.
-00007b40: 636f 6c75 6d6e 7320 3d20 7064 2e4d 756c  columns = pd.Mul
-00007b50: 7469 496e 6465 782e 6672 6f6d 5f74 7570  tiIndex.from_tup
-00007b60: 6c65 7328 6466 2e63 6f6c 756d 6e73 2e73  les(df.columns.s
-00007b70: 7472 2e73 706c 6974 2822 2e22 292e 746f  tr.split(".").to
-00007b80: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
-00007b90: 2020 6466 2e63 6f6c 756d 6e73 203d 2064    df.columns = d
-00007ba0: 662e 636f 6c75 6d6e 732e 7365 745f 6c65  f.columns.set_le
-00007bb0: 7665 6c73 285b 6c2e 6173 7479 7065 2822  vels([l.astype("
-00007bc0: 696e 7422 2920 666f 7220 6c20 696e 2064  int") for l in d
-00007bd0: 662e 636f 6c75 6d6e 732e 6c65 7665 6c73  f.columns.levels
-00007be0: 5d29 0d0a 2020 2020 2020 2020 6966 2069  ])..        if i
-00007bf0: 7369 6e73 7461 6e63 6528 6b2c 2028 696e  sinstance(k, (in
-00007c00: 742c 2049 7465 7261 626c 6529 293a 0d0a  t, Iterable)):..
-00007c10: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-00007c20: 2064 662e 6c6f 635b 3a2c 206b 5d0d 0a20   df.loc[:, k].. 
-00007c30: 2020 2020 2020 2064 6620 3d20 6466 2e73         df = df.s
-00007c40: 6f72 745f 696e 6465 7828 6178 6973 3d31  ort_index(axis=1
-00007c50: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00007c60: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
-00007c70: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
-00007c80: 5f64 6628 7365 6c66 2c0d 0a20 2020 2020  _df(self,..     
-00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ca0: 2020 2069 6e63 6c75 6465 5f63 6174 6567     include_categ
-00007cb0: 6f72 6963 616c 3a20 626f 6f6c 203d 2054  orical: bool = T
-00007cc0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00007ce0: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
-00007cf0: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 2020 2020 2020 2920 2d3e 2070 642e 4461        ) -> pd.Da
-00007d20: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
-00007d30: 2020 2222 2247 6574 2073 616d 706c 652f    """Get sample/
-00007d40: 6f62 7365 7276 6174 696f 6e20 6d65 7461  observation meta
-00007d50: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
-00007d60: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
-00007d70: 6361 7465 676f 7269 6361 6c3a 2049 6e63  categorical: Inc
-00007d80: 6c75 6465 2063 6174 6567 6f72 6963 616c  lude categorical
-00007d90: 206d 6574 6164 6174 6120 6c61 7965 7273   metadata layers
-00007da0: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
-00007db0: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
-00007dc0: 6520 696e 636c 7564 655f 6361 7465 676f  e include_catego
-00007dd0: 7269 6361 6c3a 2062 6f6f 6c2c 206f 7074  rical: bool, opt
-00007de0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
-00007df0: 7061 7261 6d20 696e 636c 7564 655f 6e75  param include_nu
-00007e00: 6d65 7269 6361 6c3a 2049 6e63 6c75 6465  merical: Include
-00007e10: 206e 756d 6572 6963 616c 206d 6574 6164   numerical metad
-00007e20: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
-00007e30: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
-00007e40: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
-00007e50: 7564 655f 6e75 6d65 7269 6361 6c3a 2062  ude_numerical: b
-00007e60: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
-00007e70: 2020 2020 2020 203a 7261 6973 6573 2056         :raises V
-00007e80: 616c 7565 4572 726f 723a 2045 7272 6f72  alueError: Error
-00007e90: 2069 6620 6d65 7461 6461 7461 2074 7970   if metadata typ
-00007ea0: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
-00007eb0: 6e69 7a65 640d 0a20 2020 2020 2020 203a  nized..        :
-00007ec0: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
-00007ed0: 696f 6e73 20c3 9720 6d65 7461 6461 7461  ions .. metadata
-00007ee0: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
-00007ef0: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
-00007f00: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
-00007f10: 2222 0d0a 2020 2020 2020 2020 6474 7970  ""..        dtyp
-00007f20: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-00007f30: 2069 6620 696e 636c 7564 655f 6361 7465   if include_cate
-00007f40: 676f 7269 6361 6c3a 0d0a 2020 2020 2020  gorical:..      
-00007f50: 2020 2020 2020 6474 7970 6573 2e61 7070        dtypes.app
-00007f60: 656e 6428 2263 6174 6567 6f72 7922 290d  end("category").
-00007f70: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
-00007f80: 7564 655f 6e75 6d65 7269 6361 6c3a 0d0a  ude_numerical:..
-00007f90: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-00007fa0: 6573 202b 3d20 5b22 666c 6f61 7422 2c20  es += ["float", 
-00007fb0: 2269 6e74 225d 0d0a 2020 2020 2020 2020  "int"]..        
-00007fc0: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
-00007fd0: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
-00007fe0: 732e 7365 6c65 6374 5f64 7479 7065 7328  s.select_dtypes(
-00007ff0: 6578 636c 7564 653d 2822 6361 7465 676f  exclude=("catego
-00008000: 7279 222c 2022 666c 6f61 7422 2c20 2269  ry", "float", "i
-00008010: 6e74 2229 292e 636f 6c75 6d6e 730d 0a20  nt")).columns.. 
-00008020: 2020 2020 2020 2069 6620 6c65 6e28 756e         if len(un
-00008030: 6578 706c 6169 6e65 645f 636f 6c73 2920  explained_cols) 
-00008040: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00008050: 2020 756e 6578 706c 6169 6e65 645f 636f    unexplained_co
-00008060: 6c5f 7374 7220 3d20 222c 2022 2e6a 6f69  l_str = ", ".joi
-00008070: 6e28 756e 6578 706c 6169 6e65 645f 636f  n(unexplained_co
-00008080: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
-00008090: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-000080a0: 7228 6622 7b75 6e65 7870 6c61 696e 6564  r(f"{unexplained
-000080b0: 5f63 6f6c 5f73 7472 7d20 6d65 7461 6461  _col_str} metada
-000080c0: 7461 2063 6f6c 756d 6e73 2068 6176 6520  ta columns have 
-000080d0: 756e 7265 636f 676e 697a 6564 2064 7479  unrecognized dty
-000080e0: 7065 732e 2229 0d0a 2020 2020 2020 2020  pes.")..        
-000080f0: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
-00008100: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
-00008110: 7328 696e 636c 7564 653d 6474 7970 6573  s(include=dtypes
-00008120: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
-00008130: 6466 2e64 726f 706e 6128 6178 6973 3d31  df.dropna(axis=1
-00008140: 2c20 686f 773d 2261 6c6c 2229 0d0a 2020  , how="all")..  
-00008150: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
-00008160: 0a20 2020 200d 0a20 2020 2064 6566 2067  .    ..    def g
-00008170: 6574 5f63 6174 6567 6f72 795f 6f76 6572  et_category_over
-00008180: 7265 7072 6573 656e 7461 7469 6f6e 2873  representation(s
-00008190: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000081c0: 7965 723a 2073 7472 2c0d 0a20 2020 2020  yer: str,..     
+00004670: 6d69 6e5f 6d65 616e 3a20 666c 6f61 7420  min_mean: float 
+00004680: 3d20 302c 0d0a 2020 2020 2020 2020 2020  = 0,..          
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 2020 206d 696e 5f73 636f           min_sco
+000046b0: 7265 3a20 666c 6f61 7420 3d20 312e 302c  re: float = 1.0,
+000046c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2074 6f70 5f6e 3a20 696e 7420       top_n: int 
+000046f0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004710: 2020 2020 2020 2020 2020 2020 7175 616e              quan
+00004720: 7469 6c65 3a20 666c 6f61 7420 3d20 4e6f  tile: float = No
+00004730: 6e65 293a 0d0a 2020 2020 2020 2020 2222  ne):..        ""
+00004740: 2253 656c 6563 7420 6f76 6572 6469 7370  "Select overdisp
+00004750: 6572 7365 6420 6765 6e65 732f 6665 6174  ersed genes/feat
+00004760: 7572 6573 2075 7369 6e67 2061 6e20 6f76  ures using an ov
+00004770: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
+00004780: 7269 632e 204f 7074 696f 6e61 6c6c 7920  ric. Optionally 
+00004790: 7365 7420 6120 6d69 6e69 6d75 6d20 6765  set a minimum ge
+000047a0: 6e65 2065 7870 7265 7373 696f 6e20 6c65  ne expression le
+000047b0: 7665 6c2e 0d0a 2020 2020 2020 2020 5365  vel...        Se
+000047c0: 7420 6120 7468 7265 7368 6f6c 6420 7573  t a threshold us
+000047d0: 696e 6720 7468 6520 746f 7020 4e20 2827  ing the top N ('
+000047e0: 746f 705f 6e27 292c 206d 696e 696d 756d  top_n'), minimum
+000047f0: 2073 636f 7265 2028 276d 696e 5f73 636f   score ('min_sco
+00004800: 7265 2729 2c20 6f72 2070 726f 706f 7274  re'), or proport
+00004810: 696f 6e20 6f66 2066 6561 7475 7265 7320  ion of features 
+00004820: 2827 7175 616e 7469 6c65 2729 206d 6574  ('quantile') met
+00004830: 686f 6473 2e0d 0a20 2020 2020 2020 204f  hods...        O
+00004840: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
+00004850: 6520 6c69 7374 2069 7320 7361 7665 6420  e list is saved 
+00004860: 696e 2074 6865 2044 6174 6173 6574 206f  in the Dataset o
+00004870: 626a 6563 742e 0d0a 0d0a 2020 2020 2020  bject.....      
+00004880: 2020 3a70 6172 616d 206f 7665 7264 6973    :param overdis
+00004890: 7065 7273 696f 6e5f 6d65 7472 6963 3a20  persion_metric: 
+000048a0: 226f 6473 636f 7265 2220 6f72 2022 7673  "odscore" or "vs
+000048b0: 636f 7265 222c 2064 6566 6175 6c74 7320  core", defaults 
+000048c0: 746f 2022 6f64 7363 6f72 6522 0d0a 2020  to "odscore"..  
+000048d0: 2020 2020 2020 3a74 7970 6520 6f76 6572        :type over
+000048e0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+000048f0: 633a 2073 7472 2c20 6f70 7469 6f6e 616c  c: str, optional
+00004900: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00004910: 206d 696e 5f6d 6561 6e3a 206d 696e 696d   min_mean: minim
+00004920: 756d 2067 656e 6520 6578 7072 6573 7369  um gene expressi
+00004930: 6f6e 2066 6f72 2067 656e 6573 2074 6f20  on for genes to 
+00004940: 6265 2063 6f75 6e74 6564 2061 7320 6f76  be counted as ov
+00004950: 6572 6469 7370 6572 7365 642c 2064 6566  erdispersed, def
+00004960: 6175 6c74 7320 746f 2030 0d0a 2020 2020  aults to 0..    
+00004970: 2020 2020 3a74 7970 6520 6d69 6e5f 6d65      :type min_me
+00004980: 616e 3a20 696e 742c 206f 7074 696f 6e61  an: int, optiona
+00004990: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+000049a0: 6d20 6d69 6e5f 7363 6f72 653a 206d 696e  m min_score: min
+000049b0: 696d 756d 2073 636f 7265 2066 6f72 206f  imum score for o
+000049c0: 7665 7264 6973 7065 7273 696f 6e2c 2064  verdispersion, d
+000049d0: 6566 6175 6c74 7320 746f 2031 2e30 0d0a  efaults to 1.0..
+000049e0: 2020 2020 2020 2020 3a74 7970 6520 6d69          :type mi
+000049f0: 6e5f 7363 6f72 653a 2066 6c6f 6174 2c20  n_score: float, 
+00004a00: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00004a10: 2020 3a70 6172 616d 2074 6f70 5f6e 3a20    :param top_n: 
+00004a20: 4368 6f6f 7365 2074 6865 2074 6f70 204e  Choose the top N
+00004a30: 206d 6f73 7420 6f76 6572 6469 7370 6572   most overdisper
+00004a40: 7365 6420 6765 6e65 732c 2064 6566 6175  sed genes, defau
+00004a50: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
+00004a60: 2020 2020 203a 7479 7065 2074 6f70 5f6e       :type top_n
+00004a70: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+00004a80: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00004a90: 7175 616e 7469 6c65 3a20 4368 6f6f 7365  quantile: Choose
+00004aa0: 2061 2071 7561 6e74 696c 6520 6f66 206f   a quantile of o
+00004ab0: 7665 7264 6973 7065 7273 696f 6e2e 2046  verdispersion. F
+00004ac0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00004ad0: 746f 7020 3130 2520 6f66 206f 7665 7264  top 10% of overd
+00004ae0: 6973 7065 7273 6564 2067 656e 6573 2077  ispersed genes w
+00004af0: 6f75 6c64 2062 6520 302e 3130 2e20 4465  ould be 0.10. De
+00004b00: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
+00004b10: 2020 2020 2020 2020 3a74 7970 6520 7175          :type qu
+00004b20: 616e 7469 6c65 3a20 666c 6f61 742c 206f  antile: float, o
+00004b30: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00004b40: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
+00004b50: 726f 723a 2045 7272 6f72 2069 6620 696e  ror: Error if in
+00004b60: 7661 6c69 6420 6f76 6572 6469 7370 6572  valid overdisper
+00004b70: 7369 6f6e 206d 6574 7269 6320 6973 2063  sion metric is c
+00004b80: 686f 7365 6e2e 0d0a 2020 2020 2020 2020  hosen...        
+00004b90: 2222 220d 0a20 2020 2020 2020 200d 0a20  """..        .. 
+00004ba0: 2020 2020 2020 2069 6620 6f76 6572 6469         if overdi
+00004bb0: 7370 6572 7369 6f6e 5f6d 6574 7269 6320  spersion_metric 
+00004bc0: 6e6f 7420 696e 2073 656c 662e 6164 6174  not in self.adat
+00004bd0: 612e 7661 722e 636f 6c75 6d6e 733a 0d0a  a.var.columns:..
+00004be0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00004bf0: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00004c00: 7472 6963 2069 6e20 2822 6f64 7363 6f72  tric in ("odscor
+00004c10: 6522 2c20 2276 7363 6f72 6522 293a 0d0a  e", "vscore"):..
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00004c40: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00004c50: 2020 2020 2020 2066 227b 6f76 6572 6469         f"{overdi
+00004c60: 7370 6572 7369 6f6e 5f6d 6574 7269 637d  spersion_metric}
+00004c70: 2068 6173 206e 6f74 2062 6565 6e20 6361   has not been ca
+00004c80: 6c63 756c 6174 6564 2066 6f72 2074 6869  lculated for thi
+00004c90: 7320 6461 7461 7365 742e 2022 0d0a 2020  s dataset. "..  
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2020 2245 6e73 7572 6520 7468 6174 2079    "Ensure that y
+00004cc0: 6f75 2063 616c 6c20 7468 6520 6044 6174  ou call the `Dat
+00004cd0: 6173 6574 2e63 6f6d 7075 7465 5f67 656e  aset.compute_gen
+00004ce0: 655f 7374 6174 7328 2960 2066 6972 7374  e_stats()` first
+00004cf0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+00004d00: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00004d10: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00004d20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00004d30: 6973 6520 5661 6c75 6545 7272 6f72 280d  ise ValueError(.
+00004d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d50: 2020 2020 2066 227b 6f76 6572 6469 7370       f"{overdisp
+00004d60: 6572 7369 6f6e 5f6d 6574 7269 637d 2069  ersion_metric} i
+00004d70: 7320 6e6f 7420 6120 7661 6c69 6420 6f76  s not a valid ov
+00004d80: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
+00004d90: 7269 632e 220d 0a20 2020 2020 2020 2020  ric."..         
+00004da0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00004db0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004dc0: 2320 7761 726e 2069 6620 6d75 6c74 6970  # warn if multip
+00004dd0: 6c65 206d 6574 686f 6473 2061 7265 2073  le methods are s
+00004de0: 656c 6563 7465 640d 0a20 2020 2020 2020  elected..       
+00004df0: 2073 656c 6563 7465 645f 6d65 7468 6f64   selected_method
+00004e00: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00004e10: 6966 206d 696e 5f73 636f 7265 2069 7320  if min_score is 
+00004e20: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00004e30: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+00004e40: 6d65 7468 6f64 732e 6170 7065 6e64 2822  methods.append("
+00004e50: 6d69 6e5f 7363 6f72 6522 290d 0a20 2020  min_score")..   
+00004e60: 2020 2020 2069 6620 746f 705f 6e20 6973       if top_n is
+00004e70: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00004e80: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004e90: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
+00004ea0: 2274 6f70 5f6e 2229 0d0a 2020 2020 2020  "top_n")..      
+00004eb0: 2020 6966 2071 7561 6e74 696c 6520 6973    if quantile is
+00004ec0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00004ed0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004ee0: 5f6d 6574 686f 6473 2e61 7070 656e 6428  _methods.append(
+00004ef0: 2271 7561 6e74 696c 6522 290d 0a20 2020  "quantile")..   
+00004f00: 2020 2020 2069 6620 6c65 6e28 7365 6c65       if len(sele
+00004f10: 6374 6564 5f6d 6574 686f 6473 2920 3e20  cted_methods) > 
+00004f20: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00004f30: 6d65 7468 6f64 7761 726e 7374 7220 3d20  methodwarnstr = 
+00004f40: 222c 2022 2e6a 6f69 6e28 7365 6c65 6374  ", ".join(select
+00004f50: 6564 5f6d 6574 686f 6473 290d 0a20 2020  ed_methods)..   
+00004f60: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00004f70: 2e77 6172 6e69 6e67 2866 224d 756c 7469  .warning(f"Multi
+00004f80: 706c 6520 636f 6e66 6c69 6374 696e 6720  ple conflicting 
+00004f90: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
+00004fa0: 6e65 2073 656c 6563 7469 6f6e 2063 7269  ne selection cri
+00004fb0: 7465 7269 6120 6861 7665 2062 6565 6e20  teria have been 
+00004fc0: 7365 6c65 6374 6564 3a20 7b6d 6574 686f  selected: {metho
+00004fd0: 6477 6172 6e73 7472 7d2e 2022 0d0a 2020  dwarnstr}. "..  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 2020 2020 2020 2020 224f 6e6c 7920            "Only 
+00005000: 7468 6520 696e 7465 7273 6563 7469 6f6e  the intersection
+00005010: 206f 6620 7468 6573 6520 6d65 7468 6f64   of these method
+00005020: 7320 7769 6c6c 2062 6520 7365 6c65 6374  s will be select
+00005030: 6564 2e22 290d 0a20 2020 2020 2020 2020  ed.")..         
+00005040: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005050: 2023 206d 696e 5f6d 6561 6e20 6669 6c74   # min_mean filt
+00005060: 6572 0d0a 2020 2020 2020 2020 7365 6c65  er..        sele
+00005070: 6374 6564 5f67 656e 6573 203d 2073 656c  cted_genes = sel
+00005080: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
+00005090: 6e5f 636f 756e 7473 225d 203e 3d20 6d69  n_counts"] >= mi
+000050a0: 6e5f 6d65 616e 0d0a 2020 2020 2020 2020  n_mean..        
+000050b0: 2320 6d69 6e5f 7363 6f72 6520 6669 6c74  # min_score filt
+000050c0: 6572 0d0a 2020 2020 2020 2020 6966 206d  er..        if m
+000050d0: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
+000050e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000050f0: 2020 2073 656c 6563 7465 645f 6765 6e65     selected_gene
+00005100: 7320 3d20 7365 6c65 6374 6564 5f67 656e  s = selected_gen
+00005110: 6573 2026 2028 7365 6c66 2e61 6461 7461  es & (self.adata
+00005120: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
+00005130: 696f 6e5f 6d65 7472 6963 5d20 3e3d 206d  ion_metric] >= m
+00005140: 696e 5f73 636f 7265 290d 0a20 2020 2020  in_score)..     
+00005150: 2020 2023 2074 6f70 5f6e 2066 696c 7465     # top_n filte
+00005160: 720d 0a20 2020 2020 2020 2069 6620 746f  r..        if to
+00005170: 705f 6e20 6973 206e 6f74 204e 6f6e 653a  p_n is not None:
+00005180: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+00005190: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
+000051a0: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
+000051b0: 696f 6e5f 6d65 7472 6963 5d2e 736f 7274  ion_metric].sort
+000051c0: 5f76 616c 7565 7328 6173 6365 6e64 696e  _values(ascendin
+000051d0: 673d 4661 6c73 6529 2e68 6561 6428 696e  g=False).head(in
+000051e0: 7428 746f 705f 6e29 292e 696e 6465 780d  t(top_n)).index.
+000051f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005200: 6563 7465 645f 6765 6e65 7320 3d20 7365  ected_genes = se
+00005210: 6c65 6374 6564 5f67 656e 6573 2026 2073  lected_genes & s
+00005220: 656c 662e 6164 6174 612e 7661 722e 696e  elf.adata.var.in
+00005230: 6465 782e 6973 696e 2867 656e 6573 290d  dex.isin(genes).
+00005240: 0a20 2020 2020 2020 2023 2071 7561 6e74  .        # quant
+00005250: 696c 6520 6669 6c74 6572 0d0a 2020 2020  ile filter..    
+00005260: 2020 2020 6966 2071 7561 6e74 696c 6520      if quantile 
+00005270: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00005280: 2020 2020 2020 2020 2020 6e5f 746f 7461            n_tota
+00005290: 6c5f 6765 6e65 7320 3d20 7365 6c66 2e61  l_genes = self.a
+000052a0: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
+000052b0: 7065 7273 696f 6e5f 6d65 7472 6963 5d2e  persion_metric].
+000052c0: 6e6f 746e 756c 6c28 292e 7375 6d28 290d  notnull().sum().
+000052d0: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
+000052e0: 6573 203d 2073 656c 662e 6164 6174 612e  es = self.adata.
+000052f0: 7661 725b 6f76 6572 6469 7370 6572 7369  var[overdispersi
+00005300: 6f6e 5f6d 6574 7269 635d 2e73 6f72 745f  on_metric].sort_
+00005310: 7661 6c75 6573 2861 7363 656e 6469 6e67  values(ascending
+00005320: 3d46 616c 7365 292e 6865 6164 2869 6e74  =False).head(int
+00005330: 2871 7561 6e74 696c 6520 2a20 6e5f 746f  (quantile * n_to
+00005340: 7461 6c5f 6765 6e65 7329 292e 696e 6465  tal_genes)).inde
+00005350: 780d 0a20 2020 2020 2020 2020 2020 2073  x..            s
+00005360: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
+00005370: 7365 6c65 6374 6564 5f67 656e 6573 2026  selected_genes &
+00005380: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
+00005390: 696e 6465 782e 6973 696e 2867 656e 6573  index.isin(genes
+000053a0: 290d 0a0d 0a20 2020 2020 2020 206e 5f73  )....        n_s
+000053b0: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
+000053c0: 7365 6c65 6374 6564 5f67 656e 6573 2e73  selected_genes.s
+000053d0: 756d 2829 0d0a 2020 2020 2020 2020 6c6f  um()..        lo
+000053e0: 6767 696e 672e 696e 666f 2866 227b 6e5f  gging.info(f"{n_
+000053f0: 7365 6c65 6374 6564 5f67 656e 6573 7d20  selected_genes} 
+00005400: 6765 6e65 7320 7365 6c65 6374 6564 2066  genes selected f
+00005410: 6f72 2066 6163 746f 7269 7a61 7469 6f6e  or factorization
+00005420: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
+00005430: 2020 2020 2020 2320 6d61 6b65 2063 6861        # make cha
+00005440: 6e67 6573 2074 6f20 4461 7461 7365 7420  nges to Dataset 
+00005450: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
+00005460: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+00005470: 7365 6c65 6374 6564 225d 203d 2073 656c  selected"] = sel
+00005480: 6563 7465 645f 6765 6e65 730d 0a20 2020  ected_genes..   
+00005490: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+000054a0: 756e 735b 226f 6467 225d 5b22 6f76 6572  uns["odg"]["over
+000054b0: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+000054c0: 6322 5d20 3d20 6f76 6572 6469 7370 6572  c"] = overdisper
+000054d0: 7369 6f6e 5f6d 6574 7269 630d 0a20 2020  sion_metric..   
+000054e0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+000054f0: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
+00005500: 6d65 616e 225d 203d 206d 696e 5f6d 6561  mean"] = min_mea
+00005510: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00005520: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00005530: 5b22 6d69 6e5f 7363 6f72 6522 5d20 3d20  ["min_score"] = 
+00005540: 6d69 6e5f 7363 6f72 6520 6966 206d 696e  min_score if min
+00005550: 5f73 636f 7265 2069 7320 6e6f 7420 4e6f  _score is not No
+00005560: 6e65 2065 6c73 6520 2222 0d0a 2020 2020  ne else ""..    
+00005570: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00005580: 6e73 5b22 6f64 6722 5d5b 2274 6f70 5f6e  ns["odg"]["top_n
+00005590: 225d 203d 2074 6f70 5f6e 2069 6620 746f  "] = top_n if to
+000055a0: 705f 6e20 6973 206e 6f74 204e 6f6e 6520  p_n is not None 
+000055b0: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
+000055c0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+000055d0: 226f 6467 225d 5b22 7175 616e 7469 6c65  "odg"]["quantile
+000055e0: 225d 203d 2071 7561 6e74 696c 6520 6966  "] = quantile if
+000055f0: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
+00005600: 204e 6f6e 6520 656c 7365 2022 220d 0a20   None else "".. 
+00005610: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+00005620: 6e64 5f74 6f5f 6869 7374 6f72 7928 224f  nd_to_history("O
+00005630: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
+00005640: 6573 2073 656c 6563 7465 6422 290d 0a20  es selected").. 
+00005650: 2020 200d 0a20 2020 2064 6566 2069 6e69     ..    def ini
+00005660: 7469 616c 697a 655f 636e 6d66 2873 656c  tialize_cnmf(sel
+00005670: 662c 2063 6e6d 665f 6f75 7470 7574 5f64  f, cnmf_output_d
+00005680: 6972 3a20 7374 722c 0d0a 2020 2020 2020  ir: str,..      
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 636e 6d66 5f6e 616d 653a 2073 7472    cnmf_name: str
+000056b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000056c0: 2020 2020 2020 2020 2020 206b 7661 6c73             kvals
+000056d0: 3a20 436f 6c6c 6563 7469 6f6e 203d 2072  : Collection = r
+000056e0: 616e 6765 2832 2c20 3631 292c 0d0a 2020  ange(2, 61),..  
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 6e5f 6974 6572 3a20 696e        n_iter: in
+00005710: 7420 3d20 3230 302c 0d0a 2020 2020 2020  t = 200,..      
+00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005730: 2020 6265 7461 5f6c 6f73 733a 2073 7472    beta_loss: str
+00005740: 203d 2022 6b75 6c6c 6261 636b 2d6c 6569   = "kullback-lei
+00005750: 626c 6572 222c 0d0a 2020 2020 2020 2020  bler",..        
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 7365 6564 3a20 4f70 7469 6f6e 616c 5b69  seed: Optional[i
+00005780: 6e74 5d20 3d20 4e6f 6e65 2920 2d3e 2063  nt] = None) -> c
+00005790: 6e6d 662e 634e 4d46 3a0d 0a20 2020 2020  nmf.cNMF:..     
+000057a0: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
+000057b0: 2061 2063 4e4d 4620 7275 6e20 666f 7220   a cNMF run for 
+000057c0: 7375 6273 6571 7565 6e74 2066 6163 746f  subsequent facto
+000057d0: 7269 7a61 7469 6f6e 2e0d 0a0d 0a20 2020  rization.....   
+000057e0: 2020 2020 203a 7061 7261 6d20 636e 6d66       :param cnmf
+000057f0: 5f6f 7574 7075 745f 6469 723a 204f 7574  _output_dir: Out
+00005800: 7075 7420 6469 7265 6374 6f72 7920 666f  put directory fo
+00005810: 7220 634e 4d46 2072 6573 756c 7473 0d0a  r cNMF results..
+00005820: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
+00005830: 6d66 5f6f 7574 7075 745f 6469 723a 2073  mf_output_dir: s
+00005840: 7472 0d0a 2020 2020 2020 2020 3a70 6172  tr..        :par
+00005850: 616d 2063 6e6d 665f 6e61 6d65 3a20 4e61  am cnmf_name: Na
+00005860: 6d65 206f 6620 7468 6520 634e 4d46 2072  me of the cNMF r
+00005870: 6573 756c 7473 2e20 4669 6c65 7320 7769  esults. Files wi
+00005880: 6c6c 2062 6520 6f75 7470 7574 2074 6f20  ll be output to 
+00005890: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
+000058a0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d2f 0d0a  ]/[cnmf_name]/..
+000058b0: 2020 2020 2020 2020 3a74 7970 6520 636e          :type cn
+000058c0: 6d66 5f6e 616d 653a 2073 7472 0d0a 2020  mf_name: str..  
+000058d0: 2020 2020 2020 3a70 6172 616d 206b 7661        :param kva
+000058e0: 6c73 3a20 5261 6e6b 7320 666f 7220 634e  ls: Ranks for cN
+000058f0: 4d46 2066 6163 746f 7269 7a61 7469 6f6e  MF factorization
+00005900: 2c20 6465 6661 756c 7473 2074 6f20 7261  , defaults to ra
+00005910: 6e67 6528 322c 2036 3129 0d0a 2020 2020  nge(2, 61)..    
+00005920: 2020 2020 3a74 7970 6520 6b76 616c 733a      :type kvals:
+00005930: 2043 6f6c 6c65 6374 696f 6e2c 206f 7074   Collection, opt
+00005940: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00005950: 7061 7261 6d20 6e5f 6974 6572 3a20 4e75  param n_iter: Nu
+00005960: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+00005970: 6e73 2066 726f 6d20 7768 6963 6820 746f  ns from which to
+00005980: 2062 7569 6c64 2061 2063 6f6e 7365 6e73   build a consens
+00005990: 7573 2073 6f6c 7574 696f 6e2c 2064 6566  us solution, def
+000059a0: 6175 6c74 7320 746f 2032 3030 0d0a 2020  aults to 200..  
+000059b0: 2020 2020 2020 3a74 7970 6520 6e5f 6974        :type n_it
+000059c0: 6572 3a20 696e 742c 206f 7074 696f 6e61  er: int, optiona
+000059d0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+000059e0: 6d20 6265 7461 5f6c 6f73 733a 2062 6574  m beta_loss: bet
+000059f0: 612d 6c6f 7373 2066 756e 6374 696f 6e2c  a-loss function,
+00005a00: 2065 6974 6865 7220 226b 756c 6c62 6163   either "kullbac
+00005a10: 6b2d 6c65 6962 6c65 7222 206f 7220 2266  k-leibler" or "f
+00005a20: 726f 6265 6e69 7573 222e 2044 6566 6175  robenius". Defau
+00005a30: 6c74 7320 746f 2022 6b75 6c6c 6261 636b  lts to "kullback
+00005a40: 2d6c 6569 626c 6572 220d 0a20 2020 2020  -leibler"..     
+00005a50: 2020 203a 7479 7065 2062 6574 615f 6c6f     :type beta_lo
+00005a60: 7373 3a20 7374 722c 206f 7074 696f 6e61  ss: str, optiona
+00005a70: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+00005a80: 6d20 7365 6564 3a20 5261 6e64 6f6d 2073  m seed: Random s
+00005a90: 6565 6420 666f 7220 7265 7072 6f64 7563  eed for reproduc
+00005aa0: 6962 696c 6974 792c 2064 6566 6175 6c74  ibility, default
+00005ab0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00005ac0: 2020 203a 7479 7065 2073 6565 643a 204f     :type seed: O
+00005ad0: 7074 696f 6e61 6c5b 696e 745d 2c20 6f70  ptional[int], op
+00005ae0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00005af0: 3a72 6574 7572 6e3a 2063 4e4d 4620 6f62  :return: cNMF ob
+00005b00: 6a65 6374 0d0a 2020 2020 2020 2020 3a72  ject..        :r
+00005b10: 7479 7065 3a20 3a63 6c61 7373 3a60 636e  type: :class:`cn
+00005b20: 6d66 736e 732e 636e 6d66 2e63 4e4d 4660  mfsns.cnmf.cNMF`
+00005b30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005b40: 2020 2020 2020 2063 6e6d 665f 6f62 6a20         cnmf_obj 
+00005b50: 3d20 636e 6d66 2e63 4e4d 4628 6f75 7470  = cnmf.cNMF(outp
+00005b60: 7574 5f64 6972 3d63 6e6d 665f 6f75 7470  ut_dir=cnmf_outp
+00005b70: 7574 5f64 6972 2c20 6e61 6d65 3d63 6e6d  ut_dir, name=cnm
+00005b80: 665f 6e61 6d65 290d 0a20 2020 2020 2020  f_name)..       
+00005b90: 200d 0a20 2020 2020 2020 2023 2077 7269   ..        # wri
+00005ba0: 7465 2054 504d 2028 6e6f 726d 616c 697a  te TPM (normaliz
+00005bb0: 6564 2920 6461 7461 0d0a 2020 2020 2020  ed) data..      
+00005bc0: 2020 7470 6d20 3d20 6164 2e41 6e6e 4461    tpm = ad.AnnDa
+00005bd0: 7461 2873 656c 662e 746f 5f64 6628 6e6f  ta(self.to_df(no
+00005be0: 726d 616c 697a 6564 3d54 7275 6529 290d  rmalized=True)).
+00005bf0: 0a20 2020 2020 2020 2074 706d 2e77 7269  .        tpm.wri
+00005c00: 7465 5f68 3561 6428 636e 6d66 5f6f 626a  te_h5ad(cnmf_obj
+00005c10: 2e70 6174 6873 5b22 7470 6d22 5d29 0d0a  .paths["tpm"])..
+00005c20: 0d0a 2020 2020 2020 2020 6765 6e65 5f74  ..        gene_t
+00005c30: 706d 5f6d 6561 6e20 3d20 6e70 2e61 7272  pm_mean = np.arr
+00005c40: 6179 2874 706d 2e58 2e6d 6561 6e28 6178  ay(tpm.X.mean(ax
+00005c50: 6973 3d30 2929 2e72 6573 6861 7065 282d  is=0)).reshape(-
+00005c60: 3129 0d0a 2020 2020 2020 2020 6765 6e65  1)..        gene
+00005c70: 5f74 706d 5f73 7464 6465 7620 3d20 6e70  _tpm_stddev = np
+00005c80: 2e61 7272 6179 2874 706d 2e58 2e73 7464  .array(tpm.X.std
+00005c90: 2861 7869 733d 302c 2064 646f 663d 3029  (axis=0, ddof=0)
+00005ca0: 292e 7265 7368 6170 6528 2d31 290d 0a20  ).reshape(-1).. 
+00005cb0: 2020 2020 2020 2069 6e70 7574 5f74 706d         input_tpm
+00005cc0: 5f73 7461 7473 203d 2070 642e 4461 7461  _stats = pd.Data
+00005cd0: 4672 616d 6528 5b67 656e 655f 7470 6d5f  Frame([gene_tpm_
+00005ce0: 6d65 616e 2c20 6765 6e65 5f74 706d 5f73  mean, gene_tpm_s
+00005cf0: 7464 6465 765d 2c20 696e 6465 7820 3d20  tddev], index = 
+00005d00: 5b27 5f5f 6d65 616e 272c 2027 5f5f 7374  ['__mean', '__st
+00005d10: 6427 5d29 2e54 0d0a 2020 2020 2020 2020  d']).T..        
+00005d20: 7574 696c 732e 7361 7665 5f64 665f 746f  utils.save_df_to
+00005d30: 5f6e 707a 2869 6e70 7574 5f74 706d 5f73  _npz(input_tpm_s
+00005d40: 7461 7473 2c20 636e 6d66 5f6f 626a 2e70  tats, cnmf_obj.p
+00005d50: 6174 6873 5b27 7470 6d5f 7374 6174 7327  aths['tpm_stats'
+00005d60: 5d29 0d0a 2020 2020 2020 2020 6f76 6572  ])..        over
+00005d70: 6469 7370 6572 7365 645f 6765 6e65 7320  dispersed_genes 
+00005d80: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+00005d90: 5b22 7365 6c65 6374 6564 225d 5b73 656c  ["selected"][sel
+00005da0: 662e 6164 6174 612e 7661 725b 2273 656c  f.adata.var["sel
+00005db0: 6563 7465 6422 5d5d 2e69 6e64 6578 0d0a  ected"]].index..
+00005dc0: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
+00005dd0: 6e74 7320 3d20 636e 6d66 5f6f 626a 2e67  nts = cnmf_obj.g
+00005de0: 6574 5f6e 6f72 6d5f 636f 756e 7473 2873  et_norm_counts(s
+00005df0: 656c 662e 6164 6174 612c 2074 706d 2c20  elf.adata, tpm, 
+00005e00: 6869 6768 5f76 6172 6961 6e63 655f 6765  high_variance_ge
+00005e10: 6e65 735f 6669 6c74 6572 3d6f 7665 7264  nes_filter=overd
+00005e20: 6973 7065 7273 6564 5f67 656e 6573 290d  ispersed_genes).
+00005e30: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
+00005e40: 5f63 6f75 6e74 732e 582e 6474 7970 6520  _counts.X.dtype 
+00005e50: 213d 206e 702e 666c 6f61 7436 343a 0d0a  != np.float64:..
+00005e60: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
+00005e70: 5f63 6f75 6e74 732e 5820 3d20 6e6f 726d  _counts.X = norm
+00005e80: 5f63 6f75 6e74 732e 582e 6173 7479 7065  _counts.X.astype
+00005e90: 286e 702e 666c 6f61 7436 3429 0d0a 2020  (np.float64)..  
+00005ea0: 2020 2020 2020 636e 6d66 5f6f 626a 2e73        cnmf_obj.s
+00005eb0: 6176 655f 6e6f 726d 5f63 6f75 6e74 7328  ave_norm_counts(
+00005ec0: 6e6f 726d 5f63 6f75 6e74 7329 0d0a 0d0a  norm_counts)....
+00005ed0: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
+00005ee0: 6172 616d 6574 6572 7320 666f 7220 6661  arameters for fa
+00005ef0: 6374 6f72 697a 6174 696f 6e20 7374 6570  ctorization step
+00005f00: 0d0a 2020 2020 2020 2020 636e 6d66 5f6f  ..        cnmf_o
+00005f10: 626a 2e73 6176 655f 6e6d 665f 6974 6572  bj.save_nmf_iter
+00005f20: 5f70 6172 616d 7328 2a63 6e6d 665f 6f62  _params(*cnmf_ob
+00005f30: 6a2e 6765 745f 6e6d 665f 6974 6572 5f70  j.get_nmf_iter_p
+00005f40: 6172 616d 7328 6b73 3d6b 7661 6c73 2c20  arams(ks=kvals, 
+00005f50: 6e5f 6974 6572 3d6e 5f69 7465 722c 2072  n_iter=n_iter, r
+00005f60: 616e 646f 6d5f 7374 6174 655f 7365 6564  andom_state_seed
+00005f70: 3d73 6565 642c 2062 6574 615f 6c6f 7373  =seed, beta_loss
+00005f80: 3d62 6574 615f 6c6f 7373 2929 0d0a 0d0a  =beta_loss))....
+00005f90: 2020 2020 2020 2020 2320 7361 7665 2070          # save p
+00005fa0: 6172 616d 6574 6572 7320 696e 2041 6e6e  arameters in Ann
+00005fb0: 4461 7461 206f 626a 6563 740d 0a20 2020  Data object..   
+00005fc0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00005fd0: 756e 735b 2263 6e6d 6622 5d20 3d20 636e  uns["cnmf"] = cn
+00005fe0: 6d66 5f6f 626a 2e67 6574 5f6e 6d66 5f69  mf_obj.get_nmf_i
+00005ff0: 7465 725f 7061 7261 6d73 286b 733d 6b76  ter_params(ks=kv
+00006000: 616c 732c 206e 5f69 7465 723d 6e5f 6974  als, n_iter=n_it
+00006010: 6572 2c20 7261 6e64 6f6d 5f73 7461 7465  er, random_state
+00006020: 5f73 6565 643d 7365 6564 2c20 6265 7461  _seed=seed, beta
+00006030: 5f6c 6f73 733d 6265 7461 5f6c 6f73 7329  _loss=beta_loss)
+00006040: 5b31 5d20 2023 2064 6963 7420 6f66 2063  [1]  # dict of c
+00006050: 6e6d 6620 7061 7261 6d65 7465 7273 0d0a  nmf parameters..
+00006060: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006070: 2020 7365 6c66 2e61 7070 656e 645f 746f    self.append_to
+00006080: 5f68 6973 746f 7279 2866 2263 4e4d 4620  _history(f"cNMF 
+00006090: 7061 7261 6d65 7465 7273 2061 6464 6564  parameters added
+000060a0: 2e20 634e 4d46 2069 6e70 7574 7320 696e  . cNMF inputs in
+000060b0: 6974 6961 6c69 7a65 6420 696e 207b 636e  itialized in {cn
+000060c0: 6d66 5f6f 7574 7075 745f 6469 727d 2f7b  mf_output_dir}/{
+000060d0: 636e 6d66 5f6e 616d 657d 2229 0d0a 2020  cnmf_name}")..  
+000060e0: 2020 2020 2020 7265 7475 726e 2063 6e6d        return cnm
+000060f0: 665f 6f62 6a0d 0a20 2020 200d 0a20 2020  f_obj..    ..   
+00006100: 2064 6566 2061 6464 5f63 6e6d 665f 7265   def add_cnmf_re
+00006110: 7375 6c74 7328 7365 6c66 2c20 636e 6d66  sults(self, cnmf
+00006120: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
+00006130: 665f 6e61 6d65 2c20 6c6f 6361 6c5f 6465  f_name, local_de
+00006140: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
+00006150: 2066 6c6f 6174 203d 204e 6f6e 652c 206c   float = None, l
+00006160: 6f63 616c 5f6e 6569 6768 626f 7268 6f6f  ocal_neighborhoo
+00006170: 645f 7369 7a65 3a20 666c 6f61 7420 3d20  d_size: float = 
+00006180: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00006190: 2222 220d 0a20 2020 2020 2020 2041 6674  """..        Aft
+000061a0: 6572 2066 6163 746f 7269 7a61 7469 6f6e  er factorization
+000061b0: 2c20 6164 6420 636f 6d70 6c65 7465 6420  , add completed 
+000061c0: 634e 4d46 2072 6573 756c 7473 2069 6e20  cNMF results in 
+000061d0: 5b63 6e6d 665f 6f75 7470 7574 5f64 6972  [cnmf_output_dir
+000061e0: 5d2f 5b63 6e6d 665f 6e61 6d65 5d20 746f  ]/[cnmf_name] to
+000061f0: 2074 6865 2064 6174 6173 6574 206f 626a   the dataset obj
+00006200: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
+00006210: 3a70 6172 616d 2063 6e6d 665f 6f75 7470  :param cnmf_outp
+00006220: 7574 5f64 6972 3a20 4f75 7470 7574 2064  ut_dir: Output d
+00006230: 6972 6563 746f 7279 2066 6f72 2063 4e4d  irectory for cNM
+00006240: 4620 7265 7375 6c74 730d 0a20 2020 2020  F results..     
+00006250: 2020 203a 7479 7065 2063 6e6d 665f 6f75     :type cnmf_ou
+00006260: 7470 7574 5f64 6972 3a20 7374 720d 0a20  tput_dir: str.. 
+00006270: 2020 2020 2020 203a 7061 7261 6d20 636e         :param cn
+00006280: 6d66 5f6e 616d 653a 204e 616d 6520 6f66  mf_name: Name of
+00006290: 2074 6865 2063 4e4d 4620 7265 7375 6c74   the cNMF result
+000062a0: 732e 2046 696c 6573 2077 696c 6c20 6265  s. Files will be
+000062b0: 206f 7574 7075 7420 746f 205b 636e 6d66   output to [cnmf
+000062c0: 5f6f 7574 7075 745f 6469 725d 2f5b 636e  _output_dir]/[cn
+000062d0: 6d66 5f6e 616d 655d 2f0d 0a20 2020 2020  mf_name]/..     
+000062e0: 2020 203a 7479 7065 2063 6e6d 665f 6e61     :type cnmf_na
+000062f0: 6d65 3a20 7374 720d 0a20 2020 2020 2020  me: str..       
+00006300: 203a 7061 7261 6d20 6c6f 6361 6c5f 6465   :param local_de
+00006310: 6e73 6974 795f 7468 7265 7368 6f6c 643a  nsity_threshold:
+00006320: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
+00006330: 6865 206c 6f63 616c 2064 656e 7369 7479  he local density
+00006340: 2066 696c 7465 7269 6e67 2070 7269 6f72   filtering prior
+00006350: 2074 6f20 4745 5020 636f 6e73 656e 7375   to GEP consensu
+00006360: 732e 2041 6363 6570 7461 626c 6520 7468  s. Acceptable th
+00006370: 7265 7368 6f6c 6473 2061 7265 203e 2030  resholds are > 0
+00006380: 2061 6e64 203c 3d20 3220 2832 2e30 2069   and <= 2 (2.0 i
+00006390: 7320 6e6f 2066 696c 7465 7269 6e67 292e  s no filtering).
+000063a0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+000063b0: 652e 0d0a 2020 2020 2020 2020 3a74 7970  e...        :typ
+000063c0: 6520 6c6f 6361 6c5f 6465 6e73 6974 795f  e local_density_
+000063d0: 7468 7265 7368 6f6c 643a 2066 6c6f 6174  threshold: float
+000063e0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000063f0: 2020 2020 3a70 6172 616d 206c 6f63 616c      :param local
+00006400: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
+00006410: 7a65 3a20 4672 6163 7469 6f6e 206f 6620  ze: Fraction of 
+00006420: 7468 6520 6e75 6d62 6572 206f 6620 7265  the number of re
+00006430: 706c 6963 6174 6573 2074 6f20 7573 6520  plicates to use 
+00006440: 6173 206e 6561 7265 7374 206e 6569 6768  as nearest neigh
+00006450: 626f 7273 2066 6f72 206c 6f63 616c 2064  bors for local d
+00006460: 656e 7369 7479 2066 696c 7465 7269 6e67  ensity filtering
+00006470: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00006480: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
+00006490: 6520 6c6f 6361 6c5f 6e65 6967 6862 6f72  e local_neighbor
+000064a0: 686f 6f64 5f73 697a 653a 2066 6c6f 6174  hood_size: float
+000064b0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000064c0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000064d0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+000064e0: 2263 6e6d 665f 6e61 6d65 225d 203d 2063  "cnmf_name"] = c
+000064f0: 6e6d 665f 6e61 6d65 0d0a 0d0a 2020 2020  nmf_name....    
+00006500: 2020 2020 2320 696e 6665 7220 6672 6f6d      # infer from
+00006510: 2066 696c 656e 616d 6573 2077 6869 6368   filenames which
+00006520: 206c 6f63 616c 2064 656e 7369 7479 2074   local density t
+00006530: 6872 6573 686f 6c64 2077 6173 2075 7365  hreshold was use
+00006540: 640d 0a20 2020 2020 2020 2073 656e 7365  d..        sense
+00006550: 645f 6c64 7473 203d 2073 6574 2829 0d0a  d_ldts = set()..
+00006560: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
+00006570: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
+00006580: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
+00006590: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
+000065a0: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e2a  f"{cnmf_name}*.*
+000065b0: 7370 6563 7472 612a 2e6b 5f2a 2229 293a  spectra*.k_*")):
+000065c0: 0d0a 2020 2020 2020 2020 2020 2020 6c64  ..            ld
+000065d0: 745f 7374 7220 3d20 6f73 2e70 6174 682e  t_str = os.path.
+000065e0: 6261 7365 6e61 6d65 2866 6e29 2e73 706c  basename(fn).spl
+000065f0: 6974 2822 2e22 295b 2d33 5d0d 0a20 2020  it(".")[-3]..   
+00006600: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00006610: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00006620: 6474 203d 2066 6c6f 6174 286c 6474 5f73  dt = float(ldt_s
+00006630: 7472 2e72 6570 6c61 6365 2822 6474 5f22  tr.replace("dt_"
+00006640: 2c20 2222 292e 7265 706c 6163 6528 225f  , "").replace("_
+00006650: 222c 2022 2e22 2929 0d0a 2020 2020 2020  ", "."))..      
+00006660: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00006670: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
+00006680: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00006690: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000066a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000066b0: 2020 2073 656e 7365 645f 6c64 7473 2e61     sensed_ldts.a
+000066c0: 6464 2828 6c64 745f 7374 722c 206c 6474  dd((ldt_str, ldt
+000066d0: 2929 0d0a 2020 2020 2020 2020 6966 206c  ))..        if l
+000066e0: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
+000066f0: 6573 686f 6c64 2069 7320 4e6f 6e65 2061  eshold is None a
+00006700: 6e64 206c 656e 2873 656e 7365 645f 6c64  nd len(sensed_ld
+00006710: 7473 2920 3d3d 2031 3a0d 0a20 2020 2020  ts) == 1:..     
+00006720: 2020 2020 2020 206c 6474 5f73 7472 2c20         ldt_str, 
+00006730: 6c64 7420 3d20 7365 6e73 6564 5f6c 6474  ldt = sensed_ldt
+00006740: 732e 706f 7028 290d 0a20 2020 2020 2020  s.pop()..       
+00006750: 2065 6c69 6620 6c6f 6361 6c5f 6465 6e73   elif local_dens
+00006760: 6974 795f 7468 7265 7368 6f6c 6420 696e  ity_threshold in
+00006770: 2028 6c64 745b 315d 2066 6f72 206c 6474   (ldt[1] for ldt
+00006780: 2069 6e20 7365 6e73 6564 5f6c 6474 7329   in sensed_ldts)
+00006790: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+000067a0: 6474 5f73 7472 2c20 6c64 7420 3d20 5b28  dt_str, ldt = [(
+000067b0: 6c64 745f 7374 722c 206c 6474 2920 666f  ldt_str, ldt) fo
+000067c0: 7220 6c64 745f 7374 722c 206c 6474 2069  r ldt_str, ldt i
+000067d0: 6e20 7365 6e73 6564 5f6c 6474 7320 6966  n sensed_ldts if
+000067e0: 206c 6474 203d 3d20 6c6f 6361 6c5f 6465   ldt == local_de
+000067f0: 6e73 6974 795f 7468 7265 7368 6f6c 645d  nsity_threshold]
+00006800: 2e70 6f70 2829 0d0a 2020 2020 2020 2020  .pop()..        
+00006810: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00006820: 2020 206c 6f67 6769 6e67 2e65 7272 6f72     logging.error
+00006830: 2866 226c 6f63 616c 5f64 656e 7369 7479  (f"local_density
+00006840: 5f74 6872 6573 686f 6c64 206f 6620 7b6c  _threshold of {l
+00006850: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
+00006860: 6573 686f 6c64 7d20 646f 6573 206e 6f74  eshold} does not
+00006870: 206d 6174 6368 2077 6861 7420 6973 2069   match what is i
+00006880: 6e20 7468 6520 634e 4d46 2072 6573 756c  n the cNMF resul
+00006890: 7420 6469 7265 6374 6f72 793a 207b 7365  t directory: {se
+000068a0: 6e73 6564 5f6c 6474 737d 2229 0d0a 2020  nsed_ldts}")..  
+000068b0: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
+000068c0: 6974 2831 290d 0a20 2020 2020 2020 2073  it(1)..        s
+000068d0: 656c 662e 6164 6174 612e 756e 735b 226c  elf.adata.uns["l
+000068e0: 6474 225d 203d 206c 6474 0d0a 2020 2020  dt"] = ldt..    
+000068f0: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00006900: 6e73 5b22 6c6e 7322 5d20 3d20 6c6f 6361  ns["lns"] = loca
+00006910: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
+00006920: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
+00006930: 200d 0a20 2020 2020 2020 2023 2049 6d70   ..        # Imp
+00006940: 6f72 7420 4745 5073 0d0a 2020 2020 2020  ort GEPs..      
+00006950: 2020 7265 7375 6c74 5f74 7970 6573 203d    result_types =
+00006960: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00006970: 2267 656e 655f 7370 6563 7472 615f 7363  "gene_spectra_sc
+00006980: 6f72 6522 3a20 2263 6e6d 665f 6765 705f  ore": "cnmf_gep_
+00006990: 7363 6f72 6522 2c0d 0a20 2020 2020 2020  score",..       
+000069a0: 2020 2020 2022 6765 6e65 5f73 7065 6374       "gene_spect
+000069b0: 7261 5f74 706d 223a 2022 636e 6d66 5f67  ra_tpm": "cnmf_g
+000069c0: 6570 5f74 706d 222c 0d0a 2020 2020 2020  ep_tpm",..      
+000069d0: 2020 2020 2020 2273 7065 6374 7261 223a        "spectra":
+000069e0: 2022 636e 6d66 5f67 6570 5f72 6177 220d   "cnmf_gep_raw".
+000069f0: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
+00006a00: 2020 2020 2020 2020 666f 7220 6d61 7463          for matc
+00006a10: 6873 7472 2c20 7265 7375 6c74 5f74 7970  hstr, result_typ
+00006a20: 6520 696e 2072 6573 756c 745f 7479 7065  e in result_type
+00006a30: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00006a40: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00006a50: 696e 666f 2866 2249 6d70 6f72 7469 6e67  info(f"Importing
+00006a60: 2047 4550 733a 207b 6d61 7463 6873 7472   GEPs: {matchstr
+00006a70: 7d22 2920 200d 0a20 2020 2020 2020 2020  }")  ..         
+00006a80: 2020 206d 6574 615f 7720 3d20 5b5d 0d0a     meta_w = []..
+00006a90: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00006aa0: 666e 2069 6e20 676c 6f62 286f 732e 7061  fn in glob(os.pa
+00006ab0: 7468 2e6a 6f69 6e28 636e 6d66 5f6f 7574  th.join(cnmf_out
+00006ac0: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
+00006ad0: 6d65 2c20 6622 7b63 6e6d 665f 6e61 6d65  me, f"{cnmf_name
+00006ae0: 7d2a 2e7b 6d61 7463 6873 7472 7d2e 6b5f  }*.{matchstr}.k_
+00006af0: 2a2e 7b6c 6474 5f73 7472 7d2e 2a74 7874  *.{ldt_str}.*txt
+00006b00: 2229 293a 0d0a 2020 2020 2020 2020 2020  ")):..          
+00006b10: 2020 2020 2020 6b20 3d20 696e 7428 6f73        k = int(os
+00006b20: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
+00006b30: 6e29 2e72 656d 6f76 6570 7265 6669 7828  n).removeprefix(
+00006b40: 6622 7b63 6e6d 665f 6e61 6d65 7d2e 7b6d  f"{cnmf_name}.{m
+00006b50: 6174 6368 7374 727d 2e22 292e 7370 6c69  atchstr}.").spli
+00006b60: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
+00006b70: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
+00006b80: 2020 2020 2020 2020 2020 2020 2020 7720                w 
+00006b90: 3d20 7064 2e72 6561 645f 7461 626c 6528  = pd.read_table(
+00006ba0: 666e 2c20 696e 6465 785f 636f 6c3d 3029  fn, index_col=0)
+00006bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006bc0: 2020 772e 696e 6465 7820 3d20 7374 7228    w.index = str(
+00006bd0: 6b29 202b 2022 2e22 202b 2077 2e69 6e64  k) + "." + w.ind
+00006be0: 6578 2e61 7374 7970 6528 7374 7229 0d0a  ex.astype(str)..
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c00: 6d65 7461 5f77 2e61 7070 656e 6428 7729  meta_w.append(w)
+00006c10: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+00006c20: 7461 5f77 203d 2070 642e 636f 6e63 6174  ta_w = pd.concat
+00006c30: 286d 6574 615f 772c 2061 7869 733d 3029  (meta_w, axis=0)
+00006c40: 2e54 2e72 6569 6e64 6578 2873 656c 662e  .T.reindex(self.
+00006c50: 6164 6174 612e 7661 722e 696e 6465 7829  adata.var.index)
+00006c60: 2e72 656e 616d 655f 6178 6973 285b 226b  .rename_axis(["k
+00006c70: 2e67 6570 225d 2c20 6178 6973 3d31 290d  .gep"], axis=1).
+00006c80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006c90: 662e 6164 6174 612e 7661 726d 5b72 6573  f.adata.varm[res
+00006ca0: 756c 745f 7479 7065 5d20 3d20 6d65 7461  ult_type] = meta
+00006cb0: 5f77 0d0a 0d0a 2020 2020 2020 2020 2320  _w....        # 
+00006cc0: 496d 706f 7274 2055 7361 6765 730d 0a20  Import Usages.. 
+00006cd0: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
+00006ce0: 6e66 6f28 6622 496d 706f 7274 696e 6720  nfo(f"Importing 
+00006cf0: 5573 6167 6573 2229 2020 0d0a 2020 2020  Usages")  ..    
+00006d00: 2020 2020 7573 6167 6520 3d20 5b5d 0d0a      usage = []..
+00006d10: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
+00006d20: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
+00006d30: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
+00006d40: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
+00006d50: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e75  f"{cnmf_name}*.u
+00006d60: 7361 6765 732e 6b5f 2a2e 7b6c 6474 5f73  sages.k_*.{ldt_s
+00006d70: 7472 7d2e 2a74 7874 2229 293a 0d0a 2020  tr}.*txt")):..  
+00006d80: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+00006d90: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+00006da0: 6d65 2866 6e29 2e72 656d 6f76 6570 7265  me(fn).removepre
+00006db0: 6669 7828 6622 7b63 6e6d 665f 6e61 6d65  fix(f"{cnmf_name
+00006dc0: 7d2e 7573 6167 6573 2e22 292e 7370 6c69  }.usages.").spli
+00006dd0: 7428 222e 2229 5b30 5d2e 7265 706c 6163  t(".")[0].replac
+00006de0: 6528 226b 5f22 2c20 2222 2929 0d0a 2020  e("k_", ""))..  
+00006df0: 2020 2020 2020 2020 2020 6820 3d20 7064            h = pd
+00006e00: 2e72 6561 645f 7461 626c 6528 666e 2c20  .read_table(fn, 
+00006e10: 696e 6465 785f 636f 6c3d 3029 0d0a 2020  index_col=0)..  
+00006e20: 2020 2020 2020 2020 2020 682e 636f 6c75            h.colu
+00006e30: 6d6e 7320 3d20 7374 7228 6b29 202b 2022  mns = str(k) + "
+00006e40: 2e22 202b 2068 2e63 6f6c 756d 6e73 2e61  ." + h.columns.a
+00006e50: 7374 7970 6528 7374 7229 0d0a 2020 2020  stype(str)..    
+00006e60: 2020 2020 2020 2020 7573 6167 652e 6170          usage.ap
+00006e70: 7065 6e64 2868 290d 0a20 2020 2020 2020  pend(h)..       
+00006e80: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
+00006e90: 5b22 636e 6d66 5f75 7361 6765 225d 203d  ["cnmf_usage"] =
+00006ea0: 2070 642e 636f 6e63 6174 2875 7361 6765   pd.concat(usage
+00006eb0: 2c20 6178 6973 3d31 292e 736f 7274 5f69  , axis=1).sort_i
+00006ec0: 6e64 6578 2861 7869 733d 3129 2e72 656e  ndex(axis=1).ren
+00006ed0: 616d 655f 6178 6973 285b 226b 2e67 6570  ame_axis(["k.gep
+00006ee0: 225d 2c20 6178 6973 3d31 290d 0a20 2020  "], axis=1)..   
+00006ef0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+00006f00: 2049 6d70 6f72 7420 6765 6e65 206c 6973   Import gene lis
+00006f10: 7420 7573 6564 2066 6f72 2066 6163 746f  t used for facto
+00006f20: 7269 7a61 7469 6f6e 0d0a 2020 2020 2020  rization..      
+00006f30: 2020 7769 7468 206f 7065 6e28 6f73 2e70    with open(os.p
+00006f40: 6174 682e 6a6f 696e 2863 6e6d 665f 6f75  ath.join(cnmf_ou
+00006f50: 7470 7574 5f64 6972 2c20 636e 6d66 5f6e  tput_dir, cnmf_n
+00006f60: 616d 652c 2066 227b 636e 6d66 5f6e 616d  ame, f"{cnmf_nam
+00006f70: 657d 2e6f 7665 7264 6973 7065 7273 6564  e}.overdispersed
+00006f80: 5f67 656e 6573 2e74 7874 2229 2920 6173  _genes.txt")) as
+00006f90: 2066 3a0d 0a20 2020 2020 2020 2020 2020   f:..           
+00006fa0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00006fb0: 2267 656e 655f 6c69 7374 225d 203d 205b  "gene_list"] = [
+00006fc0: 6c69 6e65 2e73 7472 6970 2829 2066 6f72  line.strip() for
+00006fd0: 206c 696e 6520 696e 2066 2e72 6561 646c   line in f.readl
+00006fe0: 696e 6573 2829 5d0d 0a0d 0a20 2020 2020  ines()]....     
+00006ff0: 2020 2023 2049 6d70 6f72 7420 4b2d 7365     # Import K-se
+00007000: 6c65 6374 696f 6e20 7374 6174 730d 0a20  lection stats.. 
+00007010: 2020 2020 2020 206b 7661 6c73 203d 2070         kvals = p
+00007020: 642e 4461 7461 4672 616d 6528 2a2a 6e70  d.DataFrame(**np
+00007030: 2e6c 6f61 6428 6f73 2e70 6174 682e 6a6f  .load(os.path.jo
+00007040: 696e 2863 6e6d 665f 6f75 7470 7574 5f64  in(cnmf_output_d
+00007050: 6972 2c20 636e 6d66 5f6e 616d 652c 2066  ir, cnmf_name, f
+00007060: 227b 636e 6d66 5f6e 616d 657d 2e6b 5f73  "{cnmf_name}.k_s
+00007070: 656c 6563 7469 6f6e 5f73 7461 7473 2e64  election_stats.d
+00007080: 662e 6e70 7a22 292c 2061 6c6c 6f77 5f70  f.npz"), allow_p
+00007090: 6963 6b6c 653d 5472 7565 2929 2e73 6574  ickle=True)).set
+000070a0: 5f69 6e64 6578 2822 6b22 295b 5b22 7374  _index("k")[["st
+000070b0: 6162 696c 6974 7922 2c20 2270 7265 6469  ability", "predi
+000070c0: 6374 696f 6e5f 6572 726f 7222 5d5d 0d0a  ction_error"]]..
+000070d0: 2020 2020 2020 2020 6b76 616c 732e 696e          kvals.in
+000070e0: 6465 7820 3d20 6b76 616c 732e 696e 6465  dex = kvals.inde
+000070f0: 782e 6173 7479 7065 2869 6e74 290d 0a20  x.astype(int).. 
+00007100: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00007110: 612e 756e 735b 226b 7661 6c73 225d 203d  a.uns["kvals"] =
+00007120: 206b 7661 6c73 0d0a 2020 2020 2020 2020   kvals..        
+00007130: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
+00007140: 6973 746f 7279 2822 634e 4d46 2072 6573  istory("cNMF res
+00007150: 756c 7473 2061 6464 6564 2066 726f 6d20  ults added from 
+00007160: 6f75 7470 7574 2064 6972 6563 746f 7279  output directory
+00007170: 207b 636e 6d66 5f6f 7574 7075 745f 6469   {cnmf_output_di
+00007180: 727d 2f7b 636e 6d66 5f6e 616d 657d 2229  r}/{cnmf_name}")
+00007190: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+000071a0: 7573 6167 6573 2873 656c 662c 0d0a 2020  usages(self,..  
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 206b 3a20 556e 696f 6e5b 696e 742c 2049   k: Union[int, I
+000071d0: 7465 7261 626c 655d 203d 204e 6f6e 652c  terable] = None,
+000071e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000071f0: 2020 2020 2064 6973 6372 6574 697a 653a       discretize:
+00007200: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007220: 2020 206e 6f72 6d61 6c69 7a65 3a20 626f     normalize: bo
+00007230: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
+00007240: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007250: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00007260: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00007270: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+00007280: 6520 7573 6167 6520 6f66 2065 6163 6820  e usage of each 
+00007290: 4745 5020 696e 2065 6163 6820 7361 6d70  GEP in each samp
+000072a0: 6c65 2f6f 6273 6572 7661 7469 6f6e 2e0d  le/observation..
+000072b0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+000072c0: 6d20 6b3a 2049 6620 616e 2069 6e74 6567  m k: If an integ
+000072d0: 6572 206f 7220 6c69 7374 206f 6620 696e  er or list of in
+000072e0: 7465 6765 7273 2c20 7265 7475 726e 7320  tegers, returns 
+000072f0: 7573 6167 6573 206f 6e6c 7920 666f 7220  usages only for 
+00007300: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
+00007310: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
+00007320: 726e 7320 7573 6167 6520 6f66 2061 6c6c  rns usage of all
+00007330: 2047 4550 7320 6163 726f 7373 2072 616e   GEPs across ran
+00007340: 6b73 2e20 4465 6661 756c 7473 2074 6f20  ks. Defaults to 
+00007350: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
+00007360: 7970 6520 6b3a 2069 6e74 2c20 6f70 7469  ype k: int, opti
+00007370: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00007380: 6172 616d 2064 6973 6372 6574 697a 653a  aram discretize:
+00007390: 2044 6973 6372 6574 697a 6573 2074 6865   Discretizes the
+000073a0: 2075 7361 6765 206d 6174 7269 7820 7375   usage matrix su
+000073b0: 6368 2074 6861 7420 666f 7220 6561 6368  ch that for each
+000073c0: 2076 616c 7565 206f 6620 6b2c 2065 6163   value of k, eac
+000073d0: 6820 7361 6d70 6c65 2068 6173 2075 7361  h sample has usa
+000073e0: 6765 206f 6620 6f6e 6c79 2031 2047 4550  ge of only 1 GEP
+000073f0: 2028 7468 6520 6f6e 6520 7769 7468 2074   (the one with t
+00007400: 6865 206d 6178 696d 756d 2075 7361 6765  he maximum usage
+00007410: 292e 2044 6566 6175 6c74 7320 746f 2046  ). Defaults to F
+00007420: 616c 7365 0d0a 2020 2020 2020 2020 3a74  alse..        :t
+00007430: 7970 6520 6469 7363 7265 7469 7a65 3a20  ype discretize: 
+00007440: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
+00007450: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
+00007460: 6f72 6d61 6c69 7a65 3a20 4e6f 726d 616c  ormalize: Normal
+00007470: 697a 6520 7468 6520 4745 5020 7573 6167  ize the GEP usag
+00007480: 6520 6d61 7472 6978 2073 7563 6820 7468  e matrix such th
+00007490: 6174 2066 6f72 2065 6163 6820 7661 6c75  at for each valu
+000074a0: 6520 6f66 206b 2c20 7573 6167 6520 6f66  e of k, usage of
+000074b0: 2061 6c6c 2047 4550 7320 7375 6d73 2074   all GEPs sums t
+000074c0: 6f20 312e 2044 6566 6175 6c74 7320 746f  o 1. Defaults to
+000074d0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000074e0: 3a74 7970 6520 6e6f 726d 616c 697a 653a  :type normalize:
+000074f0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00007500: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00007510: 3a20 6f62 7365 7276 6174 696f 6e20 c397  : observation ..
+00007520: 2047 4550 206d 6174 7269 780d 0a20 2020   GEP matrix..   
+00007530: 2020 2020 203a 7274 7970 653a 2070 642e       :rtype: pd.
+00007540: 4461 7461 4672 616d 650d 0a20 2020 2020  DataFrame..     
+00007550: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00007560: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
+00007570: 6f62 736d 5b22 636e 6d66 5f75 7361 6765  obsm["cnmf_usage
+00007580: 225d 2e63 6f70 7928 290d 0a20 2020 2020  "].copy()..     
+00007590: 2020 2064 662e 636f 6c75 6d6e 7320 3d20     df.columns = 
+000075a0: 7064 2e4d 756c 7469 496e 6465 782e 6672  pd.MultiIndex.fr
+000075b0: 6f6d 5f74 7570 6c65 7328 6466 2e63 6f6c  om_tuples(df.col
+000075c0: 756d 6e73 2e73 7472 2e73 706c 6974 2822  umns.str.split("
+000075d0: 2e22 292e 746f 5f6c 6973 7428 2929 0d0a  .").to_list())..
+000075e0: 2020 2020 2020 2020 6466 2e63 6f6c 756d          df.colum
+000075f0: 6e73 203d 2064 662e 636f 6c75 6d6e 732e  ns = df.columns.
+00007600: 7365 745f 6c65 7665 6c73 285b 6c2e 6173  set_levels([l.as
+00007610: 7479 7065 2822 696e 7422 2920 666f 7220  type("int") for 
+00007620: 6c20 696e 2064 662e 636f 6c75 6d6e 732e  l in df.columns.
+00007630: 6c65 7665 6c73 5d29 0d0a 2020 2020 2020  levels])..      
+00007640: 2020 6966 206e 6f72 6d61 6c69 7a65 3a0d    if normalize:.
+00007650: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
+00007660: 6d61 6c69 7a65 6420 3d20 5b5d 0d0a 2020  malized = []..  
+00007670: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
+00007680: 2073 7562 6466 2069 6e20 6466 2e67 726f   subdf in df.gro
+00007690: 7570 6279 2861 7869 733d 312c 206c 6576  upby(axis=1, lev
+000076a0: 656c 3d30 293a 0d0a 2020 2020 2020 2020  el=0):..        
+000076b0: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
+000076c0: 6564 2e61 7070 656e 6428 7375 6264 662e  ed.append(subdf.
+000076d0: 6469 7628 7375 6264 662e 7375 6d28 6178  div(subdf.sum(ax
+000076e0: 6973 3d31 292c 2061 7869 733d 3029 290d  is=1), axis=0)).
+000076f0: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+00007700: 3d20 7064 2e63 6f6e 6361 7428 6e6f 726d  = pd.concat(norm
+00007710: 616c 697a 6564 2c20 6178 6973 3d31 290d  alized, axis=1).
+00007720: 0a20 2020 2020 2020 2069 6620 6469 7363  .        if disc
+00007730: 7265 7469 7a65 3a0d 0a20 2020 2020 2020  retize:..       
+00007740: 2020 2020 2064 6973 6372 6574 697a 6564       discretized
+00007750: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00007760: 2020 2066 6f72 205f 2c20 7375 6264 6620     for _, subdf 
+00007770: 696e 2064 662e 6772 6f75 7062 7928 6178  in df.groupby(ax
+00007780: 6973 3d31 2c20 6c65 7665 6c3d 3029 3a0d  is=1, level=0):.
+00007790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077a0: 2064 6973 6372 6574 697a 6564 2e61 7070   discretized.app
+000077b0: 656e 6428 7375 6264 662e 6571 2873 7562  end(subdf.eq(sub
+000077c0: 6466 2e6d 6178 2861 7869 733d 3129 2c20  df.max(axis=1), 
+000077d0: 6178 6973 3d30 292e 6173 7479 7065 2869  axis=0).astype(i
+000077e0: 6e74 2929 0d0a 2020 2020 2020 2020 2020  nt))..          
+000077f0: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
+00007800: 2864 6973 6372 6574 697a 6564 2c20 6178  (discretized, ax
+00007810: 6973 3d31 2920 2020 2020 2020 200d 0a20  is=1)        .. 
+00007820: 2020 2020 2020 2069 6620 6b20 6973 206e         if k is n
+00007830: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00007840: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
+00007850: 635b 3a2c 206b 5d0d 0a20 2020 2020 2020  c[:, k]..       
+00007860: 2064 6620 3d20 6466 2e73 6f72 745f 696e   df = df.sort_in
+00007870: 6465 7828 6178 6973 3d30 292e 736f 7274  dex(axis=0).sort
+00007880: 5f69 6e64 6578 2861 7869 733d 3129 2020  _index(axis=1)  
+00007890: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+000078a0: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+000078b0: 6465 6620 6765 745f 6765 7073 2873 656c  def get_geps(sel
+000078c0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+000078d0: 2020 2020 206b 3a20 556e 696f 6e5b 696e       k: Union[in
+000078e0: 742c 2049 7465 7261 626c 655d 203d 204e  t, Iterable] = N
+000078f0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00007900: 2020 2020 2020 2074 7970 653d 2263 6e6d         type="cnm
+00007910: 665f 6765 705f 7363 6f72 6522 0d0a 2020  f_gep_score"..  
+00007920: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007930: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00007940: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00007950: 2020 2020 2020 2020 4765 7420 4745 5073          Get GEPs
+00007960: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
+00007970: 7261 6d20 6b3a 2049 6620 616e 2069 6e74  ram k: If an int
+00007980: 6567 6572 206f 7220 6c69 7374 206f 6620  eger or list of 
+00007990: 696e 7465 6765 7273 2c20 7265 7475 726e  integers, return
+000079a0: 7320 4745 5073 206f 6e6c 7920 666f 7220  s GEPs only for 
+000079b0: 7370 6563 6966 6965 6420 7261 6e6b 732e  specified ranks.
+000079c0: 204f 7468 6572 7769 7365 2c20 7265 7475   Otherwise, retu
+000079d0: 726e 7320 4745 5073 2066 726f 6d20 616c  rns GEPs from al
+000079e0: 6c20 7261 6e6b 732e 2044 6566 6175 6c74  l ranks. Default
+000079f0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00007a00: 2020 203a 7479 7065 206b 3a20 556e 696f     :type k: Unio
+00007a10: 6e5b 696e 742c 2049 7465 7261 626c 655d  n[int, Iterable]
+00007a20: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00007a30: 2020 2020 3a70 6172 616d 2074 7970 653a      :param type:
+00007a40: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
+00007a50: 2220 6f72 2022 636e 6d66 5f67 6570 5f74  " or "cnmf_gep_t
+00007a60: 706d 222c 2064 6566 6175 6c74 7320 746f  pm", defaults to
+00007a70: 2022 636e 6d66 5f67 6570 5f73 636f 7265   "cnmf_gep_score
+00007a80: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
+00007a90: 2074 7970 653a 2073 7472 2c20 6f70 7469   type: str, opti
+00007aa0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
+00007ab0: 6574 7572 6e3a 2066 6561 7475 7265 7320  eturn: features 
+00007ac0: c397 2047 4550 206d 6174 7269 780d 0a20  .. GEP matrix.. 
+00007ad0: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
+00007ae0: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
+00007af0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00007b00: 2020 6466 203d 2073 656c 662e 6164 6174    df = self.adat
+00007b10: 612e 7661 726d 5b74 7970 655d 2e63 6f70  a.varm[type].cop
+00007b20: 7928 290d 0a20 2020 2020 2020 2064 662e  y()..        df.
+00007b30: 636f 6c75 6d6e 7320 3d20 7064 2e4d 756c  columns = pd.Mul
+00007b40: 7469 496e 6465 782e 6672 6f6d 5f74 7570  tiIndex.from_tup
+00007b50: 6c65 7328 6466 2e63 6f6c 756d 6e73 2e73  les(df.columns.s
+00007b60: 7472 2e73 706c 6974 2822 2e22 292e 746f  tr.split(".").to
+00007b70: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
+00007b80: 2020 6466 2e63 6f6c 756d 6e73 203d 2064    df.columns = d
+00007b90: 662e 636f 6c75 6d6e 732e 7365 745f 6c65  f.columns.set_le
+00007ba0: 7665 6c73 285b 6c2e 6173 7479 7065 2822  vels([l.astype("
+00007bb0: 696e 7422 2920 666f 7220 6c20 696e 2064  int") for l in d
+00007bc0: 662e 636f 6c75 6d6e 732e 6c65 7665 6c73  f.columns.levels
+00007bd0: 5d29 0d0a 2020 2020 2020 2020 6966 2069  ])..        if i
+00007be0: 7369 6e73 7461 6e63 6528 6b2c 2028 696e  sinstance(k, (in
+00007bf0: 742c 2049 7465 7261 626c 6529 293a 0d0a  t, Iterable)):..
+00007c00: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+00007c10: 2064 662e 6c6f 635b 3a2c 206b 5d0d 0a20   df.loc[:, k].. 
+00007c20: 2020 2020 2020 2064 6620 3d20 6466 2e73         df = df.s
+00007c30: 6f72 745f 696e 6465 7828 6178 6973 3d31  ort_index(axis=1
+00007c40: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00007c50: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+00007c60: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
+00007c70: 5f64 6628 7365 6c66 2c0d 0a20 2020 2020  _df(self,..     
+00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c90: 2020 2069 6e63 6c75 6465 5f63 6174 6567     include_categ
+00007ca0: 6f72 6963 616c 3a20 626f 6f6c 203d 2054  orical: bool = T
+00007cb0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00007cd0: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
+00007ce0: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2020 2020 2020 2920 2d3e 2070 642e 4461        ) -> pd.Da
+00007d10: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
+00007d20: 2020 2222 2247 6574 2073 616d 706c 652f    """Get sample/
+00007d30: 6f62 7365 7276 6174 696f 6e20 6d65 7461  observation meta
+00007d40: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
+00007d50: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
+00007d60: 6361 7465 676f 7269 6361 6c3a 2049 6e63  categorical: Inc
+00007d70: 6c75 6465 2063 6174 6567 6f72 6963 616c  lude categorical
+00007d80: 206d 6574 6164 6174 6120 6c61 7965 7273   metadata layers
+00007d90: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
+00007da0: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
+00007db0: 6520 696e 636c 7564 655f 6361 7465 676f  e include_catego
+00007dc0: 7269 6361 6c3a 2062 6f6f 6c2c 206f 7074  rical: bool, opt
+00007dd0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00007de0: 7061 7261 6d20 696e 636c 7564 655f 6e75  param include_nu
+00007df0: 6d65 7269 6361 6c3a 2049 6e63 6c75 6465  merical: Include
+00007e00: 206e 756d 6572 6963 616c 206d 6574 6164   numerical metad
+00007e10: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
+00007e20: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
+00007e30: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
+00007e40: 7564 655f 6e75 6d65 7269 6361 6c3a 2062  ude_numerical: b
+00007e50: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+00007e60: 2020 2020 2020 203a 7261 6973 6573 2056         :raises V
+00007e70: 616c 7565 4572 726f 723a 2045 7272 6f72  alueError: Error
+00007e80: 2069 6620 6d65 7461 6461 7461 2074 7970   if metadata typ
+00007e90: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
+00007ea0: 6e69 7a65 640d 0a20 2020 2020 2020 203a  nized..        :
+00007eb0: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
+00007ec0: 696f 6e73 20c3 9720 6d65 7461 6461 7461  ions .. metadata
+00007ed0: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
+00007ee0: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
+00007ef0: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
+00007f00: 2222 0d0a 2020 2020 2020 2020 6474 7970  ""..        dtyp
+00007f10: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00007f20: 2069 6620 696e 636c 7564 655f 6361 7465   if include_cate
+00007f30: 676f 7269 6361 6c3a 0d0a 2020 2020 2020  gorical:..      
+00007f40: 2020 2020 2020 6474 7970 6573 2e61 7070        dtypes.app
+00007f50: 656e 6428 2263 6174 6567 6f72 7922 290d  end("category").
+00007f60: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
+00007f70: 7564 655f 6e75 6d65 7269 6361 6c3a 0d0a  ude_numerical:..
+00007f80: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
+00007f90: 6573 202b 3d20 5b22 666c 6f61 7422 2c20  es += ["float", 
+00007fa0: 2269 6e74 225d 0d0a 2020 2020 2020 2020  "int"]..        
+00007fb0: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
+00007fc0: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
+00007fd0: 732e 7365 6c65 6374 5f64 7479 7065 7328  s.select_dtypes(
+00007fe0: 6578 636c 7564 653d 2822 6361 7465 676f  exclude=("catego
+00007ff0: 7279 222c 2022 666c 6f61 7422 2c20 2269  ry", "float", "i
+00008000: 6e74 2229 292e 636f 6c75 6d6e 730d 0a20  nt")).columns.. 
+00008010: 2020 2020 2020 2069 6620 6c65 6e28 756e         if len(un
+00008020: 6578 706c 6169 6e65 645f 636f 6c73 2920  explained_cols) 
+00008030: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+00008040: 2020 756e 6578 706c 6169 6e65 645f 636f    unexplained_co
+00008050: 6c5f 7374 7220 3d20 222c 2022 2e6a 6f69  l_str = ", ".joi
+00008060: 6e28 756e 6578 706c 6169 6e65 645f 636f  n(unexplained_co
+00008070: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
+00008080: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00008090: 7228 6622 7b75 6e65 7870 6c61 696e 6564  r(f"{unexplained
+000080a0: 5f63 6f6c 5f73 7472 7d20 6d65 7461 6461  _col_str} metada
+000080b0: 7461 2063 6f6c 756d 6e73 2068 6176 6520  ta columns have 
+000080c0: 756e 7265 636f 676e 697a 6564 2064 7479  unrecognized dty
+000080d0: 7065 732e 2229 0d0a 2020 2020 2020 2020  pes.")..        
+000080e0: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
+000080f0: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
+00008100: 7328 696e 636c 7564 653d 6474 7970 6573  s(include=dtypes
+00008110: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
+00008120: 6466 2e64 726f 706e 6128 6178 6973 3d31  df.dropna(axis=1
+00008130: 2c20 686f 773d 2261 6c6c 2229 0d0a 2020  , how="all")..  
+00008140: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
+00008150: 0a20 2020 200d 0a20 2020 2064 6566 2067  .    ..    def g
+00008160: 6574 5f63 6174 6567 6f72 795f 6f76 6572  et_category_over
+00008170: 7265 7072 6573 656e 7461 7469 6f6e 2873  representation(s
+00008180: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081a0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+000081b0: 7965 723a 2073 7472 2c0d 0a20 2020 2020  yer: str,..     
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081f0: 2020 2074 7275 6e63 6174 655f 6e65 6761     truncate_nega
-00008200: 7469 7665 3a20 626f 6f6c 203d 2054 7275  tive: bool = Tru
-00008210: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00008240: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
-00008250: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00008260: 6174 6520 5065 6172 736f 6e20 7265 7369  ate Pearson resi
-00008270: 6475 616c 206f 6620 6368 692d 7371 7561  dual of chi-squa
-00008280: 7265 6420 7465 7374 2c20 6173 736f 6369  red test, associ
-00008290: 6174 696e 6720 4745 5073 2066 6f72 2065  ating GEPs for e
-000082a0: 6163 6820 7261 6e6b 2028 6b29 2074 6f20  ach rank (k) to 
-000082b0: 6361 7465 676f 7269 6573 206f 6620 7361  categories of sa
-000082c0: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
-000082d0: 6e73 2e20 4279 2064 6566 6175 6c74 2c20  ns. By default, 
-000082e0: 7472 756e 6361 7465 7320 6e65 6761 7469  truncates negati
-000082f0: 7665 2076 616c 7565 732e 0d0a 0d0a 2020  ve values.....  
-00008300: 2020 2020 2020 3a70 6172 616d 206c 6179        :param lay
-00008310: 6572 3a20 6e61 6d65 206f 6620 6361 7465  er: name of cate
-00008320: 676f 7269 6361 6c20 6461 7461 206c 6179  gorical data lay
-00008330: 6572 0d0a 2020 2020 2020 2020 3a74 7970  er..        :typ
-00008340: 6520 6c61 7965 723a 2073 7472 0d0a 2020  e layer: str..  
-00008350: 2020 2020 2020 3a70 6172 616d 2074 7275        :param tru
-00008360: 6e63 6174 655f 6e65 6761 7469 7665 3a20  ncate_negative: 
-00008370: 5472 756e 6361 7465 206e 6567 6174 6976  Truncate negativ
-00008380: 6520 7265 7369 6475 616c 7320 746f 2030  e residuals to 0
-00008390: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
-000083a0: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
-000083b0: 6520 7472 756e 6361 7465 5f6e 6567 6174  e truncate_negat
-000083c0: 6976 653a 2062 6f6f 6c2c 206f 7074 696f  ive: bool, optio
-000083d0: 6e61 6c0d 0a20 2020 2020 2020 203a 7265  nal..        :re
-000083e0: 7475 726e 3a20 6361 7465 676f 7279 20c3  turn: category .
-000083f0: 9720 4745 5020 6d61 7472 6978 206f 6620  . GEP matrix of 
-00008400: 6f76 6572 7265 7072 6573 656e 7461 7469  overrepresentati
-00008410: 6f6e 2076 616c 7565 730d 0a20 2020 2020  on values..     
-00008420: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
-00008430: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
-00008440: 2022 2222 0d0a 2020 2020 2020 2020 7573   """..        us
-00008450: 6167 6520 3d20 7365 6c66 2e67 6574 5f75  age = self.get_u
-00008460: 7361 6765 7328 6e6f 726d 616c 697a 653d  sages(normalize=
-00008470: 5472 7565 292e 636f 7079 2829 0d0a 2020  True).copy()..  
-00008480: 2020 2020 2020 7361 6d70 6c65 5f74 6f5f        sample_to_
-00008490: 636c 6173 7320 3d20 7365 6c66 2e67 6574  class = self.get
-000084a0: 5f6d 6574 6164 6174 615f 6466 2829 5b6c  _metadata_df()[l
-000084b0: 6179 6572 5d0d 0a20 2020 2020 2020 2075  ayer]..        u
-000084c0: 7361 6765 2e69 6e64 6578 203d 2075 7361  sage.index = usa
-000084d0: 6765 2e69 6e64 6578 2e6d 6170 2873 616d  ge.index.map(sam
-000084e0: 706c 655f 746f 5f63 6c61 7373 290d 0a20  ple_to_class).. 
-000084f0: 2020 2020 2020 206f 6273 6572 7665 6420         observed 
-00008500: 3d20 7573 6167 652e 6772 6f75 7062 7928  = usage.groupby(
-00008510: 6178 6973 3d30 2c20 6c65 7665 6c3d 3029  axis=0, level=0)
-00008520: 2e73 756d 2829 0d0a 0d0a 2020 2020 2020  .sum()....      
-00008530: 2020 6e5f 6361 7465 676f 7269 6573 203d    n_categories =
-00008540: 206f 6273 6572 7665 642e 7368 6170 655b   observed.shape[
-00008550: 305d 0d0a 2020 2020 2020 2020 6966 206e  0]..        if n
-00008560: 5f63 6174 6567 6f72 6965 7320 3c20 323a  _categories < 2:
-00008570: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00008580: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
-00008590: 4f76 6572 7265 7072 6573 656e 7461 7469  Overrepresentati
-000085a0: 6f6e 2063 6f75 6c64 206e 6f74 2062 6520  on could not be 
-000085b0: 6361 6c63 756c 6174 6564 2066 6f72 206c  calculated for l
-000085c0: 6179 6572 2027 7b6c 6179 6572 7d27 2c20  ayer '{layer}', 
-000085d0: 6173 206f 6e6c 7920 7b6e 5f63 6174 6567  as only {n_categ
-000085e0: 6f72 6965 737d 2063 6174 6567 6f72 6965  ories} categorie
-000085f0: 7320 7765 7265 2066 6f75 6e64 2069 6e20  s were found in 
-00008600: 7468 6520 6461 7461 2e20 220d 0a20 2020  the data. "..   
-00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 2020 2020 2020 2020 2066 224e 6f74 6520           f"Note 
-00008630: 7468 6174 2065 6d70 7479 2076 616c 7565  that empty value
-00008640: 7320 696e 2074 6865 206d 6574 6164 6174  s in the metadat
-00008650: 6120 6172 6520 6e6f 7420 636f 6e73 6964  a are not consid
-00008660: 6572 6564 2061 2063 6174 6567 6f72 792e  ered a category.
-00008670: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 6622 4f76 6572 7265 7072 6573 656e 7461  f"Overrepresenta
-000086a0: 7469 6f6e 2063 616e 6e6f 7420 6265 2063  tion cannot be c
-000086b0: 616c 6375 6c61 7465 6420 7769 7468 2066  alculated with f
-000086c0: 6577 6572 2074 6861 6e20 3220 6361 7465  ewer than 2 cate
-000086d0: 676f 7269 6573 2066 6f72 2065 6163 6820  gories for each 
-000086e0: 6c61 7965 722e 2022 290d 0a20 2020 2020  layer. ")..     
-000086f0: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
-00008700: 2e44 6174 6146 7261 6d65 286e 702e 4e61  .DataFrame(np.Na
-00008710: 4e2c 2069 6e64 6578 203d 206f 6273 6572  N, index = obser
-00008720: 7665 642e 696e 6465 782c 2063 6f6c 756d  ved.index, colum
-00008730: 6e73 3d6f 6273 6572 7665 642e 636f 6c75  ns=observed.colu
-00008740: 6d6e 7329 0d0a 2020 2020 2020 2020 6578  mns)..        ex
-00008750: 7065 6374 6564 203d 205b 5d0d 0a20 2020  pected = []..   
-00008760: 2020 2020 2066 6f72 206b 2c20 6f62 735f       for k, obs_
-00008770: 6b20 696e 206f 6273 6572 7665 642e 6772  k in observed.gr
-00008780: 6f75 7062 7928 6178 6973 3d31 2c20 6c65  oupby(axis=1, le
-00008790: 7665 6c3d 3129 3a0d 0a20 2020 2020 2020  vel=1):..       
-000087a0: 2020 2020 2065 7870 5f6b 203d 2070 642e       exp_k = pd.
-000087b0: 4461 7461 4672 616d 6528 6f62 735f 6b2e  DataFrame(obs_k.
-000087c0: 7375 6d28 6178 6973 3d31 2929 2040 2070  sum(axis=1)) @ p
-000087d0: 642e 4461 7461 4672 616d 6528 6f62 735f  d.DataFrame(obs_
-000087e0: 6b2e 7375 6d28 6178 6973 3d30 2929 2e54  k.sum(axis=0)).T
-000087f0: 202f 206f 6273 5f6b 2e73 756d 2829 2e73   / obs_k.sum().s
-00008800: 756d 2829 0d0a 2020 2020 2020 2020 2020  um()..          
-00008810: 2020 6578 7065 6374 6564 2e61 7070 656e    expected.appen
-00008820: 6428 6578 705f 6b29 0d0a 2020 2020 2020  d(exp_k)..      
-00008830: 2020 6578 7065 6374 6564 203d 2070 642e    expected = pd.
-00008840: 636f 6e63 6174 2865 7870 6563 7465 642c  concat(expected,
-00008850: 2061 7869 733d 3129 0d0a 2020 2020 2020   axis=1)..      
-00008860: 2020 6368 6973 715f 7265 7369 6420 3d20    chisq_resid = 
-00008870: 286f 6273 6572 7665 6420 2d20 6578 7065  (observed - expe
-00008880: 6374 6564 2920 2f20 6e70 2e73 7172 7428  cted) / np.sqrt(
-00008890: 6578 7065 6374 6564 2920 2023 2070 6561  expected)  # pea
-000088a0: 7273 6f6e 2072 6573 6964 7561 6c20 6f66  rson residual of
-000088b0: 2063 6869 2d73 7175 6172 6564 2074 6573   chi-squared tes
-000088c0: 7420 6f66 2063 6f6e 7469 6e67 656e 6379  t of contingency
-000088d0: 2074 6162 6c65 0d0a 2020 2020 2020 2020   table..        
-000088e0: 6966 2074 7275 6e63 6174 655f 6e65 6761  if truncate_nega
-000088f0: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
-00008900: 2020 2063 6869 7371 5f72 6573 6964 203d     chisq_resid =
-00008910: 2063 6869 7371 5f72 6573 6964 2e63 6c69   chisq_resid.cli
-00008920: 7028 6c6f 7765 723d 3029 0d0a 2020 2020  p(lower=0)..    
-00008930: 2020 2020 7265 7475 726e 2063 6869 7371      return chisq
-00008940: 5f72 6573 6964 0d0a 2020 2020 0d0a 2020  _resid..    ..  
-00008950: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00008960: 6765 745f 6d65 7461 6461 7461 5f63 6f72  get_metadata_cor
-00008970: 7265 6c61 7469 6f6e 2873 656c 662c 200d  relation(self, .
-00008980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 6c61 7965 723a 2073 7472 2c0d 0a20    layer: str,.. 
+000081e0: 2020 2074 7275 6e63 6174 655f 6e65 6761     truncate_nega
+000081f0: 7469 7665 3a20 626f 6f6c 203d 2054 7275  tive: bool = Tru
+00008200: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+00008230: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
+00008240: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+00008250: 6174 6520 5065 6172 736f 6e20 7265 7369  ate Pearson resi
+00008260: 6475 616c 206f 6620 6368 692d 7371 7561  dual of chi-squa
+00008270: 7265 6420 7465 7374 2c20 6173 736f 6369  red test, associ
+00008280: 6174 696e 6720 4745 5073 2066 6f72 2065  ating GEPs for e
+00008290: 6163 6820 7261 6e6b 2028 6b29 2074 6f20  ach rank (k) to 
+000082a0: 6361 7465 676f 7269 6573 206f 6620 7361  categories of sa
+000082b0: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
+000082c0: 6e73 2e20 4279 2064 6566 6175 6c74 2c20  ns. By default, 
+000082d0: 7472 756e 6361 7465 7320 6e65 6761 7469  truncates negati
+000082e0: 7665 2076 616c 7565 732e 0d0a 0d0a 2020  ve values.....  
+000082f0: 2020 2020 2020 3a70 6172 616d 206c 6179        :param lay
+00008300: 6572 3a20 6e61 6d65 206f 6620 6361 7465  er: name of cate
+00008310: 676f 7269 6361 6c20 6461 7461 206c 6179  gorical data lay
+00008320: 6572 0d0a 2020 2020 2020 2020 3a74 7970  er..        :typ
+00008330: 6520 6c61 7965 723a 2073 7472 0d0a 2020  e layer: str..  
+00008340: 2020 2020 2020 3a70 6172 616d 2074 7275        :param tru
+00008350: 6e63 6174 655f 6e65 6761 7469 7665 3a20  ncate_negative: 
+00008360: 5472 756e 6361 7465 206e 6567 6174 6976  Truncate negativ
+00008370: 6520 7265 7369 6475 616c 7320 746f 2030  e residuals to 0
+00008380: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
+00008390: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
+000083a0: 6520 7472 756e 6361 7465 5f6e 6567 6174  e truncate_negat
+000083b0: 6976 653a 2062 6f6f 6c2c 206f 7074 696f  ive: bool, optio
+000083c0: 6e61 6c0d 0a20 2020 2020 2020 203a 7265  nal..        :re
+000083d0: 7475 726e 3a20 6361 7465 676f 7279 20c3  turn: category .
+000083e0: 9720 4745 5020 6d61 7472 6978 206f 6620  . GEP matrix of 
+000083f0: 6f76 6572 7265 7072 6573 656e 7461 7469  overrepresentati
+00008400: 6f6e 2076 616c 7565 730d 0a20 2020 2020  on values..     
+00008410: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
+00008420: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
+00008430: 2022 2222 0d0a 2020 2020 2020 2020 7573   """..        us
+00008440: 6167 6520 3d20 7365 6c66 2e67 6574 5f75  age = self.get_u
+00008450: 7361 6765 7328 6e6f 726d 616c 697a 653d  sages(normalize=
+00008460: 5472 7565 292e 636f 7079 2829 0d0a 2020  True).copy()..  
+00008470: 2020 2020 2020 7361 6d70 6c65 5f74 6f5f        sample_to_
+00008480: 636c 6173 7320 3d20 7365 6c66 2e67 6574  class = self.get
+00008490: 5f6d 6574 6164 6174 615f 6466 2829 5b6c  _metadata_df()[l
+000084a0: 6179 6572 5d0d 0a20 2020 2020 2020 2075  ayer]..        u
+000084b0: 7361 6765 2e69 6e64 6578 203d 2075 7361  sage.index = usa
+000084c0: 6765 2e69 6e64 6578 2e6d 6170 2873 616d  ge.index.map(sam
+000084d0: 706c 655f 746f 5f63 6c61 7373 290d 0a20  ple_to_class).. 
+000084e0: 2020 2020 2020 206f 6273 6572 7665 6420         observed 
+000084f0: 3d20 7573 6167 652e 6772 6f75 7062 7928  = usage.groupby(
+00008500: 6178 6973 3d30 2c20 6c65 7665 6c3d 3029  axis=0, level=0)
+00008510: 2e73 756d 2829 0d0a 0d0a 2020 2020 2020  .sum()....      
+00008520: 2020 6e5f 6361 7465 676f 7269 6573 203d    n_categories =
+00008530: 206f 6273 6572 7665 642e 7368 6170 655b   observed.shape[
+00008540: 305d 0d0a 2020 2020 2020 2020 6966 206e  0]..        if n
+00008550: 5f63 6174 6567 6f72 6965 7320 3c20 323a  _categories < 2:
+00008560: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00008570: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
+00008580: 4f76 6572 7265 7072 6573 656e 7461 7469  Overrepresentati
+00008590: 6f6e 2063 6f75 6c64 206e 6f74 2062 6520  on could not be 
+000085a0: 6361 6c63 756c 6174 6564 2066 6f72 206c  calculated for l
+000085b0: 6179 6572 2027 7b6c 6179 6572 7d27 2c20  ayer '{layer}', 
+000085c0: 6173 206f 6e6c 7920 7b6e 5f63 6174 6567  as only {n_categ
+000085d0: 6f72 6965 737d 2063 6174 6567 6f72 6965  ories} categorie
+000085e0: 7320 7765 7265 2066 6f75 6e64 2069 6e20  s were found in 
+000085f0: 7468 6520 6461 7461 2e20 220d 0a20 2020  the data. "..   
+00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008610: 2020 2020 2020 2020 2066 224e 6f74 6520           f"Note 
+00008620: 7468 6174 2065 6d70 7479 2076 616c 7565  that empty value
+00008630: 7320 696e 2074 6865 206d 6574 6164 6174  s in the metadat
+00008640: 6120 6172 6520 6e6f 7420 636f 6e73 6964  a are not consid
+00008650: 6572 6564 2061 2063 6174 6567 6f72 792e  ered a category.
+00008660: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 6622 4f76 6572 7265 7072 6573 656e 7461  f"Overrepresenta
+00008690: 7469 6f6e 2063 616e 6e6f 7420 6265 2063  tion cannot be c
+000086a0: 616c 6375 6c61 7465 6420 7769 7468 2066  alculated with f
+000086b0: 6577 6572 2074 6861 6e20 3220 6361 7465  ewer than 2 cate
+000086c0: 676f 7269 6573 2066 6f72 2065 6163 6820  gories for each 
+000086d0: 6c61 7965 722e 2022 290d 0a20 2020 2020  layer. ")..     
+000086e0: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
+000086f0: 2e44 6174 6146 7261 6d65 286e 702e 4e61  .DataFrame(np.Na
+00008700: 4e2c 2069 6e64 6578 203d 206f 6273 6572  N, index = obser
+00008710: 7665 642e 696e 6465 782c 2063 6f6c 756d  ved.index, colum
+00008720: 6e73 3d6f 6273 6572 7665 642e 636f 6c75  ns=observed.colu
+00008730: 6d6e 7329 0d0a 2020 2020 2020 2020 6578  mns)..        ex
+00008740: 7065 6374 6564 203d 205b 5d0d 0a20 2020  pected = []..   
+00008750: 2020 2020 2066 6f72 206b 2c20 6f62 735f       for k, obs_
+00008760: 6b20 696e 206f 6273 6572 7665 642e 6772  k in observed.gr
+00008770: 6f75 7062 7928 6178 6973 3d31 2c20 6c65  oupby(axis=1, le
+00008780: 7665 6c3d 3129 3a0d 0a20 2020 2020 2020  vel=1):..       
+00008790: 2020 2020 2065 7870 5f6b 203d 2070 642e       exp_k = pd.
+000087a0: 4461 7461 4672 616d 6528 6f62 735f 6b2e  DataFrame(obs_k.
+000087b0: 7375 6d28 6178 6973 3d31 2929 2040 2070  sum(axis=1)) @ p
+000087c0: 642e 4461 7461 4672 616d 6528 6f62 735f  d.DataFrame(obs_
+000087d0: 6b2e 7375 6d28 6178 6973 3d30 2929 2e54  k.sum(axis=0)).T
+000087e0: 202f 206f 6273 5f6b 2e73 756d 2829 2e73   / obs_k.sum().s
+000087f0: 756d 2829 0d0a 2020 2020 2020 2020 2020  um()..          
+00008800: 2020 6578 7065 6374 6564 2e61 7070 656e    expected.appen
+00008810: 6428 6578 705f 6b29 0d0a 2020 2020 2020  d(exp_k)..      
+00008820: 2020 6578 7065 6374 6564 203d 2070 642e    expected = pd.
+00008830: 636f 6e63 6174 2865 7870 6563 7465 642c  concat(expected,
+00008840: 2061 7869 733d 3129 0d0a 2020 2020 2020   axis=1)..      
+00008850: 2020 6368 6973 715f 7265 7369 6420 3d20    chisq_resid = 
+00008860: 286f 6273 6572 7665 6420 2d20 6578 7065  (observed - expe
+00008870: 6374 6564 2920 2f20 6e70 2e73 7172 7428  cted) / np.sqrt(
+00008880: 6578 7065 6374 6564 2920 2023 2070 6561  expected)  # pea
+00008890: 7273 6f6e 2072 6573 6964 7561 6c20 6f66  rson residual of
+000088a0: 2063 6869 2d73 7175 6172 6564 2074 6573   chi-squared tes
+000088b0: 7420 6f66 2063 6f6e 7469 6e67 656e 6379  t of contingency
+000088c0: 2074 6162 6c65 0d0a 2020 2020 2020 2020   table..        
+000088d0: 6966 2074 7275 6e63 6174 655f 6e65 6761  if truncate_nega
+000088e0: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
+000088f0: 2020 2063 6869 7371 5f72 6573 6964 203d     chisq_resid =
+00008900: 2063 6869 7371 5f72 6573 6964 2e63 6c69   chisq_resid.cli
+00008910: 7028 6c6f 7765 723d 3029 0d0a 2020 2020  p(lower=0)..    
+00008920: 2020 2020 7265 7475 726e 2063 6869 7371      return chisq
+00008930: 5f72 6573 6964 0d0a 2020 2020 0d0a 2020  _resid..    ..  
+00008940: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00008950: 6765 745f 6d65 7461 6461 7461 5f63 6f72  get_metadata_cor
+00008960: 7265 6c61 7469 6f6e 2873 656c 662c 200d  relation(self, .
+00008970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 6c61 7965 723a 2073 7472 2c0d 0a20    layer: str,.. 
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 6d65 7468 6f64 3a20 7374 7220 3d20 2270  method: str = "p
-000089e0: 6561 7273 6f6e 220d 0a20 2020 2020 2020  earson"..       
-000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a00: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
-00008a10: 642e 5365 7269 6573 3a0d 0a20 2020 2020  d.Series:..     
-00008a20: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
-00008a30: 5065 6172 736f 6e20 636f 7272 656c 6174  Pearson correlat
-00008a40: 696f 6e20 6f66 2047 4550 2075 7361 6765  ion of GEP usage
-00008a50: 2074 6f20 6e75 6d65 7269 6361 6c20 6d65   to numerical me
-00008a60: 7461 6461 7461 2061 6372 6f73 7320 7361  tadata across sa
-00008a70: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
-00008a80: 6e73 2e0d 0a0d 0a20 2020 2020 2020 203a  ns.....        :
-00008a90: 7061 7261 6d20 6c61 7965 723a 206e 616d  param layer: nam
-00008aa0: 6520 6f66 206e 756d 6572 6963 616c 2064  e of numerical d
-00008ab0: 6174 6120 6c61 7965 720d 0a20 2020 2020  ata layer..     
-00008ac0: 2020 203a 7479 7065 206c 6179 6572 3a20     :type layer: 
-00008ad0: 7374 720d 0a20 2020 2020 2020 203a 7061  str..        :pa
-00008ae0: 7261 6d20 6d65 7468 6f64 3a20 436f 7272  ram method: Corr
-00008af0: 656c 6174 696f 6e20 6d65 7468 6f64 3a20  elation method: 
-00008b00: 2270 6561 7273 6f6e 222c 2022 7370 6561  "pearson", "spea
-00008b10: 726d 616e 222c 206f 7220 226b 656e 6461  rman", or "kenda
-00008b20: 6c6c 222e 2044 6566 6175 6c74 7320 746f  ll". Defaults to
-00008b30: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
-00008b40: 2020 2020 3a74 7970 6520 6d65 7468 6f64      :type method
-00008b50: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
-00008b60: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00008b70: 3a20 636f 7272 656c 6174 696f 6e20 6f66  : correlation of
-00008b80: 2047 4550 2074 6f20 6d65 7461 6461 7461   GEP to metadata
-00008b90: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00008ba0: 3a20 7064 2e53 6572 6965 730d 0a20 2020  : pd.Series..   
-00008bb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00008bc0: 2020 7573 6167 6520 3d20 7365 6c66 2e67    usage = self.g
-00008bd0: 6574 5f75 7361 6765 7328 292e 636f 7079  et_usages().copy
-00008be0: 2829 0d0a 2020 2020 2020 2020 6d65 7461  ()..        meta
-00008bf0: 6461 7461 203d 2073 656c 662e 6765 745f  data = self.get_
-00008c00: 6d65 7461 6461 7461 5f64 6628 295b 6c61  metadata_df()[la
-00008c10: 7965 725d 0d0a 2020 2020 2020 2020 6d64  yer]..        md
-00008c20: 5f63 6f72 7220 3d20 7573 6167 652e 636f  _corr = usage.co
-00008c30: 7272 7769 7468 286d 6574 6164 6174 612c  rrwith(metadata,
-00008c40: 206d 6574 686f 643d 6d65 7468 6f64 290d   method=method).
-00008c50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008c60: 6d64 5f63 6f72 720d 0a20 2020 2020 2020  md_corr..       
-00008c70: 200d 0a20 2020 2064 6566 2061 7070 656e   ..    def appen
-00008c80: 645f 746f 5f68 6973 746f 7279 2873 656c  d_to_history(sel
-00008c90: 662c 2065 6e74 7279 293a 0d0a 2020 2020  f, entry):..    
-00008ca0: 2020 2020 2222 2241 6464 2065 6e74 7279      """Add entry
-00008cb0: 2074 6f20 4461 7461 7365 7420 6869 7374   to Dataset hist
-00008cc0: 6f72 792e 0d0a 0d0a 2020 2020 2020 2020  ory.....        
-00008cd0: 3a70 6172 616d 2065 6e74 7279 3a20 4465  :param entry: De
-00008ce0: 7363 7269 7074 696f 6e20 6f66 2065 7665  scription of eve
-00008cf0: 6e74 2074 6f20 7265 636f 7264 2069 6e20  nt to record in 
-00008d00: 7468 6520 6869 7374 6f72 792e 0d0a 2020  the history...  
-00008d10: 2020 2020 2020 3a74 7970 6520 656e 7472        :type entr
-00008d20: 793a 2073 7472 0d0a 2020 2020 2020 2020  y: str..        
-00008d30: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00008d40: 662e 6164 6174 612e 756e 735b 2268 6973  f.adata.uns["his
-00008d50: 746f 7279 225d 5b64 6174 6574 696d 652e  tory"][datetime.
-00008d60: 7574 636e 6f77 2829 2e69 736f 666f 726d  utcnow().isoform
-00008d70: 6174 2829 5d20 3d20 656e 7472 790d 0a20  at()] = entry.. 
-00008d80: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00008d90: 2067 6574 5f68 6973 746f 7279 2873 656c   get_history(sel
-00008da0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00008db0: 5265 7475 726e 7320 7469 6d65 7374 616d  Returns timestam
-00008dc0: 7065 6420 6869 7374 6f72 7920 6f66 2044  ped history of D
-00008dd0: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
-00008de0: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00008df0: 6e3a 2068 6973 746f 7279 0d0a 2020 2020  n: history..    
-00008e00: 2020 2020 3a72 7479 7065 3a20 6469 6374      :rtype: dict
-00008e10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00008e20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00008e30: 6c66 2e61 6461 7461 2e75 6e73 5b22 6869  lf.adata.uns["hi
-00008e40: 7374 6f72 7922 5d                        story"]
+000089c0: 6d65 7468 6f64 3a20 7374 7220 3d20 2270  method: str = "p
+000089d0: 6561 7273 6f6e 220d 0a20 2020 2020 2020  earson"..       
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
+00008a00: 642e 5365 7269 6573 3a0d 0a20 2020 2020  d.Series:..     
+00008a10: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+00008a20: 5065 6172 736f 6e20 636f 7272 656c 6174  Pearson correlat
+00008a30: 696f 6e20 6f66 2047 4550 2075 7361 6765  ion of GEP usage
+00008a40: 2074 6f20 6e75 6d65 7269 6361 6c20 6d65   to numerical me
+00008a50: 7461 6461 7461 2061 6372 6f73 7320 7361  tadata across sa
+00008a60: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
+00008a70: 6e73 2e0d 0a0d 0a20 2020 2020 2020 203a  ns.....        :
+00008a80: 7061 7261 6d20 6c61 7965 723a 206e 616d  param layer: nam
+00008a90: 6520 6f66 206e 756d 6572 6963 616c 2064  e of numerical d
+00008aa0: 6174 6120 6c61 7965 720d 0a20 2020 2020  ata layer..     
+00008ab0: 2020 203a 7479 7065 206c 6179 6572 3a20     :type layer: 
+00008ac0: 7374 720d 0a20 2020 2020 2020 203a 7061  str..        :pa
+00008ad0: 7261 6d20 6d65 7468 6f64 3a20 436f 7272  ram method: Corr
+00008ae0: 656c 6174 696f 6e20 6d65 7468 6f64 3a20  elation method: 
+00008af0: 2270 6561 7273 6f6e 222c 2022 7370 6561  "pearson", "spea
+00008b00: 726d 616e 222c 206f 7220 226b 656e 6461  rman", or "kenda
+00008b10: 6c6c 222e 2044 6566 6175 6c74 7320 746f  ll". Defaults to
+00008b20: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
+00008b30: 2020 2020 3a74 7970 6520 6d65 7468 6f64      :type method
+00008b40: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
+00008b50: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00008b60: 3a20 636f 7272 656c 6174 696f 6e20 6f66  : correlation of
+00008b70: 2047 4550 2074 6f20 6d65 7461 6461 7461   GEP to metadata
+00008b80: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00008b90: 3a20 7064 2e53 6572 6965 730d 0a20 2020  : pd.Series..   
+00008ba0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00008bb0: 2020 7573 6167 6520 3d20 7365 6c66 2e67    usage = self.g
+00008bc0: 6574 5f75 7361 6765 7328 292e 636f 7079  et_usages().copy
+00008bd0: 2829 0d0a 2020 2020 2020 2020 6d65 7461  ()..        meta
+00008be0: 6461 7461 203d 2073 656c 662e 6765 745f  data = self.get_
+00008bf0: 6d65 7461 6461 7461 5f64 6628 295b 6c61  metadata_df()[la
+00008c00: 7965 725d 0d0a 2020 2020 2020 2020 6d64  yer]..        md
+00008c10: 5f63 6f72 7220 3d20 7573 6167 652e 636f  _corr = usage.co
+00008c20: 7272 7769 7468 286d 6574 6164 6174 612c  rrwith(metadata,
+00008c30: 206d 6574 686f 643d 6d65 7468 6f64 290d   method=method).
+00008c40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008c50: 6d64 5f63 6f72 720d 0a20 2020 2020 2020  md_corr..       
+00008c60: 200d 0a20 2020 2064 6566 2061 7070 656e   ..    def appen
+00008c70: 645f 746f 5f68 6973 746f 7279 2873 656c  d_to_history(sel
+00008c80: 662c 2065 6e74 7279 293a 0d0a 2020 2020  f, entry):..    
+00008c90: 2020 2020 2222 2241 6464 2065 6e74 7279      """Add entry
+00008ca0: 2074 6f20 4461 7461 7365 7420 6869 7374   to Dataset hist
+00008cb0: 6f72 792e 0d0a 0d0a 2020 2020 2020 2020  ory.....        
+00008cc0: 3a70 6172 616d 2065 6e74 7279 3a20 4465  :param entry: De
+00008cd0: 7363 7269 7074 696f 6e20 6f66 2065 7665  scription of eve
+00008ce0: 6e74 2074 6f20 7265 636f 7264 2069 6e20  nt to record in 
+00008cf0: 7468 6520 6869 7374 6f72 792e 0d0a 2020  the history...  
+00008d00: 2020 2020 2020 3a74 7970 6520 656e 7472        :type entr
+00008d10: 793a 2073 7472 0d0a 2020 2020 2020 2020  y: str..        
+00008d20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00008d30: 662e 6164 6174 612e 756e 735b 2268 6973  f.adata.uns["his
+00008d40: 746f 7279 225d 5b64 6174 6574 696d 652e  tory"][datetime.
+00008d50: 7574 636e 6f77 2829 2e69 736f 666f 726d  utcnow().isoform
+00008d60: 6174 2829 5d20 3d20 656e 7472 790d 0a20  at()] = entry.. 
+00008d70: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00008d80: 2067 6574 5f68 6973 746f 7279 2873 656c   get_history(sel
+00008d90: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00008da0: 5265 7475 726e 7320 7469 6d65 7374 616d  Returns timestam
+00008db0: 7065 6420 6869 7374 6f72 7920 6f66 2044  ped history of D
+00008dc0: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
+00008dd0: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00008de0: 6e3a 2068 6973 746f 7279 0d0a 2020 2020  n: history..    
+00008df0: 2020 2020 3a72 7479 7065 3a20 6469 6374      :rtype: dict
+00008e00: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00008e10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008e20: 6c66 2e61 6461 7461 2e75 6e73 5b22 6869  lf.adata.uns["hi
+00008e30: 7374 6f72 7922 5d                        story"]
```

### Comparing `cnmfsns-1.6.0/src/cnmfsns/integration.py` & `cnmfsns-1.6.5/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/plots.py` & `cnmfsns-1.6.5/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns/sns.py` & `cnmfsns-1.6.5/src/cnmfsns/sns.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 import pandas as pd
 import networkx as nx
 import matplotlib as mpl
 import igraph
 import pickle
 import distinctipy
+import tomli
 import tomli_w
 import networkx as nx
 from scipy.stats import entropy
 
 class SNS():
     def __init__(self,
                  integration: Integration,
@@ -286,14 +287,28 @@
 
         self.communities = communities
         self.gep_communities = {gep: community for community, geps in communities.items() for gep in geps}
 
         # also create a community network with default parameters, so that self.comm_graph is available if needed. However, self.create_community_network can be called again
         self.create_community_network()
 
+    def read_communities_from_toml(self, toml_file):
+
+        with open(toml_file, 'rb') as f:
+            communities = tomli.load(f)
+            
+        # community names must be strings to avoid problems with TOML persistence and flexibility for custom community naming (eg., for subclustering)
+        communities = {str(k): v for k, v in communities.items()}
+        
+        self.communities = communities
+        self.gep_communities = {gep: community for community, geps in communities.items() for gep in geps}
+
+        # also create a community network with default parameters, so that self.comm_graph is available if needed. However, self.create_community_network can be called again
+        self.create_community_network()
+
     def prune_communities(self,
                           min_nodes: int = 1,
                           min_datasets: int = 1,
                           min_nodes_per_dataset: int = 0,
                           renumber = False):
         """Prune communities based on one or more filters.
```

### Comparing `cnmfsns-1.6.0/src/cnmfsns/utils.py` & `cnmfsns-1.6.5/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.6.0/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.6.5/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.6.0
+Version: 1.6.5
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.6.0-blue)
+![version badge](https://img.shields.io/badge/version-1.6.5-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

