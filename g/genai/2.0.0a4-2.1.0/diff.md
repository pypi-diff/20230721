# Comparing `tmp/genai-2.0.0a4.tar.gz` & `tmp/genai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genai-2.0.0a4.tar", max compression
+gzip compressed data, was "genai-2.1.0.tar", max compression
```

## Comparing `genai-2.0.0a4.tar` & `genai-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1495 2023-03-11 01:05:29.282993 genai-2.0.0a4/LICENSE
--rw-r--r--   0        0        0     5669 2023-03-15 01:15:38.702724 genai-2.0.0a4/README.md
--rw-r--r--   0        0        0      598 2023-03-24 21:31:24.691480 genai-2.0.0a4/genai/__init__.py
--rw-r--r--   0        0        0       30 2023-03-24 21:31:39.310800 genai-2.0.0a4/genai/_version.py
--rw-r--r--   0        0        0     4946 2023-03-24 21:31:24.692465 genai-2.0.0a4/genai/context.py
--rw-r--r--   0        0        0     3891 2023-03-24 21:31:40.107998 genai-2.0.0a4/genai/display.py
--rw-r--r--   0        0        0     2563 2023-03-24 15:00:29.071468 genai-2.0.0a4/genai/generate.py
--rw-r--r--   0        0        0     6057 2023-03-24 21:31:24.692978 genai-2.0.0a4/genai/magics.py
--rw-r--r--   0        0        0     2253 2023-03-24 15:00:29.072055 genai-2.0.0a4/genai/prompts.py
--rw-r--r--   0        0        0     3295 2023-03-22 14:26:01.275997 genai-2.0.0a4/genai/suggestions.py
--rw-r--r--   0        0        0     2550 2023-03-18 15:24:41.999316 genai-2.0.0a4/genai/tokens.py
--rw-r--r--   0        0        0     2549 2023-03-24 21:31:39.310728 genai-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     6801 1970-01-01 00:00:00.000000 genai-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-03-11 01:05:29.282993 genai-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5577 2023-03-25 02:22:02.628119 genai-2.1.0/README.md
+-rw-r--r--   0        0        0      598 2023-03-25 10:46:32.007263 genai-2.1.0/genai/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 01:54:45.641384 genai-2.1.0/genai/_version.py
+-rw-r--r--   0        0        0     8613 2023-03-31 21:17:40.683102 genai-2.1.0/genai/context.py
+-rw-r--r--   0        0        0     3891 2023-03-25 00:42:17.894641 genai-2.1.0/genai/display.py
+-rw-r--r--   0        0        0     2563 2023-03-24 15:00:29.071468 genai-2.1.0/genai/generate.py
+-rw-r--r--   0        0        0     6057 2023-03-25 00:42:17.894870 genai-2.1.0/genai/magics.py
+-rw-r--r--   0        0        0     2253 2023-03-24 15:00:29.072055 genai-2.1.0/genai/prompts.py
+-rw-r--r--   0        0        0     3295 2023-07-21 01:52:17.642938 genai-2.1.0/genai/suggestions.py
+-rw-r--r--   0        0        0     2550 2023-03-18 15:24:41.999316 genai-2.1.0/genai/tokens.py
+-rw-r--r--   0        0        0     2735 2023-07-21 01:54:45.641681 genai-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6523 1970-01-01 00:00:00.000000 genai-2.1.0/PKG-INFO
```

### Comparing `genai-2.0.0a4/LICENSE` & `genai-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/README.md` & `genai-2.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [Install](#installation) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)
 
 # GenAI: generative AI tooling for IPython
 
-Generate code cells and get recommendations after exceptions in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+🦾 Get GPT help with code, SQL queries, DataFrames, Exceptions and more in IPython.
 
-TL;DR
+🌍 Supports all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+
+TL;DR Get started now
 
 ```
 %pip install genai
 %load_ext genai
 ```
 
 ## Genai In Action
@@ -18,15 +20,15 @@
 - [Blog Post](https://noteable.io/blog/introducing-genai/)
 - [Example Notebook](https://app.noteable.io/f/1605d16d-f5d3-4099-8fec-2ca727075b3b/Introducing-Genai.ipynb)
 
 <!-- --8<-- [start:intro] -->
 
 ## Introduction
 
-We've taken the context from IPython, mixed it with OpenAI's Large Language Models, and given you the power to generate code cells and get recommendations after exceptions in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+We've taken the context from IPython, mixed it with OpenAI's Large Language Models, and are bringing you a more informed notebook experience that works in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable. 🦾🌏
 
 <!-- --8<-- [end:intro] -->
 
 <!-- --8<-- [start:requirements] -->
 
 ## Requirements
 
@@ -116,44 +118,43 @@
 print(df_sorted)
 ```
 
 In this example, the `by` argument is set to `'Age'`, which sorts the dataframe by age in ascending order. Note that you can also pass a list of column names if you want to sort by multiple columns.
 
 ## Example
 
-```python
+````python
 In [1]: %load_ext genai
 
 In [2]: %%assist
    ...:
-   ...: # Pull census data
-   ...:
-'What would a data analyst do? 🤔'
-
-In [3]: # generated with %%assist
-   ...: # Pull census data
-   ...: # To pull census data we can use the `requests` library to send a GET request to the appropriate API endpoint.
-   ...: # First, import the requests module
-   ...: import requests
-   ...:
-   ...: # Define the URL endpoint to the Census API
-   ...: url = "https://api.census.gov/data/2019/pep/population"
+   ...: Can you explain this query to me so I can be sure we're doing the right things?
    ...:
-   ...: # Define the parameters needed for the API request, such as dataset and variables requested
-   ...: params = {
-   ...:     "get": "POP",
-   ...:     "for": "state:*",
-   ...: }
-   ...:
-   ...: # Send a GET request to the Census API endpoint with the parameters
-   ...: response = requests.get(url, params=params)
-   ...:
-   ...: # Access the response content
-   ...: content = response.content
-   ...:
-   ...: # The Census data is now stored in the `content` variable and can be processed or saved elsewhere. The user can modify the `params` variable to request different data or specify a different API endpoint.
-
-In [6]: content
-Out[6]: b'[["POP","state"],\n["4903185","01"],\n["731545","02"],\n["7278717","04"],\n["3017804","05"],\n["39512223","06"],\n["5758736","08"],\n["973764","10"],\n["705749","11"],\n["3565287","09"],\n["21477737","12"],\n["10617423","13"],\n["1787065","16"],\n["1415872","15"],\n["12671821","17"],\n["6732219","18"],\n["3155070","19"],\n["2913314","20"],\n["4467673","21"],\n["4648794","22"],\n["1344212","23"],\n["6045680","24"],\n["6892503","25"],\n["9986857","26"],\n["5639632","27"],\n["2976149","28"],\n["6137428","29"],\n["1068778","30"],\n["1934408","31"],\n["3080156","32"],\n["1359711","33"],\n["8882190","34"],\n["2096829","35"],\n["19453561","36"],\n["10488084","37"],\n["762062","38"],\n["11689100","39"],\n["3956971","40"],\n["4217737","41"],\n["12801989","42"],\n["1059361","44"],\n["5148714","45"],\n["884659","46"],\n["6829174","47"],\n["28995881","48"],\n["623989","50"],\n["3205958","49"],\n["8535519","51"],\n["7614893","53"],\n["1792147","54"],\n["5822434","55"],\n["578759","56"],\n["3193694","72"]]'
+   ...: ```sql
+   ...: SELECT
+   ...:   COUNT(*) AS num_downloads,
+   ...:   DATE_TRUNC(DATE(timestamp), DAY) AS day
+   ...: FROM `bigquery-public-data.pypi.file_downloads`
+   ...: WHERE
+   ...:   file.project = 'genai'
+   ...:   -- Only query the last 6 months of history
+   ...:   AND DATE(timestamp)
+   ...:     BETWEEN DATE_TRUNC(DATE_SUB(CURRENT_DATE(), INTERVAL 6 MONTH), MONTH)
+   ...:     AND CURRENT_DATE()
+   ...: GROUP BY day
+   ...: ORDER BY day DESC
+````
+
+```markdown
+"This is a SQL query that counts the number of downloads for the 'genai' project on the Python Package Index (PyPI) over the last 6 months, grouped by day. The query selects the count and the date, truncating the date to the day level so that it's easier to read.
+
+Here is a breakdown of each part of the query:
+
+- `SELECT COUNT(*) AS num_downloads, DATE_TRUNC(DATE(timestamp), DAY) AS day`: This selects the count of the number of rows matched by the query as `num_downloads`, and the date truncated to the day level as `day`.
+- `FROM `bigquery-public-data.pypi.file_downloads``: This specifies the table to query from.
+- `WHERE file.project = 'genai'`: This filters the rows by only including downloads for the 'genai' project.
+- `AND DATE(timestamp) BETWEEN DATE_TRUNC(DATE_SUB(CURRENT_DATE(), INTERVAL 6 MONTH), MONTH) AND CURRENT_DATE()`: This filters the rows by only including downloads from the last 6 months. The `DATE_SUB` function subtracts 6 months from the current date (`CURRENT_DATE()`), `DATE_TRUNC` truncates the result to be the start of the month and `DATE` converts the timestamp column to a date so the `BETWEEN` condition can filter rows between the start of 6 months ago and "today."
+- `GROUP BY day`: This groups the rows by day so that the counts are aggregated by date.
+- `ORDER BY day DESC`: This orders the rows so that the most recent date appears first in the result."
 ```
 
 <!-- --8<-- [end:start] -->
```

### Comparing `genai-2.0.0a4/genai/__init__.py` & `genai-2.1.0/genai/__init__.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/display.py` & `genai-2.1.0/genai/display.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/generate.py` & `genai-2.1.0/genai/generate.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/magics.py` & `genai-2.1.0/genai/magics.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/prompts.py` & `genai-2.1.0/genai/prompts.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/suggestions.py` & `genai-2.1.0/genai/suggestions.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/genai/tokens.py` & `genai-2.1.0/genai/tokens.py`

 * *Files identical despite different names*

### Comparing `genai-2.0.0a4/pyproject.toml` & `genai-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "genai"
-version = "2.0.0-alpha.4"
+version = "2.1.0"
 description = "Generative AI for IPython (enhance your code cells)"
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 maintainers = ["Kyle Kelley <rgbkrk@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 # old setup.cfg had a bdist_wheel option.
 # To build a wheel, use poetry build -f wheel
@@ -30,15 +30,14 @@
 [[tool.poetry.source]]
 name = "genai"
 url = "https://pypi.org"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openai = "^0.27.0"
-vdom = "^0.6"
 ipython = "^8.10.0"
 tabulate = "^0.9.0"
 tiktoken = "^0.3.2"
 
 [tool.poetry.dev-dependencies]
 flake8-docstrings = "^1.6.0"
 pytest = "^7.2.2"
@@ -55,14 +54,17 @@
 pandas = "^1.5.3"
 mypy = "^1.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.1"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.distutils.bdist_wheel]
+universal = 0
+
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
@@ -97,8 +99,19 @@
 [tool.coverage.report]
 exclude_lines = ["if self.debug:",
                  "pragma: no cover",
                  "raise AssertionError",
                  "raise NotImplementedError",
                  "if __name__ == '__main__':"]
 ignore_errors = true
-omit = ["genai/_version.py"]
+omit = [
+  "*/tests/*",
+  "genai/_version.py"
+]
+
+[tool.mypy]
+ignore_missing_imports = true
+warn_unused_configs = true
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+filterwarnings = "always"
```

### Comparing `genai-2.0.0a4/PKG-INFO` & `genai-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genai
-Version: 2.0.0a4
+Version: 2.1.0
 Summary: Generative AI for IPython (enhance your code cells)
 License: BSD-3-Clause
 Keywords: notebook,api,noteable,chatgpt,gpt3,openai,ipython,traceback,assist,llm
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Maintainer: Kyle Kelley
 Maintainer-email: rgbkrk@gmail.com
@@ -13,31 +13,29 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: ipython (>=8.10.0,<9.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tiktoken (>=0.3.2,<0.4.0)
-Requires-Dist: vdom (>=0.6,<0.7)
 Description-Content-Type: text/markdown
 
 [Install](#installation) | [License](./LICENSE) | [Code of Conduct](./CODE_OF_CONDUCT.md) | [Contributing](./CONTRIBUTING.md)
 
 # GenAI: generative AI tooling for IPython
 
-Generate code cells and get recommendations after exceptions in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+🦾 Get GPT help with code, SQL queries, DataFrames, Exceptions and more in IPython.
 
-TL;DR
+🌍 Supports all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+
+TL;DR Get started now
 
 ```
 %pip install genai
 %load_ext genai
 ```
 
 ## Genai In Action
@@ -47,15 +45,15 @@
 - [Blog Post](https://noteable.io/blog/introducing-genai/)
 - [Example Notebook](https://app.noteable.io/f/1605d16d-f5d3-4099-8fec-2ca727075b3b/Introducing-Genai.ipynb)
 
 <!-- --8<-- [start:intro] -->
 
 ## Introduction
 
-We've taken the context from IPython, mixed it with OpenAI's Large Language Models, and given you the power to generate code cells and get recommendations after exceptions in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable.
+We've taken the context from IPython, mixed it with OpenAI's Large Language Models, and are bringing you a more informed notebook experience that works in all Jupyter environments, including IPython, JupyterLab, Jupyter Notebook, and Noteable. 🦾🌏
 
 <!-- --8<-- [end:intro] -->
 
 <!-- --8<-- [start:requirements] -->
 
 ## Requirements
 
@@ -145,45 +143,44 @@
 print(df_sorted)
 ```
 
 In this example, the `by` argument is set to `'Age'`, which sorts the dataframe by age in ascending order. Note that you can also pass a list of column names if you want to sort by multiple columns.
 
 ## Example
 
-```python
+````python
 In [1]: %load_ext genai
 
 In [2]: %%assist
    ...:
-   ...: # Pull census data
-   ...:
-'What would a data analyst do? 🤔'
-
-In [3]: # generated with %%assist
-   ...: # Pull census data
-   ...: # To pull census data we can use the `requests` library to send a GET request to the appropriate API endpoint.
-   ...: # First, import the requests module
-   ...: import requests
-   ...:
-   ...: # Define the URL endpoint to the Census API
-   ...: url = "https://api.census.gov/data/2019/pep/population"
-   ...:
-   ...: # Define the parameters needed for the API request, such as dataset and variables requested
-   ...: params = {
-   ...:     "get": "POP",
-   ...:     "for": "state:*",
-   ...: }
+   ...: Can you explain this query to me so I can be sure we're doing the right things?
    ...:
-   ...: # Send a GET request to the Census API endpoint with the parameters
-   ...: response = requests.get(url, params=params)
-   ...:
-   ...: # Access the response content
-   ...: content = response.content
-   ...:
-   ...: # The Census data is now stored in the `content` variable and can be processed or saved elsewhere. The user can modify the `params` variable to request different data or specify a different API endpoint.
-
-In [6]: content
-Out[6]: b'[["POP","state"],\n["4903185","01"],\n["731545","02"],\n["7278717","04"],\n["3017804","05"],\n["39512223","06"],\n["5758736","08"],\n["973764","10"],\n["705749","11"],\n["3565287","09"],\n["21477737","12"],\n["10617423","13"],\n["1787065","16"],\n["1415872","15"],\n["12671821","17"],\n["6732219","18"],\n["3155070","19"],\n["2913314","20"],\n["4467673","21"],\n["4648794","22"],\n["1344212","23"],\n["6045680","24"],\n["6892503","25"],\n["9986857","26"],\n["5639632","27"],\n["2976149","28"],\n["6137428","29"],\n["1068778","30"],\n["1934408","31"],\n["3080156","32"],\n["1359711","33"],\n["8882190","34"],\n["2096829","35"],\n["19453561","36"],\n["10488084","37"],\n["762062","38"],\n["11689100","39"],\n["3956971","40"],\n["4217737","41"],\n["12801989","42"],\n["1059361","44"],\n["5148714","45"],\n["884659","46"],\n["6829174","47"],\n["28995881","48"],\n["623989","50"],\n["3205958","49"],\n["8535519","51"],\n["7614893","53"],\n["1792147","54"],\n["5822434","55"],\n["578759","56"],\n["3193694","72"]]'
+   ...: ```sql
+   ...: SELECT
+   ...:   COUNT(*) AS num_downloads,
+   ...:   DATE_TRUNC(DATE(timestamp), DAY) AS day
+   ...: FROM `bigquery-public-data.pypi.file_downloads`
+   ...: WHERE
+   ...:   file.project = 'genai'
+   ...:   -- Only query the last 6 months of history
+   ...:   AND DATE(timestamp)
+   ...:     BETWEEN DATE_TRUNC(DATE_SUB(CURRENT_DATE(), INTERVAL 6 MONTH), MONTH)
+   ...:     AND CURRENT_DATE()
+   ...: GROUP BY day
+   ...: ORDER BY day DESC
+````
+
+```markdown
+"This is a SQL query that counts the number of downloads for the 'genai' project on the Python Package Index (PyPI) over the last 6 months, grouped by day. The query selects the count and the date, truncating the date to the day level so that it's easier to read.
+
+Here is a breakdown of each part of the query:
+
+- `SELECT COUNT(*) AS num_downloads, DATE_TRUNC(DATE(timestamp), DAY) AS day`: This selects the count of the number of rows matched by the query as `num_downloads`, and the date truncated to the day level as `day`.
+- `FROM `bigquery-public-data.pypi.file_downloads``: This specifies the table to query from.
+- `WHERE file.project = 'genai'`: This filters the rows by only including downloads for the 'genai' project.
+- `AND DATE(timestamp) BETWEEN DATE_TRUNC(DATE_SUB(CURRENT_DATE(), INTERVAL 6 MONTH), MONTH) AND CURRENT_DATE()`: This filters the rows by only including downloads from the last 6 months. The `DATE_SUB` function subtracts 6 months from the current date (`CURRENT_DATE()`), `DATE_TRUNC` truncates the result to be the start of the month and `DATE` converts the timestamp column to a date so the `BETWEEN` condition can filter rows between the start of 6 months ago and "today."
+- `GROUP BY day`: This groups the rows by day so that the counts are aggregated by date.
+- `ORDER BY day DESC`: This orders the rows so that the most recent date appears first in the result."
 ```
 
 <!-- --8<-- [end:start] -->
```

