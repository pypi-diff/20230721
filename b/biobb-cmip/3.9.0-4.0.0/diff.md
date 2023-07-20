# Comparing `tmp/biobb_cmip-3.9.0.tar.gz` & `tmp/biobb_cmip-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_cmip-3.9.0.tar", last modified: Tue Jan 17 10:59:35 2023, max compression
+gzip compressed data, was "dist/biobb_cmip-4.0.0.tar", last modified: Thu Jul 20 22:44:46 2023, max compression
```

## Comparing `biobb_cmip-3.9.0.tar` & `biobb_cmip-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:54:04.000000 biobb_cmip-3.9.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)       79 2021-12-15 10:26:06.000000 biobb_cmip-3.9.0/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     4058 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     3250 2023-01-17 10:55:55.000000 biobb_cmip-3.9.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip/
--rw-r--r--   0 pau        (501) staff       (20)       61 2023-01-17 10:53:51.000000 biobb_cmip-3.9.0/biobb_cmip/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/
--rwxr-xr-x   0 pau        (501) staff       (20)      100 2022-03-03 09:50:06.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    21589 2023-01-17 09:44:11.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/cmip.py
--rw-r--r--   0 pau        (501) staff       (20)    25741 2022-11-09 12:41:12.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/common.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/dat/
--rw-r--r--   0 pau        (501) staff       (20)    32705 2021-07-09 14:56:42.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/dat/aa.lib
--rw-r--r--   0 pau        (501) staff       (20)    24096 2021-07-09 14:56:42.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/dat/nuc.lib
--rw-r--r--   0 pau        (501) staff       (20)      766 2021-07-09 14:56:42.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/dat/solv.vdwprm
--rw-r--r--   0 pau        (501) staff       (20)      611 2021-07-09 14:56:42.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/dat/vdwprm
--rw-r--r--   0 pau        (501) staff       (20)     6323 2023-01-17 09:56:44.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/ignore_residues.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6373 2023-01-17 09:56:44.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/prepare_pdb.py
--rw-r--r--   0 pau        (501) staff       (20)     7704 2023-01-17 09:56:44.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/prepare_structure.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10592 2023-01-17 09:56:44.000000 biobb_cmip-3.9.0/biobb_cmip/cmip/titration.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:54:04.000000 biobb_cmip-3.9.0/biobb_cmip/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip/utils/
--rw-r--r--   0 pau        (501) staff       (20)        0 2022-03-03 21:09:25.000000 biobb_cmip-3.9.0/biobb_cmip/utils/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     6376 2023-01-17 08:46:59.000000 biobb_cmip-3.9.0/biobb_cmip/utils/representation.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     4058 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      683 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      256 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       71 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       11 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/biobb_cmip.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-01-17 10:59:35.000000 biobb_cmip-3.9.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1580 2023-01-17 10:53:20.000000 biobb_cmip-3.9.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:54:04.000000 biobb_cmip-4.0.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)       79 2021-12-15 10:26:06.000000 biobb_cmip-4.0.0/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     4207 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     3250 2023-07-20 21:55:15.000000 biobb_cmip-4.0.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip/
+-rw-r--r--   0 pau        (501) staff       (20)       61 2023-07-20 21:53:42.000000 biobb_cmip-4.0.0/biobb_cmip/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/
+-rwxr-xr-x   0 pau        (501) staff       (20)      124 2023-07-20 21:46:21.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     6390 2023-07-20 21:12:41.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_ignore_residues.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6440 2023-07-20 21:13:43.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_prepare_pdb.py
+-rw-r--r--   0 pau        (501) staff       (20)     7692 2023-07-20 20:46:30.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_prepare_structure.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    22086 2023-07-20 11:17:39.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_run.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10649 2023-07-20 20:49:39.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_titration.py
+-rw-r--r--   0 pau        (501) staff       (20)    25741 2022-11-09 12:41:12.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/common.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/dat/
+-rw-r--r--   0 pau        (501) staff       (20)    32705 2021-07-09 14:56:42.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/dat/aa.lib
+-rw-r--r--   0 pau        (501) staff       (20)    24096 2021-07-09 14:56:42.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/dat/nuc.lib
+-rw-r--r--   0 pau        (501) staff       (20)      766 2021-07-09 14:56:42.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/dat/solv.vdwprm
+-rw-r--r--   0 pau        (501) staff       (20)      611 2021-07-09 14:56:42.000000 biobb_cmip-4.0.0/biobb_cmip/cmip/dat/vdwprm
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:54:04.000000 biobb_cmip-4.0.0/biobb_cmip/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip/utils/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2022-03-03 21:09:25.000000 biobb_cmip-4.0.0/biobb_cmip/utils/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     6376 2023-01-17 08:46:59.000000 biobb_cmip-4.0.0/biobb_cmip/utils/representation.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     4207 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      707 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      280 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       71 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       11 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/biobb_cmip.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2023-07-20 22:44:46.000000 biobb_cmip-4.0.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1749 2023-07-20 21:48:46.000000 biobb_cmip-4.0.0/setup.py
```

### Comparing `biobb_cmip-3.9.0/LICENSE` & `biobb_cmip-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/PKG-INFO` & `biobb_cmip-4.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 Metadata-Version: 2.1
 Name: biobb_cmip
-Version: 3.9.0
+Version: 4.0.0
 Summary: biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Home-page: https://github.com/bioexcel/biobb_cmip
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_cmip.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
 [![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip)
-[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v3.9.0 2022.4
+v4.0.0 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=3.9.0"
+        pip install "biobb_cmip>=4.0.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=3.9.0"
+        conda install -c bioconda "biobb_cmip>=4.0.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
```

### Comparing `biobb_cmip-3.9.0/README.md` & `biobb_cmip-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
 [![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip)
-[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v3.9.0 2022.4
+v4.0.0 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=3.9.0"
+        pip install "biobb_cmip>=4.0.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=3.9.0"
+        conda install -c bioconda "biobb_cmip>=4.0.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/cmip.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_cmip.cmip.common import create_params_file
 from biobb_cmip.cmip.common import params_preset
 from biobb_cmip.cmip.common import get_grid
 
 
-class Cmip(BiobbObject):
+class CmipRun(BiobbObject):
     """
     | biobb_cmip Titration
     | Wrapper class for the CMIP cmip module.
     | The CMIP cmip module. CMIP cmip module compute classical molecular interaction potentials.
 
     Args:
         input_pdb_path (str): Path to the input PDB file. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_cmip/master/biobb_cmip/test/data/cmip/1kim_h.pdb>`_. Accepted formats: pdb (edam:format_1476).
@@ -225,23 +225,29 @@
         # manual copy_to_host or unstage
         if self.io_dict['out'].get('output_pdb_path'):
             output_pdb_path = str(Path(self.stage_io_dict["unique_dir"]).joinpath(Path(self.io_dict['out'].get('output_pdb_path')).name))
             if Path(output_pdb_path[:-4]).exists():
                 shutil.move(output_pdb_path[:-4], self.io_dict['out'].get('output_pdb_path'))
             elif Path(output_pdb_path + ".pdb").exists():
                 shutil.move(output_pdb_path + ".pdb", self.io_dict['out'].get('output_pdb_path'))
+            elif not Path(output_pdb_path).exists():
+                fu.log(f"WARNING: File not found output_pdb_path: {output_pdb_path}", self.out_log, self.global_log)
 
         # Replace "ATOMTM" tag for "ATOM  "
+
         output_pdb_path = self.io_dict['out'].get('output_pdb_path')
         if output_pdb_path:
-            with open(output_pdb_path) as pdb_file:
-                list_pdb_lines = pdb_file.readlines()
-            with open(output_pdb_path, 'w') as pdb_file:
-                for line in list_pdb_lines:
-                    pdb_file.write(line.replace('ATOMTM', 'ATOM  '))
+            if Path(output_pdb_path).exists():
+                with open(output_pdb_path) as pdb_file:
+                    list_pdb_lines = pdb_file.readlines()
+                with open(output_pdb_path, 'w') as pdb_file:
+                    for line in list_pdb_lines:
+                        pdb_file.write(line.replace('ATOMTM', 'ATOM  '))
+            else:
+                fu.log(f"WARNING: File not found output_pdb_path: {output_pdb_path} Abs Path: {Path(output_pdb_path).resolve()}", self.out_log, self.global_log)
 
         # Create json_box_path file from CMIP log file
         if self.io_dict['out'].get('output_json_box_path'):
             origin, size, grid_params = get_grid(self.stage_io_dict["out"]["output_log_path"])
             grid_params['DIM'] = (int(grid_params['DIM'][0]),
                                   int(grid_params['DIM'][1]),
                                   int(grid_params['DIM'][2]))
@@ -283,30 +289,30 @@
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def cmip(input_pdb_path: str, input_probe_pdb_path: str = None, output_pdb_path: str = None,
-         output_grd_path: str = None, output_cube_path: str = None, output_rst_path: str = None,
-         output_byat_path: str = None, output_log_path: str = None,
-         input_vdw_params_path: str = None, input_params_path: str = None, output_json_box_path: str = None,
-         output_json_external_box_path: str = None, input_json_box_path: str = None,
-         input_json_external_box_path: str = None, properties: dict = None, **kwargs) -> int:
+def cmip_run(input_pdb_path: str, input_probe_pdb_path: str = None, output_pdb_path: str = None,
+             output_grd_path: str = None, output_cube_path: str = None, output_rst_path: str = None,
+             output_byat_path: str = None, output_log_path: str = None,
+             input_vdw_params_path: str = None, input_params_path: str = None, output_json_box_path: str = None,
+             output_json_external_box_path: str = None, input_json_box_path: str = None,
+             input_json_external_box_path: str = None, properties: dict = None, **kwargs) -> int:
     """Create :class:`Cmip <cmip.cmip.Cmip>` class and
     execute the :meth:`launch() <cmip.cmip.Cmip.launch>` method."""
 
-    return Cmip(input_pdb_path=input_pdb_path, input_probe_pdb_path=input_probe_pdb_path,
-                output_pdb_path=output_pdb_path, output_grd_path=output_grd_path, output_cube_path=output_cube_path,
-                output_rst_path=output_rst_path, output_byat_path=output_byat_path, output_log_path=output_log_path,
-                input_vdw_params_path=input_vdw_params_path, input_params_path=input_params_path,
-                output_json_box_path=output_json_box_path, output_json_external_box_path=output_json_external_box_path,
-                input_json_box_path=input_json_box_path, input_json_external_box_path=input_json_external_box_path,
-                properties=properties, **kwargs).launch()
+    return CmipRun(input_pdb_path=input_pdb_path, input_probe_pdb_path=input_probe_pdb_path,
+                   output_pdb_path=output_pdb_path, output_grd_path=output_grd_path, output_cube_path=output_cube_path,
+                   output_rst_path=output_rst_path, output_byat_path=output_byat_path, output_log_path=output_log_path,
+                   input_vdw_params_path=input_vdw_params_path, input_params_path=input_params_path,
+                   output_json_box_path=output_json_box_path, output_json_external_box_path=output_json_external_box_path,
+                   input_json_box_path=input_json_box_path, input_json_external_box_path=input_json_external_box_path,
+                   properties=properties, **kwargs).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Wrapper of the CMIP cmip module.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
@@ -328,19 +334,19 @@
     parser.add_argument('--input_json_external_box_path', required=False)
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    cmip(input_pdb_path=args.input_pdb_path, input_probe_pdb_path=args.input_probe_pdb_path,
-         output_pdb_path=args.output_pdb_path, output_grd_path=args.output_grd_path,
-         output_cube_path=args.output_cube_path, output_rst_path=args.output_rst_path,
-         output_byat_path=args.output_byat_path, output_log_path=args.output_log_path,
-         input_vdw_params_path=args.input_vdw_params_path, input_params_path=args.input_params_path,
-         output_json_box_path=args.output_json_box_path,
-         output_json_external_box_path=args.output_json_external_box_path, input_json_box_path=args.input_json_box_path,
-         input_json_external_box_path=args.input_json_external_box_path, properties=properties)
+    cmip_run(input_pdb_path=args.input_pdb_path, input_probe_pdb_path=args.input_probe_pdb_path,
+             output_pdb_path=args.output_pdb_path, output_grd_path=args.output_grd_path,
+             output_cube_path=args.output_cube_path, output_rst_path=args.output_rst_path,
+             output_byat_path=args.output_byat_path, output_log_path=args.output_log_path,
+             input_vdw_params_path=args.input_vdw_params_path, input_params_path=args.input_params_path,
+             output_json_box_path=args.output_json_box_path,
+             output_json_external_box_path=args.output_json_external_box_path, input_json_box_path=args.input_json_box_path,
+             input_json_external_box_path=args.input_json_external_box_path, properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/common.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/common.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/dat/aa.lib` & `biobb_cmip-4.0.0/biobb_cmip/cmip/dat/aa.lib`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/dat/nuc.lib` & `biobb_cmip-4.0.0/biobb_cmip/cmip/dat/nuc.lib`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/dat/solv.vdwprm` & `biobb_cmip-4.0.0/biobb_cmip/cmip/dat/solv.vdwprm`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/dat/vdwprm` & `biobb_cmip-4.0.0/biobb_cmip/cmip/dat/vdwprm`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/ignore_residues.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_ignore_residues.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from biobb_cmip.cmip.common import mark_residues
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 import biobb_common.tools.file_utils as fu
 
 
-class IgnoreResidues(BiobbObject):
+class CmipIgnoreResidues(BiobbObject):
     """
-    | biobb_cmip IgnoreResidues
+    | biobb_cmip CmipIgnoreResidues
     | Class to ignore residues in CMIP potential calculations.
     | Mark residues which will be ignored in the CMIP potential calculations except for dielectric definition.
 
     Args:
         input_cmip_pdb_path (str): Input PDB file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/data/cmip/input_ignore_res.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_cmip_pdb_path (str): Output PDB file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/ignore_res_gln3.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
@@ -25,17 +25,17 @@
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_cmip.cmip.ignore_residues import ignore_residues
+            from biobb_cmip.cmip.cmip_ignore_residues import cmip_ignore_residues
             prop = { 'residue_list': "A:3" }
-            ignore_residues(input_cmip_pdb_path='/path/to/myStructure.pdb',
+            cmip_ignore_residues(input_cmip_pdb_path='/path/to/myStructure.pdb',
                             output_cmip_pdb_path='/path/to/newStructure.pdb',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: CMIP cmip
             * version: 2.7.0
@@ -67,15 +67,16 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`IgnoreResidues <cmip.ignore_residues.IgnoreResidues>` object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
 
         if not self.ignore_all and not self.residue_list:
             fu.log(f"Residue_list is empty and ignore_all is false nothing will be done.", self.out_log, self.global_log)
             shutil.copyfile(self.io_dict["in"]["input_cmip_pdb_path"], self.io_dict["out"]["output_cmip_pdb_path"])
             return self.return_code
 
         if self.ignore_all:
@@ -99,20 +100,20 @@
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def ignore_residues(input_cmip_pdb_path: str, output_cmip_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def cmip_ignore_residues(input_cmip_pdb_path: str, output_cmip_pdb_path: str, properties: dict = None, **kwargs) -> int:
     """Create :class:`IgnoreResidues <cmip.ignore_residues.IgnoreResidues>` class and
     execute the :meth:`launch() <cmip.ignore_residues.IgnoreResidues.launch>` method."""
-    return IgnoreResidues(input_cmip_pdb_path=input_cmip_pdb_path,
-                          output_cmip_pdb_path=output_cmip_pdb_path,
-                          properties=properties, **kwargs).launch()
+    return CmipIgnoreResidues(input_cmip_pdb_path=input_cmip_pdb_path,
+                              output_cmip_pdb_path=output_cmip_pdb_path,
+                              properties=properties, **kwargs).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Mark residues which charges will be ignored in the CMIP potential calculations.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
@@ -122,14 +123,14 @@
     required_args.add_argument('-o', '--output_cmip_pdb_path', required=True, help="Output PDB file name")
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    ignore_residues(input_cmip_pdb_path=args.input_cmip_pdb_path,
-                    output_cmip_pdb_path=args.output_cmip_pdb_path,
-                    properties=properties)
+    cmip_ignore_residues(input_cmip_pdb_path=args.input_cmip_pdb_path,
+                         output_cmip_pdb_path=args.output_cmip_pdb_path,
+                         properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/prepare_pdb.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_prepare_pdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """Module containing the PreparePDB class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
-class PreparePDB(BiobbObject):
+class CmipPreparePDB(BiobbObject):
     """
-    | biobb_cmip PreparePDB
+    | biobb_cmip CmipPreparePDB
     | Class to add CMIP charges and atom types.
     | Add CMIP charges and atom types to a PDB structure using `biobb_structure_checking <https://anaconda.org/bioconda/biobb_structure_checking>`_.
 
     Args:
         input_pdb_path (str): Input PDB file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/data/cmip/1aki.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_cmip_pdb_path (str): Output PDB file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/egfr_cmip.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
@@ -25,17 +25,17 @@
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_cmip.cmip.prepare_pdb import prepare_pdb
+            from biobb_cmip.cmip.cmip_prepare_pdb import cmip_prepare_pdb
             prop = { 'restart': False }
-            prepare_pdb(input_pdb_path='/path/to/myStructure.pdb',
+            cmip_prepare_pdb(input_pdb_path='/path/to/myStructure.pdb',
                         output_cmip_pdb_path='/path/to/newStructure.pdb',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: CMIP cmip
             * version: 2.7.0
@@ -70,15 +70,16 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`PreparePDB <cmip.prepare_pdb.PreparePDB>` object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         command_list = ""
         if self.remove_water:
             command_list += 'water --remove yes; '
 
         if self.fix_backbone_atoms:
@@ -112,20 +113,20 @@
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def prepare_pdb(input_pdb_path: str, output_cmip_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def cmip_prepare_pdb(input_pdb_path: str, output_cmip_pdb_path: str, properties: dict = None, **kwargs) -> int:
     """Create :class:`PreparePDB <cmip.prepare_pdb.PreparePDB>` class and
     execute the :meth:`launch() <cmip.prepare_pdb.PreparePDB.launch>` method."""
-    return PreparePDB(input_pdb_path=input_pdb_path,
-                      output_cmip_pdb_path=output_cmip_pdb_path,
-                      properties=properties, **kwargs).launch()
+    return CmipPreparePDB(input_pdb_path=input_pdb_path,
+                          output_cmip_pdb_path=output_cmip_pdb_path,
+                          properties=properties, **kwargs).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Model the missing atoms in the backbone of a PDB structure.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
@@ -135,14 +136,14 @@
     required_args.add_argument('-o', '--output_cmip_pdb_path', required=True, help="Output PDB file name")
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    prepare_pdb(input_pdb_path=args.input_pdb_path,
-                output_cmip_pdb_path=args.output_cmip_pdb_path,
-                properties=properties)
+    cmip_prepare_pdb(input_pdb_path=args.input_pdb_path,
+                     output_cmip_pdb_path=args.output_cmip_pdb_path,
+                     properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/prepare_structure.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_prepare_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #!/usr/bin/env python3
 
 """Module containing the PrepareStructure class and the command line interface."""
-import os
 import argparse
 import warnings
-import shutil
 from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_common.command_wrapper import cmd_wrapper
+
 # Write the CMIP PDB
 from biobb_cmip.cmip.common import write_cmip_pdb
 # Dani's methods using a topology and a PDB file
 from biobb_cmip.cmip.common import get_topology_cmip_elements_canonical
 from biobb_cmip.cmip.common import get_topology_charges
 # JLG methods using just the PDB file
 from biobb_cmip.cmip.common import get_pdb_charges
 from biobb_cmip.cmip.common import get_pdb_cmip_elements_canonical
 
 
-class PrepareStructure(BiobbObject):
+class CmipPrepareStructure(BiobbObject):
     """
     | biobb_cmip PrepareStructure
     | Generate a CMIP suitable PDB input.
     | Generate a CMIP suitable PDB input from a common PDB file or a Topology + PDB file.
 
     Args:
         input_pdb_path (str): Path to the input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/data/cmip/egfr.pdb>`_. Accepted formats: pdb (edam:format_1476).
@@ -78,23 +76,25 @@
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Cmip <cmip.cmip.PrepareStructure>` object."""
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
 
         # Dani's method
         if self.io_dict['in']['input_topology_path']:
             top_file = self.io_dict['in']['input_topology_path']
             if self.io_dict['in']['input_topology_path'].lower().endswith(".zip"):
                 # Unzip topology to topology_out
                 top_file = fu.unzip_top(zip_file=self.io_dict['in']['input_topology_path'], out_log=self.out_log)
                 top_dir = str(Path(top_file).parent)
+                self.tmp_files.append(top_dir)
 
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", category=UserWarning)
                 fu.log(f'Reading: {top_file} to extract charges', self.out_log, self.global_log)
                 charges_list = get_topology_charges(top_file)
                 fu.log(f'Reading: {top_file} to extract elements', self.out_log, self.global_log)
                 elements_list = get_topology_cmip_elements_canonical(top_file)
@@ -110,30 +110,29 @@
                        self.io_dict['out']['output_cmip_pdb_path'],
                        charges_list,
                        elements_list)
 
         ###################################
 
         # remove temporary folder(s)
-        self.tmp_files.extend([top_dir])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return 0
 
 
-def prepare_structure(input_pdb_path: str, output_cmip_pdb_path: str, input_topology_path: str = None,
-                      properties: dict = None, **kwargs) -> int:
+def cmip_prepare_structure(input_pdb_path: str, output_cmip_pdb_path: str, input_topology_path: str = None,
+                           properties: dict = None, **kwargs) -> int:
     """Create :class:`Cmip <cmip.cmip.PrepareStructure>` class and
     execute the :meth:`launch() <cmip.cmip.PrepareStructure.launch>` method."""
 
-    return PrepareStructure(input_pdb_path=input_pdb_path, output_cmip_pdb_path=output_cmip_pdb_path,
-                            input_topology_path=input_topology_path, properties=properties,
-                            **kwargs).launch()
+    return CmipPrepareStructure(input_pdb_path=input_pdb_path, output_cmip_pdb_path=output_cmip_pdb_path,
+                                input_topology_path=input_topology_path, properties=properties,
+                                **kwargs).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Wrapper of the cmip prepare_structure module.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
@@ -144,15 +143,15 @@
     parser.add_argument('--input_topology_path', required=False)
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    prepare_structure(input_pdb_path=args.input_pdb_path,
-                      output_cmip_pdb_path=args.output_cmip_pdb_path,
-                      input_topology_path=args.input_topology_path,
-                      properties=properties)
+    cmip_prepare_structure(input_pdb_path=args.input_pdb_path,
+                           output_cmip_pdb_path=args.output_cmip_pdb_path,
+                           input_topology_path=args.input_topology_path,
+                           properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/cmip/titration.py` & `biobb_cmip-4.0.0/biobb_cmip/cmip/cmip_titration.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from biobb_common.tools.file_utils import launchlogger
 from biobb_common.command_wrapper import cmd_wrapper
 from biobb_cmip.cmip.common import create_params_file
 from biobb_cmip.cmip.common import params_preset
 from biobb_cmip.cmip.common import get_pdb_total_charge
 
 
-class Titration(BiobbObject):
+class CmipTitration(BiobbObject):
     """
     | biobb_cmip Titration
     | Wrapper class for the CMIP titration module.
     | The CMIP titration module. CMIP titration module adds water molecules, positive ions (Na+) and negative ions (Cl-) in the energetically most favorable structure locations.
 
     Args:
         input_pdb_path (str): Path to the input PDB file. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_cmip/master/biobb_cmip/test/data/cmip/1kim_h.pdb>`_. Accepted formats: pdb (edam:format_1476).
@@ -95,16 +95,16 @@
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Titration <cmip.titration.Titration>` object."""
         # Setup Biobb
-        if self.check_restart(): return 0
-
+        if self.check_restart():
+            return 0
 
         # Check if output_pdb_path ends with ".pdb"
         if not self.io_dict['out']['output_pdb_path'].endswith('.pdb'):
             fu.log('ERROR: output_pdb_path name must end in .pdb', self.out_log, self.global_log)
             raise ValueError("ERROR: output_pdb_path name must end in .pdb")
 
         # Adding neutral, num_negative_ions, num_positive_ions, num_wats, cutoff
@@ -158,23 +158,23 @@
         self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), combined_params_dir])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def titration(input_pdb_path: str, output_pdb_path: str,
-              input_vdw_params_path: str = None, input_params_path: str = None,
-              properties: dict = None, **kwargs) -> int:
+def cmip_titration(input_pdb_path: str, output_pdb_path: str,
+                   input_vdw_params_path: str = None, input_params_path: str = None,
+                   properties: dict = None, **kwargs) -> int:
     """Create :class:`Titration <cmip.titration.Titration>` class and
     execute the :meth:`launch() <cmip.titration.Titration.launch>` method."""
 
-    return Titration(input_pdb_path=input_pdb_path, output_pdb_path=output_pdb_path,
-                     input_vdw_params_path=input_vdw_params_path, input_params_path=input_params_path,
-                     properties=properties, **kwargs).launch()
+    return CmipTitration(input_pdb_path=input_pdb_path, output_pdb_path=output_pdb_path,
+                         input_vdw_params_path=input_vdw_params_path, input_params_path=input_params_path,
+                         properties=properties, **kwargs).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description="Wrapper of the CMIP Titration module.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
@@ -186,14 +186,14 @@
     parser.add_argument('--input_params_path', required=False)
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    titration(input_pdb_path=args.input_pdb_path, output_pdb_path=args.output_pdb_path,
-              input_vdw_params_path=args.input_vdw_params_path, input_params_path=args.input_params_path,
-              properties=properties)
+    cmip_titration(input_pdb_path=args.input_pdb_path, output_pdb_path=args.output_pdb_path,
+                   input_vdw_params_path=args.input_vdw_params_path, input_params_path=args.input_params_path,
+                   properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip/utils/representation.py` & `biobb_cmip-4.0.0/biobb_cmip/utils/representation.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-3.9.0/biobb_cmip.egg-info/PKG-INFO` & `biobb_cmip-4.0.0/biobb_cmip.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 Metadata-Version: 2.1
 Name: biobb-cmip
-Version: 3.9.0
+Version: 4.0.0
 Summary: biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Home-page: https://github.com/bioexcel/biobb_cmip
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_cmip.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
 [![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip)
-[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v3.9.0 2022.4
+v4.0.0 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=3.9.0"
+        pip install "biobb_cmip>=4.0.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=3.9.0"
+        conda install -c bioconda "biobb_cmip>=4.0.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:3.9.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.0.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:3.9.0--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
```

### Comparing `biobb_cmip-3.9.0/biobb_cmip.egg-info/SOURCES.txt` & `biobb_cmip-4.0.0/biobb_cmip.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 biobb_cmip.egg-info/PKG-INFO
 biobb_cmip.egg-info/SOURCES.txt
 biobb_cmip.egg-info/dependency_links.txt
 biobb_cmip.egg-info/entry_points.txt
 biobb_cmip.egg-info/requires.txt
 biobb_cmip.egg-info/top_level.txt
 biobb_cmip/cmip/__init__.py
-biobb_cmip/cmip/cmip.py
+biobb_cmip/cmip/cmip_ignore_residues.py
+biobb_cmip/cmip/cmip_prepare_pdb.py
+biobb_cmip/cmip/cmip_prepare_structure.py
+biobb_cmip/cmip/cmip_run.py
+biobb_cmip/cmip/cmip_titration.py
 biobb_cmip/cmip/common.py
-biobb_cmip/cmip/ignore_residues.py
-biobb_cmip/cmip/prepare_pdb.py
-biobb_cmip/cmip/prepare_structure.py
-biobb_cmip/cmip/titration.py
 biobb_cmip/cmip/dat/aa.lib
 biobb_cmip/cmip/dat/nuc.lib
 biobb_cmip/cmip/dat/solv.vdwprm
 biobb_cmip/cmip/dat/vdwprm
 biobb_cmip/test/__init__.py
 biobb_cmip/utils/__init__.py
 biobb_cmip/utils/representation.py
```

### Comparing `biobb_cmip-3.9.0/setup.py` & `biobb_cmip-4.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_cmip",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_cmip",
     project_urls={
         "Documentation": "http://biobb_cmip.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     include_package_data=True,
     install_requires=[
-        'biobb_common==3.9.0',
-        'mdanalysis==2.0.0',
-        'biobb_structure_checking==3.12.1'
+        'biobb_common==4.0.0',
+        'mdanalysis>=2.0.0',
+        'biobb_structure_checking==3.13.0'
     ],
     python_requires='>=3.7',
     entry_points={
         "console_scripts": [
-            "cmip = biobb_cmip.cmip.cmip:main",
-            "titration = biobb_cmip.cmip.titration:main",
-            "prepare_structure = biobb_cmip.cmip.prepare_structure:main",
-            "prepare_pdb = biobb_cmip.cmip.prepare_pdb:main",
-            "ignore_residues = biobb_cmip.cmip.ignore_residues:main"
+            "cmip_run = biobb_cmip.cmip.cmip:main",
+            "cmip_titration = biobb_cmip.cmip.titration:main",
+            "cmip_prepare_structure = biobb_cmip.cmip.prepare_structure:main",
+            "cmip_prepare_pdb = biobb_cmip.cmip.prepare_pdb:main",
+            "cmip_ignore_residues = biobb_cmip.cmip.ignore_residues:main"
         ]
     },
-    classifiers=[
-        "Development Status :: 3 - Alpha",
+    classifiers=(
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
-    ],
+        "Operating System :: Unix"
+    ),
 )
```

