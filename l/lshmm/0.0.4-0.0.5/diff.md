# Comparing `tmp/lshmm-0.0.4.tar.gz` & `tmp/lshmm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lshmm-0.0.4.tar", last modified: Fri Sep 23 15:26:26 2022, max compression
+gzip compressed data, was "lshmm-0.0.5.tar", last modified: Fri Jul 21 13:05:21 2023, max compression
```

## Comparing `lshmm-0.0.4.tar` & `lshmm-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,27 @@
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.407888 lshmm-0.0.4/
--rw-r--r--   0 duncan     (503) staff       (20)     1070 2022-02-24 16:28:09.000000 lshmm-0.0.4/LICENSE
--rw-r--r--   0 duncan     (503) staff       (20)       34 2022-01-25 12:03:39.000000 lshmm-0.0.4/MANIFEST.in
--rw-r--r--   0 duncan     (503) staff       (20)      444 2022-09-23 15:26:26.408066 lshmm-0.0.4/PKG-INFO
--rw-r--r--   0 duncan     (503) staff       (20)       36 2022-02-24 14:37:53.000000 lshmm-0.0.4/README.md
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.383832 lshmm-0.0.4/lshmm/
--rw-r--r--   0 duncan     (503) staff       (20)      184 2022-09-13 14:30:24.000000 lshmm-0.0.4/lshmm/__init__.py
--rw-r--r--   0 duncan     (503) staff       (20)    10619 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/api.py
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.387282 lshmm-0.0.4/lshmm/forward_backward/
--rw-r--r--   0 duncan     (503) staff       (20)        0 2021-12-10 12:20:58.000000 lshmm-0.0.4/lshmm/forward_backward/__init__.py
--rw-r--r--   0 duncan     (503) staff       (20)    17324 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/forward_backward/fb_diploid_samples_variants.py
--rw-r--r--   0 duncan     (503) staff       (20)    17740 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/forward_backward/fb_diploid_variants_samples.py
--rw-r--r--   0 duncan     (503) staff       (20)     2506 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/forward_backward/fb_haploid_samples_variants.py
--rw-r--r--   0 duncan     (503) staff       (20)     2540 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/forward_backward/fb_haploid_variants_samples.py
--rw-r--r--   0 duncan     (503) staff       (20)      889 2022-09-23 15:23:27.000000 lshmm-0.0.4/lshmm/jit.py
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.390329 lshmm-0.0.4/lshmm/simulate/
--rw-r--r--   0 duncan     (503) staff       (20)        0 2021-12-10 12:20:13.000000 lshmm-0.0.4/lshmm/simulate/__init__.py
--rw-r--r--   0 duncan     (503) staff       (20)     4806 2022-01-29 16:57:43.000000 lshmm-0.0.4/lshmm/simulate/sim_samples_variants.py
--rw-r--r--   0 duncan     (503) staff       (20)     4802 2022-01-29 16:57:47.000000 lshmm-0.0.4/lshmm/simulate/sim_variants_samples.py
--rw-r--r--   0 duncan     (503) staff       (20)    13362 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/vit_diploid_samples_variants.py
--rw-r--r--   0 duncan     (503) staff       (20)    18342 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/vit_diploid_variants_samples.py
--rw-r--r--   0 duncan     (503) staff       (20)     7004 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/vit_haploid_samples_variants.py
--rw-r--r--   0 duncan     (503) staff       (20)     8730 2022-09-23 15:24:22.000000 lshmm-0.0.4/lshmm/vit_haploid_variants_samples.py
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.398311 lshmm-0.0.4/lshmm/viterbi/
--rw-r--r--   0 duncan     (503) staff       (20)        0 2022-06-17 14:32:33.000000 lshmm-0.0.4/lshmm/viterbi/__init__.py
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.407506 lshmm-0.0.4/lshmm.egg-info/
--rw-r--r--   0 duncan     (503) staff       (20)      444 2022-09-23 15:26:26.000000 lshmm-0.0.4/lshmm.egg-info/PKG-INFO
--rw-r--r--   0 duncan     (503) staff       (20)      916 2022-09-23 15:26:26.000000 lshmm-0.0.4/lshmm.egg-info/SOURCES.txt
--rw-r--r--   0 duncan     (503) staff       (20)        1 2022-09-23 15:26:26.000000 lshmm-0.0.4/lshmm.egg-info/dependency_links.txt
--rw-r--r--   0 duncan     (503) staff       (20)        6 2022-09-23 15:26:26.000000 lshmm-0.0.4/lshmm.egg-info/requires.txt
--rw-r--r--   0 duncan     (503) staff       (20)       12 2022-09-23 15:26:26.000000 lshmm-0.0.4/lshmm.egg-info/top_level.txt
--rw-r--r--   0 duncan     (503) staff       (20)      366 2022-09-13 14:30:24.000000 lshmm-0.0.4/pyproject.toml
--rw-r--r--   0 duncan     (503) staff       (20)      578 2022-09-23 15:26:26.408969 lshmm-0.0.4/setup.cfg
-drwxr-xr-x   0 duncan     (503) staff       (20)        0 2022-09-23 15:26:26.404449 lshmm-0.0.4/tests/
--rw-r--r--   0 duncan     (503) staff       (20)        0 2022-01-25 12:03:39.000000 lshmm-0.0.4/tests/__init__.py
--rw-r--r--   0 duncan     (503) staff       (20)    10020 2022-09-23 15:24:22.000000 lshmm-0.0.4/tests/test_API.py
--rw-r--r--   0 duncan     (503) staff       (20)     7601 2022-09-23 15:24:22.000000 lshmm-0.0.4/tests/test_API_multiallelic.py
--rw-r--r--   0 duncan     (503) staff       (20)    39304 2022-09-23 15:24:22.000000 lshmm-0.0.4/tests/test_LS_haploid_diploid.py
+drwxr-xr-x   0 duncan     (503) staff       (20)        0 2023-07-21 13:05:21.354895 lshmm-0.0.5/
+-rw-r--r--   0 duncan     (503) staff       (20)     1070 2023-07-21 12:11:03.000000 lshmm-0.0.5/LICENSE
+-rw-r--r--   0 duncan     (503) staff       (20)       34 2023-07-21 12:11:03.000000 lshmm-0.0.5/MANIFEST.in
+-rw-r--r--   0 duncan     (503) staff       (20)      444 2023-07-21 13:05:21.355105 lshmm-0.0.5/PKG-INFO
+-rw-r--r--   0 duncan     (503) staff       (20)       36 2023-07-21 12:11:03.000000 lshmm-0.0.5/README.md
+drwxr-xr-x   0 duncan     (503) staff       (20)        0 2023-07-21 13:05:21.346059 lshmm-0.0.5/lshmm/
+-rw-r--r--   0 duncan     (503) staff       (20)      184 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/__init__.py
+-rw-r--r--   0 duncan     (503) staff       (20)    11724 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/api.py
+drwxr-xr-x   0 duncan     (503) staff       (20)        0 2023-07-21 13:05:21.351850 lshmm-0.0.5/lshmm/forward_backward/
+-rw-r--r--   0 duncan     (503) staff       (20)        0 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/forward_backward/__init__.py
+-rw-r--r--   0 duncan     (503) staff       (20)    17740 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/forward_backward/fb_diploid.py
+-rw-r--r--   0 duncan     (503) staff       (20)     2510 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/forward_backward/fb_haploid.py
+-rw-r--r--   0 duncan     (503) staff       (20)      881 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/jit.py
+-rw-r--r--   0 duncan     (503) staff       (20)    18343 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/vit_diploid.py
+-rw-r--r--   0 duncan     (503) staff       (20)     8732 2023-07-21 12:11:03.000000 lshmm-0.0.5/lshmm/vit_haploid.py
+drwxr-xr-x   0 duncan     (503) staff       (20)        0 2023-07-21 13:05:21.350123 lshmm-0.0.5/lshmm.egg-info/
+-rw-r--r--   0 duncan     (503) staff       (20)      444 2023-07-21 13:05:21.000000 lshmm-0.0.5/lshmm.egg-info/PKG-INFO
+-rw-r--r--   0 duncan     (503) staff       (20)      475 2023-07-21 13:05:21.000000 lshmm-0.0.5/lshmm.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan     (503) staff       (20)        1 2023-07-21 13:05:21.000000 lshmm-0.0.5/lshmm.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan     (503) staff       (20)        6 2023-07-21 13:05:21.000000 lshmm-0.0.5/lshmm.egg-info/requires.txt
+-rw-r--r--   0 duncan     (503) staff       (20)        6 2023-07-21 13:05:21.000000 lshmm-0.0.5/lshmm.egg-info/top_level.txt
+-rw-r--r--   0 duncan     (503) staff       (20)      366 2023-07-21 12:11:03.000000 lshmm-0.0.5/pyproject.toml
+-rw-r--r--   0 duncan     (503) staff       (20)      585 2023-07-21 13:05:21.356677 lshmm-0.0.5/setup.cfg
+drwxr-xr-x   0 duncan     (503) staff       (20)        0 2023-07-21 13:05:21.354268 lshmm-0.0.5/tests/
+-rw-r--r--   0 duncan     (503) staff       (20)     9884 2023-07-21 12:11:03.000000 lshmm-0.0.5/tests/test_API.py
+-rw-r--r--   0 duncan     (503) staff       (20)     7493 2023-07-21 12:11:03.000000 lshmm-0.0.5/tests/test_API_multiallelic.py
+-rw-r--r--   0 duncan     (503) staff       (20)    23884 2023-07-21 12:11:03.000000 lshmm-0.0.5/tests/test_LS_haploid_diploid.py
```

### Comparing `lshmm-0.0.4/LICENSE` & `lshmm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lshmm-0.0.4/lshmm/api.py` & `lshmm-0.0.5/lshmm/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """External API definitions."""
 import warnings
 
 import numpy as np
 
-from .forward_backward.fb_diploid_variants_samples import (
-    backward_ls_dip_loop,
-    forward_ls_dip_loop,
-)
-from .forward_backward.fb_haploid_variants_samples import (
-    backwards_ls_hap,
-    forwards_ls_hap,
-)
-from .vit_diploid_variants_samples import (
+from .forward_backward.fb_diploid import backward_ls_dip_loop, forward_ls_dip_loop
+from .forward_backward.fb_haploid import backwards_ls_hap, forwards_ls_hap
+from .vit_diploid import (
     backwards_viterbi_dip,
     forwards_viterbi_dip_low_mem,
     get_phased_path,
     path_ll_dip,
 )
-from .vit_haploid_variants_samples import (
+from .vit_haploid import (
     backwards_viterbi_hap,
     forwards_viterbi_hap_lower_mem_rescaling,
     path_ll_hap,
 )
 
 EQUAL_BOTH_HOM = 4
 UNEQUAL_BOTH_HOM = 0
@@ -47,74 +41,95 @@
     n_alleles = np.int8([(len(alleles_site)) for alleles_site in alleles])
     return n_alleles
 
 
 def checks(
     reference_panel,
     query,
-    mutation_rate,
-    recombination_rate,
+    p_mutation,
+    p_recombination,
     scale_mutation_based_on_n_alleles,
 ):
+    """
+    Checks that the input data and parameters are valid.
 
-    ref_shape = reference_panel.shape
-    ploidy = len(ref_shape) - 1
+    The reference panel must be a matrix of size (m, n) or (m, n, n).
+    The query must be a matrix of size (k, m) or (k, m, 2).
 
-    if ploidy not in (1, 2):
-        raise ValueError("Ploidy not supported.")
+    m = number of sites.
+    n = number of samples in the reference panel (haplotypes, not individuals).
+    k = number of samples in the query (haplotypes, not individuals).
+
+    :param numpy.ndarray(dtype=int) reference_panel: Matrix of size (m, n) or (m, n, n).
+    :param numpy.ndarray(dtype=int) query: Matrix of size (k, m) or (k, m, 2).
+    :param numpy.ndarray(dtype=float) p_mutation: Scalar or vector of length m.
+    :param numpy.ndarray(dtype=float) p_recombination: Scalar or vector of length m.
+    :param bool scale_mutation_based_on_n_alleles: Whether to scale the mutation probability to the set of alleles that can be mutated to based on the number of alleles (True) or not (False).
+    :return: n, m, ploidy
+    :rtype: tuple
+    """
+    # Check reference panel
+    if not len(reference_panel.shape) in (2, 3):
+        raise ValueError("Reference panel array must have 2 or 3 dimensions.")
+
+    if len(reference_panel.shape) == 2:
+        m, n = reference_panel.shape
+        ploidy = 1
+    else:
+        m, n, _ = reference_panel.shape
+        ploidy = 2
 
-    if not (query.shape[1] == ref_shape[0]):
+    if ploidy == 2 and (reference_panel.shape[1] != reference_panel.shape[2]):
         raise ValueError(
-            "Number of variants in query does not match reference_panel. If haploid, ensure variant x sample matrices are passed."
+            "Reference_panel dimensions are incorrect, perhaps a sample x sample x variant matrix was passed. Expected sites x samples x samples."
         )
 
-    if (ploidy == 2) and (not (ref_shape[1] == ref_shape[2])):
+    # Check query sequence(s)
+    if query.shape[1] != m:
         raise ValueError(
-            "reference_panel dimensions incorrect, perhaps a sample x sample x variant matrix was passed. Expected variant x sample x sample."
+            "Number of sites in query does not match reference panel. If haploid, ensure a sites x samples matrix is passed."
         )
 
-    m = ref_shape[0]
-    n = ref_shape[1]
-
-    # Ensure that the mutation rate is either a scalar or vector of length m
-    if not isinstance(mutation_rate, float) and (mutation_rate is not None):
-        if type(mutation_rate is np.ndarray):
-            if mutation_rate.shape[0] is not m:
-                raise ValueError(
-                    f"mutation_rate is not a scalar or vector of length m: {m}"
-                )
-        else:
-            raise ValueError(
-                f"mutation_rate is not a scalar or vector of length m: {m}"
+    # Ensure that the mutation probability is either a scalar or vector of length m
+    if isinstance(p_mutation, (int, float)):
+        if not scale_mutation_based_on_n_alleles:
+            warnings.warn(
+                "Passed a scalar probability of mutation, but not rescaling this probability of mutation conditional on the number of alleles at the site."
             )
-
-    # Ensure that the recombination probabilities is either a scalar or a vector of length m
-    if recombination_rate.shape[0] is not m:
-        raise ValueError(f"recombination_rate is not a vector of length m: {m}")
-
-    if isinstance(mutation_rate, float) and not (scale_mutation_based_on_n_alleles):
+    elif isinstance(p_mutation, np.ndarray) and p_mutation.shape[0] == m:
+        if scale_mutation_based_on_n_alleles:
+            warnings.warn(
+                "Passed a vector of probabilities of mutation, but rescaling each mutation probability conditional on the number of alleles at each site."
+            )
+    elif p_mutation is None:
         warnings.warn(
-            "Passed a scalar mutation rate, but not rescaling this mutation rate conditional on the number of alleles at the site"
+            "No mutation probability passed, setting mutation probability based on Li and Stephens 2003, equations (A2) and (A3)"
         )
-
-    if type(mutation_rate is np.ndarray) and (scale_mutation_based_on_n_alleles):
-        warnings.warn(
-            "Passed a vector of mutation rates, but rescaling each mutation rate conditional on the number of alleles at each site"
+    else:
+        raise ValueError(
+            f"Mutation probability is not None, a scalar, or vector of length m: {m}"
         )
 
-    return n, m, ploidy
+    # Ensure that the recombination probability is either a scalar or a vector of length m
+    if not (
+        isinstance(p_recombination, (int, float))
+        or (isinstance(p_recombination, np.ndarray) and p_recombination.shape[0] == m)
+    ):
+        raise ValueError(f"p_Recombination is not a scalar or vector of length m: {m}")
+
+    return (n, m, ploidy)
 
 
 def set_emission_probabilities(
     n,
     m,
     reference_panel,
     query,
     alleles,
-    mutation_rate,
+    p_mutation,
     ploidy,
     scale_mutation_based_on_n_alleles,
 ):
     # Check alleles should go in here, and modify e before passing to the algorithm
     # If alleles is not passed, we don't perform a test of alleles, but set n_alleles based on the reference_panel.
     if alleles is None:
         n_alleles = np.int8(
@@ -122,156 +137,157 @@
                 len(np.unique(np.append(reference_panel[j, :], query[:, j])))
                 for j in range(reference_panel.shape[0])
             ]
         )
     else:
         n_alleles = check_alleles(alleles, m)
 
-    if mutation_rate is None:
-        # Set the mutation rate to be the proposed mutation rate in Li and Stephens (2003).
+    if p_mutation is None:
+        # Set the mutation probability to be the proposed mutation probability in Li and Stephens (2003).
         theta_tilde = 1 / np.sum([1 / k for k in range(1, n - 1)])
-        mutation_rate = 0.5 * (theta_tilde / (n + theta_tilde))
+        p_mutation = 0.5 * (theta_tilde / (n + theta_tilde))
 
-    if isinstance(mutation_rate, float):
-        mutation_rate = mutation_rate * np.ones(m)
+    if isinstance(p_mutation, float):
+        p_mutation = p_mutation * np.ones(m)
 
     if ploidy == 1:
         # Haploid
-        # Evaluate emission probabilities here, using the mutation rate - this can take a scalar or vector.
+        # Evaluate emission probabilities here using p_mutation - this can take a scalar or vector.
         e = np.zeros((m, 2))
 
         if scale_mutation_based_on_n_alleles:
-            # Scale mutation based on the number of alleles - so the mutation rate is the mutation rate to one of the alleles.
-            # The overall mutation rate is then (n_alleles - 1) * mutation_rate.
-            e[:, 0] = mutation_rate - mutation_rate * np.equal(
+            # Scale mutation based on the number of alleles - so p_mutation is probability of mutation any given one of the alleles.
+            # The overall mutation probability is then (n_alleles - 1) * p_mutation.
+            e[:, 0] = p_mutation - p_mutation * np.equal(
                 n_alleles, np.ones(m)
             )  # Added boolean in case we're at an invariant site
-            e[:, 1] = 1 - (n_alleles - 1) * mutation_rate
+            e[:, 1] = 1 - (n_alleles - 1) * p_mutation
         else:
-            # No scaling based on the number of alleles - so the mutation rate is the mutation rate to anything.
-            # Which means that we must rescale the mutation rate to a different allele, by the number of alleles.
+            # No scaling based on the number of alleles - so p_mutation is the probability of mutation to anything
+            # (summing over the states we can switch to). This means that we must rescale the probability of mutation to
+            # a different allele by the number of alleles at the site.
             for j in range(m):
                 if n_alleles[j] == 1:  # In case we're at an invariant site
                     e[j, 0] = 0
                     e[j, 1] = 1
                 else:
-                    e[j, 0] = mutation_rate[j] / (n_alleles[j] - 1)
-                    e[j, 1] = 1 - mutation_rate[j]
+                    e[j, 0] = p_mutation[j] / (n_alleles[j] - 1)
+                    e[j, 1] = 1 - p_mutation[j]
     else:
         # Diploid
-        # Evaluate emission probabilities here, using the mutation rate - this can take a scalar or vector.
+        # Evaluate emission probabilities here, using the mutation probability - this can take a scalar or vector.
         # DEV: there's a wrinkle here.
         e = np.zeros((m, 8))
-        e[:, EQUAL_BOTH_HOM] = (1 - mutation_rate) ** 2
-        e[:, UNEQUAL_BOTH_HOM] = mutation_rate ** 2
-        e[:, BOTH_HET] = (1 - mutation_rate) ** 2 + mutation_rate ** 2
-        e[:, REF_HOM_OBS_HET] = 2 * mutation_rate * (1 - mutation_rate)
-        e[:, REF_HET_OBS_HOM] = mutation_rate * (1 - mutation_rate)
+        e[:, EQUAL_BOTH_HOM] = (1 - p_mutation) ** 2
+        e[:, UNEQUAL_BOTH_HOM] = p_mutation ** 2
+        e[:, BOTH_HET] = (1 - p_mutation) ** 2 + p_mutation ** 2
+        e[:, REF_HOM_OBS_HET] = 2 * p_mutation * (1 - p_mutation)
+        e[:, REF_HET_OBS_HOM] = p_mutation * (1 - p_mutation)
         e[:, MISSING_INDEX] = 1
 
     return e
 
 
-def viterbi_hap(n, m, reference_panel, query, emissions, recombination_rate):
+def viterbi_hap(n, m, reference_panel, query, emissions, p_recombination):
 
     V, P, log_likelihood = forwards_viterbi_hap_lower_mem_rescaling(
-        n, m, reference_panel, query, emissions, recombination_rate
+        n, m, reference_panel, query, emissions, p_recombination
     )
     most_likely_path = backwards_viterbi_hap(m, V, P)
 
     return most_likely_path, log_likelihood
 
 
-def viterbi_dip(n, m, reference_panel, query, emissions, recombination_rate):
+def viterbi_dip(n, m, reference_panel, query, emissions, p_recombination):
 
     V, P, log_likelihood = forwards_viterbi_dip_low_mem(
-        n, m, reference_panel, query, emissions, recombination_rate
+        n, m, reference_panel, query, emissions, p_recombination
     )
     unphased_path = backwards_viterbi_dip(m, V, P)
     most_likely_path = get_phased_path(n, unphased_path)
 
     return most_likely_path, log_likelihood
 
 
 def forwards(
     reference_panel,
     query,
-    recombination_rate,
+    p_recombination,
     alleles=None,
-    mutation_rate=None,
+    p_mutation=None,
     scale_mutation_based_on_n_alleles=True,
+    norm=True,
 ):
     """
     Run the Li and Stephens forwards algorithm on haplotype or
     unphased genotype data.
     """
-
     n, m, ploidy = checks(
         reference_panel,
         query,
-        mutation_rate,
-        recombination_rate,
+        p_mutation,
+        p_recombination,
         scale_mutation_based_on_n_alleles,
     )
 
     emissions = set_emission_probabilities(
         n,
         m,
         reference_panel,
         query,
         alleles,
-        mutation_rate,
+        p_mutation,
         ploidy,
         scale_mutation_based_on_n_alleles,
     )
 
     if ploidy == 1:
         forward_function = forwards_ls_hap
     else:
         forward_function = forward_ls_dip_loop
 
     (
         forward_array,
         normalisation_factor_from_forward,
         log_likelihood,
     ) = forward_function(
-        n, m, reference_panel, query, emissions, recombination_rate, norm=True
+        n, m, reference_panel, query, emissions, p_recombination, norm=norm
     )
 
     return forward_array, normalisation_factor_from_forward, log_likelihood
 
 
 def backwards(
     reference_panel,
     query,
     normalisation_factor_from_forward,
-    recombination_rate,
+    p_recombination,
     alleles=None,
-    mutation_rate=None,
+    p_mutation=None,
     scale_mutation_based_on_n_alleles=True,
 ):
     """
     Run the Li and Stephens backwards algorithm on haplotype or
     unphased genotype data.
     """
     n, m, ploidy = checks(
         reference_panel,
         query,
-        mutation_rate,
-        recombination_rate,
+        p_mutation,
+        p_recombination,
         scale_mutation_based_on_n_alleles,
     )
 
     emissions = set_emission_probabilities(
         n,
         m,
         reference_panel,
         query,
         alleles,
-        mutation_rate,
+        p_mutation,
         ploidy,
         scale_mutation_based_on_n_alleles,
     )
 
     if ploidy == 1:
         backward_function = backwards_ls_hap
     else:
@@ -280,95 +296,95 @@
     backwards_array = backward_function(
         n,
         m,
         reference_panel,
         query,
         emissions,
         normalisation_factor_from_forward,
-        recombination_rate,
+        p_recombination,
     )
 
     return backwards_array
 
 
 def viterbi(
     reference_panel,
     query,
-    recombination_rate,
+    p_recombination,
     alleles=None,
-    mutation_rate=None,
+    p_mutation=None,
     scale_mutation_based_on_n_alleles=True,
 ):
     """
     Run the Li and Stephens Viterbi algorithm on haplotype or
     unphased genotype data.
     """
     n, m, ploidy = checks(
         reference_panel,
         query,
-        mutation_rate,
-        recombination_rate,
+        p_mutation,
+        p_recombination,
         scale_mutation_based_on_n_alleles,
     )
 
     emissions = set_emission_probabilities(
         n,
         m,
         reference_panel,
         query,
         alleles,
-        mutation_rate,
+        p_mutation,
         ploidy,
         scale_mutation_based_on_n_alleles,
     )
 
     if ploidy == 1:
         viterbi_function = viterbi_hap
     else:
         viterbi_function = viterbi_dip
 
     most_likely_path, log_likelihood = viterbi_function(
-        n, m, reference_panel, query, emissions, recombination_rate
+        n, m, reference_panel, query, emissions, p_recombination
     )
 
     return most_likely_path, log_likelihood
 
 
 def path_ll(
     reference_panel,
     query,
     path,
-    recombination_rate,
+    p_recombination,
     alleles=None,
-    mutation_rate=None,
+    p_mutation=None,
     scale_mutation_based_on_n_alleles=True,
 ):
 
     n, m, ploidy = checks(
         reference_panel,
         query,
-        mutation_rate,
-        recombination_rate,
+        p_mutation,
+        p_recombination,
         scale_mutation_based_on_n_alleles,
     )
 
     emissions = set_emission_probabilities(
         n,
         m,
         reference_panel,
         query,
         alleles,
-        mutation_rate,
+        p_mutation,
         ploidy,
         scale_mutation_based_on_n_alleles,
     )
 
     if ploidy == 1:
         path_ll_function = path_ll_hap
     else:
         path_ll_function = path_ll_dip
 
     ll = path_ll_function(
-        n, m, reference_panel, path, query, emissions, recombination_rate
+        n, m, reference_panel, path, query, emissions, p_recombination
     )
 
     return ll
```

### Comparing `lshmm-0.0.4/lshmm/forward_backward/fb_diploid_samples_variants.py` & `lshmm-0.0.5/lshmm/forward_backward/fb_diploid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Collection of functions to run forwards and backwards algorithms
-on diploid genotype data, where the data is structured as samples x
-variants.
-"""
+"""Collection of functions to run forwards and backwards algorithms on haploid genotype data, where the data is structured as variants x samples."""
 import numpy as np
 
 from lshmm import jit
 
 EQUAL_BOTH_HOM = 4
 UNEQUAL_BOTH_HOM = 0
 BOTH_HET = 7
@@ -47,368 +43,369 @@
 
 @jit.numba_njit
 def np_argmax(array, axis):
     """Numba implementation of numpy vectorised argmax."""
     return np_apply_along_axis(np.argmax, axis, array)
 
 
-@jit.numba_njit
 def forwards_ls_dip(n, m, G, s, e, r, norm=True):
     """Matrix based diploid LS forward algorithm using numpy vectorisation."""
     # Initialise the forward tensor
-    F = np.zeros((n, n, m))
-    F[:, :, 0] = 1 / (n ** 2)
+    F = np.zeros((m, n, n))
+    F[0, :, :] = 1 / (n ** 2)
     c = np.ones(m)
     r_n = r / n
 
     if s[0, 0] == MISSING:
         index = MISSING_INDEX * np.ones(
             (n, n), dtype=np.int64
         )  # We could have chosen anything here, this just implies a multiplication by a constant.
     else:
-        index = 4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64) + 2 * (
-            G[:, :, 0] == 1
+        index = 4 * np.equal(G[0, :, :], s[0, 0]).astype(np.int64) + 2 * (
+            G[0, :, :] == 1
         ).astype(np.int64)
         if s[0, 0] == 1:
             index += 1
 
-    F[:, :, 0] *= e[index.ravel(), 0].reshape(n, n)
+    F[0, :, :] *= e[0, index]
 
     if norm:
-        c[0] = np.sum(F[:, :, 0])
-        F[:, :, 0] *= 1 / c[0]
+        c[0] = np.sum(F[0, :, :])
+        F[0, :, :] *= 1 / c[0]
 
         # Forwards
         for l in range(1, m):
             if s[0, l] == MISSING:
                 index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
             else:
-                index = 4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64) + 2 * (
-                    G[:, :, l] == 1
+                index = 4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64) + 2 * (
+                    G[l, :, :] == 1
                 ).astype(np.int64)
 
                 if s[0, l] == 1:
                     index += 1
 
             # No change in both
-            F[:, :, l] = (1 - r[l]) ** 2 * F[:, :, l - 1]
+            F[l, :, :] = (1 - r[l]) ** 2 * F[l - 1, :, :]
 
             # Both change
-            F[:, :, l] += (r_n[l]) ** 2
+            F[l, :, :] += (r_n[l]) ** 2
 
             # One changes
-            sum_j = np_sum(F[:, :, l - 1], 0).repeat(n).reshape((-1, n))
-            F[:, :, l] += ((1 - r[l]) * r_n[l]) * (sum_j + sum_j.T)
+            sum_j = np_sum(F[l - 1, :, :], 0).repeat(n).reshape((-1, n)).T
+            F[l, :, :] += ((1 - r[l]) * r_n[l]) * (sum_j + sum_j.T)
 
             # Emission
-            F[:, :, l] *= e[index.ravel(), l].reshape(n, n)
-            c[l] = np.sum(F[:, :, l])
-            F[:, :, l] *= 1 / c[l]
+            F[l, :, :] *= e[l, index]
+            c[l] = np.sum(F[l, :, :])
+            F[l, :, :] *= 1 / c[l]
 
         ll = np.sum(np.log10(c))
     else:
         # Forwards
         for l in range(1, m):
             if s[0, l] == MISSING:
-                index = MISSING_INDEX * np.ones((n, n)).astype(np.int64)
+                index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
             else:
-                index = 4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64) + 2 * (
-                    G[:, :, l] == 1
+                index = 4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64) + 2 * (
+                    G[l, :, :] == 1
                 ).astype(np.int64)
 
                 if s[0, l] == 1:
                     index += 1
 
             # No change in both
-            F[:, :, l] = (1 - r[l]) ** 2 * F[:, :, l - 1]
+            F[l, :, :] = (1 - r[l]) ** 2 * F[l - 1, :, :]
 
             # Both change
-            F[:, :, l] += (r_n[l]) ** 2 * np.sum(F[:, :, l - 1])
+            F[l, :, :] += (r_n[l]) ** 2 * np.sum(F[l - 1, :, :])
 
             # One changes
-            sum_j = np_sum(F[:, :, l - 1], 0).repeat(n).reshape((-1, n)).T
-            F[:, :, l] += ((1 - r[l]) * r_n[l]) * (sum_j + sum_j.T)
+            sum_j = np_sum(F[l - 1, :, :], 0).repeat(n).reshape((-1, n)).T
+            # sum_j2 = np_sum(F[l - 1, :, :], 1).repeat(n).reshape((-1, n))
+            F[l, :, :] += ((1 - r[l]) * r_n[l]) * (sum_j + sum_j.T)
 
             # Emission
-            F[:, :, l] *= e[index.ravel(), l].reshape(n, n)
+            F[l, :, :] *= e[l, index]
 
-        ll = np.log10(np.sum(F[:, :, l]))
+        ll = np.log10(np.sum(F[l, :, :]))
 
     return F, c, ll
 
 
-@jit.numba_njit
 def backwards_ls_dip(n, m, G, s, e, c, r):
     """Matrix based diploid LS backward algorithm using numpy vectorisation."""
     # Initialise the backward tensor
-    B = np.zeros((n, n, m))
+    B = np.zeros((m, n, n))
 
     # Initialise
-    B[:, :, m - 1] = 1
+    B[m - 1, :, :] = 1
     r_n = r / n
 
     # Backwards
     for l in range(m - 2, -1, -1):
 
         if s[0, l + 1] == MISSING:
-            index = MISSING_INDEX * np.ones((n, n), dtype=np.int64).ravel()
+            index = MISSING_INDEX * np.ones(
+                (n, n), dtype=np.int64
+            )  # We could have chosen anything here, this just implies a multiplication by a constant.
         else:
             index = (
-                4 * np.equal(G[:, :, l + 1], s[0, l + 1]).astype(np.int64)
-                + 2 * (G[:, :, l + 1] == 1).astype(np.int64)
+                4 * np.equal(G[l + 1, :, :], s[0, l + 1]).astype(np.int64)
+                + 2 * (G[l + 1, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l + 1] == 1)
-            ).ravel()
-
-        # Both change
-        B[:, :, l] = r_n[l + 1] ** 2 * np.sum(
-            e[index, l + 1].reshape(n, n) * B[:, :, l + 1]
-        )
+            )
 
         # No change in both
-        B[:, :, l] += (
-            (1 - r[l + 1]) ** 2 * B[:, :, l + 1] * e[index, l + 1].reshape(n, n)
+        B[l, :, :] = r_n[l + 1] ** 2 * np.sum(
+            e[l + 1, index.reshape((n, n))] * B[l + 1, :, :]
         )
 
-        sum_j = (
-            np_sum(B[:, :, l + 1] * e[index, l + 1].reshape(n, n), 0)
-            .repeat(n)
-            .reshape((-1, n))
+        # Both change
+        B[l, :, :] += (
+            (1 - r[l + 1]) ** 2 * B[l + 1, :, :] * e[l + 1, index.reshape((n, n))]
         )
-        B[:, :, l] += ((1 - r[l + 1]) * r_n[l + 1]) * (sum_j + sum_j.T)
-        B[:, :, l] *= 1 / c[l + 1]
+
+        # One changes
+        sum_j = np_sum(B[l + 1, :, :] * e[l + 1, index], 0).repeat(n).reshape((-1, n))
+        B[l, :, :] += ((1 - r[l + 1]) * r_n[l + 1]) * (sum_j + sum_j.T)
+        B[l, :, :] *= 1 / c[l + 1]
 
     return B
 
 
 @jit.numba_njit
 def forward_ls_dip_starting_point(n, m, G, s, e, r):
     """Naive implementation of LS diploid forwards algorithm."""
     # Initialise the forward tensor
-    F = np.zeros((n, n, m))
-    F[:, :, 0] = 1 / (n ** 2)
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64).ravel()
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        ).ravel()
-
-    F[:, :, 0] *= e[index, 0].reshape((n, n))
+    F = np.zeros((m, n, n))
     r_n = r / n
+    for j1 in range(n):
+        for j2 in range(n):
+            F[0, j1, j2] = 1 / (n ** 2)
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            F[0, j1, j2] *= e[0, index_tmp]
 
     for l in range(1, m):
 
         # Determine the various components
         F_no_change = np.zeros((n, n))
         F_j1_change = np.zeros(n)
         F_j2_change = np.zeros(n)
         F_both_change = 0
 
         for j1 in range(n):
             for j2 in range(n):
-                F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[j1, j2, l - 1]
+                F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[l - 1, j1, j2]
 
         for j1 in range(n):
             for j2 in range(n):
-                F_both_change += r_n[l] ** 2 * F[j1, j2, l - 1]
+                F_both_change += r_n[l] ** 2 * F[l - 1, j1, j2]
 
         for j1 in range(n):
             for j2 in range(n):  # This is the variable to sum over - it changes
-                F_j2_change[j1] += (1 - r[l]) * r_n[l] * F[j1, j2, l - 1]
+                F_j2_change[j1] += (1 - r[l]) * r_n[l] * F[l - 1, j1, j2]
 
         for j2 in range(n):
             for j1 in range(n):  # This is the variable to sum over - it changes
-                F_j1_change[j2] += (1 - r[l]) * r_n[l] * F[j1, j2, l - 1]
+                F_j1_change[j2] += (1 - r[l]) * r_n[l] * F[l - 1, j1, j2]
 
-        F[:, :, l] = F_both_change
+        F[l, :, :] = F_both_change
 
         for j1 in range(n):
-            F[j1, :, l] += F_j2_change
+            F[l, j1, :] += F_j2_change
 
         for j2 in range(n):
-            F[:, j2, l] += F_j1_change
+            F[l, :, j2] += F_j1_change
 
         for j1 in range(n):
             for j2 in range(n):
-                F[j1, j2, l] += F_no_change[j1, j2]
+                F[l, j1, j2] += F_no_change[j1, j2]
 
-        if s[0, l] == MISSING:
-            F[:, :, l] *= e[MISSING_INDEX, l]
-        else:
-            for j1 in range(n):
-                for j2 in range(n):
-                    # What is the emission?
+        for j1 in range(n):
+            for j2 in range(n):
+                # What is the emission?
+                if s[0, l] == MISSING:
+                    F[l, j1, j2] *= e[l, MISSING_INDEX]
+                else:
                     if s[0, l] == 1:
                         # OBS is het
-                        if G[j1, j2, l] == 1:  # REF is het
-                            F[j1, j2, l] *= e[BOTH_HET, l]
+                        if G[l, j1, j2] == 1:  # REF is het
+                            F[l, j1, j2] *= e[l, BOTH_HET]
                         else:  # REF is hom
-                            F[j1, j2, l] *= e[REF_HOM_OBS_HET, l]
+                            F[l, j1, j2] *= e[l, REF_HOM_OBS_HET]
                     else:
                         # OBS is hom
-                        if G[j1, j2, l] == 1:  # REF is het
-                            F[j1, j2, l] *= e[REF_HET_OBS_HOM, l]
+                        if G[l, j1, j2] == 1:  # REF is het
+                            F[l, j1, j2] *= e[l, REF_HET_OBS_HOM]
                         else:  # REF is hom
-                            if G[j1, j2, l] == s[0, l]:  # Equal
-                                F[j1, j2, l] *= e[EQUAL_BOTH_HOM, l]
+                            if G[l, j1, j2] == s[0, l]:  # Equal
+                                F[l, j1, j2] *= e[l, EQUAL_BOTH_HOM]
                             else:  # Unequal
-                                F[j1, j2, l] *= e[UNEQUAL_BOTH_HOM, l]
+                                F[l, j1, j2] *= e[l, UNEQUAL_BOTH_HOM]
+
+    ll = np.log10(np.sum(F[l, :, :]))
 
-    ll = np.log10(np.sum(F[:, :, l]))
     return F, ll
 
 
 @jit.numba_njit
 def backward_ls_dip_starting_point(n, m, G, s, e, r):
     """Naive implementation of LS diploid backwards algorithm."""
     # Backwards
-    B = np.zeros((n, n, m))
+    B = np.zeros((m, n, n))
 
     # Initialise
-    B[:, :, m - 1] = 1
+    B[m - 1, :, :] = 1
     r_n = r / n
 
     for l in range(m - 2, -1, -1):
 
         # Determine the various components
         B_no_change = np.zeros((n, n))
         B_j1_change = np.zeros(n)
         B_j2_change = np.zeros(n)
         B_both_change = 0
 
         # Evaluate the emission matrix at this site, for all pairs
         e_tmp = np.zeros((n, n))
         if s[0, l + 1] == MISSING:
-            e_tmp[:, :] = e[MISSING_INDEX, l + 1]
+            e_tmp[:, :] = e[l + 1, MISSING_INDEX]
         else:
             for j1 in range(n):
                 for j2 in range(n):
                     # What is the emission?
                     if s[0, l + 1] == 1:
                         # OBS is het
-                        if G[j1, j2, l + 1] == 1:  # REF is het
-                            e_tmp[j1, j2] = e[BOTH_HET, l + 1]
+                        if G[l + 1, j1, j2] == 1:  # REF is het
+                            e_tmp[j1, j2] = e[l + 1, BOTH_HET]
                         else:  # REF is hom
-                            e_tmp[j1, j2] = e[REF_HOM_OBS_HET, l + 1]
+                            e_tmp[j1, j2] = e[l + 1, REF_HOM_OBS_HET]
                     else:
                         # OBS is hom
-                        if G[j1, j2, l + 1] == 1:  # REF is het
-                            e_tmp[j1, j2] = e[REF_HET_OBS_HOM, l + 1]
+                        if G[l + 1, j1, j2] == 1:  # REF is het
+                            e_tmp[j1, j2] = e[l + 1, REF_HET_OBS_HOM]
                         else:  # REF is hom
-                            if G[j1, j2, l + 1] == s[0, l + 1]:  # Equal
-                                e_tmp[j1, j2] = e[EQUAL_BOTH_HOM, l + 1]
+                            if G[l + 1, j1, j2] == s[0, l + 1]:  # Equal
+                                e_tmp[j1, j2] = e[l + 1, EQUAL_BOTH_HOM]
                             else:  # Unequal
-                                e_tmp[j1, j2] = e[UNEQUAL_BOTH_HOM, l + 1]
+                                e_tmp[j1, j2] = e[l + 1, UNEQUAL_BOTH_HOM]
 
         for j1 in range(n):
             for j2 in range(n):
                 B_no_change[j1, j2] = (
-                    (1 - r[l + 1]) ** 2 * B[j1, j2, l + 1] * e_tmp[j1, j2]
+                    (1 - r[l + 1]) ** 2 * B[l + 1, j1, j2] * e_tmp[j1, j2]
                 )
 
         for j1 in range(n):
             for j2 in range(n):
-                B_both_change += r_n[l + 1] ** 2 * e_tmp[j1, j2] * B[j1, j2, l + 1]
+                B_both_change += r_n[l + 1] ** 2 * e_tmp[j1, j2] * B[l + 1, j1, j2]
 
         for j1 in range(n):
             for j2 in range(n):  # This is the variable to sum over - it changes
                 B_j2_change[j1] += (
-                    (1 - r[l + 1]) * r_n[l + 1] * B[j1, j2, l + 1] * e_tmp[j1, j2]
+                    (1 - r[l + 1]) * r_n[l + 1] * B[l + 1, j1, j2] * e_tmp[j1, j2]
                 )
 
         for j2 in range(n):
             for j1 in range(n):  # This is the variable to sum over - it changes
                 B_j1_change[j2] += (
-                    (1 - r[l + 1]) * r_n[l + 1] * B[j1, j2, l + 1] * e_tmp[j1, j2]
+                    (1 - r[l + 1]) * r_n[l + 1] * B[l + 1, j1, j2] * e_tmp[j1, j2]
                 )
 
-        B[:, :, l] = B_both_change
+        B[l, :, :] = B_both_change
 
         for j1 in range(n):
-            B[j1, :, l] += B_j2_change
+            B[l, j1, :] += B_j2_change
 
         for j2 in range(n):
-            B[:, j2, l] += B_j1_change
+            B[l, :, j2] += B_j1_change
 
         for j1 in range(n):
             for j2 in range(n):
-                B[j1, j2, l] += B_no_change[j1, j2]
+                B[l, j1, j2] += B_no_change[j1, j2]
 
     return B
 
 
 @jit.numba_njit
 def forward_ls_dip_loop(n, m, G, s, e, r, norm=True):
     """LS diploid forwards algoritm without vectorisation."""
     # Initialise the forward tensor
-    F = np.zeros((n, n, m))
-    F[:, :, 0] = 1 / (n ** 2)
+    F = np.zeros((m, n, n))
+    for j1 in range(n):
+        for j2 in range(n):
+            F[0, j1, j2] = 1 / (n ** 2)
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            F[0, j1, j2] *= e[0, index_tmp]
     r_n = r / n
     c = np.ones(m)
 
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        )
-    F[:, :, 0] *= e[index.ravel(), 0].reshape(n, n)
-
     if norm:
 
-        c[0] = np.sum(F[:, :, 0])
-        F[:, :, 0] *= 1 / c[0]
+        c[0] = np.sum(F[0, :, :])
+        F[0, :, :] *= 1 / c[0]
 
         for l in range(1, m):
 
             # Determine the various components
             F_no_change = np.zeros((n, n))
             F_j_change = np.zeros(n)
 
             for j1 in range(n):
                 for j2 in range(n):
-                    F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[j1, j2, l - 1]
-                    F_j_change[j1] += (1 - r[l]) * r_n[l] * F[j2, j1, l - 1]
+                    F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[l - 1, j1, j2]
+                    F_j_change[j1] += (1 - r[l]) * r_n[l] * F[l - 1, j2, j1]
 
-            F[:, :, l] = r_n[l] ** 2
+            F[l, :, :] = r_n[l] ** 2
 
             for j1 in range(n):
-                F[j1, :, l] += F_j_change
-                F[:, j1, l] += F_j_change
+                F[l, j1, :] += F_j_change
+                F[l, :, j1] += F_j_change
                 for j2 in range(n):
-                    F[j1, j2, l] += F_no_change[j1, j2]
+                    F[l, j1, j2] += F_no_change[j1, j2]
 
             if s[0, l] == MISSING:
-                F[:, :, l] *= e[MISSING_INDEX, l]
+                F[l, :, :] *= e[l, MISSING_INDEX]
             else:
                 for j1 in range(n):
                     for j2 in range(n):
                         # What is the emission?
                         if s[0, l] == 1:
                             # OBS is het
-                            if G[j1, j2, l] == 1:  # REF is het
-                                F[j1, j2, l] *= e[BOTH_HET, l]
+                            if G[l, j1, j2] == 1:  # REF is het
+                                F[l, j1, j2] *= e[l, BOTH_HET]
                             else:  # REF is hom
-                                F[j1, j2, l] *= e[REF_HOM_OBS_HET, l]
+                                F[l, j1, j2] *= e[l, REF_HOM_OBS_HET]
                         else:
                             # OBS is hom
-                            if G[j1, j2, l] == 1:  # REF is het
-                                F[j1, j2, l] *= e[REF_HET_OBS_HOM, l]
+                            if G[l, j1, j2] == 1:  # REF is het
+                                F[l, j1, j2] *= e[l, REF_HET_OBS_HOM]
                             else:  # REF is hom
-                                if G[j1, j2, l] == s[0, l]:  # Equal
-                                    F[j1, j2, l] *= e[EQUAL_BOTH_HOM, l]
+                                if G[l, j1, j2] == s[0, l]:  # Equal
+                                    F[l, j1, j2] *= e[l, EQUAL_BOTH_HOM]
                                 else:  # Unequal
-                                    F[j1, j2, l] *= e[UNEQUAL_BOTH_HOM, l]
+                                    F[l, j1, j2] *= e[l, UNEQUAL_BOTH_HOM]
 
-            c[l] = np.sum(F[:, :, l])
-            F[:, :, l] *= 1 / c[l]
+            c[l] = np.sum(F[l, :, :])
+            F[l, :, :] *= 1 / c[l]
 
         ll = np.sum(np.log10(c))
 
     else:
 
         for l in range(1, m):
 
@@ -416,108 +413,112 @@
             F_no_change = np.zeros((n, n))
             F_j1_change = np.zeros(n)
             F_j2_change = np.zeros(n)
             F_both_change = 0
 
             for j1 in range(n):
                 for j2 in range(n):
-                    F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[j1, j2, l - 1]
-                    F_j1_change[j1] += (1 - r[l]) * r_n[l] * F[j2, j1, l - 1]
-                    F_j2_change[j1] += (1 - r[l]) * r_n[l] * F[j1, j2, l - 1]
-                    F_both_change += r_n[l] ** 2 * F[j1, j2, l - 1]
+                    F_no_change[j1, j2] = (1 - r[l]) ** 2 * F[l - 1, j1, j2]
+                    F_j1_change[j1] += (1 - r[l]) * r_n[l] * F[l - 1, j2, j1]
+                    F_j2_change[j1] += (1 - r[l]) * r_n[l] * F[l - 1, j1, j2]
+                    F_both_change += r_n[l] ** 2 * F[l - 1, j1, j2]
 
-            F[:, :, l] = F_both_change
+            F[l, :, :] = F_both_change
 
             for j1 in range(n):
-                F[j1, :, l] += F_j2_change
-                F[:, j1, l] += F_j1_change
+                F[l, j1, :] += F_j2_change
+                F[l, :, j1] += F_j1_change
                 for j2 in range(n):
-                    F[j1, j2, l] += F_no_change[j1, j2]
+                    F[l, j1, j2] += F_no_change[j1, j2]
 
             if s[0, l] == MISSING:
-                F[:, :, l] *= e[MISSING_INDEX, l]
+                F[l, :, :] *= e[l, MISSING_INDEX]
             else:
                 for j1 in range(n):
                     for j2 in range(n):
                         # What is the emission?
                         if s[0, l] == 1:
                             # OBS is het
-                            if G[j1, j2, l] == 1:  # REF is het
-                                F[j1, j2, l] *= e[BOTH_HET, l]
+                            if G[l, j1, j2] == 1:  # REF is het
+                                F[l, j1, j2] *= e[l, BOTH_HET]
                             else:  # REF is hom
-                                F[j1, j2, l] *= e[REF_HOM_OBS_HET, l]
+                                F[l, j1, j2] *= e[l, REF_HOM_OBS_HET]
                         else:
                             # OBS is hom
-                            if G[j1, j2, l] == 1:  # REF is het
-                                F[j1, j2, l] *= e[REF_HET_OBS_HOM, l]
+                            if G[l, j1, j2] == 1:  # REF is het
+                                F[l, j1, j2] *= e[l, REF_HET_OBS_HOM]
                             else:  # REF is hom
-                                if G[j1, j2, l] == s[0, l]:  # Equal
-                                    F[j1, j2, l] *= e[EQUAL_BOTH_HOM, l]
+                                if G[l, j1, j2] == s[0, l]:  # Equal
+                                    F[l, j1, j2] *= e[l, EQUAL_BOTH_HOM]
                                 else:  # Unequal
-                                    F[j1, j2, l] *= e[UNEQUAL_BOTH_HOM, l]
+                                    F[l, j1, j2] *= e[l, UNEQUAL_BOTH_HOM]
 
-        ll = np.log10(np.sum(F[:, :, l]))
+            ll = np.log10(np.sum(F[l, :, :]))
 
     return F, c, ll
 
 
 @jit.numba_njit
 def backward_ls_dip_loop(n, m, G, s, e, c, r):
     """LS diploid backwards algoritm without vectorisation."""
     # Initialise the backward tensor
-    B = np.zeros((n, n, m))
-    B[:, :, m - 1] = 1
+    B = np.zeros((m, n, n))
+    B[m - 1, :, :] = 1
     r_n = r / n
 
     for l in range(m - 2, -1, -1):
 
         # Determine the various components
         B_no_change = np.zeros((n, n))
-        B_j_change = np.zeros(n)
+        B_j1_change = np.zeros(n)
+        B_j2_change = np.zeros(n)
         B_both_change = 0
 
         # Evaluate the emission matrix at this site, for all pairs
         e_tmp = np.zeros((n, n))
         if s[0, l + 1] == MISSING:
-            e_tmp[:, :] = e[MISSING_INDEX, l + 1]
+            e_tmp[:, :] = e[l + 1, MISSING_INDEX]
         else:
             for j1 in range(n):
                 for j2 in range(n):
                     # What is the emission?
+                    # else:
                     if s[0, l + 1] == 1:
                         # OBS is het
-                        if G[j1, j2, l + 1] == 1:  # REF is het
-                            e_tmp[j1, j2] = e[BOTH_HET, l + 1]
+                        if G[l + 1, j1, j2] == 1:  # REF is het
+                            e_tmp[j1, j2] = e[l + 1, BOTH_HET]
                         else:  # REF is hom
-                            e_tmp[j1, j2] = e[REF_HOM_OBS_HET, l + 1]
+                            e_tmp[j1, j2] = e[l + 1, REF_HOM_OBS_HET]
                     else:
                         # OBS is hom
-                        if G[j1, j2, l + 1] == 1:  # REF is het
-                            e_tmp[j1, j2] = e[REF_HET_OBS_HOM, l + 1]
+                        if G[l + 1, j1, j2] == 1:  # REF is het
+                            e_tmp[j1, j2] = e[l + 1, REF_HET_OBS_HOM]
                         else:  # REF is hom
-                            if G[j1, j2, l + 1] == s[0, l + 1]:  # Equal
-                                e_tmp[j1, j2] = e[EQUAL_BOTH_HOM, l + 1]
+                            if G[l + 1, j1, j2] == s[0, l + 1]:  # Equal
+                                e_tmp[j1, j2] = e[l + 1, EQUAL_BOTH_HOM]
                             else:  # Unequal
-                                e_tmp[j1, j2] = e[UNEQUAL_BOTH_HOM, l + 1]
+                                e_tmp[j1, j2] = e[l + 1, UNEQUAL_BOTH_HOM]
 
         for j1 in range(n):
             for j2 in range(n):
                 B_no_change[j1, j2] = (
-                    (1 - r[l + 1]) ** 2 * B[j1, j2, l + 1] * e_tmp[j1, j2]
+                    (1 - r[l + 1]) ** 2 * B[l + 1, j1, j2] * e_tmp[j1, j2]
+                )
+                B_j2_change[j1] += (
+                    (1 - r[l + 1]) * r_n[l + 1] * B[l + 1, j1, j2] * e_tmp[j1, j2]
                 )
-                B_j_change[j1] += (
-                    (1 - r[l + 1]) * r_n[l + 1] * B[j1, j2, l + 1] * e_tmp[j1, j2]
+                B_j1_change[j1] += (
+                    (1 - r[l + 1]) * r_n[l + 1] * B[l + 1, j2, j1] * e_tmp[j2, j1]
                 )
-                B_both_change += r_n[l + 1] ** 2 * e_tmp[j1, j2] * B[j1, j2, l + 1]
+                B_both_change += r_n[l + 1] ** 2 * e_tmp[j1, j2] * B[l + 1, j1, j2]
 
-        B[:, :, l] = B_both_change
+        B[l, :, :] = B_both_change
 
         for j1 in range(n):
-            B[:, j1, l] += B_j_change
-            B[j1, :, l] += B_j_change
-
+            B[l, j1, :] += B_j2_change
+            B[l, :, j1] += B_j1_change
             for j2 in range(n):
-                B[j1, j2, l] += B_no_change[j1, j2]
+                B[l, j1, j2] += B_no_change[j1, j2]
 
-        B[:, :, l] *= 1 / c[l + 1]
+        B[l, :, :] *= 1 / c[l + 1]
 
     return B
```

### Comparing `lshmm-0.0.4/lshmm/forward_backward/fb_haploid_samples_variants.py` & `lshmm-0.0.5/lshmm/forward_backward/fb_haploid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-"""Collection of functions to run forwards and backwards algorithms on haploid genotype data, where the data is structured as samples x variants."""
+"""Collection of functions to run forwards and backwards algorithms on haploid genotype data, where the data is structured as variants x samples."""
 import numpy as np
+
 from lshmm import jit
 
 MISSING = -1
 
+
 @jit.numba_njit
 def forwards_ls_hap(n, m, H, s, e, r, norm=True):
     """Matrix based haploid LS forward algorithm using numpy vectorisation."""
     # Initialise
-    F = np.zeros((n, m))
+    F = np.zeros((m, n))
     r_n = r / n
 
     if norm:
 
         c = np.zeros(m)
         for i in range(n):
-            F[i, 0] = (
-                1 / n * e[np.int64(np.equal(H[i, 0], s[0, 0]) or s[0, 0] == MISSING), 0]
+            F[0, i] = (
+                1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
             )
-            c[0] += F[i, 0]
+            c[0] += F[0, i]
 
         for i in range(n):
-            F[i, 0] *= 1 / c[0]
+            F[0, i] *= 1 / c[0]
 
         # Forwards pass
         for l in range(1, m):
             for i in range(n):
-                F[i, l] = F[i, l - 1] * (1 - r[l]) + r_n[l]
-                F[i, l] *= e[
-                    np.int64(np.equal(H[i, l], s[0, l]) or s[0, l] == MISSING), l
+                F[l, i] = F[l - 1, i] * (1 - r[l]) + r_n[l]
+                F[l, i] *= e[
+                    l, np.int64(np.equal(H[l, i], s[0, l]) or s[0, l] == MISSING)
                 ]
-                c[l] += F[i, l]
+                c[l] += F[l, i]
 
             for i in range(n):
-                F[i, l] *= 1 / c[l]
+                F[l, i] *= 1 / c[l]
 
         ll = np.sum(np.log10(c))
 
     else:
+
         c = np.ones(m)
 
         for i in range(n):
-            F[i, 0] = (
-                1 / n * e[np.int64(np.equal(H[i, 0], s[0, 0]) or s[0, 0] == MISSING), 0]
+            F[0, i] = (
+                1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
             )
+
         # Forwards pass
         for l in range(1, m):
             for i in range(n):
-                F[i, l] = F[i, l - 1] * (1 - r[l]) + np.sum(F[:, l - 1]) * r_n[l]
-                F[i, l] *= e[
-                    np.int64(np.equal(H[i, l], s[0, l]) or s[0, l] == MISSING), l
+                F[l, i] = F[l - 1, i] * (1 - r[l]) + np.sum(F[l - 1, :]) * r_n[l]
+                F[l, i] *= e[
+                    l, np.int64(np.equal(H[l, i], s[0, l]) or s[0, l] == MISSING)
                 ]
 
-        ll = np.log10(np.sum(F[:, m - 1]))
+        ll = np.log10(np.sum(F[m - 1, :]))
 
     return F, c, ll
 
 
 @jit.numba_njit
 def backwards_ls_hap(n, m, H, s, e, c, r):
     """Matrix based haploid LS backward algorithm using numpy vectorisation."""
     # Initialise
-    B = np.zeros((n, m))
+    B = np.zeros((m, n))
     for i in range(n):
-        B[i, m - 1] = 1
+        B[m - 1, i] = 1
     r_n = r / n
 
     # Backwards pass
     for l in range(m - 2, -1, -1):
         tmp_B = np.zeros(n)
         tmp_B_sum = 0
         for i in range(n):
             tmp_B[i] = (
                 e[
+                    l + 1,
                     np.int64(
-                        np.equal(H[i, l + 1], s[0, l + 1]) or s[0, l + 1] == MISSING
+                        np.equal(H[l + 1, i], s[0, l + 1]) or s[0, l + 1] == MISSING
                     ),
-                    l + 1,
                 ]
-                * B[i, l + 1]
+                * B[l + 1, i]
             )
             tmp_B_sum += tmp_B[i]
         for i in range(n):
-            B[i, l] = r_n[l + 1] * tmp_B_sum
-            B[i, l] += (1 - r[l + 1]) * tmp_B[i]
-            B[i, l] *= 1 / c[l + 1]
+            B[l, i] = r_n[l + 1] * tmp_B_sum
+            B[l, i] += (1 - r[l + 1]) * tmp_B[i]
+            B[l, i] *= 1 / c[l + 1]
 
     return B
```

### Comparing `lshmm-0.0.4/lshmm/jit.py` & `lshmm-0.0.5/lshmm/jit.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     ) from e
 
 # We will mostly be using disable numba for debugging and running tests for
 # coverage, so raise a loud warning in case this is being used accidentally.
 
 if not ENABLE_NUMBA:
     logger.warning(
-        "numba globally disabled for lshmm; performance will be drastically"
-        " reduced."
+        "numba globally disabled for lshmm; performance will be drastically" " reduced."
     )
 
 
 DEFAULT_NUMBA_ARGS = {
     "nopython": True,
     "cache": True,
 }
```

### Comparing `lshmm-0.0.4/lshmm/vit_diploid_samples_variants.py` & `lshmm-0.0.5/lshmm/vit_diploid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Collection of functions to run Viterbi algorithms on dipoid genotype data, where the data is structured as samples x variants."""
+"""Collection of functions to run Viterbi algorithms on dipoid genotype data, where the data is structured as variants x samples."""
 import numpy as np
+
 from . import jit
 
 MISSING = -1
 MISSING_INDEX = 3
 
 # https://github.com/numba/numba/issues/1269
 @jit.numba_njit
@@ -40,102 +41,99 @@
     return np_apply_along_axis(np.argmax, axis, array)
 
 
 @jit.numba_njit
 def forwards_viterbi_dip_naive(n, m, G, s, e, r):
     """Naive implementation of LS diploid Viterbi algorithm."""
     # Initialise
-    V = np.zeros((n, n, m))
-    P = np.zeros((n, n, m)).astype(np.int64)
+    V = np.zeros((m, n, n))
+    P = np.zeros((m, n, n)).astype(np.int64)
     c = np.ones(m)
-
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
-        # index = EQUAL_BOTH_HOM * np.ones((n, n), dtype=np.int64) + (
-        #     BOTH_HET - EQUAL_BOTH_HOM
-        # ) * (G[:, :, 0] == 1).astype(np.int64)
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        )
-
-    V[:, :, 0] = 1 / (n ** 2) * e[index.ravel(), 0].reshape(n, n)
     r_n = r / n
 
-    for l in range(1, m):
+    for j1 in range(n):
+        for j2 in range(n):
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            V[0, j1, j2] = 1 / (n ** 2) * e[0, index_tmp]
 
+    for l in range(1, m):
         if s[0, l] == MISSING:
             index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
         else:
             index = (
-                4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64)
-                + 2 * (G[:, :, l] == 1).astype(np.int64)
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l] == 1)
             )
 
         for j1 in range(n):
             for j2 in range(n):
                 # Get the vector to maximise over
                 v = np.zeros((n, n))
                 for k1 in range(n):
                     for k2 in range(n):
-                        v[k1, k2] = V[k1, k2, l - 1]
+                        v[k1, k2] = V[l - 1, k1, k2]
                         if (k1 == j1) and (k2 == j2):
                             v[k1, k2] *= (
                                 (1 - r[l]) ** 2 + 2 * (1 - r[l]) * r_n[l] + r_n[l] ** 2
                             )
                         elif (k1 == j1) or (k2 == j2):
                             v[k1, k2] *= r_n[l] * (1 - r[l]) + r_n[l] ** 2
                         else:
                             v[k1, k2] *= r_n[l] ** 2
-                V[j1, j2, l] = np.amax(v) * e[index[j1, j2], l]
-                P[j1, j2, l] = np.argmax(v)
-        c[l] = np.amax(V[:, :, l])
-        V[:, :, l] *= 1 / c[l]
+                V[l, j1, j2] = np.amax(v) * e[l, index[j1, j2]]
+                P[l, j1, j2] = np.argmax(v)
+        c[l] = np.amax(V[l, :, :])
+        V[l, :, :] *= 1 / c[l]
 
     ll = np.sum(np.log10(c))
 
     return V, P, ll
 
 
 @jit.numba_njit
 def forwards_viterbi_dip_naive_low_mem(n, m, G, s, e, r):
     """Naive implementation of LS diploid Viterbi algorithm, with reduced memory."""
     # Initialise
     V = np.zeros((n, n))
-    P = np.zeros((n, n, m)).astype(np.int64)
+    V_previous = np.zeros((n, n))
+    P = np.zeros((m, n, n)).astype(np.int64)
     c = np.ones(m)
-
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        )
-
-    V_previous = 1 / (n ** 2) * e[index.ravel(), 0].reshape(n, n)
     r_n = r / n
 
+    for j1 in range(n):
+        for j2 in range(n):
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            V_previous[j1, j2] = 1 / (n ** 2) * e[0, index_tmp]
+
     # Take a look at Haploid Viterbi implementation in Jeromes code and see if we can pinch some ideas.
     # Diploid Viterbi, with smaller memory footprint.
     for l in range(1, m):
-
         if s[0, l] == MISSING:
             index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
         else:
             index = (
-                4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64)
-                + 2 * (G[:, :, l] == 1).astype(np.int64)
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l] == 1)
             )
-
         for j1 in range(n):
             for j2 in range(n):
                 # Get the vector to maximise over
                 v = np.zeros((n, n))
                 for k1 in range(n):
                     for k2 in range(n):
                         v[k1, k2] = V_previous[k1, k2]
@@ -143,62 +141,63 @@
                             v[k1, k2] *= (
                                 (1 - r[l]) ** 2 + 2 * (1 - r[l]) * r_n[l] + r_n[l] ** 2
                             )
                         elif (k1 == j1) or (k2 == j2):
                             v[k1, k2] *= r_n[l] * (1 - r[l]) + r_n[l] ** 2
                         else:
                             v[k1, k2] *= r_n[l] ** 2
-                V[j1, j2] = np.amax(v) * e[index[j1, j2], l]
-                P[j1, j2, l] = np.argmax(v)
+                V[j1, j2] = np.amax(v) * e[l, index[j1, j2]]
+                P[l, j1, j2] = np.argmax(v)
         c[l] = np.amax(V)
         V_previous = np.copy(V) / c[l]
 
     ll = np.sum(np.log10(c))
 
     return V, P, ll
 
 
 @jit.numba_njit
 def forwards_viterbi_dip_low_mem(n, m, G, s, e, r):
     """LS diploid Viterbi algorithm, with reduced memory."""
     # Initialise
     V = np.zeros((n, n))
-    P = np.zeros((n, n, m)).astype(np.int64)
-
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        )
-
-    V_previous = 1 / (n ** 2) * e[index.ravel(), 0].reshape(n, n)
+    V_previous = np.zeros((n, n))
+    P = np.zeros((m, n, n)).astype(np.int64)
     c = np.ones(m)
     r_n = r / n
 
+    for j1 in range(n):
+        for j2 in range(n):
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            V_previous[j1, j2] = 1 / (n ** 2) * e[0, index_tmp]
+
     # Diploid Viterbi, with smaller memory footprint, rescaling, and using the structure of the HMM.
     for l in range(1, m):
-
         if s[0, l] == MISSING:
             index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
         else:
             index = (
-                4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64)
-                + 2 * (G[:, :, l] == 1).astype(np.int64)
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l] == 1)
             )
 
         c[l] = np.amax(V_previous)
         argmax = np.argmax(V_previous)
 
         V_previous *= 1 / c[l]
-        V_rowcol_max = np_amax(V_previous, axis=0)
-        arg_rowcol_max = np_argmax(V_previous, axis=0)
+        V_rowcol_max = np_amax(V_previous, 0)
+        arg_rowcol_max = np_argmax(V_previous, 0)
 
         no_switch = (1 - r[l]) ** 2 + 2 * (r_n[l] * (1 - r[l])) + r_n[l] ** 2
         single_switch = r_n[l] * (1 - r[l]) + r_n[l] ** 2
         double_switch = r_n[l] ** 2
 
         j1_j2 = 0
 
@@ -212,133 +211,227 @@
 
                 if P_single_switch == 0:
                     template_single_switch = j1 * n + arg_rowcol_max[j1]
                 else:
                     template_single_switch = arg_rowcol_max[j2] * n + j2
 
                 V[j1, j2] = V_previous[j1, j2] * no_switch  # No switch in either
-                P[j1, j2, l] = j1_j2
+                P[l, j1, j2] = j1_j2
 
                 # Single or double switch?
                 single_switch_tmp = single_switch * V_single_switch
                 if single_switch_tmp > double_switch:
                     # Then single switch is the alternative
                     if V[j1, j2] < single_switch * V_single_switch:
                         V[j1, j2] = single_switch * V_single_switch
-                        P[j1, j2, l] = template_single_switch
+                        P[l, j1, j2] = template_single_switch
                 else:
                     # Double switch is the alternative
                     if V[j1, j2] < double_switch:
                         V[j1, j2] = double_switch
-                        P[j1, j2, l] = argmax
+                        P[l, j1, j2] = argmax
 
-                V[j1, j2] *= e[index[j1, j2], l]
+                V[j1, j2] *= e[l, index[j1, j2]]
                 j1_j2 += 1
         V_previous = np.copy(V)
 
     ll = np.sum(np.log10(c)) + np.log10(np.amax(V))
 
     return V, P, ll
 
 
 @jit.numba_njit
-def forwards_viterbi_dip_naive_vec(n, m, G, s, e, r):
-    """Vectorised LS diploid Viterbi algorithm using numpy."""
+def forwards_viterbi_dip_low_mem_no_pointer(n, m, G, s, e, r):
+    """LS diploid Viterbi algorithm, with reduced memory."""
     # Initialise
-    V = np.zeros((n, n, m))
-    P = np.zeros((n, n, m)).astype(np.int64)
+    V = np.zeros((n, n))
+    V_previous = np.zeros((n, n))
     c = np.ones(m)
+    r_n = r / n
 
-    if s[0, 0] == MISSING:
-        index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
-    else:
-        index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
-            + np.int64(s[0, 0] == 1)
-        )
+    recombs_single = [
+        np.zeros(shape=0, dtype=np.int64) for _ in range(m)
+    ]  # Store all single switch recombs
+    recombs_double = [
+        np.zeros(shape=0, dtype=np.int64) for _ in range(m)
+    ]  # Store all double switch recombs
+
+    V_argmaxes = np.zeros(m)
+    V_rowcol_maxes = np.zeros((m, n))
+    V_rowcol_argmaxes = np.zeros((m, n))
+
+    for j1 in range(n):
+        for j2 in range(n):
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            V_previous[j1, j2] = 1 / (n ** 2) * e[0, index_tmp]
+
+    # Diploid Viterbi, with smaller memory footprint, rescaling, and using the structure of the HMM.
+    for l in range(1, m):
+        if s[0, l] == MISSING:
+            index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
+        else:
+            index = (
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
+                + np.int64(s[0, l] == 1)
+            )
+
+        c[l] = np.amax(V_previous)
+        argmax = np.argmax(V_previous)
+        V_argmaxes[l - 1] = argmax  # added
+
+        V_previous *= 1 / c[l]
+        V_rowcol_max = np_amax(V_previous, 0)
+        V_rowcol_maxes[l - 1, :] = V_rowcol_max
+        arg_rowcol_max = np_argmax(V_previous, 0)
+        V_rowcol_argmaxes[l - 1, :] = arg_rowcol_max
 
-    V[:, :, 0] = 1 / (n ** 2) * e[index.ravel(), 0].reshape(n, n)
+        no_switch = (1 - r[l]) ** 2 + 2 * (r_n[l] * (1 - r[l])) + r_n[l] ** 2
+        single_switch = r_n[l] * (1 - r[l]) + r_n[l] ** 2
+        double_switch = r_n[l] ** 2
+
+        j1_j2 = 0
+
+        for j1 in range(n):
+            for j2 in range(n):
+
+                V_single_switch = max(V_rowcol_max[j1], V_rowcol_max[j2])
+                V[j1, j2] = V_previous[j1, j2] * no_switch  # No switch in either
+
+                # Single or double switch?
+                single_switch_tmp = single_switch * V_single_switch
+                if single_switch_tmp > double_switch:
+                    # Then single switch is the alternative
+                    if V[j1, j2] < single_switch * V_single_switch:
+                        V[j1, j2] = single_switch * V_single_switch
+                        recombs_single[l] = np.append(recombs_single[l], j1_j2)
+                else:
+                    # Double switch is the alternative
+                    if V[j1, j2] < double_switch:
+                        V[j1, j2] = double_switch
+                        recombs_double[l] = np.append(recombs_double[l], values=j1_j2)
+
+                V[j1, j2] *= e[l, index[j1, j2]]
+                j1_j2 += 1
+        V_previous = np.copy(V)
+
+    V_argmaxes[m - 1] = np.argmax(V_previous)
+    V_rowcol_maxes[m - 1, :] = np_amax(V_previous, 0)
+    V_rowcol_argmaxes[m - 1, :] = np_argmax(V_previous, 0)
+    ll = np.sum(np.log10(c)) + np.log10(np.amax(V))
+
+    return (
+        V,
+        V_argmaxes,
+        V_rowcol_maxes,
+        V_rowcol_argmaxes,
+        recombs_single,
+        recombs_double,
+        ll,
+    )
+
+
+@jit.numba_njit
+def forwards_viterbi_dip_naive_vec(n, m, G, s, e, r):
+    """Vectorised LS diploid Viterbi algorithm using numpy."""
+    # Initialise
+    V = np.zeros((m, n, n))
+    P = np.zeros((m, n, n)).astype(np.int64)
+    c = np.ones(m)
     r_n = r / n
 
+    for j1 in range(n):
+        for j2 in range(n):
+            if s[0, 0] == MISSING:
+                index_tmp = MISSING_INDEX
+            else:
+                index_tmp = (
+                    4 * np.int64(np.equal(G[0, j1, j2], s[0, 0]))
+                    + 2 * np.int64((G[0, j1, j2] == 1))
+                    + np.int64(s[0, 0] == 1)
+                )
+            V[0, j1, j2] = 1 / (n ** 2) * e[0, index_tmp]
+
     # Jumped the gun - vectorising.
     for l in range(1, m):
-
         if s[0, l] == MISSING:
             index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
         else:
             index = (
-                4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64)
-                + 2 * (G[:, :, l] == 1).astype(np.int64)
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l] == 1)
             )
 
         for j1 in range(n):
             for j2 in range(n):
                 v = (r_n[l] ** 2) * np.ones((n, n))
                 v[j1, j2] += (1 - r[l]) ** 2
                 v[j1, :] += r_n[l] * (1 - r[l])
                 v[:, j2] += r_n[l] * (1 - r[l])
-                v *= V[:, :, l - 1]
-                V[j1, j2, l] = np.amax(v) * e[index[j1, j2], l]
-                P[j1, j2, l] = np.argmax(v)
+                v *= V[l - 1, :, :]
+                V[l, j1, j2] = np.amax(v) * e[l, index[j1, j2]]
+                P[l, j1, j2] = np.argmax(v)
 
-        c[l] = np.amax(V[:, :, l])
-        V[:, :, l] *= 1 / c[l]
+        c[l] = np.amax(V[l, :, :])
+        V[l, :, :] *= 1 / c[l]
 
     ll = np.sum(np.log10(c))
 
     return V, P, ll
 
 
 def forwards_viterbi_dip_naive_full_vec(n, m, G, s, e, r):
     """Fully vectorised naive LS diploid Viterbi algorithm using numpy."""
     char_both = np.eye(n * n).ravel().reshape((n, n, n, n))
     char_col = np.tile(np.sum(np.eye(n * n).reshape((n, n, n, n)), 3), (n, 1, 1, 1))
-    char_row = np.copy(char_col.T)
+    char_row = np.copy(char_col).T
     rows, cols = np.ogrid[:n, :n]
 
     # Initialise
-    V = np.zeros((n, n, m))
-    P = np.zeros((n, n, m)).astype(np.int64)
+    V = np.zeros((m, n, n))
+    P = np.zeros((m, n, n)).astype(np.int64)
     c = np.ones(m)
-
     if s[0, 0] == MISSING:
         index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
     else:
         index = (
-            4 * np.equal(G[:, :, 0], s[0, 0]).astype(np.int64)
-            + 2 * (G[:, :, 0] == 1).astype(np.int64)
+            4 * np.equal(G[0, :, :], s[0, 0]).astype(np.int64)
+            + 2 * (G[0, :, :] == 1).astype(np.int64)
             + np.int64(s[0, 0] == 1)
         )
-
-    V[:, :, 0] = 1 / (n ** 2) * e[index, 0]
+    V[0, :, :] = 1 / (n ** 2) * e[0, index]
     r_n = r / n
 
     for l in range(1, m):
-
         if s[0, l] == MISSING:
             index = MISSING_INDEX * np.ones((n, n), dtype=np.int64)
         else:
             index = (
-                4 * np.equal(G[:, :, l], s[0, l]).astype(np.int64)
-                + 2 * (G[:, :, l] == 1).astype(np.int64)
+                4 * np.equal(G[l, :, :], s[0, l]).astype(np.int64)
+                + 2 * (G[l, :, :] == 1).astype(np.int64)
                 + np.int64(s[0, l] == 1)
             )
-
         v = (
             (r_n[l] ** 2)
             + (1 - r[l]) ** 2 * char_both
             + (r_n[l] * (1 - r[l])) * (char_col + char_row)
         )
-        v *= V[:, :, l - 1]
-        P[:, :, l] = np.argmax(v.reshape(n, n, -1), 2)  # Have to flatten to use argmax
-        V[:, :, l] = v.reshape(n, n, -1)[rows, cols, P[:, :, l]] * e[index, l]
-        c[l] = np.amax(V[:, :, l])
-        V[:, :, l] *= 1 / c[l]
+        v *= V[l - 1, :, :]
+        P[l, :, :] = np.argmax(v.reshape(n, n, -1), 2)  # Have to flatten to use argmax
+        V[l, :, :] = v.reshape(n, n, -1)[rows, cols, P[l, :, :]] * e[l, index]
+        c[l] = np.amax(V[l, :, :])
+        V[l, :, :] *= 1 / c[l]
 
     ll = np.sum(np.log10(c))
 
     return V, P, ll
 
 
 @jit.numba_njit
@@ -348,15 +441,60 @@
     assert V_last.shape[0] == V_last.shape[1]
     # Initialisation
     path = np.zeros(m).astype(np.int64)
     path[m - 1] = np.argmax(V_last)
 
     # Backtrace
     for j in range(m - 2, -1, -1):
-        path[j] = P[:, :, j + 1].ravel()[path[j + 1]]
+        path[j] = P[j + 1, :, :].ravel()[path[j + 1]]
+
+    return path
+
+
+@jit.numba_njit
+def in_list(array, value):
+    where = np.searchsorted(array, value)
+    if where < array.shape[0]:
+        return array[where] == value
+    else:
+        return False
+
+
+@jit.numba_njit
+def backwards_viterbi_dip_no_pointer(
+    m,
+    V_argmaxes,
+    V_rowcol_maxes,
+    V_rowcol_argmaxes,
+    recombs_single,
+    recombs_double,
+    V_last,
+):
+    """Run a backwards pass to determine the most likely path."""
+    assert V_last.ndim == 2
+    assert V_last.shape[0] == V_last.shape[1]
+    # Initialisation
+    path = np.zeros(m).astype(np.int64)
+    path[m - 1] = np.argmax(V_last)
+    n = V_last.shape[0]
+
+    # Backtrace
+    for l in range(m - 2, -1, -1):
+        current_best_template = path[l + 1]
+        # if current_best_template in recombs_double[l + 1]:
+        if in_list(recombs_double[l + 1], current_best_template):
+            current_best_template = V_argmaxes[l]
+        # elif current_best_template in recombs_single[l + 1]:
+        elif in_list(recombs_single[l + 1], current_best_template):
+            (j1, j2) = divmod(current_best_template, n)
+            if V_rowcol_maxes[l, j1] > V_rowcol_maxes[l, j2]:
+                current_best_template = j1 * n + V_rowcol_argmaxes[l, j1]
+            else:
+                current_best_template = V_rowcol_argmaxes[l, j2] * n + j2
+        path[l] = current_best_template
 
     return path
 
 
 def get_phased_path(n, path):
     """Obtain the phased path."""
     return np.unravel_index(path, (n, n))
@@ -365,34 +503,33 @@
 @jit.numba_njit
 def path_ll_dip(n, m, G, phased_path, s, e, r):
     """Evaluate log-likelihood path through a reference panel which results in sequence s."""
     if s[0, 0] == MISSING:
         index = MISSING_INDEX
     else:
         index = (
-            4 * np.int64(np.equal(G[phased_path[0][0], phased_path[1][0], 0], s[0, 0]))
-            + 2 * np.int64(G[phased_path[0][0], phased_path[1][0], 0] == 1)
+            4 * np.int64(np.equal(G[0, phased_path[0][0], phased_path[1][0]], s[0, 0]))
+            + 2 * np.int64(G[0, phased_path[0][0], phased_path[1][0]] == 1)
             + np.int64(s[0, 0] == 1)
         )
-
-    log_prob_path = np.log10(1 / (n ** 2) * e[index, 0])
+    log_prob_path = np.log10(1 / (n ** 2) * e[0, index])
     old_phase = np.array([phased_path[0][0], phased_path[1][0]])
     r_n = r / n
 
     for l in range(1, m):
 
         if s[0, l] == MISSING:
             index = MISSING_INDEX
         else:
             index = (
                 4
                 * np.int64(
-                    np.equal(G[phased_path[0][l], phased_path[1][l], l], s[0, l])
+                    np.equal(G[l, phased_path[0][l], phased_path[1][l]], s[0, l])
                 )
-                + 2 * np.int64(G[phased_path[0][l], phased_path[1][l], l] == 1)
+                + 2 * np.int64(G[l, phased_path[0][l], phased_path[1][l]] == 1)
                 + np.int64(s[0, l] == 1)
             )
 
         current_phase = np.array([phased_path[0][l], phased_path[1][l]])
         phase_diff = np.sum(~np.equal(current_phase, old_phase))
 
         if phase_diff == 0:
@@ -400,11 +537,11 @@
                 (1 - r[l]) ** 2 + 2 * (r_n[l] * (1 - r[l])) + r_n[l] ** 2
             )
         elif phase_diff == 1:
             log_prob_path += np.log10(r_n[l] * (1 - r[l]) + r_n[l] ** 2)
         else:
             log_prob_path += np.log10(r_n[l] ** 2)
 
-        log_prob_path += np.log10(e[index, l])
+        log_prob_path += np.log10(e[l, index])
         old_phase = current_phase
 
     return log_prob_path
```

### Comparing `lshmm-0.0.4/lshmm/vit_haploid_samples_variants.py` & `lshmm-0.0.5/lshmm/vit_haploid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-"""Collection of functions to run Viterbi algorithms on haploid genotype data, where the data is structured as samples x variants."""
+"""Collection of functions to run Viterbi algorithms on haploid genotype data, where the data is structured as variants x samples."""
 import numpy as np
+
 from . import jit
 
 MISSING = -1
 
+
 @jit.numba_njit
 def viterbi_naive_init(n, m, H, s, e, r):
     """Initialise naive implementation of LS viterbi."""
-    V = np.zeros((n, m))
-    P = np.zeros((n, m)).astype(np.int64)
+    V = np.zeros((m, n))
+    P = np.zeros((m, n)).astype(np.int64)
     r_n = r / n
-
-    P[:, 0] = 0  # Reminder
-
     for i in range(n):
-        V[i, 0] = (
-            1 / n * e[np.int64(np.equal(H[i, 0], s[0, 0]) or s[0, 0] == MISSING), 0]
+        V[0, i] = (
+            1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
         )
 
     return V, P, r_n
 
 
 @jit.numba_njit
 def viterbi_init(n, m, H, s, e, r):
     """Initialise naive, but more space memory efficient implementation of LS viterbi."""
     V_previous = np.zeros(n)
+    V = np.zeros(n)
+    P = np.zeros((m, n)).astype(np.int64)
+    r_n = r / n
+
     for i in range(n):
         V_previous[i] = (
-            1 / n * e[np.int64(np.equal(H[i, 0], s[0, 0]) or s[0, 0] == MISSING), 0]
+            1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
         )
 
-    V = np.zeros(n)
-    P = np.zeros((n, m)).astype(np.int64)
-    P[:, 0] = 0  # Reminder
-    r_n = r / n
-
     return V, V_previous, P, r_n
 
 
 @jit.numba_njit
 def forwards_viterbi_hap_naive(n, m, H, s, e, r):
     """Naive implementation of LS haploid Viterbi algorithm."""
     # Initialise
@@ -46,69 +44,70 @@
 
     for j in range(1, m):
         for i in range(n):
             # Get the vector to maximise over
             v = np.zeros(n)
             for k in range(n):
                 v[k] = (
-                    e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
-                    * V[k, j - 1]
+                    e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
+                    * V[j - 1, k]
                 )
                 if k == i:
                     v[k] *= 1 - r[j] + r_n[j]
                 else:
                     v[k] *= r_n[j]
-            P[i, j] = np.argmax(v)
-            V[i, j] = v[P[i, j]]
+            P[j, i] = np.argmax(v)
+            V[j, i] = v[P[j, i]]
 
-    ll = np.log10(np.amax(V[:, m - 1]))
+    ll = np.log10(np.amax(V[m - 1, :]))
 
     return V, P, ll
 
 
 @jit.numba_njit
 def forwards_viterbi_hap_naive_vec(n, m, H, s, e, r):
     """Naive matrix based implementation of LS haploid forward Viterbi algorithm using numpy."""
     # Initialise
     V, P, r_n = viterbi_naive_init(n, m, H, s, e, r)
 
     for j in range(1, m):
-        v_tmp = V[:, j - 1] * r_n[j]
+        v_tmp = V[j - 1, :] * r_n[j]
         for i in range(n):
             v = np.copy(v_tmp)
-            v[i] += V[i, j - 1] * (1 - r[j])
-            v *= e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
-            P[i, j] = np.argmax(v)
-            V[i, j] = v[P[i, j]]
+            v[i] += V[j - 1, i] * (1 - r[j])
+            v *= e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
+            P[j, i] = np.argmax(v)
+            V[j, i] = v[P[j, i]]
 
-    ll = np.log10(np.amax(V[:, m - 1]))
+    ll = np.log10(np.amax(V[m - 1, :]))
 
     return V, P, ll
 
 
+@jit.numba_njit
 def forwards_viterbi_hap_naive_low_mem(n, m, H, s, e, r):
     """Naive implementation of LS haploid Viterbi algorithm, with reduced memory."""
     # Initialise
     V, V_previous, P, r_n = viterbi_init(n, m, H, s, e, r)
 
     for j in range(1, m):
         for i in range(n):
             # Get the vector to maximise over
             v = np.zeros(n)
             for k in range(n):
                 v[k] = (
-                    e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
+                    e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
                     * V_previous[k]
                 )
                 if k == i:
-                    v[k] *= (1 - r[j]) + r_n[j]
+                    v[k] *= 1 - r[j] + r_n[j]
                 else:
                     v[k] *= r_n[j]
-            P[i, j] = np.argmax(v)
-            V[i] = v[P[i, j]]
+            P[j, i] = np.argmax(v)
+            V[i] = v[P[j, i]]
         V_previous = np.copy(V)
 
     ll = np.log10(np.amax(V))
 
     return V, P, ll
 
 
@@ -123,23 +122,23 @@
         c[j] = np.amax(V_previous)
         V_previous *= 1 / c[j]
         for i in range(n):
             # Get the vector to maximise over
             v = np.zeros(n)
             for k in range(n):
                 v[k] = (
-                    e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
+                    e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
                     * V_previous[k]
                 )
                 if k == i:
-                    v[k] *= (1 - r[j]) + r_n[j]
+                    v[k] *= 1 - r[j] + r_n[j]
                 else:
                     v[k] *= r_n[j]
-            P[i, j] = np.argmax(v)
-            V[i] = v[P[i, j]]
+            P[j, i] = np.argmax(v)
+            V[i] = v[P[j, i]]
 
         V_previous = np.copy(V)
 
     ll = np.sum(np.log10(c)) + np.log10(np.amax(V))
 
     return V, P, ll
 
@@ -154,85 +153,135 @@
     for j in range(1, m):
         argmax = np.argmax(V_previous)
         c[j] = V_previous[argmax]
         V_previous *= 1 / c[j]
         V = np.zeros(n)
         for i in range(n):
             V[i] = V_previous[i] * (1 - r[j] + r_n[j])
-            P[i, j] = i
+            P[j, i] = i
             if V[i] < r_n[j]:
                 V[i] = r_n[j]
-                P[i, j] = argmax
-
-            V[i] *= e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
+                P[j, i] = argmax
+            V[i] *= e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
         V_previous = np.copy(V)
 
     ll = np.sum(np.log10(c)) + np.log10(np.max(V))
 
     return V, P, ll
 
 
 @jit.numba_njit
 def forwards_viterbi_hap_lower_mem_rescaling(n, m, H, s, e, r):
     """LS haploid Viterbi algorithm with even smaller memory footprint and exploits the Markov process structure."""
     # Initialise
     V = np.zeros(n)
     for i in range(n):
-        V[i] = 1 / n * e[np.int64(np.equal(H[i, 0], s[0, 0]) or s[0, 0] == MISSING), 0]
-    P = np.zeros((n, m)).astype(np.int64)
-    P[:, 0] = 0
+        V[i] = 1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
+    P = np.zeros((m, n)).astype(np.int64)
     r_n = r / n
     c = np.ones(m)
 
     for j in range(1, m):
         argmax = np.argmax(V)
         c[j] = V[argmax]
         V *= 1 / c[j]
         for i in range(n):
             V[i] = V[i] * (1 - r[j] + r_n[j])
-            P[i, j] = i
+            P[j, i] = i
             if V[i] < r_n[j]:
                 V[i] = r_n[j]
-                P[i, j] = argmax
-            V[i] *= e[np.int64(np.equal(H[i, j], s[0, j]) or s[0, j] == MISSING), j]
+                P[j, i] = argmax
+            V[i] *= e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
 
     ll = np.sum(np.log10(c)) + np.log10(np.max(V))
 
     return V, P, ll
 
 
 @jit.numba_njit
+def forwards_viterbi_hap_lower_mem_rescaling_no_pointer(n, m, H, s, e, r):
+    """LS haploid Viterbi algorithm with even smaller memory footprint and exploits the Markov process structure."""
+    # Initialise
+    V = np.zeros(n)
+    for i in range(n):
+        V[i] = 1 / n * e[0, np.int64(np.equal(H[0, i], s[0, 0]) or s[0, 0] == MISSING)]
+    r_n = r / n
+    c = np.ones(m)
+    recombs = [
+        np.zeros(shape=0, dtype=np.int64) for _ in range(m)
+    ]  # This is going to be filled with the templates we can recombine to that have higher prob than staying where we are.
+
+    V_argmaxes = np.zeros(m)
+
+    for j in range(1, m):
+        argmax = np.argmax(V)
+        V_argmaxes[j - 1] = argmax
+        c[j] = V[argmax]
+        V *= 1 / c[j]
+        for i in range(n):
+            V[i] = V[i] * (1 - r[j] + r_n[j])
+            if V[i] < r_n[j]:
+                V[i] = r_n[j]
+                recombs[j] = np.append(
+                    recombs[j], i
+                )  # We add template i as a potential template to recombine to at site j.
+            V[i] *= e[j, np.int64(np.equal(H[j, i], s[0, j]) or s[0, j] == MISSING)]
+
+    V_argmaxes[m - 1] = np.argmax(V)
+    ll = np.sum(np.log10(c)) + np.log10(np.max(V))
+
+    return V, V_argmaxes, recombs, ll
+
+
+# Speedier version, variants x samples
+@jit.numba_njit
 def backwards_viterbi_hap(m, V_last, P):
     """Run a backwards pass to determine the most likely path."""
     # Initialise
     assert len(V_last.shape) == 1
     path = np.zeros(m).astype(np.int64)
     path[m - 1] = np.argmax(V_last)
 
     for j in range(m - 2, -1, -1):
-        path[j] = P[path[j + 1], j + 1]
+        path[j] = P[j + 1, path[j + 1]]
+
+    return path
+
+
+@jit.numba_njit
+def backwards_viterbi_hap_no_pointer(m, V_argmaxes, recombs):
+    """Run a backwards pass to determine the most likely path."""
+    # Initialise
+    path = np.zeros(m).astype(np.int64)
+    path[m - 1] = V_argmaxes[m - 1]
+
+    for j in range(m - 2, -1, -1):
+        current_best_template = path[j + 1]
+        if current_best_template in recombs[j + 1]:
+            current_best_template = V_argmaxes[j]
+        path[j] = current_best_template
 
     return path
 
 
 @jit.numba_njit
 def path_ll_hap(n, m, H, path, s, e, r):
     """Evaluate log-likelihood path through a reference panel which results in sequence s."""
-    index = np.int64(np.equal(H[path[0], 0], s[0, 0]) or s[0, 0] == MISSING)
-    log_prob_path = np.log10((1 / n) * e[index, 0])
+    index = np.int64(np.equal(H[0, path[0]], s[0, 0]) or s[0, 0] == MISSING)
+    log_prob_path = np.log10((1 / n) * e[0, index])
     old = path[0]
     r_n = r / n
 
     for l in range(1, m):
-        index = np.int64(np.equal(H[path[l], l], s[0, l]) or s[0, l] == MISSING)
+        index = np.int64(np.equal(H[l, path[l]], s[0, l]) or s[0, l] == MISSING)
         current = path[l]
         same = old == current
 
         if same:
             log_prob_path += np.log10((1 - r[l]) + r_n[l])
         else:
             log_prob_path += np.log10(r_n[l])
 
-        log_prob_path += np.log10(e[index, l])
+        log_prob_path += np.log10(e[l, index])
         old = current
 
     return log_prob_path
```

### Comparing `lshmm-0.0.4/setup.cfg` & `lshmm-0.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = lshmm
-version = 0.0.4
+version = 0.0.5
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
 classifiers = 
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 
 [options]
-package_dir = 
-	=.
-packages = find:
+packages = 
+	lshmm
+	lshmm.forward_backward
 install_requires = 
 	numba
 python_requires = >=3.7
 include_package_data = True
 
 [options.packages.find]
 where = .
```

### Comparing `lshmm-0.0.4/tests/test_API.py` & `lshmm-0.0.5/tests/test_API.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 # Python libraries
 import msprime
 import numpy as np
 import pytest
 import tskit
 
 import lshmm as ls
-import lshmm.forward_backward.fb_diploid_variants_samples as fbd_vs
-import lshmm.forward_backward.fb_haploid_variants_samples as fbh_vs
-import lshmm.vit_diploid_variants_samples as vd_vs
-import lshmm.vit_haploid_variants_samples as vh_vs
+import lshmm.forward_backward.fb_diploid as fbd
+import lshmm.forward_backward.fb_haploid as fbh
+import lshmm.vit_diploid as vd
+import lshmm.vit_haploid as vh
 
 EQUAL_BOTH_HOM = 4
 UNEQUAL_BOTH_HOM = 0
 BOTH_HET = 7
 REF_HOM_OBS_HET = 1
 REF_HET_OBS_HOM = 2
 
 MISSING = -1
 MISSING_INDEX = 3
 
 
 class LSBase:
     """Superclass of Li and Stephens tests."""
 
-    def example_haplotypes(self, ts, num_random=10, seed=42):
+    def example_haplotypes(self, ts, seed=42):
 
         H = ts.genotype_matrix()
         s = H[:, 0].reshape(1, H.shape[0])
         H = H[:, 1:]
 
         haplotypes = [s, H[:, -1].reshape(1, H.shape[0])]
         s_tmp = s.copy()
@@ -76,15 +76,15 @@
         e[:, REF_HET_OBS_HOM] = mu * (1 - mu)
         e[:, MISSING_INDEX] = 1
 
         return e
 
     def example_parameters_haplotypes(self, ts, seed=42, scale_mutation=True):
         """Returns an iterator over combinations of haplotype, recombination and
-        mutation rates."""
+        mutation probabilities."""
         np.random.seed(seed)
         H, haplotypes = self.example_haplotypes(ts)
         n = H.shape[1]
         m = ts.get_num_sites()
 
         # Here we have equal mutation and recombination
         r = np.zeros(m) + 0.01
@@ -111,15 +111,15 @@
             )
             e = self.haplotype_emission(
                 mu, m, n_alleles, scale_mutation_based_on_n_alleles=scale_mutation
             )
             yield n, m, H, s, e, r, mu
 
     def example_genotypes(self, ts, seed=42):
-
+        np.random.seed(seed)
         H = ts.genotype_matrix()
         s = H[:, 0].reshape(1, H.shape[0]) + H[:, 1].reshape(1, H.shape[0])
         H = H[:, 2:]
 
         genotypes = [
             s,
             H[:, -1].reshape(1, H.shape[0]) + H[:, -2].reshape(1, H.shape[0]),
@@ -170,15 +170,14 @@
             r[0] = 0
             e = self.genotype_emission(mu, m)
             yield n, m, G, s, e, r, mu
 
     def example_parameters_genotypes_larger(
         self, ts, seed=42, mean_r=1e-5, mean_mu=1e-5
     ):
-
         np.random.seed(seed)
         H, G, genotypes = self.example_genotypes(ts)
 
         m = ts.get_num_sites()
         n = H.shape[1]
 
         r = mean_r * np.ones(m) * ((np.random.rand(m) + 0.5) / 2)
@@ -235,39 +234,38 @@
 
 
 class TestMethodsHap(FBAlgorithmBase):
     """Test that we compute the sample likelihoods across all implementations."""
 
     def verify(self, ts):
         for n, m, H_vs, s, e_vs, r, mu in self.example_parameters_haplotypes(ts):
-            F_vs, c_vs, ll_vs = fbh_vs.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
-            B_vs = fbh_vs.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
-            F, c, ll = ls.forwards(H_vs, s, r, mutation_rate=mu)
-            B = ls.backwards(H_vs, s, c, r, mutation_rate=mu)
+            F_vs, c_vs, ll_vs = fbh.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
+            B_vs = fbh.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
+            F, c, ll = ls.forwards(H_vs, s, r, p_mutation=mu)
+            B = ls.backwards(H_vs, s, c, r, p_mutation=mu)
             self.assertAllClose(F, F_vs)
             self.assertAllClose(B, B_vs)
             self.assertAllClose(ll_vs, ll)
-
             mu = None
             F, c, ll = ls.forwards(H_vs, s, r, mu)
             B = ls.backwards(H_vs, s, c, r, mu)
 
 
 class TestMethodsDip(FBAlgorithmBase):
     """Test that we compute the sample likelihoods across all implementations."""
 
     def verify(self, ts):
         for n, m, G_vs, s, e_vs, r, mu in self.example_parameters_genotypes(ts):
 
-            F_vs, c_vs, ll_vs = fbd_vs.forward_ls_dip_loop(
+            F_vs, c_vs, ll_vs = fbd.forward_ls_dip_loop(
                 n, m, G_vs, s, e_vs, r, norm=True
             )
-            F, c, ll = ls.forwards(G_vs, s, r, mutation_rate=mu)
-            B_vs = fbd_vs.backward_ls_dip_loop(n, m, G_vs, s, e_vs, c_vs, r)
-            B = ls.backwards(G_vs, s, c, r, mutation_rate=mu)
+            F, c, ll = ls.forwards(G_vs, s, r, p_mutation=mu)
+            B_vs = fbd.backward_ls_dip_loop(n, m, G_vs, s, e_vs, c_vs, r)
+            B = ls.backwards(G_vs, s, c, r, p_mutation=mu)
             self.assertAllClose(F, F_vs)
             self.assertAllClose(B, B_vs)
             self.assertAllClose(ll_vs, ll)
 
 
 class VitAlgorithmBase(LSBase):
     """Base for viterbi algoritm tests."""
@@ -275,32 +273,30 @@
 
 class TestViterbiHap(VitAlgorithmBase):
     """Test that we have the same log-likelihood across all implementations"""
 
     def verify(self, ts):
         for n, m, H_vs, s, e_vs, r, mu in self.example_parameters_haplotypes(ts):
 
-            V_vs, P_vs, ll_vs = vh_vs.forwards_viterbi_hap_lower_mem_rescaling(
+            V_vs, P_vs, ll_vs = vh.forwards_viterbi_hap_lower_mem_rescaling(
                 n, m, H_vs, s, e_vs, r
             )
-            path_vs = vh_vs.backwards_viterbi_hap(m, V_vs, P_vs)
-            path, ll = ls.viterbi(H_vs, s, r, mutation_rate=mu)
+            path_vs = vh.backwards_viterbi_hap(m, V_vs, P_vs)
+            path, ll = ls.viterbi(H_vs, s, r, p_mutation=mu)
 
             self.assertAllClose(ll_vs, ll)
             self.assertAllClose(path_vs, path)
 
 
 class TestViterbiDip(VitAlgorithmBase):
     """Test that we have the same log-likelihood across all implementations"""
 
     def verify(self, ts):
         for n, m, G_vs, s, e_vs, r, mu in self.example_parameters_genotypes(ts):
 
-            V_vs, P_vs, ll_vs = vd_vs.forwards_viterbi_dip_low_mem(
-                n, m, G_vs, s, e_vs, r
-            )
-            path_vs = vd_vs.backwards_viterbi_dip(m, V_vs, P_vs)
-            phased_path_vs = vd_vs.get_phased_path(n, path_vs)
-            path, ll = ls.viterbi(G_vs, s, r, mutation_rate=mu)
+            V_vs, P_vs, ll_vs = vd.forwards_viterbi_dip_low_mem(n, m, G_vs, s, e_vs, r)
+            path_vs = vd.backwards_viterbi_dip(m, V_vs, P_vs)
+            phased_path_vs = vd.get_phased_path(n, path_vs)
+            path, ll = ls.viterbi(G_vs, s, r, p_mutation=mu)
 
             self.assertAllClose(ll_vs, ll)
             self.assertAllClose(phased_path_vs, path)
```

### Comparing `lshmm-0.0.4/tests/test_API_multiallelic.py` & `lshmm-0.0.5/tests/test_API_multiallelic.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # Python libraries
 import msprime
 import numpy as np
 import pytest
 import tskit
 
 import lshmm as ls
-import lshmm.forward_backward.fb_diploid_variants_samples as fbd_vs
-import lshmm.forward_backward.fb_haploid_variants_samples as fbh_vs
-import lshmm.vit_diploid_variants_samples as vd_vs
-import lshmm.vit_haploid_variants_samples as vh_vs
+import lshmm.forward_backward.fb_diploid as fbd
+import lshmm.forward_backward.fb_haploid as fbh
+import lshmm.vit_diploid as vd
+import lshmm.vit_haploid as vh
 
 EQUAL_BOTH_HOM = 4
 UNEQUAL_BOTH_HOM = 0
 BOTH_HET = 7
 REF_HOM_OBS_HET = 1
 REF_HET_OBS_HOM = 2
 
@@ -64,15 +64,15 @@
                 else:
                     e[j, 0] = mu[j] / (n_alleles[j] - 1)
                     e[j, 1] = 1 - mu[j]
         return e
 
     def example_parameters_haplotypes(self, ts, seed=42, scale_mutation=True):
         """Returns an iterator over combinations of haplotype, recombination and
-        mutation rates."""
+        mutation probabilities."""
         np.random.seed(seed)
         H, haplotypes = self.example_haplotypes(ts)
         n = H.shape[1]
         m = ts.get_num_sites()
 
         # Here we have equal mutation and recombination
         r = np.zeros(m) + 0.01
@@ -171,33 +171,33 @@
 
 
 class TestMethodsHap(FBAlgorithmBase):
     """Test that we compute the sample likelihoods across all implementations."""
 
     def verify(self, ts):
         for n, m, H_vs, s, e_vs, r, mu in self.example_parameters_haplotypes(ts):
-            F_vs, c_vs, ll_vs = fbh_vs.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
-            B_vs = fbh_vs.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
-            F, c, ll = ls.forwards(H_vs, s, r, mutation_rate=mu)
-            B = ls.backwards(H_vs, s, c, r, mutation_rate=mu)
+            F_vs, c_vs, ll_vs = fbh.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
+            B_vs = fbh.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
+            F, c, ll = ls.forwards(H_vs, s, r, p_mutation=mu)
+            B = ls.backwards(H_vs, s, c, r, p_mutation=mu)
             self.assertAllClose(F, F_vs)
             self.assertAllClose(B, B_vs)
             # print(e_vs)
             self.assertAllClose(ll_vs, ll)
 
         for n, m, H_vs, s, e_vs, r, mu in self.example_parameters_haplotypes(
             ts, scale_mutation=False
         ):
-            F_vs, c_vs, ll_vs = fbh_vs.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
-            B_vs = fbh_vs.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
+            F_vs, c_vs, ll_vs = fbh.forwards_ls_hap(n, m, H_vs, s, e_vs, r)
+            B_vs = fbh.backwards_ls_hap(n, m, H_vs, s, e_vs, c_vs, r)
             F, c, ll = ls.forwards(
-                H_vs, s, r, mutation_rate=mu, scale_mutation_based_on_n_alleles=False
+                H_vs, s, r, p_mutation=mu, scale_mutation_based_on_n_alleles=False
             )
             B = ls.backwards(
-                H_vs, s, c, r, mutation_rate=mu, scale_mutation_based_on_n_alleles=False
+                H_vs, s, c, r, p_mutation=mu, scale_mutation_based_on_n_alleles=False
             )
             self.assertAllClose(F, F_vs)
             self.assertAllClose(B, B_vs)
             self.assertAllClose(ll_vs, ll)
 
 
 class VitAlgorithmBase(LSBase):
@@ -206,17 +206,17 @@
 
 class TestViterbiHap(VitAlgorithmBase):
     """Test that we have the same log-likelihood across all implementations"""
 
     def verify(self, ts):
         for n, m, H_vs, s, e_vs, r, mu in self.example_parameters_haplotypes(ts):
 
-            V_vs, P_vs, ll_vs = vh_vs.forwards_viterbi_hap_lower_mem_rescaling(
+            V_vs, P_vs, ll_vs = vh.forwards_viterbi_hap_lower_mem_rescaling(
                 n, m, H_vs, s, e_vs, r
             )
-            path_vs = vh_vs.backwards_viterbi_hap(m, V_vs, P_vs)
-            path_ll_hap = vh_vs.path_ll_hap(n, m, H_vs, path_vs, s, e_vs, r)
-            path, ll = ls.viterbi(H_vs, s, r, mutation_rate=mu)
+            path_vs = vh.backwards_viterbi_hap(m, V_vs, P_vs)
+            path_ll_hap = vh.path_ll_hap(n, m, H_vs, path_vs, s, e_vs, r)
+            path, ll = ls.viterbi(H_vs, s, r, p_mutation=mu)
 
             self.assertAllClose(ll_vs, ll)
             self.assertAllClose(ll_vs, path_ll_hap)
             self.assertAllClose(path_vs, path)
```

