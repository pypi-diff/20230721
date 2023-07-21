# Comparing `tmp/finqual-1.1.1.tar.gz` & `tmp/finqual-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-1.1.1.tar", last modified: Tue Jul 18 23:09:19 2023, max compression
+gzip compressed data, was "finqual-1.2.0.tar", last modified: Fri Jul 21 18:20:36 2023, max compression
```

## Comparing `finqual-1.1.1.tar` & `finqual-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 23:09:19.828358 finqual-1.1.1/
--rw-rw-rw-   0        0        0     1091 2023-07-17 21:30:26.000000 finqual-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4929 2023-07-18 23:09:19.828358 finqual-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4409 2023-07-18 22:33:40.000000 finqual-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 23:09:19.818098 finqual-1.1.1/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-1.1.1/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:09:19.828358 finqual-1.1.1/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-1.1.1/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   136125 2023-07-18 23:08:12.000000 finqual-1.1.1/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:09:19.823102 finqual-1.1.1/finqual.egg-info/
--rw-rw-rw-   0        0        0     4929 2023-07-18 23:09:19.000000 finqual-1.1.1/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-18 23:09:19.000000 finqual-1.1.1/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 23:09:19.000000 finqual-1.1.1/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 23:09:19.000000 finqual-1.1.1/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 23:09:19.828358 finqual-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-07-18 23:09:08.000000 finqual-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:20:36.399713 finqual-1.2.0/
+-rw-rw-rw-   0        0        0    17529 2023-07-21 10:00:07.000000 finqual-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4975 2023-07-21 18:20:36.398712 finqual-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4409 2023-07-18 22:33:40.000000 finqual-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 18:20:36.387742 finqual-1.2.0/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-1.2.0/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:20:36.397710 finqual-1.2.0/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-1.2.0/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   137647 2023-07-21 18:16:21.000000 finqual-1.2.0/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:20:36.393625 finqual-1.2.0/finqual.egg-info/
+-rw-rw-rw-   0        0        0     4975 2023-07-21 18:20:36.000000 finqual-1.2.0/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-21 18:20:36.000000 finqual-1.2.0/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 18:20:36.000000 finqual-1.2.0/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 18:20:36.000000 finqual-1.2.0/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 18:20:36.399713 finqual-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-07-21 18:19:58.000000 finqual-1.2.0/setup.py
```

### Comparing `finqual-1.1.1/PKG-INFO` & `finqual-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 1.1.1
+Version: 1.2.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
+Home-page: https://github.com/Myztika/finqual
 Author: Harry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
 # finqual
 
 This is a work in progress package that enables users to conduct fundamental financial research, utilising the SEC's data and REST API.
 
 ## Features
```

### Comparing `finqual-1.1.1/README.md` & `finqual-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `finqual-1.1.1/finqual/data/sec_sic.csv` & `finqual-1.2.0/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-1.1.1/finqual/finqual.py` & `finqual-1.2.0/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,50 +194,67 @@
 
         try:
             data = data["facts"]["ifrs-full"]
 
         except:
             data = data["facts"]["us-gaap"]
 
-        if (category == "income"):
+        if (category == "EPS"):
             """
             Creating search term
             """
             try:
                 df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
                 df.dropna(inplace = True)
-                df["frame"] = df["frame"].str.replace('I', '')
+
+                df["frame"] = df["frame"].str.replace('CY', '')
 
                 if (quarter != None):
                     # If looking at quarter then:
-                    search = "CY" + str(year) + "Q" + str(quarter)
+
+                    df = df[df["frame"].str.contains(str(year))]
+
+                    unique_quarters = set(df["frame"])
+                    all_quarters = [str(year) + "Q" + str(i) for i in range(1, 5)]
+                    missing_quarter = list(set(all_quarters) - unique_quarters)
+
+                    if (len(missing_quarter) == 1):
+                        df["frame"] = df["frame"].replace(str(year), missing_quarter[0])
+
+                    search = str(year) + "Q" + str(quarter)
+
                 else:
-                    search = "CY" + str(year)
+                    search = str(year)
 
                 return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
             except:
-                pass
+                return False
 
+        if (category == "income"):
+            """
+            Creating search term
+            """
             try:
                 df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
-                df.dropna(inplace=True)
+                df.dropna(inplace = True)
                 df["frame"] = df["frame"].str.replace('I', '')
 
                 if (quarter != None):
                     # If looking at quarter then:
                     search = "CY" + str(year) + "Q" + str(quarter)
                 else:
                     search = "CY" + str(year)
 
                 return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
             except:
                 return False
 
+
         if (category == "balance"):
 
             """
             Getting the desired item value
             """
             try:
 
@@ -367,16 +384,34 @@
         return values
 
     def income(self, start, end, category = "income", quarter = None, readable = None):
 
         df = self.income_helper(start, end, category, quarter, readable)
         df = df.drop(["Cost and Expenses", "Interest Expense", "Depreciation and Amortization"])
 
-        df = df.round(1).applymap('{:.1f}'.format).replace('\.0$', '', regex=True)
+        no_columns = -1*len(df.columns)
+
+        nodes = [s_b,s_d]
 
+        data = [self.year_tree_item(i, start, end, category = "EPS", quarter = True) for i in nodes]
+        print(no_columns)
+
+        for i in range(len(data)):
+            if no_columns == -1:
+                data[i] = data[i][-1]
+
+            else:
+                data[i] = data[i][no_columns:]
+
+        df.loc["Number of Basic Shares"] = data[0]
+        df.loc["Number of Diluted Shares"] = data[1]
+        df.loc["Basic EPS"] = df.loc["Net Profit"]/df.loc["Number of Basic Shares"]
+        df.loc["Diluted EPS"] = df.loc["Net Profit"]/df.loc["Number of Diluted Shares"]
+        df = df.round(1).applymap('{:.1f}'.format).replace('\.0$', '', regex=True)
+        df.replace("inf", np.nan, inplace=True)
         return df
 
     def income_helper(self, start, end, category, quarter = None, readable = None):
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 2, -1)]
@@ -385,21 +420,19 @@
         """
         Creating list of income statement items and their names
         """
         nodes = [rev, cor, gp, opex, ce,
                  oi1,
                  noi, pti1, tax1, ni,
                  cce5_2,
-                 ide1_1,
-                 eps, eps_d]
+                 ide1_1]
         node_names = ["Revenues", "Cost of Revenue", "Gross Profit", "Operating Expenses", "Cost and Expenses",
                       "Operating Profit"
                      ,"Non-Operating Income/Expense", "Pretax Profit", "Tax", "Net Profit", "Depreciation and Amortization"
-                     ,"Interest Expense"
-                     , "EPS", "Diluted EPS"]
+                     ,"Interest Expense"]
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
             data = [self.year_tree_item(i, start - 1, end, category, quarter) for i in nodes]
             df = pd.DataFrame(data, index = [node_names], columns = [quarter_list])
 
@@ -895,15 +928,22 @@
 #Level 4
 
 bl4_1 = Node("AccruedEmployeeBenefitsCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_2 = Node("AccruedSalariesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_3 = Node("WorkersCompensationLiabilityCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_4 = Node("OtherEmployeeRelatedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 
+"""
+No. of shares
+"""
+s_b = Node("WeightedAverageNumberOfSharesOutstandingBasic", attribute = "debit")
+s_d = Node("WeightedAverageNumberOfDilutedSharesOutstanding", attribute = "debit")
 
+s_b1 = Node("WeightedAverageShares", attribute = "debit", parent = s_b)
+s_d1 = Node("AdjustedWeightedAverageShares", attribute = "debit", parent = s_d)
 """
 EPS
 """
 
 eps = Node("EarningsPerShareBasic", attribute = "credit")
 eps_d = Node("EarningsPerShareDiluted", attribute = "credit")
```

### Comparing `finqual-1.1.1/finqual.egg-info/PKG-INFO` & `finqual-1.2.0/finqual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 1.1.1
+Version: 1.2.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
+Home-page: https://github.com/Myztika/finqual
 Author: Harry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
 # finqual
 
 This is a work in progress package that enables users to conduct fundamental financial research, utilising the SEC's data and REST API.
 
 ## Features
```

### Comparing `finqual-1.1.1/setup.py` & `finqual-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='1.1.1',
+    version='1.2.0',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Harry',
+    url = "https://github.com/Myztika/finqual",
     packages=['finqual'],
     package_dir = {'finqual':"finqual"},
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
     classifiers=[
```

