# Comparing `tmp/hyfi-1.5.0.tar.gz` & `tmp/hyfi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.5.0.tar", max compression
+gzip compressed data, was "hyfi-1.5.1.tar", max compression
```

## Comparing `hyfi-1.5.0.tar` & `hyfi-1.5.1.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0     1071 2023-07-21 07:33:23.773884 hyfi-1.5.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-21 07:33:23.773884 hyfi-1.5.0/README.md
--rw-r--r--   0        0        0     4928 2023-07-21 07:33:59.785934 hyfi-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2793 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 07:33:59.681934 hyfi-1.5.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7287 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    29019 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-21 07:33:59.681934 hyfi-1.5.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      864 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4204 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18424 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4354 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5849 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     3626 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 19:37:55.076695 hyfi-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 19:37:55.076695 hyfi-1.5.1/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 19:38:32.661233 hyfi-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:38:32.553231 hyfi-1.5.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    22037 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7248 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 19:37:55.084695 hyfi-1.5.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 19:38:32.553231 hyfi-1.5.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3480 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18424 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 19:37:55.088695 hyfi-1.5.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 19:37:55.092695 hyfi-1.5.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.1/PKG-INFO
```

### Comparing `hyfi-1.5.0/LICENSE` & `hyfi-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/README.md` & `hyfi-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/pyproject.toml` & `hyfi-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.5.0"
+version = "1.5.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.5.0/src/hyfi/__cli__.py` & `hyfi-1.5.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/__click__.py` & `hyfi-1.5.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/__init__.py` & `hyfi-1.5.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/about/__init__.py` & `hyfi-1.5.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/batch/__init__.py` & `hyfi-1.5.1/src/hyfi/batch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 import random
 from pathlib import Path
 from typing import Optional
 
 from pydantic import FieldValidationInfo, field_validator
 
-from hyfi.composer import BaseConfig
+from hyfi.composer.base import BaseConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 class BatchConfig(BaseConfig):
     """
```

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.5.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.5.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.5.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/common.py` & `hyfi-1.5.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.5.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/meta.py` & `hyfi-1.5.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/progress.py` & `hyfi-1.5.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.5.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.5.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.5.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.5.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.5.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/testing.py` & `hyfi-1.5.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/cached_path/util.py` & `hyfi-1.5.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/composer/__init__.py` & `hyfi-1.5.1/src/hyfi/composer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
     Hydra configuration management
 """
 import collections.abc
 import os
 import re
 from enum import Enum
-from pathlib import Path
-from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union
+from typing import Any, Callable, Dict, List, Mapping, Set, Tuple, Union
 
 import hydra
 from hydra.core.global_hydra import GlobalHydra
 from omegaconf import DictConfig
-from pydantic import BaseModel, ConfigDict, PrivateAttr, model_validator
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 
 from hyfi.core import (
     __about__,
     __hydra_config__,
     __hydra_default_config_group_value__,
     __hydra_version_base__,
 )
@@ -578,192 +577,7 @@
         cfg = Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
             global_package=global_package,
         )
         Composer.print(cfg)
-
-
-class BaseConfig(BaseModel):
-    """
-    Base class for all config classes.
-    """
-
-    _config_name_: str = "__init__"
-    _config_group_: str = ""
-    verbose: bool = False
-
-    _init_args_: Dict[str, Any] = {}
-    _exclude_: Set[str] = set()
-    _property_set_methods_: Dict[str, str] = {}
-    _subconfigs_: Dict[str, Any] = {}
-
-    model_config = ConfigDict(
-        arbitrary_types_allowed=True,
-        extra="allow",
-        validate_assignment=False,
-    )  # type: ignore
-
-    def __init__(self, **config_kwargs):
-        logger.debug(
-            "init %s with %s args", self.__class__.__name__, len(config_kwargs)
-        )
-        super().__init__(**config_kwargs)
-        self.initialize_subconfigs(config_kwargs)
-
-    def __setattr__(self, key, val):
-        """
-        Overrides the default __setattr__ method to allow for custom property set methods.
-
-        Args:
-            key (str): The name of the attribute to set.
-            val (Any): The value to set the attribute to.
-        """
-        if method := self._property_set_methods_.get(key):  # type: ignore
-            logger.info(
-                "Setting %s to %s",
-                key,
-                val if isinstance(val, (str, int)) else type(val),
-            )
-            getattr(self, method)(val)
-        super().__setattr__(key, val)
-
-    @model_validator(mode="before")
-    def validate_model_config_before(cls, data):
-        # logger.debug("Validating model config before validating each field.")
-        _config_name_ = data.get("_config_name_", getattr(cls._config_name_, "default", "__init__"))  # type: ignore
-        _config_group_ = data.get("_config_group_", getattr(cls._config_group_, "default"))  # type: ignore
-        _class_name_ = cls.__name__  # type: ignore
-        if not _config_group_:
-            logger.debug("There is no config group specified.")
-            return data
-        # Initialize the config with the given config_name.
-        logger.info(
-            "Composing `%s` class with `%s` config in `%s` group.",
-            _class_name_,
-            _config_name_,
-            _config_group_,
-        )
-        cfg = Composer(
-            config_group=f"{_config_group_}={_config_name_}",
-            config_data=data,
-        ).config_as_dict
-        data = Composer.update(cfg, data)
-        # Exclude any attributes specified in the class's `exclude` list.
-        exclude = getattr(cls._exclude_, "default", set())  # type: ignore
-        for name in exclude:
-            if name in data:
-                del data[name]  # type: ignore
-        return data
-
-    # @model_validator(mode="after")  # type: ignore
-    # def validate_model_config_after(cls, model):
-    #     logger.debug("validate_model_config_after")
-    #     return model
-
-    def initialize_subconfigs(self, config_kwargs: Dict[str, Any]):
-        """
-        Initializes subconfigs with the given config data.
-        The function updates the object's dictionary with the given config data,
-        after excluding any attributes specified in the object's `exclude` list.
-
-        Args:
-            config_kwargs (Dict[str, Any]): The config data to initialize the subconfigs with.
-
-        Returns:
-            None
-        """
-        self._subconfigs_ = self._subconfigs_ or {}
-        for name, config in self._subconfigs_.items():
-            if name in config_kwargs and isinstance(config_kwargs[name], dict):
-                cfg = config_kwargs[name]
-                logger.debug("Initializing subconfig %s with %s", name, cfg)
-                setattr(self, name, config.model_validate(cfg))
-
-    def export_config(
-        self,
-        exclude: Optional[Union[str, List[str], Set[str], None]] = None,
-        exclude_none: bool = True,
-        only_include: Optional[Union[str, List[str], Set[str], None]] = None,
-    ) -> Dict[str, Any]:
-        """
-        Export the configuration to a dictionary.
-
-        Args:
-            exclude (Optional[Union[str, List[str], Set[str], None]]): Keys to exclude from the saved configuration.
-                Defaults to None.
-            exclude_none (bool): Whether to exclude keys with None values. Defaults to True.
-            only_include (Optional[Union[str, List[str], Set[str], None]]): Keys to include in the saved configuration.
-                Defaults to None.
-
-        Returns:
-            Dict[str, Any]: The configuration dictionary.
-        """
-        if not exclude:
-            exclude = self._exclude_  # type: ignore
-        if isinstance(exclude, str):
-            exclude = [exclude]
-        if exclude is None:
-            exclude = []
-        if isinstance(only_include, str):
-            only_include = [only_include]
-        if only_include is None:
-            only_include = []
-
-        config = self.model_dump(exclude=exclude, exclude_none=exclude_none)  # type: ignore
-        if only_include:
-            config = {key: config[key] for key in only_include if key in config}
-
-        return config
-
-    def save_config(
-        self,
-        filepath: Union[str, Path],
-        exclude: Optional[Union[str, List[str], Set[str], None]] = None,
-        exclude_none: bool = True,
-        only_include: Optional[Union[str, List[str], Set[str], None]] = None,
-    ) -> str:
-        """
-        Save the batch configuration to file.
-
-        Args:
-            filepath ([Union[str, Path]): The filepath to save the configuration to.
-            exclude (Optional[Union[str, List[str], Set[str], None]]): Keys to exclude from the saved configuration.
-                Defaults to None.
-            exclude_none (bool): Whether to exclude keys with None values. Defaults to True.
-            only_include (Optional[Union[str, List[str], Set[str], None]]): Keys to include in the saved configuration.
-                Defaults to None.
-
-        Returns:
-            str: The filename of the saved configuration.
-        """
-        logger.info("Saving config to %s", filepath)
-
-        config_to_save = self.export_config(
-            exclude=exclude, exclude_none=exclude_none, only_include=only_include
-        )
-
-        Composer.save(config_to_save, filepath)
-        return str(filepath)
-
-    def save_config_as_json(
-        self,
-        filepath: Union[str, Path],
-        exclude: Optional[Union[str, List[str], Set[str], None]] = None,
-        exclude_none: bool = True,
-        only_include: Optional[Union[str, List[str], Set[str], None]] = None,
-    ) -> str:
-        def dumper(obj):
-            return Composer.to_dict(obj) if isinstance(obj, DictConfig) else str(obj)
-
-        config_to_save = self.export_config(
-            exclude=exclude, exclude_none=exclude_none, only_include=only_include
-        )
-        logger.info("Saving config to %s", filepath)
-        Composer.save_json(config_to_save, filepath, default=dumper)
-        return str(filepath)
-
-    def print_config(
-        self,
-    ):
-        Composer.print(self.model_dump())
```

### Comparing `hyfi-1.5.0/src/hyfi/composer/pydantic.py` & `hyfi-1.5.1/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.5.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.5.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/copier/__init__.py` & `hyfi-1.5.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/core/__init__.py` & `hyfi-1.5.1/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/core/config.py` & `hyfi-1.5.1/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/core/hydra.py` & `hyfi-1.5.1/src/hyfi/core/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.5.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/graphics/__init__.py` & `hyfi-1.5.1/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/graphics/collage.py` & `hyfi-1.5.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/graphics/motion.py` & `hyfi-1.5.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/graphics/utils.py` & `hyfi-1.5.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/joblib/__init__.py` & `hyfi-1.5.1/src/hyfi/joblib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 from pydantic import PrivateAttr
 from tqdm.auto import tqdm
 
 from hyfi import core
-from hyfi.composer import BaseConfig
+from hyfi.composer.base import BaseConfig
 from hyfi.joblib.batch import batcher
 from hyfi.joblib.batch.apply import decorator_apply
 from hyfi.joblib.batch.batcher import Batcher
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
```

### Comparing `hyfi-1.5.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.5.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.5.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.5.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/main/__init__.py` & `hyfi-1.5.1/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/path/__init__.py` & `hyfi-1.5.1/src/hyfi/path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from hyfi.composer import BaseConfig
+from hyfi.composer.base import BaseConfig
 from hyfi.core import __about__
 from hyfi.path.base import BasePathConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
```

### Comparing `hyfi-1.5.0/src/hyfi/path/base.py` & `hyfi-1.5.1/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/path/batch.py` & `hyfi-1.5.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/path/dirnames.py` & `hyfi-1.5.1/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/path/task.py` & `hyfi-1.5.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/pipe/__init__.py` & `hyfi-1.5.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/pipe/test.py` & `hyfi-1.5.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.5.1/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/pipeline/configs.py` & `hyfi-1.5.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/project/__init__.py` & `hyfi-1.5.1/src/hyfi/project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 from typing import Union
 
 from pydantic import field_validator
 
-from hyfi.composer import BaseConfig
+from hyfi.composer.base import BaseConfig
 from hyfi.core import __about__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.joblib import JobLibConfig
 from hyfi.path import PathConfig
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
```

### Comparing `hyfi-1.5.0/src/hyfi/task/__init__.py` & `hyfi-1.5.1/src/hyfi/task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
-from hyfi.composer import BaseConfig, Composer
+from hyfi.composer import Composer
+from hyfi.composer.base import BaseConfig
 from hyfi.module import ModuleConfig
 from hyfi.path.task import TaskPathConfig
 from hyfi.project import ProjectConfig
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
 
 logger = LOGGING.getLogger(__name__)
```

### Comparing `hyfi-1.5.0/src/hyfi/task/batch.py` & `hyfi-1.5.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/conf.py` & `hyfi-1.5.1/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/contexts.py` & `hyfi-1.5.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/datasets.py` & `hyfi-1.5.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/envs.py` & `hyfi-1.5.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/funcs.py` & `hyfi-1.5.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/gpumon.py` & `hyfi-1.5.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/iolibs.py` & `hyfi-1.5.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/logging.py` & `hyfi-1.5.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/notebooks.py` & `hyfi-1.5.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/utils/packages.py` & `hyfi-1.5.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/src/hyfi/workflow/__init__.py` & `hyfi-1.5.1/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.0/PKG-INFO` & `hyfi-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.5.0
+Version: 1.5.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

