# Comparing `tmp/junifer-0.0.3.dev75.tar.gz` & `tmp/junifer-0.0.3.dev89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.3.dev75.tar", last modified: Tue Jun 20 10:30:03 2023, max compression
+gzip compressed data, was "junifer-0.0.3.dev89.tar", last modified: Wed Jun 21 09:41:29 2023, max compression
```

## Comparing `junifer-0.0.3.dev75.tar` & `junifer-0.0.3.dev89.tar`

### file list

```diff
@@ -1,375 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.396937 junifer-0.0.3.dev75/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.396937 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.396937 junifer-0.0.3.dev75/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.384937 junifer-0.0.3.dev75/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.400938 junifer-0.0.3.dev75/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.404938 junifer-0.0.3.dev75/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/220.doc
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/222.change
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/222.enh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/223.bugfix
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/223.enh
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/226.enh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/227.enh
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/228.misc
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/changes/newsfragments/230.misc
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.404938 junifer-0.0.3.dev75/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.404938 junifer-0.0.3.dev75/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.404938 junifer-0.0.3.dev75/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.404938 junifer-0.0.3.dev75/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.408938 junifer-0.0.3.dev75/docs/using/
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.408938 junifer-0.0.3.dev75/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.408938 junifer-0.0.3.dev75/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.408938 junifer-0.0.3.dev75/junifer/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24652 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.412938 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.416938 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.416938 junifer-0.0.3.dev75/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.388937 junifer-0.0.3.dev75/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.388937 junifer-0.0.3.dev75/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.420939 junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/datalad_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.388937 junifer-0.0.3.dev75/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 10:29:49.000000 junifer-0.0.3.dev75/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-06-20 10:29:49.000000 junifer-0.0.3.dev75/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 10:29:49.000000 junifer-0.0.3.dev75/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-20 10:29:49.000000 junifer-0.0.3.dev75/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-20 10:29:49.000000 junifer-0.0.3.dev75/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.424939 junifer-0.0.3.dev75/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.428939 junifer-0.0.3.dev75/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.428939 junifer-0.0.3.dev75/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.428939 junifer-0.0.3.dev75/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.428939 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.428939 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.432939 junifer-0.0.3.dev75/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.436939 junifer-0.0.3.dev75/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.408938 junifer-0.0.3.dev75/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:30:03.000000 junifer-0.0.3.dev75/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:30:03.440940 junifer-0.0.3.dev75/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 10:29:48.000000 junifer-0.0.3.dev75/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.589001 junifer-0.0.3.dev89/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.589001 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.589001 junifer-0.0.3.dev89/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.581001 junifer-0.0.3.dev89/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.593001 junifer-0.0.3.dev89/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/220.doc
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/222.change
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/222.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/223.bugfix
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/223.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/226.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/227.enh
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/228.misc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/229.misc
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/changes/newsfragments/230.misc
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.597001 junifer-0.0.3.dev89/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24632 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.605001 junifer-0.0.3.dev89/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.605001 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.605001 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.605001 junifer-0.0.3.dev89/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.585001 junifer-0.0.3.dev89/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.585001 junifer-0.0.3.dev89/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27444 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/datalad_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.609001 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.585001 junifer-0.0.3.dev89/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.613001 junifer-0.0.3.dev89/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.617001 junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21922 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.621001 junifer-0.0.3.dev89/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28543 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.601001 junifer-0.0.3.dev89/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 09:41:29.000000 junifer-0.0.3.dev89/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:41:29.625001 junifer-0.0.3.dev89/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-21 09:41:19.000000 junifer-0.0.3.dev89/tox.ini
```

### Comparing `junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.3.dev89/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/workflows/ci-docs.yml` & `junifer-0.0.3.dev89/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/workflows/ci.yml` & `junifer-0.0.3.dev89/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/workflows/docs-preview.yml` & `junifer-0.0.3.dev89/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/workflows/docs.yml` & `junifer-0.0.3.dev89/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.github/workflows/pypi.yml` & `junifer-0.0.3.dev89/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/.gitignore` & `junifer-0.0.3.dev89/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/LICENSE.md` & `junifer-0.0.3.dev89/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/PKG-INFO` & `junifer-0.0.3.dev89/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev75
+Version: 0.0.3.dev89
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -36,14 +36,15 @@
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.3.dev75/README.md` & `junifer-0.0.3.dev89/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.3.dev75/codecov.yml` & `junifer-0.0.3.dev89/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/conda-env.yml` & `junifer-0.0.3.dev89/conda-env.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,16 @@
   - furo>=2022.9.29,<2023.0.0
   - numpydoc=1.5.*
   - sphinx-copybutton=0.5.*
   - towncrier=22.12.*
   - sphinxcontrib-mermaid=0.8.*
   - tox
   - ipykernel
-  - isort
   - pytest-cov
   - pytest
   - black
-  - flake8
-  - flake8-docstrings
-  - flake8-bugbear
+  - ruff
   - codespell
   - pip
   - pip:
     - datalad>=0.15.4,<0.19
     - julearn==0.2.5
```

### Comparing `junifer-0.0.3.dev75/docs/Makefile` & `junifer-0.0.3.dev89/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/_static/css/custom.css` & `junifer-0.0.3.dev89/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/_templates/versions.html` & `junifer-0.0.3.dev89/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/builtin.rst` & `junifer-0.0.3.dev89/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/changes/contributors.inc` & `junifer-0.0.3.dev89/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/conf.py` & `junifer-0.0.3.dev89/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "sklearn": ("https://scikit-learn.org/stable", None),
     "nilearn": ("https://nilearn.github.io/stable/", None),
     "julearn": ("https://juaml.github.io/julearn/main", None),
     "nibabel": ("https://nipy.org/nibabel/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
-    "numpy": ("https://numpy.org/doc/stable/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/dev", None),
     # "sqlalchemy": ("https://docs.sqlalchemy.org/en/20/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
 }
 
 # -- numpydoc configuration --------------------------------------------------
```

### Comparing `junifer-0.0.3.dev75/docs/contribution.rst` & `junifer-0.0.3.dev89/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/coordinates.rst` & `junifer-0.0.3.dev89/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/datagrabber.rst` & `junifer-0.0.3.dev89/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/extension.rst` & `junifer-0.0.3.dev89/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/index.rst` & `junifer-0.0.3.dev89/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/marker.rst` & `junifer-0.0.3.dev89/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/masks.rst` & `junifer-0.0.3.dev89/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/extending/parcellations.rst` & `junifer-0.0.3.dev89/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/faq.rst` & `junifer-0.0.3.dev89/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/help.rst` & `junifer-0.0.3.dev89/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/images/junifer_logo.png` & `junifer-0.0.3.dev89/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/index.rst` & `junifer-0.0.3.dev89/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/installation.rst` & `junifer-0.0.3.dev89/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/links.inc` & `junifer-0.0.3.dev89/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/maintaining.rst` & `junifer-0.0.3.dev89/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.3.dev89/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/starting.rst` & `junifer-0.0.3.dev89/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/data.rst` & `junifer-0.0.3.dev89/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/datagrabber.rst` & `junifer-0.0.3.dev89/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/datareader.rst` & `junifer-0.0.3.dev89/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/index.rst` & `junifer-0.0.3.dev89/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/marker.rst` & `junifer-0.0.3.dev89/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/pipeline.rst` & `junifer-0.0.3.dev89/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/preprocess.rst` & `junifer-0.0.3.dev89/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/understanding/storage.rst` & `junifer-0.0.3.dev89/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/using/codeless.rst` & `junifer-0.0.3.dev89/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/using/index.rst` & `junifer-0.0.3.dev89/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/using/masks.rst` & `junifer-0.0.3.dev89/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/using/queueing.rst` & `junifer-0.0.3.dev89/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/using/running.rst` & `junifer-0.0.3.dev89/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/docs/whats_new.rst` & `junifer-0.0.3.dev89/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/norun_hcpfc_pearson.py` & `junifer-0.0.3.dev89/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/norun_ukbvm_gmd.py` & `junifer-0.0.3.dev89/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/run_compute_parcel_mean.py` & `junifer-0.0.3.dev89/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.3.dev89/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/run_ets_rss_marker.py` & `junifer-0.0.3.dev89/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/run_junifer_julearn.py` & `junifer-0.0.3.dev89/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/run_run_gmd_mean.py` & `junifer-0.0.3.dev89/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/yamls/gmd_mean.yaml` & `junifer-0.0.3.dev89/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.3.dev89/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/api/cli.py` & `junifer-0.0.3.dev89/junifer/api/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     "--verbose",
     type=click.UNPROCESSED,
     callback=_validate_verbose,
     default="info",
 )
 def run(filepath: click.Path, element: str, verbose: Union[str, int]) -> None:
     """Run command for CLI.
+
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
     element : str
         The element to operate using.
@@ -178,14 +179,15 @@
     "--verbose",
     type=click.UNPROCESSED,
     callback=_validate_verbose,
     default="info",
 )
 def collect(filepath: click.Path, verbose: Union[str, int]) -> None:
     """Collect command for CLI.
+
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
     verbose : click.Choice
         The verbosity level: warning, info or debug (default "info").
@@ -220,14 +222,15 @@
     filepath: click.Path,
     element: str,
     overwrite: bool,
     submit: bool,
     verbose: Union[str, int],
 ) -> None:
     """Queue command for CLI.
+
     \f
     Parameters
     ----------
     filepath : click.Path
         The filepath to the configuration file.
     element : str
         The element to operate using.
@@ -257,14 +260,15 @@
     )
 
 
 @cli.command()
 @click.option("--long", "long_", is_flag=True)
 def wtf(long_: bool) -> None:
     """Wtf command for CLI.
+
     \f
     Parameters
     ----------
     long_ : bool
         Whether to report long version or not.
 
     """
@@ -278,14 +282,15 @@
     click.echo(yaml.dump(report, stream=sys.stdout))
 
 
 @cli.command()
 @click.argument("subpkg", type=str)
 def selftest(subpkg: str) -> None:
     """Selftest command for CLI.
+
     \f
     Parameters
     ----------
     subpkg : {"all", "api", "configs", "data", "datagrabber", "datareader",
         "markers", "pipeline", "preprocess", "storage", "testing", "utils",
         "stats"}
         The sub-package to run tests for.
```

### Comparing `junifer-0.0.3.dev75/junifer/api/decorators.py` & `junifer-0.0.3.dev89/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/api/functions.py` & `junifer-0.0.3.dev89/junifer/api/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,27 +230,27 @@
     ValueError
         If the value of ``kind`` is invalid.
 
     """
     # Create a folder within the CWD to store the job files / config
     cwd = Path.cwd()
     jobdir = cwd / "junifer_jobs" / jobname
-    logger.info(f"Creating job in {str(jobdir.absolute())}")
+    logger.info(f"Creating job in {jobdir.absolute()!s}")
     if jobdir.exists():
         if not overwrite:
             raise_error(
                 f"Job folder for {jobname} already exists. "
                 "This error is raised to prevent overwriting job files "
                 "that might be scheduled but not yet executed. "
-                f"Either delete the directory {str(jobdir.absolute())} "
+                f"Either delete the directory {jobdir.absolute()!s} "
                 "or set overwrite=True."
             )
         else:
             logger.info(
-                f"Deleting existing job directory at {str(jobdir.absolute())}"
+                f"Deleting existing job directory at {jobdir.absolute()!s}"
             )
             shutil.rmtree(jobdir)
     jobdir.mkdir(exist_ok=True, parents=True)
 
     if "with" in config:
         to_load = config["with"]
         # If there is a list of files to load, copy and remove the path
@@ -264,15 +264,15 @@
                 shutil.copy(item, jobdir)
                 fixed_load.append(Path(item).name)
             else:
                 fixed_load.append(item)
         config["with"] = fixed_load
 
     yaml_config = jobdir / "config.yaml"
-    logger.info(f"Writing YAML config to {str(yaml_config.absolute())}")
+    logger.info(f"Writing YAML config to {yaml_config.absolute()!s}")
     yaml.dump(config, stream=yaml_config)
 
     # Get list of elements
     if elements is None:
         if "elements" in config:
             elements = config["elements"]
         else:
@@ -374,19 +374,19 @@
     ------
     ValueError
         If the value of `env` is invalid.
 
     """
     logger.debug("Creating HTCondor job")
     run_junifer_args = (
-        f"run {str(yaml_config.absolute())} "
+        f"run {yaml_config.absolute()!s} "
         f"--verbose {verbose} --element $(element)"
     )
     collect_junifer_args = (
-        f"collect {str(yaml_config.absolute())} --verbose {verbose} "
+        f"collect {yaml_config.absolute()!s} --verbose {verbose} "
     )
 
     if not isinstance(collect, str):
         raise_error("collect must be a string")
 
     collect = collect.lower()
     if collect not in ["yes", "no", "on_success_only"]:
@@ -397,15 +397,15 @@
     if env is None:
         env = {"kind": "local"}
     if env["kind"] == "conda":
         env_name = env["name"]
         executable = "run_conda.sh"
         arguments = f"{env_name} junifer"
         exec_path = jobdir / executable
-        logger.info(f"Copying {executable} to {str(exec_path.absolute())}")
+        logger.info(f"Copying {executable} to {exec_path.absolute()!s}")
         shutil.copy(Path(__file__).parent / "res" / executable, exec_path)
         make_executable(exec_path)
     elif env["kind"] == "venv":
         env_name = env["name"]
         executable = "run_venv.sh"
         arguments = f"{env_name} junifer"
         # TODO: Copy run_venv.sh to jobdir
@@ -437,26 +437,26 @@
 
         # Resources
         request_cpus = {cpus}
         request_memory = {mem}
         request_disk = {disk}
 
         # Executable
-        initial_dir = {str(jobdir.absolute())}
+        initial_dir = {jobdir.absolute()!s}
         executable = $(initial_dir)/{executable}
         transfer_executable = False
 
         arguments = {arguments} {run_junifer_args}
 
         {extra_preamble}
 
         # Logs
-        log = {str(log_dir.absolute())}/junifer_run_$(log_element).log
-        output = {str(log_dir.absolute())}/junifer_run_$(log_element).out
-        error = {str(log_dir.absolute())}/junifer_run_$(log_element).err
+        log = {log_dir.absolute()!s}/junifer_run_$(log_element).log
+        output = {log_dir.absolute()!s}/junifer_run_$(log_element).out
+        error = {log_dir.absolute()!s}/junifer_run_$(log_element).err
         """
 
     submit_run_fname = jobdir / f"run_{jobname}.submit"
     submit_collect_fname = jobdir / f"collect_{jobname}.submit"
     dag_fname = jobdir / f"{jobname}.dag"
 
     # Write to run submit files
@@ -471,26 +471,26 @@
 
         # Resources
         request_cpus = {cpus}
         request_memory = {mem}
         request_disk = {disk}
 
         # Executable
-        initial_dir = {str(jobdir.absolute())}
+        initial_dir = {jobdir.absolute()!s}
         executable = $(initial_dir)/{executable}
         transfer_executable = False
 
         arguments = {arguments} {collect_junifer_args}
 
         {extra_preamble}
 
         # Logs
-        log = {str(log_dir.absolute())}/junifer_collect.log
-        output = {str(log_dir.absolute())}/junifer_collect.out
-        error = {str(log_dir.absolute())}/junifer_collect.err
+        log = {log_dir.absolute()!s}/junifer_collect.log
+        output = {log_dir.absolute()!s}/junifer_collect.out
+        error = {log_dir.absolute()!s}/junifer_collect.err
         """
 
     # Now create the collect submit file
     with open(submit_collect_fname, "w") as submit_file:
         submit_file.write(textwrap.dedent(collect_preamble))
         submit_file.write("queue\n")
 
@@ -531,15 +531,15 @@
 
     # Submit job(s)
     if submit is True:
         logger.info("Submitting HTCondor job")
         subprocess.run(["condor_submit_dag", dag_fname])
         logger.info("HTCondor job submitted")
     else:
-        cmd = f"condor_submit_dag {str(dag_fname.absolute())}"
+        cmd = f"condor_submit_dag {dag_fname.absolute()!s}"
         logger.info(
             f"HTCondor job files created, to submit the job, run `{cmd}`"
         )
 
 
 def _queue_slurm(
     jobname: str,
```

### Comparing `junifer-0.0.3.dev75/junifer/api/parser.py` & `junifer-0.0.3.dev89/junifer/api/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         The contents represented as dictionary.
 
     """
     # Convert str to Path
     if not isinstance(filepath, Path):
         filepath = Path(filepath)
 
-    logger.info(f"Parsing yaml file: {str(filepath.absolute())}")
+    logger.info(f"Parsing yaml file: {filepath.absolute()!s}")
     # Filepath existence check
     if not filepath.exists():
-        raise_error(f"File does not exist: {str(filepath.absolute())}")
+        raise_error(f"File does not exist: {filepath.absolute()!s}")
     # Filepath reading
     contents = yaml.load(filepath)
     if "elements" in contents:
         if contents["elements"] is None:
             raise_error(
                 "The elements key was defined but its content is empty. "
                 "Please define the elements to operate on or remove the key."
```

### Comparing `junifer-0.0.3.dev75/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.3.dev89/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/api/tests/test_api_utils.py` & `junifer-0.0.3.dev89/junifer/api/tests/test_api_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,30 @@
     assert python_information["version"] == pl.python_version()
     assert python_information["implementation"] == pl.python_implementation()
 
 
 def test_get_dependency_information_short() -> None:
     """Test short version of _get_dependency_information()."""
     dependency_information = _get_dependency_information(long_=False)
-    assert [key for key in dependency_information.keys()] == [
+    assert list(dependency_information.keys()) == [
         "click",
         "numpy",
         "datalad",
         "pandas",
         "nibabel",
         "nilearn",
         "sqlalchemy",
         "ruamel.yaml",
     ]
 
 
 def test_get_dependency_information_long() -> None:
     """Test long version of _get_dependency_information()."""
     dependency_information = _get_dependency_information(long_=True)
-    dependency_information_keys = [
-        key for key in dependency_information.keys()
-    ]
+    dependency_information_keys = list(dependency_information.keys())
     for key in [
         "click",
         "numpy",
         "datalad",
         "pandas",
         "nibabel",
         "nilearn",
```

### Comparing `junifer-0.0.3.dev75/junifer/api/tests/test_cli.py` & `junifer-0.0.3.dev89/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/api/tests/test_functions.py` & `junifer-0.0.3.dev89/junifer/api/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 
             run_submit_file_path = Path(
                 tmp_path / "junifer_jobs" / jobname / f"run_{jobname}.submit"
             )
             # Check junifer run submit file
             assert run_submit_file_path.is_file()
             # Read run submit file to check if resources are correct
-            with open(run_submit_file_path, "r") as f:
+            with open(run_submit_file_path) as f:
                 for line in f.read().splitlines():
                     if "request_cpus" in line:
                         assert int(line.split("=")[1].strip()) == cpus
                     if "request_memory" in line:
                         assert line.split("=")[1].strip() == mem
                     if "request_disk" in line:
                         assert line.split("=")[1].strip() == disk
@@ -740,15 +740,15 @@
             )
             # Check junifer dag file
             assert dag_file_path.is_file()
             # Read dag file to check if collect job is found
             element_count = 0
             has_collect_job = False
             has_final_collect_job = False
-            with open(dag_file_path, "r") as f:
+            with open(dag_file_path) as f:
                 for line in f.read().splitlines():
                     if "JOB" in line:
                         element_count += 1
                     if "collect" in line:
                         has_collect_job = True
                     if "FINAL" in line:
                         has_final_collect_job = True
@@ -808,24 +808,24 @@
             extra_preamble=extra_preamble,
         )
 
         # Check extra preamble in run submit file
         run_submit_file_path = Path(
             tmp_path / "junifer_jobs" / jobname / f"run_{jobname}.submit"
         )
-        with open(run_submit_file_path, "r") as f:
+        with open(run_submit_file_path) as f:
             for line in f.read().splitlines():
                 if "FOO" in line:
                     assert line.strip() == extra_preamble
 
         # Check extra preamble in collect submit file
         collect_submit_file_path = Path(
             tmp_path / "junifer_jobs" / jobname / f"collect_{jobname}.submit"
         )
-        with open(collect_submit_file_path, "r") as f:
+        with open(collect_submit_file_path) as f:
             for line in f.read().splitlines():
                 if "FOO" in line:
                     assert line.strip() == extra_preamble
 
 
 def test_queue_condor_submission_fail(
     tmp_path: Path,
```

### Comparing `junifer-0.0.3.dev75/junifer/api/tests/test_parser.py` & `junifer-0.0.3.dev89/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/api/utils.py` & `junifer-0.0.3.dev89/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.3.dev89/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.3.dev89/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.3.dev89/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.3.dev89/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.3.dev89/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/coordinates.py` & `junifer-0.0.3.dev89/junifer/data/coordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,14 @@
     """
     if name not in _available_coordinates:
         raise_error(f"Coordinates {name} not found.")
     t_coord = _available_coordinates[name]
     if isinstance(t_coord, Path):
         df_coords = pd.read_csv(t_coord, sep="\t", header=None)
         coords = df_coords.iloc[:, [0, 1, 2]].to_numpy()
-        names = [x for x in df_coords.iloc[:, [3]].values[:, 0]]
+        names = list(df_coords.iloc[:, [3]].values[:, 0])
     else:
         coords = t_coord["coords"]
         coords = typing.cast(ArrayLike, coords)
         names = t_coord["voi_names"]
         names = typing.cast(List[str], names)
     return coords, names
```

### Comparing `junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.3.dev89/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/masks.py` & `junifer-0.0.3.dev89/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/parcellations.py` & `junifer-0.0.3.dev89/junifer/data/parcellations.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         Does not apply to built-in parcellations (default False).
 
     Raises
     ------
     ValueError
         If the parcellation name is already registered and overwrite is set to
         False or if the parcellation name is a built-in parcellation.
+
     """
     # Check for attempt of overwriting built-in parcellations
     if name in _available_parcellations:
         if overwrite is True:
             logger.info(f"Overwriting {name} parcellation")
             if (
                 _available_parcellations[name]["family"]
@@ -135,14 +136,15 @@
 def list_parcellations() -> List[str]:
     """List all the available parcellations.
 
     Returns
     -------
     list of str
         A list with all available parcellations.
+
     """
     return sorted(_available_parcellations.keys())
 
 
 # def _check_resolution(resolution, valid_resolution):
 #     if resolution is None:
 #         return None
@@ -183,14 +185,15 @@
     -------
     Nifti1Image or None
         Loaded parcellation image.
     list of str
         Parcellation labels.
     pathlib.Path
         File path to the parcellation image.
+
     """
     # Invalid parcellation name
     if name not in _available_parcellations:
         raise_error(
             f"Parcellation {name} not found. "
             f"Valid options are: {list_parcellations()}"
         )
@@ -205,15 +208,15 @@
         parcellation_fname, parcellation_labels = _retrieve_parcellation(
             family=t_family,
             parcellations_dir=parcellations_dir,
             resolution=resolution,
             **parcellation_definition,
         )
 
-    logger.info(f"Loading parcellation {str(parcellation_fname.absolute())}")
+    logger.info(f"Loading parcellation {parcellation_fname.absolute()!s}")
 
     parcellation_img = None
     if path_only is False:
         parcellation_img = nib.load(parcellation_fname)
         parcel_values = np.unique(parcellation_img.get_fdata())
         if len(parcel_values) - 1 != len(parcellation_labels):
             raise_error(
@@ -250,20 +253,20 @@
         Path where the retrieved parcellations file are stored. The default
         location is "$HOME/junifer/data/parcellations" (default None).
     resolution : float, optional
         The desired resolution of the parcellation to load. If it is not
         available, the closest resolution will be loaded. Preferably, use a
         resolution higher than the desired one. By default, will load the
         highest one (default None).
+    **kwargs
+        Use to specify parcellation-specific keyword arguments found in the
+        following section.
 
     Other Parameters
     ----------------
-    **kwargs
-        Use to specify parcellation-specific keyword arguments:
-
     * Schaefer :
       ``n_rois`` : {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
             Granularity of parcellation to be used.
        ``yeo_network`` : {7, 17}, optional
             Number of yeo networks to use (default 7).
     * Tian :
         ``scale`` : {1, 2, 3, 4}
@@ -285,14 +288,15 @@
     list of str
         Parcellation labels.
 
     Raises
     ------
     ValueError
         If the parcellation's name is invalid.
+
     """
     if parcellations_dir is None:
         parcellations_dir = (
             Path().home() / "junifer" / "data" / "parcellations"
         )
         # Create default junifer data directory if not present
         parcellations_dir.mkdir(exist_ok=True, parents=True)
@@ -360,14 +364,15 @@
         Parcellation labels.
 
     Raises
     ------
     ValueError
         If invalid value is provided for `n_rois` or `yeo_networks` or if
         there is a problem fetching the parcellation.
+
     """
     logger.info("Parcellation parameters:")
     logger.info(f"\tn_rois: {n_rois}")
     logger.info(f"\tyeo_networks: {yeo_networks}")
     logger.info(f"\tresolution: {resolution}")
 
     _valid_n_rois = [100, 200, 300, 400, 500, 600, 700, 800, 900, 1000]
@@ -467,14 +472,15 @@
         Parcellation labels.
 
     Raises
     ------
     ValueError
         If invalid value is provided for `scale` or `magneticfield` or `space`
         or if there is a problem fetching the parcellation.
+
     """
     # show parameters to user
     logger.info("Parcellation parameters:")
     logger.info(f"\tscale: {scale}")
     logger.info(f"\tspace: {space}")
     logger.info(f"\tmagneticfield: {magneticfield}")
     logger.info(f"\tresolution: {resolution}")
@@ -615,25 +621,26 @@
         highest one (default None). Available resolutions for this parcellation
         are 1mm and 2mm.
     space : {"MNI", "SUIT"}, optional
         Space of parcellation (default "MNI"). (For more information
         see http://www.diedrichsenlab.org/imaging/suit.htm).
 
     Returns
-    ------
+    -------
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
     ValueError
         If invalid value is provided for `space` or if there is a problem
         fetching the parcellation.
+
     """
     logger.info("Parcellation parameters:")
     logger.info(f"\tspace: {space}")
 
     _valid_spaces = ["MNI", "SUIT"]
 
     # check validity of parameters
```

### Comparing `junifer-0.0.3.dev75/junifer/data/tests/test_coordinates.py` & `junifer-0.0.3.dev89/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/tests/test_data_utils.py` & `junifer-0.0.3.dev89/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/tests/test_masks.py` & `junifer-0.0.3.dev89/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/data/tests/test_parcellations.py` & `junifer-0.0.3.dev89/junifer/data/tests/test_parcellations.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     # Test wrong number of labels
     register_parcellation("WrongLabels", schaefer_path, labels[:10])
 
     with pytest.raises(ValueError, match=r"has 100 parcels but 10"):
         load_parcellation("WrongLabels")
 
     # Test wrong number of labels
-    register_parcellation("WrongLabels2", schaefer_path, labels + ["wrong"])
+    register_parcellation("WrongLabels2", schaefer_path, [*labels, "wrong"])
 
     with pytest.raises(ValueError, match=r"has 100 parcels but 101"):
         load_parcellation("WrongLabels2")
 
     schaefer_data = schaefer.get_fdata().copy()
     schaefer_data[schaefer_data == 50] = 0
     new_schaefer_path = tmp_path / "new_schaefer.nii.gz"
```

### Comparing `junifer-0.0.3.dev75/junifer/data/utils.py` & `junifer-0.0.3.dev89/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/__init__.py` & `junifer-0.0.3.dev89/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.3.dev89/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/base.py` & `junifer-0.0.3.dev89/junifer/datagrabber/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
         Yields
         ------
         object
             An element that can be indexed by the DataGrabber.
 
         """
-        for elem in self.get_elements():
-            yield elem
+        yield from self.get_elements()
 
     def __getitem__(self, element: Union[str, Tuple]) -> Dict[str, Dict]:
         """Enable indexing support.
 
         Parameters
         ----------
         element : str or tuple
```

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/datalad_base.py` & `junifer-0.0.3.dev89/junifer/datagrabber/datalad_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                 raise_error(
                     "Dataset already installed but with a different "
                     f"ID: {self._dataset.id} (local) != {remote_id} (remote)"
                 )
 
             # Check for dirty datasets:
             status = self._dataset.status()
-            if any([x["state"] != "clean" for x in status]):
+            if any(x["state"] != "clean" for x in status):
                 self.datalad_dirty = True
                 warn_with_log(
                     "At least one file is not clean, Junifer will "
                     "consider this dataset as dirty."
                 )
             else:
                 logger.debug("Dataset is clean")
```

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 raise_error(
                     f"'{pe}' is not a valid HCP-YA phase encoding. "
                     "Valid phase encoding can be any or all of "
                     f"{all_phase_encodings}."
                 )
 
         if ica_fix:
-            if not all([task in ["REST1", "REST2"] for task in self.tasks]):
+            if not all(task in ["REST1", "REST2"] for task in self.tasks):
                 raise_error(
                     "ICA+FIX is only available for 'REST1' and 'REST2' tasks."
                 )
         suffix = "_hp2000_clean" if ica_fix else ""
         # The types of data
         types = ["BOLD"]
         # The patterns
```

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.3.dev89/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/multiple.py` & `junifer-0.0.3.dev89/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/pattern.py` & `junifer-0.0.3.dev89/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.3.dev89/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_multiple.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     expected_subs = [
         (f"sub-{i:02d}", f"ses-{j:02d}")
         for j in range(1, 3)
         for i in range(1, 10)
     ]
 
     with dg:
-        subs = [x for x in dg]
+        subs = list(dg)
         assert set(subs) == set(expected_subs)
 
         elem = dg[("sub-01", "ses-01")]
         assert "T1w" in elem
         assert "BOLD" in elem
         assert "meta" in elem["BOLD"]
         meta = elem["BOLD"]["meta"]["datagrabber"]
@@ -105,15 +105,15 @@
         patterns=pattern2,
         replacements=replacements,
     )
 
     dg = MultipleDataGrabber([dg1, dg2])
     expected_subs = set()
     with dg:
-        subs = [x for x in dg]
+        subs = list(dg)
         assert set(subs) == set(expected_subs)
 
 
 def test_MultipleDataGrabber_get_item() -> None:
     """Test MultipleDataGrabber get_item() error."""
     repo_uri1 = _testing_dataset["example_bids"]["uri"]
     rootdir = "example_bids_ses"
```

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.3.dev89/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     with PatternDataladDataGrabber(
         rootdir=rootdir,
         uri=repo_uri,
         types=types,
         patterns=patterns,
         replacements=replacements,
     ) as dg:
-        subs = [x for x in dg]
+        subs = list(dg)
         expected_subs = [f"sub-{i:02d}" for i in range(1, 10)]
         assert set(subs) == set(expected_subs)
 
         for elem in dg:
             t_sub = dg[elem]
             assert "path" in t_sub["T1w"]
             assert t_sub["T1w"]["path"] == (
@@ -82,15 +82,15 @@
             assert "class" in dg_meta
             assert dg_meta["class"] == "PatternDataladDataGrabber"
             assert "uri" in dg_meta
             assert dg_meta["uri"] == repo_uri
             assert "datalad_commit_id" in dg_meta
             assert dg_meta["datalad_commit_id"] == repo_commit
 
-            with open(t_sub["T1w"]["path"], "r") as f:
+            with open(t_sub["T1w"]["path"]) as f:
                 assert f.readlines()[0].startswith("placeholder")
 
 
 def test_bids_PatternDataladDataGrabber_datadir() -> None:
     """Test PatternDataladDataGrabber with a datadir set to a relative path."""
     # Define types
     types = ["T1w", "BOLD"]
@@ -155,15 +155,15 @@
     with PatternDataladDataGrabber(
         rootdir=rootdir,
         uri=repo_uri,
         types=types,
         patterns=patterns,
         replacements=replacements,
     ) as dg:
-        subs = [x for x in dg]
+        subs = list(dg)
         expected_subs = [
             (f"sub-{i:02d}", f"ses-{j:02d}")
             for j in range(1, 3)
             for i in range(1, 10)
         ]
         assert set(subs) == set(expected_subs)
 
@@ -175,14 +175,14 @@
     with PatternDataladDataGrabber(
         rootdir=rootdir,
         uri=repo_uri,
         types=types,
         patterns=patterns,
         replacements=replacements,
     ) as dg:
-        subs = [x for x in dg]
+        subs = list(dg)
         expected_subs = [
             (f"sub-{i:02d}", f"ses-{j:02d}")
             for j in range(1, 4)
             for i in range(1, 10)
         ]
         assert set(subs) == set(expected_subs)
```

### Comparing `junifer-0.0.3.dev75/junifer/datagrabber/utils.py` & `junifer-0.0.3.dev89/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datareader/default.py` & `junifer-0.0.3.dev89/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.3.dev89/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.3.dev89/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.3.dev89/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.3.dev89/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev89/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         Indicates, in millimeters, the radius for the sphere around the seed.
     allow_overlap : boolean
         If False, a ValueError is raised if VOIs overlap
     mask_img : Niimg-like object, optional
         Mask to apply to regions before extracting signals. If niimg is None,
         mask_img is used as a reference space in which the spheres 'indices are
         placed.
+
     Returns
     -------
     X : 2D numpy.ndarray
         Signal for each brain voxel in the (masked) niimgs.
         shape: (number of scans, number of voxels)
     A : scipy.sparse.lil_matrix
         Contains the boolean indices for each sphere.
@@ -257,22 +258,22 @@
         self,
         imgs: Union["Nifti1Image", "Nifti2Image"],
     ) -> Tuple["ArrayLike", None]:
         """Implement function call overloading.
 
         Parameters
         ----------
-         imgs : 4D Niimg-like object
-            If ``imgs`` is an iterable, checks if data is really 4D. Then,
-            considering that it is a list of ``img``, load them one by one.
-            If ``img`` is a string, consider it as a path to Nifti image and
-            call :func:`nibabel.load` on it.
-            If it is an object, check if the affine attribute is present and
-            that :func:`nilearn.image.get_data` returns a result, eval raise
-            TypeError.
+        imgs : 4D Niimg-like object
+           If ``imgs`` is an iterable, checks if data is really 4D. Then,
+           considering that it is a list of ``img``, load them one by one.
+           If ``img`` is a string, consider it as a path to Nifti image and
+           call :func:`nibabel.load` on it.
+           If it is an object, check if the affine attribute is present and
+           that :func:`nilearn.image.get_data` returns a result, eval raise
+           TypeError.
 
         Raises
         ------
         TypeError
             If ``img`` in ``imgs`` is an object without the affine attribute.
 
         Returns
```

### Comparing `junifer-0.0.3.dev75/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev89/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 def test_nifti_spheres_masker_overlap() -> None:
     """Test overlapping sphere extraction."""
     # Test resampling in NiftiMapsMasker
     affine = np.eye(4)
     shape = (5, 5, 5)
 
-    data = np.random.RandomState(42).random_sample(shape + (5,))
+    data = np.random.RandomState(42).random_sample((*shape, 5))
     fmri_img = nibabel.Nifti1Image(data, affine)
 
     seeds = [(0, 0, 0), (2, 2, 2)]
 
     overlapping_masker = JuniferNiftiSpheresMasker(
         seeds,
         radius=1,
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/__init__.py` & `junifer-0.0.3.dev89/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/base.py` & `junifer-0.0.3.dev89/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/collection.py` & `junifer-0.0.3.dev89/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/ets_rss.py` & `junifer-0.0.3.dev89/junifer/markers/ets_rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Nicolás Nieto <n.nieto@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 import numpy as np
 
 from ..api.decorators import register_marker
 from ..utils import logger
 from .base import BaseMarker
 from .parcel_aggregation import ParcelAggregation
@@ -38,15 +38,15 @@
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     """
 
-    _DEPENDENCIES = {"nilearn"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn"}
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/falff_base.py` & `junifer-0.0.3.dev89/junifer/markers/falff/falff_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
 # License: AGPL
 
 from abc import abstractmethod
-from typing import Dict, List, Optional
+from typing import ClassVar, Dict, List, Optional, Union
 
 from ...utils.logging import raise_error
 from ..base import BaseMarker
 from .falff_estimator import ALFFEstimator
 
 
 class ALFFBase(BaseMarker):
@@ -40,15 +40,17 @@
         computation. If a dataset is correctly preprocessed, the TR should be
         extracted from the NIFTI without any issue. However, it has been
         reported that some preprocessed data might not have the correct TR in
         the NIFTI header.
 
     """
 
-    _EXT_DEPENDENCIES = [
+    _EXT_DEPENDENCIES: ClassVar[
+        List[Dict[str, Union[str, bool, List[str]]]]
+    ] = [
         {
             "name": "afni",
             "optional": True,
             "commands": ["3dRSFC", "3dAFNItoNIFTI"],
         },
     ]
 
@@ -151,15 +153,15 @@
             input_data=input,
             highpass=self.highpass,
             lowpass=self.lowpass,
             tr=self.tr,
         )
         post_data = falff if self.fractional else alff
 
-        post_input = {k: v for k, v in input.items()}
+        post_input = dict(input.items())
         post_input["data"] = post_data
         post_input["path"] = None
 
         out = self._postprocess(post_input, extra_input=extra_input)
 
         return out
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.3.dev89/junifer/markers/falff/falff_estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         python_falff[denom_mask] = 0
 
         python_alff = numerator / np.sqrt(timeseries.shape[-1])
         alff_img = nimg.new_img_like(data, python_alff)
         falff_img = nimg.new_img_like(data, python_falff)
         return alff_img, falff_img
 
-    @lru_cache(maxsize=None, typed=True)  # noqa: B019
+    @lru_cache(maxsize=None, typed=True)
     def _compute(
         self,
         use_afni: bool,
         data: Union["Nifti1Image", "Nifti2Image"],
         highpass: float,
         lowpass: float,
         tr: Optional[float],
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,30 @@
         lowpass=0.1,
         tr=None,
     )
     first_time = time.time() - start_time
     logger.info(f"ALFF Estimator First time: {first_time}")
     assert isinstance(alff, Nifti1Image)
     assert isinstance(falff, Nifti1Image)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now fit again, should be faster
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=False,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     second_time = time.time() - start_time
     logger.info(f"ALFF Estimator Second time: {second_time}")
     assert second_time < (first_time / 1000)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now change a parameter, should compute again, without clearing the
     # cache
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=False,
@@ -63,30 +63,30 @@
         highpass=0.01,
         lowpass=0.11,
         tr=None,
     )
     third_time = time.time() - start_time
     logger.info(f"ALFF Estimator Third time: {third_time}")
     assert third_time > (first_time / 10)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now fit again with the previous params, should be fast
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=False,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     fourth = time.time() - start_time
     logger.info(f"ALFF Estimator Fourth time: {fourth}")
     assert fourth < (first_time / 1000)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now change the data, it should clear the cache
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-02"]
 
     input = DefaultDataReader().fit_transform(input)
@@ -98,15 +98,15 @@
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     fifth = time.time() - start_time
     logger.info(f"ALFF Estimator Fifth time: {fifth}")
     assert fifth > (first_time / 10)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
 def test_ALFFEstimator_cache_afni() -> None:
@@ -125,30 +125,30 @@
         lowpass=0.1,
         tr=None,
     )
     first_time = time.time() - start_time
     logger.info(f"ALFF Estimator First time: {first_time}")
     assert isinstance(alff, Nifti1Image)
     assert isinstance(falff, Nifti1Image)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 3  # input + alff + falff
 
     # Now fit again, should be faster
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=True,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     second_time = time.time() - start_time
     logger.info(f"ALFF Estimator Second time: {second_time}")
     assert second_time < (first_time / 1000)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 3  # input + alff + falff
 
     # Now change a parameter, should compute again, without clearing the
     # cache
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=True,
@@ -156,30 +156,30 @@
         highpass=0.01,
         lowpass=0.11,
         tr=None,
     )
     third_time = time.time() - start_time
     logger.info(f"ALFF Estimator Third time: {third_time}")
     assert third_time > (first_time / 10)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 5  # input + 2 * alff + 2 * falff
 
     # Now fit again with the previous params, should be fast
     start_time = time.time()
     alff, falff = estimator.fit_transform(
         use_afni=True,
         input_data=input["BOLD"],
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     fourth = time.time() - start_time
     logger.info(f"ALFF Estimator Fourth time: {fourth}")
     assert fourth < (first_time / 1000)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 5  # input + 2 * alff + 2 * falff
 
     # Now change the data, it should clear the cache
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-02"]
 
     input = DefaultDataReader().fit_transform(input)
@@ -191,15 +191,15 @@
         highpass=0.01,
         lowpass=0.1,
         tr=None,
     )
     fifth = time.time() - start_time
     logger.info(f"ALFF Estimator Fifth time: {fifth}")
     assert fifth > (first_time / 10)
-    n_files = len([x for x in estimator.temp_dir_path.glob("*")])
+    n_files = len(list(estimator.temp_dir_path.glob("*")))
     assert n_files == 3  # input + alff + falff
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
 def test_ALFFEstimator_afni_vs_python() -> None:
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,17 @@
 def test_ALFFParcels_python_vs_afni(
     fractional: bool,
 ) -> None:
     """Test ALFFParcels using python.
 
     Parameters
     ----------
-    factional : bool
+    fractional : bool
         Whether to compute fractional ALFF or not.
+
     """
 
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
 
     input = DefaultDataReader().fit_transform(input)
     # Create ParcelAggregation object
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide marker class to calculate cross-parcellation FC."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 import pandas as pd
 
 from ...api.decorators import register_marker
 from ...utils import logger, raise_error
 from ..base import BaseMarker
 from ..parcel_aggregation import ParcelAggregation
@@ -35,15 +35,15 @@
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name
         (default None).
     """
 
-    _DEPENDENCIES = {"nilearn"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn"}
 
     def __init__(
         self,
         parcellation_one: str,
         parcellation_two: str,
         aggregation_method: str = "mean",
         correlation_method: str = "pearson",
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provide abstract base class for functional connectivity (FC)."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 
 from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 from nilearn.connectome import ConnectivityMeasure
 from sklearn.covariance import EmpiricalCovariance
 
 from ...utils import raise_error
 from ..base import BaseMarker
 
@@ -38,15 +38,15 @@
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     """
 
-    _DEPENDENCIES = {"nilearn", "scikit-learn"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn", "scikit-learn"}
 
     def __init__(
         self,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         cor_method: str = "covariance",
         cor_method_params: Optional[Dict] = None,
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from nilearn import image
 
 from junifer.markers.functional_connectivity import CrossParcellationFC
 from junifer.storage import SQLiteFeatureStorage
 from junifer.testing.datagrabbers import SPMAuditoryTestingDataGrabber
 
 
-parcellation_ONE = "Schaefer100x17"
-parcellation_TWO = "Schaefer200x17"
+parcellation_one = "Schaefer100x17"
+parcellation_two = "Schaefer200x17"
 
 
 def test_compute() -> None:
     """Test CrossParcellationFC compute()."""
 
     with SPMAuditoryTestingDataGrabber() as dg:
         out = dg["sub001"]
@@ -29,16 +29,16 @@
                 "data": niimg,
                 "path": out["BOLD"]["path"],
                 "meta": {"element": "sub001"},
             }
         }
 
         crossparcellation = CrossParcellationFC(
-            parcellation_one=parcellation_ONE,
-            parcellation_two=parcellation_TWO,
+            parcellation_one=parcellation_one,
+            parcellation_two=parcellation_two,
             correlation_method="spearman",
         )
         out = crossparcellation.compute(input_dict["BOLD"])
         assert out["data"].shape == (200, 100)
         assert len(out["col_names"]) == 100
         assert len(out["row_names"]) == 200
 
@@ -56,16 +56,16 @@
     with SPMAuditoryTestingDataGrabber() as dg:
         input_dict = dg["sub001"]
         niimg = image.load_img(str(input_dict["BOLD"]["path"].absolute()))
 
         input_dict["BOLD"]["data"] = niimg
 
         crossparcellation = CrossParcellationFC(
-            parcellation_one=parcellation_ONE,
-            parcellation_two=parcellation_TWO,
+            parcellation_one=parcellation_one,
+            parcellation_two=parcellation_two,
             correlation_method="spearman",
         )
         uri = tmp_path / "test_crossparcellation.sqlite"
         storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
         crossparcellation.fit_transform(input_dict, storage=storage)
         features = storage.list_features()
         assert any(
@@ -73,15 +73,15 @@
         )
 
 
 def test_get_output_type() -> None:
     """Test CrossParcellationFC get_output_type()."""
 
     crossparcellation = CrossParcellationFC(
-        parcellation_one=parcellation_ONE, parcellation_two=parcellation_TWO
+        parcellation_one=parcellation_one, parcellation_two=parcellation_two
     )
     input_ = "BOLD"
     output = crossparcellation.get_output_type(input_)
     assert output == "matrix"
 
 
 def test_init_() -> None:
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/parcel_aggregation.py` & `junifer-0.0.3.dev89/junifer/markers/parcel_aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide class for parcel aggregation."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 import numpy as np
 from nilearn.image import math_img, resample_to_img
 from nilearn.maskers import NiftiMasker
 
 from ..api.decorators import register_marker
 from ..data import get_mask, load_parcellation, merge_parcellations
@@ -47,15 +47,15 @@
         The data types to apply the marker to. If None, will work on all
         available data (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
     """
 
-    _DEPENDENCIES = {"nilearn", "numpy"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn", "numpy"}
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         method: str,
         method_params: Optional[Dict[str, Any]] = None,
         time_method: Optional[str] = None,
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/reho_base.py` & `junifer-0.0.3.dev89/junifer/markers/reho/reho_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide base class for regional homogeneity (ReHo)."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional, Union
 
 from ...utils import logger, raise_error
 from ..base import BaseMarker
 from .reho_estimator import ReHoEstimator
 
 
 if TYPE_CHECKING:
@@ -25,15 +25,17 @@
         if available (default None).
     name : str, optional
         The name of the marker. If None, it will use the class name
         (default None).
 
     """
 
-    _EXT_DEPENDENCIES = [
+    _EXT_DEPENDENCIES: ClassVar[
+        List[Dict[str, Union[str, bool, List[str]]]]
+    ] = [
         {
             "name": "afni",
             "optional": True,
             "commands": ["3dReHo", "3dAFNItoNIFTI"],
         },
     ]
 
@@ -98,15 +100,15 @@
         Niimg-like object
 
         References
         ----------
         .. [1] Jiang, L., & Zuo, X. N. (2016).
                Regional Homogeneity: A Multimodal, Multiscale Neuroimaging
                Marker of the Human Connectome.
-               The Neuroscientist, Volume 22(5), Pages 486–505.
+               The Neuroscientist, Volume 22(5), Pages 486-505.
                https://doi.org/10.1177/1073858415595004
 
         """
         if self.use_afni is None:
             raise_error(
                 "Parameter `use_afni` must be set to True or False in order "
                 "to compute this marker. It is currently set to None (default "
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.3.dev89/junifer/markers/reho/reho_estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,15 @@
 
             * 7 : for facewise neighbours only
             * 19 : for face- and edge-wise nieghbours
             * 27 : for face-, edge-, and node-wise neighbors
             * 125 : for 5x5 cuboidal volume
 
             (default 27).
+
         Returns
         -------
         Niimg-like object
 
         Raises
         ------
         ValueError
@@ -477,15 +478,15 @@
     """Calculate Kendall's coefficient of concordance (KCC) for ReHo map.
 
     ..note:: This function should only be used to calculate KCC for a ReHo map.
              For general use, check out ``junifer.stats.kendall_w``.
 
     Parameters
     ----------
-    timeseries_matrix : 2D numpy.ndarray
+    timeseries_ranks : 2D numpy.ndarray
         A matrix of ranks of a subset subject's brain voxels.
     tied_rank_corrections : 3D numpy.ndarray
         A 3D array consisting of the tied rank corrections for the ranks
         of a subset subject's brain voxels.
 
     Returns
     -------
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/reho/reho_parcels.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
-        parcel_aggregation_input = {k: v for k, v in input.items()}
+        parcel_aggregation_input = dict(input.items())
         parcel_aggregation_input["data"] = reho_map
         parcel_aggregation_input["path"] = None
 
         output = parcel_aggregation.compute(
             input=parcel_aggregation_input,
             extra_input=extra_input,
         )
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/reho/reho_spheres.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
-        sphere_aggregation_input = {k: v for k, v in input.items()}
+        sphere_aggregation_input = dict(input.items())
         sphere_aggregation_input["data"] = reho_map
         sphere_aggregation_input["path"] = None
         output = sphere_aggregation.compute(
             input=sphere_aggregation_input, extra_input=extra_input
         )
         # Only use the first row and expand row dimension
         output["data"] = output["data"][0][np.newaxis, :]
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     )
     first_toc = time.time()
     logger.info(
         f"ReHo estimator in Python without cache: {first_toc - first_tic}"
     )
     assert isinstance(reho_map_without_cache, nib.Nifti1Image)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now fit again, should be faster
     second_tic = time.time()
     reho_map_with_cache = reho_estimator.fit_transform(
         use_afni=False,
         input_data=subject_data["BOLD"],
@@ -52,15 +52,15 @@
     logger.info(
         f"ReHo estimator in Python with cache: {second_toc - second_tic}"
     )
     assert isinstance(reho_map_with_cache, nib.Nifti1Image)
     # Check that cache is being used
     assert (second_toc - second_tic) < ((first_toc - first_tic) / 1000)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now change a parameter, should compute again, without clearing the
     # cache
     third_tic = time.time()
     reho_map_with_partial_cache = reho_estimator.fit_transform(
         use_afni=False,
@@ -71,15 +71,15 @@
     logger.info(
         f"ReHo estimator in Python with partial cache: {third_toc - third_tic}"
     )
     assert isinstance(reho_map_with_partial_cache, nib.Nifti1Image)
     # Should require more time
     assert (third_toc - third_tic) > ((first_toc - first_tic) / 10)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now fit again with the previous params, should be fast
     fourth_tic = time.time()
     reho_map_with_new_cache = reho_estimator.fit_transform(
         use_afni=False,
         input_data=subject_data["BOLD"],
@@ -89,15 +89,15 @@
     logger.info(
         f"ReHo estimator in Python with new cache: {fourth_toc - fourth_tic}"
     )
     assert isinstance(reho_map_with_new_cache, nib.Nifti1Image)
     # Should require less time
     assert (fourth_toc - fourth_tic) < ((first_toc - first_tic) / 1000)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
     # Now change the data, it should clear the cache
     with PartlyCloudyTestingDataGrabber() as dg:
         subject = dg["sub-02"]
     # Read data for new subject
     subject_data = DefaultDataReader().fit_transform(subject)
@@ -113,15 +113,15 @@
         "ReHo estimator in Python with different cache: "
         f"{fifth_toc - fifth_tic}"
     )
     assert isinstance(reho_map_with_different_cache, nib.Nifti1Image)
     # Should take less time
     assert (fifth_toc - fifth_tic) > ((first_toc - first_tic) / 10)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 0  # no files in python
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
 def test_reho_estimator_cache_afni() -> None:
@@ -142,15 +142,15 @@
     )
     first_toc = time.time()
     logger.info(
         f"ReHo estimator in AFNI without cache: {first_toc - first_tic}"
     )
     assert isinstance(reho_map_without_cache, nib.Nifti1Image)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 2  # input + reho
 
     # Now fit again, should be faster
     second_tic = time.time()
     reho_map_with_cache = reho_estimator.fit_transform(
         use_afni=True,
         input_data=subject_data["BOLD"],
@@ -159,15 +159,15 @@
     second_toc = time.time()
     logger.info(
         f"ReHo estimator in AFNI with cache: {second_toc - second_tic}"
     )
     assert isinstance(reho_map_with_cache, nib.Nifti1Image)
     assert (second_toc - second_tic) < ((first_toc - first_tic) / 1000)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 2  # input + reho
 
     # Now change a parameter, should compute again, without clearing the
     # cache
     third_tic = time.time()
     reho_map_with_partial_cache = reho_estimator.fit_transform(
         use_afni=True,
@@ -178,15 +178,15 @@
     logger.info(
         f"ReHo estimator in AFNI with partial cache: {third_toc - third_tic}"
     )
     assert isinstance(reho_map_with_partial_cache, nib.Nifti1Image)
     # Should require more time
     assert (third_toc - third_tic) > ((first_toc - first_tic) / 10)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 3  # input + 2 * reho
 
     # Now fit again with the previous params, should be fast
     fourth_tic = time.time()
     reho_map_with_new_cache = reho_estimator.fit_transform(
         use_afni=True,
         input_data=subject_data["BOLD"],
@@ -195,15 +195,15 @@
     fourth_toc = time.time()
     logger.info(
         f"ReHo estimator in AFNI with new cache: {fourth_toc - fourth_tic}"
     )
     assert isinstance(reho_map_with_new_cache, nib.Nifti1Image)
     # Should require less time
     assert (fourth_toc - fourth_tic) < ((first_toc - first_tic) / 1000)
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 3  # input + 2 * reho
 
     # Now change the data, it should clear the cache
     with PartlyCloudyTestingDataGrabber() as dg:
         subject = dg["sub-02"]
     # Read data for new subject
     subject_data = DefaultDataReader().fit_transform(subject)
@@ -218,15 +218,15 @@
     logger.info(
         f"ReHo estimator in AFNI with different cache: {fifth_toc - fifth_tic}"
     )
     assert isinstance(reho_map_with_different_cache, nib.Nifti1Image)
     # Should take less time
     assert (fifth_toc - fifth_tic) > ((first_toc - first_tic) / 10)
     # Count intermediate files
-    n_files = len([x for x in reho_estimator.temp_dir_path.glob("*")])
+    n_files = len(list(reho_estimator.temp_dir_path.glob("*")))
     assert n_files == 2  # input + reho
 
 
 @pytest.mark.skipif(
     _check_afni() is False, reason="requires afni to be in PATH"
 )
 def test_reho_estimator_afni_vs_python() -> None:
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/sphere_aggregation.py` & `junifer-0.0.3.dev89/junifer/markers/sphere_aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide class for sphere aggregation."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 from ..api.decorators import register_marker
 from ..data import get_mask, load_coordinates
 from ..external.nilearn import JuniferNiftiSpheresMasker
 from ..stats import get_aggfunc_by_name
 from ..utils import logger, raise_error, warn_with_log
 from .base import BaseMarker
@@ -53,15 +53,15 @@
         available data (default None).
     name : str, optional
         The name of the marker. By default, it will use KIND_SphereAggregation
         where KIND is the kind of data it was applied to (default None).
 
     """
 
-    _DEPENDENCIES = {"nilearn", "numpy"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn", "numpy"}
 
     def __init__(
         self,
         coords: str,
         radius: Optional[float] = None,
         allow_overlap: bool = False,
         method: str = "mean",
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provide abstract base class for temporal signal-to-noise ratio (tSNR)."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 # License: AGPL
 
 
 from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 from nilearn import image as nimg
 
 from ...utils import raise_error
 from ..base import BaseMarker
 
 
@@ -30,15 +30,15 @@
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     """
 
-    _DEPENDENCIES = {"nilearn"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn"}
 
     def __init__(
         self,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
```

### Comparing `junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.3.dev89/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_collection.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.3.dev89/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/markers/utils.py` & `junifer-0.0.3.dev89/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.3.dev89/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/registry.py` & `junifer-0.0.3.dev89/junifer/pipeline/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     ----------
     step : str
         Name of the step.
     name : str
         Name of the function.
     baseclass : class
         Class to be checked against.
-    init_parms : dict, optional
+    init_params : dict or None, optional
         Parameters to pass to the base class constructor (default None).
 
     Returns
     -------
     object
         An instance of the given base class.
 
@@ -135,17 +135,17 @@
     logger.debug(f"Building {step}/{name}")
     klass = get_class(step=step, name=name)
     logger.debug(f"\tClass: {klass.__name__}")
     logger.debug(f"\tInit params: {init_params}")
     try:
         # Create instance of the class
         object_ = klass(**init_params)
-    except Exception as e:
+    except (ValueError, TypeError) as e:
         raise_error(
-            msg=(f"Failed to create {step} ({name}). " f"Error: {e}"),
+            msg=f"Failed to create {step} ({name}). Error: {e}",
             klass=RuntimeError,
             exception=e,
         )
     # Verify created instance belongs to the base class
     if not isinstance(object_, baseclass):
         raise_error(
             msg=(
```

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.3.dev89/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provide tests for pipeline mixin."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import warnings
-from typing import Dict, List
+from typing import ClassVar, Dict, List, Set, Union
 
 import pytest
 
 from junifer.pipeline.pipeline_step_mixin import PipelineStepMixin
 from junifer.pipeline.utils import _check_afni
 
 
@@ -26,15 +26,15 @@
 
 def test_pipeline_step_mixin_validate_correct_dependencies() -> None:
     """Test validate with correct dependencies."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _DEPENDENCIES = {"setuptools"}
+        _DEPENDENCIES: ClassVar[Set[str]] = {"setuptools"}
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
@@ -47,15 +47,15 @@
 
 def test_pipeline_step_mixin_validate_incorrect_dependencies() -> None:
     """Test validate with incorrect dependencies."""
 
     class IncorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _DEPENDENCIES = {"foobar"}
+        _DEPENDENCIES: ClassVar[Set[str]] = {"foobar"}
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
@@ -72,15 +72,17 @@
 )
 def test_pipeline_step_mixin_validate_correct_ext_dependencies() -> None:
     """Test validate with correct external dependencies."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _EXT_DEPENDENCIES = [{"name": "afni", "optional": False}]
+        _EXT_DEPENDENCIES: ClassVar[List[Dict[str, Union[str, bool]]]] = [
+            {"name": "afni", "optional": False}
+        ]
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
@@ -96,17 +98,17 @@
 )
 def test_pipeline_step_mixin_validate_ext_deps_correct_commands() -> None:
     """Test validate with correct external dependencies' correct commands."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _EXT_DEPENDENCIES = [
-            {"name": "afni", "optional": False, "commands": ["3dReHo"]}
-        ]
+        _EXT_DEPENDENCIES: ClassVar[
+            List[Dict[str, Union[str, bool, List[str]]]]
+        ] = [{"name": "afni", "optional": False, "commands": ["3dReHo"]}]
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
@@ -124,17 +126,17 @@
 )
 def test_pipeline_step_mixin_validate_ext_deps_incorrect_commands() -> None:
     """Test validate with correct external dependencies' incorrect commands."""
 
     class CorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _EXT_DEPENDENCIES = [
-            {"name": "afni", "optional": False, "commands": ["3d"]}
-        ]
+        _EXT_DEPENDENCIES: ClassVar[
+            List[Dict[str, Union[str, bool, List[str]]]]
+        ] = [{"name": "afni", "optional": False, "commands": ["3d"]}]
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
 
@@ -148,15 +150,17 @@
 
 def test_pipeline_step_mixin_validate_incorrect_ext_dependencies() -> None:
     """Test validate with incorrect external dependencies."""
 
     class IncorrectMixer(PipelineStepMixin):
         """Test class for validation."""
 
-        _EXT_DEPENDENCIES = [{"name": "foobar", "optional": True}]
+        _EXT_DEPENDENCIES: ClassVar[List[Dict[str, Union[str, bool]]]] = [
+            {"name": "foobar", "optional": True}
+        ]
 
         def validate_input(self, input: List[str]) -> List[str]:
             return input
 
         def get_output_type(self, input_type: str) -> str:
             return input_type
```

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.3.dev89/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.3.dev89/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from junifer.pipeline.update_meta_mixin import UpdateMetaMixin
 
 
 @pytest.mark.parametrize(
     "input, step_name, dependencies, expected",
     [
         ({}, "step_name", None, set()),
-        ({}, "step_name", ["numpy"], set(["numpy"])),
-        ({}, "step_name", "numpy", set(["numpy"])),
-        ({}, "step_name", set(["numpy"]), set(["numpy"])),
+        ({}, "step_name", ["numpy"], {"numpy"}),
+        ({}, "step_name", "numpy", {"numpy"}),
+        ({}, "step_name", {"numpy"}, {"numpy"}),
     ],
 )
 def test_UpdateMetaMixin(
     input: Dict,
     step_name: str,
     dependencies: Union[Set, List, str, None],
     expected: Set,
```

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.3.dev89/junifer/pipeline/update_meta_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,9 @@
         input["meta"][step_name] = t_meta
         if "dependencies" not in input["meta"]:
             input["meta"]["dependencies"] = set()
 
         dependencies = getattr(self, "_DEPENDENCIES", set())
         if dependencies is not None:
             if not isinstance(dependencies, (set, list)):
-                dependencies = set([dependencies])
+                dependencies = {dependencies}
             input["meta"]["dependencies"].update(dependencies)
```

### Comparing `junifer-0.0.3.dev75/junifer/pipeline/utils.py` & `junifer-0.0.3.dev89/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/preprocess/base.py` & `junifer-0.0.3.dev89/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.3.dev89/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """Provide class for confound removal using fMRIPrep format."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 
 import numpy as np
 import pandas as pd
 from nilearn._utils.niimg_conversions import check_niimg_4d
 from nilearn.image import clean_img
 
 from ...api.decorators import register_preprocessor
@@ -137,15 +147,15 @@
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
 
     """
 
-    _DEPENDENCIES = {"numpy", "nilearn"}
+    _DEPENDENCIES: ClassVar[Set[str]] = {"numpy", "nilearn"}
 
     def __init__(
         self,
         strategy: Optional[Dict[str, str]] = None,
         spike: Optional[float] = None,
         detrend: bool = True,
         standardize: bool = True,
@@ -204,14 +214,15 @@
         """Validate the input to the pipeline step.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
             available Junifer Data object keys.
+
         Returns
         -------
         list of str
             The actual elements of the input that will be processed by this
             pipeline step.
 
         Raises
@@ -539,15 +550,15 @@
             Dictionary containing the ``BOLD`` value from the
             Junifer Data object.
         extra_input : dict, optional
             Dictionary containing the rest of the Junifer Data object. Must
             include the ``BOLD_confounds`` key.
 
         Returns
-        --------
+        -------
         Niimg-like object
             Input image with confounds removed.
 
         """
         assert extra_input is not None  # Not the case, data is validated
         confounds_df = self._pick_confounds(extra_input["BOLD_confounds"])
         confounds_array = confounds_df.values
```

### Comparing `junifer-0.0.3.dev75/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.3.dev89/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         "trans_z",
         "rot_x",
         "rot_y",
         "rot_z",
     ]
 
     # Build mappings dictionary
-    mappings = {x: y for x, y in zip(adhoc_names, fmriprep_names)}
+    mappings = dict(zip(adhoc_names, fmriprep_names))
     input = {
         "mappings": {"fmriprep": mappings},
         "data": adhoc_df,
     }
 
     confound_remover._map_adhoc_to_fmriprep(input)
     # This should work in-place
@@ -166,15 +166,15 @@
         "white_matter_derivative1_power2",
     ]
 
     all_names = var_names + missing_der_names + missing_sq_names
 
     confounds_df = pd.DataFrame(
         np.random.randn(7, len(var_names) + 1),
-        columns=var_names + ["framewise_displacement"],
+        columns=[*var_names, "framewise_displacement"],
     )
     out = confound_remover._process_fmriprep_spec({"data": confounds_df})
     to_select, sq_to_compute, der_to_compute, spike_name = out
     assert set(to_select) == set(all_names)
     assert set(sq_to_compute) == set(missing_sq_names)
     assert set(der_to_compute) == set(missing_der_names)
     assert spike_name == "framewise_displacement"
@@ -244,15 +244,15 @@
         "csf_derivative1",
         "white_matter_derivative1",
         "csf_derivative1_power2",
         "white_matter_derivative1_power2",
     ]
 
     # Build mappings dictionary
-    mappings = {x: y for x, y in zip(adhoc_names, fmriprep_names)}
+    mappings = dict(zip(adhoc_names, fmriprep_names))
     input = {
         "mappings": {"fmriprep": mappings},
         "data": adhoc_df,
         "format": "adhoc",
     }
 
     out = confound_remover._pick_confounds(input)
@@ -277,21 +277,21 @@
 
     reader = DefaultDataReader()
     out1, out2 = None, None
     with PartlyCloudyTestingDataGrabber() as dg:
         input = dg["sub-01"]
         input = reader.fit_transform(input)
         out1 = confound_remover._pick_confounds(input["BOLD_confounds"])
-        assert set(out1.columns) == set(fmriprep_all_vars + ["spike"])
+        assert set(out1.columns) == {*fmriprep_all_vars, "spike"}
 
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
         input = dg["sub-01"]
         input = reader.fit_transform(input)
         out2 = confound_remover._pick_confounds(input["BOLD_confounds"])
-        assert set(out2.columns) == set(fmriprep_all_vars + ["spike"])
+        assert set(out2.columns) == {*fmriprep_all_vars, "spike"}
 
     assert_frame_equal(out1, out2)
 
 
 def test_FMRIPRepConfoundRemover__pick_confounds_fmriprep_compute() -> None:
     """Test if fmriprep returns the same derivatives/power2 as we compute."""
```

### Comparing `junifer-0.0.3.dev75/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.3.dev89/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/stats.py` & `junifer-0.0.3.dev89/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/base.py` & `junifer-0.0.3.dev89/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/hdf5.py` & `junifer-0.0.3.dev89/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/pandas_base.py` & `junifer-0.0.3.dev89/junifer/storage/pandas_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,18 +127,20 @@
     def store_df(
         self, meta_md5: str, element: Dict, df: Union[pd.DataFrame, pd.Series]
     ) -> None:
         """Implement pandas DataFrame storing.
 
         Parameters
         ----------
+        meta_md5 : str
+            The metadata MD5 hash.
+        element : dict
+            The element as a dictionary.
         df : pandas.DataFrame or pandas.Series
             The pandas DataFrame or Series to store.
-        meta : dict
-            The metadata as a dictionary.
 
         Raises
         ------
         ValueError
             If the dataframe index has items that are not in the index
             generated from the metadata.
```

### Comparing `junifer-0.0.3.dev75/junifer/storage/sqlite.py` & `junifer-0.0.3.dev89/junifer/storage/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             )
         # Convert str to Path
         if not isinstance(uri, Path):
             uri = Path(uri)
         # Create parent directories if not present
         if not uri.parent.exists():
             logger.info(
-                f"Output directory ({str(uri.parent.absolute())}) "
+                f"Output directory ({uri.parent.absolute()!s}) "
                 "does not exist, creating now."
             )
             uri.parent.mkdir(parents=True, exist_ok=True)
         # Available storage kinds
         storage_types = ["vector", "timeseries", "matrix"]
         super().__init__(
             uri=uri,
@@ -347,18 +347,20 @@
     def store_df(
         self, meta_md5: str, element: Dict, df: Union[pd.DataFrame, pd.Series]
     ) -> None:
         """Implement pandas DataFrame storing.
 
         Parameters
         ----------
+        meta_md5 : str
+            The metadata MD5 hash.
+        element : dict
+            The element as a dictionary.
         df : pandas.DataFrame or pandas.Series
             The pandas DataFrame or Series to store.
-        meta : dict
-            The metadata as a dictionary.
 
         Raises
         ------
         ValueError
             If the dataframe index has items that are not in the index
             generated from the metadata.
 
@@ -472,15 +474,15 @@
                 msg="The number of columns is greater than 2000. "
                 "The data will be stored in long format. "
                 "This will make it slower to collect the data. "
                 "Future versions of junifer will provide additional storage "
                 "options that will not raise this warning.",
             )
             data_df = data_df.stack()
-            new_names = [x for x in data_df.index.names[:-1]]
+            new_names = list(data_df.index.names[:-1])
             new_names.append("pair")
             data_df.index.names = new_names
 
         # Store dataframe
         self.store_df(meta_md5=meta_md5, element=element, df=data_df)
 
     def collect(self) -> None:
@@ -502,15 +504,15 @@
             f"{self.uri.parent}/*{self.uri.name}"  # type: ignore
         )
         # Create new instance
         out_storage = SQLiteFeatureStorage(uri=self.uri, upsert="ignore")
         # Glob files
         files = self.uri.parent.glob(f"*{self.uri.name}")  # type: ignore
         for elem in tqdm(files, desc="file"):
-            logger.debug(f"Reading from {str(elem.absolute())}")
+            logger.debug(f"Reading from {elem.absolute()!s}")
             in_storage = SQLiteFeatureStorage(uri=elem)
             in_engine = in_storage.get_engine()
             # Open "meta" table
             t_meta_df = pd.read_sql(
                 sql="meta", con=in_engine, index_col="meta_md5"
             )
             # Save metadata
```

### Comparing `junifer-0.0.3.dev75/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.3.dev89/junifer/storage/tests/test_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -878,14 +878,20 @@
 ) -> None:
     """Test multi output storing and collection.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
+    n_elements : int
+        The parametrized element count.
+    chunk_size : int
+        The parametrized chunk size.
+    kind : str
+        The parametrized storage kind.
 
     """
     uri = tmp_path / "test_multi_output_store_and_collect.hdf5"
     storage = HDF5FeatureStorage(
         uri=uri, single_output=False, chunk_size=chunk_size
     )
```

### Comparing `junifer-0.0.3.dev75/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.3.dev89/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.3.dev89/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.3.dev89/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/tests/test_utils.py` & `junifer-0.0.3.dev89/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/storage/utils.py` & `junifer-0.0.3.dev89/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.3.dev89/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/datagrabbers.py` & `junifer-0.0.3.dev89/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/registry.py` & `junifer-0.0.3.dev89/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.3.dev89/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.3.dev89/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.3.dev89/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.3.dev89/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/testing/utils.py` & `junifer-0.0.3.dev89/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/tests/test_stats.py` & `junifer-0.0.3.dev89/junifer/tests/test_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,23 @@
     output = winsorized_mean(input, limits=[0.1, 0.1])
     assert output == 5.5
 
 
 def test_count() -> None:
     """Test count."""
     input = np.zeros((10, 3))
-    ax1 = np.ones((10)) * 3
-    ax2 = np.ones((3)) * 10
+    ax1 = np.ones(10) * 3
+    ax2 = np.ones(3) * 10
     assert_array_equal(count(input, axis=-1), ax1)
     assert_array_equal(count(input, axis=1), ax1)
     assert_array_equal(count(input, axis=0), ax2)
 
     input = np.zeros((10, 0))
-    ax1 = np.zeros((10))
-    ax2 = np.zeros((0))
+    ax1 = np.zeros(10)
+    ax2 = np.zeros(0)
 
     assert_array_equal(count(input, axis=-1), ax1)
     assert_array_equal(count(input, axis=1), ax1)
     assert_array_equal(count(input, axis=0), ax2)
 
 
 def test_select() -> None:
```

### Comparing `junifer-0.0.3.dev75/junifer/utils/logging.py` & `junifer-0.0.3.dev89/junifer/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
 }
 
 
 class WrapStdOut(logging.StreamHandler):
-    """
-    Dynamically wrap to sys.stdout.
+    """Dynamically wrap to sys.stdout.
 
     This makes packages that monkey-patch sys.stdout (e.g.doctest,
     sphinx-gallery) work properly.
 
     """
 
     def __getattr__(self, name: str) -> str:
@@ -235,17 +234,18 @@
     # Set logging output handler
     if fname is not None:
         # Convert str to Path
         if not isinstance(fname, Path):
             fname = Path(fname)
         if fname.exists() and overwrite is None:
             warn(
-                f"File ({str(fname.absolute())}) exists. "
+                f"File ({fname.absolute()!s}) exists. "
                 "Messages will be appended. Use overwrite=True to "
-                "overwrite or overwrite=False to avoid this message."
+                "overwrite or overwrite=False to avoid this message.",
+                stacklevel=2,
             )
             overwrite = False
         mode = "w" if overwrite else "a"
         lh = logging.FileHandler(fname, mode=mode)
     else:
         lh = logging.StreamHandler(WrapStdOut())  # type: ignore
 
@@ -299,8 +299,8 @@
     msg : str
         Warning message.
     category : subclass of Warning, optional
         The warning subclass (default RuntimeWarning).
 
     """
     logger.warning(msg)
-    warn(msg, category=category)
+    warn(msg, category=category, stacklevel=2)
```

### Comparing `junifer-0.0.3.dev75/junifer/utils/tests/test_fs.py` & `junifer-0.0.3.dev89/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/junifer/utils/tests/test_logging.py` & `junifer-0.0.3.dev89/junifer/utils/tests/test_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,16 @@
     """Test logging versions.
 
     tmp_path : Path
         The path to the test directory.
 
     """
     # Import third-party packages
-    import numpy as np  # noqa
-    import pandas  # noqa
+    import numpy  # noqa: F401
+    import pandas  # noqa: F401
 
     log_file_path = tmp_path / "test_lib_logging.log"
     configure_logging(fname=log_file_path, level="INFO")
     logger.info("first message")
     with open(log_file_path) as f:
         lines = f.readlines()
         assert any("numpy" in line for line in lines)
```

### Comparing `junifer-0.0.3.dev75/junifer.egg-info/PKG-INFO` & `junifer-0.0.3.dev89/junifer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev75
+Version: 0.0.3.dev89
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -36,14 +36,15 @@
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
```

### Comparing `junifer-0.0.3.dev75/junifer.egg-info/SOURCES.txt` & `junifer-0.0.3.dev89/junifer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 docs/changes/newsfragments/222.change
 docs/changes/newsfragments/222.enh
 docs/changes/newsfragments/223.bugfix
 docs/changes/newsfragments/223.enh
 docs/changes/newsfragments/226.enh
 docs/changes/newsfragments/227.enh
 docs/changes/newsfragments/228.misc
+docs/changes/newsfragments/229.misc
 docs/changes/newsfragments/230.misc
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
```

### Comparing `junifer-0.0.3.dev75/pyproject.toml` & `junifer-0.0.3.dev89/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 [project]
 name = "junifer"
 description = "JUelich NeuroImaging FEature extractoR"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "AGPL-3.0-only"}
 authors = [
-    {name = "Fede Raimondo", email = "f.raimondo@fz-juelich.de"},
-    {name = "Synchon Mandal", email = "s.mandal@fz-juelich.de"},
+    { name = "Fede Raimondo", email = "f.raimondo@fz-juelich.de" },
+    { name = "Synchon Mandal", email = "s.mandal@fz-juelich.de" },
 ]
 maintainers = [
-    {name = "Fede Raimondo", email = "f.raimondo@fz-juelich.de"},
-    {name = "Synchon Mandal", email = "s.mandal@fz-juelich.de"},
+    { name = "Fede Raimondo", email = "f.raimondo@fz-juelich.de" },
+    { name = "Synchon Mandal", email = "s.mandal@fz-juelich.de" },
 ]
 keywords = [
     "neuroimaging",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -84,29 +84,110 @@
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
 write_to = "junifer/_version.py"
 
 [tool.black]
 line-length = 79
-target-version = ["py38"]
+target-version = ["py38", "py39", "py310", "py311"]
 extend-exclude = """
 (
   junifer/external/h5io
 )
 """
 
 [tool.codespell]
 skip = "*/auto_examples/*,*.html,.git/,*.pyc,*/_build/*,*/h5io/*"
 count = ""
 quiet-level = 3
 ignore-words = "ignore_words.txt"
 interactive = 0
 builtin = "clear,rare,informal,names,usage,code"
 
+[tool.ruff]
+line-length = 79
+select = [
+    # flake8-bugbear
+    "B",
+    # flake8-blind-except
+    "BLE",
+    # flake8-comprehensions
+    "C4",
+    # mccabe
+    "C90",
+    # pydocstyle
+    "D",
+    # pycodestyle errors
+    "E",
+    # pyflakes
+    "F",
+    # isort
+    "I",
+    # pep8-naming
+    "N",
+    # pygrep-hooks
+    "PGH",
+    # ruff
+    "RUF",
+    # flake8-type-checking
+    "TCH",
+    # pyupgrade
+    "UP",
+    # pycodestyle warnings
+    "W",
+    # flake8-2020
+    "YTT",
+]
+extend-exclude = [
+    "__init__.py",
+    "junifer/external/h5io",
+    "docs",
+    "examples",
+    "tools",
+]
+extend-ignore = [
+    # Use of `functools.lru_cache` or `functools.cache` on methods can lead to
+    # memory leaks. The cache may retain instance references, preventing garbage
+    # collection.
+    "B019",
+    # abstract class with no abstract methods
+    "B024",
+    "D202",
+    # missing docstring in __init__, incompatible with numpydoc
+    "D107",
+    # use r""" if any backslashes in a docstring
+    "D301",
+    # class names should use CapWords convention
+    "N801",
+    # function name should be lowercase
+    "N802",
+    # variable in function should be lowercase
+    "N806",
+    # use specific rule codes when ignoring type issues
+    "PGH003",
+]
+
+[tool.ruff.isort]
+lines-after-imports = 2
+known-first-party = ["junifer"]
+known-third-party =[
+    "click",
+    "numpy",
+    "datalad",
+    "pandas",
+    "nibabel",
+    "nilearn",
+    "sqlalchemy",
+    "yaml",
+    "pytest",
+]
+
+[tool.ruff.mccabe]
+max-complexity = 20
+
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "--ignore=junifer/external/h5io -vv"
 
 [tool.towncrier]
 directory = "docs/changes/newsfragments"
 filename = "docs/whats_new.rst"
```

### Comparing `junifer-0.0.3.dev75/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.3.dev89/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.3.dev89/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.3.dev89/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/tools/create_bids_example_dataset.py` & `junifer-0.0.3.dev89/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.3.dev89/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev75/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.3.dev89/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

