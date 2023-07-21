# Comparing `tmp/otf-addons-aws-0.4.0.tar.gz` & `tmp/otf-addons-aws-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf-addons-aws-0.4.0.tar", last modified: Wed Mar 29 10:06:11 2023, max compression
+gzip compressed data, was "otf-addons-aws-0.5.1.tar", last modified: Fri Jul 21 13:39:14 2023, max compression
```

## Comparing `otf-addons-aws-0.4.0.tar` & `otf-addons-aws-0.5.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.287054 otf-addons-aws-0.4.0/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       71 2023-01-30 12:58:57.000000 otf-addons-aws-0.4.0/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35148 2023-01-30 12:58:57.000000 otf-addons-aws-0.4.0/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       43 2023-03-27 12:04:07.000000 otf-addons-aws-0.4.0/MANIFEST.in
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5402 2023-03-29 10:06:11.287054 otf-addons-aws-0.4.0/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4562 2023-03-29 10:03:50.000000 otf-addons-aws-0.4.0/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1767 2023-03-29 10:02:13.000000 otf-addons-aws-0.4.0/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-03-29 10:06:11.287054 otf-addons-aws-0.4.0/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      221 2023-01-30 15:19:37.000000 otf-addons-aws-0.4.0/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.191053 otf-addons-aws-0.4.0/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.191053 otf-addons-aws-0.4.0/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.187053 otf-addons-aws-0.4.0/src/opentaskpy/addons/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.207053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-01-30 15:20:12.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.219053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-01-30 15:22:32.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      766 2023-03-02 17:46:17.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/aws.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3848 2023-03-02 17:46:17.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/lambda.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9558 2023-03-02 17:46:17.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/s3.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.187053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.187053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.231053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      463 2023-03-24 16:29:18.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      409 2023-03-24 16:40:57.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.239053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      409 2023-03-24 16:50:27.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      338 2023-03-24 16:51:30.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.243053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.243053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      161 2023-03-24 16:46:15.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      466 2023-03-24 16:43:38.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      363 2023-03-24 16:49:07.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.243053 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      273 2023-03-24 17:02:14.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      400 2023-03-24 16:43:46.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      550 2023-03-24 16:49:24.000000 otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.191053 otf-addons-aws-0.4.0/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.191053 otf-addons-aws-0.4.0/src/opentaskpy/plugins/lookup/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.243053 otf-addons-aws-0.4.0/src/opentaskpy/plugins/lookup/aws/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2261 2023-02-23 13:47:36.000000 otf-addons-aws-0.4.0/src/opentaskpy/plugins/lookup/aws/ssm.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.251053 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5402 2023-03-29 10:06:11.000000 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1577 2023-03-29 10:06:11.000000 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-03-29 10:06:11.000000 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      234 2023-03-29 10:06:11.000000 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2023-03-29 10:06:11.000000 otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-29 10:06:11.279054 otf-addons-aws-0.4.0/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      670 2023-03-24 15:55:29.000000 otf-addons-aws-0.4.0/tests/test_lambda_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2826 2023-03-28 16:52:39.000000 otf-addons-aws-0.4.0/tests/test_plugin_ssm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8960 2023-03-28 17:00:04.000000 otf-addons-aws-0.4.0/tests/test_remotehandler_lambda_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2089 2023-03-28 16:53:22.000000 otf-addons-aws-0.4.0/tests/test_remotehandler_s3_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    25296 2023-03-28 16:54:18.000000 otf-addons-aws-0.4.0/tests/test_remotehandler_s3_transfer.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2242 2023-03-28 15:13:46.000000 otf-addons-aws-0.4.0/tests/test_s3_source_schema_validate.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.816904 otf-addons-aws-0.5.1/
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/AUTHORS
+-rw-r--r--   0 adam       (501) staff       (20)    35149 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)       44 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     5382 2023-07-21 13:39:14.816766 otf-addons-aws-0.5.1/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     4543 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/README.md
+-rw-r--r--   0 adam       (501) staff       (20)    13202 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-21 13:39:14.816941 otf-addons-aws-0.5.1/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810105 otf-addons-aws-0.5.1/src/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809967 otf-addons-aws-0.5.1/src/opentaskpy/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809470 otf-addons-aws-0.5.1/src/opentaskpy/addons/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.811627 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.812593 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)      942 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/creds.py
+-rw-r--r--   0 adam       (501) staff       (20)     4580 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py
+-rw-r--r--   0 adam       (501) staff       (20)    12798 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/s3.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809796 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809735 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.812911 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
+-rw-r--r--   0 adam       (501) staff       (20)      542 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
+-rw-r--r--   0 adam       (501) staff       (20)      506 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.813266 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
+-rw-r--r--   0 adam       (501) staff       (20)      503 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      429 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.813764 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814086 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
+-rw-r--r--   0 adam       (501) staff       (20)      279 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
+-rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      485 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814431 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
+-rw-r--r--   0 adam       (501) staff       (20)      398 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
+-rw-r--r--   0 adam       (501) staff       (20)      500 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      663 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810007 otf-addons-aws-0.5.1/src/opentaskpy/plugins/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810047 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814586 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/
+-rw-r--r--   0 adam       (501) staff       (20)     2819 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/ssm.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.815304 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     5382 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1570 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)      208 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.816578 otf-addons-aws-0.5.1/tests/
+-rw-r--r--   0 adam       (501) staff       (20)      670 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/tests/test_lambda_execution_schema_validate.py
+-rw-r--r--   0 adam       (501) staff       (20)     2853 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_plugin_ssm.py
+-rw-r--r--   0 adam       (501) staff       (20)     9676 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_lambda_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)     2113 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_s3_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)    21869 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_s3_transfer.py
+-rw-r--r--   0 adam       (501) staff       (20)     2272 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/tests/test_s3_source_schema_validate.py
```

### Comparing `otf-addons-aws-0.4.0/LICENSE` & `otf-addons-aws-0.5.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `otf-addons-aws-0.4.0/PKG-INFO` & `otf-addons-aws-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 0.4.0
+Version: 0.5.1
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
-
 ![unittest status](https://github.com/adammcdonagh/otf-addons-aws/actions/workflows/main.yml/badge.svg)
 
 This repository contains addons to allow integration with AWS components via [Open Task Framework (OTF)](https://github.com/adammcdonagh/open-task-framework)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 These addons include several additional features:
-  * A new plugin for SSM Param Store to pull dynamic variables
-  * A new remotehandler to push/pull files via AWS S3
-  * A new remote handler to trigger AWS Lambda functions
+
+- A new plugin for SSM Param Store to pull dynamic variables
+- A new remotehandler to push/pull files via AWS S3
+- A new remote handler to trigger AWS Lambda functions
 
 # AWS Credentials
 
-This package uses boto3 to communicate with AWS. 
+This package uses boto3 to communicate with AWS.
 
 Credentials can be set via config using equivalently named variables alongside the protocol definition e.g;
+
 ```json
 "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
     "access_key_id": "some_key",
     "secret_access_key": "some_secret_key",
     "region_name": "eu-west-1"
 }
@@ -48,22 +49,24 @@
 # Transfers
 
 Transfers are defined the same as a normal SSH based transfer.
 
 As part of the upload, the `bucket-owner-full-control` ACL flag is applied to all files. This can be disabled by setting `disableBucketOwnerControlACL` to `true` in the `protocol` definition
 
 ### Supported features
-   * Plain file watch
-   * File watch/transfer with file size and age constraints
-   * `move` & `delete` post copy actions
-   * Touching empty files after transfer. e.g. `.fin` files used as completion flags
-   * Touching empty files as an execution
+
+- Plain file watch
+- File watch/transfer with file size and age constraints
+- `move` & `delete` post copy actions
+- Touching empty files after transfer. e.g. `.fin` files used as completion flags
+- Touching empty files as an execution
 
 ### Limitations
-   * No support for log watch
+
+- No support for log watch
 
 # Configuration
 
 JSON configs for transfers can be defined as follows:
 
 ## Example File Watch Only
 
@@ -91,27 +94,29 @@
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example S3 Upload
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "protocol": {
           "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
         }
     }
 ]
 ```
 
 ## Example S3 upload with flag files
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "flag": {
           "fullPath": "dest/some_fin.flg"
@@ -125,34 +130,35 @@
 
 # Executions
 
 The Lambda remote handler allows AWS Lambda functions to be called. When provided with a `functionArn` the function will be called with no parameters. If there's a payload to pass in, use the `payload` attribute in the execution definition to specify a JSON object to pass into the function.
 
 ## Asynchronous vs Synchronous Execution
 
-Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`. 
+Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`.
 
 `Event` is asynchronous, and tells the Lambda function to trigger, but does not check that it ran successfully. This means it's up to you to make sure that you have appropriate monitoring of your Lambda functions.
 
 `RequestResponse` will block until the Lambda function either completes, or times out. Boto3 has a timeout of 60 seconds, so this cannot be used for long running functions (over 1 minute). This also causes issues when used in conjunction with batches and timeouts. Since the request blocks, the thread cannot be killed by the batch thread, meaning that it will block any further execution until 60 seconds after triggering the lambda function.
 
-
 ## Example S3 Execution touch flag file
+
 ```json
 {
   "type": "execution",
   "bucket": "test-bucket",
   "key": "test_key.flg",
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example Lambda function call
+
 ```json
 {
   "type": "execution",
   "functionArn": "arn:aws:lambda:eu-west-1:000000000000:function:my-function",
   "invocationType": "Event",
   "payload": {
     "file-name": "some_file.txt"
```

### Comparing `otf-addons-aws-0.4.0/README.md` & `otf-addons-aws-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-
 ![unittest status](https://github.com/adammcdonagh/otf-addons-aws/actions/workflows/main.yml/badge.svg)
 
 This repository contains addons to allow integration with AWS components via [Open Task Framework (OTF)](https://github.com/adammcdonagh/open-task-framework)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 These addons include several additional features:
-  * A new plugin for SSM Param Store to pull dynamic variables
-  * A new remotehandler to push/pull files via AWS S3
-  * A new remote handler to trigger AWS Lambda functions
+
+- A new plugin for SSM Param Store to pull dynamic variables
+- A new remotehandler to push/pull files via AWS S3
+- A new remote handler to trigger AWS Lambda functions
 
 # AWS Credentials
 
-This package uses boto3 to communicate with AWS. 
+This package uses boto3 to communicate with AWS.
 
 Credentials can be set via config using equivalently named variables alongside the protocol definition e.g;
+
 ```json
 "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
     "access_key_id": "some_key",
     "secret_access_key": "some_secret_key",
     "region_name": "eu-west-1"
 }
@@ -29,22 +30,24 @@
 # Transfers
 
 Transfers are defined the same as a normal SSH based transfer.
 
 As part of the upload, the `bucket-owner-full-control` ACL flag is applied to all files. This can be disabled by setting `disableBucketOwnerControlACL` to `true` in the `protocol` definition
 
 ### Supported features
-   * Plain file watch
-   * File watch/transfer with file size and age constraints
-   * `move` & `delete` post copy actions
-   * Touching empty files after transfer. e.g. `.fin` files used as completion flags
-   * Touching empty files as an execution
+
+- Plain file watch
+- File watch/transfer with file size and age constraints
+- `move` & `delete` post copy actions
+- Touching empty files after transfer. e.g. `.fin` files used as completion flags
+- Touching empty files as an execution
 
 ### Limitations
-   * No support for log watch
+
+- No support for log watch
 
 # Configuration
 
 JSON configs for transfers can be defined as follows:
 
 ## Example File Watch Only
 
@@ -72,27 +75,29 @@
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example S3 Upload
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "protocol": {
           "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
         }
     }
 ]
 ```
 
 ## Example S3 upload with flag files
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "flag": {
           "fullPath": "dest/some_fin.flg"
@@ -106,40 +111,41 @@
 
 # Executions
 
 The Lambda remote handler allows AWS Lambda functions to be called. When provided with a `functionArn` the function will be called with no parameters. If there's a payload to pass in, use the `payload` attribute in the execution definition to specify a JSON object to pass into the function.
 
 ## Asynchronous vs Synchronous Execution
 
-Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`. 
+Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`.
 
 `Event` is asynchronous, and tells the Lambda function to trigger, but does not check that it ran successfully. This means it's up to you to make sure that you have appropriate monitoring of your Lambda functions.
 
 `RequestResponse` will block until the Lambda function either completes, or times out. Boto3 has a timeout of 60 seconds, so this cannot be used for long running functions (over 1 minute). This also causes issues when used in conjunction with batches and timeouts. Since the request blocks, the thread cannot be killed by the batch thread, meaning that it will block any further execution until 60 seconds after triggering the lambda function.
 
-
 ## Example S3 Execution touch flag file
+
 ```json
 {
   "type": "execution",
   "bucket": "test-bucket",
   "key": "test_key.flg",
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example Lambda function call
+
 ```json
 {
   "type": "execution",
   "functionArn": "arn:aws:lambda:eu-west-1:000000000000:function:my-function",
   "invocationType": "Event",
   "payload": {
     "file-name": "some_file.txt"
   },
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution"
   }
 }
-```
+```
```

### Comparing `otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/lambda.py` & `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,48 @@
+"""AWS Lambda remote handler."""
 import base64
 import json
 import os
 
 import boto3
 import botocore.exceptions
-import opentaskpy.logging
+import opentaskpy.otflogging
+from opentaskpy.exceptions import InvalidConfigError
 from opentaskpy.remotehandlers.remotehandler import RemoteExecutionHandler
 
-from .aws import set_aws_creds
+from .creds import set_aws_creds
 
 
 class LambdaExecution(RemoteExecutionHandler):
+    """AWS Lambda remote handler."""
+
     TASK_TYPE = "E"
 
-    def tidy(self):
+    def tidy(self) -> None:
+        """Tidy up the lambda client."""
         self.lambda_client.close()
 
-    def __init__(self, spec):
-        self.spec = spec
+    def __init__(self, spec: dict):
+        """Initialise the LambdaExecution handler.
 
+        Args:
+            spec (dict): The spec for the execution.
+        """
         # Ensure that function_arn is defined in the spec
-        if "functionArn" not in self.spec:
-            raise Exception("functionArn not defined in spec")
+        # This is really handled by the schema checks
 
-        self.logger = opentaskpy.logging.init_logging(
+        self.logger = opentaskpy.otflogging.init_logging(
             __name__, os.environ.get("OTF_TASK_ID"), self.TASK_TYPE
         )
 
+        super().__init__(spec)
+
+        if "functionArn" not in self.spec:
+            raise InvalidConfigError("functionArn not defined in spec")
+
         set_aws_creds(self)
 
         # Use boto3 to setup the required object
         kwargs = {
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "region_name": self.region_name,
@@ -42,27 +54,36 @@
         # Set the client to only try once. This prevents the lambda function being called more than once
         # and issues when working with batch timeouts if a lambda function takes longer than the batch timeout
         # It still means that the timeout of a lambda function is always at least 60 seconds due to the way boto3's HTTP timeout works
         kwargs["config"] = botocore.client.Config(retries={"max_attempts": 0})
 
         self.lambda_client = boto3.client("lambda", **kwargs)
 
-    def kill(self):
+    def kill(self) -> None:
+        """Kill the lambda function.
+
+        This doesn't do a huge amount. Lambda functions don't run for a long period of
+        time anyway, so this is more a way to clean up the client nicely.
+        """
         # We need to kill the running execute function
         self.tidy()
-        self.logger.info("Killing thread")
-
-    # Triggers the lambda function. The synchronous invocation type will cause this thread
-    # to block. This can be an issue with batch jobs and their timeout.
-    # Boto3 will timeout after 60 seconds regardless, so Lambda functions that are called should not be long running. Their own timeout should be less than the
-    # batch timeout if one is used.
+        self.logger.info("Closed Lambda client")
 
-    # An async call will not check the status of the lambda function, only if there are errors with invoking it.
+    def execute(self) -> bool:
+        """Execute the lambda function.
 
-    def execute(self):
+        Triggers the lambda function. The synchronous invocation type will cause this
+        thread to block. This can be an issue with batch jobs and their timeout. Boto3
+        will timeout after 60 seconds regardless, so Lambda functions that are called
+        should not be long running. Their own timeout should be less than the batch timeout
+        if one is used.
+
+        An async call will not check the status of the lambda function, only if there
+        are errors with invoking it.
+        """
         result = True
 
         function_arn = self.spec["functionArn"]
         invocation_type = (
             self.spec["invocationType"] if "invocationType" in self.spec else "Event"
         )
         payload = None
@@ -81,22 +102,23 @@
                 and invoke_response["StatusCode"] != 202
             ):
                 self.logger.error(f"Failed to run lambda function: {function_arn}")
                 return False
 
             if "FunctionError" in invoke_response:
                 self.logger.error(
-                    f"Lambda function returned an error: {function_arn} - AWS Exception message: {invoke_response['FunctionError']}"
+                    f"Lambda function returned an error: {function_arn} - AWS Exception"
+                    f" message: {invoke_response['FunctionError']}"
                 )
                 return False
 
             # Log the response if there is one
             if "LogResult" in invoke_response:
                 # base64 decode the result
-                log_result = base64.b64decode(invoke_response["LogResult"])
+                log_result = base64.b64decode(invoke_response["LogResult"]).decode()
 
                 self.logger.debug(f"Lambda function response: {log_result}")
 
         except botocore.exceptions.ClientError as e:
             self.logger.error(f"Failed to run lambda function: {function_arn}")
             self.logger.error(e)
             result = False
```

### Comparing `otf-addons-aws-0.4.0/src/opentaskpy/addons/aws/remotehandlers/s3.py` & `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/s3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,69 @@
+"""AWS S3 remote handler."""
 import glob
 import os
 import re
 
 import boto3
-import opentaskpy.logging
+import opentaskpy.otflogging
 from opentaskpy.remotehandlers.remotehandler import (
     RemoteExecutionHandler,
     RemoteTransferHandler,
 )
 
-from .aws import set_aws_creds
+from .creds import set_aws_creds
 
 MAX_OBJECTS_PER_QUERY = 100
 
 
 class S3Transfer(RemoteTransferHandler):
+    """S3 remote transfer handler."""
+
     TASK_TYPE = "T"
 
-    def __init__(self, spec):
-        self.spec = spec
+    def __init__(self, spec: dict):
+        """Initialise the S3Transfer handler.
 
-        self.logger = opentaskpy.logging.init_logging(
+        Args:
+            spec (dict): The spec for the transfer. This is either the source, or the
+            destination spec.
+        """
+        self.logger = opentaskpy.otflogging.init_logging(
             __name__, os.environ.get("OTF_TASK_ID"), self.TASK_TYPE
         )
 
+        super().__init__(spec)
+
         set_aws_creds(self)
 
         # Use boto3 to setup the required object for the transfer
         kwargs = {
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "region_name": self.region_name,
         }
         # If there's an override for endpoint_url in the environment, then use that
         if os.environ.get("AWS_ENDPOINT_URL"):
             kwargs["endpoint_url"] = os.environ.get("AWS_ENDPOINT_URL")
 
         self.s3_client = boto3.client("s3", **kwargs)
 
-    def handle_post_copy_action(self, files):
+    def supports_direct_transfer(self) -> bool:
+        """Return True, as you can do bucket to bucket transfers."""
+        return True
+
+    def handle_post_copy_action(self, files: list[str]) -> int:
+        """Handle the post copy action specified in the config.
+
+        Args:
+            files (list[str]): A list of files that need to be handled.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         # Determine the action to take
         # Delete the files
         if self.spec["postCopyAction"]["action"] == "delete":
             self.s3_client.delete_objects(
                 Bucket=self.spec["bucket"],
                 Delete={
                     "Objects": [{"Key": file} for file in files],
@@ -51,95 +72,118 @@
             )
         # Copy the files to the new location, and then delete the originals
         if (
             self.spec["postCopyAction"]["action"] == "move"
             or self.spec["postCopyAction"]["action"] == "rename"
         ):
             for file in files:
-                # If this is a rename, then we need to determine the new key
-                new_file = file
+                new_file = (
+                    f"{self.spec['postCopyAction']['destination']}{file.split('/')[-1]}"
+                )
                 if self.spec["postCopyAction"]["action"] == "rename":
-                    new_file = f"{self.spec['postCopyAction']['destination']}{file.split('/')[-1]}"
-
                     # Use the pattern and sub values to rename the file correctly
                     new_file = re.sub(
                         self.spec["postCopyAction"]["pattern"],
                         self.spec["postCopyAction"]["sub"],
                         new_file,
                     )
 
                 self.s3_client.copy_object(
                     Bucket=self.spec["bucket"],
                     CopySource={
                         "Bucket": self.spec["bucket"],
                         "Key": file,
                     },
-                    Key=f"{self.spec['postCopyAction']['destination']}/{new_file}",
+                    Key=new_file,
                 )
                 self.s3_client.delete_objects(
                     Bucket=self.spec["bucket"],
                     Delete={
                         "Objects": [{"Key": file}],
                         "Quiet": True,
                     },
                 )
         return 0
 
-    def list_files(self, directory=None, file_pattern=None):
+    def list_files(
+        self, directory: str | None = None, file_pattern: str | None = None
+    ) -> dict:
+        """Return list of files that match the source definition.
+
+        Args:
+            directory (str, optional): The directory to search in. Defaults to None.
+            file_pattern (str, optional): The file pattern to search for. Defaults to
+            None.
+
+        Returns:
+            dict: A dict of files that match the source definition.
+        """
         kwargs = {
             "Bucket": self.spec["bucket"],
             "MaxKeys": MAX_OBJECTS_PER_QUERY,
         }
         if directory:
             kwargs["Prefix"] = directory
+        elif str(self.spec["directory"]):
+            kwargs["Prefix"] = str(self.spec["directory"])
 
-        remote_files = dict()
+        remote_files = {}
 
         while True:
             response = self.s3_client.list_objects_v2(**kwargs)
 
             if response["KeyCount"]:
-                for object in response["Contents"]:
-                    key = object["Key"]
+                for object_ in response["Contents"]:
+                    key = object_["Key"]
                     # Get the filename from the key
                     filename = key.split("/")[-1]  #
                     self.logger.debug(f"Found file: {filename}")
                     if file_pattern and not re.match(file_pattern, filename):
                         continue
-                    else:
-                        # Get the size and modified time
-                        file_attr = self.s3_client.head_object(
-                            Bucket=self.spec["bucket"], Key=key
-                        )
-
-                        remote_files[key] = {
-                            "size": file_attr["ContentLength"],
-                            "modified_time": file_attr["LastModified"].timestamp(),
-                        }
+
+                    # Get the size and modified time
+                    file_attr = self.s3_client.head_object(
+                        Bucket=self.spec["bucket"], Key=key
+                    )
+
+                    remote_files[key] = {
+                        "size": file_attr["ContentLength"],
+                        "modified_time": file_attr["LastModified"].timestamp(),
+                    }
 
                 # This handles the pagination
-                # if the NextContinuationToken doesnt exist, then we'll break out
+                # if the NextContinuationToken doesn't exist, then we'll break out
                 # of the loop
                 try:
                     kwargs["ContinuationToken"] = response["NextContinuationToken"]
                 except KeyError:
                     break
-            else:
-                return None
+            break
 
         return remote_files
 
-    def move_files_to_final_location(self, files):
-        raise NotImplementedError()
+    def move_files_to_final_location(self, files: list[str]) -> None:
+        """Not implemented for this handler."""
+        raise NotImplementedError
 
     # When S3 is the destination
-    def pull_files(self, files, remote_spec):
-        raise NotImplementedError()
-
-    def push_files_from_worker(self, local_staging_directory):
+    def pull_files(self, files: list[str]) -> None:
+        """Not implemented for this handler."""
+        raise NotImplementedError
+
+    def push_files_from_worker(self, local_staging_directory: str) -> int:
+        """Push files from the worker to the destination server.
+
+        Args:
+            local_staging_directory (str): The local staging directory to upload the
+            files from.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         result = 0
         files = glob.glob(f"{local_staging_directory}/*")
         kwargs = {}
         if self.bucket_owner_full_control:
             kwargs["ACL"] = "bucket-owner-full-control"
 
         for file in files:
@@ -151,41 +195,72 @@
             try:
                 self.s3_client.upload_file(
                     file,
                     self.spec["bucket"],
                     f"{self.spec['directory']}/{file_name}",
                     ExtraArgs=kwargs,
                 )
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-exception-caught
                 self.logger.error(f"Failed to transfer file: {file}")
                 self.logger.error(e)
                 result = 1
 
         return result
 
-    def pull_files_to_worker(self, files, local_staging_directory):
+    def pull_files_to_worker(
+        self, files: list[str], local_staging_directory: str
+    ) -> int:
+        """Pull files to the worker.
+
+        Download files from AWS S3 to the local staging directory.
+
+        Args:
+            files (list): A list of files to download.
+            local_staging_directory (str): The local staging directory to download the
+            files to.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         result = 0
         for file in files:
             # Strip the directory from the file
             file_name = file.split("/")[-1]
             self.logger.debug(f"Transferring file: {file}")
             try:
                 self.s3_client.download_file(
                     self.spec["bucket"],
                     file,
                     f"{local_staging_directory}/{file_name}",
                 )
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-exception-caught
                 self.logger.error(f"Failed to transfer file: {file}")
                 self.logger.error(e)
                 result = 1
 
         return result
 
-    def transfer_files(self, files, remote_spec, dest_remote_handler=None):
+    def transfer_files(
+        self,
+        files: list[str],
+        remote_spec: dict,
+        dest_remote_handler: RemoteTransferHandler,
+    ) -> int:
+        """Transfer files from the source S3 bucket to the destination bucket.
+
+        Args:
+            files (dict): A dictionary of files to transfer.
+            remote_spec (dict): Not used by this handler.
+            dest_remote_handler (RemoteTransferHandler): The remote handler
+            for the destination bucket
+
+        Returns:
+            int: 0 if successful, if not, then 1
+            command.
+        """
         # Check the remote handler, if it's another S3Transfer, then it's simple
         # to do an S3 copy via boto
 
         result = 0
         for file in files:
             # Strip the directory from the file
             file_name = file.split("/")[-1]
@@ -195,78 +270,101 @@
                     {
                         "Bucket": self.spec["bucket"],
                         "Key": file,
                     },
                     dest_remote_handler.spec["bucket"],
                     f"{dest_remote_handler.spec['directory']}/{file_name}",
                 )
-            except Exception as e:
+            except Exception as e:  # pylint: disable=broad-exception-caught
                 self.logger.error(f"Error transferring file: {file}")
                 self.logger.error(e)
                 result = 1
 
         return result
 
-    def create_flag_files(self):
+    def create_flag_files(self) -> int:
+        """Create the flag files on the S3 bucket.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         result = 0
 
         object_key = self.spec["flags"]["fullPath"]
         self.logger.debug(f"Creating flag file: {object_key}")
         kwargs = {
             "Bucket": self.spec["bucket"],
             "Key": object_key,
         }
         if self.bucket_owner_full_control:
             kwargs["ACL"] = "bucket-owner-full-control"
 
         try:
             self.s3_client.put_object(**kwargs)
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-exception-caught
             self.logger.error(f"Error creating flag file: {object_key}")
             self.logger.error(e)
             result = 1
 
         return result
 
-    def tidy(self):
+    def tidy(self) -> None:
+        """Tidy up the S3 client."""
         self.s3_client.close()
 
 
 class S3Execution(RemoteExecutionHandler):
+    """S3 remote execution handler.
+
+    This is a strange one, because it's not really an execution. But it's a way to
+    create flag files without having to define an entire transfer specification.
+    """
+
     TASK_TYPE = "E"
 
-    def tidy(self):
+    def tidy(self) -> None:
+        """Tidy up the S3 client."""
         self.s3_client.close()
 
-    def __init__(self, spec):
-        self.spec = spec
+    def __init__(self, spec: dict):
+        """Initialise the S3Execution handler.
 
-        self.logger = opentaskpy.logging.init_logging(
+        Args:
+            spec (dict): The spec for the execution.
+        """
+        self.logger = opentaskpy.otflogging.init_logging(
             __name__, os.environ.get("OTF_TASK_ID"), self.TASK_TYPE
         )
 
+        super().__init__(spec)
+
         set_aws_creds(self)
 
         # Use boto3 to setup the required object
         kwargs = {
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "region_name": self.region_name,
         }
         # If there's an override for endpoint_url in the environment, then use that
         if os.environ.get("AWS_ENDPOINT_URL"):
             kwargs["endpoint_url"] = os.environ.get("AWS_ENDPOINT_URL")
 
         self.s3_client = boto3.client("s3", **kwargs)
 
-    # This cannot be long running, so kill doesnt really need to do anything
-    def kill(self):
-        pass
-
-    def execute(self):
+    # This cannot be long running, so kill doesn't really need to do anything
+    def kill(self) -> None:
+        """Kill the remote process."""
+
+    def execute(self) -> bool:
+        """Execute the remote command.
+
+        Returns:
+            bool: True if the command was executed successfully, False otherwise
+        """
         result = True
 
         object_key = self.spec["key"]
         bucket = self.spec["bucket"]
 
         kwargs = {
             "Bucket": bucket,
@@ -274,13 +372,13 @@
         }
         if self.bucket_owner_full_control:
             kwargs["ACL"] = "bucket-owner-full-control"
 
         # Use the boto client to write a blank file with this name to the bucket
         try:
             self.s3_client.put_object(**kwargs)
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-exception-caught
             self.logger.error(f"Failed to create flag file: {object_key}")
             self.logger.error(e)
             result = False
 
         return result
```

### Comparing `otf-addons-aws-0.4.0/src/opentaskpy/plugins/lookup/aws/ssm.py` & `otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/ssm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,64 @@
-"""
-SSM Param Store lookup plugin
+"""SSM Param Store lookup plugin.
 
 Uses boto3 to pull out a parameter from AWS Parameter Store
 This uses AWS authentication, either from the IAM role of the host,
 by using environment variables, or variables in variables.json file
-
 """
 import os
 
 import boto3
-import opentaskpy.logging
+import opentaskpy.otflogging
 from botocore.exceptions import ClientError
+from opentaskpy.exceptions import LookupPluginError
 
-logger = opentaskpy.logging.init_logging(__name__)
+logger = opentaskpy.otflogging.init_logging(__name__)
 
 plugin_name = "ssm"
 
 
-def run(**kwargs):
+def run(**kwargs):  # type: ignore[no-untyped-def]
+    """Pull a variable from AWS SSM.
+
+    Args:
+        **kwargs: Expect a kwarg named name. This should be the key within SSM to the
+        variable to obtain. The value should be a string.
+
+    Raises:
+        LookupPluginError: Returned if the kwarg 'name' is not provided
+        FileNotFoundError: Returned if the file does not exist
+
+    Returns:
+        _type_: The value read from the file
+    """
     # Expect a kwarg named url, and value
     expected_kwargs = ["name"]
     for kwarg in expected_kwargs:
         if kwarg not in kwargs:
-            raise Exception(
-                f"Missing kwarg: '{kwarg}' while trying to run lookup plugin '{plugin_name}'"
+            raise LookupPluginError(
+                f"Missing kwarg: '{kwarg}' while trying to run lookup plugin"
+                f" '{plugin_name}'"
             )
 
-    globals = kwargs["globals"] if "globals" in kwargs else None
+    globals_ = kwargs["globals"] if "globals" in kwargs else None
 
     aws_access_key_id = (
-        globals["AWS_ACCESS_KEY_ID"]
-        if globals and "AWS_ACCESS_KEY_ID" in globals
+        globals_["AWS_ACCESS_KEY_ID"]
+        if globals_ and "AWS_ACCESS_KEY_ID" in globals_
         else os.environ.get("AWS_ACCESS_KEY_ID")
     )
     aws_secret_access_key = (
-        globals["AWS_SECRET_ACCESS_KEY"]
-        if globals and "AWS_SECRET_ACCESS_KEY" in globals
+        globals_["AWS_SECRET_ACCESS_KEY"]
+        if globals_ and "AWS_SECRET_ACCESS_KEY" in globals_
         else os.environ.get("AWS_SECRET_ACCESS_KEY")
     )
 
     region_name = (
-        globals["AWS_REGION"]
-        if globals and "AWS_REGION" in globals
+        globals_["AWS_REGION"]
+        if globals_ and "AWS_REGION" in globals_
         else os.environ.get("AWS_REGION")
     )
     boto3_kwargs = {
         "aws_access_key_id": aws_access_key_id,
         "aws_secret_access_key": aws_secret_access_key,
         "region_name": region_name,
     }
@@ -61,13 +74,12 @@
 
         logger.log(12, f"Read '{result}' from param {kwargs['name']}")
 
     except ClientError as e:
         if e.response["Error"]["Code"] == "ParameterNotFound":
             logger.error(f"Parameter not found: {kwargs['name']}: {e}")
             raise e
-        else:
-            raise e
-    except Exception as e:
+        raise e
+    except Exception as e:  # pylint: disable=broad-exception-caught
         logger.error(f"Failed to read from SSM parameter: {kwargs['name']}: {e}")
 
     return result
```

### Comparing `otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/PKG-INFO` & `otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 0.4.0
+Version: 0.5.1
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
-
 ![unittest status](https://github.com/adammcdonagh/otf-addons-aws/actions/workflows/main.yml/badge.svg)
 
 This repository contains addons to allow integration with AWS components via [Open Task Framework (OTF)](https://github.com/adammcdonagh/open-task-framework)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 These addons include several additional features:
-  * A new plugin for SSM Param Store to pull dynamic variables
-  * A new remotehandler to push/pull files via AWS S3
-  * A new remote handler to trigger AWS Lambda functions
+
+- A new plugin for SSM Param Store to pull dynamic variables
+- A new remotehandler to push/pull files via AWS S3
+- A new remote handler to trigger AWS Lambda functions
 
 # AWS Credentials
 
-This package uses boto3 to communicate with AWS. 
+This package uses boto3 to communicate with AWS.
 
 Credentials can be set via config using equivalently named variables alongside the protocol definition e.g;
+
 ```json
 "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
     "access_key_id": "some_key",
     "secret_access_key": "some_secret_key",
     "region_name": "eu-west-1"
 }
@@ -48,22 +49,24 @@
 # Transfers
 
 Transfers are defined the same as a normal SSH based transfer.
 
 As part of the upload, the `bucket-owner-full-control` ACL flag is applied to all files. This can be disabled by setting `disableBucketOwnerControlACL` to `true` in the `protocol` definition
 
 ### Supported features
-   * Plain file watch
-   * File watch/transfer with file size and age constraints
-   * `move` & `delete` post copy actions
-   * Touching empty files after transfer. e.g. `.fin` files used as completion flags
-   * Touching empty files as an execution
+
+- Plain file watch
+- File watch/transfer with file size and age constraints
+- `move` & `delete` post copy actions
+- Touching empty files after transfer. e.g. `.fin` files used as completion flags
+- Touching empty files as an execution
 
 ### Limitations
-   * No support for log watch
+
+- No support for log watch
 
 # Configuration
 
 JSON configs for transfers can be defined as follows:
 
 ## Example File Watch Only
 
@@ -91,27 +94,29 @@
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example S3 Upload
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "protocol": {
           "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
         }
     }
 ]
 ```
 
 ## Example S3 upload with flag files
+
 ```json
 "destination": [
     {
         "bucket": "some-bucket",
         "directory": "dest",
         "flag": {
           "fullPath": "dest/some_fin.flg"
@@ -125,34 +130,35 @@
 
 # Executions
 
 The Lambda remote handler allows AWS Lambda functions to be called. When provided with a `functionArn` the function will be called with no parameters. If there's a payload to pass in, use the `payload` attribute in the execution definition to specify a JSON object to pass into the function.
 
 ## Asynchronous vs Synchronous Execution
 
-Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`. 
+Lambda functions can be called with either an `invocationType` of `Event` (default if not specified) or `RequestResponse`.
 
 `Event` is asynchronous, and tells the Lambda function to trigger, but does not check that it ran successfully. This means it's up to you to make sure that you have appropriate monitoring of your Lambda functions.
 
 `RequestResponse` will block until the Lambda function either completes, or times out. Boto3 has a timeout of 60 seconds, so this cannot be used for long running functions (over 1 minute). This also causes issues when used in conjunction with batches and timeouts. Since the request blocks, the thread cannot be killed by the batch thread, meaning that it will block any further execution until 60 seconds after triggering the lambda function.
 
-
 ## Example S3 Execution touch flag file
+
 ```json
 {
   "type": "execution",
   "bucket": "test-bucket",
   "key": "test_key.flg",
   "protocol": {
     "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
   }
 }
 ```
 
 ## Example Lambda function call
+
 ```json
 {
   "type": "execution",
   "functionArn": "arn:aws:lambda:eu-west-1:000000000000:function:my-function",
   "invocationType": "Event",
   "payload": {
     "file-name": "some_file.txt"
```

### Comparing `otf-addons-aws-0.4.0/src/otf_addons_aws.egg-info/SOURCES.txt` & `otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 src/opentaskpy/addons/aws/__init__.py
 src/opentaskpy/addons/aws/remotehandlers/__init__.py
-src/opentaskpy/addons/aws/remotehandlers/aws.py
+src/opentaskpy/addons/aws/remotehandlers/creds.py
 src/opentaskpy/addons/aws/remotehandlers/lambda.py
 src/opentaskpy/addons/aws/remotehandlers/s3.py
 src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
 src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
 src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
 src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
 src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
```

### Comparing `otf-addons-aws-0.4.0/tests/test_lambda_execution_schema_validate.py` & `otf-addons-aws-0.5.1/tests/test_lambda_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.4.0/tests/test_plugin_ssm.py` & `otf-addons-aws-0.5.1/tests/test_plugin_ssm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+# pylint: skip-file
 import json
 import logging
 
 import pytest
 from botocore.exceptions import ClientError
-from fixtures.localstack import *  # noqa:F401
 from opentaskpy.config.loader import ConfigLoader
 from pytest_shell import fs
 
 from opentaskpy.plugins.lookup.aws.ssm import run
+from tests.fixtures.localstack import *  # noqa: F403
 
 PLUGIN_NAME = "ssm"
 
 # Get the default logger and set it to DEBUG
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
```

### Comparing `otf-addons-aws-0.4.0/tests/test_remotehandler_lambda_execution.py` & `otf-addons-aws-0.5.1/tests/test_remotehandler_lambda_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+# pylint: skip-file
 import io
 import json
 import logging
 import os
 import re
 import subprocess
 import time
 import zipfile
+from contextlib import suppress
 
 import botocore.exceptions
-import opentaskpy.logging
+import opentaskpy.otflogging
 import pytest
-from fixtures.localstack import *  # noqa:F401
 from opentaskpy.config.loader import ConfigLoader
 from opentaskpy.taskhandlers import batch, execution
 from pytest_shell import fs
 
+from tests.fixtures.localstack import *  # noqa: F403, F405
+
 os.environ["OTF_NO_LOG"] = "0"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 BUCKET_NAME = "otf-addons-aws-lambda-execution-test"
 BUCKET_NAME_1 = "otf-addons-aws-lambda-execution-test-1"
 BUCKET_NAME_2 = "otf-addons-aws-lambda-execution-test-2"
-logger = opentaskpy.logging.init_logging(__name__)
+logger = opentaskpy.otflogging.init_logging(__name__)
 
 logger.setLevel(logging.DEBUG)
 
-root_dir_ = get_root_dir()
+root_dir_ = os.path.join(
+    os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
+    "test",
+)
 
 lambda_execution_task_definition = {
     "type": "execution",
     "functionArn": None,
     "payload": {"bucket_name": BUCKET_NAME, "file_name": "function_test.txt"},
     "protocol": {
         "name": "opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution",
@@ -60,18 +66,16 @@
         info = zipfile.ZipInfo(lambda_handler)
         info.compress_type = zipfile.ZIP_DEFLATED
         info.external_attr = 0o777 << 16  # give full access
         zf.writestr(info, lambda_code)
     zip_buffer.seek(0)
 
     # Delete existing function
-    try:
+    with suppress(Exception):
         lambda_client.delete_function(FunctionName="my-function")
-    except Exception:
-        pass
 
     # Create a lambda function that creates a file on our test S3 bucket
     lambda_response = lambda_client.create_function(
         FunctionName="my-function",
         Runtime="python3.9",
         Code={
             "ZipFile": zip_buffer.read(),
@@ -79,14 +83,28 @@
         Handler=f"{re.sub('.py', '', lambda_handler)}.lambda_handler",
         Role="arn:aws:iam::123456789012:role/lambda-role",
         Timeout=300,
         MemorySize=128,
     )
     function_arn = lambda_response["FunctionArn"]
 
+    # Wait for the function status to become Active, from Pending before proceeding
+    counter = 0
+    while True:
+        lambda_response = lambda_client.get_function(FunctionName=function_arn)
+        if lambda_response["Configuration"]["State"] == "Active":
+            break
+        counter += 1
+        # If we get to 10, then fail the text
+        if counter >= 10:
+            raise Exception(
+                "Lambda function failed to become active in reasonable time"
+            )
+        time.sleep(1)
+
     # Manually call the function to check it's actually working
     if invoke:
         lambda_client.invoke(
             FunctionName=function_arn,
             InvocationType="RequestResponse",
             Payload=json.dumps(payload),
         )
@@ -100,16 +118,18 @@
 def setup_bucket(credentials):
     # This all relies on docker container for the AWS stack being set up and running
     # The AWS CLI should also be installed
 
     buckets = [BUCKET_NAME, BUCKET_NAME_1, BUCKET_NAME_2]
     # Delete existing buckets and recreate
     for bucket in buckets:
-        subprocess.run(["awslocal", "s3", "rb", f"s3://{bucket}", "--force"])
-        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"])
+        subprocess.run(
+            ["awslocal", "s3", "rb", f"s3://{bucket}", "--force"], check=False
+        )
+        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"], check=False)
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
 def test_remote_handler(credentials):
     execution_obj = execution.Execution(
@@ -121,15 +141,15 @@
     # Validate some things were set as expected
     assert execution_obj.remote_handlers[0].__class__.__name__ == "LambdaExecution"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_run_lambda_function(setup_bucket, lambda_client, s3_client):
+def test_run_lambda_function(credentials, lambda_client, s3_client, setup_bucket):
     function_arn = create_lambda_function(
         lambda_client,
         "lambda_write_to_s3.py",
         {
             "bucket_name": BUCKET_NAME,
             "file_name": "function_test.txt",
         },
@@ -212,17 +232,17 @@
     lambda_execution_task_definition_invalid_payload = (
         lambda_execution_task_definition.copy()
     )
     # Update the task definition with the ARN of the function we just created
     lambda_execution_task_definition_invalid_payload["functionArn"] = function_arn
     # Remove the payload from the definition
     lambda_execution_task_definition_invalid_payload.pop("payload")
-    lambda_execution_task_definition_invalid_payload[
-        "invocationType"
-    ] = "RequestResponse"
+    lambda_execution_task_definition_invalid_payload["invocationType"] = (
+        "RequestResponse"
+    )
 
     # Call the execution and check whether the lambda function ran successfully
     execution_obj = execution.Execution(
         None, "call-lambda-function", lambda_execution_task_definition_invalid_payload
     )
 
     assert not execution_obj.run()
@@ -245,15 +265,15 @@
     function_arn = create_lambda_function(
         lambda_client, "lambda_sleep_60.py", None, invoke=False
     )
 
     # set the arn in lambda_execution_task_definition
     lambda_execution_task_definition["functionArn"] = function_arn
 
-    # We need to write the lambda execution defintion to a file for the config_loader to read from
+    # We need to write the lambda execution definition to a file for the config_loader to read from
     with open(f"{tmpdir}/lambda_execution_task_definition.json", "w") as f:
         json.dump(lambda_execution_task_definition, f)
 
     # Write a dummy variables file
     fs.create_files([{f"{tmpdir}/variables.json": {"content": "{}"}}])
 
     config_loader = ConfigLoader(tmpdir)
```

### Comparing `otf-addons-aws-0.4.0/tests/test_remotehandler_s3_execution.py` & `otf-addons-aws-0.5.1/tests/test_remotehandler_s3_execution.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,69 @@
+# pylint: skip-file
 import os
 import subprocess
 
 import pytest
-from fixtures.localstack import *  # noqa:F401
 from opentaskpy.taskhandlers import execution
 
+from tests.fixtures.localstack import *  # noqa: F403, F405
+
 os.environ["OTF_NO_LOG"] = "0"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 BUCKET_NAME = "otf-addons-aws-s3-execution-test"
 
-root_dir_ = get_root_dir()
 
+root_dir_ = os.path.join(
+    os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
+    "test",
+)
 
-@pytest.fixture(scope="function")
-def s3_execution_task_definition():
-    return {
-        "type": "execution",
-        "bucket": BUCKET_NAME,
-        "key": "test_flag.txt",
-        "protocol": {
-            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Execution",
-        },
-    }
+s3_execution_task_definition = {
+    "type": "execution",
+    "bucket": BUCKET_NAME,
+    "key": "test_flag.txt",
+    "protocol": {
+        "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Execution",
+    },
+}
 
 
 @pytest.fixture(scope="module")
 def setup_bucket(credentials):
     # This all relies on docker container for the AWS stack being set up and running
     # The AWS CLI should also be installed
 
     buckets = [BUCKET_NAME]
     # Delete existing buckets and recreate
     for bucket in buckets:
-        subprocess.run(["awslocal", "s3", "rb", f"s3://{bucket}", "--force"])
-        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"])
+        subprocess.run(
+            ["awslocal", "s3", "rb", f"s3://{bucket}", "--force"], check=False
+        )
+        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"], check=False)
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_remote_handler(s3_execution_task_definition):
+def test_remote_handler():
     execution_obj = execution.Execution(
         None, "s3-flag-file", s3_execution_task_definition
     )
 
     execution_obj._set_remote_handlers()
 
     # Validate some things were set as expected
     assert execution_obj.remote_handlers[0].__class__.__name__ == "S3Execution"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_touch_file(setup_bucket, s3_execution_task_definition):
+def test_s3_touch_file(setup_bucket):
     execution_obj = execution.Execution(
         None, "s3-flag-file", s3_execution_task_definition
     )
 
     assert execution_obj.run()
 
     # Check that the file has been created in the bucket
```

### Comparing `otf-addons-aws-0.4.0/tests/test_remotehandler_s3_transfer.py` & `otf-addons-aws-0.5.1/tests/test_remotehandler_s3_transfer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,316 +1,296 @@
+# pylint: skip-file
 import datetime
 import os
 import shutil
 import subprocess
 import threading
 
 import pytest
-from fixtures.localstack import *  # noqa:F401
 from opentaskpy.taskhandlers import transfer
 from pytest_shell import fs
 
 from opentaskpy import exceptions
+from tests.fixtures.localstack import *  # noqa: F403, F405
 
 os.environ["OTF_NO_LOG"] = "0"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 BUCKET_NAME = "otf-addons-aws-s3-test"
 BUCKET_NAME_2 = "otf-addons-aws-s3-test-2"
 
 
-root_dir_ = get_root_dir()
+root_dir_ = os.path.join(
+    os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
+    "test",
+)
 
 
-@pytest.fixture(scope="function")
-def s3_file_watch_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "protocol": {
-                "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-            },
-            "fileWatch": {
-                "timeout": 10,
-                "directory": "src",
-                "fileRegex": ".*\\.txt",
-            },
+s3_file_watch_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": ".*\\.txt",
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+        "fileWatch": {
+            "timeout": 10,
+        },
+    },
+}
+
+
+s3_age_conditions_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "fileRegex": ".*\\.txt",
+        "conditionals": {
+            "age": {
+                "gt": 10,
+                "lt": 18,
+            }
         },
-    }
-
-
-@pytest.fixture(scope="function")
-def s3_age_conditions_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "fileRegex": ".*\\.txt",
-            "conditionals": {
-                "age": {
-                    "gt": 10,
-                    "lt": 18,
-                }
-            },
-            "protocol": {
-                "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-            },
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
-
-
-@pytest.fixture(scope="function")
-def s3_file_size_conditions_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "fileRegex": ".*\\.txt",
-            "conditionals": {
-                "size": {
-                    "gt": 10,
-                    "lt": 20,
-                }
-            },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
             },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
-
+    ],
+}
 
-@pytest.fixture(scope="function")
-def s3_file_watch_custom_creds_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
+s3_file_size_conditions_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "fileRegex": ".*\\.txt",
+        "conditionals": {
+            "size": {
+                "gt": 10,
+                "lt": 20,
+            }
+        },
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                "access_key_id": "test",
-                "secret_access_key": "test",
-                "region_name": "eu-west-1",
-            },
-            "fileWatch": {
-                "timeout": 10,
-                "directory": "src",
-                "fileRegex": ".*\\.txt",
             },
         },
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_s3_copy_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
+s3_file_watch_custom_creds_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+            "access_key_id": "test",
+            "secret_access_key": "test",
+            "region_name": "eu-west-1",
+        },
+        "fileWatch": {
+            "timeout": 10,
             "directory": "src",
             "fileRegex": ".*\\.txt",
-            "protocol": {
-                "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-            },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
+    },
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_s3_copy_with_fin_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "directory": "src",
-            "fileRegex": ".*\\.txt",
+s3_to_s3_copy_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": ".*\\.txt",
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
             },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "flags": {
-                    "fullPath": "dest/my_fin.fin",
-                },
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_s3_pca_delete_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "directory": "src",
-            "fileRegex": "file-pca\\.txt",
-            "postCopyAction": {
-                "action": "delete",
+s3_to_s3_copy_with_fin_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": ".*\\.txt",
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
+            "flags": {
+                "fullPath": "dest/my_fin.fin",
             },
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
             },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_s3_pca_move_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "directory": "src",
-            "fileRegex": "file-pca\\.txt",
-            "postCopyAction": {
-                "action": "move",
-                "destination": "src/archive/",
-            },
+s3_to_s3_pca_delete_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": "file-pca\\.txt",
+        "postCopyAction": {
+            "action": "delete",
+        },
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
             },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_s3_pca_rename_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "directory": "src",
-            "fileRegex": "file-pca-rename-(.*)\\.txt",
-            "postCopyAction": {
-                "action": "rename",
-                "destination": "src/archive/",
-                "pattern": "file-pca-rename-(.*)\\.txt",
-                "sub": "file-pca-rename-\\1-renamed.txt",
-            },
+s3_to_s3_pca_move_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": "file-pca\\.txt",
+        "postCopyAction": {
+            "action": "move",
+            "destination": "src/archive/",
+        },
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
             "protocol": {
                 "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
             },
         },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME_2,
-                "directory": "dest",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
-                },
-            },
-        ],
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def s3_to_ssh_copy_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "bucket": BUCKET_NAME,
-            "directory": "src",
-            "fileRegex": ".*\\.txt",
-            "protocol": {"name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"},
+s3_to_s3_pca_rename_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": "file-pca-rename-(.*)\\.txt",
+        "postCopyAction": {
+            "action": "rename",
+            "destination": "src/archive/",
+            "pattern": "file-pca-rename-(.*)\\.txt",
+            "sub": "file-pca-rename-\\1-renamed.txt",
+        },
+        "protocol": {
+            "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME_2,
+            "directory": "dest",
+            "protocol": {
+                "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer",
+            },
         },
-        "destination": [
-            {
-                "hostname": "172.16.1.12",
-                "directory": "/tmp/testFiles/dest",
-                "protocol": {
-                    "name": "ssh",
-                    "credentials": {
-                        "username": "application",
-                        "keyFile": f"{root_dir_}/testFiles/id_rsa",
-                    },
-                },
-            }
-        ],
-    }
+    ],
+}
 
 
-@pytest.fixture(scope="function")
-def ssh_to_s3_copy_task_definition():
-    return {
-        "type": "transfer",
-        "source": {
-            "hostname": "172.16.1.12",
-            "directory": "/tmp/testFiles/src",
-            "fileRegex": ".*\\.txt",
+s3_to_ssh_copy_task_definition = {
+    "type": "transfer",
+    "source": {
+        "bucket": BUCKET_NAME,
+        "directory": "src",
+        "fileRegex": ".*\\.txt",
+        "protocol": {"name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"},
+    },
+    "destination": [
+        {
+            "hostname": "127.0.0.1",
+            "directory": "/tmp/testFiles/dest",
             "protocol": {
                 "name": "ssh",
+                "port": "3221",
                 "credentials": {
                     "username": "application",
                     "keyFile": f"{root_dir_}/testFiles/id_rsa",
                 },
             },
-        },
-        "destination": [
-            {
-                "bucket": BUCKET_NAME,
-                "directory": "dest",
-                "fileRegex": ".*\\.txt",
-                "protocol": {
-                    "name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"
-                },
-            }
-        ],
-    }
+        }
+    ],
+}
+
+ssh_to_s3_copy_task_definition = {
+    "type": "transfer",
+    "source": {
+        "hostname": "127.0.0.1",
+        "directory": "/tmp/testFiles/src",
+        "fileRegex": ".*\\.txt",
+        "protocol": {
+            "name": "ssh",
+            "port": "3222",
+            "credentials": {
+                "username": "application",
+                "keyFile": f"{root_dir_}/testFiles/id_rsa",
+            },
+        },
+    },
+    "destination": [
+        {
+            "bucket": BUCKET_NAME,
+            "directory": "dest",
+            "fileRegex": ".*\\.txt",
+            "protocol": {"name": "opentaskpy.addons.aws.remotehandlers.s3.S3Transfer"},
+        }
+    ],
+}
 
 
 @pytest.fixture(scope="session")
 def test_files(root_dir):
     # Get the root directory of the project
 
     structure = [
@@ -341,23 +321,24 @@
     address = f"{docker_services.docker_ip}:{port}"
     return address
 
 
 @pytest.fixture(scope="session")
 def setup_ssh_keys(docker_services, root_dir, test_files, ssh_1, ssh_2):
     # Run command locally
-    # if ssh key dosent exist yet
+    # if ssh key doesn't exist yet
     ssh_private_key_file = f"{root_dir}/testFiles/id_rsa"
     if not os.path.isfile(ssh_private_key_file):
         subprocess.run(
-            ["ssh-keygen", "-t", "rsa", "-N", "", "-f", ssh_private_key_file]
-        ).returncode
+            ["ssh-keygen", "-t", "rsa", "-N", "", "-f", ssh_private_key_file],
+            check=True,
+        )
 
         # Copy the file into the ssh directory for each host
-        for i in ["1", "2"]:
+        for i in ("1", "2"):
             shutil.copy(
                 ssh_private_key_file, f"{root_dir}/testFiles/ssh_{i}/ssh/id_rsa"
             )
             shutil.copy(
                 f"{root_dir}/testFiles/id_rsa.pub",
                 f"{root_dir}/testFiles/ssh_{i}/ssh/authorized_keys",
             )
@@ -375,35 +356,37 @@
             "/tmp/testFiles/ssh/authorized_keys",
             "/home/application/.ssh/authorized_keys",
         ),
         ("chown", "-R", "application", "/home/application/.ssh"),
         ("chmod", "-R", "700", "/home/application/.ssh"),
         ("chown", "-R", "application", "/tmp/testFiles"),
     ]
-    for host in ["ssh_1", "ssh_2"]:
+    for host in ("ssh_1", "ssh_2"):
         for command in commands:
             docker_services.execute(host, *command)
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture(scope="function")
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
 def setup_bucket(credentials):
     # This all relies on docker container for the AWS stack being set up and running
     # The AWS CLI should also be installed
 
     buckets = [BUCKET_NAME, BUCKET_NAME_2]
     # Delete existing buckets and recreate
     for bucket in buckets:
-        subprocess.run(["awslocal", "s3", "rb", f"s3://{bucket}", "--force"])
-        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"])
+        subprocess.run(
+            ["awslocal", "s3", "rb", f"s3://{bucket}", "--force"], check=False
+        )
+        subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"], check=False)
 
 
-def test_remote_handler(s3_file_watch_task_definition):
+def test_remote_handler():
     transfer_obj = transfer.Transfer(
         None, "s3-file-watch", s3_file_watch_task_definition
     )
 
     transfer_obj._set_remote_handlers()
 
     # Validate some things were set as expected
@@ -412,15 +395,15 @@
     # dest_remote_handler should be None
     assert transfer_obj.dest_remote_handlers is None
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_file_watch(setup_bucket, tmp_path, s3_file_watch_task_definition):
+def test_s3_file_watch(setup_bucket, tmp_path):
     transfer_obj = transfer.Transfer(
         None, "s3-file-watch", s3_file_watch_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d")
 
@@ -436,25 +419,25 @@
     # This time write the contents after 5 seconds
     t = threading.Timer(
         5,
         create_s3_file,
         [f"{tmp_path}/{datestamp}.txt", "src/test.txt"],
     )
     t.start()
-    print("Started thread - Expect file in 5 seconds, starting task-run now...")
+    print(  # noqa: T201
+        "Started thread - Expect file in 5 seconds, starting task-run now..."
+    )
 
     assert transfer_obj.run()
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_age_conditions_size(
-    setup_bucket, tmp_path, s3_age_conditions_task_definition
-):
+def test_s3_age_conditions_size(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-age-conditions", s3_age_conditions_task_definition
     )
 
     # Write a test file locally
     files = [
         {f"{tmp_path}/too_old_file.txt": {"content": "123"}},
@@ -468,35 +451,24 @@
         file_name = os.path.basename(list(file.keys())[0])
         create_s3_file(list(file.keys())[0], f"src/{file_name}")
         # Sleep 6 seconds
         time.sleep(6)
 
     assert transfer_obj.run()
 
-    # Check that only correct_file.txt is in the bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/",
-        ],
-        stdout=subprocess.PIPE,
-    )
-    assert "correct_file.txt" in result.stdout.decode("utf-8")
-    assert "too_old_file.txt" not in result.stdout.decode("utf-8")
-    assert "too_new_file.txt" not in result.stdout.decode("utf-8")
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    # check that the correct_file.txt is in the bucket, and not the other 2
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "dest/correct_file.txt"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_file_conditions_size(
-    setup_bucket, tmp_path, s3_file_size_conditions_task_definition
-):
+def test_s3_file_conditions_size(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-file-size-conditions", s3_file_size_conditions_task_definition
     )
 
     # Write a test file locally
     files = [
         {f"{tmp_path}/too_small_file.txt": {"content": "1"}},
@@ -506,112 +478,75 @@
     fs.create_files(files)
     for file in files:
         file_name = os.path.basename(list(file.keys())[0])
         create_s3_file(list(file.keys())[0], f"src/{file_name}")
 
     assert transfer_obj.run()
 
-    # Check that only correct_file.txt is in the bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/",
-        ],
-        stdout=subprocess.PIPE,
-    )
-    assert "correct_file.txt" in result.stdout.decode("utf-8")
-    assert "too_small_file.txt" not in result.stdout.decode("utf-8")
-    assert "too_large_file.txt" not in result.stdout.decode("utf-8")
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    # check that the correct_file.txt is in the bucket, and not the other 2
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "dest/correct_file.txt"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_copy(setup_bucket, tmp_path, s3_to_s3_copy_task_definition):
+def test_s3_to_s3_copy(setup_bucket, s3_client, tmp_path):
     transfer_obj = transfer.Transfer(None, "s3-to-s3", s3_to_s3_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
     create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/test.txt",
-        ],
-        capture_output=True,
+    s3_response = s3_client.head_object(
+        Bucket=BUCKET_NAME_2,
+        Key="dest/test.txt",
     )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    assert s3_response["ResponseMetadata"]["HTTPStatusCode"] == 200
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_with_fin_copy(
-    setup_bucket, tmp_path, s3_to_s3_copy_with_fin_task_definition
-):
+def test_s3_to_s3_with_fin_copy(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-with-fin", s3_to_s3_copy_with_fin_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
     create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
-    # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/test.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
 
-    # Make sure that the fin file has been created
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/my_fin.fin",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    assert len(objects["Contents"]) == 2
+    # Check that the file and fin file are in the destination bucket
+    object_keys = [obj["Key"] for obj in objects["Contents"]]
+    assert "dest/test.txt" in object_keys
+    assert "dest/my_fin.fin" in object_keys
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_copy_disable_bucket_owner_acl(
-    setup_bucket, tmp_path, s3_to_s3_copy_task_definition
-):
+def test_s3_to_s3_copy_disable_bucket_owner_acl(setup_bucket, s3_client, tmp_path):
     s3_to_s3_copy_task_definition["destination"][0]["protocol"][
         "disableBucketOwnerControlACL"
     ] = True
     transfer_obj = transfer.Transfer(None, "s3-to-s3", s3_to_s3_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
@@ -619,171 +554,104 @@
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
     create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
-    # Cant really test this works with localstack, since there's no actual IAM permissions set on anything
+    # Can't really test this works with localstack, since there's no actual IAM permissions set on anything
     # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/test.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "dest/test.txt"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_copy_pca_delete(
-    setup_bucket, tmp_path, s3_to_s3_pca_delete_task_definition
-):
+def test_s3_to_s3_copy_pca_delete(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-delete", s3_to_s3_pca_delete_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
     create_s3_file(f"{tmp_path}/{datestamp}.txt", f"src/{datestamp}.txt")
 
     assert transfer_obj.run()
 
-    # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/{datestamp}.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    # check that the correct_file.txt is in the bucket, and not the other 2
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == f"dest/{datestamp}.txt"
 
     # Check that the file is not in the source bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME}/src/{datestamp}.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 1
-    assert result.returncode == 1
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME)
+    assert "Contents" not in objects
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_copy_pca_move(
-    setup_bucket, tmp_path, s3_to_s3_pca_move_task_definition
-):
+def test_s3_to_s3_copy_pca_move(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-move", s3_to_s3_pca_move_task_definition
     )
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/pca-move.txt": {"content": "test1234"}}])
     create_s3_file(f"{tmp_path}/pca-move.txt", "src/pca-move.txt")
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/pca-move.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "dest/pca-move.txt"
 
     # Check that the file has been moved to archive
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME}/src/archive/pca-move.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 1
-    assert result.returncode == 1
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME)
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "src/archive/pca-move.txt"
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_s3_to_s3_copy_pca_rename(
-    setup_bucket, tmp_path, s3_to_s3_pca_rename_task_definition
-):
+def test_s3_to_s3_copy_pca_rename(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-rename", s3_to_s3_pca_rename_task_definition
     )
 
     # Write a test file locally
     fs.create_files([{f"{tmp_path}/file-pca-rename-1234.txt": {"content": "test1234"}}])
     create_s3_file(
         f"{tmp_path}/file-pca-rename-1234.txt", "src/file-pca-rename-1234.txt"
     )
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME_2}/dest/file-pca-rename-1234.txt",
-        ],
-        capture_output=True,
-    )
-    # Asset result.returncode is 0
-    assert result.returncode == 0
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
+    assert len(objects["Contents"]) == 1
+    assert objects["Contents"][0]["Key"] == "dest/file-pca-rename-1234.txt"
 
-    # Check that the file has been moved to archive
-    result = subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "ls",
-            f"s3://{BUCKET_NAME}/src/archive/file-pca-rename-renamed.txt",
-        ],
-        capture_output=True,
+    objects = s3_client.list_objects(Bucket=BUCKET_NAME)
+    assert len(objects["Contents"]) == 1
+    assert (
+        objects["Contents"][0]["Key"] == "src/archive/file-pca-rename-1234-renamed.txt"
     )
-    # Asset result.returncode is 1
-    assert result.returncode == 1
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
-def test_s3_to_ssh_copy(
-    setup_bucket, tmp_path, setup_ssh_keys, s3_to_ssh_copy_task_definition
-):
+def test_s3_to_ssh_copy(setup_bucket, tmp_path, setup_ssh_keys):
     transfer_obj = transfer.Transfer(None, "s3-to-ssh", s3_to_ssh_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
@@ -791,17 +659,15 @@
 
     assert transfer_obj.run()
 
 
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
-def test_ssh_to_s3_copy(
-    setup_bucket, root_dir, setup_ssh_keys, ssh_to_s3_copy_task_definition
-):
+def test_ssh_to_s3_copy(setup_bucket, root_dir, setup_ssh_keys):
     transfer_obj = transfer.Transfer(None, "ssh-to-s3", ssh_to_s3_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
     fs.create_files(
@@ -827,15 +693,14 @@
 @pytest.mark.skipif(
     condition=github_actions(), reason="cannot run localstack tests in github actions"
 )
 def test_s3_file_watch_custom_creds(
     setup_bucket,
     tmp_path,
     cleanup_credentials,
-    s3_file_watch_custom_creds_task_definition,
 ):
     transfer_obj = transfer.Transfer(
         None, "s3-file-watch-custom-creds", s3_file_watch_custom_creds_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d")
```

### Comparing `otf-addons-aws-0.4.0/tests/test_s3_source_schema_validate.py` & `otf-addons-aws-0.5.1/tests/test_s3_source_schema_validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 from opentaskpy.config.schemas import validate_transfer_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
     return {
@@ -9,25 +10,25 @@
     }
 
 
 @pytest.fixture(scope="function")
 def valid_transfer(valid_protocol_definition):
     return {
         "bucket": "test-bucket",
-        "path": "/src",
+        "directory": "/src",
         "fileRegex": ".*\\.txt",
         "protocol": valid_protocol_definition,
     }
 
 
 @pytest.fixture(scope="function")
 def valid_destination(valid_protocol_definition):
     return {
         "bucket": "test-bucket",
-        "path": "/dest",
+        "directory": "/dest",
         "protocol": valid_protocol_definition,
     }
 
 
 def test_s3_source_basic(valid_transfer):
     json_data = {
         "type": "transfer",
```

