# Comparing `tmp/pyft-0.1.2.tar.gz` & `tmp/pyft-0.1.3.tar.gz`

## Comparing `pyft-0.1.2.tar` & `pyft-0.1.3.tar`

### file list

```diff
@@ -1,92 +1,90 @@
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.2/local_dependencies/bio-io/Cargo.toml
--rw-r--r--   0      501       20     9047 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/bio-io/src/lib.rs
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 pyft-0.1.2/local_dependencies/bamlift/Cargo.toml
--rw-r--r--   0      501       20    10341 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/bamlift/src/lib.rs
--rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 pyft-0.1.2/local_dependencies/fibertools-rs/Cargo.toml
--rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.cargo/config
--rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.dockerignore
--rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.github/workflows/CI.yml
--rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.github/workflows/release.yml
--rw-r--r--   0      501       20      199 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.gitignore
--rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.pre-commit-config.yaml
--rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.2/local_dependencies/fibertools-rs/.readthedocs.yaml
--rw-r--r--   0      501       20   105870 2023-07-20 03:50:06.000000 pyft-0.1.2/local_dependencies/fibertools-rs/CHANGELOG.md
--rw-r--r--   0      501       20    63045 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/Cargo.lock
--rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.2/local_dependencies/fibertools-rs/Dockerfile
--rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.2/local_dependencies/fibertools-rs/INSTALL.md
--rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/NOTES.md
--rw-r--r--   0      501       20     4386 2023-07-20 18:44:24.000000 pyft-0.1.2/local_dependencies/fibertools-rs/README.md
--rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/_config.yml
--rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/center.png
--rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
--rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
--rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
--rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/logo.png
--rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.2/local_dependencies/fibertools-rs/build.rs
--rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft--help.md
--rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
--rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-all-columns.md
--rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-center-help.md
--rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
--rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-extract-help.md
--rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
--rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
--rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/docs/make_help_docs.sh
--rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.2/local_dependencies/fibertools-rs/env.yaml
--rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
--rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_torch.pt
--rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
--rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_torch.pt
--rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
--rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
--rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
--rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
--rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
--rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
--rw-r--r--   0      501       20    57302 2023-07-19 17:45:37.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/other/m6A_revio_s3_noinit_semi_supervised_cnn.best.torch.pickle.onnx
--rw-r--r--   0      501       20    57304 2023-07-19 17:46:07.000000 pyft-0.1.2/local_dependencies/fibertools-rs/models/other/revio.onnx
--rw-r--r--   0      501       20    15625 2023-07-20 19:04:29.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/basemods/mod.rs
--rw-r--r--   0      501       20    12213 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/center.rs
--rw-r--r--   0      501       20    10971 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/cli.rs
--rw-r--r--   0      501       20    18878 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/extract.rs
--rw-r--r--   0      501       20     4077 2023-07-19 22:27:32.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/lib.rs
--rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/main.rs
--rw-r--r--   0      501       20    12899 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/nucleosomes.rs
--rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
--rw-r--r--   0      501       20    18371 2023-06-29 17:02:56.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
--rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
--rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.2/local_dependencies/fibertools-rs/src/strip_basemods.rs
--rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/all.bam
--rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/all.bam.bai
--rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bam
--rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bam.bai
--rw-r--r--   0      501       20     3349 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bed
--rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
--rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/test.txt
--rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/test.txt.gz
--rw-r--r--   0      501       20     1997 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/extract_test.rs
--rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.2/local_dependencies/fibertools-rs/tests/run_test.rs
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 pyft-0.1.2/Cargo.toml
--rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.2/.gitignore
--rw-r--r--   0      501       20      924 2023-07-20 19:49:12.000000 pyft-0.1.2/README.md
--rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.2/docs/Makefile
--rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.2/docs/_static/css/rtd_dark.css
--rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.2/docs/_static/img/fiber_tools_grey.png
--rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.2/docs/_templates/layout.html
--rw-r--r--   0      501       20     1565 2023-07-20 19:08:31.000000 pyft-0.1.2/docs/conf.py
--rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.2/docs/environment.yml
--rw-r--r--   0      501       20      596 2023-07-20 19:15:12.000000 pyft-0.1.2/docs/index.rst
--rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.2/docs/make.bat
--rw-r--r--   0      501       20       46 2023-07-20 17:01:46.000000 pyft-0.1.2/docs/modules.rst
--rw-r--r--   0      501       20      141 2023-07-20 17:44:28.000000 pyft-0.1.2/docs/pyft.rst
--rw-r--r--   0      501       20        4 2023-07-20 16:47:52.000000 pyft-0.1.2/docs/requirements.txt
--rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.2/pyproject.toml
--rw-r--r--   0      501       20     7108 2023-07-20 19:40:20.000000 pyft-0.1.2/src/fiberdata.rs
--rw-r--r--   0      501       20      460 2023-07-20 19:36:11.000000 pyft-0.1.2/src/lib.rs
--rw-r--r--   0      501       20      157 2023-07-20 19:36:50.000000 pyft-0.1.2/test.py
--rw-r--r--   0      501       20    57429 2023-07-20 19:53:19.000000 pyft-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 pyft-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 pyft-0.1.3/local_dependencies/bamlift/Cargo.toml
+-rw-r--r--   0      501       20    10004 2023-07-21 05:33:24.000000 pyft-0.1.3/local_dependencies/bamlift/src/lib.rs
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.3/local_dependencies/bio-io/Cargo.toml
+-rw-r--r--   0      501       20    11069 2023-07-21 04:27:30.000000 pyft-0.1.3/local_dependencies/bio-io/src/lib.rs
+-rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 pyft-0.1.3/local_dependencies/fibertools-rs/Cargo.toml
+-rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.cargo/config
+-rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.dockerignore
+-rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.github/workflows/release.yml
+-rw-r--r--   0      501       20      199 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.gitignore
+-rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.3/local_dependencies/fibertools-rs/.readthedocs.yaml
+-rw-------   0      501       20   122462 2023-07-21 08:31:15.000000 pyft-0.1.3/local_dependencies/fibertools-rs/CHANGELOG.md
+-rw-r--r--   0      501       20    63045 2023-07-21 08:18:33.000000 pyft-0.1.3/local_dependencies/fibertools-rs/Cargo.lock
+-rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.3/local_dependencies/fibertools-rs/Dockerfile
+-rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.3/local_dependencies/fibertools-rs/INSTALL.md
+-rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/NOTES.md
+-rw-r--r--   0      501       20     4471 2023-07-21 07:53:23.000000 pyft-0.1.3/local_dependencies/fibertools-rs/README.md
+-rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/_config.yml
+-rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/center.png
+-rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
+-rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
+-rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/logo.png
+-rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.3/local_dependencies/fibertools-rs/build.rs
+-rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft--help.md
+-rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
+-rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-all-columns.md
+-rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-center-help.md
+-rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
+-rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-extract-help.md
+-rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
+-rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
+-rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/docs/make_help_docs.sh
+-rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.3/local_dependencies/fibertools-rs/env.yaml
+-rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
+-rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_torch.pt
+-rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
+-rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_torch.pt
+-rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
+-rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
+-rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
+-rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
+-rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
+-rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.3/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
+-rw-r--r--   0      501       20    18322 2023-07-21 07:30:00.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/basemods/mod.rs
+-rw-r--r--   0      501       20    12212 2023-07-21 05:39:47.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/center.rs
+-rw-r--r--   0      501       20    10971 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/cli.rs
+-rw-r--r--   0      501       20    18967 2023-07-21 08:36:48.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/extract.rs
+-rw-r--r--   0      501       20     4105 2023-07-20 23:59:39.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/lib.rs
+-rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/main.rs
+-rw-r--r--   0      501       20    12907 2023-07-21 05:47:41.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/nucleosomes.rs
+-rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
+-rw-r--r--   0      501       20    18361 2023-07-21 00:03:41.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
+-rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
+-rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.3/local_dependencies/fibertools-rs/src/strip_basemods.rs
+-rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/all.bam
+-rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/all.bam.bai
+-rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bam
+-rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bam.bai
+-rw-r--r--   0      501       20     3349 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bed
+-rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
+-rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/test.txt
+-rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/test.txt.gz
+-rw-r--r--   0      501       20     1992 2023-07-21 05:45:51.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/extract_test.rs
+-rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.3/local_dependencies/fibertools-rs/tests/run_test.rs
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pyft-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.3/.gitignore
+-rw-r--r--   0      501       20      924 2023-07-20 19:57:36.000000 pyft-0.1.3/README.md
+-rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.3/docs/Makefile
+-rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.3/docs/_static/css/rtd_dark.css
+-rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.3/docs/_static/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.3/docs/_templates/layout.html
+-rw-r--r--   0      501       20     1565 2023-07-20 19:08:31.000000 pyft-0.1.3/docs/conf.py
+-rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.3/docs/environment.yml
+-rw-r--r--   0      501       20      596 2023-07-20 19:15:12.000000 pyft-0.1.3/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.3/docs/make.bat
+-rw-r--r--   0      501       20       46 2023-07-20 17:01:46.000000 pyft-0.1.3/docs/modules.rst
+-rw-r--r--   0      501       20      141 2023-07-20 17:44:28.000000 pyft-0.1.3/docs/pyft.rst
+-rw-r--r--   0      501       20        4 2023-07-20 16:47:52.000000 pyft-0.1.3/docs/requirements.txt
+-rw-r--r--   0      501       20      282 2023-07-20 23:32:48.000000 pyft-0.1.3/example.py
+-rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20     8583 2023-07-21 08:03:52.000000 pyft-0.1.3/src/fiberdata.rs
+-rw-r--r--   0      501       20      660 2023-07-20 23:34:28.000000 pyft-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20    57739 2023-07-21 15:17:39.000000 pyft-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 pyft-0.1.3/PKG-INFO
```

### Comparing `pyft-0.1.2/local_dependencies/bio-io/Cargo.toml` & `pyft-0.1.3/local_dependencies/bio-io/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 categories = ["library"]
 description = "My utilities for reading and writing bioinformatics file formats"
 edition = "2021"
 keywords = ["bam", "bfx"]
 license = "MIT"
 name = "bio-io"
 repository = "https://github.com/fiberseq/fibertools-rs"
-version = "0.1.0"
+version = "0.1.1"
 
 [dependencies]
 anyhow = "1.0.58"
 colored = "2.0.0"
 gzp = "0.11.3"
 #indicatif = {version = "0.17.0", features = ["rayon"]}
 #env_logger = "0.9.0"
 itertools = "0.10.5"
 lazy_static = "1.4.0"
 log = "0.4"
 niffler = {version = "2.5.0", default-features = false, features = ["gz"]}
 regex = "1.5.4"
-rust-htslib = "0.43.1"
+rust-htslib = "0.44.1"
```

### Comparing `pyft-0.1.2/local_dependencies/bio-io/src/lib.rs` & `pyft-0.1.3/local_dependencies/bio-io/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use gzp::deflate::Bgzf; //, Gzip, Mgzip, RawDeflate};
 use gzp::{Compression, ZBuilder};
 use itertools::Itertools;
 use lazy_static::lazy_static;
 use niffler::get_reader;
 use regex::Regex;
 use rust_htslib::bam;
+use rust_htslib::bam::record::Aux;
 use rust_htslib::bam::Read;
 use std::collections::HashMap;
 use std::env;
 use std::ffi::OsStr;
 use std::fs::File;
 use std::io::{self, stdout, BufReader, BufWriter, Write};
 use std::path::{Path, PathBuf};
@@ -185,15 +186,15 @@
             cur_vec.push(r.unwrap())
         }
         // return
         if cur_vec.is_empty() {
             None
         } else {
             let duration = start.elapsed().as_secs_f64();
-            log::info!(
+            log::debug!(
                 "Read {} bam records at {}.",
                 format!("{:}", cur_vec.len()).bright_magenta().bold(),
                 format!("{:.2?} reads/s", cur_vec.len() as f64 / duration)
                     .bright_cyan()
                     .bold(),
             );
             Some(cur_vec)
@@ -269,7 +270,73 @@
     log::info!(
         "Bam header implies PacBio chemistry {} binding kit {}.",
         chem,
         binding_kit
     );
     chemistry.clone()
 }
+
+///```
+/// use rust_htslib::{bam, bam::Read};
+/// use log;
+/// let mut bam = bam::Reader::from_path(&"../tests/data/all.bam").unwrap();
+/// for record in bam.records() {
+///     let record = record.unwrap();
+///     let n_s = bio_io::get_u32_tag(&record, b"ns");
+///     let n_l = bio_io::get_u32_tag(&record, b"nl");
+///     let a_s = bio_io::get_u32_tag(&record, b"as");
+///     let a_l = bio_io::get_u32_tag(&record, b"al");
+///     log::debug!("{:?}", a_s);
+/// }
+///```
+pub fn get_u32_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<i64> {
+    if let Ok(Aux::ArrayU32(array)) = record.aux(tag) {
+        let read_array = array.iter().map(|x| x as i64).collect::<Vec<_>>();
+        read_array
+    } else {
+        vec![]
+    }
+}
+
+pub fn get_u8_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<u8> {
+    if let Ok(Aux::ArrayU8(array)) = record.aux(tag) {
+        let read_array = array.iter().collect::<Vec<_>>();
+        read_array
+    } else {
+        vec![]
+    }
+}
+
+/// Convert the PacBio u16 tag into the u8 tag we normally expect.
+pub fn get_pb_u16_tag_as_u8(record: &bam::Record, tag: &[u8; 2]) -> Vec<u8> {
+    if let Ok(Aux::ArrayU16(array)) = record.aux(tag) {
+        let read_array = array.iter().collect::<Vec<_>>();
+        read_array
+            .iter()
+            .map(|&x| {
+                if x < 64 {
+                    x
+                } else if x < 191 {
+                    (x - 64) / 2 + 64
+                } else if x < 445 {
+                    (x - 192) / 4 + 128
+                } else if x < 953 {
+                    (x - 448) / 8 + 192
+                } else {
+                    255
+                }
+            })
+            .map(|x| x as u8)
+            .collect()
+    } else {
+        vec![]
+    }
+}
+
+pub fn get_f32_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<f32> {
+    if let Ok(Aux::ArrayFloat(array)) = record.aux(tag) {
+        let read_array = array.iter().collect::<Vec<_>>();
+        read_array
+    } else {
+        vec![]
+    }
+}
```

### Comparing `pyft-0.1.2/local_dependencies/bamlift/src/lib.rs` & `pyft-0.1.3/local_dependencies/bamlift/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use rust_htslib::{bam, bam::ext::BamRecordExtensions, bam::record::Aux};
+use rust_htslib::{bam, bam::ext::BamRecordExtensions};
 use std::fmt::{Debug, Display};
 
 /// Merge two lists into a sorted list
 /// Normal sort is supposed to be very fast on two sorted lists
 /// <https://doc.rust-lang.org/std/vec/struct.Vec.html#current-implementation-6>
 pub fn merge_two_lists<T>(left: &[T], right: &[T]) -> Vec<T>
 where
@@ -213,15 +213,15 @@
                 (start, end - start)
             }
         })
         .collect()
 }
 
 /// liftover positions using the cigar string
-fn liftover_exact(record: &bam::Record, positions: &[i64], get_reference: bool) -> Vec<i64> {
+fn _liftover_exact_old(record: &bam::Record, positions: &[i64], get_reference: bool) -> Vec<i64> {
     // find the shared positions in the reference
     let mut return_positions = vec![];
     let mut cur_pos = 0;
     for [q_pos, r_pos] in record.aligned_pairs() {
         // check whether we are searching for an exact position in
         // the reference or the query
         let val_to_match = if get_reference { q_pos } else { r_pos };
@@ -246,14 +246,68 @@
     while positions.len() > return_positions.len() {
         return_positions.push(-1);
     }
     assert_eq!(positions.len(), return_positions.len());
     return_positions
 }
 
+/// liftover positions using the cigar string
+fn liftover_exact_new(record: &bam::Record, positions: &[i64], get_reference: bool) -> Vec<i64> {
+    // find the shared positions in the reference
+    let mut return_positions = vec![];
+    let mut cur_idx = 0;
+    // ends are not inclusive, I checked.
+    for ([q_st, q_en], [r_st, r_en]) in record.aligned_block_pairs() {
+        let (st, en) = if get_reference {
+            (q_st, q_en)
+        } else {
+            (r_st, r_en)
+        };
+        // check bounds
+        if cur_idx == positions.len() {
+            break;
+        }
+        let mut cur_pos = positions[cur_idx];
+        // need to go to the next block
+        while cur_pos < en {
+            if cur_pos >= st {
+                let dist_from_start = cur_pos - st;
+                let rtn_pos = if get_reference {
+                    r_st + dist_from_start
+                } else {
+                    q_st + dist_from_start
+                };
+                return_positions.push(rtn_pos);
+            } else {
+                return_positions.push(-1);
+            }
+            // reset current position
+            cur_idx += 1;
+            if cur_idx == positions.len() {
+                break;
+            }
+            cur_pos = positions[cur_idx];
+        }
+    }
+
+    // add values for things that won't lift at the end
+    while positions.len() > return_positions.len() {
+        return_positions.push(-1);
+    }
+    assert_eq!(positions.len(), return_positions.len());
+    return_positions
+}
+
+fn liftover_exact(record: &bam::Record, positions: &[i64], get_reference: bool) -> Vec<i64> {
+    let new = liftover_exact_new(record, positions, get_reference);
+    //let old = _liftover_exact_old(record, positions, get_reference);
+    //assert_eq!(new, old);
+    new
+}
+
 pub fn get_exact_reference_positions(record: &bam::Record, query_positions: &[i64]) -> Vec<i64> {
     if record.is_unmapped() {
         query_positions.iter().map(|_x| -1).collect()
     } else {
         liftover_exact(record, query_positions, true)
     }
 }
@@ -261,75 +315,7 @@
 pub fn get_exact_query_positions(record: &bam::Record, reference_positions: &[i64]) -> Vec<i64> {
     if record.is_unmapped() {
         reference_positions.iter().map(|_x| -1).collect()
     } else {
         liftover_exact(record, reference_positions, false)
     }
 }
-
-///```
-/// use rust_htslib::{bam, bam::Read};
-/// use log;
-/// use env_logger::{Builder, Target};;
-/// Builder::new().target(Target::Stderr).filter(None, log::LevelFilter::Debug).init();
-/// let mut bam = bam::Reader::from_path(&"../tests/data/all.bam").unwrap();
-/// for record in bam.records() {
-///     let record = record.unwrap();
-///     let n_s = bamlift::get_u32_tag(&record, b"ns");
-///     let n_l = bamlift::get_u32_tag(&record, b"nl");
-///     let a_s = bamlift::get_u32_tag(&record, b"as");
-///     let a_l = bamlift::get_u32_tag(&record, b"al");
-///     log::debug!("{:?}", a_s);
-/// }
-///```
-pub fn get_u32_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<i64> {
-    if let Ok(Aux::ArrayU32(array)) = record.aux(tag) {
-        let read_array = array.iter().map(|x| x as i64).collect::<Vec<_>>();
-        read_array
-    } else {
-        vec![]
-    }
-}
-
-pub fn get_u8_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<u8> {
-    if let Ok(Aux::ArrayU8(array)) = record.aux(tag) {
-        let read_array = array.iter().collect::<Vec<_>>();
-        read_array
-    } else {
-        vec![]
-    }
-}
-
-/// Convert the PacBio u16 tag into the u8 tag we normally expect.
-pub fn get_pb_u16_tag_as_u8(record: &bam::Record, tag: &[u8; 2]) -> Vec<u8> {
-    if let Ok(Aux::ArrayU16(array)) = record.aux(tag) {
-        let read_array = array.iter().collect::<Vec<_>>();
-        read_array
-            .iter()
-            .map(|&x| {
-                if x < 64 {
-                    x
-                } else if x < 191 {
-                    (x - 64) / 2 + 64
-                } else if x < 445 {
-                    (x - 192) / 4 + 128
-                } else if x < 953 {
-                    (x - 448) / 8 + 192
-                } else {
-                    255
-                }
-            })
-            .map(|x| x as u8)
-            .collect()
-    } else {
-        vec![]
-    }
-}
-
-pub fn get_f32_tag(record: &bam::Record, tag: &[u8; 2]) -> Vec<f32> {
-    if let Ok(Aux::ArrayFloat(array)) = record.aux(tag) {
-        let read_array = array.iter().collect::<Vec<_>>();
-        read_array
-    } else {
-        vec![]
-    }
-}
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/Cargo.toml` & `pyft-0.1.3/local_dependencies/fibertools-rs/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 edition = "2021"
 homepage = "https://fiberseq.github.io/fibertools-rs/"
 keywords = ["cli", "bam", "bfx"]
 license = "MIT"
 name = "fibertools-rs"
 readme = "README.md"
 repository = "https://github.com/fiberseq/fibertools-rs"
-version = "0.2.5"
+version = "0.2.6"
 
 [[bin]]
 name = "ft"
 path = "src/main.rs"
 
 [dependencies]
 anstyle = "1.0.0"
 anyhow = "1.0.58"
-bamlift = {version = "0.1.0", path = "../bamlift" }
+bamlift = {path = "../bamlift", version = "0.1.1"}
 bio = "1.2.0"
-bio-io = {version = "0.1.0", path = "../bio-io" }
+bio-io = {path = "../bio-io", version = "0.1.1"}
 clap = {version = "4.3.4", features = ["cargo", "wrap_help", "color", "unstable-styles", "derive"]}
 clap_complete = "4.0.6"
 clap_mangen = "0.2.5"
 colored = "2.0.0"
 console = "0.15"
 env_logger = "0.9.0"
 gbdt = "0.1.1"
 indicatif = {version = "0.17.0", features = ["rayon"]}
 itertools = "0.10.5"
 lazy_static = "1.4.0"
 log = "0.4"
 ordered-float = "3.4.0"
 rayon = "1.5"
 regex = "1.5.4"
-rust-htslib = "0.43.1"
+rust-htslib = "0.44.1"
 serde = {version = "1.0.104", features = ["derive"]}
 serde_json = "1.0.48"
 spin = "0.9.8"
 tch = {version = "0.13.0", optional = true}
 tempfile = "3.3.0"
 
 [features]
@@ -51,7 +51,12 @@
 [profile.dist]
 debug = true
 inherits = "release"
 split-debuginfo = "packed"
 
 [profile.dev]
 opt-level = 2
+
+[profile.release]
+codegen-units = 1
+debug = true
+lto = "thin"
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/.github/workflows/CI.yml` & `pyft-0.1.3/local_dependencies/fibertools-rs/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/.github/workflows/release.yml` & `pyft-0.1.3/local_dependencies/fibertools-rs/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/CHANGELOG.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,218 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and the project tries but probably doesn't to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## Unreleased
+## 0.2.6 (2023-07-21)
+
+<csr-id-66b98f9f3c2644e79bf72de2ed070fba75b2ba38/>
+<csr-id-9e8cda2fb47eff101eb3d458cf4599543e7d05a2/>
+<csr-id-23e6b12a7601afb4aa21454048a53d803ca1bcdf/>
+<csr-id-b03df77d99a8f28ecd6d43509a43ff92fb300329/>
+<csr-id-6e8cd6f9f25dcabc15ef2a25595b3a3ee86de241/>
+<csr-id-79ca845b0e72e832cdc57b1e1b58090a09417936/>
+<csr-id-41bcd27e9de8654fd46bfb50d3c7efabad59a17e/>
+<csr-id-66338fd576a66ee230aa4234d072a93b3a3b21d5/>
+<csr-id-6f910c53a4e0cb7be411b724385e540517f21306/>
+<csr-id-85d471df45a0c88567857427725852c491c041ff/>
+<csr-id-c5eb60a8d42616eacfafb871cf4f46fb2fa924c8/>
+<csr-id-5bd6803c346a409150daea7713878af46995e836/>
+<csr-id-a59f41d0b2d4b97b277b738f04b23010be8d6449/>
+<csr-id-7a633d71272a9425ae276d9b846fcda38f6526e5/>
+<csr-id-8d16055edc4bf9bc5f94d5be42b86b2a2df712c8/>
+<csr-id-467072ae6419b3ece8329f587467d0d0bf316911/>
+<csr-id-09994bdbdd3949186d44ecef36199a8d228ea280/>
+<csr-id-8ea9fb1efc4897e191468ee10aa66500456fa0fc/>
+<csr-id-82399e6e702033acbb455ef6aea3a9935338d77f/>
+<csr-id-fd115b7fdb6754d6f6885e901bc34d7364bfc7df/>
+<csr-id-1d25caf7e8c19f97d39dec8eb69de7219e85621b/>
+<csr-id-e73e00c849726e4577344ec8e964b3eda93ddbc6/>
+<csr-id-a3f29cd798fcbeb071fce7ea7041c4e71a98f8f6/>
+<csr-id-e85afd963f513fe578b2d0f3e368a7ae56b59d84/>
+<csr-id-580968a9da3c2a66740d01dfcc0d8c574bfd46c8/>
+<csr-id-6b1e714ccda049aef3199563c03d6f5ec1df9dfa/>
+<csr-id-c8502ac7cf87d375a5aa9fcf3494a3cf8f43105c/>
+<csr-id-b9274c2a7064cd615b079b3cc0b44d9e2f4b5e50/>
+<csr-id-eb44bdaf8280689eb06e536266b64802f509a7b3/>
+<csr-id-b98edf9f855ae24f81389a5ea481bf0b16dcd794/>
+<csr-id-32f01826bbf06ac726464d59eee2769dfe80b138/>
+<csr-id-94dfd521a3f637df47c996fd046d1de3cde85776/>
+<csr-id-b3fa1c3b218379a3290fbed2382572b5e1c3e091/>
+<csr-id-d4b75b1a569d694495bc1e87de651c1bb4e63778/>
+<csr-id-73c918f9344fe362f602fa5356b11c9574c5ffec/>
+<csr-id-5f635e04085c012d39d8afa362416ca3642fc7c5/>
+<csr-id-c86cc585993506c55bd0243936767afe4a5f671c/>
+<csr-id-15b825ed80a4b099c9ea9f21f64f1b695e20554a/>
+<csr-id-26ef86389490b3161546271bea194e4c8a4a8b7f/>
+<csr-id-d953400d9c7f676fea70fee51264c331ba7e1067/>
+<csr-id-10bf0df63acca5812e3d2d3ad5134bc75abe73b4/>
+<csr-id-cdde18e3b119ef36d57feed2f4740b7bde30c011/>
+<csr-id-ac1987d33daf7fb7395ed1cf15b311390a15e60c/>
+<csr-id-2f7c08e2b24a07054d547088ac2c96463a6229d3/>
+
+### Bug Fixes
+
+ - <csr-id-9fe3676efa853b79af85e2e1f6bb7849c013a0ec/> speed options
+ - <csr-id-066ca9427211f5147f9528e66a342111e273296f/> rework fiberdata to consume bam record to avoid extra copy
+
+### New Features
+
+ - <csr-id-3ea32b01fda3e12f0cacae90d5a52495cec0b6bd/> add cpg to python modele and make easier access in the rust basemod api
+ - <csr-id-1f6fea3cf07e1e798649df45d944a5396bf82902/> I have a minimal working python package yay!
+
+### Chore
+
+ - <csr-id-66b98f9f3c2644e79bf72de2ed070fba75b2ba38/> rename iterator
+ - <csr-id-9e8cda2fb47eff101eb3d458cf4599543e7d05a2/> rename iterator
+ - <csr-id-23e6b12a7601afb4aa21454048a53d803ca1bcdf/> rename iterator
+ - <csr-id-b03df77d99a8f28ecd6d43509a43ff92fb300329/> rename iterator
+ - <csr-id-6e8cd6f9f25dcabc15ef2a25595b3a3ee86de241/> docs
+ - <csr-id-79ca845b0e72e832cdc57b1e1b58090a09417936/> docs
+ - <csr-id-41bcd27e9de8654fd46bfb50d3c7efabad59a17e/> docs
+ - <csr-id-66338fd576a66ee230aa4234d072a93b3a3b21d5/> docs
+ - <csr-id-6f910c53a4e0cb7be411b724385e540517f21306/> docs
+ - <csr-id-85d471df45a0c88567857427725852c491c041ff/> docs
+ - <csr-id-c5eb60a8d42616eacfafb871cf4f46fb2fa924c8/> docs
+ - <csr-id-5bd6803c346a409150daea7713878af46995e836/> docs
+ - <csr-id-a59f41d0b2d4b97b277b738f04b23010be8d6449/> docs
+ - <csr-id-7a633d71272a9425ae276d9b846fcda38f6526e5/> docs
+ - <csr-id-8d16055edc4bf9bc5f94d5be42b86b2a2df712c8/> docs
+ - <csr-id-467072ae6419b3ece8329f587467d0d0bf316911/> docs
+ - <csr-id-09994bdbdd3949186d44ecef36199a8d228ea280/> docs
+ - <csr-id-8ea9fb1efc4897e191468ee10aa66500456fa0fc/> docs
+ - <csr-id-82399e6e702033acbb455ef6aea3a9935338d77f/> docs
+ - <csr-id-fd115b7fdb6754d6f6885e901bc34d7364bfc7df/> docs
+ - <csr-id-1d25caf7e8c19f97d39dec8eb69de7219e85621b/> docs
+ - <csr-id-e73e00c849726e4577344ec8e964b3eda93ddbc6/> docs
+ - <csr-id-a3f29cd798fcbeb071fce7ea7041c4e71a98f8f6/> docs
+ - <csr-id-e85afd963f513fe578b2d0f3e368a7ae56b59d84/> docs
+ - <csr-id-580968a9da3c2a66740d01dfcc0d8c574bfd46c8/> docs
+ - <csr-id-6b1e714ccda049aef3199563c03d6f5ec1df9dfa/> docs
+ - <csr-id-c8502ac7cf87d375a5aa9fcf3494a3cf8f43105c/> docs
+ - <csr-id-b9274c2a7064cd615b079b3cc0b44d9e2f4b5e50/> docs
+ - <csr-id-eb44bdaf8280689eb06e536266b64802f509a7b3/> docs
+ - <csr-id-b98edf9f855ae24f81389a5ea481bf0b16dcd794/> python docs
+ - <csr-id-32f01826bbf06ac726464d59eee2769dfe80b138/> python docs
+ - <csr-id-94dfd521a3f637df47c996fd046d1de3cde85776/> python docs
+ - <csr-id-b3fa1c3b218379a3290fbed2382572b5e1c3e091/> python docs
+ - <csr-id-d4b75b1a569d694495bc1e87de651c1bb4e63778/> python docs
+ - <csr-id-73c918f9344fe362f602fa5356b11c9574c5ffec/> python docs
+ - <csr-id-5f635e04085c012d39d8afa362416ca3642fc7c5/> python docs
+ - <csr-id-c86cc585993506c55bd0243936767afe4a5f671c/> python docs
+ - <csr-id-15b825ed80a4b099c9ea9f21f64f1b695e20554a/> python docs
+ - <csr-id-26ef86389490b3161546271bea194e4c8a4a8b7f/> python docs
+ - <csr-id-d953400d9c7f676fea70fee51264c331ba7e1067/> python docs
+ - <csr-id-10bf0df63acca5812e3d2d3ad5134bc75abe73b4/> python docs
+ - <csr-id-cdde18e3b119ef36d57feed2f4740b7bde30c011/> readme
+ - <csr-id-ac1987d33daf7fb7395ed1cf15b311390a15e60c/> add to changelog
+ - <csr-id-2f7c08e2b24a07054d547088ac2c96463a6229d3/> add to changelog
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 1 commit contributed to the release.
- - 0 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 78 commits contributed to the release over the course of 2 calendar days.
+ - 2 days passed between releases.
+ - 48 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release fibertools-rs v0.2.6 ([`e973f17`](https://github.com/fiberseq/fibertools-rs/commit/e973f17def31e7c4731ae10143e6c5be5e01425a))
+    - Release fibertools-rs v0.2.6 ([`ba8df9b`](https://github.com/fiberseq/fibertools-rs/commit/ba8df9b8e918be85beef13411cb3aab588634056))
+    - Release fibertools-rs v0.2.6 ([`1b5dcfa`](https://github.com/fiberseq/fibertools-rs/commit/1b5dcfa18eef69a8e4a3f7e3e514bb5d5ae87b7f))
+    - Release fibertools-rs v0.2.6 ([`5aa1908`](https://github.com/fiberseq/fibertools-rs/commit/5aa19089b0cf0614a7a8d0b4f8dc477d6e808ea5))
+    - Release fibertools-rs v0.2.6 ([`656682a`](https://github.com/fiberseq/fibertools-rs/commit/656682a1b70871df4ca52484351d8296755cbe02))
+    - Release fibertools-rs v0.2.6 ([`2d2f0f9`](https://github.com/fiberseq/fibertools-rs/commit/2d2f0f96800779088138f6671ab81acfb61cdacc))
+    - Release fibertools-rs v0.2.6 ([`b80d856`](https://github.com/fiberseq/fibertools-rs/commit/b80d8567ee7ee899734fa5d2c5fd2b6604d45c78))
+    - Release fibertools-rs v0.2.6 ([`14562fd`](https://github.com/fiberseq/fibertools-rs/commit/14562fd4b9552752ddba160cd3cba04e5f90102b))
+    - Try again ([`4aa06eb`](https://github.com/fiberseq/fibertools-rs/commit/4aa06eb00c66afb2e5c0273247b81dbabfa15417))
+    - Release fibertools-rs v0.2.6 ([`e247747`](https://github.com/fiberseq/fibertools-rs/commit/e24774703e6addefabcbe4b1a4df0a91383bdfa8))
+    - Try again ([`09da733`](https://github.com/fiberseq/fibertools-rs/commit/09da733566d266063c7d74cbd610da2fe33b5f2f))
+    - Release fibertools-rs v0.2.6 ([`9b1c3f2`](https://github.com/fiberseq/fibertools-rs/commit/9b1c3f2241dce70ece8ded8feeed19251687d1b1))
+    - Release fibertools-rs v0.2.6 ([`0c525b5`](https://github.com/fiberseq/fibertools-rs/commit/0c525b5e0d6d81a1a82dd14a7fb6ea3c500c8c35))
+    - Py-ft release ([`4de2b11`](https://github.com/fiberseq/fibertools-rs/commit/4de2b11dbcdec8836b53d0abef5444f87fd8c372))
+    - Py-ft release ([`b909bc8`](https://github.com/fiberseq/fibertools-rs/commit/b909bc8df6adda1e0cef2ce6198c14e44ba6cbeb))
+    - Larger chunks not worth ([`911bf40`](https://github.com/fiberseq/fibertools-rs/commit/911bf40a22eaace2afe659efc1000808078792fa))
+    - Larger chunks ([`171cf51`](https://github.com/fiberseq/fibertools-rs/commit/171cf5104464aea984c8c1266835a2f385e49fa0))
+    - Speed options ([`9fe3676`](https://github.com/fiberseq/fibertools-rs/commit/9fe3676efa853b79af85e2e1f6bb7849c013a0ec))
+    - Rework fiberdata to consume bam record to avoid extra copy ([`066ca94`](https://github.com/fiberseq/fibertools-rs/commit/066ca9427211f5147f9528e66a342111e273296f))
+    - Clippy ([`ecd0a61`](https://github.com/fiberseq/fibertools-rs/commit/ecd0a61bf1518476fa19be4c77554c68076b96fd))
+    - Update rusthtslib version ([`d262afa`](https://github.com/fiberseq/fibertools-rs/commit/d262afac986cf53e97f3a53d41c87d605231c03e))
+    - Move bam tags into bio_io ([`abcbcda`](https://github.com/fiberseq/fibertools-rs/commit/abcbcda65a9006c21c892bfdff509cf6e7e55c55))
+    - Add logging and iterator and aligned blocks ([`7671998`](https://github.com/fiberseq/fibertools-rs/commit/76719983d8104a04cabd9846a5529f8e65fc7f96))
+    - Rename iterator ([`66b98f9`](https://github.com/fiberseq/fibertools-rs/commit/66b98f9f3c2644e79bf72de2ed070fba75b2ba38))
+    - Rename iterator ([`9e8cda2`](https://github.com/fiberseq/fibertools-rs/commit/9e8cda2fb47eff101eb3d458cf4599543e7d05a2))
+    - Rename iterator ([`23e6b12`](https://github.com/fiberseq/fibertools-rs/commit/23e6b12a7601afb4aa21454048a53d803ca1bcdf))
+    - Rename iterator ([`b03df77`](https://github.com/fiberseq/fibertools-rs/commit/b03df77d99a8f28ecd6d43509a43ff92fb300329))
+    - Docs ([`6e8cd6f`](https://github.com/fiberseq/fibertools-rs/commit/6e8cd6f9f25dcabc15ef2a25595b3a3ee86de241))
+    - Docs ([`79ca845`](https://github.com/fiberseq/fibertools-rs/commit/79ca845b0e72e832cdc57b1e1b58090a09417936))
+    - Add cpg to python modele and make easier access in the rust basemod api ([`3ea32b0`](https://github.com/fiberseq/fibertools-rs/commit/3ea32b01fda3e12f0cacae90d5a52495cec0b6bd))
+    - Docs ([`41bcd27`](https://github.com/fiberseq/fibertools-rs/commit/41bcd27e9de8654fd46bfb50d3c7efabad59a17e))
+    - Docs ([`66338fd`](https://github.com/fiberseq/fibertools-rs/commit/66338fd576a66ee230aa4234d072a93b3a3b21d5))
+    - Docs ([`6f910c5`](https://github.com/fiberseq/fibertools-rs/commit/6f910c53a4e0cb7be411b724385e540517f21306))
+    - Docs ([`85d471d`](https://github.com/fiberseq/fibertools-rs/commit/85d471df45a0c88567857427725852c491c041ff))
+    - Docs ([`c5eb60a`](https://github.com/fiberseq/fibertools-rs/commit/c5eb60a8d42616eacfafb871cf4f46fb2fa924c8))
+    - Docs ([`5bd6803`](https://github.com/fiberseq/fibertools-rs/commit/5bd6803c346a409150daea7713878af46995e836))
+    - Docs ([`a59f41d`](https://github.com/fiberseq/fibertools-rs/commit/a59f41d0b2d4b97b277b738f04b23010be8d6449))
+    - Docs ([`7a633d7`](https://github.com/fiberseq/fibertools-rs/commit/7a633d71272a9425ae276d9b846fcda38f6526e5))
+    - Docs ([`8d16055`](https://github.com/fiberseq/fibertools-rs/commit/8d16055edc4bf9bc5f94d5be42b86b2a2df712c8))
+    - Docs ([`467072a`](https://github.com/fiberseq/fibertools-rs/commit/467072ae6419b3ece8329f587467d0d0bf316911))
+    - Docs ([`09994bd`](https://github.com/fiberseq/fibertools-rs/commit/09994bdbdd3949186d44ecef36199a8d228ea280))
+    - Docs ([`8ea9fb1`](https://github.com/fiberseq/fibertools-rs/commit/8ea9fb1efc4897e191468ee10aa66500456fa0fc))
+    - Docs ([`82399e6`](https://github.com/fiberseq/fibertools-rs/commit/82399e6e702033acbb455ef6aea3a9935338d77f))
+    - Docs ([`fd115b7`](https://github.com/fiberseq/fibertools-rs/commit/fd115b7fdb6754d6f6885e901bc34d7364bfc7df))
+    - Docs ([`1d25caf`](https://github.com/fiberseq/fibertools-rs/commit/1d25caf7e8c19f97d39dec8eb69de7219e85621b))
+    - Docs ([`e73e00c`](https://github.com/fiberseq/fibertools-rs/commit/e73e00c849726e4577344ec8e964b3eda93ddbc6))
+    - Docs ([`a3f29cd`](https://github.com/fiberseq/fibertools-rs/commit/a3f29cd798fcbeb071fce7ea7041c4e71a98f8f6))
+    - Docs ([`e85afd9`](https://github.com/fiberseq/fibertools-rs/commit/e85afd963f513fe578b2d0f3e368a7ae56b59d84))
+    - Docs ([`580968a`](https://github.com/fiberseq/fibertools-rs/commit/580968a9da3c2a66740d01dfcc0d8c574bfd46c8))
+    - Docs ([`6b1e714`](https://github.com/fiberseq/fibertools-rs/commit/6b1e714ccda049aef3199563c03d6f5ec1df9dfa))
+    - Docs ([`c8502ac`](https://github.com/fiberseq/fibertools-rs/commit/c8502ac7cf87d375a5aa9fcf3494a3cf8f43105c))
+    - Docs ([`b9274c2`](https://github.com/fiberseq/fibertools-rs/commit/b9274c2a7064cd615b079b3cc0b44d9e2f4b5e50))
+    - Docs ([`eb44bda`](https://github.com/fiberseq/fibertools-rs/commit/eb44bdaf8280689eb06e536266b64802f509a7b3))
+    - Rtd theme ([`44f93a4`](https://github.com/fiberseq/fibertools-rs/commit/44f93a42b1d5cb30fefad99e1b4dcf19f4f7f0c0))
+    - Python docs ([`b98edf9`](https://github.com/fiberseq/fibertools-rs/commit/b98edf9f855ae24f81389a5ea481bf0b16dcd794))
+    - Python docs ([`32f0182`](https://github.com/fiberseq/fibertools-rs/commit/32f01826bbf06ac726464d59eee2769dfe80b138))
+    - Python docs ([`94dfd52`](https://github.com/fiberseq/fibertools-rs/commit/94dfd521a3f637df47c996fd046d1de3cde85776))
+    - Python docs ([`b3fa1c3`](https://github.com/fiberseq/fibertools-rs/commit/b3fa1c3b218379a3290fbed2382572b5e1c3e091))
+    - Python docs ([`d4b75b1`](https://github.com/fiberseq/fibertools-rs/commit/d4b75b1a569d694495bc1e87de651c1bb4e63778))
+    - Python docs ([`73c918f`](https://github.com/fiberseq/fibertools-rs/commit/73c918f9344fe362f602fa5356b11c9574c5ffec))
+    - Python docs ([`5f635e0`](https://github.com/fiberseq/fibertools-rs/commit/5f635e04085c012d39d8afa362416ca3642fc7c5))
+    - Python docs ([`c86cc58`](https://github.com/fiberseq/fibertools-rs/commit/c86cc585993506c55bd0243936767afe4a5f671c))
+    - Python docs ([`15b825e`](https://github.com/fiberseq/fibertools-rs/commit/15b825ed80a4b099c9ea9f21f64f1b695e20554a))
+    - Python docs ([`26ef863`](https://github.com/fiberseq/fibertools-rs/commit/26ef86389490b3161546271bea194e4c8a4a8b7f))
+    - Python docs ([`d953400`](https://github.com/fiberseq/fibertools-rs/commit/d953400d9c7f676fea70fee51264c331ba7e1067))
+    - Python docs ([`10bf0df`](https://github.com/fiberseq/fibertools-rs/commit/10bf0df63acca5812e3d2d3ad5134bc75abe73b4))
+    - Readme ([`cdde18e`](https://github.com/fiberseq/fibertools-rs/commit/cdde18e3b119ef36d57feed2f4740b7bde30c011))
+    - I have a minimal working python package yay! ([`1f6fea3`](https://github.com/fiberseq/fibertools-rs/commit/1f6fea3cf07e1e798649df45d944a5396bf82902))
+    - Start a python package ([`7e5fbde`](https://github.com/fiberseq/fibertools-rs/commit/7e5fbde9f0f52496fd1f2facbbd55d80d0b64a26))
+    - Add to changelog ([`ac1987d`](https://github.com/fiberseq/fibertools-rs/commit/ac1987d33daf7fb7395ed1cf15b311390a15e60c))
+    - Add to changelog ([`2f7c08e`](https://github.com/fiberseq/fibertools-rs/commit/2f7c08e2b24a07054d547088ac2c96463a6229d3))
+    - Merge pull request #19 from fiberseq/development ([`202025d`](https://github.com/fiberseq/fibertools-rs/commit/202025dcdefdf88e0754ac78be03731c707c0b1b))
+    - Update docs ([`c61762b`](https://github.com/fiberseq/fibertools-rs/commit/c61762b423129c7428ca946981febec491a9d853))
+    - Update changelog ([`75a3a32`](https://github.com/fiberseq/fibertools-rs/commit/75a3a320729cfcedb3c99fd084cb2db16104ed70))
+    - Unsed ([`4bc52a2`](https://github.com/fiberseq/fibertools-rs/commit/4bc52a229ef8be46eac45f765cfec6842d5d1d36))
+    - Start a changelog ([`2aa57f5`](https://github.com/fiberseq/fibertools-rs/commit/2aa57f5fc1d7c38701964afea6ed5c20a76eb0d2))
     - Reorganize test data ([`966ac80`](https://github.com/fiberseq/fibertools-rs/commit/966ac80890e820da571164e01e360fc4c5507845))
+    - Merge pull request #18 from fiberseq/development ([`2369f27`](https://github.com/fiberseq/fibertools-rs/commit/2369f2702c9caeb18d6c8475c9d1a52a6cbe423e))
 </details>
 
 ## v0.2.5 (2023-07-18)
 
+<csr-id-082190756233e077b692839f979df466fd5c7239/>
+
 The default output for `ft extract` is now in reference coordinates instead of molecular.
 
 `ft extract` can now produce compressed files by adding the gz extension. e.g.:
 ```
 ft extract -t 16 --m6a m6a.bed.gz --cpg cpg.bed.gz --nuc nuc.bed.gz --msp msp.bed.gz --all all.bed.gz ../PS00243_ft.bam
 ```
 And this is `bgzp` compression, so it is compatible with `tabix` indexing. 
@@ -39,15 +221,15 @@
 
  - <csr-id-082190756233e077b692839f979df466fd5c7239/> Release fibertools-rs version 0.2.5
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 9 commits contributed to the release over the course of 5 calendar days.
+ - 11 commits contributed to the release over the course of 6 calendar days.
  - 6 days passed between releases.
  - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
@@ -57,30 +239,34 @@
  * **Uncategorized**
     - Release fibertools-rs version 0.2.5 ([`0821907`](https://github.com/fiberseq/fibertools-rs/commit/082190756233e077b692839f979df466fd5c7239))
     - Irnogre ([`938df0e`](https://github.com/fiberseq/fibertools-rs/commit/938df0e7e1aa88d05eb8b7e247eb88370e11d2b7))
     - Correct path ([`ac0166b`](https://github.com/fiberseq/fibertools-rs/commit/ac0166bb5cc1ac8b0b93df71ced2f8fd7689564f))
     - Better var name ([`fb3ad6d`](https://github.com/fiberseq/fibertools-rs/commit/fb3ad6d7c35e930cfb1ead67d494844eea62de93))
     - Fix off by one that sometimes happened in the final msp when doing nuc/msp calling ([`da5763d`](https://github.com/fiberseq/fibertools-rs/commit/da5763d24a322db2f1e6bdc53af57358776a51f4))
     - Fix off by one in minus strand nuc and msp coordiantes ([`91e2bc5`](https://github.com/fiberseq/fibertools-rs/commit/91e2bc558ab94b85e1ede25dccb2bf0e2878a023))
+    - Merge pull request #17 from fiberseq/development ([`8f3d278`](https://github.com/fiberseq/fibertools-rs/commit/8f3d278d3285f8b5eafd429d5e6174b79adbbc49))
     - Check for bgz ([`14724dd`](https://github.com/fiberseq/fibertools-rs/commit/14724dd9270db0af9c12434fbc40252fd684b2fd))
     - Rewrite ft center so I can use threads? ([`7180f8e`](https://github.com/fiberseq/fibertools-rs/commit/7180f8e126a72fa49c4761e166bde1535c306aa2))
     - Rewrite ft center so I can use threads? ([`4485c5e`](https://github.com/fiberseq/fibertools-rs/commit/4485c5e46534b3bcdebf2295709e06830b404279))
+    - Merge pull request #16 from fiberseq/development ([`759ee9f`](https://github.com/fiberseq/fibertools-rs/commit/759ee9fae9484f20255ae90b431587302c1f1cba))
 </details>
 
 ## v0.2.4 (2023-07-11)
 
+<csr-id-98a51ab3030ed03ce6adc7e160ee7feed49a7222/>
+
 ### Chore
 
  - <csr-id-98a51ab3030ed03ce6adc7e160ee7feed49a7222/> Release fibertools-rs version 0.2.4
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 21 commits contributed to the release over the course of 13 calendar days.
+ - 22 commits contributed to the release over the course of 13 calendar days.
  - 17 days passed between releases.
  - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
@@ -89,14 +275,15 @@
 
  * **Uncategorized**
     - Release fibertools-rs version 0.2.4 ([`98a51ab`](https://github.com/fiberseq/fibertools-rs/commit/98a51ab3030ed03ce6adc7e160ee7feed49a7222))
     - Unsed deps ([`4603bb6`](https://github.com/fiberseq/fibertools-rs/commit/4603bb6920fd42e0c74d2b8d240d50b2d34c8a02))
     - Unsed deps ([`b542514`](https://github.com/fiberseq/fibertools-rs/commit/b542514c3353d5afba985763a51645a10cacdf1e))
     - Ci ([`60c065e`](https://github.com/fiberseq/fibertools-rs/commit/60c065e0515df493957929a0de16f916300df761))
     - Bio-io updates ([`8615452`](https://github.com/fiberseq/fibertools-rs/commit/8615452ba8743caa7b46c39f7acb583abe7ee129))
+    - Merge pull request #15 from fiberseq/development ([`d8cfd67`](https://github.com/fiberseq/fibertools-rs/commit/d8cfd6773c37691c4aac73837a5124f9c7f4c6b7))
     - Change extract defaults ([`b009dda`](https://github.com/fiberseq/fibertools-rs/commit/b009ddacc3c07f9f86562ce25d987d04ab717c11))
     - CI ([`57880cc`](https://github.com/fiberseq/fibertools-rs/commit/57880cc16b29cbc250f9dfbf68dffd3c99f3c0fa))
     - Rename ([`a00e0d3`](https://github.com/fiberseq/fibertools-rs/commit/a00e0d30cf80d6ac987d4bfbcaa0bf46b128a067))
     - Set vars ([`eedb613`](https://github.com/fiberseq/fibertools-rs/commit/eedb613c2f4374ba826d1a8bca5402b97d5ccdee))
     - Fix version in bamwriter ([`c3e3781`](https://github.com/fiberseq/fibertools-rs/commit/c3e378118394b9d2deb8d7dde45ac7de28b48a3b))
     - Adding a compressed bgzip writer for files with .gz ([`e425ee3`](https://github.com/fiberseq/fibertools-rs/commit/e425ee32388b2870ae80e644af3f83d6ec167279))
     - Adding a buff reader that can be compressed optionally ([`4235b77`](https://github.com/fiberseq/fibertools-rs/commit/4235b7768e2530e0721cf70c9181811066ff9b75))
@@ -109,14 +296,16 @@
     - Add HTSlib ([`fd058ba`](https://github.com/fiberseq/fibertools-rs/commit/fd058bac7084510f4c652c1da7e59df0db26bc77))
     - Put ft in a path that doesn't need root access ([`b024da2`](https://github.com/fiberseq/fibertools-rs/commit/b024da202fe250d89c59d4860639b9429ace8a36))
     - Uncomment compile line ([`d792d98`](https://github.com/fiberseq/fibertools-rs/commit/d792d98b46ec2b46c36ba3837a06db424c3acba7))
 </details>
 
 ## v0.2.3 (2023-06-24)
 
+<csr-id-6bb81e5a15f2f18bfe1a31b2ba207248e6a4e7b2/>
+
 ### Chore
 
  - <csr-id-6bb81e5a15f2f18bfe1a31b2ba207248e6a4e7b2/> Release fibertools-rs version 0.2.3
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -153,14 +342,16 @@
     - Simplify ([`5920f5b`](https://github.com/fiberseq/fibertools-rs/commit/5920f5bdc2af15812a5b335a5703be53dacc86ca))
     - Moving bamlift to its own crate ([`efd2a8b`](https://github.com/fiberseq/fibertools-rs/commit/efd2a8b6bf4e7ffe16ad3f91701cace194ea3967))
     - Moving bamlift to its own crate ([`ccd0969`](https://github.com/fiberseq/fibertools-rs/commit/ccd096963fe46b7ccbe00781b0da99cab87388ef))
 </details>
 
 ## v0.2.2 (2023-06-15)
 
+<csr-id-7cd3d115ffa9c824218ac8ea9f2454682cb91ca9/>
+
 ### Chore
 
  - <csr-id-7cd3d115ffa9c824218ac8ea9f2454682cb91ca9/> Release fibertools-rs version 0.2.2
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -180,14 +371,16 @@
     - Add run tests and fix comments in bed files for center ([`8e00047`](https://github.com/fiberseq/fibertools-rs/commit/8e00047cdd769ad03a7e79197bfeb0e4bf00e6c4))
     - Add run tests ([`b5d1e8e`](https://github.com/fiberseq/fibertools-rs/commit/b5d1e8eca77d7fefec5eece5330f00a1e50abac9))
     - Hide some subcommands ([`03e7006`](https://github.com/fiberseq/fibertools-rs/commit/03e7006ab662e8fbb2ed0d3e11f7ffe1946ba4f1))
 </details>
 
 ## v0.2.1 (2023-06-14)
 
+<csr-id-53094a13be5fdc883bd87e46940bf93d48e41b1c/>
+
 ### Chore
 
  - <csr-id-53094a13be5fdc883bd87e46940bf93d48e41b1c/> Release fibertools-rs version 0.2.1
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -209,14 +402,16 @@
     - Remove unused libs ([`fedd892`](https://github.com/fiberseq/fibertools-rs/commit/fedd892e1d360acb93b26f42a8b4d369c3fa8a48))
     - Bring back the colors ([`d336911`](https://github.com/fiberseq/fibertools-rs/commit/d3369115667fc7887eaf786de9f78a9f5504399f))
     - Bring back the colors ([`0af601a`](https://github.com/fiberseq/fibertools-rs/commit/0af601a8b6f8905be3ec79a0cc6db96bba940e61))
 </details>
 
 ## v0.2.0 (2023-06-10)
 
+<csr-id-cd387947c4aafd5d70d087650e1e5fe929808e81/>
+
 ### Chore
 
  - <csr-id-cd387947c4aafd5d70d087650e1e5fe929808e81/> Release fibertools-rs version 0.2.0
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -252,14 +447,16 @@
     - Make logging more clear ([`ed8785a`](https://github.com/fiberseq/fibertools-rs/commit/ed8785ab203c7566426f220e2f6095e7bd6078b2))
     - Readme ([`2e25423`](https://github.com/fiberseq/fibertools-rs/commit/2e2542385974f2e584fcfe42b0bd76dedfefa6f3))
     - Readme ([`715e25d`](https://github.com/fiberseq/fibertools-rs/commit/715e25d9bbe82b36910984944b9ff3108a8f3bf3))
 </details>
 
 ## v0.1.4 (2023-04-19)
 
+<csr-id-4f95956d0a60a75b6b1a4d446829935426b2ffaf/>
+
 ### Chore
 
  - <csr-id-4f95956d0a60a75b6b1a4d446829935426b2ffaf/> Release fibertools-rs version 0.1.4
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -320,14 +517,16 @@
     - Adding a command that lets me add simple nuc calls ([`819a90b`](https://github.com/fiberseq/fibertools-rs/commit/819a90bd1255bbd8298ee60fde55b16a1bfccfe2))
     - Adding a command that lets me add simple nuc calls ([`33e0ee8`](https://github.com/fiberseq/fibertools-rs/commit/33e0ee84f8457d85ea52f45a430a61fcdc20dd8c))
     - Adding a command that lets me add simple nuc calls ([`cd3ec8f`](https://github.com/fiberseq/fibertools-rs/commit/cd3ec8fb718cf9353f43348b2b2c9741117f96d1))
 </details>
 
 ## v0.1.3 (2023-03-14)
 
+<csr-id-84e4ee9e1ae31396f8743d9d02c1af02dbe84bb7/>
+
 ### Chore
 
  - <csr-id-84e4ee9e1ae31396f8743d9d02c1af02dbe84bb7/> Release fibertools-rs version 0.1.3
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -354,14 +553,16 @@
     - Add the option to read the ML models from env variables FT_MODEL and FT_JSON ([`8314d8e`](https://github.com/fiberseq/fibertools-rs/commit/8314d8e62b21efe929c4e16c7509e7dd2bc312e4))
     - Add RG to extract ([`355088e`](https://github.com/fiberseq/fibertools-rs/commit/355088e59eac4c726b1d30212da3cc46d8bc59c2))
     - Theads help msg ([`595db94`](https://github.com/fiberseq/fibertools-rs/commit/595db94ef3b844ce49d829c25d79ee4b6d97f44d))
 </details>
 
 ## v0.1.2 (2023-02-13)
 
+<csr-id-7df4056ecc335f5be92f5688215a156623f927cd/>
+
 ### Chore
 
  - <csr-id-7df4056ecc335f5be92f5688215a156623f927cd/> Release fibertools-rs version 0.1.2
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -381,14 +582,17 @@
     - Release fibertools-rs version 0.1.2 ([`7df4056`](https://github.com/fiberseq/fibertools-rs/commit/7df4056ecc335f5be92f5688215a156623f927cd))
     - Remvoe libtorch check since it is packaged in conda now ([`28c3614`](https://github.com/fiberseq/fibertools-rs/commit/28c3614ee3913451b3eb81697f904f104160930b))
     - Update url for new repo ([`021ae38`](https://github.com/fiberseq/fibertools-rs/commit/021ae389cf520391b5d3ccb066ffa8952ea32997))
 </details>
 
 ## v0.1.1 (2023-02-02)
 
+<csr-id-9f8f35b4f75ae3a944d137a8fd7bb562529a634e/>
+<csr-id-d8f2ea597075a4f13be9d1d68c173c2476c02f63/>
+
 ### Chore
 
  - <csr-id-9f8f35b4f75ae3a944d137a8fd7bb562529a634e/> Release fibertools-rs version 0.1.1
  - <csr-id-d8f2ea597075a4f13be9d1d68c173c2476c02f63/> Release fibertools-rs version 0.1.1-alpha.4
 
 ### Commit Statistics
 
@@ -411,14 +615,16 @@
     - Fix ci ([`2d6fa56`](https://github.com/fiberseq/fibertools-rs/commit/2d6fa5617c814b651ee1f0e8f7214696c772d271))
     - Release fibertools-rs version 0.1.1-alpha.4 ([`d8f2ea5`](https://github.com/fiberseq/fibertools-rs/commit/d8f2ea597075a4f13be9d1d68c173c2476c02f63))
     - Restor version of ubunut ([`6ace556`](https://github.com/fiberseq/fibertools-rs/commit/6ace556673fe953e3bbdc50fbe9abff59e59aa0a))
 </details>
 
 ## v0.1.1-alpha.3 (2023-02-01)
 
+<csr-id-c1161138edd4b1bd7153a1cc5b724bb2eef29a4c/>
+
 ### Chore
 
  - <csr-id-c1161138edd4b1bd7153a1cc5b724bb2eef29a4c/> Release fibertools-rs version 0.1.1-alpha.3
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -436,14 +642,16 @@
  * **Uncategorized**
     - Release fibertools-rs version 0.1.1-alpha.3 ([`c116113`](https://github.com/fiberseq/fibertools-rs/commit/c1161138edd4b1bd7153a1cc5b724bb2eef29a4c))
     - Older version of ubunut ([`a043398`](https://github.com/fiberseq/fibertools-rs/commit/a04339858db5f2944f3a46be44eb2c3c367f1939))
 </details>
 
 ## v0.1.1-alpha.2 (2023-02-01)
 
+<csr-id-dda2ea4236a46e4cba2ac0f7415a871c09f5777a/>
+
 ### Chore
 
  - <csr-id-dda2ea4236a46e4cba2ac0f7415a871c09f5777a/> Release fibertools-rs version 0.1.1-alpha.2
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -461,14 +669,16 @@
  * **Uncategorized**
     - Release fibertools-rs version 0.1.1-alpha.2 ([`dda2ea4`](https://github.com/fiberseq/fibertools-rs/commit/dda2ea4236a46e4cba2ac0f7415a871c09f5777a))
     - Adding libtorch enviorment checks ([`3d0c77c`](https://github.com/fiberseq/fibertools-rs/commit/3d0c77c3bc89b1e6cce43e27ef1e92190339dcb2))
 </details>
 
 ## v0.1.1-alpha.1 (2023-02-01)
 
+<csr-id-c6f50df845bcd931b61cfa8151e4d38b1c9ccbdd/>
+
 ### Chore
 
  - <csr-id-c6f50df845bcd931b61cfa8151e4d38b1c9ccbdd/> Release fibertools-rs version 0.1.1-alpha.1
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
@@ -486,14 +696,16 @@
  * **Uncategorized**
     - Release fibertools-rs version 0.1.1-alpha.1 ([`c6f50df`](https://github.com/fiberseq/fibertools-rs/commit/c6f50df845bcd931b61cfa8151e4d38b1c9ccbdd))
     - Change targets ([`1ad406a`](https://github.com/fiberseq/fibertools-rs/commit/1ad406a1de44d64ea84002442a9cab1d269d1ef8))
 </details>
 
 ## v0.1.1-alpha (2023-02-01)
 
+<csr-id-3eede8cd716b8a03090a6f5dcc593460c6a943a1/>
+
 ### Chore
 
  - <csr-id-3eede8cd716b8a03090a6f5dcc593460c6a943a1/> Release fibertools-rs version 0.1.1-alpha
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/Cargo.lock` & `pyft-0.1.3/local_dependencies/fibertools-rs/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bamlift"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "env_logger",
  "log",
  "rust-htslib",
 ]
 
 [[package]]
@@ -185,15 +185,15 @@
  "thiserror",
  "triple_accel",
  "vec_map",
 ]
 
 [[package]]
 name = "bio-io"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "colored",
  "gzp",
  "itertools",
  "lazy_static",
  "log",
@@ -709,15 +709,15 @@
 name = "feature-probe"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "835a3dc7d1ec9e75e2b5fb4ba75396837112d2060b03f7d43bc1897c7f7211da"
 
 [[package]]
 name = "fibertools-rs"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "anstyle",
  "anyhow",
  "assert_cmd",
  "bamlift",
  "bio",
  "bio-io",
@@ -952,17 +952,17 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "hts-sys"
-version = "2.0.3"
+version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dba4fc406d3686926c84f98fd53026b625319d119e6056a40313862a6e3c4eb"
+checksum = "deebfb779c734d542e7f14c298597914b9b5425e4089aef482eacb5cab941915"
 dependencies = [
  "bzip2-sys",
  "cc",
  "curl-sys",
  "fs-utils",
  "glob",
  "libz-sys",
@@ -1781,17 +1781,17 @@
 name = "roff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b833d8d034ea094b1ea68aa6d5c740e0d04bad9d16568d08ba6f76823a114316"
 
 [[package]]
 name = "rust-htslib"
-version = "0.43.1"
+version = "0.44.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53881800f22b91fa893cc3f6d70e6e9aa96d200133bfe112e36aee37aad70bf5"
+checksum = "7c7eb0f29fce64a4e22578905efef3d72389058016023279a58b282eb5c0c467"
 dependencies = [
  "bio-types",
  "byteorder",
  "custom_derive",
  "derive-new",
  "hts-sys",
  "ieee754",
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/Dockerfile` & `pyft-0.1.3/local_dependencies/fibertools-rs/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/INSTALL.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/README.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 # TODO items
 - [ ] Add a python API (see py-ft for progress)
 - [ ] Use new iterator for `ft extract` and group writes to try and improve the speed
 - [x] Set filters for ML depending on the model used
 - [ ] long format extract command
 - [ ] add option result to bamlift
+- [ ] improve speed of liftover closest in bamlift. It takes about 50% of the time. 
 - [x] Add more test cases, learn about test modules in folders
 - [x] GPU support
     - [ ] see if I can simplify or statically link PyTorch to get it onto bioconda
     - [ ] Detect GPU memory to set batch size dynamically.
 - [ ] Improve progress bar for predict-m6a.
     - [ ] Get size of bam, say how far we are through the bam in terms of MB/GB?
 - [ ] Add unaligned, secondary, supplemental reads to the test bam.
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/center.png` & `pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/center.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png` & `pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png` & `pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png` & `pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/assets/img/logo.png` & `pyft-0.1.3/local_dependencies/fibertools-rs/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/build.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/build.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft--help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft--help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-center-help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-center-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-extract-help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-extract-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/docs/make_help_docs.sh` & `pyft-0.1.3/local_dependencies/fibertools-rs/docs/make_help_docs.sh`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_semi_torch.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.0_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.0_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_semi_torch.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/2.2_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/2.2_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/3.2_semi_torch.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/3.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/Revio_semi_torch.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/Revio_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json` & `pyft-0.1.3/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/basemods/mod.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/basemods/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 use bamlift::*;
 use bio::alphabets::dna::revcomp;
+use bio_io::*;
 use itertools::{izip, multiunzip};
 use lazy_static::lazy_static;
 use regex::Regex;
 use rust_htslib::{
     bam,
     bam::record::{Aux, AuxArray},
 };
+use std::collections::HashMap;
+
 use std::convert::TryFrom;
 
-#[derive(Eq, PartialEq, Debug)]
+#[derive(Eq, PartialEq, Debug, PartialOrd, Ord)]
 pub struct BaseMod {
     pub modified_base: u8,
     pub strand: char,
     pub modification_type: char,
     record_is_reverse: bool,
     modified_bases: Vec<i64>,
     modified_bases_forward: Vec<i64>,
@@ -91,14 +94,21 @@
 #[derive(Eq, PartialEq, Debug)]
 pub struct BaseMods {
     pub base_mods: Vec<BaseMod>,
 }
 
 impl BaseMods {
     pub fn new(record: &bam::Record, min_ml_score: u8) -> BaseMods {
+        // my basemod parser is ~25% faster than rust_htslib's
+        // let new = BaseMods::rust_htslib_mm_ml_parser(record, min_ml_score);
+        //assert_eq!(new, old);
+        BaseMods::my_mm_ml_parser(record, min_ml_score)
+    }
+
+    pub fn my_mm_ml_parser(record: &bam::Record, min_ml_score: u8) -> BaseMods {
         // regex for matching the MM tag
         lazy_static! {
             static ref MM_RE: Regex =
                 Regex::new(r"((([ACGTUN])([-+])([a-z]+|[0-9]+))[.?]?((,[0-9]+)*;)*)").unwrap();
         }
         // Array to store all the different modifications within the MM tag
         let mut rtn = vec![];
@@ -176,14 +186,18 @@
                 let (modified_probabilities, modified_positions): (Vec<u8>, Vec<i64>) =
                     unfiltered_modified_probabilities
                         .iter()
                         .zip(unfiltered_modified_positions.iter())
                         .filter(|(&ml, &_mm)| ml >= min_ml_score)
                         .unzip();
 
+                // don't add empty basemods
+                if modified_positions.is_empty() {
+                    continue;
+                }
                 // add to a struct
                 let mods = BaseMod::new(
                     record,
                     mod_base,
                     mod_strand.chars().next().unwrap(),
                     modification_type.chars().next().unwrap(),
                     modified_positions,
@@ -198,18 +212,74 @@
         if ml_tag.len() != num_mods_seen {
             log::warn!(
                 "ML tag ({}) different number than MM tag ({}).",
                 ml_tag.len(),
                 num_mods_seen
             );
         }
+        // needed so I can compare methods
+        rtn.sort();
+        BaseMods { base_mods: rtn }
+    }
 
+    pub fn hashmap_to_basemods(
+        map: HashMap<(i32, i32, i32), Vec<(i64, u8)>>,
+        record: &bam::Record,
+    ) -> BaseMods {
+        let mut rtn = vec![];
+        for (mod_info, mods) in map {
+            let mod_base = mod_info.0 as u8;
+            let mod_type = mod_info.1 as u8 as char;
+            let mod_strand = if mod_info.2 == 0 { '+' } else { '-' };
+            let (mut positions, mut qualities): (Vec<i64>, Vec<u8>) = mods.into_iter().unzip();
+            if record.is_reverse() {
+                let length = record.seq_len() as i64;
+                positions = positions
+                    .into_iter()
+                    .rev()
+                    .map(|p| length - p - 1)
+                    .collect();
+                qualities.reverse();
+            }
+            let mods = BaseMod::new(record, mod_base, mod_strand, mod_type, positions, qualities);
+            rtn.push(mods);
+        }
+        // needed so I can compare methods
+        rtn.sort();
         BaseMods { base_mods: rtn }
     }
 
+    /// this is actually way slower than my parser for some reason...
+    /// so I am not going to use it
+    pub fn rust_htslib_mm_ml_parser(record: &bam::Record, min_ml_score: u8) -> BaseMods {
+        let mut base_mods = HashMap::new();
+
+        match record.basemods_iter() {
+            Ok(mods) => {
+                for bp in mods {
+                    let (pos, m) = bp.unwrap();
+                    if min_ml_score > m.qual as u8 {
+                        continue;
+                    }
+                    let z = (m.canonical_base, m.modified_base, m.strand);
+                    let cur_mod = base_mods.entry(z).or_insert(vec![]);
+                    cur_mod.push((pos as i64, m.qual as u8));
+                    continue;
+                }
+            }
+            _ => {
+                return {
+                    log::warn!("Rust hts-lib failed to parse basemods, trying custom parser.");
+                    BaseMods::my_mm_ml_parser(record, min_ml_score)
+                }
+            }
+        }
+        BaseMods::hashmap_to_basemods(base_mods, record)
+    }
+
     /// remove m6a base mods from the struct
     pub fn drop_m6a(&mut self) {
         self.base_mods.retain(|bm| !bm.is_m6a());
     }
 
     /// remove cpg/5mc base mods from the struct
     pub fn drop_cpg(&mut self) {
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/center.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/center.rs`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     header_view: &rust_htslib::bam::HeaderView,
     center_position: CenterPosition,
     min_ml_score: u8,
     wide: bool,
     dist: Option<i64>,
     reference: bool,
 ) {
-    let fiber_data = FiberseqData::from_records(&records, header_view, min_ml_score);
+    let fiber_data = FiberseqData::from_records(records, header_view, min_ml_score);
     let total = fiber_data.len();
     let mut seen = 0;
 
     fiber_data
         .into_par_iter()
         .map(|fiber| {
             match CenteredFiberData::new(fiber, center_position.clone(), dist, reference) {
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/cli.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/cli.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/extract.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/extract.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,39 +19,39 @@
     pub ref_msp: Vec<(i64, i64)>,
     pub base_mods: BaseMods,
     pub ec: f32,
     pub target_name: String,
 }
 
 impl FiberseqData {
-    pub fn new(record: &bam::Record, target_name: Option<&String>, min_ml_score: u8) -> Self {
-        let mut nuc_starts = get_u32_tag(record, b"ns");
-        let mut msp_starts = get_u32_tag(record, b"as");
-        let mut nuc_length = get_u32_tag(record, b"nl");
-        let mut msp_length = get_u32_tag(record, b"al");
+    pub fn new(record: bam::Record, target_name: Option<&String>, min_ml_score: u8) -> Self {
+        let mut nuc_starts = get_u32_tag(&record, b"ns");
+        let mut msp_starts = get_u32_tag(&record, b"as");
+        let mut nuc_length = get_u32_tag(&record, b"nl");
+        let mut msp_length = get_u32_tag(&record, b"al");
         let mut nuc_ends = nuc_starts
             .iter()
             .zip(nuc_length.iter())
             .map(|(&x, &y)| x + y)
             .collect::<Vec<_>>();
         let mut msp_ends = msp_starts
             .iter()
             .zip(msp_length.iter())
             .map(|(&x, &y)| x + y)
             .collect::<Vec<_>>();
         // get new starts, ends, and lengths in reference orientation
         // i.e. query coordinates in bam format
         if record.is_reverse() {
             (nuc_ends, nuc_starts) = (
-                positions_on_complimented_sequence(record, &nuc_starts),
-                positions_on_complimented_sequence(record, &nuc_ends),
+                positions_on_complimented_sequence(&record, &nuc_starts),
+                positions_on_complimented_sequence(&record, &nuc_ends),
             );
             (msp_ends, msp_starts) = (
-                positions_on_complimented_sequence(record, &msp_starts),
-                positions_on_complimented_sequence(record, &msp_ends),
+                positions_on_complimented_sequence(&record, &msp_starts),
+                positions_on_complimented_sequence(&record, &msp_ends),
             );
 
             // because coordinates are [) we need to modify positions when complements so they remain [) instead of (]
             nuc_starts = nuc_starts.iter().map(|&x| x + 1).collect::<Vec<_>>();
             nuc_ends = nuc_ends.iter().map(|&x| x + 1).collect::<Vec<_>>();
             msp_starts = msp_starts.iter().map(|&x| x + 1).collect::<Vec<_>>();
             msp_ends = msp_ends.iter().map(|&x| x + 1).collect::<Vec<_>>();
@@ -66,16 +66,16 @@
                 .iter()
                 .zip(msp_ends.iter())
                 .map(|(&x, &y)| y - x)
                 .collect::<Vec<_>>();
         }
 
         // range positions
-        let ref_nuc = get_closest_reference_range(&nuc_starts, &nuc_length, record);
-        let ref_msp = get_closest_reference_range(&msp_starts, &msp_length, record);
+        let ref_nuc = get_closest_reference_range(&nuc_starts, &nuc_length, &record);
+        let ref_msp = get_closest_reference_range(&msp_starts, &msp_length, &record);
 
         assert_eq!(ref_nuc.len(), nuc_starts.len());
         assert_eq!(ref_msp.len(), msp_starts.len());
 
         // get the number of passes
         let ec = if let Ok(Aux::Float(f)) = record.aux(b"ec") {
             log::trace!("{f}");
@@ -83,30 +83,31 @@
         } else {
             0.0
         };
         let target_name = match target_name {
             Some(t) => t.clone(),
             None => ".".to_string(),
         };
+        let base_mods = BaseMods::new(&record, min_ml_score);
         //
         FiberseqData {
-            record: record.clone(),
+            record,
             nuc: nuc_starts
                 .iter()
                 .cloned()
                 .zip(nuc_length.iter().cloned())
                 .collect(),
             msp: msp_starts
                 .iter()
                 .cloned()
                 .zip(msp_length.iter().cloned())
                 .collect(),
             ref_nuc,
             ref_msp,
-            base_mods: BaseMods::new(record, min_ml_score),
+            base_mods,
             ec,
             target_name,
         }
     }
 
     pub fn dict_from_head_view(head_view: &HeaderView) -> HashMap<i32, String> {
         let target_u8s = head_view.target_names();
@@ -123,22 +124,25 @@
     }
 
     pub fn target_name_from_tid(tid: i32, target_dict: &HashMap<i32, String>) -> Option<&String> {
         target_dict.get(&tid)
     }
 
     pub fn from_records(
-        records: &Vec<bam::Record>,
+        records: Vec<bam::Record>,
         head_view: &HeaderView,
         min_ml_score: u8,
     ) -> Vec<Self> {
         let target_dict = Self::dict_from_head_view(head_view);
         records
-            .par_iter()
-            .map(|r| (r, Self::target_name_from_tid(r.tid(), &target_dict)))
+            .into_par_iter()
+            .map(|r| {
+                let tid = r.tid();
+                (r, Self::target_name_from_tid(tid, &target_dict))
+            })
             .map(|(r, target_name)| Self::new(r, target_name, min_ml_score))
             .collect::<Vec<_>>()
     }
 
     pub fn get_nuc(&self, reference: bool, get_starts: bool) -> Vec<i64> {
         let (starts, lengths): (Vec<_>, Vec<_>) = if reference {
             self.ref_nuc.iter().map(|(a, b)| (a, b)).unzip()
@@ -475,15 +479,15 @@
         write!(&mut rtn, "{}", format_args!("{}\n", end - start - 1)).unwrap();
         rtn
     }
 }
 
 #[allow(clippy::too_many_arguments)]
 pub fn process_bam_chunk(
-    records: &Vec<bam::Record>,
+    records: Vec<bam::Record>,
     so_far: usize,
     out_files: &mut FiberOut,
     head_view: &HeaderView,
 ) {
     let start = Instant::now();
     let fiber_data = FiberseqData::from_records(records, head_view, out_files.min_ml_score);
 
@@ -547,18 +551,18 @@
         }
         None => {}
     }
 
     let duration = start.elapsed().as_secs_f64();
     log::info!(
         "Processing {}, {} reads done so far.",
-        format!("{:.2?} reads/s", records.len() as f64 / duration)
+        format!("{:.2?} reads/s", fiber_data.len() as f64 / duration)
             .bright_cyan()
             .bold(),
-        format!("{:}", so_far + records.len())
+        format!("{:}", so_far + fiber_data.len())
             .bright_magenta()
             .bold()
     );
 }
 
 pub fn extract_contained(bam: &mut bam::Reader, mut out_files: FiberOut) {
     let header = bam::Header::from_template(bam.header());
@@ -582,11 +586,11 @@
     let chunk_size = current_num_threads() * 500;
     let bam_chunk_iter = BamChunk {
         bam: bam.records(),
         chunk_size,
     };
     let mut processed_reads = 0;
     for chunk in bam_chunk_iter {
-        process_bam_chunk(&chunk, processed_reads, &mut out_files, &head_view);
         processed_reads += chunk.len();
+        process_bam_chunk(chunk, processed_reads, &mut out_files, &head_view);
     }
 }
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/lib.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pub mod predict_m6a;
 /// Remove base modifications from a bam record
 pub mod strip_basemods;
 
 use anyhow::Result;
 use bio_io::*;
 use indicatif::{style, ProgressBar};
+#[cfg(feature = "predict")]
 use itertools::Itertools;
 use rust_htslib::{bam, bam::Read};
 use std::env;
 use std::io::Write;
 
 pub const VERSION: &str = env!("CARGO_PKG_VERSION");
 pub const GIT_HASH: &str = env!("CARGO_GIT_HASH");
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/main.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/nucleosomes.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/nucleosomes.rs`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             .progress_chars("##-");
 
         // add nuc calls
         let records: Vec<&mut Record> = chunk
             .par_iter_mut()
             .progress_with_style(style)
             .map(|record| {
-                let fd = extract::FiberseqData::new(record, None, 0);
+                let fd = extract::FiberseqData::new(record.clone(), None, 0);
                 let m6a = fd.base_mods.forward_m6a();
                 add_nucleosomes_to_record(record, &m6a.0, &options);
                 record
             })
             .collect();
 
         records
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use super::*;
 use anyhow::anyhow;
-use bamlift;
 use bio::alphabets::dna::revcomp;
+use bio_io;
 use indicatif::{style, ParallelProgressIterator};
 use nucleosomes;
 use ordered_float::OrderedFloat;
 use rayon::iter::ParallelIterator;
 use rayon::prelude::IntoParallelRefMutIterator;
 use rayon::{current_num_threads, prelude::IndexedParallelIterator};
 use rust_htslib::{
@@ -277,15 +277,15 @@
             .filter(|&x| *x > -0.00000001)
             .count(),
         predictions.len()
     );
 
     // add full probabilities if needed requested
     if predict_options.full_float {
-        let mut mp = bamlift::get_f32_tag(record, b"mp");
+        let mut mp = bio_io::get_f32_tag(record, b"mp");
         record.remove_aux(b"mp").unwrap_or(());
         mp.extend(&full_probabilities_forward);
         let aux_array: AuxArray<f32> = (&mp).into();
         let aux_array_field = Aux::ArrayFloat(aux_array);
         record.push_aux(b"mp", aux_array_field).unwrap();
     }
 
@@ -318,35 +318,35 @@
             "Skipping secondary alignment of {}",
             String::from_utf8_lossy(record.qname())
         );
         return None;
     }
 
     let extend = WINDOW / 2;
-    let mut f_ip = bamlift::get_u8_tag(record, b"fi");
+    let mut f_ip = bio_io::get_u8_tag(record, b"fi");
     let r_ip;
     let f_pw;
     let r_pw;
     // check if we maybe are getting u16 input instead of u8
     if f_ip.is_empty() {
-        f_ip = bamlift::get_pb_u16_tag_as_u8(record, b"fi");
+        f_ip = bio_io::get_pb_u16_tag_as_u8(record, b"fi");
         if f_ip.is_empty() {
             // missing u16 as well, set all to empty arrays
             r_ip = vec![];
             f_pw = vec![];
             r_pw = vec![];
         } else {
-            r_ip = bamlift::get_pb_u16_tag_as_u8(record, b"ri");
-            f_pw = bamlift::get_pb_u16_tag_as_u8(record, b"fp");
-            r_pw = bamlift::get_pb_u16_tag_as_u8(record, b"rp");
+            r_ip = bio_io::get_pb_u16_tag_as_u8(record, b"ri");
+            f_pw = bio_io::get_pb_u16_tag_as_u8(record, b"fp");
+            r_pw = bio_io::get_pb_u16_tag_as_u8(record, b"rp");
         }
     } else {
-        r_ip = bamlift::get_u8_tag(record, b"ri");
-        f_pw = bamlift::get_u8_tag(record, b"fp");
-        r_pw = bamlift::get_u8_tag(record, b"rp");
+        r_ip = bio_io::get_u8_tag(record, b"ri");
+        f_pw = bio_io::get_u8_tag(record, b"fp");
+        r_pw = bio_io::get_u8_tag(record, b"rp");
     }
     // return if missing kinetics
     if f_ip.is_empty() || r_ip.is_empty() || f_pw.is_empty() || r_pw.is_empty() {
         log::debug!(
             "Hifi kinetics are missing for: {}",
             String::from_utf8_lossy(record.qname())
         );
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/src/strip_basemods.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/src/strip_basemods.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/all.bam` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/all.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/all.bam.bai` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/all.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bam` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bam.bai` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/center.bed` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/center.bed`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/extract_test.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/extract_test.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use rust_htslib::bam::Read;
 
 fn get_fiber_data_from_test_bam(bam_file: &str) -> Vec<fibertools_rs::extract::FiberseqData> {
     let mut bam = bio_io::bam_reader(bam_file, 1);
     bam.records()
         .map(|r| {
             let record = r.unwrap();
-            let fiber_data = fibertools_rs::extract::FiberseqData::new(&record, None, 0);
+            let fiber_data = fibertools_rs::extract::FiberseqData::new(record, None, 0);
             fiber_data
         })
         .collect::<Vec<_>>()
 }
 
 #[test]
 fn test_msp_extract() -> Result<(), Box<dyn std::error::Error>> {
@@ -25,15 +25,15 @@
     assert_eq!(msp_starts, expected_msp_starts);
     Ok(())
 }
 
 #[test]
 fn test_many_msps() {
     let fiber_records = get_fiber_data_from_test_bam("tests/data/all.bam");
-    for mut fiber_data in fiber_records {
+    for fiber_data in fiber_records {
         let m6a = fiber_data.base_mods.m6a_positions(false);
         if m6a.is_empty() {
             continue;
         }
         let msp_starts = fiber_data.get_msp(false, true);
         let msp_lengths = fiber_data.get_msp(false, false);
         let msp_ends = msp_starts
```

### Comparing `pyft-0.1.2/local_dependencies/fibertools-rs/tests/run_test.rs` & `pyft-0.1.3/local_dependencies/fibertools-rs/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/Cargo.toml` & `pyft-0.1.3/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [package]
 edition = "2021"
 name = "pyft"
-version = "0.1.2"
+version = "0.1.3"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "pyft"
 
 [dependencies]
 anyhow = "1.0.58"
 bamlift = {path = "local_dependencies/bamlift" }
 bio-io = {path = "local_dependencies/bio-io" }
 colored = "2.0.0"
+env_logger = "0.10"
 fibertools-rs = {path = "local_dependencies/fibertools-rs", default-features = false}
 itertools = "0.10.5"
 lazy_static = "1.4.0"
 log = "0.4"
 pyo3 = "0.19.0"
 regex = "1.5.4"
-rust-htslib = "0.43.1"
+rust-htslib = "0.44.1"
```

### Comparing `pyft-0.1.2/.github/workflows/CI.yml` & `pyft-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/.gitignore` & `pyft-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/README.md` & `pyft-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/Makefile` & `pyft-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/_static/css/rtd_dark.css` & `pyft-0.1.3/docs/_static/css/rtd_dark.css`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/_static/img/fiber_tools_grey.png` & `pyft-0.1.3/docs/_static/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/conf.py` & `pyft-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/index.rst` & `pyft-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/docs/make.bat` & `pyft-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyft-0.1.2/src/fiberdata.rs` & `pyft-0.1.3/src/fiberdata.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use fibertools_rs::extract::FiberseqData;
+use log;
 use pyo3::iter::IterNextOutput;
 use pyo3::prelude::*;
 use rust_htslib::{bam, bam::ext::BamRecordExtensions, bam::record::Aux, bam::Read};
+use std::vec::IntoIter;
 //use rust_htslib::bam::Read;
 //use std::io::Result;
 
 #[pyclass]
 /// Record class for fiberseq data, corresponding to a single bam record
 pub struct Fiberdata {
     /// Number of ccs passes
@@ -49,31 +51,59 @@
     pub cpg: Basemods,
     /// :class:`~pyft.Ranges` object for msp features
     #[pyo3(get, set)]
     pub msp: Ranges,
     /// :class:`~pyft.Ranges` object for nuc features
     #[pyo3(get, set)]
     pub nuc: Ranges,
+    /// hiden
+    fiber: FiberseqData,
 }
 #[pymethods]
 impl Fiberdata {
     pub fn __str__(&self) -> String {
         format!(
-            "{}\t{}\t{}\t{}\n{:?}",
-            self.qname, self.chrom, self.start, self.end, self.m6a.starts,
+            "fiber: {}\t\
+            chrom: {}\tstart: {}\tend {}\t\
+            num m6a: {}\t num cpg: {}\t\
+            num nuc: {}\t num msp: {}",
+            self.qname,
+            self.chrom,
+            self.start,
+            self.end,
+            self.m6a.starts.len(),
+            self.cpg.starts.len(),
+            self.nuc.starts.len(),
+            self.msp.starts.len()
         )
     }
 
     /// return the length of the sequence
     pub fn get_seq_length(&self) -> usize {
         self.seq.len()
     }
+
+    /// Return a :class:`~pyft.Ranges` object for the continuous aligned regions of the fiber
+    pub fn get_aligned_ranges(&self) -> Ranges {
+        let (fiber, genome): (Vec<[i64; 2]>, Vec<[i64; 2]>) = self
+            .fiber
+            .record
+            .aligned_block_pairs()
+            .collect::<Vec<_>>()
+            .into_iter()
+            .unzip();
+        let starts = fiber.iter().map(|x| x[0]).collect();
+        let lengths = fiber.iter().map(|x| x[1] - x[0]).collect();
+        let reference_starts = genome.iter().map(|x| x[0]).collect();
+        let reference_lengths = genome.iter().map(|x| x[1] - x[0]).collect();
+        Ranges::new(starts, lengths, reference_starts, reference_lengths)
+    }
 }
 
-fn new_py_fiberdata(fiber: &FiberseqData) -> Fiberdata {
+fn new_py_fiberdata(fiber: FiberseqData) -> Fiberdata {
     // PB features
     let ec = fiber.ec.round() as i64;
 
     // record features
     let qname = std::str::from_utf8(fiber.record.qname()).unwrap();
     let sam_flag = fiber.record.flags();
     let rq = match fiber.get_rq() {
@@ -129,50 +159,58 @@
         end,
         strand,
         rg: rg.to_string(),
         m6a,
         cpg,
         msp,
         nuc,
+        fiber,
     }
 }
 
 #[pyclass]
 /// Create a fibertools iterator from an indexed bam file.
 /// Must provide a valid chrom, start, and end.
 /// Returns an iterator over :class:`~pyft.Fiberdata` objects.
 pub struct FiberdataFetch {
-    count: usize,
-    fiberdata: Vec<FiberseqData>,
+    fiberdata: IntoIter<FiberseqData>,
+    //_inner: Rc<RefCell<bam::IndexedReader>>,
+    //fiberdata: Box<dyn Iterator<Item = FiberseqData> + Send + 'static>,
+    //fiberdata: Box<dyn Iterator<Item = FiberseqData> + Send + 'static>,
 }
 
 #[pymethods]
 impl FiberdataFetch {
     #[new]
     pub fn new(f: &str, chrom: &str, start: i64, end: i64) -> Self {
         let mut bam = bam::IndexedReader::from_path(f).expect("unable to open indexed bam file");
+        bam.set_threads(8).unwrap();
         let header = bam::Header::from_template(bam.header());
         let head_view = bam::HeaderView::from_header(&header);
         bam.fetch((chrom, start, end))
             .expect("unable to fetch region");
         let records: Vec<bam::Record> = bam.records().map(|r| r.unwrap()).collect();
-        let fiberdata = FiberseqData::from_records(&records, &head_view, 0);
-        Self {
-            count: 0,
-            fiberdata,
-        }
+        log::info!("{} records fetched", records.len());
+        let fiberdata = FiberseqData::from_records(records, &head_view, 0).into_iter();
+        log::info!("fiberdata created from records");
+        /*let fiberdata = bam
+        .records()
+        .map(|rec| FiberseqData::new(&rec.unwrap(), None, 0))
+        .into_iter();*/
+        Self { fiberdata }
     }
 
     fn __next__(&mut self) -> IterNextOutput<Fiberdata, &'static str> {
-        if self.count < self.fiberdata.len() {
-            self.count += 1;
-            // Given an instance `counter`, First five `next(counter)` calls yield 1, 2, 3, 4, 5.
-            IterNextOutput::Yield(new_py_fiberdata(&self.fiberdata[self.count - 1]))
-        } else {
-            IterNextOutput::Return("Ended")
+        let data = self.fiberdata.next();
+        match data {
+            Some(fiber) => IterNextOutput::Yield(new_py_fiberdata(fiber)),
+            None => {
+                log::info!("\n\nDone iterating over fibers");
+                IterNextOutput::Return("Ended")
+            }
         }
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
 }
```

### Comparing `pyft-0.1.2/Cargo.lock` & `pyft-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bamlift"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
- "env_logger",
+ "env_logger 0.9.3",
  "log",
  "rust-htslib",
 ]
 
 [[package]]
 name = "bio"
 version = "1.3.1"
@@ -154,15 +154,15 @@
  "thiserror",
  "triple_accel",
  "vec_map",
 ]
 
 [[package]]
 name = "bio-io"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "colored",
  "gzp",
  "itertools",
  "lazy_static",
  "log",
@@ -557,14 +557,27 @@
  "humantime",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "env_logger"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
+dependencies = [
+ "humantime",
+ "is-terminal",
+ "log",
+ "regex",
+ "termcolor",
+]
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -594,27 +607,27 @@
 name = "feature-probe"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "835a3dc7d1ec9e75e2b5fb4ba75396837112d2060b03f7d43bc1897c7f7211da"
 
 [[package]]
 name = "fibertools-rs"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "anstyle",
  "anyhow",
  "bamlift",
  "bio",
  "bio-io",
  "clap",
  "clap_complete",
  "clap_mangen",
  "colored",
  "console",
- "env_logger",
+ "env_logger 0.9.3",
  "gbdt",
  "indicatif",
  "itertools",
  "lazy_static",
  "log",
  "ordered-float",
  "rayon",
@@ -1346,20 +1359,21 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyft"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "bamlift",
  "bio-io",
  "colored",
+ "env_logger 0.10.0",
  "fibertools-rs",
  "itertools",
  "lazy_static",
  "log",
  "pyo3",
  "regex",
  "rust-htslib",
@@ -1665,17 +1679,17 @@
 name = "roff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b833d8d034ea094b1ea68aa6d5c740e0d04bad9d16568d08ba6f76823a114316"
 
 [[package]]
 name = "rust-htslib"
-version = "0.43.1"
+version = "0.44.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53881800f22b91fa893cc3f6d70e6e9aa96d200133bfe112e36aee37aad70bf5"
+checksum = "7c7eb0f29fce64a4e22578905efef3d72389058016023279a58b282eb5c0c467"
 dependencies = [
  "bio-types",
  "byteorder",
  "custom_derive",
  "derive-new",
  "hts-sys",
  "ieee754",
```

### Comparing `pyft-0.1.2/PKG-INFO` & `pyft-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyft
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # pyft: python bindings for fibertools-rs
```

