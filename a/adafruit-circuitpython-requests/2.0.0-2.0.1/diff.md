# Comparing `tmp/adafruit-circuitpython-requests-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-requests-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-2.0.0.tar", last modified: Sat Jul  8 14:20:32 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-requests-2.0.1.tar", last modified: Fri Jul 21 21:38:16 2023, max compression
```

## Comparing `adafruit-circuitpython-requests-2.0.0.tar` & `adafruit-circuitpython-requests-2.0.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)     5677 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cellular.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_youtube.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_github_cpython.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_https_circuitpython.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_https_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_multiple_cookies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2986 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2506 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cellular.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/post_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.935489 adafruit-circuitpython-requests-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.923489 adafruit-circuitpython-requests-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.923489 adafruit-circuitpython-requests-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.927489 adafruit-circuitpython-requests-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.927489 adafruit-circuitpython-requests-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-21 21:38:16.935489 adafruit-circuitpython-requests-2.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.927489 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-21 21:38:16.000000 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-21 21:38:16.000000 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:38:16.000000 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 21:38:16.000000 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 21:38:16.000000 adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.927489 adafruit-circuitpython-requests-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.931489 adafruit-circuitpython-requests-2.0.1/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5677 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.935489 adafruit-circuitpython-requests-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_advanced.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_api_youtube.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_github_cpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_https_circuitpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_https_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_multiple_cookies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2986 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2506 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_cellular.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:38:16.935489 adafruit-circuitpython-requests-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:38:16.935489 adafruit-circuitpython-requests-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/post_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-21 21:38:08.000000 adafruit-circuitpython-requests-2.0.1/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 21:37:58.000000 adafruit-circuitpython-requests-2.0.1/tox.ini
```

### Comparing `adafruit-circuitpython-requests-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-requests-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/.gitignore` & `adafruit-circuitpython-requests-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-requests-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/.pylintrc` & `adafruit-circuitpython-requests-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-requests-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/LICENSE` & `adafruit-circuitpython-requests-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-requests-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-requests-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-requests-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/PKG-INFO` & `adafruit-circuitpython-requests-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 2.0.0
+Version: 2.0.1
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-2.0.0/README.rst` & `adafruit-circuitpython-requests-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 2.0.0
+Version: 2.0.1
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit-circuitpython-requests-2.0.1/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/adafruit_requests.py` & `adafruit-circuitpython-requests-2.0.1/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import sys
 
 import json as json_module
```

### Comparing `adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-requests-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/docs/conf.py` & `adafruit-circuitpython-requests-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/docs/index.rst` & `adafruit-circuitpython-requests-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_adafruit_discord_active_online.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cellular.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cpython.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_ethernet.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_advanced_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_discord.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_youtube.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # SPDX-FileCopyrightText: 2022 DJDevon3 for Adafruit Industries
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.0
-"""DJDevon3 Adafruit Feather ESP32-S2 Discord_API_Example"""
+"""DJDevon3 Adafruit Feather ESP32-S2 YouTube_API_Example"""
 import gc
 import time
 import ssl
 import json
 import wifi
 import socketpool
 import adafruit_requests
 
-# Active Logged in User Account Required, no tokens required
-# WEB SCRAPE authorization key required. Visit URL below.
-# Learn how: https://github.com/lorenz234/Discord-Data-Scraping
-
-# Ensure this is in secrets.py or .env
-# "Discord_Authorization": "Discord Authorization from browser console"
+# Ensure these are uncommented and in secrets.py or .env
+# "YT_username": "Your YouTube Username",
+# "YT_token" : "Your long API developer token",
 
 # Initialize WiFi Pool (There can be only 1 pool & top of script)
 pool = socketpool.SocketPool(wifi.radio)
 
 # Time between API refreshes
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
 sleep_time = 900
@@ -39,19 +36,22 @@
 elif 3600 <= sleep_time < 86400:
     sleep_int = sleep_time / 60 / 60
     sleep_time_conversion = "hours"
 else:
     sleep_int = sleep_time / 60 / 60 / 24
     sleep_time_conversion = "days"
 
-discord_header = {"Authorization": "" + secrets["Discord_Authorization"]}
-ADA_SOURCE = (
-    "https://discord.com/api/v10/guilds/"
-    + "327254708534116352"  # Adafruit Discord ID
-    + "/preview"
+# https://youtube.googleapis.com/youtube/v3/channels?part=statistics&forUsername=[YOUR_USERNAME]&key=[YOUR_API_KEY]
+YT_SOURCE = (
+    "https://youtube.googleapis.com/youtube/v3/channels?"
+    + "part=statistics"
+    + "&forUsername="
+    + secrets["YT_username"]
+    + "&key="
+    + secrets["YT_token"]
 )
 
 # Connect to Wi-Fi
 print("\n===============================")
 print("Connecting to WiFi...")
 requests = adafruit_requests.Session(pool, ssl.create_default_context())
 while not wifi.radio.ipv4_address:
@@ -62,44 +62,54 @@
         print("Retrying in 10 seconds")
     time.sleep(10)
     gc.collect()
 print("Connected!\n")
 
 while True:
     try:
-        print(
-            "\nAttempting to GET DISCORD PREVIEW!"
-        )  # --------------------------------
-        # Print Request to Serial
+        print("Attempting to GET YouTube Stats!")  # ----------------------------------
         debug_request = False  # Set true to see full request
         if debug_request:
-            print("Full API GET URL: ", ADA_SOURCE)
+            print("Full API GET URL: ", YT_SOURCE)
         print("===============================")
         try:
-            ada_res = requests.get(url=ADA_SOURCE, headers=discord_header).json()
+            response = requests.get(YT_SOURCE).json()
         except ConnectionError as e:
             print("Connection Error:", e)
             print("Retrying in 10 seconds")
 
         # Print Full JSON to Serial
-        discord_debug_response = False  # Change to true to see full response
-        if discord_debug_response:
-            ada_discord_dump_object = json.dumps(ada_res)
-            print("JSON Dump: ", ada_discord_dump_object)
-
-        # Print keys to Serial
-        discord_debug_keys = True  # Set to True to print Serial data
-        if discord_debug_keys:
-            ada_discord_all_members = ada_res["approximate_member_count"]
-            print("Members: ", ada_discord_all_members)
-
-            ada_discord_all_members_online = ada_res["approximate_presence_count"]
-            print("Online: ", ada_discord_all_members_online)
-
-        print("Monotonic: ", time.monotonic())
+        debug_response = False  # Set true to see full response
+        if debug_response:
+            dump_object = json.dumps(response)
+            print("JSON Dump: ", dump_object)
+
+        # Print to Serial
+        yt_debug_keys = True  # Set to True to print Serial data
+        if yt_debug_keys:
+            print("Matching Results: ", response["pageInfo"]["totalResults"])
+
+            YT_request_kind = response["items"][0]["kind"]
+            print("Request Kind: ", YT_request_kind)
+
+            YT_response_kind = response["kind"]
+            print("Response Kind: ", YT_response_kind)
+
+            YT_channel_id = response["items"][0]["id"]
+            print("Channel ID: ", YT_channel_id)
+
+            YT_videoCount = response["items"][0]["statistics"]["videoCount"]
+            print("Videos: ", YT_videoCount)
+
+            YT_viewCount = response["items"][0]["statistics"]["viewCount"]
+            print("Views: ", YT_viewCount)
+
+            YT_subsCount = response["items"][0]["statistics"]["subscriberCount"]
+            print("Subscribers: ", YT_subsCount)
+            print("Monotonic: ", time.monotonic())
 
         print("\nFinished!")
         print("Next Update in %s %s" % (int(sleep_int), sleep_time_conversion))
         print("===============================")
         gc.collect()
 
     except (ValueError, RuntimeError) as e:
```

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_github.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_github.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_mastodon.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_private.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private_area.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_public.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_openskynetwork_public.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_steam.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitch.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitter.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_twitter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_api_youtube.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_api_discord.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,108 @@
-# SPDX-FileCopyrightText: 2022 DJDevon3 for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.0
-"""DJDevon3 Adafruit Feather ESP32-S2 YouTube_API_Example"""
-import gc
+# Coded for Circuit Python 8.2
+# DJDevon3 Adafruit Feather ESP32-S3 Discord API Example
+import os
 import time
 import ssl
 import json
 import wifi
 import socketpool
 import adafruit_requests
 
-# Ensure these are uncommented and in secrets.py or .env
-# "YT_username": "Your YouTube Username",
-# "YT_token" : "Your long API developer token",
+# Active Logged in User Account Required, no tokens required
+# WEB SCRAPE authorization key required. Visit URL below.
+# Learn how: https://github.com/lorenz234/Discord-Data-Scraping
+
+# Ensure this is in settings.toml
+# "Discord_Authorization": "Request Header Auth here"
+
+# Uses settings.toml for credentials
+ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+appw = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+Discord_Auth = os.getenv("Discord_Authorization")
 
 # Initialize WiFi Pool (There can be only 1 pool & top of script)
 pool = socketpool.SocketPool(wifi.radio)
 
-# Time between API refreshes
+# API Polling Rate
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
 sleep_time = 900
 
-try:
-    from secrets import secrets
-except ImportError:
-    print("Secrets File Import Error")
-    raise
-
-if sleep_time < 60:
-    sleep_time_conversion = "seconds"
-    sleep_int = sleep_time
-elif 60 <= sleep_time < 3600:
-    sleep_int = sleep_time / 60
-    sleep_time_conversion = "minutes"
-elif 3600 <= sleep_time < 86400:
-    sleep_int = sleep_time / 60 / 60
-    sleep_time_conversion = "hours"
-else:
-    sleep_int = sleep_time / 60 / 60 / 24
-    sleep_time_conversion = "days"
-
-# https://youtube.googleapis.com/youtube/v3/channels?part=statistics&forUsername=[YOUR_USERNAME]&key=[YOUR_API_KEY]
-YT_SOURCE = (
-    "https://youtube.googleapis.com/youtube/v3/channels?"
-    + "part=statistics"
-    + "&forUsername="
-    + secrets["YT_username"]
-    + "&key="
-    + secrets["YT_token"]
+
+# Converts seconds to human readable minutes/hours/days
+def time_calc(input_time):  # input_time in seconds
+    if input_time < 60:
+        sleep_int = input_time
+        time_output = f"{sleep_int:.0f} seconds"
+    elif 60 <= input_time < 3600:
+        sleep_int = input_time / 60
+        time_output = f"{sleep_int:.0f} minutes"
+    elif 3600 <= input_time < 86400:
+        sleep_int = input_time / 60 / 60
+        time_output = f"{sleep_int:.1f} hours"
+    else:
+        sleep_int = input_time / 60 / 60 / 24
+        time_output = f"{sleep_int:.1f} days"
+    return time_output
+
+
+discord_header = {"Authorization": "" + Discord_Auth}
+ADA_SOURCE = (
+    "https://discord.com/api/v10/guilds/"
+    + "327254708534116352"  # Adafruit Discord ID
+    + "/preview"
 )
 
 # Connect to Wi-Fi
 print("\n===============================")
 print("Connecting to WiFi...")
 requests = adafruit_requests.Session(pool, ssl.create_default_context())
 while not wifi.radio.ipv4_address:
     try:
-        wifi.radio.connect(secrets["ssid"], secrets["password"])
+        wifi.radio.connect(ssid, appw)
     except ConnectionError as e:
         print("Connection Error:", e)
         print("Retrying in 10 seconds")
     time.sleep(10)
-    gc.collect()
-print("Connected!\n")
+print("Connected!✅")
 
 while True:
     try:
-        print("Attempting to GET YouTube Stats!")  # ----------------------------------
-        debug_request = False  # Set true to see full request
+        print("\nAttempting to GET Discord Data!")  # --------------------------------
+        # STREAMER WARNING this will show your credentials!
+        debug_request = False  # Set True to see full request
         if debug_request:
-            print("Full API GET URL: ", YT_SOURCE)
+            print("Full API GET URL: ", ADA_SOURCE)
         print("===============================")
         try:
-            response = requests.get(YT_SOURCE).json()
+            ada_res = requests.get(url=ADA_SOURCE, headers=discord_header).json()
         except ConnectionError as e:
             print("Connection Error:", e)
             print("Retrying in 10 seconds")
 
         # Print Full JSON to Serial
-        debug_response = False  # Set true to see full response
-        if debug_response:
-            dump_object = json.dumps(response)
-            print("JSON Dump: ", dump_object)
-
-        # Print to Serial
-        yt_debug_keys = True  # Set to True to print Serial data
-        if yt_debug_keys:
-            print("Matching Results: ", response["pageInfo"]["totalResults"])
-
-            YT_request_kind = response["items"][0]["kind"]
-            print("Request Kind: ", YT_request_kind)
-
-            YT_response_kind = response["kind"]
-            print("Response Kind: ", YT_response_kind)
-
-            YT_channel_id = response["items"][0]["id"]
-            print("Channel ID: ", YT_channel_id)
-
-            YT_videoCount = response["items"][0]["statistics"]["videoCount"]
-            print("Videos: ", YT_videoCount)
-
-            YT_viewCount = response["items"][0]["statistics"]["viewCount"]
-            print("Views: ", YT_viewCount)
-
-            YT_subsCount = response["items"][0]["statistics"]["subscriberCount"]
-            print("Subscribers: ", YT_subsCount)
-            print("Monotonic: ", time.monotonic())
-
-        print("\nFinished!")
-        print("Next Update in %s %s" % (int(sleep_int), sleep_time_conversion))
+        discord_debug_response = False  # Set True to see full response
+        if discord_debug_response:
+            ada_discord_dump_object = json.dumps(ada_res)
+            print("JSON Dump: ", ada_discord_dump_object)
+
+        # Print keys to Serial
+        discord_debug_keys = True  # Set True to print Serial data
+        if discord_debug_keys:
+            ada_discord_all_members = ada_res["approximate_member_count"]
+            print("Members: ", ada_discord_all_members)
+
+            ada_discord_all_members_online = ada_res["approximate_presence_count"]
+            print("Online: ", ada_discord_all_members_online)
+
+        print("Finished ✅")
+        print("Board Uptime: ", time_calc(time.monotonic()))
+        print("Next Update: ", time_calc(sleep_time))
         print("===============================")
-        gc.collect()
 
-    except (ValueError, RuntimeError) as e:
+    except (ConnectionError, ValueError, NameError) as e:
         print("Failed to get data, retrying\n", e)
         time.sleep(60)
         continue
     time.sleep(sleep_time)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_github_cpython.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_github_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_https_circuitpython.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_https_circuitpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_https_cpython.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_https_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_multiple_cookies.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cellular.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cpython.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_ethernet.py` & `adafruit-circuitpython-requests-2.0.1/examples/requests_simpletest_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/pyproject.toml` & `adafruit-circuitpython-requests-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/chunk_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/chunked_redirect_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/concurrent_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/header_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/mocket.py` & `adafruit-circuitpython-requests-2.0.1/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/parse_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/post_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/post_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/protocol_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-2.0.0/tests/reuse_test.py` & `adafruit-circuitpython-requests-2.0.1/tests/reuse_test.py`

 * *Files identical despite different names*

