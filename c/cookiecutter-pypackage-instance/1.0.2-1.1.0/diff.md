# Comparing `tmp/cookiecutter_pypackage_instance-1.0.2.tar.gz` & `tmp/cookiecutter_pypackage_instance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_pypackage_instance-1.0.2.tar", max compression
+gzip compressed data, was "cookiecutter_pypackage_instance-1.1.0.tar", max compression
```

## Comparing `cookiecutter_pypackage_instance-1.0.2.tar` & `cookiecutter_pypackage_instance-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/LICENSE
--rw-r--r--   0        0        0     4136 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/README.md
--rw-r--r--   0        0        0     4952 2023-05-25 16:39:05.019072 cookiecutter_pypackage_instance-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/__init__.py
--rw-r--r--   0        0        0      417 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
--rw-r--r--   0        0        0        0 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/py.typed
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-21 06:17:50.180215 cookiecutter_pypackage_instance-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4320 2023-07-21 06:17:50.180215 cookiecutter_pypackage_instance-1.1.0/README.md
+-rw-r--r--   0        0        0     5106 2023-07-21 06:17:51.556273 cookiecutter_pypackage_instance-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
+-rw-r--r--   0        0        0        0 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/py.typed
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.1.0/PKG-INFO
```

### Comparing `cookiecutter_pypackage_instance-1.0.2/LICENSE` & `cookiecutter_pypackage_instance-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_pypackage_instance-1.0.2/README.md` & `cookiecutter_pypackage_instance-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,18 @@
   </a>
   <a href="https://opensource.org/licenses/MIT">
     <img
       src="https://img.shields.io/pypi/l/cookiecutter-pypackage-instance"
       alt="PyPI - License"
     />
   </a>
-  <a href="https://gitpod.io/from-referrer/">
+  <a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/billsioros/cookiecutter-pypackage-instance">
     <img
-      src="https://img.shields.io/badge/Open%20on-Gitpod-blue?logo=gitpod&style=flat"
-      alt="Open on Gitpod"
+      src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode"
+      alt="Open in GitHub Codespaces"
     />
   </a>
   <a href="https://github.com/billsioros/cookiecutter-pypackage">
     <img
       src="https://img.shields.io/badge/cookiecutter-template-D4AA00.svg?style=flat&logo=cookiecutter"
       alt="Cookiecutter Template">
   </a>
@@ -92,14 +92,15 @@
 
 # Create a virtual environment using poetry and install the required dependencies
 poetry shell
 poetry install
 
 # Install pre-commit hooks
 pre-commit install --install-hooks
+pre-commit autoupdate
 ```
 
 ## :book: Documentation
 
 The project's documentation can be found [here](https://billsioros.github.io/cookiecutter-pypackage-instance/).
 
 ## :heart: Support the project
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
                  ****** Cookiecutter Pypackage Instance ******
   ð An awesome python package by the name Cookiecutter Pypackage Instance
 [PyPI_-_Python_Version] [PyPI] [CI] [CD] [pre-commit.ci_status] [Test_Coverage]
-[PyPI_-_License] [Open_on_Gitpod] [Cookiecutter_Template] [Renovate_-_Enabled]
-                       [Buy_me_a_coffee] [FOSSA_Status]
+[PyPI_-_License] [Open_in_GitHub_Codespaces] [Cookiecutter_Template] [Renovate
+                  -_Enabled] [Buy_me_a_coffee] [FOSSA_Status]
 ## :cd: Installation ```bash pip install cookiecutter-pypackage-instance ``` In
 order to locally set up the project please follow the instructions below:
 ```shell # Set up the GitHub repository git init git config --local user.name
 Vasilis Sioros git config --local user.email billsioros97@gmail.com git add .
 git commit -m "feat: initial commit" git remote add origin https://github.com/
 billsioros/cookiecutter-pypackage-instance # Create a virtual environment using
 poetry and install the required dependencies poetry shell poetry install #
-Install pre-commit hooks pre-commit install --install-hooks ``` ## :book:
-Documentation The project's documentation can be found [here](https://
-billsioros.github.io/cookiecutter-pypackage-instance/). ## :heart: Support the
-project Feel free to [**Buy me a coffee! â**](https://www.buymeacoffee.com/
-billsioros). ## :sparkles: Contributing If you would like to contribute to the
-project, please go through the [Contributing Guidelines](https://
-billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/
-) first. ## :label: Credits This project was generated with [`billsioros/
-cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage)
-cookiecutter template.
+Install pre-commit hooks pre-commit install --install-hooks pre-commit
+autoupdate ``` ## :book: Documentation The project's documentation can be found
+[here](https://billsioros.github.io/cookiecutter-pypackage-instance/). ## :
+heart: Support the project Feel free to [**Buy me a coffee! â**](https://
+www.buymeacoffee.com/billsioros). ## :sparkles: Contributing If you would like
+to contribute to the project, please go through the [Contributing Guidelines]
+(https://billsioros.github.io/cookiecutter-pypackage-instance/latest/
+CONTRIBUTING/) first. ## :label: Credits This project was generated with
+[`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/
+cookiecutter-pypackage) cookiecutter template.
```

### Comparing `cookiecutter_pypackage_instance-1.0.2/pyproject.toml` & `cookiecutter_pypackage_instance-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,82 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core>=1",
+]
+
+[tool.black]
+line-length = 99
+target-version = ["py37", "py38"]
+skip-string-normalization = true
+
+[tool.isort]
+profile = "black"
+src_paths = ["src/cookiecutter_pypackage_instance", "tests"]
+line_length = 99
+known_first_party = "cookiecutter_pypackage_instance"
+
+[tool.pytest.ini_options]
+addopts = "-vv --color=yes"
+log_cli = false
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+log_cli_format = "%(asctime)s %(levelname)s %(message)s"
+log_cli_level = "INFO"
+python_files = "test_*.py"
+python_functions = "test_*"
+testpaths = "tests"
+
+[tool.coverage.paths]
+source = ["src"]
+
+[tool.coverage.run]
+branch = true
+source = ["cookiecutter_pypackage_instance"]
+
+[tool.coverage.report]
+show_missing = true
+fail_under = 100
+exclude_lines = ["if self.debug:", "pragma: no cover", "raise NotImplementedError", "if __name__ == .__main__.:"]
+ignore_errors = true
+omit = ["tests/*"]
+
+[tool.mypy]
+files = ["src/cookiecutter_pypackage_instance"]
+warn_unused_configs = true
+warn_return_any = true
+ignore_missing_imports = true
+pretty = true
+color_output = true
+show_column_numbers = true
+show_error_codes = true
+show_error_context = true
+strict = true
 
 [tool.poetry]
 name = "cookiecutter-pypackage-instance"
-version = "1.0.2"
+version = "1.1.0"
 description = "🐍 An awesome python package by the name Cookiecutter Pypackage Instance"
 readme = "README.md"
 authors = ["Vasilis Sioros <billsioros97@gmail.com>"]
 license = "MIT"
 homepage = "https://billsioros.github.io/cookiecutter-pypackage-instance"
 repository = "https://github.com/billsioros/cookiecutter-pypackage-instance"
 keywords = []
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/billsioros/cookiecutter-pypackage-instance/issues"
 "Changelog" = "https://github.com/billsioros/cookiecutter-pypackage-instance/releases"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.7,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "*"
 isort = "*"
 mypy = "*"
 black = "*"
 pre-commit = "*"
@@ -43,81 +91,14 @@
 mkdocs-minify-plugin = "*"
 mkdocs-redirects = "*"
 mkdocstrings = { extras = ["python"], version = "*" }
 mdx-truly-sane-lists = "*"
 mike = "*"
 ruff = "*"
 
-[tool.semantic_release]
-version_toml = "pyproject.toml:tool.poetry.version"
-changelog_components = "semantic_release.changelog.changelog_headers,semantic_release.changelog.compare_url"
-build_command = "python -m pip install poetry && poetry build"
-
-[tool.vulture]
-min_confidence = 95
-paths = ["src/cookiecutter_pypackage_instance", "tests"]
-
-[tool.poe.tasks]
-clean = { cmd = "rm -rf ./**/__pycache__ dist site .pytest_cache .mypy_cache .coverage", help = "Clean up any auxiliary files" }
-format = { shell = "poetry run isort .; poetry run black .", help = "Format your codebase" }
-hooks = { cmd = "poetry run pre-commit run --all-files", help = "Run all pre-commit hooks" }
-test = { cmd = "poetry run pytest --cov=cookiecutter_pypackage_instance", help = "Run the test suite and produce a coverage report" }
-type-check = { cmd = "poetry run mypy", help = "Run static type checking on your codebase" }
-lint = { cmd = "poetry run ruff check src", help = "Lint your code for errors" }
-docs = { shell = "python -c 'import webbrowser; webbrowser.open(\"http://127.0.0.1:8000\")'; poetry run mkdocs serve", help = "Build and serve the documentation" }
-export = { cmd = "poetry export --without-hashes --dev -o requirements.txt" }
-
-[tool.pytest.ini_options]
-addopts = "-vv --color=yes"
-log_cli = false
-log_cli_date_format = "%Y-%m-%d %H:%M:%S"
-log_cli_format = "%(asctime)s %(levelname)s %(message)s"
-log_cli_level = "INFO"
-python_files = "test_*.py"
-python_functions = "test_*"
-testpaths = "tests"
-
-[tool.coverage.paths]
-source = ["src"]
-
-[tool.coverage.run]
-branch = true
-source = ["cookiecutter_pypackage_instance"]
-
-[tool.coverage.report]
-show_missing = true
-fail_under = 100
-exclude_lines = ["if self.debug:", "pragma: no cover", "raise NotImplementedError", "if __name__ == .__main__.:"]
-ignore_errors = true
-omit = ["tests/*"]
-
-[tool.isort]
-profile = "black"
-src_paths = ["src/cookiecutter_pypackage_instance", "tests"]
-line_length = 99
-known_first_party = "cookiecutter_pypackage_instance"
-
-[tool.black]
-line-length = 99
-target-version = ["py37", "py38"]
-skip-string-normalization = true
-
-[tool.mypy]
-files = ["src/cookiecutter_pypackage_instance"]
-warn_unused_configs = true
-warn_return_any = true
-ignore_missing_imports = true
-pretty = true
-color_output = true
-show_column_numbers = true
-show_error_codes = true
-show_error_context = true
-strict = true
-
-
 [tool.ruff]
 select = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 ignore = []
 
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
@@ -156,7 +137,39 @@
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
+
+[tool.semantic_release]
+version_toml = "pyproject.toml:tool.poetry.version"
+changelog_components = "semantic_release.changelog.changelog_headers,semantic_release.changelog.compare_url"
+build_command = "python -m pip install poetry && poetry build"
+
+[tool.vulture]
+min_confidence = 95
+paths = ["src/cookiecutter_pypackage_instance", "tests"]
+
+[tool.poe.tasks]
+clean = { cmd = "rm -rf ./**/__pycache__ dist site .pytest_cache .mypy_cache .coverage", help = "Clean up any auxiliary files" }
+format = { shell = "poetry run isort .; poetry run black .", help = "Format your codebase" }
+hooks = { cmd = "poetry run pre-commit run --all-files", help = "Run all pre-commit hooks" }
+test = { cmd = "poetry run pytest --cov=cookiecutter_pypackage_instance", help = "Run the test suite and produce a coverage report" }
+type-check = { cmd = "poetry run mypy", help = "Run static type checking on your codebase" }
+lint = { cmd = "poetry run ruff check src", help = "Lint your code for errors" }
+docs = { shell = "python -c 'import webbrowser; webbrowser.open(\"http://127.0.0.1:8000\")'; poetry run mkdocs serve", help = "Build and serve the documentation" }
+export = { cmd = "poetry export --without-hashes --dev -o requirements.txt" }
+
+[tool.docformatter]
+black = true
+non-strict = true
+non-cap = [
+  "cookiecutter_pypackage_instance",
+]
+recursive = true
+in-place = true
+
+[tool.bandit]
+recursive = true
+exclude_dirs = ["tests"]
```

### Comparing `cookiecutter_pypackage_instance-1.0.2/PKG-INFO` & `cookiecutter_pypackage_instance-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: cookiecutter-pypackage-instance
-Version: 1.0.2
+Version: 1.1.0
 Summary: 🐍 An awesome python package by the name Cookiecutter Pypackage Instance
 Home-page: https://billsioros.github.io/cookiecutter-pypackage-instance
 License: MIT
 Author: Vasilis Sioros
 Author-email: billsioros97@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Bug Tracker, https://github.com/billsioros/cookiecutter-pypackage-instance/issues
 Project-URL: Changelog, https://github.com/billsioros/cookiecutter-pypackage-instance/releases
 Project-URL: Repository, https://github.com/billsioros/cookiecutter-pypackage-instance
@@ -61,18 +63,18 @@
   </a>
   <a href="https://opensource.org/licenses/MIT">
     <img
       src="https://img.shields.io/pypi/l/cookiecutter-pypackage-instance"
       alt="PyPI - License"
     />
   </a>
-  <a href="https://gitpod.io/from-referrer/">
+  <a href="https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/billsioros/cookiecutter-pypackage-instance">
     <img
-      src="https://img.shields.io/badge/Open%20on-Gitpod-blue?logo=gitpod&style=flat"
-      alt="Open on Gitpod"
+      src="https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode"
+      alt="Open in GitHub Codespaces"
     />
   </a>
   <a href="https://github.com/billsioros/cookiecutter-pypackage">
     <img
       src="https://img.shields.io/badge/cookiecutter-template-D4AA00.svg?style=flat&logo=cookiecutter"
       alt="Cookiecutter Template">
   </a>
@@ -113,14 +115,15 @@
 
 # Create a virtual environment using poetry and install the required dependencies
 poetry shell
 poetry install
 
 # Install pre-commit hooks
 pre-commit install --install-hooks
+pre-commit autoupdate
 ```
 
 ## :book: Documentation
 
 The project's documentation can be found [here](https://billsioros.github.io/cookiecutter-pypackage-instance/).
 
 ## :heart: Support the project
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.0.2
+Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.1.0
 Summary: ð An awesome python package by the name Cookiecutter Pypackage
 Instance Home-page: https://billsioros.github.io/cookiecutter-pypackage-
 instance License: MIT Author: Vasilis Sioros Author-email:
-billsioros97@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+billsioros97@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Project-URL: Bug Tracker, https://github.com/billsioros/
-cookiecutter-pypackage-instance/issues Project-URL: Changelog, https://
-github.com/billsioros/cookiecutter-pypackage-instance/releases Project-URL:
-Repository, https://github.com/billsioros/cookiecutter-pypackage-instance
-Description-Content-Type: text/markdown
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3 :: Only Project-URL: Bug Tracker, https://
+github.com/billsioros/cookiecutter-pypackage-instance/issues Project-URL:
+Changelog, https://github.com/billsioros/cookiecutter-pypackage-instance/
+releases Project-URL: Repository, https://github.com/billsioros/cookiecutter-
+pypackage-instance Description-Content-Type: text/markdown
                  ****** Cookiecutter Pypackage Instance ******
   ð An awesome python package by the name Cookiecutter Pypackage Instance
 [PyPI_-_Python_Version] [PyPI] [CI] [CD] [pre-commit.ci_status] [Test_Coverage]
-[PyPI_-_License] [Open_on_Gitpod] [Cookiecutter_Template] [Renovate_-_Enabled]
-                       [Buy_me_a_coffee] [FOSSA_Status]
+[PyPI_-_License] [Open_in_GitHub_Codespaces] [Cookiecutter_Template] [Renovate
+                  -_Enabled] [Buy_me_a_coffee] [FOSSA_Status]
 ## :cd: Installation ```bash pip install cookiecutter-pypackage-instance ``` In
 order to locally set up the project please follow the instructions below:
 ```shell # Set up the GitHub repository git init git config --local user.name
 Vasilis Sioros git config --local user.email billsioros97@gmail.com git add .
 git commit -m "feat: initial commit" git remote add origin https://github.com/
 billsioros/cookiecutter-pypackage-instance # Create a virtual environment using
 poetry and install the required dependencies poetry shell poetry install #
-Install pre-commit hooks pre-commit install --install-hooks ``` ## :book:
-Documentation The project's documentation can be found [here](https://
-billsioros.github.io/cookiecutter-pypackage-instance/). ## :heart: Support the
-project Feel free to [**Buy me a coffee! â**](https://www.buymeacoffee.com/
-billsioros). ## :sparkles: Contributing If you would like to contribute to the
-project, please go through the [Contributing Guidelines](https://
-billsioros.github.io/cookiecutter-pypackage-instance/latest/CONTRIBUTING/
-) first. ## :label: Credits This project was generated with [`billsioros/
-cookiecutter-pypackage`](https://github.com/billsioros/cookiecutter-pypackage)
-cookiecutter template.
+Install pre-commit hooks pre-commit install --install-hooks pre-commit
+autoupdate ``` ## :book: Documentation The project's documentation can be found
+[here](https://billsioros.github.io/cookiecutter-pypackage-instance/). ## :
+heart: Support the project Feel free to [**Buy me a coffee! â**](https://
+www.buymeacoffee.com/billsioros). ## :sparkles: Contributing If you would like
+to contribute to the project, please go through the [Contributing Guidelines]
+(https://billsioros.github.io/cookiecutter-pypackage-instance/latest/
+CONTRIBUTING/) first. ## :label: Credits This project was generated with
+[`billsioros/cookiecutter-pypackage`](https://github.com/billsioros/
+cookiecutter-pypackage) cookiecutter template.
```

