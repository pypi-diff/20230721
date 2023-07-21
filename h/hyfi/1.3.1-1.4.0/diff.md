# Comparing `tmp/hyfi-1.3.1.tar.gz` & `tmp/hyfi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.3.1.tar", max compression
+gzip compressed data, was "hyfi-1.4.0.tar", max compression
```

## Comparing `hyfi-1.3.1.tar` & `hyfi-1.4.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1071 2023-07-20 04:42:00.215841 hyfi-1.3.1/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-20 04:42:00.215841 hyfi-1.3.1/README.md
--rw-r--r--   0        0        0     4928 2023-07-20 04:42:25.473207 hyfi-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3606 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2465 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-20 04:42:25.397204 hyfi-1.3.1/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7287 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    26153 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-20 04:42:25.397204 hyfi-1.3.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      159 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      213 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      124 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      864 2023-07-20 04:42:00.219842 hyfi-1.3.1/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4214 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    14582 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4354 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5849 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     3626 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20881 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-20 04:42:00.223842 hyfi-1.3.1/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 02:31:51.337707 hyfi-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 02:31:51.337707 hyfi-1.4.0/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 02:32:22.415505 hyfi-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 02:32:22.323500 hyfi-1.4.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7287 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    29019 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 02:32:22.323500 hyfi-1.4.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3480 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4214 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18424 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4354 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5849 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3626 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20881 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.4.0/PKG-INFO
```

### Comparing `hyfi-1.3.1/LICENSE` & `hyfi-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/README.md` & `hyfi-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/pyproject.toml` & `hyfi-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.3.1"
+version = "1.4.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.3.1/src/hyfi/__cli__.py` & `hyfi-1.4.0/src/hyfi/__cli__.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,44 +14,14 @@
 )
 from hyfi.core.config import HyfiConfig
 from hyfi.main import HyFI
 
 logger = HyFI.getLogger(__name__)
 
 
-def about(**args):
-    """
-    Print the about information for Hyfi.
-    This is a wrapper around _about which takes a HyfiConfig as an argument
-    """
-    HyFI.run(args)
-
-
-def run_copy(**args):
-    """
-    Copy all config files to the current working directory.
-    This is a wrapper around HyfiConfig to allow us to pass arguments to it.
-    """
-    HyFI.run(args, "copier")
-
-
-def run_task(**args):
-    """
-    Run a task. This is a wrapper around HyFI
-    """
-    HyFI.run(args, "task")
-
-
-def run_workflow(**args):
-    """
-    Run a workflow. This is a wrapper around HyFI. run_workflow
-    """
-    HyFI.run(args, "workflow")
-
-
 def cli_main(cfg: DictConfig) -> None:
     """
     Main function for the command line interface.
     Initializes Hydra and instantiates the class.
     Prints the configuration to standard out if verbose is set to True
 
     Args:
@@ -79,20 +49,15 @@
         else:
             logger.info("## hydra configuration ##")
             print(HyFI.to_yaml(cfg))
 
         logger.info("Hydra working directory : %s", os.getcwd())
         logger.info("Orig working directory  : %s", hydra.utils.get_original_cwd())
 
-    if HyFI.is_instantiatable(cfg):
-        logger.info("Instantiating HyFI")
-        HyFI.instantiate(cfg)
-    else:
-        logger.info("HyFI is not instantiatable, running HyFI directly")
-        HyFI.run(cfg)
+    HyFI.run_config(config=cfg)
 
     HyFI.terminate()
 
 
 def hydra_main(
     config_path: Optional[str] = __config_path__,
     config_name: Optional[str] = __config_name__,
```

### Comparing `hyfi-1.3.1/src/hyfi/__click__.py` & `hyfi-1.4.0/src/hyfi/__click__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,60 @@
 
 import click
 
 from hyfi._version import __version__
 from hyfi.copier import Copier
 from hyfi.core import __hyfi_path__
 from hyfi.core.config import HyfiConfig
+from hyfi.main import HyFI
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
-@click.group()
+
+@click.group(invoke_without_command=True, context_settings=CONTEXT_SETTINGS)
 @click.version_option(__version__)
-def cli():
-    pass
+@click.option(
+    "--config",
+    "-c",
+    show_default=True,
+    help="Config group to compose and run",
+)
+@click.option(
+    "--print",
+    "-p",
+    show_default=True,
+    is_flag=True,
+    default=False,
+    help="Print the configuration instead of running it",
+)
+@click.pass_context
+def cli(ctx, config: str, print: bool):
+    """This is the auxiliary command line interface for Hyfi. The main command line
+    interface is 'hyfi'.
+
+    It is used to help run HyFI applications. If no command is specified, it will
+    compose a configuration and run it.
+
+    It is also used to copy configuration files to the destination directory and
+    to install shell completion for Hyfi.
+    \f
+
+    :param click.core.Context ctx: Click context.
+    """
+    if ctx.invoked_subcommand is None:
+        if config:
+            if print:
+                HyFI.print_config(config)
+            else:
+                HyFI.run(config_group=config)
+        else:
+            click.echo(ctx.get_help())
 
 
 @cli.command()
 @click.option(
     "--src_path",
     show_default=True,
     default=f"{__hyfi_path__()}/conf",
```

### Comparing `hyfi-1.3.1/src/hyfi/__init__.py` & `hyfi-1.4.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/about/__init__.py` & `hyfi-1.4.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/batch/__init__.py` & `hyfi-1.4.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/__init__.py` & `hyfi-1.4.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.4.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/cache_file.py` & `hyfi-1.4.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/common.py` & `hyfi-1.4.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/file_lock.py` & `hyfi-1.4.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/meta.py` & `hyfi-1.4.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/progress.py` & `hyfi-1.4.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.4.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.4.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.4.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.4.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.4.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/testing.py` & `hyfi-1.4.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/cached_path/util.py` & `hyfi-1.4.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/composer/__init__.py` & `hyfi-1.4.0/src/hyfi/composer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
 
 if level := os.environ.get("HYFI_LOG_LEVEL"):
     LOGGING.setLogger(level)
 logger = LOGGING.getLogger(__name__)
 
+__global_package_list__: Set[str] = {"cmd", "mode", "workflow"}
+
 
 class SpecialKeys(str, Enum):
     """Special keys in configs used by HyFI."""
 
     CALL = "_call_"
     CONFIG = "_config_"
     CONFIG_GROUP = "_config_group_"
@@ -276,14 +278,16 @@
             logger.debug("returning config_group_kwargs without composing")
             return config_data
         # Set overrides to the empty list if None
         if overrides is None:
             overrides = []
         # Set the group key and value of the config group.
         config_group, group_key, group_value = Composer.split_config_group(config_group)
+        if group_key in __global_package_list__:
+            global_package = True
         # If group_key and group_value are specified in the configuration file.
         if group_key and group_value:
             # Initialize hydra configuration module.
             cfg = Composer.hydra_compose(
                 root_config_name=root_config_name,
                 config_module=config_module,
                 overrides=overrides,
@@ -307,38 +311,38 @@
         # Initialize hydra and return the configuration.
         cfg = Composer.hydra_compose(
             root_config_name=root_config_name,
             config_module=config_module,
             overrides=overrides,
         )
         # Add config group overrides to overrides list.
-        group_overrides: List[str] = []
-        group_cfg = Composer.select(
-            cfg,
-            key=group_key,
-            default=None,
-            throw_on_missing=False,
-            throw_on_resolution_failure=False,
-        )
-        if config_data and group_cfg:
-            group_overrides.extend(
-                f"{group_key}.{k}={v}"
-                for k, v in config_data.items()
-                if isinstance(v, (str, int, float, bool)) and k in group_cfg
-            )
-        if group_overrides:
-            overrides.extend(group_overrides)
-            cfg = Composer.hydra_compose(
-                root_config_name=root_config_name,
-                config_module=config_module,
-                overrides=overrides,
+        if group_key and not global_package:
+            group_overrides: List[str] = []
+            group_cfg = Composer.select(
+                cfg,
+                key=group_key,
+                default=None,
+                throw_on_missing=False,
+                throw_on_resolution_failure=False,
             )
+            if config_data and group_cfg:
+                group_overrides.extend(
+                    f"{group_key}.{k}={v}"
+                    for k, v in config_data.items()
+                    if isinstance(v, (str, int, float, bool)) and k in group_cfg
+                )
+            if group_overrides:
+                overrides.extend(group_overrides)
+                cfg = Composer.hydra_compose(
+                    root_config_name=root_config_name,
+                    config_module=config_module,
+                    overrides=overrides,
+                )
 
-        # Select the group_key from the configuration.
-        if group_key and not global_package:
+            # Select the group_key from the configuration.
             cfg = Composer.select(
                 cfg,
                 key=group_key,
                 default=None,
                 throw_on_missing=throw_on_missing,
                 throw_on_resolution_failure=throw_on_resolution_failure,
             )
@@ -515,14 +519,74 @@
 
         Args:
             obj: The object to print the source code of.
 
         """
         print(Composer.getsource(obj))
 
+    @staticmethod
+    def instantiate_config(
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        global_package: bool = False,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any:
+        """
+        Instantiates an object using the provided config group and overrides.
+
+        Args:
+            config_group: Name of the config group to compose (`config_group=name`)
+            overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
+            global_package: If True, the config assumed to be a global package
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
+                    parameters in the config object. Parameters not present
+                    in the config objects are being passed as is to the target.
+                    IMPORTANT: dataclasses instances in kwargs are interpreted as config
+                                and cannot be used as passthrough
+
+        Returns:
+            if _target_ is a class name: the instantiated object
+            if _target_ is a callable: the return value of the call
+        """
+        cfg = Composer._compose(
+            config_group=config_group,
+            overrides=overrides,
+            config_data=config_data,
+            global_package=global_package,
+        )
+        return Composer.instantiate(cfg, *args, **kwargs)
+
+    @staticmethod
+    def print_config(
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        global_package: bool = False,
+    ):
+        """
+        Print the configuration
+
+        Args:
+            config_group: Name of the config group to compose (`config_group=name`)
+            overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
+            global_package: If True, the config assumed to be a global package
+        """
+        cfg = Composer._compose(
+            config_group=config_group,
+            overrides=overrides,
+            config_data=config_data,
+            global_package=global_package,
+        )
+        Composer.print(cfg)
+
 
 class BaseConfig(BaseModel):
     """
     Base class for all config classes.
     """
 
     _config_name_: str = "__init__"
```

### Comparing `hyfi-1.3.1/src/hyfi/composer/pydantic.py` & `hyfi-1.4.0/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.4.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.4.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/copier/__init__.py` & `hyfi-1.4.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/core/__init__.py` & `hyfi-1.4.0/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/core/config.py` & `hyfi-1.4.0/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/core/hydra.py` & `hyfi-1.4.0/src/hyfi/core/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/dotenv/__init__.py` & `hyfi-1.4.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/graphics/__init__.py` & `hyfi-1.4.0/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/graphics/collage.py` & `hyfi-1.4.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/graphics/motion.py` & `hyfi-1.4.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/graphics/utils.py` & `hyfi-1.4.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/joblib/__init__.py` & `hyfi-1.4.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/joblib/batch/apply.py` & `hyfi-1.4.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.4.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.4.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/main/__init__.py` & `hyfi-1.4.0/src/hyfi/main/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -250,17 +250,17 @@
 
         Args:
             **kwargs: Additional keyword arguments to pass to the WorkflowConfig constructor.
 
         Returns:
             WorkflowConfig: An instance of the WorkflowConfig class.
         """
-        if _config_name_ := kwargs.get("_config_name_"):
+        if config_name := kwargs.get("workflow_name"):
             cfg = HyFI.compose_as_dict(
-                config_group=f"workflow={_config_name_}",
+                config_group=f"workflow={config_name}",
                 config_data=kwargs,
                 global_package=True,
             )
         else:
             cfg = kwargs
         if __global_config__.project and "project" in cfg:
             del cfg["project"]
@@ -349,14 +349,74 @@
             config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
+    def instantiate_config(
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        global_package: bool = False,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any:
+        """
+        Instantiates an object using the provided config group and overrides
+
+        Args:
+            config_group: Name of the config group to compose (`config_group=name`)
+            overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
+            global_package: If True, the config assumed to be a global package
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
+                    parameters in the config object. Parameters not present
+                    in the config objects are being passed as is to the target.
+                    IMPORTANT: dataclasses instances in kwargs are interpreted as config
+                                and cannot be used as passthrough
+
+        Returns:
+            if _target_ is a class name: the instantiated object
+            if _target_ is a callable: the return value of the call
+        """
+        return Composer.instantiate_config(
+            config_group=config_group,
+            overrides=overrides,
+            config_data=config_data,
+            global_package=global_package,
+            *args,
+            **kwargs,
+        )
+
+    @staticmethod
+    def print_config(
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
+        config_data: Union[Dict[str, Any], DictConfig, None] = None,
+        global_package: bool = False,
+    ):
+        """
+        Print the configuration
+
+        Args:
+            config_group: Name of the config group to compose (`config_group=name`)
+            overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
+            global_package: If True, the config assumed to be a global package
+        """
+        Composer.print_config(
+            config_group=config_group,
+            overrides=overrides,
+            config_data=config_data,
+            global_package=global_package,
+        )
+
+    @staticmethod
     def partial(
         config: Union[str, Dict],
         *args: Any,
         **kwargs: Any,
     ) -> Callable:
         return Composer.partial(config, *args, **kwargs)
 
@@ -376,24 +436,57 @@
     def viewsource(obj):
         return Composer.viewsource(obj)
 
     ###############################
     # Pipeline related functions
     ###############################
     @staticmethod
-    def run(cfg: Union[Dict, DictConfig], target: Optional[str] = None):
-        """Run the config"""
-        cfg = HyFI.to_dict(cfg)
-        if "tasks" in cfg:
-            workflow = HyFI.workflow(**cfg)
-            HyFI.run_workflow(workflow)
-        elif "task" in cfg and (target is None or target == "task"):
-            project = HyFI.init_project(**cfg["project"]) if "project" in cfg else None
-            task = HyFI.task(**cfg["task"])
-            HyFI.run_task(task, project=project)
-        elif "copier" in cfg and (target is None or target == "copier"):
-            with Copier(**cfg["copier"]) as worker:
-                worker.run_copy()
+    def run(**cfg):
+        """Run the provided config"""
+        HyFI.run_config(config=cfg)
+
+    @staticmethod
+    def run_config(
+        config_group: Optional[str] = None,
+        overrides: Optional[List[str]] = None,
+        config: Optional[Union[Dict[str, Any], DictConfig]] = None,
+        global_package=False,
+        **kwargs,
+    ):
+        """Run the config by composing it and running it"""
+        if config_group:
+            logger.info("Composing the HyFI config from config group %s", config_group)
+            config = HyFI.compose_as_dict(
+                config_group=config_group,
+                overrides=overrides,
+                config_data=config,
+                global_package=global_package,
+            )
+        config = HyFI.to_dict(config) if config else {}
+        if not isinstance(config, dict):
+            raise ValueError("The config must be a dictionary")
+        cmd_name = config.get("cmd_name")
+        # Check if the config is instantiatable
+        if HyFI.is_instantiatable(config):
+            logger.info("Instantiating the HyFI config")
+            HyFI.instantiate(config)
         else:
-            if target and target not in cfg:
-                logger.warning("Target %s not found in config", target)
-            HyFI.about(**cfg.get("about", {}))
+            logger.info(
+                "The HyFI config is not instantiatable, running HyFI task with the config"
+            )
+            # Run the HyFI task
+            if "tasks" in config or cmd_name == "run_workflow":
+                workflow = HyFI.workflow(**config)
+                HyFI.run_workflow(workflow)
+            elif "task" in config and (cmd_name is None or cmd_name == "run_task"):
+                project = (
+                    HyFI.init_project(**config["project"])
+                    if "project" in config
+                    else None
+                )
+                task = HyFI.task(**config["task"])
+                HyFI.run_task(task, project=project)
+            elif "copier" in config and (cmd_name is None or cmd_name == "copy_conf"):
+                with Copier(**config["copier"]) as worker:
+                    worker.run_copy()
+            else:
+                HyFI.about(**config.get("about", {}))
```

### Comparing `hyfi-1.3.1/src/hyfi/path/__init__.py` & `hyfi-1.4.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/path/base.py` & `hyfi-1.4.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/path/batch.py` & `hyfi-1.4.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/path/dirnames.py` & `hyfi-1.4.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/path/task.py` & `hyfi-1.4.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/pipe/__init__.py` & `hyfi-1.4.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/pipe/test.py` & `hyfi-1.4.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/pipeline/__init__.py` & `hyfi-1.4.0/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/pipeline/configs.py` & `hyfi-1.4.0/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/project/__init__.py` & `hyfi-1.4.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/task/__init__.py` & `hyfi-1.4.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/task/batch.py` & `hyfi-1.4.0/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/conf.py` & `hyfi-1.4.0/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/contexts.py` & `hyfi-1.4.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/datasets.py` & `hyfi-1.4.0/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/envs.py` & `hyfi-1.4.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/funcs.py` & `hyfi-1.4.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/gpumon.py` & `hyfi-1.4.0/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/iolibs.py` & `hyfi-1.4.0/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/logging.py` & `hyfi-1.4.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/notebooks.py` & `hyfi-1.4.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/utils/packages.py` & `hyfi-1.4.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/src/hyfi/workflow/__init__.py` & `hyfi-1.4.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.3.1/PKG-INFO` & `hyfi-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.3.1
+Version: 1.4.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

