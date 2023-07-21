# Comparing `tmp/bowtie_json_schema-2023.7.8.tar.gz` & `tmp/bowtie_json_schema-2023.7.9.tar.gz`

## Comparing `bowtie_json_schema-2023.7.8.tar` & `bowtie_json_schema-2023.7.9.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.flake8
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.readthedocs.yml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/test-requirements.in
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/SECURITY.md
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/release.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/build-frontend.yml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/deploy-frontend.yml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/images.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/__main__.py
--rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/cli.rst
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/conf.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/contributing.rst
--rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/requirements.in
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/requirements.txt
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/docs/_static/dreamed.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/.eslintrc.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/index.html
--rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/package-lock.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/package.json
--rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/vite.config.js
--rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/public/favicon.ico
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/MainContainer.jsx
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/ReportDataHandler.jsx
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/ReportView.jsx
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/index.jsx
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/CopyToClipboard.jsx
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/LoadingAnimation.jsx
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/NavBar.jsx
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionItem.jsx
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionSvg.jsx
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/CasesSection.jsx
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Cases/SchemaDisplay.jsx
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.jsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Modals/DetailsButtonModal.jsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Modals/RunTimeInfoModal.jsx
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/RunInfo/RunInfoSection.jsx
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.jsx
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummarySection.jsx
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummaryTable.jsx
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/context/BowtieVersionContext.jsx
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/context/ThemeContext.jsx
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/pyproject.toml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.8/PKG-INFO
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.flake8
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/test-requirements.in
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/SECURITY.md
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/release.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/documentation-links.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/__main__.py
+-rw-r--r--   0        0        0    31626 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/cli.rst
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/contributing.rst
+-rw-r--r--   0        0        0    34138 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/requirements.in
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/requirements.txt
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/index.html
+-rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/package-lock.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/package.json
+-rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.7.9/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.7.8/.flake8` & `bowtie_json_schema-2023.7.9/.flake8`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.pre-commit-config.yaml` & `bowtie_json_schema-2023.7.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.9.0
     hooks:
       - id: pyupgrade
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
+    rev: "v0.0.278"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
     rev: v1.31.1
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
@@ -65,28 +65,28 @@
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: "3.0.0"
     hooks:
       - name: rubocop (ruby implementations)
         id: rubocop
         args: ["--auto-correct"]
   - repo: https://github.com/JohnnyMorganz/StyLua
-    rev: v0.18.0
+    rev: v0.18.1
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: v16.0.6
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.44.0
+    rev: v8.45.0
     hooks:
       - name: eslint
         id: eslint
         files: ^frontend/src/.*\.jsx?$
         types: [file]
         additional_dependencies:
           - eslint@8.43.0
```

### Comparing `bowtie_json_schema-2023.7.8/noxfile.py` & `bowtie_json_schema-2023.7.9/noxfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import ExitStack
+from functools import wraps
 from pathlib import Path
 from tempfile import TemporaryDirectory
 import os
 import shlex
 
 import nox
 
@@ -137,81 +138,91 @@
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
     session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
 
 
-@session(default=False, tags=["perf"], name="bench(info)")
-def bench_info(session):
+def benchmark(fn):
     """
-    Time how long ``bowtie info`` takes to run (effectively startup time).
+    A non-default noxenv to run a specific benchmark.
     """
-    session.install(ROOT)
-    executable = Path(session.bin) / "bowtie"
 
-    cmd = f"{executable} info -i {{implementation}}"
+    name = fn.__name__.removeprefix("bench_")
+
+    @session(default=False, tags=["perf"], name=f"bench({name})")
+    @wraps(fn)
+    def _benchmark(session):
+        session.install(ROOT)
+        bowtie = Path(session.bin) / "bowtie"
+        hyperfine_args, command = fn(session=session, bowtie=bowtie)
+        session.run("hyperfine", *hyperfine_args, command, external=True)
+
+    return _benchmark
+
 
+@benchmark
+def bench_info(session, bowtie):
+    """
+    Time how long ``bowtie info`` takes to run (effectively startup time).
+    """
     if session.posargs:
         args = session.posargs
     else:
         args = [
             "--warmup",
             "3",
             "-L",
             "implementation",
             ",".join(p.name for p in IMPLEMENTATIONS.iterdir() if p.is_dir()),
         ]
-
-    session.run("hyperfine", *args, cmd, external=True)
+    return args, f"{bowtie} info -i {{implementation}}"
 
 
-@session(default=False, tags=["perf"], name="bench(smoke)")
-def bench_smoke(session):
+@benchmark
+def bench_smoke(session, bowtie):
     """
     Time how long ``bowtie smoke`` takes to run (startup + ~2 simple examples).
     """
-    session.install(ROOT)
-    executable = Path(session.bin) / "bowtie"
-
-    cmd = f"{executable} smoke -i {{implementation}}"
-
     if session.posargs:
         args = session.posargs
     else:
         args = [
             "--warmup",
             "3",
             "-L",
             "implementation",
             ",".join(p.name for p in IMPLEMENTATIONS.iterdir() if p.is_dir()),
         ]
+    return args, f"{bowtie} smoke -i {{implementation}}"
 
-    session.run("hyperfine", *args, cmd, external=True)
 
-
-@session(default=False, tags=["perf"], name="bench(suite)")
-def bench_suite(session):
+@benchmark
+def bench_suite(session, bowtie):
+    """
+    Time how long ``bowtie suite`` takes to run a version of the test suite.
+    """
     if not session.posargs:
         session.error("Provide a test suite to benchmark")
 
-    session.install(ROOT)
-    bowtie = Path(session.bin) / "bowtie"
-
     posargs = shlex.join(session.posargs)
     if "-i" not in session.posargs:
         args = [
+            "--warmup",
+            "1",
+            # because not all implementations will likely support the dialect
+            "--ignore-failure",
             "-L",
             "implementation",
             ",".join(p.name for p in IMPLEMENTATIONS.iterdir() if p.is_dir()),
-            f"{bowtie} suite -i {{implementation}} {posargs}",
         ]
+        command = f"{bowtie} suite -i {{implementation}} {posargs}"
     else:
-        args = [f"{bowtie} suite {posargs}"]
-    session.run("hyperfine", "--warmup", "1", *args, external=True)
+        args, command = [], f"{bowtie} suite {posargs}"
+    return args, command
 
 
 @session(default=False)
 def requirements(session):
     session.install("pip-tools")
     for each in [DOCS / "requirements.in", ROOT / "test-requirements.in"]:
         session.run(
```

### Comparing `bowtie_json_schema-2023.7.8/test-requirements.txt` & `bowtie_json_schema-2023.7.9/test-requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --resolver=backtracking test-requirements.in
+#    pip-compile test-requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
 aiohttp==3.8.4
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
 attrs==23.1.0
     # via
     #   aiohttp
     #   bowtie-json-schema
     #   jsonschema
+    #   referencing
 file:.#egg=bowtie-json-schema
     # via -r test-requirements.in
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via
     #   aiohttp
     #   requests
-click==8.1.3
+click==8.1.5
     # via
     #   bowtie-json-schema
     #   trogon
-cryptography==41.0.1
+cryptography==41.0.2
     # via pyjwt
-frozenlist==1.3.3
+frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema
 icdiff==2.0.6
     # via pytest-icdiff
 idna==3.4
     # via
     #   requests
     #   yarl
-importlib-metadata==6.6.0
+importlib-metadata==6.8.0
     # via textual
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via bowtie-json-schema
-jsonschema==4.17.3
+jsonschema==4.18.3
     # via bowtie-json-schema
+jsonschema-specifications==2023.6.1
+    # via jsonschema
 linkify-it-py==2.0.2
     # via markdown-it-py
-markdown-it-py[linkify,plugins]==2.2.0
+markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.3
     # via jinja2
 mdit-py-plugins==0.4.0
@@ -68,58 +71,64 @@
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 packaging==23.1
     # via pytest
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 pprintpp==0.4.0
     # via pytest-icdiff
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via rich
 pyjwt[crypto]==2.7.0
     # via github3-py
-pyrsistent==0.19.3
-    # via jsonschema
-pytest==7.3.1
+pytest==7.4.0
     # via
     #   -r test-requirements.in
     #   pytest-asyncio
     #   pytest-icdiff
-pytest-asyncio==0.21.0
+pytest-asyncio==0.21.1
     # via -r test-requirements.in
 pytest-icdiff==0.6
     # via -r test-requirements.in
 python-dateutil==2.8.2
     # via github3-py
+referencing==0.29.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via github3-py
-rich==13.4.1
+rich==13.4.2
     # via
     #   bowtie-json-schema
     #   textual
+rpds-py==0.8.11
+    # via
+    #   jsonschema
+    #   referencing
 six==1.16.0
     # via python-dateutil
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.27.0
+textual==0.29.0
     # via trogon
-trogon==0.4.0
+trogon==0.5.0
     # via bowtie-json-schema
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 yarl==1.9.2
     # via aiohttp
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.7.8/.github/SECURITY.md` & `bowtie_json_schema-2023.7.9/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/dependabot.yml` & `bowtie_json_schema-2023.7.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/build-frontend.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/build-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/ci.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/deploy-frontend.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/deploy-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/images.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/images.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.github/workflows/report.yml` & `bowtie_json_schema-2023.7.9/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/_cli.py` & `bowtie_json_schema-2023.7.9/bowtie/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     NoSuchImage,
     StartupFailed,
 )
 from bowtie.exceptions import (
     _ProtocolError,  # type: ignore[reportPrivateUsage]
 )
 
+_EX_CONFIG = getattr(os, "EX_CONFIG", 1)
+
 IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
 TEST_SUITE_URL = "https://github.com/json-schema-org/json-schema-test-suite"
 
 DRAFT2020 = "https://json-schema.org/draft/2020-12/schema"
 DRAFT2019 = "https://json-schema.org/draft/2019-09/schema"
 DRAFT7 = "http://json-schema.org/draft-07/schema#"
 DRAFT6 = "http://json-schema.org/draft-06/schema#"
@@ -473,22 +475,22 @@
         make_validator=validator_for_dialect,
         reporter=_report.Reporter(),
     ) as starting:
         for each in asyncio.as_completed(starting):
             try:
                 implementation = await each
             except NoSuchImage as error:
-                exit_code |= os.EX_CONFIG
+                exit_code |= _EX_CONFIG
                 click.echo(
                     f"❗ (error): {error.name!r} is not a known Bowtie implementation.",  # noqa: E501
                 )
                 continue
 
             if implementation.metadata is None:
-                exit_code |= os.EX_CONFIG
+                exit_code |= _EX_CONFIG
                 click.echo("  ❗ (error): startup failed")
                 continue
 
             metadata = {
                 k: v
                 for k, v in sorted(
                     implementation.metadata.items(),
@@ -534,25 +536,25 @@
         make_validator=validator_for_dialect,
         reporter=_report.Reporter(),
     ) as starting:
         for each in asyncio.as_completed(starting):
             try:
                 implementation = await each
             except NoSuchImage as error:
-                exit_code |= os.EX_CONFIG
+                exit_code |= _EX_CONFIG
                 click.echo(
                     f"❗ (error): {error.name!r} is not a known Bowtie implementation.",  # noqa: E501
                     file=sys.stderr,
                 )
                 continue
 
             click.echo(f"Testing {implementation.name!r}...", file=sys.stderr)
 
             if implementation.metadata is None:
-                exit_code |= os.EX_CONFIG
+                exit_code |= _EX_CONFIG
                 click.echo("  ❗ (error): startup failed", file=sys.stderr)
                 continue
 
             dialect = implementation.dialects[0]
             runner = await implementation.start_speaking(dialect)
 
             cases = [
@@ -742,47 +744,47 @@
         **kwargs,
     ) as starting:
         reporter.will_speak(dialect=dialect)
         for each in asyncio.as_completed(starting):
             try:
                 implementation = await each
             except StartupFailed as error:
-                exit_code = os.EX_CONFIG
+                exit_code = _EX_CONFIG
                 reporter.startup_failed(name=error.name, stderr=error.stderr)
                 continue
             except NoSuchImage as error:
-                exit_code = os.EX_CONFIG
+                exit_code = _EX_CONFIG
                 reporter.no_such_image(name=error.name)
                 continue
 
             try:
                 if dialect in implementation.dialects:
                     try:
                         runner = await implementation.start_speaking(dialect)
                     except GotStderr as error:
-                        exit_code = os.EX_CONFIG
+                        exit_code = _EX_CONFIG
                         reporter.dialect_error(
                             implementation=implementation,
                             stderr=error.stderr.decode(),
                         )
                     else:
                         runner.warn_if_unacknowledged(reporter=reporter)
                         acknowledged.append(implementation)
                         runners.append(runner)
                 else:
                     reporter.unsupported_dialect(
                         implementation=implementation,
                         dialect=dialect,
                     )
             except StartupFailed as error:
-                exit_code = os.EX_CONFIG
+                exit_code = _EX_CONFIG
                 reporter.startup_failed(name=error.name, stderr=error.stderr)
 
         if not runners:
-            exit_code = os.EX_CONFIG
+            exit_code = _EX_CONFIG
             reporter.no_implementations()
         else:
             reporter.ready(
                 _report.RunInfo.from_implementations(
                     implementations=acknowledged,
                     dialect=dialect,
                     metadata=run_metadata,
```

### Comparing `bowtie_json_schema-2023.7.8/bowtie/_commands.py` & `bowtie_json_schema-2023.7.9/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/_core.py` & `bowtie_json_schema-2023.7.9/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/_report.py` & `bowtie_json_schema-2023.7.9/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/exceptions.py` & `bowtie_json_schema-2023.7.9/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/Makefile` & `bowtie_json_schema-2023.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/cli.rst` & `bowtie_json_schema-2023.7.9/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/conf.py` & `bowtie_json_schema-2023.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/contributing.rst` & `bowtie_json_schema-2023.7.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/implementers.rst` & `bowtie_json_schema-2023.7.9/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/index.rst` & `bowtie_json_schema-2023.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/docs/requirements.txt` & `bowtie_json_schema-2023.7.9/docs/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --resolver=backtracking docs/requirements.in
+#    pip-compile --config=pyproject.toml docs/requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
 aiohttp==3.8.4
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
@@ -15,99 +15,102 @@
 async-timeout==4.0.2
     # via aiohttp
 attrs==23.1.0
     # via
     #   aiohttp
     #   bowtie-json-schema
     #   jsonschema
+    #   referencing
 babel==2.12.1
     # via sphinx
 beautifulsoup4==4.12.2
     # via furo
 file:.#egg=bowtie-json-schema
     # via -r docs/requirements.in
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via
     #   aiohttp
     #   requests
-click==8.1.3
+click==8.1.5
     # via
     #   bowtie-json-schema
     #   sphinx-click
     #   trogon
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.1
+cryptography==41.0.2
     # via pyjwt
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-click
-fonttools==4.39.4
+fonttools==4.41.0
     # via matplotlib
-frozenlist==1.3.3
+frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 furo==2023.5.20
     # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
 idna==3.4
     # via
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.6.0
+importlib-metadata==6.8.0
     # via textual
 jinja2==3.1.2
     # via
     #   bowtie-json-schema
     #   sphinx
-jsonschema==4.17.3
+jsonschema==4.18.3
     # via bowtie-json-schema
+jsonschema-specifications==2023.6.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 linkify-it-py==2.0.2
     # via markdown-it-py
-lxml==4.9.2
+lxml==4.9.3
     # via sphinx-json-schema-spec
-markdown-it-py[linkify,plugins]==2.2.0
+markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 markupsafe==2.1.3
     # via jinja2
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via sphinxext-opengraph
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-numpy==1.24.3
+numpy==1.25.1
     # via
     #   contourpy
     #   matplotlib
 packaging==23.1
     # via
     #   matplotlib
     #   sphinx
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pycparser==2.21
     # via cffi
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
 pygments==2.15.1
     # via
@@ -117,28 +120,34 @@
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
 pyjwt[crypto]==2.7.0
     # via github3-py
 pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   github3-py
     #   matplotlib
+referencing==0.29.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   github3-py
     #   sphinx
-rich==13.4.1
+rich==13.4.2
     # via
     #   bowtie-json-schema
     #   textual
+rpds-py==0.8.11
+    # via
+    #   jsonschema
+    #   referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==7.0.1
@@ -147,15 +156,15 @@
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
-sphinx-basic-ng==1.0.0b1
+sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==4.4.0
     # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
 sphinx-json-schema-spec==2023.5.3
     # via -r docs/requirements.in
@@ -173,27 +182,27 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.27.0
+textual==0.29.0
     # via trogon
-trogon==0.4.0
+trogon==0.5.0
     # via bowtie-json-schema
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 uritemplate==4.1.1
     # via github3-py
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 yarl==1.9.2
     # via
     #   -r docs/requirements.in
     #   aiohttp
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
```

### Comparing `bowtie_json_schema-2023.7.8/docs/_static/dreamed.png` & `bowtie_json_schema-2023.7.9/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/package-lock.json` & `bowtie_json_schema-2023.7.9/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/package.json` & `bowtie_json_schema-2023.7.9/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2023.7.9/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/public/favicon.ico` & `bowtie_json_schema-2023.7.9/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/ReportDataHandler.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/ReportDataHandler.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/index.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/index.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/CopyToClipboard.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/CopyToClipboard.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/LoadingAnimation.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/LoadingAnimation.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/NavBar.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/NavBar.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionItem.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionItem.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/AccordionSvg.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/AccordionSvg.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/CasesSection.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/CasesSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Cases/SchemaDisplay.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Cases/SchemaDisplay.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/DragAndDrop/DragAndDrop.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/DragAndDrop/DragAndDrop.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Modals/DetailsButtonModal.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Modals/DetailsButtonModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Modals/RunTimeInfoModal.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Modals/RunTimeInfoModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/RunInfo/RunInfoSection.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/RunInfo/RunInfoSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/ImplementationRow.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/ImplementationRow.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummarySection.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummarySection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/components/Summary/SummaryTable.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/components/Summary/SummaryTable.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/context/ThemeContext.jsx` & `bowtie_json_schema-2023.7.9/frontend/src/context/ThemeContext.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2023.7.9/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/tests/test_integration.py` & `bowtie_json_schema-2023.7.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.7.9/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.7.9/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.7.9/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.7.9/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.7.9/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/.gitignore` & `bowtie_json_schema-2023.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/LICENSE` & `bowtie_json_schema-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/README.rst` & `bowtie_json_schema-2023.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/pyproject.toml` & `bowtie_json_schema-2023.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.7.8/PKG-INFO` & `bowtie_json_schema-2023.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.7.8
+Version: 2023.7.9
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

