# Comparing `tmp/hf-deepali-0.4.0.tar.gz` & `tmp/hf-deepali-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf-deepali-0.4.0.tar", last modified: Thu Jul 20 21:47:07 2023, max compression
+gzip compressed data, was "hf-deepali-0.4.1.tar", last modified: Thu Jul 20 22:36:42 2023, max compression
```

## Comparing `hf-deepali-0.4.0.tar` & `hf-deepali-0.4.1.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.994537 hf-deepali-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.devenv.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.linux-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.osx-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.win-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.win-64.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/basics/example-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/basics/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.994537 hf-deepali-0.4.0/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/domain.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/flow.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/kernels.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/data/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/sampler.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/transforms.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/losses/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/modules/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/networks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/composite.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/transformer.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/utils/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/example-myst-notebook.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/example-notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/pairwise-registration-intro.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/ffd/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/istn/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/istn/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/itn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/src/deepali/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.014537 hf-deepali-0.4.0/src/deepali/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/_kornia.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    78487 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/nnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.014537 hf-deepali-0.4.0/src/deepali/data/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    66499 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/acti.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/nonrigid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/average_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/multilabel_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/output_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/score_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/imageio/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/sitk.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ipython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/simpleitk/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/polydataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/simpleitk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/src/hf_deepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/_test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_data_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_data_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_utils_imageio_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.300182 hf-deepali-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.300182 hf-deepali-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.linux-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.osx-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/conda/environment.win-64.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docker/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.304183 hf-deepali-0.4.1/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/basics/example-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/basics/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/core/kernels.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/sampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/data/transforms.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/losses/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/modules/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/networks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/composite.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/spatial/transformer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/reference/utils/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/example-myst-notebook.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/example-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/docs/tutorials/pairwise-registration-intro.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.308183 hf-deepali-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/ffd/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/ffd/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/istn/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.312183 hf-deepali-0.4.1/examples/istn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/itn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/models/stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/examples/istn/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:36:42.336184 hf-deepali-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.296182 hf-deepali-0.4.1/src/deepali/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.316183 hf-deepali-0.4.1/src/deepali/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/_kornia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78487 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/nnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/core/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/data/transforms/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66499 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/losses/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.320183 hf-deepali-0.4.1/src/deepali/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/modules/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/blocks/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/acti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.324183 hf-deepali-0.4.1/src/deepali/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/nonrigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/spatial/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/aws/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/average_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/multilabel_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/output_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ignite/score_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.328184 hf-deepali-0.4.1/src/deepali/utils/imageio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/imageio/sitk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/deepali/utils/simpleitk/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/simpleitk/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/deepali/utils/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/polydataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/src/deepali/utils/vtk/simpleitk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/src/hf_deepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 22:36:42.000000 hf-deepali-0.4.1/src/hf_deepali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:42.332184 hf-deepali-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/_test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_core_tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_data_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_network_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-20 22:36:23.000000 hf-deepali-0.4.1/tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.4.0/.github/workflows/docs.yml` & `hf-deepali-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.github/workflows/release.yml` & `hf-deepali-0.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.github/workflows/tests.yml` & `hf-deepali-0.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.gitignore` & `hf-deepali-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.vscode/extensions.json` & `hf-deepali-0.4.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.vscode/launch.json` & `hf-deepali-0.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/.vscode/settings.json` & `hf-deepali-0.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/CITATION.cff` & `hf-deepali-0.4.1/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     family-names: Schuh
     affiliation: HeartFlow U.K. Ltd.
     orcid: https://orcid.org/0000-0002-8214-116X
   - given-names: Huaqi
     family-names: Qiu
     affiliation: Imperial College London
   - name: HeartFlow Research
+doi: 10.5281/zenodo.8170161
 url: https://biomedia.github.io/deepali/
 repository-code: https://github.com/BioMedIA/deepali
 keywords:
   - medical-imaging
   - image-registration
   - spatial-transformer-networks
 license: Apache-2.0
```

### Comparing `hf-deepali-0.4.0/CODE_OF_CONDUCT.md` & `hf-deepali-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/LICENSE` & `hf-deepali-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/PKG-INFO` & `hf-deepali-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.0
+Version: 0.4.1
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -29,14 +29,15 @@
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
 ![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
+[![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
 *[Deepali](https://en.wikipedia.org/wiki/Deepali)* is a Hindu/Sanskrit Indian given name, which means "joy" as in the gratification one may feel working with code built on a modern tensor library with support for automatic differentiation, and "chain of lamps" alluding to the application of the chain rule by *torch.autograd*, the concatenation of spatial coordinate transformations, and furthermore the (sequential) composition of PyTorch modules. In addition, the English words "deep" and "ali(-gnment)" partially contained in this name should highlight that this project is not only suitable for traditional non-learning based registration, but in particular facilitates deep learning based approaches to image alignment.
 
 [HeartFlow-Imperial College London]: https://www.heartflow.com/newsroom/heartflow-announces-collaborative-research-agreement-with-imperial-college-london/
 [Biomedical Image Analysis Group]: https://biomedia.doc.ic.ac.uk/
@@ -68,14 +69,15 @@
 
 ## Dependencies
 
 The following lists the main dependencies of this project. For a complete list, please open file [setup.py](setup.py).
 
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
+- [nibabel] (optional): Used by [deepali.data] to read and write images in NIfTI file formats if available.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
 This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
@@ -106,19 +108,24 @@
 
 
 [conda]: https://docs.conda.io/en/latest/
 [pip]: https://pip.pypa.io/en/stable/
 [PyPI]: https://pypi.org/
 [Miniconda]: https://docs.conda.io/en/latest/miniconda.html
 
+## Citation
+
+Schuh, A., Qiu, H., and HeartFlow Research. *deepali: Image, point set, and surface registration in PyTorch* (2023). [doi:10.5281/zenodo.8170161](https://doi.org/10.5281/zenodo.8170161)
 
 ## Contributing
 
 We appreciate all contributions. If you are planning to contribute bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions or extensions, we would appreciate if you first open an issue and discuss the feature with us. Please also read the [CONTRIBUTING](https://github.com/BioMedIA/deepali/tree/main/CONTRIBUTING.md) notes. The participation in this open source project is subject to the [Code of Conduct](https://github.com/BioMedIA/deepali/tree/main/CODE_OF_CONDUCT.md).
 
+By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
+
 Contributors to this project may want to install this package in development mode using
 
 ```
 git clone https://github.com/BioMedIA/deepali.git
 make -C deepali/conda env EDITABLE=1
 conda activate deepali
 ```
@@ -139,14 +146,15 @@
 
 
 [AIRLab]: https://github.com/airlab-unibas/airlab
 [DeepReg]: https://github.com/DeepRegNet/DeepReg
 [Mermaid]: https://github.com/uncbiag/mermaid
 [MONAI]: https://github.com/Project-MONAI/MONAI
 [Neurite]: https://github.com/adalca/neurite
+[nibabel]: https://nipy.org/nibabel/
 [NITorch]: https://github.com/balbasty/nitorch
 [NumPy]: https://numpy.org/
 [PyTorch]: https://pytorch.org/
 [PyTorch Ecosystem]: https://pytorch.org/ecosystem/
 [SimpleITK]: https://simpleitk.org/
 [TensorFlow]: https://www.tensorflow.org/
 [TorchIO]: https://torchio.readthedocs.io/
```

### Comparing `hf-deepali-0.4.0/README.md` & `hf-deepali-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
 ![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
+[![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
 *[Deepali](https://en.wikipedia.org/wiki/Deepali)* is a Hindu/Sanskrit Indian given name, which means "joy" as in the gratification one may feel working with code built on a modern tensor library with support for automatic differentiation, and "chain of lamps" alluding to the application of the chain rule by *torch.autograd*, the concatenation of spatial coordinate transformations, and furthermore the (sequential) composition of PyTorch modules. In addition, the English words "deep" and "ali(-gnment)" partially contained in this name should highlight that this project is not only suitable for traditional non-learning based registration, but in particular facilitates deep learning based approaches to image alignment.
 
 [HeartFlow-Imperial College London]: https://www.heartflow.com/newsroom/heartflow-announces-collaborative-research-agreement-with-imperial-college-london/
 [Biomedical Image Analysis Group]: https://biomedia.doc.ic.ac.uk/
@@ -41,14 +42,15 @@
 
 ## Dependencies
 
 The following lists the main dependencies of this project. For a complete list, please open file [setup.py](setup.py).
 
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
+- [nibabel] (optional): Used by [deepali.data] to read and write images in NIfTI file formats if available.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
 This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
@@ -79,19 +81,24 @@
 
 
 [conda]: https://docs.conda.io/en/latest/
 [pip]: https://pip.pypa.io/en/stable/
 [PyPI]: https://pypi.org/
 [Miniconda]: https://docs.conda.io/en/latest/miniconda.html
 
+## Citation
+
+Schuh, A., Qiu, H., and HeartFlow Research. *deepali: Image, point set, and surface registration in PyTorch* (2023). [doi:10.5281/zenodo.8170161](https://doi.org/10.5281/zenodo.8170161)
 
 ## Contributing
 
 We appreciate all contributions. If you are planning to contribute bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions or extensions, we would appreciate if you first open an issue and discuss the feature with us. Please also read the [CONTRIBUTING](https://github.com/BioMedIA/deepali/tree/main/CONTRIBUTING.md) notes. The participation in this open source project is subject to the [Code of Conduct](https://github.com/BioMedIA/deepali/tree/main/CODE_OF_CONDUCT.md).
 
+By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
+
 Contributors to this project may want to install this package in development mode using
 
 ```
 git clone https://github.com/BioMedIA/deepali.git
 make -C deepali/conda env EDITABLE=1
 conda activate deepali
 ```
@@ -112,14 +119,15 @@
 
 
 [AIRLab]: https://github.com/airlab-unibas/airlab
 [DeepReg]: https://github.com/DeepRegNet/DeepReg
 [Mermaid]: https://github.com/uncbiag/mermaid
 [MONAI]: https://github.com/Project-MONAI/MONAI
 [Neurite]: https://github.com/adalca/neurite
+[nibabel]: https://nipy.org/nibabel/
 [NITorch]: https://github.com/balbasty/nitorch
 [NumPy]: https://numpy.org/
 [PyTorch]: https://pytorch.org/
 [PyTorch Ecosystem]: https://pytorch.org/ecosystem/
 [SimpleITK]: https://simpleitk.org/
 [TensorFlow]: https://www.tensorflow.org/
 [TorchIO]: https://torchio.readthedocs.io/
```

### Comparing `hf-deepali-0.4.0/TODO` & `hf-deepali-0.4.1/TODO`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/Makefile` & `hf-deepali-0.4.1/conda/Makefile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/README.md` & `hf-deepali-0.4.1/conda/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.conda-lock.yml` & `hf-deepali-0.4.1/conda/environment.conda-lock.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.devenv.yml` & `hf-deepali-0.4.1/conda/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.linux-64.lock` & `hf-deepali-0.4.1/conda/environment.linux-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.linux-64.yml` & `hf-deepali-0.4.1/conda/environment.linux-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.osx-64.lock` & `hf-deepali-0.4.1/conda/environment.osx-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.osx-64.yml` & `hf-deepali-0.4.1/conda/environment.osx-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.win-64.lock` & `hf-deepali-0.4.1/conda/environment.win-64.lock`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/conda/environment.win-64.yml` & `hf-deepali-0.4.1/conda/environment.win-64.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docker/Dockerfile` & `hf-deepali-0.4.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docker/build` & `hf-deepali-0.4.1/docker/build`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docker/run` & `hf-deepali-0.4.1/docker/run`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/_citations.bib` & `hf-deepali-0.4.1/docs/_citations.bib`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/_config.yml` & `hf-deepali-0.4.1/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/_images/logo.png` & `hf-deepali-0.4.1/docs/_images/logo.png`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/_toc.yml` & `hf-deepali-0.4.1/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/basics/example-page.md` & `hf-deepali-0.4.1/docs/basics/example-page.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/basics/installation.md` & `hf-deepali-0.4.1/docs/basics/installation.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/index.md` & `hf-deepali-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/core/flow.md` & `hf-deepali-0.4.1/docs/reference/core/flow.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/core/image.md` & `hf-deepali-0.4.1/docs/reference/core/image.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/data/transforms.md` & `hf-deepali-0.4.1/docs/reference/data/transforms.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/spatial/common.md` & `hf-deepali-0.4.1/docs/reference/spatial/common.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/spatial/composite.md` & `hf-deepali-0.4.1/docs/reference/spatial/composite.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/reference/utils/index.md` & `hf-deepali-0.4.1/docs/reference/utils/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/tutorials/example-myst-notebook.md` & `hf-deepali-0.4.1/docs/tutorials/example-myst-notebook.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/tutorials/example-notebook.ipynb` & `hf-deepali-0.4.1/docs/tutorials/example-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/docs/tutorials/pairwise-registration-intro.ipynb` & `hf-deepali-0.4.1/docs/tutorials/pairwise-registration-intro.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/README.md` & `hf-deepali-0.4.1/examples/ffd/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/engine.py` & `hf-deepali-0.4.1/examples/ffd/engine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/hooks.py` & `hf-deepali-0.4.1/examples/ffd/hooks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/losses.py` & `hf-deepali-0.4.1/examples/ffd/losses.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/optim.py` & `hf-deepali-0.4.1/examples/ffd/optim.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/pairwise.py` & `hf-deepali-0.4.1/examples/ffd/pairwise.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/params.yaml` & `hf-deepali-0.4.1/examples/ffd/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/ffd/register.py` & `hf-deepali-0.4.1/examples/ffd/register.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/istn/models/__init__.py` & `hf-deepali-0.4.1/examples/istn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/istn/models/itn.py` & `hf-deepali-0.4.1/examples/istn/models/itn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/istn/models/stn.py` & `hf-deepali-0.4.1/examples/istn/models/stn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/istn/params.yaml` & `hf-deepali-0.4.1/examples/istn/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/examples/istn/train.py` & `hf-deepali-0.4.1/examples/istn/train.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/pyproject.toml` & `hf-deepali-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/__init__.py` & `hf-deepali-0.4.1/src/deepali/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/_kornia.py` & `hf-deepali-0.4.1/src/deepali/core/_kornia.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/affine.py` & `hf-deepali-0.4.1/src/deepali/core/affine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/argparse.py` & `hf-deepali-0.4.1/src/deepali/core/argparse.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/bspline.py` & `hf-deepali-0.4.1/src/deepali/core/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/collections.py` & `hf-deepali-0.4.1/src/deepali/core/collections.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/config.py` & `hf-deepali-0.4.1/src/deepali/core/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/cube.py` & `hf-deepali-0.4.1/src/deepali/core/cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/enum.py` & `hf-deepali-0.4.1/src/deepali/core/enum.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/environ.py` & `hf-deepali-0.4.1/src/deepali/core/environ.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/flow.py` & `hf-deepali-0.4.1/src/deepali/core/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/functional.py` & `hf-deepali-0.4.1/src/deepali/core/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/grid.py` & `hf-deepali-0.4.1/src/deepali/core/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/image.py` & `hf-deepali-0.4.1/src/deepali/core/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/itertools.py` & `hf-deepali-0.4.1/src/deepali/core/itertools.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/kernels.py` & `hf-deepali-0.4.1/src/deepali/core/kernels.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/linalg.py` & `hf-deepali-0.4.1/src/deepali/core/linalg.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/logging.py` & `hf-deepali-0.4.1/src/deepali/core/logging.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/math.py` & `hf-deepali-0.4.1/src/deepali/core/math.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/nnutils.py` & `hf-deepali-0.4.1/src/deepali/core/nnutils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/pathlib.py` & `hf-deepali-0.4.1/src/deepali/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/pointset.py` & `hf-deepali-0.4.1/src/deepali/core/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/psutil.py` & `hf-deepali-0.4.1/src/deepali/core/psutil.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/random.py` & `hf-deepali-0.4.1/src/deepali/core/random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/tempfile.py` & `hf-deepali-0.4.1/src/deepali/core/tempfile.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/tensor.py` & `hf-deepali-0.4.1/src/deepali/core/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/core/typing.py` & `hf-deepali-0.4.1/src/deepali/core/typing.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/__init__.py` & `hf-deepali-0.4.1/src/deepali/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/collate.py` & `hf-deepali-0.4.1/src/deepali/data/collate.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/dataset.py` & `hf-deepali-0.4.1/src/deepali/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/flow.py` & `hf-deepali-0.4.1/src/deepali/data/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/image.py` & `hf-deepali-0.4.1/src/deepali/data/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/partition.py` & `hf-deepali-0.4.1/src/deepali/data/partition.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/prepare.py` & `hf-deepali-0.4.1/src/deepali/data/prepare.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/sample.py` & `hf-deepali-0.4.1/src/deepali/data/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/sampler.py` & `hf-deepali-0.4.1/src/deepali/data/sampler.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/tensor.py` & `hf-deepali-0.4.1/src/deepali/data/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/transforms/__init__.py` & `hf-deepali-0.4.1/src/deepali/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/transforms/image.py` & `hf-deepali-0.4.1/src/deepali/data/transforms/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/data/transforms/item.py` & `hf-deepali-0.4.1/src/deepali/data/transforms/item.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/__init__.py` & `hf-deepali-0.4.1/src/deepali/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/base.py` & `hf-deepali-0.4.1/src/deepali/losses/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/flow.py` & `hf-deepali-0.4.1/src/deepali/losses/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/functional.py` & `hf-deepali-0.4.1/src/deepali/losses/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/image.py` & `hf-deepali-0.4.1/src/deepali/losses/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/params.py` & `hf-deepali-0.4.1/src/deepali/losses/params.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/losses/pointset.py` & `hf-deepali-0.4.1/src/deepali/losses/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/__init__.py` & `hf-deepali-0.4.1/src/deepali/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/basic.py` & `hf-deepali-0.4.1/src/deepali/modules/basic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/flow.py` & `hf-deepali-0.4.1/src/deepali/modules/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/image.py` & `hf-deepali-0.4.1/src/deepali/modules/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/lambd.py` & `hf-deepali-0.4.1/src/deepali/modules/lambd.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/mixins.py` & `hf-deepali-0.4.1/src/deepali/modules/mixins.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/output.py` & `hf-deepali-0.4.1/src/deepali/modules/output.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/sample.py` & `hf-deepali-0.4.1/src/deepali/modules/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/modules/utilities.py` & `hf-deepali-0.4.1/src/deepali/modules/utilities.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/__init__.py` & `hf-deepali-0.4.1/src/deepali/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/blocks/residual.py` & `hf-deepali-0.4.1/src/deepali/networks/blocks/residual.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/blocks/skip.py` & `hf-deepali-0.4.1/src/deepali/networks/blocks/skip.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/__init__.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/acti.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/acti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/conv.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/conv.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/join.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/join.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/linear.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/norm.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/norm.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/pool.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/pool.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/layers/upsample.py` & `hf-deepali-0.4.1/src/deepali/networks/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/resnet.py` & `hf-deepali-0.4.1/src/deepali/networks/resnet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/unet.py` & `hf-deepali-0.4.1/src/deepali/networks/unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/networks/utils.py` & `hf-deepali-0.4.1/src/deepali/networks/utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/__init__.py` & `hf-deepali-0.4.1/src/deepali/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/base.py` & `hf-deepali-0.4.1/src/deepali/spatial/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/bspline.py` & `hf-deepali-0.4.1/src/deepali/spatial/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/composite.py` & `hf-deepali-0.4.1/src/deepali/spatial/composite.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/generic.py` & `hf-deepali-0.4.1/src/deepali/spatial/generic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/linear.py` & `hf-deepali-0.4.1/src/deepali/spatial/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/nonrigid.py` & `hf-deepali-0.4.1/src/deepali/spatial/nonrigid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/parametric.py` & `hf-deepali-0.4.1/src/deepali/spatial/parametric.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/spatial/transformer.py` & `hf-deepali-0.4.1/src/deepali/spatial/transformer.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/aws/s3/client.py` & `hf-deepali-0.4.1/src/deepali/utils/aws/s3/client.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/aws/s3/config.py` & `hf-deepali-0.4.1/src/deepali/utils/aws/s3/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/aws/s3/object.py` & `hf-deepali-0.4.1/src/deepali/utils/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/handlers.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/handlers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/average_loss.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/binary_classification.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/binary_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/multilabel_classification.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/metrics/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/output_transforms.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/output_transforms.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/ignite/score_functions.py` & `hf-deepali-0.4.1/src/deepali/utils/ignite/score_functions.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/imageio/__init__.py` & `hf-deepali-0.4.1/src/deepali/utils/imageio/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/imageio/meta.py` & `hf-deepali-0.4.1/src/deepali/utils/imageio/meta.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/imageio/nifti.py` & `hf-deepali-0.4.1/src/deepali/utils/imageio/nifti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/imageio/sitk.py` & `hf-deepali-0.4.1/src/deepali/utils/imageio/sitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/simpleitk/grid.py` & `hf-deepali-0.4.1/src/deepali/utils/simpleitk/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/simpleitk/imageio.py` & `hf-deepali-0.4.1/src/deepali/utils/simpleitk/imageio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/simpleitk/numpy.py` & `hf-deepali-0.4.1/src/deepali/utils/simpleitk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/simpleitk/sample.py` & `hf-deepali-0.4.1/src/deepali/utils/simpleitk/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/simpleitk/torch.py` & `hf-deepali-0.4.1/src/deepali/utils/simpleitk/torch.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/storage.py` & `hf-deepali-0.4.1/src/deepali/utils/storage.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/tensorboard.py` & `hf-deepali-0.4.1/src/deepali/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/vtk/idlist.py` & `hf-deepali-0.4.1/src/deepali/utils/vtk/idlist.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/vtk/image.py` & `hf-deepali-0.4.1/src/deepali/utils/vtk/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/vtk/numpy.py` & `hf-deepali-0.4.1/src/deepali/utils/vtk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/vtk/polydataio.py` & `hf-deepali-0.4.1/src/deepali/utils/vtk/polydataio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/deepali/utils/vtk/simpleitk.py` & `hf-deepali-0.4.1/src/deepali/utils/vtk/simpleitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/src/hf_deepali.egg-info/PKG-INFO` & `hf-deepali-0.4.1/src/hf_deepali.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.4.0
+Version: 0.4.1
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -29,14 +29,15 @@
 
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
 ![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
+[![doi](https://zenodo.org/badge/DOI/10.5281/zenodo.8170161.svg)](https://doi.org/10.5281/zenodo.8170161)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
 *[Deepali](https://en.wikipedia.org/wiki/Deepali)* is a Hindu/Sanskrit Indian given name, which means "joy" as in the gratification one may feel working with code built on a modern tensor library with support for automatic differentiation, and "chain of lamps" alluding to the application of the chain rule by *torch.autograd*, the concatenation of spatial coordinate transformations, and furthermore the (sequential) composition of PyTorch modules. In addition, the English words "deep" and "ali(-gnment)" partially contained in this name should highlight that this project is not only suitable for traditional non-learning based registration, but in particular facilitates deep learning based approaches to image alignment.
 
 [HeartFlow-Imperial College London]: https://www.heartflow.com/newsroom/heartflow-announces-collaborative-research-agreement-with-imperial-college-london/
 [Biomedical Image Analysis Group]: https://biomedia.doc.ic.ac.uk/
@@ -68,14 +69,15 @@
 
 ## Dependencies
 
 The following lists the main dependencies of this project. For a complete list, please open file [setup.py](setup.py).
 
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
+- [nibabel] (optional): Used by [deepali.data] to read and write images in NIfTI file formats if available.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
 This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
@@ -106,19 +108,24 @@
 
 
 [conda]: https://docs.conda.io/en/latest/
 [pip]: https://pip.pypa.io/en/stable/
 [PyPI]: https://pypi.org/
 [Miniconda]: https://docs.conda.io/en/latest/miniconda.html
 
+## Citation
+
+Schuh, A., Qiu, H., and HeartFlow Research. *deepali: Image, point set, and surface registration in PyTorch* (2023). [doi:10.5281/zenodo.8170161](https://doi.org/10.5281/zenodo.8170161)
 
 ## Contributing
 
 We appreciate all contributions. If you are planning to contribute bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions or extensions, we would appreciate if you first open an issue and discuss the feature with us. Please also read the [CONTRIBUTING](https://github.com/BioMedIA/deepali/tree/main/CONTRIBUTING.md) notes. The participation in this open source project is subject to the [Code of Conduct](https://github.com/BioMedIA/deepali/tree/main/CODE_OF_CONDUCT.md).
 
+By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
+
 Contributors to this project may want to install this package in development mode using
 
 ```
 git clone https://github.com/BioMedIA/deepali.git
 make -C deepali/conda env EDITABLE=1
 conda activate deepali
 ```
@@ -139,14 +146,15 @@
 
 
 [AIRLab]: https://github.com/airlab-unibas/airlab
 [DeepReg]: https://github.com/DeepRegNet/DeepReg
 [Mermaid]: https://github.com/uncbiag/mermaid
 [MONAI]: https://github.com/Project-MONAI/MONAI
 [Neurite]: https://github.com/adalca/neurite
+[nibabel]: https://nipy.org/nibabel/
 [NITorch]: https://github.com/balbasty/nitorch
 [NumPy]: https://numpy.org/
 [PyTorch]: https://pytorch.org/
 [PyTorch Ecosystem]: https://pytorch.org/ecosystem/
 [SimpleITK]: https://simpleitk.org/
 [TensorFlow]: https://www.tensorflow.org/
 [TorchIO]: https://torchio.readthedocs.io/
```

### Comparing `hf-deepali-0.4.0/src/hf_deepali.egg-info/SOURCES.txt` & `hf-deepali-0.4.1/src/hf_deepali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/_test_core_bspline.py` & `hf-deepali-0.4.1/tests/_test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_bspline.py` & `hf-deepali-0.4.1/tests/test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_cube.py` & `hf-deepali-0.4.1/tests/test_core_cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_grid.py` & `hf-deepali-0.4.1/tests/test_core_grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_image_utils.py` & `hf-deepali-0.4.1/tests/test_core_image_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_random.py` & `hf-deepali-0.4.1/tests/test_core_random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_core_tensor_utils.py` & `hf-deepali-0.4.1/tests/test_core_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_data_flow.py` & `hf-deepali-0.4.1/tests/test_data_flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_data_image.py` & `hf-deepali-0.4.1/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_network_blocks.py` & `hf-deepali-0.4.1/tests/test_network_blocks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_network_layers.py` & `hf-deepali-0.4.1/tests/test_network_layers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_network_unet.py` & `hf-deepali-0.4.1/tests/test_network_unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.4.0/tests/test_utils_imageio_meta.py` & `hf-deepali-0.4.1/tests/test_utils_imageio_meta.py`

 * *Files identical despite different names*

