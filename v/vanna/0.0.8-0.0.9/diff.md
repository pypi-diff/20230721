# Comparing `tmp/vanna-0.0.8.tar.gz` & `tmp/vanna-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.8.tar", last modified: Wed Jul 12 16:48:33 2023, max compression
+gzip compressed data, was "vanna-0.0.9.tar", last modified: Wed Jul 19 06:32:19 2023, max compression
```

## Comparing `vanna-0.0.8.tar` & `vanna-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 16:48:06.000000 vanna-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-12 16:48:33.458595 vanna-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-12 16:48:06.000000 vanna-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-12 16:48:06.000000 vanna-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:48:33.458595 vanna-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.454595 vanna-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)    16009 2023-07-12 16:48:06.000000 vanna-0.0.8/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-12 16:48:06.000000 vanna-0.0.8/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:48:33.458595 vanna-0.0.8/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 16:48:33.000000 vanna-0.0.8/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:32:19.841868 vanna-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-19 06:32:08.000000 vanna-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-19 06:32:19.841868 vanna-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-19 06:32:08.000000 vanna-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-19 06:32:08.000000 vanna-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:32:19.841868 vanna-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:32:19.837867 vanna-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:32:19.841868 vanna-0.0.9/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-07-19 06:32:08.000000 vanna-0.0.9/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-19 06:32:08.000000 vanna-0.0.9/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:32:19.841868 vanna-0.0.9/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-19 06:32:19.000000 vanna-0.0.9/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-19 06:32:19.000000 vanna-0.0.9/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:32:19.000000 vanna-0.0.9/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 06:32:19.000000 vanna-0.0.9/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 06:32:19.000000 vanna-0.0.9/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.8/LICENSE` & `vanna-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.8/PKG-INFO` & `vanna-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 | GitHub | PyPI | Colab | Documentation |
 | ------ | ---- | ----- | ------------- |
-| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/vanna_py_overview.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
+| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/notebooks/vn-starter.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
 
 # Vanna.AI
 
 Vanna is a Python-based AI SQL co-pilot. Our initial users are data-savvy data analysts, data scientists, engineers, and similar people that use Vanna to automate writing complex SQL.
 
 Vanna can:
 - [Convert natural language to SQL](#natural-language-to-sql)
```

### Comparing `vanna-0.0.8/README.md` & `vanna-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 | GitHub | PyPI | Colab | Documentation |
 | ------ | ---- | ----- | ------------- |
-| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/vanna_py_overview.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
+| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/notebooks/vn-starter.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
 
 # Vanna.AI
 
 Vanna is a Python-based AI SQL co-pilot. Our initial users are data-savvy data analysts, data scientists, engineers, and similar people that use Vanna to automate writing complex SQL.
 
 Vanna can:
 - [Convert natural language to SQL](#natural-language-to-sql)
```

### Comparing `vanna-0.0.8/pyproject.toml` & `vanna-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vanna-0.0.8/src/vanna/__init__.py` & `vanna-0.0.9/src/vanna/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 r'''
 # What is Vanna.AI?
 Vanna.AI is a platform that allows you to ask questions about your data in plain English. It is an AI-powered data analyst that can answer questions about your data, generate SQL, and create visualizations.
 
 # API Reference
 '''
-print("Vanna.AI Imported")
 
 import requests
 import pandas as pd
 import json
 import dataclasses
 import plotly
 import plotly.express as px
 import plotly.graph_objects as go
-from .types import SQLAnswer, Explanation, QuestionSQLPair, Question, QuestionId, DataResult, PlotlyResult, Status, FullQuestionDocument, QuestionList, QuestionCategory, AccuracyStats, UserEmail, UserOTP, ApiKey, OrganizationList, Organization, NewOrganization
-from typing import List, Dict, Any, Union, Optional
+from .types import SQLAnswer, Explanation, QuestionSQLPair, Question, QuestionId, DataResult, PlotlyResult, Status, FullQuestionDocument, QuestionList, QuestionCategory, AccuracyStats, UserEmail, UserOTP, ApiKey, OrganizationList, Organization, NewOrganization, StringData, QuestionStringList, Visibility, NewOrganizationMember, DataFrameJSON
+from typing import List, Dict, Any, Union, Optional, Callable, Tuple
+import warnings
+import traceback
 
 """Set the API key for Vanna.AI."""
 api_key: Union[str, None] = None # API key for Vanna.AI
 
+"""Set the SQL to DataFrame function for Vanna.AI."""
+sql_to_df: Union[Callable[[str], pd.DataFrame], None] = None # Function to convert SQL to a Pandas DataFrame
+
 __org: Union[str, None] = None # Organization name for Vanna.AI
 
-_endpoint = "https://ask.vanna.ai/rpc"
-_unauthenticated_endpoint = "https://ask.vanna.ai/unauthenticated_rpc"
+_endpoint = "https://vanna-rpc-test-x5y3argz6q-uc.a.run.app/rpc"
+_unauthenticated_endpoint = "https://vanna-rpc-test-x5y3argz6q-uc.a.run.app/unauthenticated_rpc"
 
 def __unauthenticated_rpc_call(method, params):
     headers = {
         'Content-Type': 'application/json',
     }
     data = {
         "method": method,
@@ -97,17 +101,17 @@
             return False
 
         status = Status(**d['result'])
 
         if not status.success:
             return False
 
-        otp = input("Check your email for the code and enter it here: ")
+        otp_code = input("Check your email for the code and enter it here: ")
 
-    params = [UserOTP(email=email, otp=otp)]
+    params = [UserOTP(email=email, otp=otp_code)]
 
     d = __unauthenticated_rpc_call(method="verify_otp", params=params)
 
     if 'result' not in d:
         return False
 
     key = ApiKey(**d['result'])
@@ -164,28 +168,82 @@
     if 'result' not in d:
         return False
 
     status = Status(**d['result'])
 
     return status.success
 
+def add_user_to_org(org: str, email: str, is_admin: bool) -> bool:
+    """
+    ## Example
+    ```python
+    vn.add_user_to_org(org="my-org", email="user@example.com")
+    ```
 
-def set_org(org: str) -> None:
+    Add a user to an organization.
+
+    Args:
+        org (str): The name of the organization to add the user to.
+        email (str): The email address of the user to add.
+
+    Returns:
+        bool: True if the user was added successfully, False otherwise.
+    """
+
+    params = [NewOrganizationMember(org_name=org, email=email, is_admin=is_admin)]
+
+    d = __rpc_call(method="add_user_to_org", params=params)
+
+    if 'result' not in d:
+        return False
+
+    status = Status(**d['result'])
+    
+    if not status.success:
+        print(status.message)
+
+    return status.success
+
+def set_org_visibility(visibility: bool) -> bool:
     """
     ## Example
     ```python
-    vn.set_org("my-org")
+    vn.set_org_visibility(org="my-org", visibility=True)
     ```
 
-    Set the organization name for the Vanna.AI API.
+    Set the visibility of an organization. If an organization is visible, anyone can see it. If it is not visible, only members of the organization can see it.
+
+    Args:
+        org (str): The name of the organization to set the visibility of.
+        visibility (bool): Whether or not the organization should be visible.
+
+    Returns:
+        bool: True if the organization visibility was set successfully, False otherwise.
+    """
+    params = [Visibility(visibility=visibility)]
+
+    d = __rpc_call(method="set_org_visibility", params=params)
+
+    if 'result' not in d:
+        return False
+
+    status = Status(**d['result'])
+
+    return status.success
+
+def set_org(org: str) -> None:
+    """
+    DEPRECATED. Use [`use_datasets`][vanna.use_datasets] instead.
 
     Args:
         org (str): The organization name.
     """
     global __org
+    print("vn.set_org is deprecated. Please use vn.use_datasets instead.")
+    warnings.warn("vn.set_org is deprecated. Please use vn.use_datasets instead.", DeprecationWarning)
 
     my_orgs = list_orgs()
     if org not in my_orgs:
         # Check if org exists
         d = __unauthenticated_rpc_call(method="check_org_exists", params=[Organization(name=org, user=None, connection=None)])
 
         if 'result' not in d:
@@ -205,44 +263,146 @@
                 __org = org
             else:
                 __org = None
                 raise Exception("Failed to create organization")
     else:
         __org = org
 
-def store_sql(question: str, sql: str) -> bool:
+def _set_org(org: str) -> None:
+    global __org
+
+    my_orgs = list_orgs()
+    if org not in my_orgs:
+        # Check if org exists
+        d = __unauthenticated_rpc_call(method="check_org_exists", params=[Organization(name=org, user=None, connection=None)])
+
+        if 'result' not in d:
+            raise Exception("Failed to check if organization exists")
+
+        status = Status(**d['result'])
+
+        if status.success:
+            raise Exception(f"An organization with the name {org} already exists")
+
+        create = input(f"Would you like to create organization '{org}'? (y/n): ")
+
+        if create.lower() == 'y':
+            db_type = input("What type of database would you like to use? (Snowflake, BigQuery, Postgres, etc.): ")
+            __org = 'demo-tpc-h'
+            if create_org(org=org, db_type=db_type):
+                __org = org
+            else:
+                __org = None
+                raise Exception("Failed to create organization")
+    else:
+        __org = org
+
+
+def use_datasets(datasets: List[str]):
+    """
+    ## Example
+    ```python
+    vn.use_datasets(datasets=["employees", "departments"])
+    ```
+
+    Set the datasets to use for the Vanna.AI API.
+
+    Args:
+        datasets (List[str]): A list of dataset names.
+
+    Returns:
+        bool: True if the datasets were set successfully, False otherwise.
+    """
+    if len(datasets) >= 1:
+        _set_org(org=datasets[0])
+    else:
+        raise Exception("No datasets provided")
+
+def store_sql(question: str, sql: str, tag: Union[str, None] = "Manually Trained") -> bool:
     """
     ## Example
     ```python
     vn.store_sql(
         question="What is the average salary of employees?", 
         sql="SELECT AVG(salary) FROM employees"
     )
     ```
 
     Store a question and its corresponding SQL query in the Vanna.AI database.
 
     Args:
         question (str): The question to store.
         sql (str): The SQL query to store.
+        tag (Union[str, None]): A tag to associate with the question and SQL query.
     """
     params = [QuestionSQLPair(        
         question=question,
         sql=sql,
+        tag=tag
     )]
 
     d = __rpc_call(method="store_sql", params=params)
 
     if 'result' not in d:
         return False
     
     status = Status(**d['result'])
 
     return status.success
 
+def store_ddl(ddl: str) -> bool:
+    """
+    ## Example
+    ```python
+    vn.store_ddl(
+        ddl="CREATE TABLE employees (id INT, name VARCHAR(255), salary INT)"
+    )
+    ```
+
+    Store a DDL statement in the Vanna.AI database.
+
+    Args:
+        ddl (str): The DDL statement to store.
+    """
+    params = [StringData(data=ddl)]
+
+    d = __rpc_call(method="store_ddl", params=params)
+
+    if 'result' not in d:
+        return False
+    
+    status = Status(**d['result'])
+
+    return status.success
+
+def store_documentation(documentation: str) -> bool:
+    """
+    ## Example
+    ```python
+    vn.store_documentation(
+        documentation="This is a documentation string for the employees table."
+    )
+    ```
+
+    Store a documentation string in the Vanna.AI database.
+
+    Args:
+        documentation (str): The documentation string to store.
+    """
+    params = [StringData(data=documentation)]
+
+    d = __rpc_call(method="store_documentation", params=params)
+
+    if 'result' not in d:
+        return False
+    
+    status = Status(**d['result'])
+
+    return status.success
+
 def train(question: str, sql: str) -> bool:
     """
     ## Example
     ```python
     vn.train(
         question="What is the average salary of employees?", 
         sql="SELECT AVG(salary) FROM employees"
@@ -363,31 +523,100 @@
         return None
 
     # Load the result into a dataclass
     sql_answer = SQLAnswer(**d['result'])
 
     return sql_answer.sql
 
-def ask(question: str) -> str:
+def generate_questions() -> List[str]:
+    """
+    ## Example
+    ```python
+    vn.generate_questions()
+    # ['What is the average salary of employees?', 'What is the total salary of employees?', ...]
+    ```
+
+    Generate questions using the Vanna.AI API.
+
+    Returns:
+        List[str] or None: The questions, or None if an error occurred.
+    """
+    d = __rpc_call(method="generate_questions", params=[])
+
+    if 'result' not in d:
+        return None
+
+    # Load the result into a dataclass
+    question_string_list = QuestionStringList(**d['result'])
+
+    return question_string_list.questions
+
+def ask(question: Union[str, None] = None, print_results: bool = True, auto_train: bool = True) -> Tuple[Union[str, None], Union[pd.DataFrame, None], Union[plotly.graph_objs.Figure, None]]:
     """
     ## Example
     ```python
     vn.ask(question="What is the average salary of employees?")
     # SELECT AVG(salary) FROM employees
     ```
 
-    Ask a question using the Vanna.AI API. This is equivalent to calling [`generate_sql()`][vanna.generate_sql].
+    Ask a question using the Vanna.AI API. This generates an SQL query, runs it, and returns the results in a dataframe and a Plotly figure.
 
     Args:
-        question (str): The question to ask.
+        question (str): The question to ask. If None, you will be prompted to enter a question.
 
     Returns:
         str or None: The SQL query, or None if an error occurred.
+        pd.DataFrame or None: The results of the SQL query, or None if an error occurred.
+        plotly.graph_objs.Figure or None: The Plotly figure, or None if an error occurred.
     """
-    return generate_sql(question=question)
+
+    if question is None:
+        question = input("Enter a question: ")
+
+    try:
+        sql = generate_sql(question=question)
+    except Exception as e:
+        print(e)
+        return None, None, None
+
+    if print_results:
+        print(sql)
+
+    if sql_to_df is None:
+        print("If you want to run the SQL query, provide a vn.sql_to_df function.")
+        return sql, None, None
+
+    try:
+        df = sql_to_df(sql=sql)
+
+        if print_results:
+            print(df.head().to_markdown())
+
+        try:
+            plotly_code = generate_plotly_code(question=question, sql=sql, df=df)
+            fig = get_plotly_figure(plotly_code=plotly_code, df=df)
+            if print_results:
+                fig.show()
+
+            if len(df) > 0 and auto_train:
+                store_sql(question=question, sql=sql, tag="Assumed Correct")
+
+            return sql, df, fig
+
+        except Exception as e:
+            # Print stack trace
+            traceback.print_exc()
+            print("Couldn't run plotly code: ", e)
+            return sql, df, None
+
+    except Exception as e:
+        print("Couldn't run sql: ", e)
+        return sql, None, None
+
+
 
 def generate_plotly_code(question: Union[str, None], sql: Union[str, None], df: pd.DataFrame) -> str:
     """
     ## Example
     ```python
     vn.generate_plotly_code(
         question="What is the average salary of employees?",
@@ -454,28 +683,28 @@
     if dark_mode:
         fig.update_layout(template="plotly_dark")
 
     return fig
 
 def get_results(cs, default_database: str, sql: str) -> pd.DataFrame:
     """
-    ## Example
-    ```python
-    df = vn.get_results(cs=cs, default_database="PUBLIC", sql="SELECT * FROM students")
-    ```
+    DEPRECATED. Use [`vanna.sql_to_df()`][vanna.sql_to_df] instead.
     Run the SQL query and return the results as a pandas dataframe. This is just a helper function that does not use the Vanna.AI API.
 
     Args:
         cs: Snowflake connection cursor.
         default_database (str): The default database to use.
         sql (str): The SQL query to execute.
 
     Returns:
         pd.DataFrame: The results of the SQL query.
     """
+    print("`vn.get_results()` is deprecated. Use `vn.sql_to_df()` instead.")
+    warnings.warn("`vn.get_results()` is deprecated. Use `vn.sql_to_df()` instead.")
+
     cs.execute(f"USE DATABASE {default_database}")
 
     cur = cs.execute(sql)
 
     results = cur.fetchall()
         
     # Create a pandas dataframe from the results
@@ -550,59 +779,35 @@
         return None
 
     # Load the result into a dataclass
     question = Question(**d['result'])
 
     return question.question
 
-def get_flagged_questions() -> QuestionList:
+def get_all_questions() -> pd.DataFrame:
     """
 
     ## Example
     ```python
-    questions = vn.get_flagged_questions()
+    questions = vn.get_all_questions()
     ```
     
-    Get a list of flagged questions from the Vanna.AI API.
+    Get a list of questions from the Vanna.AI API.
 
     Returns:
-        List[FullQuestionDocument] or None: The list of flagged questions, or None if an error occurred.
+        pd.DataFrame or None: The list of questions, or None if an error occurred.
 
     """
     # params = [Question(question="")]
     params = []
 
-    d = __rpc_call(method="get_flagged_questions", params=params)
+    d = __rpc_call(method="get_all_questions", params=params)
 
     if 'result' not in d:
         return None
 
     # Load the result into a dataclass
-    flagged_questions = QuestionList(**d['result'])
-
-    return flagged_questions
-
-def get_accuracy_stats() -> AccuracyStats:
-    """
-
-    ## Example
-    ```python
-    vn.get_accuracy_stats()
-    ```
-    
-    Get the accuracy statistics from the Vanna.AI API.
-
-    Returns:
-        dict or None: The accuracy statistics, or None if an error occurred.
-
-    """
-    params = []
-
-    d = __rpc_call(method="get_accuracy_stats", params=params)
+    all_questions = DataFrameJSON(**d['result'])
 
-    if 'result' not in d:
-        return None
+    df = pd.read_json(all_questions.data)
 
-    # Load the result into a dataclass
-    accuracy_stats = AccuracyStats(**d['result'])
-
-    return accuracy_stats
+    return df
```

### Comparing `vanna-0.0.8/src/vanna/types.py` & `vanna-0.0.9/src/vanna/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import List, Dict
+from typing import List, Dict, Union
 from dataclasses import dataclass
 
 @dataclass
 class Status:
     success: bool
     message: str
 
@@ -19,35 +19,50 @@
     data: DataResult | None
     plotly: PlotlyResult | None
 
 @dataclass
 class QuestionSQLPair:
     question: str
     sql: str
+    tag: Union[str, None]
 
 @dataclass
 class Organization:
     name: str
     user: str | None
     connection: Connection | None
 
 @dataclass
 class OrganizationList:
     organizations: List[str]
 
 @dataclass
+class QuestionStringList:
+    questions: List[str]
+
+@dataclass
+class Visibility:
+    visibility: bool
+
+@dataclass
 class UserEmail:
     email: str
 
 @dataclass
 class NewOrganization:
     org_name: str
     db_type: str
 
 @dataclass
+class NewOrganizationMember:
+    org_name: str
+    email: str
+    is_admin: bool
+
+@dataclass
 class UserOTP:
     email: str
     otp: str
 
 @dataclass
 class ApiKey:
     key: str
@@ -136,8 +151,16 @@
     is_foreign_key: bool
     foreign_key_table: str
     foreign_key_column: str
 
 @dataclass
 class Diagram:
     raw: str
-    mermaid_code: str
+    mermaid_code: str
+
+@dataclass
+class StringData:
+    data: str
+
+@dataclass
+class DataFrameJSON:
+    data: str
```

### Comparing `vanna-0.0.8/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.9/src/vanna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 | GitHub | PyPI | Colab | Documentation |
 | ------ | ---- | ----- | ------------- |
-| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/vanna_py_overview.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
+| [![GitHub](https://img.shields.io/badge/GitHub-vanna--py-blue?logo=github)](https://github.com/vanna-ai/vanna-py) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Colab](https://img.shields.io/badge/Colab-vanna--py-blue?logo=google-colab)](https://colab.research.google.com/github/vanna-ai/vanna-py/blob/main/notebooks/vn-starter.ipynb) | [![Documentation](https://img.shields.io/badge/Documentation-vanna--py-blue?logo=read-the-docs)](https://docs.vanna.ai) |
 
 # Vanna.AI
 
 Vanna is a Python-based AI SQL co-pilot. Our initial users are data-savvy data analysts, data scientists, engineers, and similar people that use Vanna to automate writing complex SQL.
 
 Vanna can:
 - [Convert natural language to SQL](#natural-language-to-sql)
```

