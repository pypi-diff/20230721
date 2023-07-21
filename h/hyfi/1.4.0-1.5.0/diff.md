# Comparing `tmp/hyfi-1.4.0.tar.gz` & `tmp/hyfi-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.4.0.tar", max compression
+gzip compressed data, was "hyfi-1.5.0.tar", max compression
```

## Comparing `hyfi-1.4.0.tar` & `hyfi-1.5.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1071 2023-07-21 02:31:51.337707 hyfi-1.4.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-21 02:31:51.337707 hyfi-1.4.0/README.md
--rw-r--r--   0        0        0     4928 2023-07-21 02:32:22.415505 hyfi-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2793 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 02:32:22.323500 hyfi-1.4.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7287 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-21 02:31:51.341707 hyfi-1.4.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    29019 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-21 02:32:22.323500 hyfi-1.4.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      864 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4214 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-21 02:31:51.345707 hyfi-1.4.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18424 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4354 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5849 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     3626 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20881 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-21 02:31:51.349707 hyfi-1.4.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 07:33:23.773884 hyfi-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 07:33:23.773884 hyfi-1.5.0/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 07:33:59.785934 hyfi-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 07:33:59.681934 hyfi-1.5.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7287 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 07:33:23.777884 hyfi-1.5.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    29019 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 07:33:59.681934 hyfi-1.5.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3480 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 07:33:23.781884 hyfi-1.5.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4204 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18424 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4354 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5849 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3626 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 07:33:23.785884 hyfi-1.5.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 07:33:23.789884 hyfi-1.5.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.0/PKG-INFO
```

### Comparing `hyfi-1.4.0/LICENSE` & `hyfi-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/README.md` & `hyfi-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/pyproject.toml` & `hyfi-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.4.0"
+version = "1.5.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.4.0/src/hyfi/__cli__.py` & `hyfi-1.5.0/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/__click__.py` & `hyfi-1.5.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/__init__.py` & `hyfi-1.5.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/about/__init__.py` & `hyfi-1.5.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/batch/__init__.py` & `hyfi-1.5.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.5.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.5.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.5.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/common.py` & `hyfi-1.5.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.5.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/meta.py` & `hyfi-1.5.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/progress.py` & `hyfi-1.5.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.5.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.5.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.5.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.5.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.5.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/testing.py` & `hyfi-1.5.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/cached_path/util.py` & `hyfi-1.5.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/composer/__init__.py` & `hyfi-1.5.0/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/composer/pydantic.py` & `hyfi-1.5.0/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.5.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.5.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/copier/__init__.py` & `hyfi-1.5.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/core/__init__.py` & `hyfi-1.5.0/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/core/config.py` & `hyfi-1.5.0/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/core/hydra.py` & `hyfi-1.5.0/src/hyfi/core/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.5.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/graphics/__init__.py` & `hyfi-1.5.0/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/graphics/collage.py` & `hyfi-1.5.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/graphics/motion.py` & `hyfi-1.5.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/graphics/utils.py` & `hyfi-1.5.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/joblib/__init__.py` & `hyfi-1.5.0/src/hyfi/joblib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     _config_name_: str = "__init__"
     _config_group_: str = "joblib"
 
     backend: str = "joblib"
     initialize_backend: bool = False
     minibatch_size: int = 1_000
     num_workers: int = 1
-    task_num_gpus: int = 0
+    num_gpus: int = 0
 
     _initilized_: bool = PrivateAttr(False)
     _batcher_instance_: Optional[Batcher] = PrivateAttr(None)
 
     def initialize(self):
         self.init_backend()
 
@@ -50,15 +50,15 @@
 
             core._batcher_instance_ = batcher.Batcher(
                 backend_handle=backend_handle,
                 backend=self.backend,
                 procs=self.num_workers,
                 minibatch_size=self.minibatch_size,
                 task_num_cpus=self.num_workers,
-                task_num_gpus=self.task_num_gpus,
+                task_num_gpus=self.num_gpus,
                 verbose=self.verbose,
             )
             self._batcher_instance_ = core._batcher_instance_
             logger.info("initialized batcher with %s", core._batcher_instance_)
         self._initilized_ = True
 
     def stop_backend(self):
```

### Comparing `hyfi-1.4.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.5.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.5.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.5.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/main/__init__.py` & `hyfi-1.5.0/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/path/__init__.py` & `hyfi-1.5.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/path/base.py` & `hyfi-1.5.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/path/batch.py` & `hyfi-1.5.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/path/dirnames.py` & `hyfi-1.5.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/path/task.py` & `hyfi-1.5.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/pipe/__init__.py` & `hyfi-1.5.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/pipe/test.py` & `hyfi-1.5.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.5.0/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/pipeline/configs.py` & `hyfi-1.5.0/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/project/__init__.py` & `hyfi-1.5.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/task/__init__.py` & `hyfi-1.5.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/task/batch.py` & `hyfi-1.5.0/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/conf.py` & `hyfi-1.5.0/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/contexts.py` & `hyfi-1.5.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/datasets.py` & `hyfi-1.5.0/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/envs.py` & `hyfi-1.5.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/funcs.py` & `hyfi-1.5.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/gpumon.py` & `hyfi-1.5.0/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/iolibs.py` & `hyfi-1.5.0/src/hyfi/utils/iolibs.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import tempfile
 import time
 import warnings
 from glob import glob
 from pathlib import Path, PosixPath, WindowsPath
 from types import TracebackType
-from typing import Callable, Iterator, List, Tuple, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import gdown
 
 from hyfi.cached_path import _cached_path
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.types import PathLikeType
 
@@ -552,14 +552,88 @@
                         return f
             return cache_path
 
         else:
             logger.warning("Unknown url: %s", url)
             return None
 
+    @staticmethod
+    def save_wordlist(
+        words: List[str],
+        filepath: Union[str, PosixPath, WindowsPath, Path],
+        sort: bool = True,
+        verbose: bool = True,
+        encoding="utf-8",
+        **kwargs,
+    ):
+        """Save the word list to the file."""
+        if sort:
+            words = sorted(words)
+        if verbose:
+            logger.info(
+                "Save the list to the file: %s, no. of words: %s", filepath, len(words)
+            )
+        with open(filepath, "w", encoding=encoding) as fo_:
+            for word in words:
+                fo_.write(word + "\n")
+
+    @staticmethod
+    def load_wordlist(
+        filepath: Union[str, PosixPath, WindowsPath, Path],
+        sort: bool = True,
+        lowercase: bool = False,
+        unique: bool = True,
+        remove_tag: bool = False,
+        max_ngram_to_include: Optional[int] = None,
+        ngram_delimiter: str = ";",
+        remove_delimiter: bool = False,
+        verbose: bool = True,
+        encoding="utf-8",
+        **kwargs,
+    ) -> List[str]:
+        """Load the word list from the file."""
+        filepath = Path(filepath)
+        if filepath.is_file():
+            with open(filepath, encoding=encoding) as fo_:
+                words = [
+                    word.strip().split()[0] for word in fo_ if len(word.strip()) > 0
+                ]
+        else:
+            logger.warning("File not found: %s", filepath)
+            return []
+
+        if remove_delimiter:
+            words = [word.replace(ngram_delimiter, "") for word in words]
+        if max_ngram_to_include:
+            words = [
+                word
+                for word in words
+                if len(word.split(ngram_delimiter)) <= max_ngram_to_include
+            ]
+        if verbose:
+            logger.info("Loaded the file: %s, No. of words: %s", filepath, len(words))
+
+        if remove_tag:
+            words = [word.split("/")[0] for word in words]
+        words = [
+            word.lower() if lowercase else word
+            for word in words
+            if not word.startswith("#")
+        ]
+        if unique:
+            words = list(set(words))
+            if verbose:
+                logger.info(
+                    "Remove duplicate words, No. of words: %s",
+                    len(words),
+                )
+        if sort:
+            words = sorted(words)
+        return words
+
 
 # See https://github.com/copier-org/copier/issues/345
 class TemporaryDirectory(tempfile.TemporaryDirectory):
     """A custom version of `tempfile.TemporaryDirectory` that handles read-only files better.
 
     On Windows, before Python 3.8, `shutil.rmtree` does not handle read-only files very well.
     This custom class makes use of a [special error handler][copier.tools.handle_remove_readonly]
```

### Comparing `hyfi-1.4.0/src/hyfi/utils/logging.py` & `hyfi-1.5.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/notebooks.py` & `hyfi-1.5.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/utils/packages.py` & `hyfi-1.5.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/src/hyfi/workflow/__init__.py` & `hyfi-1.5.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.4.0/PKG-INFO` & `hyfi-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.4.0
+Version: 1.5.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

