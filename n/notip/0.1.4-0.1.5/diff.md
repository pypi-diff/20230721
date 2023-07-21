# Comparing `tmp/notip-0.1.4.tar.gz` & `tmp/notip-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notip-0.1.4.tar", last modified: Wed Apr 19 20:35:27 2023, max compression
+gzip compressed data, was "notip-0.1.5.tar", last modified: Fri Jul 21 17:31:32 2023, max compression
```

## Comparing `notip-0.1.4.tar` & `notip-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-19 20:35:27.354179 notip-0.1.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/notip/
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.4/notip/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    37519 2023-04-19 20:34:39.000000 notip-0.1.4/notip/posthoc_fmri.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 20:35:27.354179 notip-0.1.4/notip.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      108 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-19 20:35:27.000000 notip-0.1.4/notip.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-19 20:35:27.354179 notip-0.1.4/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      976 2023-04-19 20:35:13.000000 notip-0.1.4/setup.py
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/
+-rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 17:31:32.474754 notip-0.1.5/PKG-INFO
+-rw-r--r--   0 ablain   (666989) soda     (202037)      848 2023-05-08 21:35:42.000000 notip-0.1.5/README.md
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/notip/
+-rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-05-08 21:35:42.000000 notip-0.1.5/notip/__init__.py
+-rw-r--r--   0 ablain   (666989) soda     (202037)    45671 2023-06-21 12:32:40.000000 notip-0.1.5/notip/posthoc_fmri.py
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/notip.egg-info/
+-rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/PKG-INFO
+-rw-r--r--   0 ablain   (666989) soda     (202037)      212 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/SOURCES.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/dependency_links.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)      108 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/requires.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)        6 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/top_level.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)       79 2023-07-21 17:31:32.474754 notip-0.1.5/setup.cfg
+-rw-r--r--   0 ablain   (666989) soda     (202037)      976 2023-07-21 17:31:05.000000 notip-0.1.5/setup.py
```

### Comparing `notip-0.1.4/PKG-INFO` & `notip-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.4/README.md` & `notip-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `notip-0.1.4/notip/posthoc_fmri.py` & `notip-0.1.5/notip/posthoc_fmri.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 import os
 import json
 import pandas as pd
 from tqdm import tqdm
 
 from string import ascii_lowercase
 from scipy import ndimage
+from joblib import Memory
 
 from nilearn.image import threshold_img
 from nilearn.image.resampling import coord_transform
 from nilearn._utils import check_niimg_3d
 from nilearn._utils.niimg import _safe_get_data
 
 from nilearn.reporting._get_clusters_table import _local_max
+from sanssouci import row_welch_tests
 
 
 def get_data_driven_template_two_tasks(
         task1, task2, smoothing_fwhm=4,
         collection=1952, B=100, cap_subjects=False, n_jobs=1, seed=None):
     """
     Get (task1 - task2) data-driven template for two Neurovault contrasts
@@ -452,14 +454,15 @@
     return bounds_tot
 
 
 def sim_experiment_notip(dim, FWHM, pi0, sig_train, sig_test, fdr, alpha=0.05, n_train=5, n_test=5, train_on_same=False, repeats=10, B=10, n_jobs=1, seed=None):
 
     '''
     Check if the FDP is successfully controlled for a given number of experiments on simulated data
+    using the Notip procedure.
     '''
     np.random.seed(seed)
 
     fdp_ari = []
     fdp_simes = []
     fdp_learned = []
     #fdp_bh = []
@@ -519,83 +522,157 @@
     tdp_learned = np.array(tdp_learned)
 
     return fdp_ari, fdp_simes, fdp_learned, ((tdp_simes - tdp_ari)/tdp_ari) * 100, ((tdp_learned - tdp_ari)/tdp_ari) * 100, ((tdp_learned - tdp_simes)/tdp_simes) * 100
     # return fdp_ari, fdp_simes, fdp_learned, tdp_ari, tdp_simes, tdp_learned
 
 
 def report_fdp_tdp(p_values, cutoff, beta_true, n_clusters):
-        selected = np.where(p_values <= cutoff)[0]
-        prediction = np.array([0] * n_clusters)
-        prediction[selected] = 1
-        conf = confusion_matrix(beta_true, prediction)
-        tn, fp, fn, tp = conf.ravel()
-        if fp + tp == 0:
-            fdp = 0
-            tdp = 0
-        else:
-            fdp = fp/(fp+tp)
-            tdp = tp/np.sum(beta_true)
-
-        return fdp, tdp
-
-
-def get_clusters_table_TDP(stat_img, stat_threshold, fmri_input,
-                           learned_templates, alpha=0.05,
-                           k_max=1000, B=1000, cluster_threshold=None,
-                           two_sided=False, min_distance=8., seed=None):
+    """Report the FDP and TDP for a given cutoff
+
+    Args:
+        p_values: p-values
+        cutoff: cutoff
+        beta_true: true beta
+        n_clusters: number of clusters
+    Returns:
+        fdp: false discovery proportion
+        tdp: true discovery proportion
+    """        
+    selected = np.where(p_values <= cutoff)[0]
+    prediction = np.array([0] * n_clusters)
+    prediction[selected] = 1
+    conf = confusion_matrix(beta_true, prediction)
+    tn, fp, fn, tp = conf.ravel()
+    if fp + tp == 0:
+        fdp = 0
+        tdp = 0
+    else:
+        fdp = fp/(fp+tp)
+        tdp = tp/np.sum(beta_true)
+
+    return fdp, tdp
+
+
+def compute_thr_family(fmri_input, alpha=0.05, k_max=1000,
+                       n_permutations=1000, n_jobs=1, seed=None):
+    
+    """Compute the calibrated threshold family.
+
+    Parameters
+    ----------
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
+    alpha : float
+        risk level
+    k_max : int
+        threshold families length
+    n_permutations : int
+        number of permutations in Notip procedure
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=1.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
+    
+    Returns
+    -------
+    thr_family : `np.ndarray` of shape (k_max,)
+        Calibrated threshold family.
+    """
+    if seed is None:
+        seed_ = None
+    else:
+        seed_ = seed + 1
+    
+    pval0 = sa.get_permuted_p_values_one_sample(fmri_input,
+                                                B=n_permutations,
+                                                n_jobs=n_jobs,
+                                                seed=seed)
+    learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
+                                                             B=n_permutations,
+                                                             n_jobs=n_jobs,
+                                                             seed=seed_)
+    learned_templates = np.sort(learned_templates_, axis=0)
+    
+    # Gain time by only considering credible families
+    learned_templates = learned_templates[:int(2*alpha*n_permutations)]
+
+    thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
+
+    return thr
+
+
+def get_clusters_table_TDP_1samp(fmri_input, stat_threshold=3,
+                                alpha=0.05,
+                                k_max=1000, n_permutations=1000, cluster_threshold=None,
+                                methods=['Notip'],
+                                nifti_masker=None,
+                                two_sided=False, min_distance=8.,
+                                cache_dir='./cachedir',
+                                n_jobs=2, seed=None):
     """Creates pandas dataframe with img cluster statistics.
+
     Parameters
     ----------
-    stat_img : Niimg-like object,
-       Statistical image (presumably in z- or p-scale).
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
     stat_threshold : `float`
         Cluster forming threshold in same scale as `stat_img` (either a
         p-value or z-scale value).
-    fmri_input : array of shape (n_subjects, p)
-        Masked fMRI data
-    learned_templates : array of shape (B_train, p)
-        sorted quantile curves computed on training data
     alpha : float
         risk level
     k_max : int
         threshold families length
-    B : int
-        number of permutations at inference step
+    n_permutations : int
+        number of permutations in Notip procedure
     cluster_threshold : `int` or `None`, optional
         Cluster size threshold, in voxels.
+    methods : `list` of `str`
+        List of methods to use for TDP lower bounds.
+        Options are: 'ARI', 'Notip'.
+    nifti_masker: `NiftiMasker` instance
+        NiftiMasker instance used to mask the data.
     two_sided : `bool`, optional
         Whether to employ two-sided thresholding or to evaluate positive values
         only. Default=False.
     min_distance : `float`, optional
         Minimum distance between subpeaks in mm. Default=8mm.
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=2.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
     Returns
     -------
     df : `pandas.DataFrame`
-        Table with peaks, subpeaks and estimated TDP using three methods
-        from thresholded `stat_img`. For binary clusters
-        (clusters with >1 voxel containing only one value), the table
-        reports the center of mass of the cluster,
-        rather than any peaks/subpeaks.
+        Table with peaks, subpeaks and TDP lower bound from thresholded `stat_img`.
+        For binary clusters, the table reports the center
+        of mass of the cluster, rather than any peaks/subpeaks.
     """
-    cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
-            'TDP (ARI)', 'TDP (Calibrated Simes)', 'TDP (Learned)']
     # Replace None with 0
     cluster_threshold = 0 if cluster_threshold is None else cluster_threshold
     # print(cluster_threshold)
     # check that stat_img is niimg-like object and 3D
+
+    # Let's run a one-sample t test on these data
+    stats_, p_values = stats.ttest_1samp(fmri_input, 0, alternative='greater')
+
+    stat_img = nifti_masker.inverse_transform(stats_)
     stat_img = check_niimg_3d(stat_img)
 
     stat_map_ = _safe_get_data(stat_img)
     # Perform calibration before thresholding
     stat_map_nonzero = stat_map_[stat_map_ != 0]
     hommel = _compute_hommel_value(stat_map_nonzero, alpha)
     ari_thr = sa.linear_template(alpha, hommel, hommel)
-    pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=B, seed=seed)
-    learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
+
+    location = cache_dir
+    memory = Memory(location, mmap_mode='r', verbose=0)
+    compute_thr_family_cached = memory.cache(compute_thr_family)
+    learned_thr = compute_thr_family_cached(fmri_input, alpha=alpha, 
+                                            k_max=k_max, n_permutations=n_permutations, 
+                                            n_jobs=n_jobs, seed=seed)
 
     # Apply threshold(s) to image
     stat_img = threshold_img(
         img=stat_img,
         threshold=stat_threshold,
         cluster_threshold=cluster_threshold,
         two_sided=two_sided,
@@ -645,15 +722,15 @@
         for c_id, c_val in enumerate(clust_ids):
             cluster_mask = label_map == c_val
             masked_data = temp_stat_map * cluster_mask
             masked_data_ = masked_data[masked_data != 0]
             # Compute TDP bounds on cluster using our 3 methods
             cluster_p_values = norm.sf(masked_data_)
             ari_tdp = sa.min_tdp(cluster_p_values, ari_thr)
-            simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
+            # simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
             learned_tdp = sa.min_tdp(cluster_p_values, learned_thr)
             cluster_size_mm = int(np.sum(cluster_mask) * voxel_size)
 
             # Get peaks, subpeaks and associated statistics
             subpeak_ijk, subpeak_vals = _local_max(
                 masked_data,
                 stat_img.affine,
@@ -670,113 +747,144 @@
             ).tolist()
             subpeak_xyz = np.array(subpeak_xyz).T
 
             # Only report peak and, at most, top 3 subpeaks.
             n_subpeaks = np.min((len(subpeak_vals), 4))
             for subpeak in range(n_subpeaks):
                 if subpeak == 0:
-                    row = [
-                        c_id + 1,
-                        subpeak_xyz[subpeak, 0],
-                        subpeak_xyz[subpeak, 1],
-                        subpeak_xyz[subpeak, 2],
-                        "{0:.2f}".format(subpeak_vals[subpeak]),
-                        cluster_size_mm,
-                        "{0:.2f}".format(ari_tdp),
-                        "{0:.2f}".format(simes_tdp),
-                        "{0:.2f}".format(learned_tdp),
-                    ]
+                        if methods == ['ARI', 'Notip']:
+                            cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
+                                    'TDP (ARI)', 'TDP (Notip)']
+                            row = [
+                                c_id + 1,
+                                subpeak_xyz[subpeak, 0],
+                                subpeak_xyz[subpeak, 1],
+                                subpeak_xyz[subpeak, 2],
+                                "{0:.2f}".format(subpeak_vals[subpeak]),
+                                cluster_size_mm,
+                                "{0:.2f}".format(ari_tdp),
+                                "{0:.2f}".format(learned_tdp)]
+                        else:
+                            cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
+                                    'TDP (Notip)']
+                            row = [
+                                c_id + 1,
+                                subpeak_xyz[subpeak, 0],
+                                subpeak_xyz[subpeak, 1],
+                                subpeak_xyz[subpeak, 2],
+                                "{0:.2f}".format(subpeak_vals[subpeak]),
+                                cluster_size_mm,
+                                "{0:.2f}".format(learned_tdp)]                           
+                                    
                 else:
                     # Subpeak naming convention is cluster num+letter:
                     # 1a, 1b, etc
                     sp_id = '{0}{1}'.format(
                         c_id + 1,
                         ascii_lowercase[subpeak - 1],
                     )
                     row = [
                         sp_id,
                         subpeak_xyz[subpeak, 0],
                         subpeak_xyz[subpeak, 1],
                         subpeak_xyz[subpeak, 2],
                         "{0:.2f}".format(subpeak_vals[subpeak]),
-                        '',
-                        '',
-                        '',
-                        '',
-                    ]
+                        '']
+                    
+                    row += [''] * len(methods)
+
                 rows += [row]
 
         # If we reach this point, there are clusters in this sign
         no_clusters_found = False
 
     if no_clusters_found:
         df = pd.DataFrame(columns=cols)
     else:
         df = pd.DataFrame(columns=cols, data=rows)
 
     return df
 
 
-def get_clusters_table_with_TDP(stat_img, fmri_input, stat_threshold=3,
+def get_clusters_table_TDP_2samp(fmri_input, y, stat_threshold=3,
                                 alpha=0.05,
                                 k_max=1000, n_permutations=1000, cluster_threshold=None,
                                 methods=['Notip'],
+                                nifti_masker=None,
                                 two_sided=False, min_distance=8., n_jobs=2, seed=None):
     """Creates pandas dataframe with img cluster statistics.
+
     Parameters
     ----------
-    stat_img : Niimg-like object,
-       Statistical image (presumably in z- or p-scale).
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
+    y : array of shape (n_subjects,)
+        Target variable
     stat_threshold : `float`
         Cluster forming threshold in same scale as `stat_img` (either a
         p-value or z-scale value).
-    fmri_input : array of shape (n_subjects, p)
-        Masked fMRI data
-    learned_templates : array of shape (B_train, p)
-        sorted quantile curves computed on training data
     alpha : float
         risk level
     k_max : int
         threshold families length
-    B : int
-        number of permutations at inference step
+    n_permutations : int
+        number of permutations in Notip procedure
     cluster_threshold : `int` or `None`, optional
         Cluster size threshold, in voxels.
+    methods : `list` of `str`
+        List of methods to use for TDP lower bounds.
+        Options are: 'ARI', 'Notip'.
+    nifti_masker: `NiftiMasker` instance
+        NiftiMasker instance used to mask the data.
     two_sided : `bool`, optional
         Whether to employ two-sided thresholding or to evaluate positive values
         only. Default=False.
     min_distance : `float`, optional
         Minimum distance between subpeaks in mm. Default=8mm.
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=2.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
     Returns
     -------
     df : `pandas.DataFrame`
-        Table with peaks, subpeaks and estimated TDP using three methods
-        from thresholded `stat_img`. For binary clusters
-        (clusters with >1 voxel containing only one value), the table
-        reports the center of mass of the cluster,
-        rather than any peaks/subpeaks.
+        Table with peaks, subpeaks and TDP lower bound from thresholded `stat_img`.
+        For binary clusters, the table reports the center
+        of mass of the cluster, rather than any peaks/subpeaks.
     """
     # Replace None with 0
     cluster_threshold = 0 if cluster_threshold is None else cluster_threshold
     # print(cluster_threshold)
     # check that stat_img is niimg-like object and 3D
+
+    # Let's run a one-sample t test on these data
+    two_samp_test = sa.row_welch_tests(fmri_input, y)
+    stats_, p_values = two_samp_test['statistic'], two_samp_test['p_value']
+
+    stat_img = nifti_masker.inverse_transform(stats_)
     stat_img = check_niimg_3d(stat_img)
 
     stat_map_ = _safe_get_data(stat_img)
     # Perform calibration before thresholding
     stat_map_nonzero = stat_map_[stat_map_ != 0]
     hommel = _compute_hommel_value(stat_map_nonzero, alpha)
     ari_thr = sa.linear_template(alpha, hommel, hommel)
-    pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=n_permutations, seed=seed)
-    learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
-                                                             B=n_permutations,
-                                                             n_jobs=n_jobs,
-                                                             seed=None)
+    
+    pval0 = sa.get_permuted_p_values(fmri_input, y,
+                                     B=n_permutations,
+                                     row_test_fun=row_welch_tests)
+    learned_templates_ = sa.get_permuted_p_values(fmri_input, y,
+                                                  B=n_permutations,
+                                                  row_test_fun=row_welch_tests)
     learned_templates = np.sort(learned_templates_, axis=0)
+    
+    # Gain time by only considering credible families
+    print(int(2*alpha*n_permutations))
+    learned_templates = learned_templates[:int(2*alpha*n_permutations)]
+
     learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
 
     # Apply threshold(s) to image
     stat_img = threshold_img(
         img=stat_img,
         threshold=stat_threshold,
         cluster_threshold=cluster_threshold,
@@ -827,15 +935,15 @@
         for c_id, c_val in enumerate(clust_ids):
             cluster_mask = label_map == c_val
             masked_data = temp_stat_map * cluster_mask
             masked_data_ = masked_data[masked_data != 0]
             # Compute TDP bounds on cluster using our 3 methods
             cluster_p_values = norm.sf(masked_data_)
             ari_tdp = sa.min_tdp(cluster_p_values, ari_thr)
-            simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
+            # simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
             learned_tdp = sa.min_tdp(cluster_p_values, learned_thr)
             cluster_size_mm = int(np.sum(cluster_mask) * voxel_size)
 
             # Get peaks, subpeaks and associated statistics
             subpeak_ijk, subpeak_vals = _local_max(
                 masked_data,
                 stat_img.affine,
@@ -906,98 +1014,219 @@
         df = pd.DataFrame(columns=cols)
     else:
         df = pd.DataFrame(columns=cols, data=rows)
 
     return df
 
 
-def get_tdp_bound_notip(stat_img, fmri_input, cluster_mask,
-                        alpha=0.05,
-                        k_max=1000, n_permutations=1000, cluster_threshold=None,
-                        two_sided=False, min_distance=8., n_jobs=2, seed=None):
+
+def get_clusters_table_TDP_paired(fmri_input, y, stat_threshold=3,
+                                alpha=0.05,
+                                k_max=1000, n_permutations=1000, cluster_threshold=None,
+                                methods=['Notip'],
+                                nifti_masker=None,
+                                two_sided=False, min_distance=8., 
+                                cache_dir='./cachedir',
+                                n_jobs=2, seed=None):
     """Creates pandas dataframe with img cluster statistics.
+
     Parameters
     ----------
-    stat_img : Niimg-like object,
-       Statistical image (presumably in z- or p-scale).
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
+    y : array of shape (n_subjects,)
+        Binary labels of the paired samples
     stat_threshold : `float`
         Cluster forming threshold in same scale as `stat_img` (either a
         p-value or z-scale value).
-    fmri_input : array of shape (n_subjects, p)
-        Masked fMRI data
-    learned_templates : array of shape (B_train, p)
-        sorted quantile curves computed on training data
     alpha : float
         risk level
     k_max : int
         threshold families length
-    B : int
-        number of permutations at inference step
+    n_permutations : int
+        number of permutations in Notip procedure
     cluster_threshold : `int` or `None`, optional
         Cluster size threshold, in voxels.
+    methods : `list` of `str`
+        List of methods to use for TDP lower bounds.
+        Options are: 'ARI', 'Notip'.
+    nifti_masker: `NiftiMasker` instance
+        NiftiMasker instance used to mask the data.
     two_sided : `bool`, optional
         Whether to employ two-sided thresholding or to evaluate positive values
         only. Default=False.
     min_distance : `float`, optional
         Minimum distance between subpeaks in mm. Default=8mm.
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=2.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
     Returns
     -------
     df : `pandas.DataFrame`
-        Table with peaks, subpeaks and estimated TDP using three methods
-        from thresholded `stat_img`. For binary clusters
-        (clusters with >1 voxel containing only one value), the table
-        reports the center of mass of the cluster,
-        rather than any peaks/subpeaks.
+        Table with peaks, subpeaks and TDP lower bound from thresholded `stat_img`.
+        For binary clusters, the table reports the center
+        of mass of the cluster, rather than any peaks/subpeaks.
+    """
+    
+    conds = np.unique(y)
+
+    input_difference = fmri_input[y == conds[1]] - fmri_input[y == conds[0]]
+
+
+    df = get_clusters_table_TDP_1samp(input_difference, stat_threshold=stat_threshold,
+                                alpha=alpha,
+                                k_max=k_max, n_permutations=n_permutations, cluster_threshold=cluster_threshold,
+                                methods=methods,
+                                nifti_masker=nifti_masker,
+                                two_sided=two_sided, min_distance=min_distance, 
+                                cache_dir=cache_dir, n_jobs=n_jobs, seed=seed)
+
+    return df
+
+
+def tdp_bound_notip_1samp(fmri_input, cluster_mask,
+                        alpha=0.05,
+                        k_max=1000, n_permutations=1000,
+                        nifti_masker=None,
+                        two_sided=False, min_distance=8.,
+                        cache_dir='./cachedir',
+                        n_jobs=2, seed=None):
+    """Computes TDP lower bound for a given cluster.
+
+    Parameters
+    ----------
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
+    cluster_mask : array of shape (p,)
+        Mask of the cluster
+    alpha : float
+        risk level
+    k_max : int
+        threshold families length
+    n_permutations : int
+        number of permutations in Notip procedure
+    nifti_masker: `NiftiMasker` instance
+        NiftiMasker instance used to mask the data.
+    two_sided : `bool`, optional
+        Whether to employ two-sided thresholding or to evaluate positive values
+        only. Default=False.
+    min_distance : `float`, optional
+        Minimum distance between subpeaks in mm. Default=8mm.
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=2.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
+    Returns
+    -------
+    learned_tdp : `float`
+        TDP lower bound for the cluster.
+    stat_img : `nibabel.Nifti1Image`
+        Statistical image of the cluster.
     """
     cols = ['Cluster ID', 'X', 'Y', 'Z', 'Peak Stat', 'Cluster Size (mm3)',
             'TDP (ARI)', 'TDP (Notip)']
-    # Replace None with 0
-    cluster_threshold = 0 if cluster_threshold is None else cluster_threshold
-    # print(cluster_threshold)
-    # check that stat_img is niimg-like object and 3D
+
+    # Let's run a one-sample t test on these data
+    stats_, p_values = stats.ttest_1samp(fmri_input, 0, alternative='greater')
+    stats_[np.where(np.isnan((p_values)))] = 0
+    p_values[np.where(np.isnan((p_values)))] = 1
+    
+    stat_img = nifti_masker.inverse_transform(stats_)
+    
     stat_img = check_niimg_3d(stat_img)
 
-    stat_map_ = _safe_get_data(stat_img)
-    # Perform calibration before thresholding
-    stat_map_nonzero = stat_map_[stat_map_ != 0]
-    hommel = _compute_hommel_value(stat_map_nonzero, alpha)
-    ari_thr = sa.linear_template(alpha, hommel, hommel)
-    pval0, simes_thr = calibrate_simes(fmri_input, alpha,
-                                       k_max=k_max, B=n_permutations, seed=seed)
-    learned_templates_ = sa.get_permuted_p_values_one_sample(fmri_input,
-                                                             B=n_permutations,
-                                                             n_jobs=n_jobs,
-                                                             seed=None)
-    learned_templates = np.sort(learned_templates_, axis=0)
-    learned_thr = sa.calibrate_jer(alpha, learned_templates, pval0, k_max)
+    # Perform calibration
+
+    location = cache_dir
+    memory = Memory(location, mmap_mode='r', verbose=0)
+    compute_thr_family_cached = memory.cache(compute_thr_family)
+    learned_thr = compute_thr_family_cached(fmri_input, alpha=alpha, 
+                                            k_max=k_max, n_permutations=n_permutations, 
+                                            n_jobs=n_jobs, seed=seed)
 
     # If cluster threshold is used, there is chance that stat_map will be
     # modified, therefore copy is needed
     stat_map = _safe_get_data(stat_img, ensure_finite=True)
                              
     voxel_size = np.prod(stat_img.header.get_zooms())
     no_clusters_found = True
     rows = []
 
-    masked_data = stat_map * cluster_mask
+    masked_data = stat_map * _safe_get_data(cluster_mask, ensure_finite=True)
     masked_data_ = masked_data[masked_data != 0]
     c_id = 0
     c_val = np.max(masked_data_)
             
-    # Compute TDP bounds on cluster using our 3 methods
+    # Compute TDP bounds on cluster using Notip
     cluster_p_values = norm.sf(masked_data_)
-    ari_tdp = sa.min_tdp(cluster_p_values, ari_thr)
-    simes_tdp = sa.min_tdp(cluster_p_values, simes_thr)
     learned_tdp = sa.min_tdp(cluster_p_values, learned_thr)
 
     stat_img_ = new_img_like(stat_img, masked_data)
 
     return learned_tdp, stat_img_
 
 
+def tdp_bound_notip_paired(fmri_input, y, cluster_mask,
+                        alpha=0.05,
+                        k_max=1000, n_permutations=1000,
+                        nifti_masker=None,
+                        two_sided=False, min_distance=8.,
+                        cache_dir='./cachedir', 
+                        n_jobs=2, seed=None):
+
+    """Computes TDP lower bound for a given cluster.
+
+    Parameters
+    ----------
+    fmri_input : array of shape (n_subjects, p)
+        Masked fMRI data
+    y : array of shape (n_subjects,)
+        Binary labels of the paired samples
+    cluster_mask : array of shape (p,)
+        Mask of the cluster
+    alpha : float
+        risk level
+    k_max : int
+        threshold families length
+    n_permutations : int
+        number of permutations in Notip procedure
+    nifti_masker: `NiftiMasker` instance
+        NiftiMasker instance used to mask the data.
+    two_sided : `bool`, optional
+        Whether to employ two-sided thresholding or to evaluate positive values
+        only. Default=False.
+    min_distance : `float`, optional
+        Minimum distance between subpeaks in mm. Default=8mm.
+    n_jobs : `int`, optional
+        Number of jobs to run in parallel. Default=2.
+    seed : `int` or None, optional
+        Seed for random number generator. Default=None.
+    Returns
+    -------
+    learned_tdp : `float`
+        TDP lower bound for the cluster.
+    stat_img : `nibabel.Nifti1Image`
+        Statistical image of the cluster.
+    """
+
+    conds = np.unique(y)
+
+    input_difference = fmri_input[y == conds[1]] - fmri_input[y == conds[0]]
+
+    learned_tdp, stat_img_ = tdp_bound_notip_1samp(input_difference, cluster_mask, alpha=alpha,
+                                                   k_max=k_max, n_permutations=n_permutations,
+                                                   nifti_masker=nifti_masker,
+                                                   two_sided=two_sided, min_distance=min_distance,
+                                                   cache_dir=cache_dir, n_jobs=n_jobs, seed=seed)
+    
+    return learned_tdp, stat_img_
+
+
+
 def _compute_hommel_value(z_vals, alpha, verbose=False):
     """Compute the All-Resolution Inference hommel-value"""
     if alpha < 0 or alpha > 1:
         raise ValueError('alpha should be between 0 and 1')
     z_vals_ = - np.sort(- z_vals)
     p_vals = norm.sf(z_vals_)
     n_samples = len(p_vals)
```

### Comparing `notip-0.1.4/notip.egg-info/PKG-INFO` & `notip-0.1.5/notip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.4/setup.py` & `notip-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = ["numpy>=1.15.0", "scipy>=1.0.0",
                 "joblib>=1.0.1", "scikit-learn>=0.22",
                 "nilearn","sanssouci","matplotlib",
                 "pandas", "joblib", "tqdm"]
 
 setup(
     name="notip",
-    version="0.1.4",
+    version="0.1.5",
     author="Alexandre Blain",
     author_email="alexandre.blain@inria.fr",
     description="Nonparametric True Discovery Proportion control for brain imaging",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/alexblnn/Notip",
     download_url="https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz",
```

