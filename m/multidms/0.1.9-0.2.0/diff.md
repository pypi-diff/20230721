# Comparing `tmp/multidms-0.1.9-py3-none-any.whl.zip` & `tmp/multidms-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 35664 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1897 b- defN 23-Jul-18 22:51 multidms/__init__.py
--rw-r--r--  2.0 unx    13845 b- defN 23-Jul-18 22:51 multidms/biophysical.py
--rw-r--r--  2.0 unx    21658 b- defN 23-Jul-18 22:51 multidms/data.py
--rw-r--r--  2.0 unx    41562 b- defN 23-Jul-18 22:51 multidms/model.py
--rw-r--r--  2.0 unx    31052 b- defN 23-Jul-18 22:51 multidms/plot.py
--rw-r--r--  2.0 unx     9924 b- defN 23-Jul-18 22:51 multidms/utils.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Jul-18 22:53 multidms-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     3730 b- defN 23-Jul-18 22:53 multidms-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 22:53 multidms-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-18 22:53 multidms-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-Jul-18 22:53 multidms-0.1.9.dist-info/RECORD
-11 files, 125709 bytes uncompressed, 34260 bytes compressed:  72.7%
+Zip file size: 36831 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1995 b- defN 23-Jul-21 21:41 multidms/__init__.py
+-rw-r--r--  2.0 unx    13851 b- defN 23-Jul-21 21:41 multidms/biophysical.py
+-rw-r--r--  2.0 unx    24850 b- defN 23-Jul-21 21:41 multidms/data.py
+-rw-r--r--  2.0 unx    42354 b- defN 23-Jul-21 21:41 multidms/model.py
+-rw-r--r--  2.0 unx    31292 b- defN 23-Jul-21 21:41 multidms/plot.py
+-rw-r--r--  2.0 unx     9969 b- defN 23-Jul-21 21:41 multidms/utils.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4072 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/RECORD
+11 files, 130424 bytes uncompressed, 35427 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: multidms/plot.py
 Comment: 
 
 Filename: multidms/utils.py
 Comment: 
 
-Filename: multidms-0.1.9.dist-info/LICENSE
+Filename: multidms-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: multidms-0.1.9.dist-info/METADATA
+Filename: multidms-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: multidms-0.1.9.dist-info/WHEEL
+Filename: multidms-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: multidms-0.1.9.dist-info/top_level.txt
+Filename: multidms-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: multidms-0.1.9.dist-info/RECORD
+Filename: multidms-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## multidms/__init__.py

```diff
@@ -49,20 +49,23 @@
 
  - :const:`~multidms.alphabets.AAS_WITHSTOP_WITHGAP`
 
 """
 
 __author__ = "Jared Galloway"
 __email__ = "jgallowa@fredhutch.org"
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 __url__ = "https://github.com/matsengrp/multidms"
 
 from polyclonal.alphabets import AAS  # noqa: F401
 from polyclonal.alphabets import AAS_WITHGAP  # noqa: F401
 from polyclonal.alphabets import AAS_WITHSTOP  # noqa: F401
 from polyclonal.alphabets import AAS_WITHSTOP_WITHGAP  # noqa: F401
 
 from multidms.data import Data  # noqa: F401
 from multidms.model import Model  # noqa: F401
 
 import multidms.biophysical  # noqa: F401
 import multidms.utils  # noqa: F401
+
+# This lets Sphinx know you want to document foo.foo.Foo as foo.Foo.
+__all__ = ["Data", "Model"]
```

## multidms/biophysical.py

```diff
@@ -177,15 +177,15 @@
 
     Where:
 
     - :math:`n` is the number of units in the hidden layer.
     - :math:`w^{l}_{i}` and :math:`w^{o}_{i}` are free parameters representing latent
       and output tranformations, respectively, associated with unit `i` in the
       hidden layer of the network.
-    - :math:`b^{l}_{i}` is a free parameter, as an added bias term to unit $i$.
+    - :math:`b^{l}_{i}` is a free parameter, as an added bias term to unit `i`.
     - :math:`b^{o}` is a constant, singular free parameter.
 
     .. Note::
         This is an advanced feature and we advise against its use
         unless the other options are not sufficiently parameterized for particularly
         complex experimental conditions.
 
@@ -230,16 +230,16 @@
     The rate of change at the hinge is defined by 'hinge_scale'.
 
     In essence, this is a modified _softplus_ activation,
     (:math:`\text{softplus}(x)=\log(1 + e^{x})`)
     with a lower bound at :math:`l + \gamma_{h}`,
     as well as a ramping coefficient, :math:`\lambda_{\text{sp}}`.
 
-    Concretely, if we let $z' = g(\phi_d(v))$, then the predicted functional score of
-    our model is given by:
+    Concretely, if we let :math:`z' = g(\phi_d(v))`, then the predicted functional score
+    of our model is given by:
 
     .. math::
         t(z') = \lambda_{sp}\log(1 + e^{\frac{z' - l}{\lambda_{sp}}}) + l
 
     Functionally speaking, this truncates scores below a lower bound,
     while leaving scores above (mostly) unaltered.
     There is a small range of input values where the function smoothly
```

## multidms/data.py

```diff
@@ -9,15 +9,15 @@
 
 import os
 from functools import partial
 import warnings
 
 import binarymap as bmap
 import numpy as onp
-import pandas
+import pandas as pd
 from polyclonal.plot import DEFAULT_POSITIVE_COLORS
 from polyclonal.utils import MutationParser
 from tqdm.auto import tqdm
 
 from multidms import AAS
 from multidms.utils import split_subs
 
@@ -34,54 +34,55 @@
 
 
 class Data:
     r"""
     Prep and store one-hot encoding of
     variant substitutions data.
     Individual objects of this type can be shared
-    by multiple ``multidms.Model`` Objects
+    by multiple :py:class:`multidms.Model` Objects
     for effeciently fitting various models to the same data.
 
     Note
     ----
-    You can initialize a :class:`Data` object with a ``pd.DataFrame``
+    You can initialize a :class:`Data` object with a :class:`pandas.DataFrame`
     with a row for each variant sampled and annotations
     provided in the required columns:
 
     1. `condition` - Experimental condition from
         which a sample measurement was obtained.
     2. `aa_substitutions` - Defines each variant
-        :math:`v` as a string of substitutions (e.g., 'M3A K5G').
+        :math:`v` as a string of substitutions (e.g., ``'M3A K5G'``).
         Note that while conditions may have differing wild types
         at a given site, the sites between conditions should reference
         the same site when alignment is performed between
         condition wild types.
     3. `func_score` - The functional score computed from experimental
         measurements.
 
     Parameters
     ----------
-    variants_df : pandas.DataFrame or None
+    variants_df : :class:`pandas.DataFrame` or None
         The variant level information from all experiments you
-        wish to analyze. Should have columns named 'condition',
-        'aa_substitutions', and 'func_score'.
+        wish to analyze. Should have columns named ``'condition'``,
+        ``'aa_substitutions'``, and ``'func_score'``.
         See the class note for descriptions of each of the features.
     reference : str
         Name of the condition which annotates the reference.
         variants. Note that for model fitting this class will convert all
         amino acid substitutions for non-reference condition groups
         to relative to the reference condition.
         For example, if the wild type amino acid at site 30 is an
         A in the reference condition, and a G in a non-reference condition,
         then a Y30G mutation in the non-reference condition is recorded as an A30G
         mutation relative to the reference. This way, each condition informs
         the exact same parameters, even at sites that differ in wild type amino acid.
-        These are encoded in a ``BinaryMap`` object for each condtion,
+        These are encoded in a :class:`binarymap.binarymap.BinaryMap` object for each
+        condtion,
         where all sites that are non-identical to the reference are 1's.
-        For motivation, see the `Model overview` section in `multidms.Model`
+        For motivation, see the `Model overview` section in :class:`multidms.Model`
         class notes.
     collapse_identical_variants : {'mean', 'median', False}
         If identical variants in ``variants_df`` (same 'aa_substitutions'),
         exist within individual condition groups,
         collapse them by taking mean or median of 'func_score', or
         (if `False`) do not collapse at all. Collapsing will make fitting faster,
         but *not* a good idea if you are doing bootstrapping.
@@ -95,108 +96,110 @@
         by each condition, or an array of colors that are sequentially assigned
         to the conditions.
     letter_suffixed_sites: bool
         True if sites are sequential and integer, False otherwise.
 
     Example
     -------
-    Simple example with two conditions (`1` and `2`)
+    Simple example with two conditions (``'a'`` and ``'b'``)
 
     >>> import pandas as pd
     >>> import multidms
     >>> func_score_data = {
     ...     'condition' : ["a","a","a","a", "b","b","b","b","b","b"],
     ...     'aa_substitutions' : [
-                'M1E', 'G3R', 'G3P', 'M1W', 'M1E',
-                'P3R', 'P3G', 'M1E P3G', 'M1E P3R', 'P2T'
-            ],
+    ...         'M1E', 'G3R', 'G3P', 'M1W', 'M1E',
+    ...         'P3R', 'P3G', 'M1E P3G', 'M1E P3R', 'P2T'
+    ...     ],
     ...     'func_score' : [2, -7, -0.5, 2.3, 1, -5, 0.4, 2.7, -2.7, 0.3],
     ... }
     >>> func_score_df = pd.DataFrame(func_score_data)
-    >>> func_score_df
-      condition aa_substitutions  func_score
-      0         1              M1E         2.0
-      1         1              G3R        -7.0
-      2         1              G3P        -0.5
-      3         1              M1W         2.3
-      4         2              M1E         1.0
-      5         2              P3R        -5.0
-      6         2              P3G         0.4
-      7         2          M1E P3G         2.7
-      8         2          M1E P3R        -2.7
-      9         2              P2T         0.3
+    >>> func_score_df  # doctest: +NORMALIZE_WHITESPACE
+    condition aa_substitutions  func_score
+    0         a              M1E         2.0
+    1         a              G3R        -7.0
+    2         a              G3P        -0.5
+    3         a              M1W         2.3
+    4         b              M1E         1.0
+    5         b              P3R        -5.0
+    6         b              P3G         0.4
+    7         b          M1E P3G         2.7
+    8         b          M1E P3R        -2.7
+    9         b              P2T         0.3
 
     Instantiate a ``Data`` Object allowing for stop codon variants
-    and declaring condition '1' as the reference condition.
+    and declaring condition `"a"` as the reference condition.
 
     >>> data = multidms.Data(
     ...     func_score_df,
     ...     alphabet = multidms.AAS_WITHSTOP,
-    ...     reference = "a"
-    ... )
+    ...     reference = "a",
+    ... )  # doctest: +ELLIPSIS
+    INFO: Pandarallel will run on ... workers.
+    ...
 
     Note this may take some time due to the string
     operations that must be performed when converting
     amino acid substitutions to be with respect to a
     reference wild type sequence.
 
     After the object has finished being instantiated,
     we now have access to a few 'static' properties
     of our data. See individual property docstrings
     for more information.
 
     >>> data.reference
-    '1'
+    'a'
 
     >>> data.conditions
-    ('1', '2')
+    ('a', 'b')
 
     >>> data.mutations
     ('M1E', 'M1W', 'G3P', 'G3R')
 
-    >>> data.site_map
-       1  2
-       3  G  P
-       1  M  M
+    >>> data.site_map  # doctest: +NORMALIZE_WHITESPACE
+    a  b
+    1  M  M
+    3  G  P
 
-    >>> data.mutations_df
-      mutation wts  sites muts  times_seen_1  times_seen_2
+    >>> data.mutations_df  # doctest: +NORMALIZE_WHITESPACE
+      mutation wts  sites muts  times_seen_a  times_seen_b
     0      M1E   M      1    E             1           3.0
     1      M1W   M      1    W             1           0.0
     2      G3P   G      3    P             1           1.0
     3      G3R   G      3    R             1           2.0
 
-    >>> data.variants_df
-      condition aa_substitutions  weight  func_score var_wrt_ref
-    0         1              G3P       1        -0.5         G3P
-    1         1              G3R       1        -7.0         G3R
-    2         1              M1E       1         2.0         M1E
-    3         1              M1W       1         2.3         M1W
-    4         2              M1E       1         1.0     G3P M1E
-    5         2          M1E P3G       1         2.7         M1E
-    6         2          M1E P3R       1        -2.7     G3R M1E
-    8         2              P3G       1         0.4
-    9         2              P3R       1        -5.0         G3R
+    >>> data.variants_df  # doctest: +NORMALIZE_WHITESPACE
+      condition aa_substitutions  func_score var_wrt_ref
+    0         a              M1E         2.0         M1E
+    1         a              G3R        -7.0         G3R
+    2         a              G3P        -0.5         G3P
+    3         a              M1W         2.3         M1W
+    4         b              M1E         1.0     G3P M1E
+    5         b              P3R        -5.0         G3R
+    6         b              P3G         0.4
+    7         b          M1E P3G         2.7         M1E
+    8         b          M1E P3R        -2.7     G3R M1E
     """
 
     def __init__(
         self,
-        variants_df: pandas.DataFrame,
+        variants_df: pd.DataFrame,
         reference: str,
         alphabet=AAS,
         collapse_identical_variants=False,
         condition_colors=DEFAULT_POSITIVE_COLORS,
         letter_suffixed_sites=False,
         assert_site_integrity=False,
         verbose=False,
         nb_workers=None,
     ):
         """See main class docstring."""
         # Check and initialize conditions attribute
-        if pandas.isnull(variants_df["condition"]).any():
+        if pd.isnull(variants_df["condition"]).any():
             raise ValueError("condition name cannot be null")
         if variants_df["condition"].dtype.kind in "biufc":
             warnings.warn(
                 "condition column looks to be numeric type, converting to string",
                 UserWarning,
             )
         self._conditions = tuple(variants_df["condition"].astype(str).unique())
@@ -261,89 +264,161 @@
         self._split_subs = partial(split_subs, parser=self._mutparser.parse_mut)
         df["wts"], df["sites"], df["muts"] = zip(
             *df["aa_substitutions"].map(self._split_subs)
         )
 
         # Use the "aa_substitutions" to infer the
         # wild type for each condition
-        site_map = pandas.DataFrame()
+        site_map = pd.DataFrame()
         for hom, hom_func_df in df.groupby("condition"):
             if verbose:
                 print(f"inferring site map for {hom}")
-            for idx, row in hom_func_df.iterrows():
+            for idx, row in tqdm(
+                hom_func_df.iterrows(), total=len(hom_func_df), disable=not verbose
+            ):
                 for wt, site in zip(row.wts, row.sites):
                     site_map.loc[site, hom] = wt
 
         if assert_site_integrity:
             if verbose:
                 print("Asserting site integrity")
             for hom, hom_func_df in df.groupby("condition"):
-                for idx, row in hom_func_df.iterrows():
+                for idx, row in tqdm(
+                    hom_func_df.iterrows(), total=len(hom_func_df), disable=not verbose
+                ):
                     for wt, site in zip(row.wts, row.sites):
                         assert site_map.loc[site, hom] == wt
 
         # Throw variants if they contain non overlapping
         # mutations with all other conditions.
         na_rows = site_map.isna().any(axis=1)
         sites_to_throw = na_rows[na_rows].index
         site_map.dropna(inplace=True)
 
-        nb_workers = os.cpu_count() if not nb_workers else nb_workers
+        nb_workers = min(os.cpu_count(), 4) if nb_workers is None else nb_workers
         pandarallel.initialize(progress_bar=verbose, nb_workers=nb_workers)
 
         def flags_invalid_sites(disallowed_sites, sites_list):
             """Check to see if a sites list contains
             any disallowed sites
             """
             for site in sites_list:
                 if site in disallowed_sites:
                     return False
             return True
 
-        df["allowed_variant"] = df.sites.apply(
+        df["allowed_variant"] = df.sites.parallel_apply(
             lambda sl: flags_invalid_sites(sites_to_throw, sl)
         )
-        len(df)
-        df = df[df["allowed_variant"]]
+        if verbose:
+            print(
+                f"unknown cond wildtype at sites: {list(sites_to_throw.values)},"
+                f"\ndropping: {len(df) - len(df[df['allowed_variant']])} variants"
+                "which have mutations at those sites."
+            )
+
+        df.query("allowed_variant", inplace=True)
         df.drop("allowed_variant", axis=1, inplace=True)
+        site_map.sort_index(inplace=True)
 
-        self._site_map = site_map.sort_index()
+        def get_nis_from_site_map(site_map):
+            """Get non-identical sites from a site map"""
+            non_identical_sites = {}
+            reference_sequence_conditions = [self._reference]
+            for condition in self._conditions:
+                if condition == self._reference:
+                    non_identical_sites[condition] = []
+                    continue
+
+                nis = site_map.where(
+                    site_map[self.reference] != site_map[condition],
+                ).dropna()
+
+                if len(nis) == 0:
+                    non_identical_sites[condition] = []
+                    reference_sequence_conditions.append(condition)
+                else:
+                    non_identical_sites[condition] = nis[[self._reference, condition]]
+            return non_identical_sites, reference_sequence_conditions
 
-        # identify and write site map differences for each condition
-        non_identical_mutations = {}
-        non_identical_sites = {}
-        self._reference_sequence_conditions = [self._reference]
-        for condition in self._conditions:
-            if condition == self._reference:
-                non_identical_mutations[condition] = ""
-                non_identical_sites[condition] = []
+        (non_identical_sites, reference_sequence_conditions) = get_nis_from_site_map(
+            site_map
+        )
+
+        # invalid nis see https://github.com/matsengrp/multidms/issues/84
+        observed_ref_muts = (
+            df.query("condition == @self.reference")
+            .aa_substitutions.str.split()
+            .explode()
+            .unique()
+        )
+        invalid_nim = []
+        for condition in self.conditions:
+            if (
+                condition == self.reference
+                or condition in reference_sequence_conditions
+            ):
                 continue
+            observed_cond_muts = (
+                df.query("condition == @condition")
+                .aa_substitutions.str.split()
+                .explode()
+                .unique()
+            )
+            for site, cond_wts in non_identical_sites[condition].iterrows():
+                ref_wt, cond_wt = cond_wts[self.reference], cond_wts[condition]
+                forward_mut = f"{ref_wt}{site}{cond_wt}"
+                reversion_mut = f"{cond_wt}{site}{ref_wt}"
+
+                condition_1 = forward_mut in observed_ref_muts
+                condition_2 = reversion_mut in observed_cond_muts
+                if not (condition_1 and condition_2):
+                    invalid_nim.append(site)
+
+        # find variants that contain mutations at invalid sites
+        df["allowed_variant"] = df.sites.parallel_apply(
+            lambda sl: flags_invalid_sites(invalid_nim, sl)
+        )
+        if verbose:
+            print(
+                f"invalid non-identical-sites: {invalid_nim}, dropping "
+                f"{len(df) - len(df[df['allowed_variant']])} variants"
+            )
 
-            nis = self._site_map.where(
-                self._site_map[self.reference] != self.site_map[condition],
-            ).dropna()
+        # drop variants that contain mutations at invalid sites
+        df.query("allowed_variant", inplace=True)
+        df.drop("allowed_variant", axis=1, inplace=True)
 
-            if len(nis) == 0:
-                non_identical_mutations[condition] = ""
-                non_identical_sites[condition] = []
-                self._reference_sequence_conditions.append(condition)
-            else:
-                muts = nis[self._reference] + nis.index.astype(str) + nis[condition]
-                muts_string = " ".join(muts.values)
-                non_identical_mutations[condition] = muts_string
-                non_identical_sites[condition] = nis[[self._reference, condition]]
+        # drop invalid sites from site map
+        self._site_map = site_map.drop(invalid_nim, inplace=False)
 
+        # recompute non-identical sites for static property
+        (
+            self._non_identical_sites,
+            self._reference_sequence_conditions,
+        ) = get_nis_from_site_map(self._site_map)
+
+        # compute the static non_identical_mutations property
+        non_identical_mutations = {}
+        for condition in self.conditions:
+            if condition in self.reference_sequence_conditions:
+                non_identical_mutations[condition] = ""
+                continue
+            nis = self.non_identical_sites[condition]
+            muts = nis[self.reference] + nis.index.astype(str) + nis[condition]
+            muts_string = " ".join(muts.values)
+            non_identical_mutations[condition] = muts_string
         self._non_identical_mutations = non_identical_mutations
-        self._non_identical_sites = non_identical_sites
 
+        # compute all substitution conversions for all conditions which
+        # do not share the reference sequence
         df = df.assign(var_wrt_ref=df["aa_substitutions"])
         for condition, condition_func_df in df.groupby("condition"):
             if verbose:
                 print(f"Converting mutations for {condition}")
-
             if condition in self.reference_sequence_conditions:
                 if verbose:
                     print("is reference, skipping")
                 continue
 
             idx = condition_func_df.index
             df.loc[idx, "var_wrt_ref"] = condition_func_df.parallel_apply(
@@ -371,15 +446,15 @@
         df.drop(["wts", "sites", "muts"], axis=1, inplace=True)
         self._variants_df = df
         self._training_data = {"X": X, "y": y}
         self._binarymaps = binmaps
         self._mutations = tuple(ref_bmap.all_subs)
 
         # initialize single mutational effects df
-        mut_df = pandas.DataFrame({"mutation": self._mutations})
+        mut_df = pd.DataFrame({"mutation": self._mutations})
 
         mut_df["wts"], mut_df["sites"], mut_df["muts"] = zip(
             *mut_df["mutation"].map(self._mutparser.parse_mut)
         )
 
         # compute times seen in data
         for condition, condition_vars in self._variants_df.groupby("condition"):
@@ -411,25 +486,25 @@
         """
         A tuple of all mutations in the order reletive to their index into
         the binarymap.
         """
         return self._mutations
 
     @property
-    def mutations_df(self) -> pandas.DataFrame:
+    def mutations_df(self) -> pd.DataFrame:
         """A dataframe summarizing all single mutations"""
         return self._mutations_df
 
     @property
-    def variants_df(self) -> pandas.DataFrame:
+    def variants_df(self) -> pd.DataFrame:
         """A dataframe summarizing all variants in the training data."""
         return self._variants_df
 
     @property
-    def site_map(self) -> pandas.DataFrame:
+    def site_map(self) -> pd.DataFrame:
         """
         A dataframe indexed by site, with columns
         for all conditions giving the wild type amino acid
         at each site.
         """
         return self._site_map
 
@@ -442,15 +517,15 @@
         """
         return self._non_identical_mutations
 
     @property
     def non_identical_sites(self) -> dict:
         """
         A dictionary keyed by condition names with values
-        being a pandas.DataFrame indexed by site,
+        being a :class:`pandas.DataFrame` indexed by site,
         with columns for the reference
         and non-reference amino acid at each site that differs.
         """
         return self._non_identical_sites
 
     @property
     def reference_sequence_conditions(self) -> list:
```

## multidms/model.py

```diff
@@ -82,97 +82,122 @@
     init_theta_scale : float
         Initialize the scaling parameter :math:`\theta_{\text{scale}}` of
         a two-parameter epistatic model (Sigmoid or Softplus).
     init_theta_bias : float
         Initialize the bias parameter :math:`\theta_{\text{bias}}` of
         a two parameter epistatic model (Sigmoid or Softplus).
     n_hidden_units : int or None
-        If using `biophysical.multidms.biophysical.nn_global_epistasis`
+        If using :func:`multidms.biophysical.nn_global_epistasis`
         as the epistatic model, this is the number of hidden units
         used in the transform.
     lower_bound : float or None
-        If using `biophysical.multidms.biophysical.softplus_activation`
+        If using :func:`multidms.biophysical.softplus_activation`
         as the output activation, this is the lower bound of the
         softplus function.
 
     Example
     -------
-    To create a ``Model`` object, all you need is
-    the respective ``Data`` object for parameter fitting.
+    To create a :class:`Model` object, all you need is
+    the respective :class:`Data` object for parameter fitting.
 
+    >>> import multidms
+    >>> from tests.test_data import data
     >>> model = multidms.Model(data)
 
     Upon initialization, you will now have access to the underlying data
     and parameters.
 
     >>> model.data.mutations
     ('M1E', 'M1W', 'G3P', 'G3R')
     >>> model.data.conditions
-    ('1', '2')
+    ('a', 'b')
     >>> model.data.reference
-    '1'
+    'a'
     >>> model.data.condition_colors
-    {'1': '#0072B2', '2': '#009E73'}
+    {'a': '#0072B2', 'b': '#CC79A7'}
 
     The mutations_df and variants_df may of course also be accessed.
+    First, we set pandas to display all rows and columns.
 
-    >>> model.data.mutations_df
-      mutation wts  sites muts  times_seen_1  times_seen_2
+    >>> import pandas as pd
+    >>> pd.set_option('display.max_rows', None)
+    >>> pd.set_option('display.max_columns', None)
+
+    >>> model.data.mutations_df  # doctest: +NORMALIZE_WHITESPACE
+      mutation wts  sites muts  times_seen_a  times_seen_b
     0      M1E   M      1    E             1           3.0
     1      M1W   M      1    W             1           0.0
     2      G3P   G      3    P             1           1.0
     3      G3R   G      3    R             1           2.0
 
-    However, if accessed directly through the Model object, you will
+    However, if accessed directly through the :class:`Model` object, you will
     get the same information, along with model/parameter specific
     features included. These are automatically updated each time you
     request the property.
 
-    >>> model.mutations_df
-      mutation wts  sites muts  times_seen_1  ... beta  shift_1  F_1        shift_2   F_2
-    0      M1E   M      1    E             1  ...  0.080868  0.0 -0.030881  0.0 -0.030881
-    1      M1W   M      1    W             1  ... -0.386247  0.0 -0.049086  0.0 -0.049086
-    2      G3P   G      3    P             1  ... -0.375656  0.0 -0.048574  0.0 -0.048574
-    3      G3R   G      3    R             1  ...  1.668974  0.0 -0.006340  0.0 -0.006340
-
-    Notice the respective single mutation effects ("beta"), conditional shifts (shift_d),
-    and predicted functional score (F_d) of each mutation in the model are now
+    >>> model.mutations_df  # doctest: +NORMALIZE_WHITESPACE
+      mutation wts  sites muts  times_seen_a  times_seen_b      beta  \
+    0      M1E   M      1    E             1           3.0  0.080868   
+    1      M1W   M      1    W             1           0.0 -0.386247   
+    2      G3P   G      3    P             1           1.0 -0.375656   
+    3      G3R   G      3    R             1           2.0  1.668974   
+    <BLANKLINE>
+       predicted_func_score  shift_b  
+    0             -2.398970      0.0  
+    1             -2.976895      0.0  
+    2             -2.964124      0.0  
+    3             -0.792805      0.0  
+
+    Notice the respective single mutation effects (``"beta"``), conditional shifts
+    (``shift_d``),
+    and predicted functional score (``F_d``) of each mutation in the model are now
     easily accessible. Similarly, we can take a look at the variants_df for the model,
 
-    >>> model.variants_df
-      condition aa_substitutions  ...  predicted_func_score  corrected_func_score
-    0         1              G3P  ...             -0.048574                  -0.5
-    1         1              G3R  ...             -0.006340                  -7.0
-    2         1              M1E  ...             -0.030881                   2.0
-    3         1              M1W  ...             -0.049086                   2.3
-    4         2              M1E  ...             -0.044834                   1.0
-    5         2          M1E P3G  ...             -0.030881                   2.7
-    6         2          M1E P3R  ...             -0.005848                  -2.7
-    8         2              P3G  ...             -0.033464                   0.4
-    9         2              P3R  ...             -0.006340                  -5.0
+    >>> model.variants_df  # doctest: +NORMALIZE_WHITESPACE
+      condition aa_substitutions  func_score var_wrt_ref  predicted_latent  \
+    0         a              M1E         2.0         M1E          0.080868   
+    1         a              G3R        -7.0         G3R          1.668974   
+    2         a              G3P        -0.5         G3P         -0.375656   
+    3         a              M1W         2.3         M1W         -0.386247   
+    4         b              M1E         1.0     G3P M1E         -0.294788   
+    5         b              P3R        -5.0         G3R          1.668974   
+    6         b              P3G         0.4                      0.000000   
+    7         b          M1E P3G         2.7         M1E          0.080868   
+    8         b          M1E P3R        -2.7     G3R M1E          1.749842   
+    <BLANKLINE>
+       predicted_func_score  
+    0             -2.398970  
+    1             -0.792805  
+    2             -2.964124  
+    3             -2.976895  
+    4             -2.865839  
+    5             -0.792805  
+    6             -2.500000  
+    7             -2.398970  
+    8             -0.740336  
 
     We now have access to the predicted (and gamma corrected) functional scores
     as predicted by the models current parameters.
 
     So far, these parameters and predictions results from them have not been tuned
     to the dataset. Let's take a look at the loss on the training dataset
     given our initialized parameters
 
     >>> model.loss
-    DeviceArray(4.40537408, dtype=float64)
+    Array(7.19312981, dtype=float64)
 
     Next, we fit the model with some chosen hyperparameters.
 
     >>> model.fit(maxiter=1000, lasso_shift=1e-5)
     >>> model.loss
-    DeviceArray(1.01582782, dtype=float64)
+    Array(4.37424567e-05, dtype=float64)
 
     The model tunes its parameters in place, and the subsequent call to retrieve
     the loss reflects our models loss given its updated parameters.
-    """
+    """  # noqa: E501
 
     def __init__(
         self,
         data: Data,
         epistatic_model=multidms.biophysical.sigmoidal_global_epistasis,
         output_activation=multidms.biophysical.identity_activation,
         conditional_shifts=True,
@@ -525,15 +550,15 @@
             if col in df.columns and not overwrite_cols:
                 raise ValueError(f"`df` already contains column {col}")
             ret[col] = onp.nan
 
         for condition, condition_df in df.groupby(condition_col):
             variant_subs = condition_df[substitutions_col]
             if condition not in self.data.reference_sequence_conditions:
-                variant_subs = condition_df.parallel_apply(
+                variant_subs = condition_df.apply(
                     lambda x: self.data.convert_subs_wrt_ref_seq(
                         condition, x[substitutions_col]
                     ),
                     axis=1,
                 )
 
             if converted_substitutions_col is not None:
@@ -654,15 +679,15 @@
         X = jnp.array(
             [
                 self.data.binarymaps[self.data.reference].sub_str_to_binary(
                     converted_subs
                 )
             ]
         )
-        return self.phenotype_frombinary(X)
+        return self.phenotype_frombinary(X, condition)
 
     def latent_fromsubs(self, aa_subs, condition=None):
         """
         take a single string of subs which are
         not already converted wrt reference, convert them and
         then make a latent prediction and return the result.
         """
@@ -670,15 +695,15 @@
         X = jnp.array(
             [
                 self.data.binarymaps[self.data.reference].sub_str_to_binary(
                     converted_subs
                 )
             ]
         )
-        return self.latent_frombinary(X)
+        return self.latent_frombinary(X, condition)
 
     def phenotype_frombinary(self, X, condition=None):
         """
         Condition specific functional score prediction
         on X using the biophysical model
         given current model parameters.
```

## multidms/plot.py

```diff
@@ -1,14 +1,13 @@
 """
 ==========
 plot
 ==========
 
 Plotting functions.
-
 """
 
 
 from functools import reduce
 import altair as alt
 import matplotlib.colors
 import natsort
@@ -36,15 +35,16 @@
     Returns
     -------
     list
         List of hex codes for colors spanning `start` to `end`.
 
     Example
     -------
-    >>> color_gradient_hex('white', 'red', n=5)
+    >>> import multidms.plot as mplt
+    >>> mplt.color_gradient_hex('white', 'red', n=5)
     ['#ffffff', '#ffbfbf', '#ff8080', '#ff4040', '#ff0000']
 
     """
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
         name="_", colors=[start, end], N=n
     )
     return [matplotlib.colors.rgb2hex(tup) for tup in cmap(list(range(0, n)))]
@@ -704,17 +704,22 @@
         mut_df = reduce(
             lambda left, right: pandas.merge(
                 left, right, left_index=True, right_index=True, how="inner"
             ),
             mutations_dfs,
         )
 
+        # for now, we're simply dropping the functional scores
+        mut_df.drop(
+            [c for c in mut_df.columns if "func_score" in c], axis=1, inplace=True
+        )
+
         # now compute replicate averages
         for c in fit.mutations_df.columns:
-            if c == "mutation" or "times_seen" in c:
+            if c == "mutation" or "times_seen" in c or "func_score" in c:
                 continue
             cols_to_combine = [f"{replicate}_{c}" for replicate in fit_data.keys()]
             if c in ["wts", "sites", "muts"]:
                 mut_df[c] = mut_df[cols_to_combine[0]]
                 mut_df.drop(cols_to_combine, axis=1, inplace=True)
             else:
                 mut_df[f"value_{c}"] = mut_df[cols_to_combine].mean(axis=1)
```

## multidms/utils.py

```diff
@@ -77,15 +77,15 @@
     """
     Fit a multidms model to a dataset. This is a wrapper around the multidms
     fit method that allows for easy specification of the fit parameters.
     This method is helpful for comparing and organizing multiple fits.
 
     Parameters
     ----------
-    dataset : multidms.Dataset
+    dataset : :class:`multidms.Data`
         The dataset to fit to.
     huber_scale_huber : float, optional
         The scale of the huber loss function. The default is 1.
     scale_coeff_lasso_shift : float, optional
         The scale of the lasso penalty on the shift parameter. The default is 2e-5.
     scale_coeff_ridge_beta : float, optional
         The scale of the ridge penalty on the beta parameter. The default is 0.
@@ -124,15 +124,15 @@
     save_model_at : list, optional
         The iterations at which to save the model. The default is [2000, 10000, 20000].
     PRNGKey : int, optional
         The PRNGKey to use to initialize model parameters. The default is 0.
 
     Returns
     -------
-    fit_series : pd.Series
+    fit_series : :class:`pandas.Series`
         A series containing the fit attributes and pickled model objects
         at the specified save_model_at steps.
     """
     if lock_beta and not warmup_beta:
         raise ValueError("Cannot lock beta without warming up beta")
 
     fit_attributes = locals().copy()
@@ -190,37 +190,37 @@
         if onp.isnan(float(imodel.loss)):
             break
 
         fit_attributes["step_loss"][training_step] = float(imodel.loss)
 
         print(
             f"training_step {training_step}/{num_training_steps},"
-            "Loss: {imodel.loss}, Time: {fit_time} Seconds",
+            f"Loss: {imodel.loss}, Time: {fit_time} Seconds",
             flush=True,
         )
 
         if total_iterations in save_model_at:
             fit_attributes[f"model_{total_iterations}"] = copy.copy(imodel)
 
     fit_series = pd.Series(fit_attributes).to_frame().T
 
     return fit_series
 
 
 def plot_loss_simple(models):
     """
     Plot the loss of a set of models.
-    Uses matplotlib.pyplot.show() to display the plot.
+    Uses :func:`matplotlib.pyplot.show` to display the plot.
 
 
     Parameters
     ----------
-    models : pd.DataFrame
+    models : :class:`pandas.DataFrame`
         A dataframe where each row is the fit attributes of a model
-        as output by the multidms.utils.fit_wrapper() function.
+        as output by the :func:`multidms.utils.fit_wrapper` function.
 
 
     Returns
     -------
     None.
     """
     fig, ax = plt.subplots(figsize=[7, 7])
```

## Comparing `multidms-0.1.9.dist-info/LICENSE` & `multidms-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `multidms-0.1.9.dist-info/METADATA` & `multidms-0.2.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: multidms
-Version: 0.1.9
-Summary: Represent and model one or more dms experiments and identify variant predicted fitness, and individual mutation effects and shifts.
+Version: 0.2.0
+Summary: Joint modeling of multiple deep mutational scanning experiments.
 Author-email: Jared Galloway <jgallowa@fredhutch.org>, Hugh Haddox <hkhaddox@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Fred Hutchinson Cancer Research Center
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -39,42 +39,48 @@
 Requires-Dist: typing-extensions
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: binarymap
 Requires-Dist: altair
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
-Requires-Dist: notebook
 Requires-Dist: scipy
 Requires-Dist: tqdm
-Requires-Dist: ipywidgets
 Requires-Dist: pandarallel
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-pep8 ; extra == 'dev'
 Requires-Dist: pytest-datadir ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
+Requires-Dist: notebook ; extra == 'dev'
+Requires-Dist: ipywidgets ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'dev'
-Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 Requires-Dist: nbsphinx ; extra == 'dev'
 Requires-Dist: nbsphinx-link ; extra == 'dev'
 Requires-Dist: bumpver ; extra == 'dev'
 Requires-Dist: sphinxcontrib-bibtex ; extra == 'dev'
+Requires-Dist: ruff ; extra == 'dev'
 
 # multidms
 
-[![Build](https://github.com/matsengrp/multidms/actions/workflows/build_test_package.yml/badge.svg)](https://github.com/matsengrp/multidms/actions/workflows/build_test_package.yml)
 ![License](https://img.shields.io/github/license/matsengrp/multidms)
+[![PyPI version](https://badge.fury.io/py/multidms.svg)](https://badge.fury.io/py/multidms)
+[![Build](https://github.com/matsengrp/multidms/actions/workflows/build_test_package.yml/badge.svg)](https://github.com/matsengrp/multidms/actions/workflows/build_test_package.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-Model one or more deep mutational scanning (DMS) experiments
-and identify variant predicted fitness, and 
-individual mutation effects and shifts.
-
-`multidms` is a Python package written by the [Matsen Group](https://matsen.fhcrc.org/) in collaboration with the [Bloom lab](https://research.fhcrc.org/bloom/en.html)
+`multidms` is a Python package written by the 
+[Matsen group](https://matsen.fhcrc.org/)
+in collaboration with 
+[William DeWitt](https://wsdewitt.github.io/)
+and the
+[Bloom Lab](https://research.fhcrc.org/bloom/en.html).
+It can be used to jointly fit a global-epistasis model to one or more deep mutational scanning experiments, 
+with the goal of estimating the effects of individual mutations, 
+and how much the effects differ between experiments.
 
 The source code is [on GitHub](https://github.com/matsengrp/multidms).
 
 Please see the [Documentation](https://matsengrp.github.io/multidms/) for details on installation and usage.
 
 To contribute to this package, read the instructions in [CONTRIBUTING.rst](CONTRIBUTING.rst).
```

