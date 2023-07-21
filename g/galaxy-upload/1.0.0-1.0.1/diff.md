# Comparing `tmp/galaxy-upload-1.0.0.tar.gz` & `tmp/galaxy-upload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-upload-1.0.0.tar", last modified: Fri Aug 12 17:13:40 2022, max compression
+gzip compressed data, was "galaxy-upload-1.0.1.tar", last modified: Fri Jul 21 14:36:39 2023, max compression
```

## Comparing `galaxy-upload-1.0.0.tar` & `galaxy-upload-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2022-08-12 17:13:40.396409 galaxy-upload-1.0.0/
--rw-rw-r--   0 nate      (1000) nate      (1000)       85 2022-07-12 16:38:13.000000 galaxy-upload-1.0.0/HISTORY.rst
--rw-rw-r--   0 nate      (1000) nate      (1000)     1071 2022-07-11 18:56:44.000000 galaxy-upload-1.0.0/LICENSE
--rw-rw-r--   0 nate      (1000) nate      (1000)       22 2022-07-12 16:48:01.000000 galaxy-upload-1.0.0/MANIFEST.in
--rw-rw-r--   0 nate      (1000) nate      (1000)     8045 2022-08-12 17:13:40.396409 galaxy-upload-1.0.0/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)     6817 2022-07-13 22:43:04.000000 galaxy-upload-1.0.0/README.rst
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2022-08-12 17:13:40.396409 galaxy-upload-1.0.0/galaxy_upload/
--rw-rw-r--   0 nate      (1000) nate      (1000)       22 2022-08-12 17:12:44.000000 galaxy-upload-1.0.0/galaxy_upload/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2371 2022-07-13 23:01:20.000000 galaxy-upload-1.0.0/galaxy_upload/history.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     6089 2022-08-12 17:07:08.000000 galaxy-upload-1.0.0/galaxy_upload/upload.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2022-08-12 17:13:40.396409 galaxy-upload-1.0.0/galaxy_upload.egg-info/
--rw-rw-r--   0 nate      (1000) nate      (1000)     8045 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      366 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)      111 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/entry_points.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       60 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       14 2022-08-12 17:13:40.000000 galaxy-upload-1.0.0/galaxy_upload.egg-info/top_level.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       81 2022-07-07 18:12:23.000000 galaxy-upload-1.0.0/pyproject.toml
--rw-rw-r--   0 nate      (1000) nate      (1000)     1540 2022-08-12 17:13:40.400409 galaxy-upload-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:39.977349 galaxy-upload-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-21 14:36:39.977349 galaxy-upload-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:39.977349 galaxy-upload-1.0.1/galaxy_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/galaxy_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/galaxy_upload/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/galaxy_upload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:39.977349 galaxy-upload-1.0.1/galaxy_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 14:36:39.000000 galaxy-upload-1.0.1/galaxy_upload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 14:36:21.000000 galaxy-upload-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-21 14:36:39.977349 galaxy-upload-1.0.1/setup.cfg
```

### Comparing `galaxy-upload-1.0.0/LICENSE` & `galaxy-upload-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-upload-1.0.0/PKG-INFO` & `galaxy-upload-1.0.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,20 @@
-Metadata-Version: 2.1
-Name: galaxy-upload
-Version: 1.0.0
-Summary: Galaxy Upload Utility
-Home-page: https://github.com/galaxyproject/galaxy-upload
-Author: Galaxy Project and Community
-Author-email: galaxy-committers@lists.galaxyproject.org
-License: MIT
-Project-URL: Bug Tracker, https://github.com/galaxyproject/galaxy-upload/issues
-Project-URL: Documentation, https://galaxy-upload.readthedocs.io/
-Project-URL: Source Code, https://github.com/galaxyproject/galaxy-upload
-Keywords: Galaxy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ====================================================
  galaxy-upload - Galaxy Command-Line Upload Utility
 ====================================================
 
 A utility for uploading files to a Galaxy server from the command line. galaxy-upload supports `Galaxy`_ servers 22.01+,
 which include support for resumable uploads with the `tus`_ protocol.
 
 Installation
 ============
 
+Using pip
+---------
+
 Python 3.7 or later is required.
 
 To install::
 
     $ pip install galaxy-upload
 
 This installs two commands: ``galaxy-upload``, used to upload file(s) to a Galaxy server, and ``galaxy-history-search``,
@@ -48,14 +23,54 @@
 To make your life easier, you are encourged to install into a Python virtual environment. The easiest way to do this is
 with Python's built-in `venv`_ module::
 
     $ python3 -m venv ~/galaxy-upload
     $ . ~/galaxy-upload/bin/activate
     $ pip install galaxy-upload
 
+Using Conda
+-----------
+
+Alternatively, galaxy-upload can be installed using the `Conda`_ package manager. The `galaxy-upload Conda package`_ can
+be found on the `bioconda`_ channel and installed like so::
+
+    $ conda create -n galaxy-upload -c conda-forge -c bioconda galaxy-upload
+    $ conda activate galaxy-upload
+
+Using Containers
+----------------
+
+It is also possible to run galaxy-upload in either a `Docker`_ or `Singularity`_/`Apptainer`_ container. The
+`galaxy-upload BioContainer`_ is automatically built and maintained by the `BioContainers`_ project.
+
+To use the Docker container::
+
+    $ docker run -it --rm -v "$(pwd):$(pwd)" -w "$(pwd)" -u "$(id -u):$(id -g)" \
+        quay.io/biocontainers/galaxy-upload:1.0.0--pyhdfd78af_0 /bin/bash
+
+Or as a single command without entering an interactive shell::
+
+    $ docker run --rm -v "$(pwd):$(pwd)" -w "$(pwd)" -u "$(id -u):$(id -g)" \
+        quay.io/biocontainers/galaxy-upload:1.0.0--pyhdfd78af_0 galaxy-upload
+
+Adjust the values of ``-v`` and ``-w`` according to where the data you want to upload are located. In the example above,
+it is assumed they are in the current working directory.
+
+To use the Singularity container::
+
+    $ singularity run https://depot.galaxyproject.org/singularity/galaxy-upload:1.0.0--pyhdfd78af_0
+
+Or as a single command without entering an interactive shell::
+
+    $ singularity run https://depot.galaxyproject.org/singularity/galaxy-upload:1.0.0--pyhdfd78af_0 galaxy-upload
+
+Additional (newer) versions of the container may be available, BioContainers does not use the ``latest`` tag, but you
+can find all tags (which are valid for the Singularity images hosted on depot.galaxyproject.org as well as the Docker
+images) at the `galaxy-upload quay.io page`_
+
 Usage
 =====
 
 Upload a pair of fastq.gz files::
 
     $ galaxy-upload --url https://usegalaxy.org \
         --api-key 70ffeec0ffeea11e1eaccede1337loaf --history-name 'Run 2' \
@@ -127,16 +142,16 @@
 
 Note that if you are trying to re-upload (not resume) a file that you have already uploaded once before, you will need
 to remove it from the storage file or use a different storage file.
 
 .. _Galaxy: http://galaxyproject.org/
 .. _tus: https://tus.io/
 .. _venv: https://docs.python.org/3/library/venv.html
-
-=========
- History
-=========
-
-0.0.1
-=====
-
-- Initial release for comment and testing
+.. _Conda: https://docs.conda.io/
+.. _galaxy-upload Conda package: https://anaconda.org/bioconda/galaxy-upload
+.. _bioconda: https://bioconda.github.io/
+.. _Docker: https://www.docker.com/
+.. _Singularity: https://sylabs.io/docs/
+.. _Apptainer: https://apptainer.org/
+.. _galaxy-upload BioContainer: https://biocontainers.pro/tools/galaxy-upload
+.. _BioContainers: https://biocontainers.pro/
+.. _galaxy-upload quay.io page: https://quay.io/repository/biocontainers/galaxy-upload
```

### Comparing `galaxy-upload-1.0.0/galaxy_upload/history.py` & `galaxy-upload-1.0.1/galaxy_upload/history.py`

 * *Files identical despite different names*

### Comparing `galaxy-upload-1.0.0/galaxy_upload/upload.py` & `galaxy-upload-1.0.1/galaxy_upload/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 @optgroup.option(
     "--storage", type=click.Path(), required=False, help="Store URLs to resume here"
 )
 @optgroup.option(
     "--silent", is_flag=True, default=False, help="No output while uploading"
 )
 @optgroup.option("--debug", is_flag=True, default=False, help="Debug output")
-@click.argument("path", type=click.Path(), nargs=-1)
+@click.argument("path", type=click.Path(exists=True, dir_okay=False), nargs=-1)
 def main(url, path, api_key, **kwargs):
     paths = path
     if not paths:
         message = "WARNING: No paths to upload specified (see --help)"
         click.echo(click.style(message, bold=True, fg="yellow"), err=True)
     elif len(paths) > 1 and kwargs["file_name"]:
         message = "ERROR: --file-name option cannot be used with multiple paths"
```

### Comparing `galaxy-upload-1.0.0/galaxy_upload.egg-info/PKG-INFO` & `galaxy-upload-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-upload
-Version: 1.0.0
+Version: 1.0.1
 Summary: Galaxy Upload Utility
 Home-page: https://github.com/galaxyproject/galaxy-upload
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/galaxyproject/galaxy-upload/issues
 Project-URL: Documentation, https://galaxy-upload.readthedocs.io/
@@ -17,14 +17,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================================================
  galaxy-upload - Galaxy Command-Line Upload Utility
@@ -32,14 +33,17 @@
 
 A utility for uploading files to a Galaxy server from the command line. galaxy-upload supports `Galaxy`_ servers 22.01+,
 which include support for resumable uploads with the `tus`_ protocol.
 
 Installation
 ============
 
+Using pip
+---------
+
 Python 3.7 or later is required.
 
 To install::
 
     $ pip install galaxy-upload
 
 This installs two commands: ``galaxy-upload``, used to upload file(s) to a Galaxy server, and ``galaxy-history-search``,
@@ -48,14 +52,54 @@
 To make your life easier, you are encourged to install into a Python virtual environment. The easiest way to do this is
 with Python's built-in `venv`_ module::
 
     $ python3 -m venv ~/galaxy-upload
     $ . ~/galaxy-upload/bin/activate
     $ pip install galaxy-upload
 
+Using Conda
+-----------
+
+Alternatively, galaxy-upload can be installed using the `Conda`_ package manager. The `galaxy-upload Conda package`_ can
+be found on the `bioconda`_ channel and installed like so::
+
+    $ conda create -n galaxy-upload -c conda-forge -c bioconda galaxy-upload
+    $ conda activate galaxy-upload
+
+Using Containers
+----------------
+
+It is also possible to run galaxy-upload in either a `Docker`_ or `Singularity`_/`Apptainer`_ container. The
+`galaxy-upload BioContainer`_ is automatically built and maintained by the `BioContainers`_ project.
+
+To use the Docker container::
+
+    $ docker run -it --rm -v "$(pwd):$(pwd)" -w "$(pwd)" -u "$(id -u):$(id -g)" \
+        quay.io/biocontainers/galaxy-upload:1.0.0--pyhdfd78af_0 /bin/bash
+
+Or as a single command without entering an interactive shell::
+
+    $ docker run --rm -v "$(pwd):$(pwd)" -w "$(pwd)" -u "$(id -u):$(id -g)" \
+        quay.io/biocontainers/galaxy-upload:1.0.0--pyhdfd78af_0 galaxy-upload
+
+Adjust the values of ``-v`` and ``-w`` according to where the data you want to upload are located. In the example above,
+it is assumed they are in the current working directory.
+
+To use the Singularity container::
+
+    $ singularity run https://depot.galaxyproject.org/singularity/galaxy-upload:1.0.0--pyhdfd78af_0
+
+Or as a single command without entering an interactive shell::
+
+    $ singularity run https://depot.galaxyproject.org/singularity/galaxy-upload:1.0.0--pyhdfd78af_0 galaxy-upload
+
+Additional (newer) versions of the container may be available, BioContainers does not use the ``latest`` tag, but you
+can find all tags (which are valid for the Singularity images hosted on depot.galaxyproject.org as well as the Docker
+images) at the `galaxy-upload quay.io page`_
+
 Usage
 =====
 
 Upload a pair of fastq.gz files::
 
     $ galaxy-upload --url https://usegalaxy.org \
         --api-key 70ffeec0ffeea11e1eaccede1337loaf --history-name 'Run 2' \
@@ -127,16 +171,37 @@
 
 Note that if you are trying to re-upload (not resume) a file that you have already uploaded once before, you will need
 to remove it from the storage file or use a different storage file.
 
 .. _Galaxy: http://galaxyproject.org/
 .. _tus: https://tus.io/
 .. _venv: https://docs.python.org/3/library/venv.html
+.. _Conda: https://docs.conda.io/
+.. _galaxy-upload Conda package: https://anaconda.org/bioconda/galaxy-upload
+.. _bioconda: https://bioconda.github.io/
+.. _Docker: https://www.docker.com/
+.. _Singularity: https://sylabs.io/docs/
+.. _Apptainer: https://apptainer.org/
+.. _galaxy-upload BioContainer: https://biocontainers.pro/tools/galaxy-upload
+.. _BioContainers: https://biocontainers.pro/
+.. _galaxy-upload quay.io page: https://quay.io/repository/biocontainers/galaxy-upload
 
 =========
  History
 =========
 
+1.0.1
+=====
+
+- Document installation/usage with conda and containers by @natefoo in https://github.com/galaxyproject/galaxy-upload/pull/7
+- Use click to require file arg to exist by @natefoo in https://github.com/galaxyproject/galaxy-upload/pull/9
+- Pin tuspy to !=1.0.1 due to issue with upload_chunk(). by @natefoo in https://github.com/galaxyproject/galaxy-upload/pull/10
+
+1.0.0
+=====
+
+- Initial release
+
 0.0.1
 =====
 
-- Initial release for comment and testing
+- Initial prerelease for comment and testing
```

### Comparing `galaxy-upload-1.0.0/setup.cfg` & `galaxy-upload-1.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development
 description = Galaxy Upload Utility
 keywords = 
 	Galaxy
 license = MIT
 license_files = 
 	LICENSE
@@ -42,15 +43,15 @@
 [options]
 include_package_data = True
 install_requires = 
 	bioblend>=0.18.0
 	click
 	click-option-group
 	rich
-	tuspy>=1.0.0
+	tuspy>=1.0.0,!=1.0.1
 packages = find:
 python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
 	galaxy-upload = galaxy_upload.upload:main
 	galaxy-history-search = galaxy_upload.history:main
```

