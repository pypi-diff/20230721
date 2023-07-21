# Comparing `tmp/checkatlas-0.3.6.tar.gz` & `tmp/checkatlas-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.3.6.tar", max compression
+gzip compressed data, was "checkatlas-0.3.7.tar", max compression
```

## Comparing `checkatlas-0.3.6.tar` & `checkatlas-0.3.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1506 2023-07-19 23:44:16.628232 checkatlas-0.3.6/LICENSE
--rw-r--r--   0        0        0     4452 2023-07-19 23:44:16.628232 checkatlas-0.3.6/README.md
--rw-r--r--   0        0        0      111 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/__init__.py
--rw-r--r--   0        0        0     4658 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/__main__.py
--rw-r--r--   0        0        0    24756 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/atlas.py
--rw-r--r--   0        0        0     4715 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/cellranger.py
--rw-r--r--   0        0        0    10077 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     2913 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0       45 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      254 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4108 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/seurat.py
--rw-r--r--   0        0        0        6 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/VERSION
--rw-r--r--   0        0        0      107 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4483 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     4239 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/checkatlas_workflow_arguments.py
--rw-r--r--   0        0        0     2759 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-19 23:44:16.628232 checkatlas-0.3.6/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1427 2023-07-19 23:44:16.824236 checkatlas-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 checkatlas-0.3.6/setup.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-21 13:19:30.149579 checkatlas-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-21 13:19:30.149579 checkatlas-0.3.7/README.md
+-rw-r--r--   0        0        0      111 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4674 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24921 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/atlas.py
+-rw-r--r--   0        0        0     9680 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/cellranger.py
+-rw-r--r--   0        0        0    11434 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     2913 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0       45 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      254 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4124 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/seurat.py
+-rw-r--r--   0        0        0        6 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/utils/VERSION
+-rw-r--r--   0        0        0      107 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4523 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     4239 2023-07-21 13:19:30.149579 checkatlas-0.3.7/checkatlas/utils/checkatlas_workflow_arguments.py
+-rw-r--r--   0        0        0     2759 2023-07-21 13:19:30.153579 checkatlas-0.3.7/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-21 13:19:30.153579 checkatlas-0.3.7/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-21 13:19:30.153579 checkatlas-0.3.7/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1427 2023-07-21 13:19:30.385588 checkatlas-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 checkatlas-0.3.7/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.7/PKG-INFO
```

### Comparing `checkatlas-0.3.6/LICENSE` & `checkatlas-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/README.md` & `checkatlas-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/__main__.py` & `checkatlas-0.3.7/checkatlas/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Set logger level
     if args.debug:
         logger.setLevel(getattr(logging, "DEBUG"))
     else:
         logger.setLevel(getattr(logging, "INFO"))
 
     logger.debug(f"Program arguments: {args}")
-    
+
     #   ######    Run Checkatlas   #########
     (
         clean_scanpy_list,
         clean_cellranger_list,
         clean_seurat_list,
     ) = checkatlas.read_list_atlases(args.path)
     clean_scanpy_list = clean_scanpy_list.to_dict("index")
@@ -55,14 +55,15 @@
         atlas_info = clean_seurat_list[args.atlas_name]
     else:
         logger.error(f"Cannot found {args.atlas_name}")
     logger.debug(f"Found atlas: {atlas_info}")
     # Run process
     process = args.process
     atlas_type = atlas_info[checkatlas.ATLAS_TYPE_KEY]
+    print(atlas_info)
     if (
         atlas_type == atlas.ANNDATA_TYPE
         or atlas_type == cellranger.CELLRANGER_TYPE_CURRENT
         or atlas_type == cellranger.CELLRANGER_TYPE_OBSOLETE
     ):
         if process == checkatlas.PROCESS_TYPE[0]:
             adata = atlas.read_atlas(atlas_info)
@@ -71,15 +72,15 @@
             atlas.create_anndata_table(adata, atlas_info, args)
             atlas.create_umap_fig(adata, atlas_info, args)
             atlas.create_tsne_fig(adata, atlas_info, args)
         elif process == checkatlas.PROCESS_TYPE[1]:
             adata = atlas.read_atlas(atlas_info)
             adata = atlas.clean_scanpy_atlas(adata, atlas_info)
             atlas.create_qc_tables(adata, atlas_info, args)
-            # atlas.create_qc_plots(adata, atlas_info, args)
+            atlas.create_qc_plots(adata, atlas_info, args)
         elif process == checkatlas.PROCESS_TYPE[2]:
             adata = atlas.read_atlas(atlas_info)
             adata = atlas.clean_scanpy_atlas(adata, atlas_info)
             atlas.create_metric_cluster(adata, atlas_info, args)
         elif process == checkatlas.PROCESS_TYPE[3]:
             adata = atlas.read_atlas(atlas_info)
             adata = atlas.clean_scanpy_atlas(adata, atlas_info)
```

### Comparing `checkatlas-0.3.6/checkatlas/atlas.py` & `checkatlas-0.3.7/checkatlas/atlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 OBS_CLUSTERS = [
     "cell_type",
     "CellType",
     "celltype",
     "ann_finest_level",
     "cellranger_graphclust",
+    "cellranger_kmeans",
     "seurat_clusters",
     "RNA_snn_res.0.5",
     "louvain",
     "leiden",
     "orig.ident",
 ]
 
@@ -104,24 +105,24 @@
     )
     try:
         if (
             atlas_info[checkatlas.ATLAS_TYPE_KEY]
             == cellranger.CELLRANGER_TYPE_CURRENT
         ):
             logger.debug(
-                "Read Cellranger results "
+                "Read Cellranger >= v3 results "
                 f"{atlas_info[checkatlas.ATLAS_PATH_KEY]}"
             )
             adata = cellranger.read_cellranger_current(atlas_info)
         elif (
             atlas_info[checkatlas.ATLAS_TYPE_KEY]
             == cellranger.CELLRANGER_TYPE_OBSOLETE
         ):
             logger.debug(
-                "Read Cellranger results "
+                "Read Cellranger < v3 results "
                 f"{atlas_info[checkatlas.ATLAS_PATH_KEY]}"
             )
             adata = cellranger.read_cellranger_obsolete(atlas_info)
         else:
             logger.debug(
                 f"Read Scanpy file {atlas_info[checkatlas.ATLAS_PATH_KEY]}"
             )
@@ -584,18 +585,21 @@
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
     obsm_keys = get_viable_obsm(adata, args)
     r = re.compile(".*umap*.")
     obsm_umap_keys = list(filter(r.match, obsm_keys))
     r = re.compile(".*tsne*.")
     obsm_tsne_keys = list(filter(r.match, obsm_keys))
+    obsm_key_representation = ""
     if len(obsm_umap_keys) > 0:
         obsm_key_representation = obsm_umap_keys[0]
+        print("reach", obsm_key_representation)
     elif len(obsm_tsne_keys) > 0:
         obsm_key_representation = obsm_tsne_keys[0]
+        print("reach", obsm_key_representation)
 
     if len(obs_keys) > 0:
         logger.debug(f"Calc clustering metrics for {atlas_name}")
         for obs_key in obs_keys:
             dict_line = {
                 "Clust_Sample": [atlas_name + "_" + obs_key],
                 "obs": [obs_key],
```

### Comparing `checkatlas-0.3.6/checkatlas/checkatlas.py` & `checkatlas-0.3.7/checkatlas/checkatlas.py`

 * *Files 18% similar despite different names*

```diff
@@ -292,12 +292,46 @@
         + path_fig
         + """\" >\n</div>\n"""
     )
 
 
 if __name__ == "__main__":
     path = "/data/analysis/data_becavin/checkatlas_test/tuto"
-    path = "/Users/christophebecavin/Documents/testatlas/"
-    # atlas_path = "/Users/christophebecavin/Documents/testatlas/"
-    atlas_info = ["test_version", "Scanpy", ".h5ad", "data/test_version.h5ad"]
-    # folders.checkatlas_folders(path)
+    atlas_info = {
+        "Atlas_name": "pbmc_6k_v1_v1",
+        "Atlas_type": "Cellranger < v3",
+        "Atlas_extension": ".mtx",
+        "Atlas_path": "/data/analysis/data_becavin/"
+        "checkatlas_test/tuto/data5/"
+        "pbmc_6k_v1_v1/outs/"
+        "filtered_matrices_mex/hg19/matrix.mtx",
+    }
+
+    """ atlas_info = {'Atlas_name': 'pbmc_5k_v3_v3',
+                   'Atlas_type': 'Cellranger >= v3',
+                     'Atlas_extension': '.h5',
+                       'Atlas_path':
+                       '/data/analysis/data_becavin/'
+                       'checkatlas_test/tuto/data5/'
+                       'pbmc_5k_v3_v3/outs/'
+                       '5k_pbmc_v3_filtered_feature_bc_matrix.h5'}
+
+    atlas_info = {'Atlas_name': 'pbmc_5k_v3_v7',
+                   'Atlas_type': 'Cellranger >= v3',
+                     'Atlas_extension': '.h5',
+                       'Atlas_path':
+                       '/data/analysis/data_becavin/'
+                       'checkatlas_test/tuto/data5/'
+                       'pbmc_5k_v3_v7/outs/'
+                       'SC3pv3_GEX_Human_PBMC_filtered_feature_bc_matrix.h5'}
+
+    atlas_info = {'Atlas_name': 'pbmc_3k_multiome',
+                   'Atlas_type': 'Cellranger >= v3',
+                     'Atlas_extension': '.h5',
+                       'Atlas_path':
+                       '/data/analysis/data_becavin/'
+                       'checkatlas_test/tuto/data5/'
+                       'pbmc_3k_multiome/outs/'
+                       'pbmc_unsorted_3k_filtered_feature_bc_matrix.h5'} """
+
+    adata = atlas.read_atlas(atlas_info)
     # atlas_list = list_atlases(path)
```

### Comparing `checkatlas-0.3.6/checkatlas/checkatlas_workflow.py` & `checkatlas-0.3.7/checkatlas/checkatlas_workflow.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.7/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/metrics/metrics.py` & `checkatlas-0.3.7/checkatlas/metrics/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
 def calc_metric_cluster_scanpy(
     metric, adata, obs_key, obsm_key_representation
 ):
     if metric in METRICS_CLUST:
         metric_module = getattr(cluster, metric)
         annotations = adata.obs[obs_key]
-        if obsm_key_representation:
+        if obsm_key_representation != "":
             count_repr = adata.obsm[obsm_key_representation]
             return metric_module.run(count_repr, annotations)
         else:
-            original_count = adata.X
+            original_count = adata.X.toarray()
             return metric_module.run(original_count, annotations)
     else:
         logger.warning(
             f"{metric} is not a recognized "
             f"cluster metric.\n"
             f"List of clustering metrics: {METRICS_CLUST}"
         )
```

### Comparing `checkatlas-0.3.6/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.7/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.7/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.7/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.7/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/seurat.py` & `checkatlas-0.3.7/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.3.7/checkatlas/utils/checkatlas_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import argparse
 from importlib.resources import files
+
 from checkatlas import atlas, checkatlas
 from checkatlas.metrics import annot, cluster, dimred
 
+
 def create_parser():
     parser = argparse.ArgumentParser(
         prog="checkatlas",
         usage="checkatlas [OPTIONS] process atlas_name your_search_folder/",
         description="CheckAtlas is a one liner tool to check the "
         "quality of your single-cell atlases. For "
         "every atlas, it produces the quality control "
@@ -98,16 +100,17 @@
         "use in the clustering metric calculus."
         "Example: --obs_cluster celltype leuven seurat_clusters",
     )
     metric_options.add_argument(
         "--metric_cluster",
         nargs="+",
         type=str,
+        default=["davies_bouldin"],
         # default=["silhouette", "davies_bouldin"],
-        default=[""],
+        # default=[""],
         help="Specify the list of clustering metrics to calculate.\n"
         "   Example: --metric_cluster silhouette davies_bouldin\n"
         f"   List of cluster metrics: {cluster.__all__}",
     )
     metric_options.add_argument(
         "--metric_annot",
         nargs="+",
```

### Comparing `checkatlas-0.3.6/checkatlas/utils/checkatlas_workflow_arguments.py` & `checkatlas-0.3.7/checkatlas/utils/checkatlas_workflow_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/utils/files.py` & `checkatlas-0.3.7/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/utils/folders.py` & `checkatlas-0.3.7/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.3.7/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.6/pyproject.toml` & `checkatlas-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.3.6"
+version = "0.3.7"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf","pyproject.toml"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.3.6/setup.py` & `checkatlas-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.3.6/PKG-INFO` & `checkatlas-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.3.6
+Version: 0.3.7
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

