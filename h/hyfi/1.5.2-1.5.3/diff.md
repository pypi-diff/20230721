# Comparing `tmp/hyfi-1.5.2.tar.gz` & `tmp/hyfi-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.5.2.tar", max compression
+gzip compressed data, was "hyfi-1.5.3.tar", max compression
```

## Comparing `hyfi-1.5.2.tar` & `hyfi-1.5.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1071 2023-07-21 20:18:20.948999 hyfi-1.5.2/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-21 20:18:20.948999 hyfi-1.5.2/README.md
--rw-r--r--   0        0        0     4928 2023-07-21 20:18:49.697538 hyfi-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2793 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 20:18:49.617536 hyfi-1.5.2/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24426 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-21 20:18:49.617536 hyfi-1.5.2/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-21 20:18:20.952999 hyfi-1.5.2/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      864 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18852 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-21 20:18:20.956999 hyfi-1.5.2/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 20:56:29.475244 hyfi-1.5.3/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 20:56:29.475244 hyfi-1.5.3/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 20:56:55.783770 hyfi-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 20:56:55.703768 hyfi-1.5.3/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24378 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 20:56:55.703768 hyfi-1.5.3/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      865 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3480 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18823 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.3/PKG-INFO
```

### Comparing `hyfi-1.5.2/LICENSE` & `hyfi-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/README.md` & `hyfi-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/pyproject.toml` & `hyfi-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.5.2"
+version = "1.5.3"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.5.2/src/hyfi/__cli__.py` & `hyfi-1.5.3/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/__click__.py` & `hyfi-1.5.3/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/__init__.py` & `hyfi-1.5.3/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/about/__init__.py` & `hyfi-1.5.3/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/batch/__init__.py` & `hyfi-1.5.3/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/__init__.py` & `hyfi-1.5.3/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.5.3/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/cache_file.py` & `hyfi-1.5.3/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/common.py` & `hyfi-1.5.3/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/file_lock.py` & `hyfi-1.5.3/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/meta.py` & `hyfi-1.5.3/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/progress.py` & `hyfi-1.5.3/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.5.3/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.5.3/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.5.3/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.5.3/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.5.3/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/testing.py` & `hyfi-1.5.3/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/cached_path/util.py` & `hyfi-1.5.3/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/composer/__init__.py` & `hyfi-1.5.3/src/hyfi/composer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 
 
 class Composer(BaseModel, CONFs):
     """
     Compose a configuration by applying overrides
     """
 
-    config_group: Union[str, None] = None
-    overrides: Union[List[str], None] = None
-    config_data: Union[Dict[str, Any], DictConfig, None] = None
+    config_group: Optional[str] = None
+    overrides: Optional[List[str]] = None
+    config_data: Optional[Union[Dict[str, Any], DictConfig]] = None
     throw_on_resolution_failure: bool = True
     throw_on_missing: bool = False
-    config_name: Union[str, None] = None
-    config_module: Union[str, None] = None
+    config_name: Optional[str] = None
+    config_module: Optional[str] = None
     global_package: bool = False
     verbose: bool = False
 
     _cfg_: DictConfig = PrivateAttr({})
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
@@ -84,22 +84,22 @@
             config_module=self.config_module,
             global_package=self.global_package,
             verbose=self.verbose,
         )
 
     def compose(
         self,
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         """
         Compose a configuration by applying overrides
 
         Args:
@@ -144,22 +144,22 @@
         """
         Return the configuration as a dictionary.
         """
         return Composer.to_dict(self._cfg_)
 
     def __call__(
         self,
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         return self.compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
@@ -197,17 +197,17 @@
         return hash(self._cfg_)
 
     def __getstate__(self):
         return self._cfg_
 
     @staticmethod
     def hydra_compose(
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
     ):
         is_initialized = GlobalHydra.instance().is_initialized()  # type: ignore
         config_module = config_module or __hydra_config__.hyfi_config_module
         logger.debug("config_module: %s", config_module)
         if is_initialized:
             # Hydra is already initialized.
             logger.debug("Hydra is already initialized")
@@ -219,15 +219,15 @@
                 version_base=__hydra_version_base__,
             ):
                 cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         return cfg
 
     @staticmethod
     def split_config_group(
-        config_group: Union[str, None] = None,
+        config_group: Optional[str] = None,
     ) -> Tuple[str, str, str]:
         if config_group:
             group_ = config_group.split("=")
             # group_key group_value group_key group_value group_key group_value default
             if len(group_) == 2:
                 group_key, group_value = group_
             else:
@@ -238,22 +238,22 @@
             group_key = ""
             group_value = ""
             config_group = ""
         return config_group, group_key, group_value
 
     @staticmethod
     def _compose_as_dict(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         **kwargs,
     ) -> Dict:
         return Composer.to_dict(
             Composer._compose(
                 config_group=config_group,
                 overrides=overrides,
@@ -582,17 +582,17 @@
             obj: The object to print the source code of.
 
         """
         print(Composer.getsource(obj))
 
     @staticmethod
     def instantiate_config(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         global_package: bool = False,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
         """
         Instantiates an object using the provided config group and overrides.
 
@@ -618,17 +618,17 @@
             config_data=config_data,
             global_package=global_package,
         )
         return Composer.instantiate(cfg, *args, **kwargs)
 
     @staticmethod
     def print_config(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         global_package: bool = False,
     ):
         """
         Print the configuration
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
```

### Comparing `hyfi-1.5.2/src/hyfi/composer/base.py` & `hyfi-1.5.3/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/composer/pydantic.py` & `hyfi-1.5.3/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.5.3/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.5.3/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/copier/__init__.py` & `hyfi-1.5.3/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/core/__init__.py` & `hyfi-1.5.3/src/hyfi/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from hyfi.about import AboutConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
-__hydra_default_config_group_value__ = "default"
+__hydra_default_config_group_value__ = "__init__"
 __config_path__ = "conf"
 __config_name__ = "config"
 
 __about__ = AboutConfig()
 _batcher_instance_ = None
```

### Comparing `hyfi-1.5.2/src/hyfi/core/config.py` & `hyfi-1.5.3/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/core/hydra.py` & `hyfi-1.5.3/src/hyfi/core/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/dotenv/__init__.py` & `hyfi-1.5.3/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/graphics/__init__.py` & `hyfi-1.5.3/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/graphics/collage.py` & `hyfi-1.5.3/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/graphics/motion.py` & `hyfi-1.5.3/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/graphics/utils.py` & `hyfi-1.5.3/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/joblib/__init__.py` & `hyfi-1.5.3/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/joblib/batch/apply.py` & `hyfi-1.5.3/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.5.3/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.5.3/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/main/__init__.py` & `hyfi-1.5.3/src/hyfi/main/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,37 +267,37 @@
         wf = WorkflowConfig(**cfg)
         if __global_config__.project:
             wf.project = __global_config__.project
         return wf
 
     @staticmethod
     def compose_as_dict(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> Dict:
         """
         Compose a configuration by applying overrides and return the result as a dict(
 
         Args:
-            config_group (Union[str, None], optional): Name of the config group to compose (`config_group=name`). Defaults to None.
+            config_group (Optional[str], optional): Name of the config group to compose (`config_group=name`). Defaults to None.
             overrides (Union[List[str], None], optional): List of config groups to apply overrides to (`overrides=["override_name"]`). Defaults to None.
             config_data (Union[Dict[str, Any], DictConfig, None], optional): Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`). Defaults to None.
             throw_on_compose_failure (bool, optional): If True throw an exception if composition fails. Defaults to True.
             throw_on_resolution_failure (bool, optional): If True throw an exception if resolution fails. Defaults to True.
             throw_on_missing (bool, optional): If True throw an exception if config_group doesn't exist. Defaults to False.
-            root_config_name (Union[str, None], optional): Name of the root config to be used (e.g. `hconf`). Defaults to None.
-            config_module (Union[str, None], optional): Name of the module containing the configuration. Defaults to None.
+            root_config_name (Optional[str], optional): Name of the root config to be used (e.g. `hconf`). Defaults to None.
+            config_module (Optional[str], optional): Name of the module containing the configuration. Defaults to None.
             global_package (bool, optional): If True, the configuration is loaded from the global package. Defaults to False.
             verbose (bool, optional): If True, print verbose output. Defaults to False.
 
         Returns:
             Dict: The composed configuration as a dictionary.
         """
         return Composer._compose_as_dict(
@@ -311,22 +311,22 @@
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
     def compose(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         throw_on_compose_failure: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        root_config_name: Union[str, None] = None,
-        config_module: Union[str, None] = None,
+        root_config_name: Optional[str] = None,
+        config_module: Optional[str] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         """
         Compose a configuration by applying overrides
 
         Args:
@@ -356,17 +356,17 @@
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
     def instantiate_config(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         global_package: bool = False,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
         """
         Instantiates an object using the provided config group and overrides
 
@@ -393,17 +393,17 @@
             global_package=global_package,
             *args,
             **kwargs,
         )
 
     @staticmethod
     def print_config(
-        config_group: Union[str, None] = None,
-        overrides: Union[List[str], None] = None,
-        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config_data: Optional[Union[Dict[str, Any], DictConfig]] = None,
         global_package: bool = False,
     ):
         """
         Print the configuration
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
```

### Comparing `hyfi-1.5.2/src/hyfi/path/__init__.py` & `hyfi-1.5.3/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/path/base.py` & `hyfi-1.5.3/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/path/batch.py` & `hyfi-1.5.3/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/path/dirnames.py` & `hyfi-1.5.3/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/path/task.py` & `hyfi-1.5.3/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/pipe/__init__.py` & `hyfi-1.5.3/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/pipe/test.py` & `hyfi-1.5.3/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/pipeline/__init__.py` & `hyfi-1.5.3/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/pipeline/configs.py` & `hyfi-1.5.3/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/project/__init__.py` & `hyfi-1.5.3/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/task/__init__.py` & `hyfi-1.5.3/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/task/batch.py` & `hyfi-1.5.3/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/conf.py` & `hyfi-1.5.3/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/contexts.py` & `hyfi-1.5.3/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/datasets.py` & `hyfi-1.5.3/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/envs.py` & `hyfi-1.5.3/src/hyfi/utils/envs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Environment variable utilities"""
 import os
 import sys
 from collections import defaultdict
 from pathlib import Path
 from string import Template
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional
 
 import dotenv
 import hydra
 
 from hyfi.utils.iolibs import IOLIBs
 from hyfi.utils.logging import LOGGING
 
@@ -205,15 +205,15 @@
             raise_error_if_not_found=raise_error_if_not_found,
             usecwd=usecwd,
         ):
             return os.path.dirname(dotenv_path)
         return ""
 
     @staticmethod
-    def get_osenv(key: str = "", default: Union[str, None] = None) -> Any:
+    def get_osenv(key: str = "", default: Optional[str] = None) -> Any:
         """Get the value of an environment variable or return the default value"""
         ENVs.load_dotenv()
         return os.environ.get(key, default) if key else os.environ
 
     @staticmethod
     def set_osenv(key: str, value: Any) -> None:
         """Set the value of an environment variable"""
```

### Comparing `hyfi-1.5.2/src/hyfi/utils/funcs.py` & `hyfi-1.5.3/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/gpumon.py` & `hyfi-1.5.3/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/iolibs.py` & `hyfi-1.5.3/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/logging.py` & `hyfi-1.5.3/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/notebooks.py` & `hyfi-1.5.3/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/utils/packages.py` & `hyfi-1.5.3/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/src/hyfi/workflow/__init__.py` & `hyfi-1.5.3/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.2/PKG-INFO` & `hyfi-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.5.2
+Version: 1.5.3
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

