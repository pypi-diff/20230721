# Comparing `tmp/hyfi-1.5.1.tar.gz` & `tmp/hyfi-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.5.1.tar", max compression
+gzip compressed data, was "hyfi-1.5.2.tar", max compression
```

## Comparing `hyfi-1.5.1.tar` & `hyfi-1.5.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1071 2023-07-21 19:37:55.076695 hyfi-1.5.1/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-21 19:37:55.076695 hyfi-1.5.1/README.md
--rw-r--r--   0        0        0     4928 2023-07-21 19:38:32.661233 hyfi-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2793 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 19:38:32.553231 hyfi-1.5.1/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    22037 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7248 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-21 19:38:32.553231 hyfi-1.5.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      864 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18424 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 20:18:20.948999 hyfi-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 20:18:20.948999 hyfi-1.5.2/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 20:18:49.697538 hyfi-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 20:18:49.617536 hyfi-1.5.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24426 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 20:18:49.617536 hyfi-1.5.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3480 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18852 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.2/PKG-INFO
```

### Comparing `hyfi-1.5.1/LICENSE` & `hyfi-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/README.md` & `hyfi-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/pyproject.toml` & `hyfi-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.5.1"
+version = "1.5.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.5.1/src/hyfi/__cli__.py` & `hyfi-1.5.2/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/__click__.py` & `hyfi-1.5.2/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/__init__.py` & `hyfi-1.5.2/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/about/__init__.py` & `hyfi-1.5.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/batch/__init__.py` & `hyfi-1.5.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/__init__.py` & `hyfi-1.5.2/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.5.2/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/cache_file.py` & `hyfi-1.5.2/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/common.py` & `hyfi-1.5.2/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/file_lock.py` & `hyfi-1.5.2/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/meta.py` & `hyfi-1.5.2/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/progress.py` & `hyfi-1.5.2/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.5.2/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.5.2/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.5.2/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.5.2/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.5.2/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/testing.py` & `hyfi-1.5.2/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/cached_path/util.py` & `hyfi-1.5.2/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/composer/__init__.py` & `hyfi-1.5.2/src/hyfi/composer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Hydra configuration management
 """
 import collections.abc
 import os
 import re
 from enum import Enum
-from typing import Any, Callable, Dict, List, Mapping, Set, Tuple, Union
+from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 import hydra
 from hydra.core.global_hydra import GlobalHydra
 from omegaconf import DictConfig
 from pydantic import BaseModel, ConfigDict, PrivateAttr
 
 from hyfi.core import (
@@ -87,14 +87,15 @@
         )
 
     def compose(
         self,
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
@@ -102,28 +103,30 @@
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
             config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group.key=value`)
             return_as_dict: Return the result as a dict
+            throw_on_compose_failure: If True throw an exception if composition fails
             throw_on_resolution_failure: If True throw an exception if resolution fails
             throw_on_missing: If True throw an exception if config_group doesn't exist
             root_config_name: Name of the root config to be used (e.g. `hconf`)
             config_module: Module of the config to be used (e.g. `hyfi.conf`)
             global_package: If True, the config assumed to be a global package
             verbose: If True print configuration to stdout
 
         Returns:
             A config object or a dictionary with the composed config
         """
         self._cfg_ = Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
+            throw_on_compose_failure=throw_on_compose_failure,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             root_config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
@@ -144,25 +147,27 @@
         return Composer.to_dict(self._cfg_)
 
     def __call__(
         self,
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         return self.compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
+            throw_on_compose_failure=throw_on_compose_failure,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             root_config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
@@ -236,49 +241,82 @@
         return config_group, group_key, group_value
 
     @staticmethod
     def _compose_as_dict(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         **kwargs,
     ) -> Dict:
         return Composer.to_dict(
             Composer._compose(
                 config_group=config_group,
                 overrides=overrides,
                 config_data=config_data,
+                throw_on_compose_failure=throw_on_compose_failure,
                 throw_on_resolution_failure=throw_on_resolution_failure,
                 throw_on_missing=throw_on_missing,
                 root_config_name=root_config_name,
                 config_module=config_module,
                 global_package=global_package,
                 **kwargs,
             )
         )
 
     @staticmethod
     def _compose(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
+        global_package: bool = False,
+        **kwargs,
+    ) -> DictConfig:
+        try:
+            return Composer._compose_internal(
+                config_group=config_group,
+                overrides=overrides,
+                config_data=config_data,
+                throw_on_resolution_failure=throw_on_resolution_failure,
+                throw_on_missing=throw_on_missing,
+                root_config_name=root_config_name,
+                config_module=config_module,
+                global_package=global_package,
+                **kwargs,
+            )
+        except Exception as e:
+            logger.error("Error composing config: %s", e)
+            if throw_on_compose_failure:
+                raise e
+            return DictConfig(config_data) if config_data else DictConfig({})
+
+    @staticmethod
+    def _compose_internal(
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
+        throw_on_resolution_failure: bool = True,
+        throw_on_missing: bool = False,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         **kwargs,
     ) -> DictConfig:
         if isinstance(config_data, DictConfig):
-            logger.debug("returning config_group_kwargs without composing")
+            logger.debug("returning config_data without composing")
             return config_data
         # Set overrides to the empty list if None
         if overrides is None:
             overrides = []
         # Set the group key and value of the config group.
         config_group, group_key, group_value = Composer.split_config_group(config_group)
         if group_key in __global_package_list__:
@@ -301,15 +339,15 @@
             override = config_group if cfg is not None else f"+{config_group}"
             # Add override to overrides list.
             if isinstance(override, str):
                 if overrides:
                     overrides.append(override)
                 else:
                     overrides = [override]
-        # if verbose:
+
         logger.debug(f"compose config with overrides: {overrides}")
         # Initialize hydra and return the configuration.
         cfg = Composer.hydra_compose(
             root_config_name=root_config_name,
             config_module=config_module,
             overrides=overrides,
         )
@@ -341,18 +379,42 @@
             cfg = Composer.select(
                 cfg,
                 key=group_key,
                 default=None,
                 throw_on_missing=throw_on_missing,
                 throw_on_resolution_failure=throw_on_resolution_failure,
             )
-        # logger.debug("Composed config: %s", OmegaConf.to_yaml(_to_dict(cfg)))
         return cfg
 
     @staticmethod
+    def is_composable(
+        config_group: str,
+        config_module: Optional[str] = None,
+    ) -> bool:
+        """
+        Determines whether the input configuration object is composable.
+
+        Args:
+            config_group (str): The name of the configuration group to check.
+            config_module (Optional[str], optional): The name of the configuration module to check. Defaults to None.
+
+        Returns:
+            bool: True if the configuration object is composable, False otherwise.
+        """
+        try:
+            cfg = Composer._compose(
+                config_group=config_group,
+                config_module=config_module,
+            )
+            return cfg is not None
+        except Exception as e:
+            logger.error("Error composing config: %s", e)
+            return False
+
+    @staticmethod
     def is_instantiatable(cfg: Any):
         """
         Determines whether the input configuration object is instantiatable.
 
         Args:
             cfg (Any): The configuration object to check.
```

### Comparing `hyfi-1.5.1/src/hyfi/composer/base.py` & `hyfi-1.5.2/src/hyfi/composer/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,19 @@
         # Initialize the config with the given config_name.
         logger.info(
             "Composing `%s` class with `%s` config in `%s` group.",
             _class_name_,
             _config_name_,
             _config_group_,
         )
+        config_group = f"{_config_group_}={_config_name_}"
         cfg = Composer(
-            config_group=f"{_config_group_}={_config_name_}",
+            config_group=config_group,
             config_data=data,
+            throw_on_compose_failure=False,
         ).config_as_dict
         data = Composer.update(cfg, data)
         # Exclude any attributes specified in the class's `exclude` list.
         exclude = getattr(cls._exclude_, "default", set())  # type: ignore
         for name in exclude:
             if name in data:
                 del data[name]  # type: ignore
```

### Comparing `hyfi-1.5.1/src/hyfi/composer/pydantic.py` & `hyfi-1.5.2/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.5.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.5.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/copier/__init__.py` & `hyfi-1.5.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/core/__init__.py` & `hyfi-1.5.2/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/core/config.py` & `hyfi-1.5.2/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/core/hydra.py` & `hyfi-1.5.2/src/hyfi/core/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/dotenv/__init__.py` & `hyfi-1.5.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/graphics/__init__.py` & `hyfi-1.5.2/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/graphics/collage.py` & `hyfi-1.5.2/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/graphics/motion.py` & `hyfi-1.5.2/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/graphics/utils.py` & `hyfi-1.5.2/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/joblib/__init__.py` & `hyfi-1.5.2/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/joblib/batch/apply.py` & `hyfi-1.5.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.5.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.5.2/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/main/__init__.py` & `hyfi-1.5.2/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,55 +270,59 @@
         return wf
 
     @staticmethod
     def compose_as_dict(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> Dict:
         """
         Compose a configuration by applying overrides and return the result as a dict(
 
         Args:
             config_group (Union[str, None], optional): Name of the config group to compose (`config_group=name`). Defaults to None.
             overrides (Union[List[str], None], optional): List of config groups to apply overrides to (`overrides=["override_name"]`). Defaults to None.
             config_data (Union[Dict[str, Any], DictConfig, None], optional): Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`). Defaults to None.
+            throw_on_compose_failure (bool, optional): If True throw an exception if composition fails. Defaults to True.
             throw_on_resolution_failure (bool, optional): If True throw an exception if resolution fails. Defaults to True.
             throw_on_missing (bool, optional): If True throw an exception if config_group doesn't exist. Defaults to False.
             root_config_name (Union[str, None], optional): Name of the root config to be used (e.g. `hconf`). Defaults to None.
             config_module (Union[str, None], optional): Name of the module containing the configuration. Defaults to None.
             global_package (bool, optional): If True, the configuration is loaded from the global package. Defaults to False.
             verbose (bool, optional): If True, print verbose output. Defaults to False.
 
         Returns:
             Dict: The composed configuration as a dictionary.
         """
         return Composer._compose_as_dict(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
+            throw_on_compose_failure=throw_on_compose_failure,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
     def compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
@@ -326,28 +330,30 @@
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
             config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
             return_as_dict: Return the result as a dict
+            throw_on_compose_failure: If True throw an exception if composition fails
             throw_on_resolution_failure: If True throw an exception if resolution fails
             throw_on_missing: If True throw an exception if config_group doesn't exist
             root_config_name: Name of the root config to be used (e.g. `hconf`)
             config_module: Module of the config to be used (e.g. `hyfi.conf`)
             global_package: If True, the config assumed to be a global package
             verbose: If True print configuration to stdout
 
         Returns:
             A config object or a dictionary with the composed config
         """
         return Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
+            throw_on_compose_failure=throw_on_compose_failure,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
```

### Comparing `hyfi-1.5.1/src/hyfi/path/__init__.py` & `hyfi-1.5.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/path/base.py` & `hyfi-1.5.2/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/path/batch.py` & `hyfi-1.5.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/path/dirnames.py` & `hyfi-1.5.2/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/path/task.py` & `hyfi-1.5.2/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/pipe/__init__.py` & `hyfi-1.5.2/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/pipe/test.py` & `hyfi-1.5.2/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/pipeline/__init__.py` & `hyfi-1.5.2/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/pipeline/configs.py` & `hyfi-1.5.2/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/project/__init__.py` & `hyfi-1.5.2/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/task/__init__.py` & `hyfi-1.5.2/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/task/batch.py` & `hyfi-1.5.2/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/conf.py` & `hyfi-1.5.2/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/contexts.py` & `hyfi-1.5.2/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/datasets.py` & `hyfi-1.5.2/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/envs.py` & `hyfi-1.5.2/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/funcs.py` & `hyfi-1.5.2/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/gpumon.py` & `hyfi-1.5.2/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/iolibs.py` & `hyfi-1.5.2/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/logging.py` & `hyfi-1.5.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/notebooks.py` & `hyfi-1.5.2/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/utils/packages.py` & `hyfi-1.5.2/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/src/hyfi/workflow/__init__.py` & `hyfi-1.5.2/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.1/PKG-INFO` & `hyfi-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.5.1
+Version: 1.5.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

