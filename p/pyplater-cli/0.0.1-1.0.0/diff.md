# Comparing `tmp/pyplater_cli-0.0.1.tar.gz` & `tmp/pyplater_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplater_cli-0.0.1.tar", max compression
+gzip compressed data, was "pyplater_cli-1.0.0.tar", max compression
```

## Comparing `pyplater_cli-0.0.1.tar` & `pyplater_cli-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,46 @@
--rw-r--r--   0        0        0     1097 2023-07-14 00:38:13.436148 pyplater_cli-0.0.1/LICENSE.md
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.436148 pyplater_cli-0.0.1/pyplater_cli/__init__.py
--rw-r--r--   0        0        0     6627 2023-07-14 00:38:13.437148 pyplater_cli-0.0.1/pyplater_cli/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.437148 pyplater_cli-0.0.1/pyplater_cli/snippets/cython/cython/__init__.py
--rw-r--r--   0        0        0      144 2023-07-14 00:38:13.438150 pyplater_cli-0.0.1/pyplater_cli/snippets/cython/cython/loop.pyx
--rw-r--r--   0        0        0      347 2023-07-14 00:38:13.438150 pyplater_cli-0.0.1/pyplater_cli/snippets/cython/setup.py
--rw-r--r--   0        0        0      323 2023-07-14 00:38:13.438150 pyplater_cli-0.0.1/pyplater_cli/snippets/pip/pyproject.toml
--rw-r--r--   0        0        0       28 2023-07-14 00:38:13.439148 pyplater_cli-0.0.1/pyplater_cli/snippets/pip/requirements.dev.txt
--rw-r--r--   0        0        0       20 2023-07-14 00:38:13.439148 pyplater_cli-0.0.1/pyplater_cli/snippets/pip/requirements.txt
--rw-r--r--   0        0        0      667 2023-07-14 00:38:13.439148 pyplater_cli-0.0.1/pyplater_cli/snippets/poetry/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.440147 pyplater_cli-0.0.1/pyplater_cli/snippets/pytest/tests/__init__.py
--rw-r--r--   0        0        0      242 2023-07-14 00:38:13.440147 pyplater_cli-0.0.1/pyplater_cli/snippets/pytest/tests/test_project.py
--rw-r--r--   0        0        0      268 2023-07-14 00:38:13.440147 pyplater_cli-0.0.1/pyplater_cli/snippets/sqlalchemy/db/crud.py
--rw-r--r--   0        0        0      484 2023-07-14 00:38:13.441147 pyplater_cli-0.0.1/pyplater_cli/snippets/sqlalchemy/db/database.py
--rw-r--r--   0        0        0      845 2023-07-14 00:38:13.441147 pyplater_cli-0.0.1/pyplater_cli/snippets/sqlalchemy/db/model.py
--rw-r--r--   0        0        0      301 2023-07-14 00:38:13.441147 pyplater_cli-0.0.1/pyplater_cli/snippets/sqlalchemy/db/schema.py
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.442147 pyplater_cli-0.0.1/pyplater_cli/snippets/unittest/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-07-14 00:38:13.442147 pyplater_cli-0.0.1/pyplater_cli/snippets/unittest/tests/test_project.py
--rw-r--r--   0        0        0       43 2023-07-14 00:38:13.442147 pyplater_cli-0.0.1/pyplater_cli/templates/starter/cookiecutter.json
--rw-r--r--   0        0        0       31 2023-07-14 00:38:13.443147 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/.env.example
--rw-r--r--   0        0        0       76 2023-07-14 00:38:13.443147 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/.flake8
--rw-r--r--   0        0        0     1978 2023-07-14 00:38:13.443147 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     1021 2023-07-14 00:38:13.444146 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0     1173 2023-07-14 00:38:13.443147 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.444146 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      242 2023-07-14 00:38:13.444146 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/tests/test_project.py
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.445149 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
--rw-r--r--   0        0        0      184 2023-07-14 00:38:13.445149 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/config.py
--rw-r--r--   0        0        0      124 2023-07-14 00:38:13.445149 pyplater_cli-0.0.1/pyplater_cli/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
--rw-r--r--   0        0        0        0 2023-07-14 00:38:13.446149 pyplater_cli-0.0.1/pyplater_cli/tests/__init__.py
--rw-r--r--   0        0        0     4562 2023-07-14 00:38:13.446149 pyplater_cli-0.0.1/pyplater_cli/tests/test_cli.py
--rw-r--r--   0        0        0     2191 2023-07-14 00:38:13.447148 pyplater_cli-0.0.1/pyplater_cli/tests/test_questionary.py
--rw-r--r--   0        0        0     1225 2023-07-14 00:38:13.447148 pyplater_cli-0.0.1/pyplater_cli/tests/test_tree.py
--rw-r--r--   0        0        0     1037 2023-07-14 00:38:13.447148 pyplater_cli-0.0.1/pyplater_cli/utils/questionary.py
--rw-r--r--   0        0        0     2568 2023-07-14 00:38:13.448148 pyplater_cli-0.0.1/pyplater_cli/utils/tree.py
--rw-r--r--   0        0        0     1064 2023-07-14 00:39:25.277403 pyplater_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3320 2023-07-14 00:38:13.436148 pyplater_cli-0.0.1/README.md
--rw-r--r--   0        0        0     3940 1970-01-01 00:00:00.000000 pyplater_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     4156 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/__init__.py
+-rw-r--r--   0        0        0       55 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/base.py
+-rw-r--r--   0        0        0      942 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/delete.py
+-rw-r--r--   0        0        0     1249 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/edit.py
+-rw-r--r--   0        0        0     3402 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/git.py
+-rw-r--r--   0        0        0     1122 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/insert.py
+-rw-r--r--   0        0        0      864 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/save.py
+-rw-r--r--   0        0        0     1204 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/groups/view.py
+-rw-r--r--   0        0        0      905 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/main.py
+-rw-r--r--   0        0        0      258 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/snippets/sqlalchemy/db/crud.py
+-rw-r--r--   0        0        0      464 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/snippets/sqlalchemy/db/database.py
+-rw-r--r--   0        0        0      821 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/snippets/sqlalchemy/db/model.py
+-rw-r--r--   0        0        0      284 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/snippets/sqlalchemy/db/schema.py
+-rw-r--r--   0        0        0       40 2023-07-21 01:07:17.439460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/cookiecutter.json
+-rw-r--r--   0        0        0       31 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/.env.example
+-rw-r--r--   0        0        0       73 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/.flake8
+-rw-r--r--   0        0        0     1843 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     1115 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0      979 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/tests/test_project.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0      173 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/config.py
+-rw-r--r--   0        0        0      115 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_base.py
+-rw-r--r--   0        0        0     1046 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_delete.py
+-rw-r--r--   0        0        0      655 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_edit.py
+-rw-r--r--   0        0        0      773 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_git.py
+-rw-r--r--   0        0        0      833 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_insert.py
+-rw-r--r--   0        0        0     2130 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_questionary.py
+-rw-r--r--   0        0        0     1564 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_save.py
+-rw-r--r--   0        0        0     1214 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_tree.py
+-rw-r--r--   0        0        0     1004 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/tests/test_view.py
+-rw-r--r--   0        0        0       71 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2488 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/classes/DisplayPath.py
+-rw-r--r--   0        0        0     5332 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/classes/Git.py
+-rw-r--r--   0        0        0     1267 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/classes/Questionary.py
+-rw-r--r--   0        0        0      240 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/classes/__init__.py
+-rw-r--r--   0        0        0      394 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/constants.py
+-rw-r--r--   0        0        0     2451 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyplater_cli/utils/helpers.py
+-rw-r--r--   0        0        0     1085 2023-07-21 01:07:17.443460 pyplater_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 pyplater_cli-1.0.0/PKG-INFO
```

### Comparing `pyplater_cli-0.0.1/LICENSE.md` & `pyplater_cli-1.0.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 David Rose-Franklin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 David Rose-Franklin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyplater_cli-0.0.1/pyplater_cli/snippets/poetry/pyproject.toml` & `pyplater_cli-1.0.0/pyplater_cli/pyplater-templates/templates/starter/{{cookiecutter.project_slug}}/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,43 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry]
-name = "{{project_slug}}"
-version = "0.1.0"
-description = ""
-authors = ["Your Name <you@example.com>"]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pydantic-settings = "^2.0.1"
-
-[tool.poetry.group.dev.dependencies]
-flake8 = "6.0.0"
-black = "23.3.0"
-
-[build]
-include = ["script/**/*.py"]
-
-[pyplater.scripts]
-script = "poetry run python ./script/main.py"
-test = "poetry run python -m unittest discover tests"
-lint = "poetry run flake8"
-format = "poetry run black . -v"
-install = "poetry install"
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "{{cookiecutter.project_slug}}"
+version = "0.1.0"
+description = ""
+authors = ["Your Name <you@example.com>"]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+pydantic-settings = "^2.0.0"
+
+[tool.poetry.group.dev.dependencies]
+flake8 = "6.0.0"
+black = "23.3.0"
+pytest = "7.4.0"
+coverage = "7.2.7"
+
+[tool.poetry.scripts]
+script = "{{cookiecutter.project_slug}}.main:main"
+
+[build]
+include = ["{{cookiecutter.project_slug}}/**/*.py"]
+
+[tool.black]
+line-length = 88
+target-version = ['py38']
+include = '\.pyi?$'
+
+[flake8]
+max-line-length = 88
+
+[pyplater.scripts]
+script = "poetry run python run ./{{cookiecutter.project_slug}}/main.py"
+test = "poetry run pytest"
+lint = "poetry run flake8"
+coverage = "poetry run coverage run -m pytest"
+report = "poetry run coverage report"
+format = "poetry run black . -v"
+install = "poetry install"
 install-dev = "poetry install group -dev"
```

### Comparing `pyplater_cli-0.0.1/pyplater_cli/tests/test_questionary.py` & `pyplater_cli-1.0.0/pyplater_cli/tests/test_questionary.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from unittest.mock import MagicMock
-import click
-from pyplater.utils.questionary import (
-    QuestionaryInput,
-    QuestionaryConfirm,
-    QuestionaryOption,
-)
-
-
-def test_questionary_input_prompt_for_value(mocker):
-    mock_ctx = MagicMock()
-
-    mock_ask = MagicMock(return_value="Test")
-
-    mock_text = mocker.patch("questionary.text")
-    mock_text.return_value.ask = mock_ask
-
-    instance = QuestionaryInput(["--name"], prompt="What is your name?")
-
-    val = instance.prompt_for_value(mock_ctx)
-
-    assert val == "Test"
-
-    mock_text.assert_called_once_with("What is your name?")
-    mock_ask.assert_called_once()
-
-
-def test_questionary_confirm_prompt_for_value(mocker):
-    mock_ctx = MagicMock()
-
-    mock_ask = MagicMock(return_value=True)
-
-    mock_confirm = mocker.patch("questionary.confirm")
-    mock_confirm.return_value.ask = mock_ask
-
-    instance = QuestionaryConfirm(["--confirm"], prompt="Do you confirm?")
-
-    val = instance.prompt_for_value(mock_ctx)
-
-    assert val is True
-
-    mock_confirm.assert_called_once_with("Do you confirm?")
-    mock_ask.assert_called_once()
-
-
-def test_questionary_option_prompt_for_value(mocker):
-    # Create a mock context (ctx)
-    mock_ctx = MagicMock()
-
-    # Mock the 'unsafe_ask' method to return 'option1'
-    mock_unsafe_ask = MagicMock(return_value="option1")
-
-    # Mock the 'select' function
-    mock_select = mocker.patch("questionary.select")
-    # Make it so that calling select() and then unsafe_ask() returns 'option1'
-    mock_select.return_value.unsafe_ask = mock_unsafe_ask
-
-    # Create an instance of your class with the correct arguments
-    instance = QuestionaryOption(
-        ["--option"], type=click.Choice(["option1", "option2"]), prompt="an option"
-    )
-
-    # Call the method under test
-    val = instance.prompt_for_value(mock_ctx)
-
-    # Assert that the method returns the expected value
-    assert val == "option1"
-
-    # Assert that the mock was called with the correct argument
-    mock_select.assert_called_once_with(
-        "Choose an option:", choices=["option1", "option2"]
-    )
-    mock_unsafe_ask.assert_called_once()
+from unittest.mock import MagicMock
+import click
+from pyplater_cli.utils.classes.Questionary import (
+    QuestionaryInput,
+    QuestionaryConfirm,
+    QuestionaryOption,
+)
+
+
+def test_questionary_input_prompt_for_value(mocker):
+    mock_ctx = MagicMock()
+
+    mock_ask = MagicMock(return_value="Test")
+
+    mock_text = mocker.patch("questionary.text")
+    mock_text.return_value.ask = mock_ask
+
+    instance = QuestionaryInput(["--name"], prompt="What is your name?")
+
+    val = instance.prompt_for_value(mock_ctx)
+
+    assert val == "Test"
+
+    mock_text.assert_called_once_with("What is your name?")
+    mock_ask.assert_called_once()
+
+
+def test_questionary_confirm_prompt_for_value(mocker):
+    mock_ctx = MagicMock()
+
+    mock_ask = MagicMock(return_value=True)
+
+    mock_confirm = mocker.patch("questionary.confirm")
+    mock_confirm.return_value.ask = mock_ask
+
+    instance = QuestionaryConfirm(["--confirm"], prompt="Do you confirm?")
+
+    val = instance.prompt_for_value(mock_ctx)
+
+    assert val is True
+
+    mock_confirm.assert_called_once_with("Do you confirm?")
+    mock_ask.assert_called_once()
+
+
+def test_questionary_option_prompt_for_value(mocker):
+    # Create a mock context (ctx)
+    mock_ctx = MagicMock()
+
+    # Mock the 'unsafe_ask' method to return 'option1'
+    mock_unsafe_ask = MagicMock(return_value="option1")
+
+    # Mock the 'select' function
+    mock_select = mocker.patch("questionary.select")
+    # Make it so that calling select() and then unsafe_ask() returns 'option1'
+    mock_select.return_value.unsafe_ask = mock_unsafe_ask
+
+    # Create an instance of your class with the correct arguments
+    instance = QuestionaryOption(
+        ["--option"], type=click.Choice(["option1", "option2"]), prompt="an option"
+    )
+
+    # Call the method under test
+    val = instance.prompt_for_value(mock_ctx)
+
+    # Assert that the method returns the expected value
+    assert val == "option1"
+
+    # Assert that the mock was called with the correct argument
+    mock_select.assert_called_once_with(
+        "Choose an option:", choices=["option1", "option2"]
+    )
+    mock_unsafe_ask.assert_called_once()
```

### Comparing `pyplater_cli-0.0.1/pyplater_cli/tests/test_tree.py` & `pyplater_cli-1.0.0/pyplater_cli/tests/test_tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from pyplater.utils.tree import DisplayablePath
-from pathlib import Path
-from pyfakefs.fake_filesystem_unittest import TestCase
-
-
-class TestDisplayablePath(TestCase):
-    def setUp(self):
-        self.setUpPyfakefs()
-
-    def test_make_tree(self):
-        # Set up a fake filesystem
-        self.fs.create_dir("/root/dir1")
-        self.fs.create_file("/root/dir1/file1.txt")
-        self.fs.create_file("/root/dir1/file2.txt")
-        self.fs.create_dir("/root/dir2")
-        self.fs.create_file("/root/file3.txt")
-
-        # Test the make_tree class method
-        tree = list(DisplayablePath.make_tree(Path("/root")))
-        assert len(tree) == 6
-        assert tree[0].displayname == "root/"
-        assert tree[1].displayname == "dir1/"
-        assert tree[2].displayname == "file1.txt"
-        assert tree[3].displayname == "file2.txt"
-        assert tree[4].displayname == "dir2/"
-        assert tree[5].displayname == "file3.txt"
-        assert tree[2].displayable() == "│   ├── file1.txt"
-        assert tree[3].displayable() == "│   └── file2.txt"
-        assert tree[4].displayable() == "├── dir2/"
-        assert tree[5].displayable() == "└── file3.txt"
+from pyplater_cli.utils.classes.DisplayPath import DisplayablePath
+from pathlib import Path
+from pyfakefs.fake_filesystem_unittest import TestCase
+
+
+class TestDisplayablePath(TestCase):
+    def setUp(self):
+        self.setUpPyfakefs()
+
+    def test_make_tree(self):
+        # Set up a fake filesystem
+        self.fs.create_dir("/root/dir1")
+        self.fs.create_file("/root/dir1/file1.txt")
+        self.fs.create_file("/root/dir1/file2.txt")
+        self.fs.create_dir("/root/dir2")
+        self.fs.create_file("/root/file3.txt")
+
+        # Test the make_tree class method
+        tree = list(DisplayablePath.make_tree(Path("/root")))
+        assert len(tree) == 6
+        assert tree[0].displayname == "root/"
+        assert tree[1].displayname == "dir1/"
+        assert tree[2].displayname == "file1.txt"
+        assert tree[3].displayname == "file2.txt"
+        assert tree[4].displayname == "dir2/"
+        assert tree[5].displayname == "file3.txt"
+        assert tree[2].displayable() == "│   ├── file1.txt"
+        assert tree[3].displayable() == "│   └── file2.txt"
+        assert tree[4].displayable() == "├── dir2/"
+        assert tree[5].displayable() == "└── file3.txt"
```

### Comparing `pyplater_cli-0.0.1/pyplater_cli/utils/tree.py` & `pyplater_cli-1.0.0/pyplater_cli/utils/classes/DisplayPath.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from pathlib import Path
-
-
-class DisplayablePath(object):
-    display_filename_prefix_middle = "├──"
-    display_filename_prefix_last = "└──"
-    display_parent_prefix_middle = "    "
-    display_parent_prefix_last = "│   "
-
-    def __init__(self, path, parent_path, is_last):
-        self.path = Path(str(path))
-        self.parent = parent_path
-        self.is_last = is_last
-        if self.parent:
-            self.depth = self.parent.depth + 1
-        else:
-            self.depth = 0
-
-    @classmethod
-    def make_tree(cls, root, parent=None, is_last=False, criteria=None):
-        root = Path(str(root))
-        criteria = criteria or cls._default_criteria
-
-        displayable_root = cls(root, parent, is_last)
-        yield displayable_root
-
-        children = sorted(
-            list(path for path in root.iterdir() if criteria(path)),
-            key=lambda s: (not s.is_dir(), str(s).lower()),
-        )  # Sort directories first, then files
-        count = 1
-        for path in children:
-            is_last = count == len(children)
-            if path.is_dir():
-                yield from cls.make_tree(
-                    path, parent=displayable_root, is_last=is_last, criteria=criteria
-                )
-            else:
-                yield cls(path, displayable_root, is_last)
-            count += 1
-
-    @classmethod
-    def _default_criteria(cls, path):
-        return True
-
-    @property
-    def displayname(self):
-        if self.path.is_dir():
-            name = self.path.name
-            if name == "{{cookiecutter.project_slug}}":
-                name = "<project-name>"
-            return name + "/"
-        else:
-            name = self.path.name
-            if name == "{{cookiecutter.project_slug}}":
-                name = "<project-name>"
-            return name
-
-    def displayable(self):
-        if self.parent is None:
-            return self.displayname
-
-        _filename_prefix = (
-            self.display_filename_prefix_last
-            if self.is_last
-            else self.display_filename_prefix_middle
-        )
-
-        parts = ["{!s} {!s}".format(_filename_prefix, self.displayname)]
-
-        parent = self.parent
-        while parent and parent.parent is not None:
-            parts.append(
-                self.display_parent_prefix_middle
-                if parent.is_last
-                else self.display_parent_prefix_last
-            )
-            parent = parent.parent
-
-        return "".join(reversed(parts))
+from pathlib import Path
+
+
+class DisplayablePath(object):
+    display_filename_prefix_middle = "├──"
+    display_filename_prefix_last = "└──"
+    display_parent_prefix_middle = "    "
+    display_parent_prefix_last = "│   "
+
+    def __init__(self, path, parent_path, is_last):
+        self.path = Path(str(path))
+        self.parent = parent_path
+        self.is_last = is_last
+        if self.parent:
+            self.depth = self.parent.depth + 1
+        else:
+            self.depth = 0
+
+    @classmethod
+    def make_tree(cls, root, parent=None, is_last=False, criteria=None):
+        root = Path(str(root))
+        criteria = criteria or cls._default_criteria
+
+        displayable_root = cls(root, parent, is_last)
+        yield displayable_root
+
+        children = sorted(
+            list(path for path in root.iterdir() if criteria(path)),
+            key=lambda s: (not s.is_dir(), str(s).lower()),
+        )  # Sort directories first, then files
+        count = 1
+        for path in children:
+            is_last = count == len(children)
+            if path.is_dir():
+                yield from cls.make_tree(
+                    path, parent=displayable_root, is_last=is_last, criteria=criteria
+                )
+            else:
+                yield cls(path, displayable_root, is_last)
+            count += 1
+
+    @classmethod
+    def _default_criteria(cls, path):
+        return True
+
+    @property
+    def displayname(self):
+        if self.path.is_dir():
+            name = self.path.name
+            if name == "{{cookiecutter.project_slug}}":
+                name = "<project-name>"
+            return name + "/"
+        else:
+            name = self.path.name
+            if name == "{{cookiecutter.project_slug}}":
+                name = "<project-name>"
+            return name
+
+    def displayable(self):
+        if self.parent is None:
+            return self.displayname
+
+        _filename_prefix = (
+            self.display_filename_prefix_last
+            if self.is_last
+            else self.display_filename_prefix_middle
+        )
+
+        parts = ["{!s} {!s}".format(_filename_prefix, self.displayname)]
+
+        parent = self.parent
+        while parent and parent.parent is not None:
+            parts.append(
+                self.display_parent_prefix_middle
+                if parent.is_last
+                else self.display_parent_prefix_last
+            )
+            parent = parent.parent
+
+        return "".join(reversed(parts))
```

### Comparing `pyplater_cli-0.0.1/pyproject.toml` & `pyplater_cli-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry]
-name = "pyplater-cli"
-version = "0.0.1"
-description = "Create Python Script CLI"
-authors = ["David Rose-Franklin <david.rosefranklin96@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",  
-    "Programming Language :: Python :: 3.10",  
-    "Operating System :: Microsoft :: Windows",
-]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-click = "^8.0.3"
-questionary = "^1.10.0"
-cookiecutter = "^2.2.2"
-toml = "^0.10.2"
-
-[tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
-black = "^23.7.0"
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
-pytest-mock = "^3.11.1"
-pyfakefs = "^5.2.3"
-
-[tool.poetry.scripts]
-pyplater = 'pyplater_cli.cli:pyplater'
-
-[tool.black]
-line-length = 88
-include = '\.pyi?$'
-
-[tool.pytest.ini_options]
-addopts = "--ignore=pyplater/templates --ignore=pyplater/snippets"
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "pyplater-cli"
+version = "1.0.0"
+description = "Create Python Script CLI"
+authors = ["David Rose-Franklin <david.rosefranklin96@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",  
+    "Programming Language :: Python :: 3.10",  
+    "Operating System :: Microsoft :: Windows",
+]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+click = "^8.1.5"
+questionary = "^1.10.0"
+cookiecutter = "^2.2.3"
+toml = "^0.10.2"
+requests = "^2.31.0"
+
+[tool.poetry.group.dev.dependencies]
+flake8 = "^6.0.0"
+black = "^23.7.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.11.1"
+pyfakefs = "^5.2.3"
+
+[tool.poetry.scripts]
+pyplater = 'pyplater_cli.main:pyplater'
+
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+
+[tool.pytest.ini_options]
+addopts = "--ignore=pyplater/templates --ignore=pyplater/snippets"
+
+[pyplater.scripts]
+test = "echo 'test'"
```

