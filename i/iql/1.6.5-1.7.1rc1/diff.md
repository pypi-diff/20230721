# Comparing `tmp/iql-1.6.5-py3-none-any.whl.zip` & `tmp/iql-1.7.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,30 @@
-Zip file size: 48555 bytes, number of entries: 27
--rw-r--r--  2.0 unx      327 b- defN 23-Jun-23 19:56 iql/__init__.py
--rw-r--r--  2.0 unx      101 b- defN 23-Jun-23 19:57 iql/_version.py
--rw-r--r--  2.0 unx    34190 b- defN 23-Jun-23 19:56 iql/iqmoql.py
--rw-r--r--  2.0 unx     1282 b- defN 23-Jun-23 19:56 iql/options_parser.py
--rw-r--r--  2.0 unx      432 b- defN 23-Jun-23 19:56 iql/q_cache_base.py
--rw-r--r--  2.0 unx     2191 b- defN 23-Jun-23 19:56 iql/threading_experimental.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-23 19:56 iql/bbg_bql/__init__.py
--rw-r--r--  2.0 unx    10069 b- defN 23-Jun-23 19:56 iql/bbg_bql/bql_datamodel.py
--rw-r--r--  2.0 unx     9377 b- defN 23-Jun-23 19:56 iql/bbg_bql/bql_extension.py
--rw-r--r--  2.0 unx    14632 b- defN 23-Jun-23 19:56 iql/bbg_bql/bql_wrapper.py
--rw-r--r--  2.0 unx      692 b- defN 23-Jun-23 19:56 iql/bbg_bql/debug_tools.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-23 19:56 iql/db_connectors/__init__.py
--rw-r--r--  2.0 unx     5109 b- defN 23-Jun-23 19:56 iql/db_connectors/duckdb_connector.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-23 19:56 iql/extensions/__init__.py
--rw-r--r--  2.0 unx     3407 b- defN 23-Jun-23 19:56 iql/extensions/aws_s3_extension.py
--rw-r--r--  2.0 unx     7829 b- defN 23-Jun-23 19:56 iql/extensions/edgar_extension.py
--rw-r--r--  2.0 unx     4279 b- defN 23-Jun-23 19:56 iql/extensions/fred_extension.py
--rw-r--r--  2.0 unx     4106 b- defN 23-Jun-23 19:56 iql/extensions/kaggle_extension.py
--rw-r--r--  2.0 unx     2495 b- defN 23-Jun-23 19:56 iql/extensions/pandas_extension.py
--rw-r--r--  2.0 unx      666 b- defN 23-Jun-23 19:56 iql/extensions/template_extension.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-23 19:56 iql/jupyter_magics/__init__.py
--rw-r--r--  2.0 unx     4131 b- defN 23-Jun-23 19:56 iql/jupyter_magics/iql_magic.py
--rw-r--r--  2.0 unx      535 b- defN 23-Jun-23 19:57 iql-1.6.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    25591 b- defN 23-Jun-23 19:57 iql-1.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 19:57 iql-1.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-23 19:57 iql-1.6.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2208 b- defN 23-Jun-23 19:57 iql-1.6.5.dist-info/RECORD
-27 files, 134053 bytes uncompressed, 45005 bytes compressed:  66.4%
+Zip file size: 50151 bytes, number of entries: 28
+-rw-r--r--  2.0 unx      327 b- defN 23-Jul-21 21:04 iql/__init__.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jul-21 21:04 iql/_version.py
+-rw-r--r--  2.0 unx    36865 b- defN 23-Jul-21 21:04 iql/iqmoql.py
+-rw-r--r--  2.0 unx     1289 b- defN 23-Jul-21 21:04 iql/options_parser.py
+-rw-r--r--  2.0 unx      432 b- defN 23-Jul-21 21:04 iql/q_cache_base.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-21 21:04 iql/threading_experimental.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-21 21:04 iql/bbg_bql/__init__.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jul-21 21:04 iql/bbg_bql/bql_datamodel.py
+-rw-r--r--  2.0 unx     9485 b- defN 23-Jul-21 21:04 iql/bbg_bql/bql_extension.py
+-rw-r--r--  2.0 unx    15045 b- defN 23-Jul-21 21:04 iql/bbg_bql/bql_wrapper.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Jul-21 21:04 iql/bbg_bql/debug_tools.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-21 21:04 iql/db_connectors/__init__.py
+-rw-r--r--  2.0 unx     5174 b- defN 23-Jul-21 21:04 iql/db_connectors/duckdb_connector.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-21 21:04 iql/extensions/__init__.py
+-rw-r--r--  2.0 unx     3407 b- defN 23-Jul-21 21:04 iql/extensions/aws_s3_extension.py
+-rw-r--r--  2.0 unx     1575 b- defN 23-Jul-21 21:04 iql/extensions/cache_extension.py
+-rw-r--r--  2.0 unx     7829 b- defN 23-Jul-21 21:04 iql/extensions/deprecated_edgar_extension.py
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jul-21 21:04 iql/extensions/fred_extension.py
+-rw-r--r--  2.0 unx     4106 b- defN 23-Jul-21 21:04 iql/extensions/kaggle_extension.py
+-rw-r--r--  2.0 unx     2495 b- defN 23-Jul-21 21:04 iql/extensions/pandas_extension.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jul-21 21:04 iql/extensions/template_extension.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-21 21:04 iql/jupyter_magics/__init__.py
+-rw-r--r--  2.0 unx     4131 b- defN 23-Jul-21 21:04 iql/jupyter_magics/iql_magic.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Jul-21 21:04 iql-1.7.1rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    25594 b- defN 23-Jul-21 21:04 iql-1.7.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 21:04 iql-1.7.1rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-21 21:04 iql-1.7.1rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2324 b- defN 23-Jul-21 21:04 iql-1.7.1rc1.dist-info/RECORD
+28 files, 139109 bytes uncompressed, 46407 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -39,15 +39,18 @@
 
 Filename: iql/extensions/__init__.py
 Comment: 
 
 Filename: iql/extensions/aws_s3_extension.py
 Comment: 
 
-Filename: iql/extensions/edgar_extension.py
+Filename: iql/extensions/cache_extension.py
+Comment: 
+
+Filename: iql/extensions/deprecated_edgar_extension.py
 Comment: 
 
 Filename: iql/extensions/fred_extension.py
 Comment: 
 
 Filename: iql/extensions/kaggle_extension.py
 Comment: 
@@ -60,23 +63,23 @@
 
 Filename: iql/jupyter_magics/__init__.py
 Comment: 
 
 Filename: iql/jupyter_magics/iql_magic.py
 Comment: 
 
-Filename: iql-1.6.5.dist-info/LICENSE
+Filename: iql-1.7.1rc1.dist-info/LICENSE
 Comment: 
 
-Filename: iql-1.6.5.dist-info/METADATA
+Filename: iql-1.7.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: iql-1.6.5.dist-info/WHEEL
+Filename: iql-1.7.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: iql-1.6.5.dist-info/top_level.txt
+Filename: iql-1.7.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: iql-1.6.5.dist-info/RECORD
+Filename: iql-1.7.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iql/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__="1.6.5"
-__commit__="28d9cd78b29bd78980252077270c15f16b610223"
-__commit_short__="28d9cd7"
+__version__="1.7.1rc1"
+__commit__="acddf8651e708873d718f264d157c4723636ba83"
+__commit_short__="acddf86"
```

## iql/iqmoql.py

```diff
@@ -9,15 +9,15 @@
 from typing import List, Dict, Optional, Union, Tuple, Callable
 from pandas import DataFrame
 import pandas as pd
 from abc import abstractmethod
 from iql.q_cache_base import QueryCacheBase
 from iql import options_parser
 from iql import threading_experimental as te
-
+import json
 
 # Cache Settings
 # Use iqmoql.activate_cache() before first execute() to
 # ensure settings propogate to individual extensions.
 # Infinite in memory cache by default
 
 DEFAULT_EXT_DIRECTORY = None
@@ -41,23 +41,48 @@
 _KNOWN_EXTENSIONS: Dict[str, str] = {
     "bql": "iql.bbg_bql.bql_extension",
     "s3": "iql.extensions.aws_s3_extension",
     "fred": "iql.extensions.fred_extension",
     "kaggle": "iql.extensions.kaggle_extension",
     "edgar": "iql.extensions.edgar_extension",
     "pandas": "iql.extensions.pandas_extension",
+    "cache": "iql.extensions.cache_extension",
 }
 
 _ALIASES: Dict[
     str, Callable[[], str]
 ] = {}  # Callable, so we can either use text or external files
 
 logger = logging.getLogger(__name__)
 
 
+default_cache_policy_toplevel = {
+    "max_age": 3600,
+    "s3": False,
+    "fcache": False,
+    "memory": False,
+}
+
+default_cache_policies_keywords = {
+    "bql": {"max_age": 3600, "fcache": True, "memory": True}
+}
+
+
+def get_policy_from_query(string: str) -> Optional[Dict[str, object]]:
+    matches = re.search(r"cache\{(.+?)\}\s*\n", string)
+
+    if matches:
+        extracted_value = matches.group(1)
+        logger.info(f"Query has policy: {extracted_value}")
+
+        return dict(json.loads(f"{{{extracted_value}}}"))
+
+    return {}
+
+
 def _find_closing_paren(text: str, start: int) -> int:
     # TODO: Handle escaping
     paren_depth = 1
     quote_stack = []
     for i in range(start, len(text)):
         c = text[i]
         if c == "(" and len(quote_stack) == 0:
@@ -279,30 +304,34 @@
 
                 sq.dataframe = df
 
                 sq.save_to_cache()
 
                 return df
 
-    def execute_batch(self, queries: List["SubQuery"]) -> List[IqlResult]:
+    def execute_batch(
+        self,
+        queries: List["SubQuery"],
+        cache_policy: Optional[Dict[str, object]] = None,
+    ) -> List[IqlResult]:
         """Default implementation runs individually, override for functions that can be batched, such as
         BQL's _many functions.
         Executes all subqueries first, then merges as required.
         SubQueries are executed in a threadpool, which has minimal benefit."""
 
         completed_results = []
         # context = get_context('spawn')
 
         subqueries_flat = get_subqueries_flat(queries)
         # Get all the queries (and any queries inside SubQueryGroups)
 
         # Executes the ungrouped queries
 
         if te.ENABLED and te.MAX_PROCESSES > 1 and len(queries) > 1:
-            te.execute_batch(subqueries_flat, self.execute)
+            te.execute_batch(subqueries_flat, self.execute, cache_policy)
         else:
             for query in subqueries_flat:
                 try:
                     self.execute(query)  # type: ignore
                 except Exception as e:
                     raise ValueError(f"Error from {query}") from e
 
@@ -310,15 +339,21 @@
         for query in queries:
             # For single subqueries, this is a noop
             # For subquery groups, this merges the results of the children
             query.merge()
 
             df = query.dataframe
             if df is None and not self.use_path_replacement():
-                raise ValueError(f"Empty DF, {query.get_query()} failed")
+                q = "Unknown"
+                try:
+                    q = query.get_query()
+                except Exception:
+                    pass
+                raise ValueError(f"Empty DF, {q} failed")
+
             elif df is None:
                 logger.debug("Using path replacement, no DF")
             else:
                 query.dataframe = df  # type: ignore
 
                 ir = IqlResultData(name=query.name, query=query.subquery, _data=df)
                 completed_results.append(ir)
@@ -336,15 +371,15 @@
         self,
         query: str,
         name: str,
         iqc: "IqlQueryContainer",
         create_function: Optional[Callable] = None,
     ) -> List["SubQuery"]:
         """Converted to always return a single item, but left logic in place to support multiple"""
-        logger.debug(f"Creating a subquery {name} for {query}")
+        logger.debug(f"Creating a subquery {name[:50]} for {query[:50]}")
 
         if create_function is None:
             create_function = self.create_subquery
 
         sq = create_function(subquery=query, name=name, iqc=iqc)
 
         # If a paramlist is passed, create one subquery for each value
@@ -383,15 +418,18 @@
             if isinstance(parameter_values, str):
                 parameter_values = [parameter_values]
         else:
             parameter_name = None
             parameter_values = None  # type: ignore
 
         if parameter_name is not None:
-            assert parameter_values is not None and len(parameter_values) > 0
+            if parameter_values is None or len(parameter_values) == 0:
+                parameter_values = {None}  # type: ignore
+                # raise ValueError(f"{parameter_name}: No parameter values passed for query: {query}")
+
             sqs: List["SubQuery"] = []
             count = 1
 
             if not parameter_name.startswith("$"):
                 logger.debug("Parameter name doesn't start with $, inserting one")
                 # This is helpful to avoid replacing the paramquery when substituting
                 parameter_name = f"${parameter_name}"
@@ -466,22 +504,22 @@
 
         return working_df
 
     def pivot(self, working_df: DataFrame, pivot_option: Union[str, List]) -> DataFrame:
         if pivot_option is None:
             return working_df
 
-        isauto = False
+        # isauto = False
         logger.debug(f"Pivoting by {pivot_option}")
         if isinstance(pivot_option, str):
             if pivot_option.lower() == "none":
                 # Pivot disabled / noop
                 return working_df
             elif pivot_option.lower() == "auto":
-                isauto = True
+                # isauto = True
                 index = []
                 column = "name"
                 value = "value"
 
                 if column not in working_df.columns or value not in working_df.columns:
                     raise ValueError(
                         f"{column} or {value} not found in dataframe columns. Auto should only be used with BQL results."
@@ -547,32 +585,17 @@
             # Needed to allow pivoting by datetime columns
             for col in column:
                 if pd.api.types.is_datetime64_any_dtype(working_df[col]):
                     working_df[col] = working_df[col].dt.strftime("%Y-%m-%d")
 
         logger.debug(f"Pivot index {index} columns {column} values {value}")
 
-        try:
-            working_df = working_df.pivot(
-                index=index,
-                columns=column,
-                values=value,
-            )
-        except Exception as e:
-            if not isauto:
-                raise e
-            else:
-                logger.debug("Failed to auto pivot, trying a wider pivot")
-                index = [col for col in working_df.columns if col.lower() not in [column.lower(), value.lower()]]  # type: ignore
-
-                working_df = working_df.pivot(
-                    index=index,
-                    columns=column,
-                    values=value,
-                )
+        working_df = working_df.pivot_table(
+            index=index, columns=column, values=value, aggfunc="last", dropna=False
+        )
 
         working_df = working_df.reset_index()
 
         if isinstance(value, list) and len(value) > 1:
             working_df.columns = [
                 "_".join(reversed(str(col) if type(col) == int else col))
                 for col in working_df.columns.values
@@ -611,15 +634,15 @@
 @dataclass
 class SubQuery:
     extension: IqlExtension
     subquery: str
     name: str
     iqc: "IqlQueryContainer"
     dataframe: Optional[DataFrame] = field(default=None, init=False)
-
+    cache_policy: Optional[Dict[str, object]] = field(default=None, init=False)
     options: Dict[str, object] = field(default_factory=dict, init=False)
     input_data: object = field(default=None, init=False)
 
     local_dfs: Dict[str, object] = field(default_factory=dict, init=False)
 
     def get_subqueries_flat(self) -> List["SubQuery"]:
         return [self]
@@ -634,29 +657,33 @@
         if len(self.options) == 0:
             raise ValueError(f"Options not properly passed or parsed ({self.subquery})")
 
         query = next(iter(self.options.keys()))
         return query
 
     def __post_init__(self):
-        if self.subquery is not None:
-            self.options: Dict[str, object] = options_parser.options_to_list(
-                self.subquery
-            )
-            logger.debug(f"Options: {self.options}")
+        try:
+            if self.subquery is not None:
+                self.options: Dict[str, object] = options_parser.options_to_list(
+                    self.subquery
+                )
+                # logger.debug(f"Options: {str(self.options)[:50]}")
+        except Exception:
+            logger.exception(f"Exception in {str(self.subquery)[:50]}")
+            raise ValueError(f"Parse Exception of {str(self.subquery)[:50]}")
 
     def populate_from_cache(self) -> bool:
         """Returns cached value if it's available"""
         cache_val = self.subquery
 
-        logger.debug(f"Checking cache for {cache_val}, {type(self)}")
+        logger.debug(f"Checking cache for {str(cache_val)[:50]}, {type(self)}")
         if not self.extension.allow_cache_read(self):
             return False
 
-        df = CACHE.get(key=cache_val)
+        df = CACHE.get(key=cache_val, policy=self.cache_policy)
         if df is not None:
             logger.debug("Using cached SubQuery")
             self.dataframe = df  # type: ignore
             return True
         else:
             logger.debug("Not found in cache")
             return False
@@ -664,15 +691,15 @@
     def save_to_cache(self):
         if not self.extension.allow_cache_save(self):
             return
 
         cache_val = self.subquery
 
         if self.dataframe is not None:
-            CACHE.save(key=cache_val, data=self.dataframe)
+            CACHE.save(key=cache_val, data=self.dataframe, policy=self.cache_policy)
 
 
 @dataclass
 class SubQueryGroup(SubQuery):
     """SubQueryGroups represent a set of queries whose outputs will be combined.
     SubQueries are executed in parallel (via get_subqueries_flat),
     so this step is needed to gather the results.
@@ -716,25 +743,29 @@
             logger.info(f"Writing to final parquet file {outfile}")
 
             df.to_parquet(outfile)
 
         else:
             dfs: List[DataFrame] = [sq.dataframe for sq in self.subqueries]  # type: ignore
             logger.debug(f"Concatting {len(dfs)}")
-            self.dataframe = pd.concat(dfs)
+            if len(dfs) == 1:
+                self.dataframe = dfs[0]
+            else:
+                self.dataframe = pd.concat(dfs)
 
         logger.info(f"Done merging {len(self.subqueries)} subqueries")
 
 
 class IqlQueryContainer:
     # This is used so we can run the bql_queries as an async batch, separate from processing the results.
     orig_query: str
     query: str
     subqueries: List[SubQuery]
     db: Optional[object]
+    cache_policy: Optional[Dict[str, object]] = None
 
     def extract_subqueries(self):
         subqueries: List[SubQuery] = []
 
         i = 0
 
         replacements: Dict[str, Optional[str]] = {}
@@ -766,15 +797,15 @@
 
                 result = " UNION ".join(querystrings)
                 result = f"({result})"
 
             replacements[outer] = result
 
         for old, new in replacements.items():
-            logger.debug(f"Replacing {old} with {new}")
+            logger.debug(f"Replacing {str(old)[:50]} with {str(new)[:50]}")
             query = query.replace(old, new)  # type: ignore
 
         # if only one function without a beginning subquery
         if len(replacements) > 0:
             values = [value for value in replacements.values() if value is not None]
             if re.match(rf"(?s)\s*({'|'.join(values)}).*", query) is not None:
                 logger.info(f"Starts with replacement {values}")
@@ -785,14 +816,18 @@
         return subqueries
 
     def __init__(self, query: str, db: IqlDatabase):
         self.orig_query = query
         self.query = query
         self.db = db
 
+        self.cache_policy = get_policy_from_query(query)
+        if self.cache_policy is None:
+            self.cache_policy = default_cache_policy_toplevel
+
         self.subqueries = self.extract_subqueries()
         # self.subqueries = self._extract_replacements()
         # Sanity checks. These don't take into account escaping or quoting, so they're just warnings.
         if query.count("(") != query.count(")"):
             logger.warning("Left and Right Paren counts aren't equal")
 
         if query.count("'") % 2 != 0:
@@ -814,33 +849,63 @@
     def execute(self) -> Tuple[Optional[DataFrame], List[IqlResult]]:
         """Returns the final df, plus the intermediate subquery dataframes.
         If the query is not a Select, returns a None"""
         # Execute the subqueries
 
         completed_results: List[IqlResult] = []
 
+        logger.debug(f"checking cache {self.orig_query}, {self.cache_policy}")
+        df = CACHE.get(key=self.orig_query, policy=self.cache_policy)
+        if df is not None:
+            logger.debug("Query found fully in cache, using.")
+            return (df, [])
+
         for (keyword, subword), e in _EXTENSIONS.items():
             sqs: List[SubQuery] = self.get_subqueries_by_extension(keyword, subword)  # type: ignore
 
-            e_results = e.execute_batch(sqs)  # type: ignore
+            # If the cache policy has a policy for the subtype, use that, otherwise use defaults
+            # Don't use the top level cache policy
+            sub_policy: Optional[Dict[str, object]] = (  # type: ignore
+                self.cache_policy.get(keyword, None)
+                if self.cache_policy is not None
+                else None
+            )
+            if sub_policy is None:
+                sub_policy = default_cache_policies_keywords.get(keyword, None)  # type: ignore
 
+            if sub_policy is not None:
+                for q in sqs:
+                    q.cache_policy = sub_policy  # type: ignore
+
+                    if hasattr(q, "subqueries"):
+                        for sqq in q.subqueries:  # type: ignore
+                            sqq.cache_policy = sub_policy  # type: ignore
+
+            try:
+                e_results = e.execute_batch(sqs, sub_policy)  # type: ignore
+            except Exception as e:
+                raise ValueError(
+                    f"Failed to execute batch {keyword} {subword}: {self.query} {sqs}"
+                ) from e
             completed_results += e_results
 
         result = self.db.execute_query(query=self.query, completed_results=completed_results)  # type: ignore
 
         if result is None:
             df = None
         else:
             df = result.df_numpy()
 
         # add the final result to the completions
         final_result = IqlResultData(name="final", query=self.query, _data=df)  # type: ignore
 
         completed_results.append(final_result)
 
+        CACHE.save(key=self.orig_query, data=df, policy=self.cache_policy)
+
         return (df, completed_results)  # type: ignore
 
 
 class IqlPlan:
     pass
 
 
@@ -871,15 +936,15 @@
         newquery = newquery.replace(outer, sql)
         # logger.info(f"After alias replacement {query}")
 
     return newquery
 
 
 def execute_debug(
-    query: str, con: Optional[object] = None, params: Dict[str, object] = None
+    query: str, con: Optional[object] = None, params: Optional[Dict[str, object]] = None
 ) -> Tuple[bool, Optional[DataFrame], Optional[Dict[str, List[IqlResult]]]]:
     """Returns the success (True or False), final query result, and the debug results: all the intermediate queries and subqueries."""
     # Connection to database
 
     # TODO: Get rid of this special case for BQL only.
     if query.strip().startswith("get") or query.strip().startswith("let"):
         query = query.replace('"', '"')
@@ -926,15 +991,15 @@
 
     finally:
         if con is None:  # DB was created here, so close it
             db.close_db()
 
 
 def execute(
-    query: str, con: Optional[object] = None, params: Dict[str, object] = None
+    query: str, con: Optional[object] = None, params: Optional[Dict[str, object]] = None
 ) -> Optional[DataFrame]:
     """Executes the given SQL query. Keyword is only used to run a single subquery without SQL."""
 
     success, df, completed_results = execute_debug(query, con, params=params)
 
     return df
 
@@ -1023,7 +1088,11 @@
     file_directory: None (no file cache), string (output directory)
     """
     global DEFAULT_EXT_DIRECTORY
     DEFAULT_EXT_DIRECTORY = temp_dir
 
     if max_processes is not None:
         te.MAX_PROCESSES = max_processes
+
+
+def get_bql_default_policy():
+    return default_cache_policies_keywords.get("bql", None)
```

## iql/options_parser.py

```diff
@@ -26,15 +26,15 @@
     elif isinstance(node, ast.Num):
         return node.n
     else:
         return node.id
 
 
 def options_to_list(options: str) -> Dict[str, object]:
-    logger.debug(f"Analyzing {options}")
+    # logger.debug(f"Analyzing {options[:50]}")
     options = options.replace("\n", " ")
     p = ast.parse(options)
 
     results = {}
 
     for e in p.body:
         if isinstance(e.value, ast.Name):  # type: ignore
```

## iql/threading_experimental.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 #
 
-from typing import List
+from typing import List, Optional, Dict
 import concurrent.futures as cf
 import logging
 from iql import iqmoql
 
 import inspect
 
 logger = logging.getLogger(__name__)
@@ -46,15 +46,19 @@
             if o is None:
                 logger.info(f"Couldn't load {opt} from currentframes")
             if o is not None:
                 logger.debug(f"Registering {opt}")
                 sq.local_dfs[opt] = o
 
 
-def execute_batch(subqueries_flat: List["iqmoql.SubQuery"], execute):
+def execute_batch(
+    subqueries_flat: List["iqmoql.SubQuery"],
+    execute,
+    cache_policy: Optional[Dict[str, object]] = None,
+):
     processPool = cf.ThreadPoolExecutor(MAX_PROCESSES)
 
     futures = []
     futuretuples = []
     for query in subqueries_flat:
         # when running parallel, subqueries can't use the DuckDB connections
```

## iql/bbg_bql/bql_datamodel.py

```diff
@@ -66,15 +66,15 @@
             new_str = self.bql_query_string.replace(SECURITY_KEYWORD, self.security)
         else:
             new_str = self.bql_query_string
 
         for param, value in self.params.items():
             new_str = new_str.replace(param, value)
 
-        logger.debug(f"Raw query to string: {new_str}")
+        logger.debug(f"Raw query to string: {str(new_str)[:50]}")
 
         if "preferences" not in new_str:
             logger.debug("Adding default preferences")
             new_str += " \n preferences(addcols=all)"
         return new_str
```

## iql/bbg_bql/bql_extension.py

```diff
@@ -173,15 +173,19 @@
         iqc: IqlQueryContainer,
         create_function: object = None,
     ) -> List["SubQuery"]:
         return super().create_subqueries(
             query=query, name=name, iqc=iqc, create_function=self.create_subquery
         )
 
-    def execute_batch(self, subqueries: List[_IqmoBqlQuery]) -> List[IqlResultData]:
+    def execute_batch(
+        self,
+        subqueries: List[_IqmoBqlQuery],
+        cache_policy: Optional[Dict[str, object]] = None,
+    ) -> List[IqlResultData]:
         # Caching operates at two levels here:
         # The SubQuery result, and within the bql_wrapper
         # To force a refresh, we'll clear both the subquery and bql raw query
         # cache
 
         subqueries_flat: List[_IqmoBqlQuery] = get_subqueries_flat(subqueries)  # type: ignore
 
@@ -200,15 +204,15 @@
             sq for sq in subqueries_flat if sq.dataframe is None
         ]
 
         queries = [q.bqlquery for q in to_run]
 
         # We already checked whether its cached AND whether caching is allowed in sq.populate_from_cache
         logger.debug(f"Executing {len(queries)}")
-        execute_bql_str_list_async_q(queries)
+        execute_bql_str_list_async_q(queries, cache_policy=cache_policy)
 
         # Then update the subqueries
         for q in subqueries_flat:
             if q.bqlquery.execution_status == BaseBqlQuery.STATUS_FAILURE:
                 if q.options.get("allow_failure") is None:
                     raise ValueError(
                         f"BQL SubQuery failed {q.bqlquery.exception_msg}: {q.bqlquery.to_bql_query()} {q.options}"
```

## iql/bbg_bql/bql_wrapper.py

```diff
@@ -10,19 +10,18 @@
 from datetime import datetime
 from functools import partial
 from typing import List, Optional, Union, Dict
 from pandas import DataFrame
 from abc import abstractmethod
 import bql  # pyright: ignore pylint: disable=C0413 # noqa: E402
 from iql import get_cache
-
+from iql.iqmoql import get_bql_default_policy
 
 _MAX_CONCURRENT = 128
 _SHIFT_DUPLICATES = True
-
 logger = logging.getLogger(__name__)
 
 bqService = None
 _disabled = False
 
 # Used to avoid multiple threads from simultaneously running bql statements
 bqllock = Lock()
@@ -234,27 +233,31 @@
     errorlist.append(msg)
 
 
 def execute_bql_str_list_async_q(
     queries_input: List[BaseBqlQuery],
     suppress_warning_log: bool = False,
     max_queries: int = _MAX_CONCURRENT,
+    allow_async: bool = True,
+    cache_policy: Optional[Dict[str, object]] = None,
 ):
+    if cache_policy is None:
+        cache_policy = get_bql_default_policy()
     if _disabled:
         raise ValueError("BQL is disabled")
     """Note: Not multi-process safe due to underlying BQL APIs
     and (presumably) its use a Singleton for bqapi requests.
     Either batch requests through a single requester thread, or
     distribute workload across requesters.
     """
     logger.debug("Checking to see if any are already cached")
 
     for q in queries_input:
         qstr = q.to_bql_query()
-        data = get_cache().get(key=qstr, prefix="bql")  # type: ignore
+        data = get_cache().get(key=qstr, prefix="bql", policy=cache_policy)  # type: ignore
         if data is not None:
             logger.debug(f"Found in cache: {qstr}")
 
             if isinstance(data, DataFrame):
                 q._df = data
             else:
                 q._data = data  # type: ignore
@@ -284,50 +287,57 @@
         count = count + 1
 
         # t1 = threading.Thread(target=asyncio.run, args=(_execute_bql_str_list_async_callbacks(query_group, suppress_warning_log),))
         # t1.start()
         # t1.join
 
         logger.debug("Done async with callbacks")
-        _execute_bql_str_list_async_orig(query_group, suppress_warning_log)
+        _execute_bql_str_list_async_orig(
+            query_group, suppress_warning_log, allow_async=allow_async
+        )
 
     end = time.time()
     logger.info(f"Elapsed time running queries: {round(end-start)} seconds")
 
     for q in queries_not_cached:
         logger.debug("Saving to cache")
         if q._data is not None:
-            get_cache().save(key=q.to_bql_query(), data=q._data, prefix="bql")
+            get_cache().save(
+                key=q.to_bql_query(), data=q.to_df(), prefix="bql", policy=cache_policy
+            )
 
     return
 
 
 def is_bquant():
     return False  # os.environ.get("BQUANT_USERNAME") is not None
 
 
 def _execute_bql_str_list_async_orig(
-    queries: List[BaseBqlQuery], suppress_warning_log: bool = False
+    queries: List[BaseBqlQuery],
+    suppress_warning_log: bool = False,
+    allow_async: bool = True,
 ):
     with bqllock:
         query_strings = [query.to_bql_query() for query in queries]
 
         bqService = get_bqservice()
 
         # TODO: Out of order errors are not handled here. Not an issue in many cases
         # but is still very likely.
         errorlist: List[str] = []
 
         try:
-            if is_bquant():
+            if is_bquant() and allow_async:
                 logger.debug("Using submit fetch many")
 
-                gen = bqService.submit_fetch_many(
+                gen = bqService._submit_fetch_many(
                     query_strings,
                     on_request_error=partial(error_callback, errorlist=errorlist),
+                    num_retries=1,
                 )
             else:
                 gen = bqService.execute_many(
                     query_strings,
                     on_request_error=partial(error_callback, errorlist=errorlist),
                 )
         except Exception as e:
```

## iql/db_connectors/duckdb_connector.py

```diff
@@ -131,16 +131,17 @@
                 self._connection.close()  # type: ignore
                 self._connection = None
         except Exception:
             logger.exception("Unable to close")
 
 
 class _DuckDbConnector(IqlDatabaseConnector):
-    def create_database(self) -> _DuckDB:
-        con = duckdb.connect(database=":memory:")
+    def create_database(self, file=":memory:") -> _DuckDB:
+        con = duckdb.connect(database=file)
+        con.execute("SET enable_progress_bar=false;")
         return _DuckDB(_connection=con, _started_thread=threading.get_ident())
 
     def create_database_from_con(self, con: object) -> _DuckDB:
         return _DuckDB(_connection=con, _started_thread=threading.get_ident())
 
 
 def getConnector() -> IqlDatabaseConnector:
```

## Comparing `iql/extensions/edgar_extension.py` & `iql/extensions/deprecated_edgar_extension.py`

 * *Files identical despite different names*

## Comparing `iql-1.6.5.dist-info/LICENSE` & `iql-1.7.1rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iql-1.6.5.dist-info/METADATA` & `iql-1.7.1rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iql
-Version: 1.6.5
+Version: 1.7.1rc1
 Summary: SQL Overlay Language with support for Bloomberg BQL, FRED, Edgar, Kaggle and other financial data sources within SQL
 Home-page: https://github.com/iqmo-org/iql_dev
 Author: Paul Timmins
 Author-email: paul@iqmo.com
 Keywords: IQMO Query Language IQMOQL BQL BQUANT FRED EDGAR KAGGLE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `iql-1.6.5.dist-info/RECORD` & `iql-1.7.1rc1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 iql/__init__.py,sha256=jzOPdBHzwKo5ExTZjDslEBPo7xH33GChRhRILmHPrD0,327
-iql/_version.py,sha256=LBQfxvQt7o_oQ_KRTM3GBehT7dCDsOLbRAjVgWLg4gU,101
-iql/iqmoql.py,sha256=Hbwp9aZQMP_8xjEVj2561I6DUTM-QC040vusQz1JeMY,34190
-iql/options_parser.py,sha256=Sk6iRFCDrAbOZf0yYbUNLVKR5YvvMK8dJLNFPKy0xRc,1282
+iql/_version.py,sha256=4aApRg5V4vSXSiSLtHuCgniMlv5OCRPnT6i1DuvBuKY,104
+iql/iqmoql.py,sha256=a64AXxCfvsWfC0aZYHNite4dxUEy6fp2P6kztFwAzlA,36865
+iql/options_parser.py,sha256=p0ycmeXb-IDlSNm2tbu31fbo76_dDUflIWEj5n7tkCw,1289
 iql/q_cache_base.py,sha256=y4BaW-CXnUOwzqNGnXrXhsY2h6rJWbbJXo2kNV38EDI,432
-iql/threading_experimental.py,sha256=bKsGee-Y05Rr5z1Pf1P7gBqMHUzc86l5Tbe2CXn25Hc,2191
+iql/threading_experimental.py,sha256=BB8uXN2ROy6MliV6p26C6WTPXd7qcPhkNqpXfFBS1Gc,2272
 iql/bbg_bql/__init__.py,sha256=nCTs4I9SAb24B7wg2Zd0wGsVLwamTu4BpFIIpRK0cDw,77
-iql/bbg_bql/bql_datamodel.py,sha256=1YPVfJVQE3vfaRMtAcKCxUNrrzQTeCm7D7bntIX35xw,10069
-iql/bbg_bql/bql_extension.py,sha256=6CcJ3i777igrdDFPV2p9gcpe1yiHNNgM328wHGNR0Hw,9377
-iql/bbg_bql/bql_wrapper.py,sha256=mTzxF47kkn400eh4m_jJfTycbTpk5HXTpAHLz05Ysfs,14632
+iql/bbg_bql/bql_datamodel.py,sha256=ww8CuwKYkUMA1Qx_97MJRh_FLu43GFQzWR5yAf21uHE,10079
+iql/bbg_bql/bql_extension.py,sha256=_QnWyz12hNqMuw5dBEFugWOSXxsl6oSIuFy5D8Qg5d8,9485
+iql/bbg_bql/bql_wrapper.py,sha256=nCAmgSdvPT9bq8c4Ro6gbn5TAHIjYxJeYjb364JxjRk,15045
 iql/bbg_bql/debug_tools.py,sha256=Rfs-HivxSYgGyTrByhPwiZ6QKtCn2iUnuNNmcKf1BtQ,692
 iql/db_connectors/__init__.py,sha256=nCTs4I9SAb24B7wg2Zd0wGsVLwamTu4BpFIIpRK0cDw,77
-iql/db_connectors/duckdb_connector.py,sha256=POvFTnKCnd8hudlnzOOZiJjzuTxL1mXJJiND1dnaUJo,5109
+iql/db_connectors/duckdb_connector.py,sha256=h5L0BEpU61tnChiwY2pxi7fK4glEEAZMqmKiGqOyXDM,5174
 iql/extensions/__init__.py,sha256=nCTs4I9SAb24B7wg2Zd0wGsVLwamTu4BpFIIpRK0cDw,77
 iql/extensions/aws_s3_extension.py,sha256=3yyY9LNWsZCZFFGjeIy45-zFZGIWwz7UXEAsTbV-z0g,3407
-iql/extensions/edgar_extension.py,sha256=DQEsLSMY0J5gw3bLigbRJ7emMUiNEPhbPSCGJDo0Zi0,7829
+iql/extensions/cache_extension.py,sha256=2TY4rm1omoDbOwVF7uHOOWHkn9ku0UL7QUigB7xmtCw,1575
+iql/extensions/deprecated_edgar_extension.py,sha256=DQEsLSMY0J5gw3bLigbRJ7emMUiNEPhbPSCGJDo0Zi0,7829
 iql/extensions/fred_extension.py,sha256=YZbAMy3o8fzZ01ulvO2j5rhEQRsE9BrH96WP9NyrWX0,4279
 iql/extensions/kaggle_extension.py,sha256=h1dSdWiUF-h_J7aZjwqU3Pn2s5kw_XiKcQUT0ElmPVE,4106
 iql/extensions/pandas_extension.py,sha256=soG4cxNRzB1lesrXcj5s4JL3eND4wIjsXcRNlTgphVg,2495
 iql/extensions/template_extension.py,sha256=jvF1r-ShKTM0o69wIw9aU448pe4S_lqw5Q86rusnybY,666
 iql/jupyter_magics/__init__.py,sha256=nCTs4I9SAb24B7wg2Zd0wGsVLwamTu4BpFIIpRK0cDw,77
 iql/jupyter_magics/iql_magic.py,sha256=E3BZUd7OsN3F6V8pVY30ObArsHypTRrAuhe__fpjwfk,4131
-iql-1.6.5.dist-info/LICENSE,sha256=fRoQlSrnKvIqTnrbUywcGohiS97ofE1quZqsib7WE0c,535
-iql-1.6.5.dist-info/METADATA,sha256=kCG0Y6WSjkJEnlvUgYOSYT0YWJYXmfih3EfwTojENpc,25591
-iql-1.6.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-iql-1.6.5.dist-info/top_level.txt,sha256=Tk45SvyMJ3Qip3gIAemqP9BvRhIokV7hGo3MyTS8Q0c,4
-iql-1.6.5.dist-info/RECORD,,
+iql-1.7.1rc1.dist-info/LICENSE,sha256=fRoQlSrnKvIqTnrbUywcGohiS97ofE1quZqsib7WE0c,535
+iql-1.7.1rc1.dist-info/METADATA,sha256=wCTRyO_5gutLfAFKYSmlx4a9uEiA6W9RlqGU1Yq5n-w,25594
+iql-1.7.1rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+iql-1.7.1rc1.dist-info/top_level.txt,sha256=Tk45SvyMJ3Qip3gIAemqP9BvRhIokV7hGo3MyTS8Q0c,4
+iql-1.7.1rc1.dist-info/RECORD,,
```

