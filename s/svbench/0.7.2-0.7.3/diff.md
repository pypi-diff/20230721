# Comparing `tmp/svbench-0.7.2.tar.gz` & `tmp/svbench-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.2.tar", last modified: Thu Jul  6 15:13:31 2023, max compression
+gzip compressed data, was "svbench-0.7.3.tar", last modified: Fri Jul 21 08:26:30 2023, max compression
```

## Comparing `svbench-0.7.2.tar` & `svbench-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.856224 svbench-0.7.2/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.2/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.2/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-06 15:13:31.855849 svbench-0.7.2/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.2/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-06 15:13:31.856321 svbench-0.7.2/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-06 15:13:27.000000 svbench-0.7.2/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.852742 svbench-0.7.2/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.2/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.2/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1357 2023-07-06 15:05:30.000000 svbench-0.7.2/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    69878 2023-07-06 15:05:30.000000 svbench-0.7.2/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.2/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.855534 svbench-0.7.2/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.2/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.2/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-06 15:13:31.855101 svbench-0.7.2/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-06 15:13:31.000000 svbench-0.7.2/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.417331 svbench-0.7.3/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.3/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.3/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-21 08:26:30.416991 svbench-0.7.3/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.3/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-21 08:26:30.417415 svbench-0.7.3/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-12 11:56:56.000000 svbench-0.7.3/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.404105 svbench-0.7.3/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.3/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.3/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1989 2023-07-19 14:28:51.000000 svbench-0.7.3/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    70673 2023-07-12 16:35:27.000000 svbench-0.7.3/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.3/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.416633 svbench-0.7.3/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.3/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.3/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-21 08:26:30.416214 svbench-0.7.3/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-21 08:26:30.000000 svbench-0.7.3/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.2/LICENSE.md` & `svbench-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.2/README.rst` & `svbench-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `svbench-0.7.2/svbench/.DS_Store` & `svbench-0.7.3/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.2/svbench/cli.py` & `svbench-0.7.3/svbench/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,35 @@
 
 version = pkg_resources.require("svbench")[0].version
 
 
 @click.command()
 @click.argument('reference_vcf', required=True, type=click.Path())
 @click.argument('query_vcfs', required=True, type=click.Path(), nargs=-1)
+@click.option("--include", help="Include regions .bed file", type=click.Path(), show_default=False, required=False)
 @click.option("--pass-only", help="Assess only PASS variants", is_flag=True, flag_value=True, show_default=False, default=False)
 @click.option("--slop", help="Add intervals +/- slop around breakpoints", default=250, type=int, show_default=True)
-@click.option("--min-size", help="Min SV length", default=20, type=int, show_default=True)
+@click.option("--min-size-ref", help="Min SV length", default=0, type=int, show_default=True)
+@click.option("--min-size-query", help="Min SV length", default=30, type=int, show_default=True)
+@click.option("--no-duplicates", help="Don't quantify duplicate true positives", is_flag=True, flag_value=True, show_default=False, default=False)
 @click.version_option()
-def main(reference_vcf, query_vcfs, pass_only, slop, min_size):
+def main(reference_vcf, query_vcfs, include, pass_only, slop, min_size_ref, min_size_query, no_duplicates):
     keep = [svb.Col("FILTER", op="eq", thresh=None)] if pass_only else []
     ref = CallSet(dataset="REFERENCE", no_translocations=False).\
         load_vcf(reference_vcf, other_cols=["FILTER"], keep=keep). \
-        filter_by_size(min_size, None, keep_translocations=True)
+        filter_by_size(min_size_ref, None, keep_translocations=True)
+
+    if include:
+        ref.filter_include_bed(include, inplace=True)
+    # print(ref.breaks_df.head())
     ref.add_intervals(slop)
     query = [CallSet(dataset="REFERENCE", caller=path.split("/")[-1], no_translocations=False).
-             load_vcf(path, other_cols=["FILTER"], keep=keep).
-             filter_by_size(min_size, None, keep_translocations=True)
+             load_vcf(path, other_cols=["FILTER"], keep=keep).filter_by_size(min_size_query, None, keep_translocations=True)
              for path in query_vcfs]
-    svb.score(ref, query)
+
+    if include:
+        [i.filter_include_bed(include, inplace=True) for i in query]
+    svb.score(ref, query, allow_duplicate_tp=not no_duplicates)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `svbench-0.7.2/svbench/io_tools.py` & `svbench-0.7.3/svbench/io_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,17 +630,17 @@
         else:
             max_s = max_size
 
         l_before = len(cs.breaks_df)
         df = cs.breaks_df
 
         if keep_translocations:
-            size_filter = ((df["svlen"] >= min_s) & (df["svlen"] < max_s)) | (df["chrom"] != df["chrom2"])
+            size_filter = np.array([True if ((svlen >= min_s and svlen < max_s) or chrom1 != chrom2 or svlen is None or svlen != svlen) else False for svlen, chrom1, chrom2 in zip(df['svlen'], df['chrom'], df['chrom2'])])
         else:
-            size_filter = (df["svlen"] >= min_s) & (df["svlen"] < max_s)
+            size_filter = np.array([True if ((svlen >= min_s and svlen < max_s) or svlen is None or svlen != svlen) else False for svlen, chrom1, chrom2 in zip(df['svlen'], df['chrom'], df['chrom2'])])
 
         df["size_filter_pass"] = size_filter
         if not soft:
             df = df[size_filter]
         print("Filtered by min_size={}, max_size={}, caller={}, dataset={} rows before {}, after {}".format(
             min_size, max_size, self.caller, self.dataset,l_before, size_filter.sum()),
               file=stderr)
@@ -881,31 +881,36 @@
                 if isinstance(r.ALT, list):
                     la = len(r.ALT[0])
                 else:
                     la = len(r.ALT)
                 if lr > 1 or la > 1:
                     if lr > la:
                         r.INFO["SVTYPE"] = "DEL"
+                        svtype = "DEL"
                     else:
                         r.INFO["SVTYPE"] = "INS"
+                        svtype = "INS"
+                else:
+                    r.INFO["SVTYPE"] = "BND"
+                    svtype = "BND"
 
             try:
                 if allowed_svtypes is not None and svtype not in allowed_svtypes:
                     continue
             except TypeError:
                 if isinstance(svtype, list):
                     svtype = svtype[0]
                     if allowed_svtypes is not None and svtype not in allowed_svtypes:
                         continue
 
             if keep is not None and not check_passed(operations, r, keep):
                 continue
 
             svlen = -1
-            if r.ID.endswith("_2"):  # Skip second part of BND, or multirow record
+            if isinstance(r.ID, str) and r.ID.endswith("_2"):  # Skip second part of BND, or multirow record
                 continue
             if svtype == "BND":
                 if r.ALT[0] is None:
                     continue
                 try:
                     chrom2 = r.ALT[0].chr
                     end = r.ALT[0].pos
@@ -1508,33 +1513,40 @@
                "Precision": None, "Recall": None, "F1": None, "Duplication": None, "quantified": None, "strata": None}]
         # return data
         data.scores = pd.DataFrame.from_records(ts)[["T >=", "Ref", "Total", "TP", "FP", "DTP", "FN", "Duplication", "Precision",
                                                      "Recall", "F1"]]
         data.false_negative_indexes = ref_bedpe.index
         return
 
-    for query_idx, chrom, start, chrom2, end, svtype, w in zip(dta.index, dta["chrom"], dta["start"], dta["chrom2"], dta["end"],
-                                                       dta["svtype"], dta["w"]):
+    for query_idx, chrom, start, chrom2, end, svtype, w, d_id in zip(dta.index, dta["chrom"], dta["start"], dta["chrom2"], dta["end"],
+                                                       dta["svtype"], dta["w"], dta["id"]):
         if chrom == chrom2 and start == end:
             end += 1  # prevent 0 width interval
         chrom, start, chrom2, end = sv_key(chrom, start, chrom2, end)
 
         ol_start = intersecter(tree, chrom, start, start + 1)
+        # if d_id == '54109':
+        #     print('start', ol_start, (start, start+1), file=stderr)
+        #     quit()
         if not ol_start:
             # print("FALSE1", chrom, start, chrom2, end, svtype, file=stderr)
             continue
 
         ol_end = intersecter(tree, chrom2, end, end + 1)
+        # if d_id == '54109':
+        #     print('end', ol_end, file=stderr)
+        #     quit()
         if not ol_end:
             # print("FALSE2", chrom, start, chrom2, end, svtype, file=stderr)
             continue
 
-        # if start == 57861455:
-        #     print(ol_start)
-        #     print(ol_end)
+        # if d_id == '54109':
+        #     print(ol_start, file=stderr)
+        #     print(ol_end, file=stderr)
+        #     quit()
 
         # Get the ref_data index
         common_idxs = set([i[2] for i in ol_start]).intersection([i[2] for i in ol_end])
         if len(common_idxs) == 0:
             continue
 
         # Choose an index by highest weight/lowest total distance, meeting reciprocal_overlap threshold
@@ -1803,7 +1815,9 @@
             t.update({k: v for k, v in Counter(data.breaks_df.GT).items() if v == v})
 
             data.gt_scores = pd.DataFrame({k: [v] for k, v in t.items()})
 
             if show_table:
                 print("GT scores:", file=stderr)
                 print(data.gt_scores, file=stderr)
+
+    # print(data.breaks_df[data.breaks_df["FP"]], file=stderr)
```

### Comparing `svbench-0.7.2/svbench/loaders.py` & `svbench-0.7.3/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.2/svbench/quant_tools.py` & `svbench-0.7.3/svbench/quant_tools.py`

 * *Files identical despite different names*

