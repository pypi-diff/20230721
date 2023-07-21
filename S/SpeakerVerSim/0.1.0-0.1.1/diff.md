# Comparing `tmp/SpeakerVerSim-0.1.0.tar.gz` & `tmp/SpeakerVerSim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpeakerVerSim-0.1.0.tar", last modified: Thu Jul  6 02:54:45 2023, max compression
+gzip compressed data, was "SpeakerVerSim-0.1.1.tar", last modified: Thu Jul  6 21:45:46 2023, max compression
```

## Comparing `SpeakerVerSim-0.1.0.tar` & `SpeakerVerSim-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 02:54:45.345252 SpeakerVerSim-0.1.0/
--rw-r--r--   0 quan      (1000) quan      (1000)    11339 2023-07-06 02:50:18.000000 SpeakerVerSim-0.1.0/LICENSE
--rw-r--r--   0 quan      (1000) quan      (1000)     4198 2023-07-06 02:54:45.345252 SpeakerVerSim-0.1.0/PKG-INFO
--rw-r--r--   0 quan      (1000) quan      (1000)     3690 2023-07-06 02:40:16.000000 SpeakerVerSim-0.1.0/README.md
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 02:54:45.345252 SpeakerVerSim-0.1.0/SpeakerVerSim/
--rw-r--r--   0 quan      (1000) quan      (1000)     1334 2023-07-04 15:23:03.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/__init__.py
--rw-r--r--   0 quan      (1000) quan      (1000)    13509 2023-07-05 00:51:56.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/common.py
--rw-r--r--   0 quan      (1000) quan      (1000)     6099 2023-07-05 14:07:45.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/server_double.py
--rw-r--r--   0 quan      (1000) quan      (1000)     1730 2023-07-05 14:07:52.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_hash.py
--rw-r--r--   0 quan      (1000) quan      (1000)     2893 2023-07-05 14:07:58.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_multiprofile.py
--rw-r--r--   0 quan      (1000) quan      (1000)     7251 2023-07-05 14:13:22.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_simple.py
--rw-r--r--   0 quan      (1000) quan      (1000)     5522 2023-07-05 22:24:17.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_sync.py
--rw-r--r--   0 quan      (1000) quan      (1000)      990 2023-07-05 14:12:25.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/simulator.py
--rw-r--r--   0 quan      (1000) quan      (1000)     3957 2023-07-06 00:43:55.000000 SpeakerVerSim-0.1.0/SpeakerVerSim/test_simulation.py
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 02:54:45.345252 SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/
--rw-r--r--   0 quan      (1000) quan      (1000)     4198 2023-07-06 02:54:45.000000 SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/PKG-INFO
--rw-r--r--   0 quan      (1000) quan      (1000)      469 2023-07-06 02:54:45.000000 SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/SOURCES.txt
--rw-r--r--   0 quan      (1000) quan      (1000)        1 2023-07-06 02:54:45.000000 SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/dependency_links.txt
--rw-r--r--   0 quan      (1000) quan      (1000)       14 2023-07-06 02:54:45.000000 SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/top_level.txt
--rw-r--r--   0 quan      (1000) quan      (1000)       38 2023-07-06 02:54:45.345252 SpeakerVerSim-0.1.0/setup.cfg
--rw-r--r--   0 quan      (1000) quan      (1000)      795 2023-07-06 02:54:08.000000 SpeakerVerSim-0.1.0/setup.py
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 21:45:46.715162 SpeakerVerSim-0.1.1/
+-rw-r--r--   0 quan      (1000) quan      (1000)    11339 2023-07-06 02:50:18.000000 SpeakerVerSim-0.1.1/LICENSE
+-rw-r--r--   0 quan      (1000) quan      (1000)     4936 2023-07-06 21:45:46.715162 SpeakerVerSim-0.1.1/PKG-INFO
+-rw-r--r--   0 quan      (1000) quan      (1000)     4428 2023-07-06 21:44:39.000000 SpeakerVerSim-0.1.1/README.md
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 21:45:46.715162 SpeakerVerSim-0.1.1/SpeakerVerSim/
+-rw-r--r--   0 quan      (1000) quan      (1000)     1334 2023-07-04 15:23:03.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/__init__.py
+-rw-r--r--   0 quan      (1000) quan      (1000)    13640 2023-07-06 21:33:37.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/common.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     6021 2023-07-06 21:33:36.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/server_double.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     1679 2023-07-06 21:28:56.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_hash.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     2842 2023-07-06 21:29:19.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_multiprofile.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     7200 2023-07-06 21:29:03.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_simple.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     5471 2023-07-06 21:28:46.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_sync.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     1365 2023-07-06 21:41:22.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/simulator.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     4255 2023-07-06 21:39:20.000000 SpeakerVerSim-0.1.1/SpeakerVerSim/test_simulation.py
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-06 21:45:46.715162 SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/
+-rw-r--r--   0 quan      (1000) quan      (1000)     4936 2023-07-06 21:45:46.000000 SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/PKG-INFO
+-rw-r--r--   0 quan      (1000) quan      (1000)      469 2023-07-06 21:45:46.000000 SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/SOURCES.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)        1 2023-07-06 21:45:46.000000 SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/dependency_links.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)       14 2023-07-06 21:45:46.000000 SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/top_level.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)       38 2023-07-06 21:45:46.715162 SpeakerVerSim-0.1.1/setup.cfg
+-rw-r--r--   0 quan      (1000) quan      (1000)      795 2023-07-06 21:45:42.000000 SpeakerVerSim-0.1.1/setup.py
```

### Comparing `SpeakerVerSim-0.1.0/LICENSE` & `SpeakerVerSim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SpeakerVerSim-0.1.0/PKG-INFO` & `SpeakerVerSim-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: SpeakerVerSim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulation framework for version control strategies of speaker recognition systems.
 Home-page: https://github.com/wq2012/SpeakerVerSim
 Author: Quan Wang
 Author-email: quanw@google.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml)
+# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml) [![PyPI Version](https://img.shields.io/pypi/v/SpeakerVerSim.svg)](https://pypi.python.org/pypi/SpeakerVerSim) [![Python Versions](https://img.shields.io/pypi/pyversions/SpeakerVerSim.svg)](https://pypi.org/project/SpeakerVerSim) [![Downloads](https://pepy.tech/badge/SpeakerVerSim)](https://pepy.tech/project/SpeakerVerSim)
 
 
 ## Overview
 SpeakerVerSim is an easily-extensible Python-based simulation framework for different version control strategies of speaker recognition systems under different network configurations.
 
 These simulations are used in the paper [Version Control of Speaker Recognition Systems](https://arxiv.org/abs/2007.12069).
 
 ## How to use
 
+### Install
+
+The `SpeakerVerSim` library can be installed with:
+
+```
+pip install SpeakerVerSim
+```
+
 ### Run one simulation
 
 You can easily start a simulation by running:
 
 ```
 python run_simulator.py
 ```
@@ -41,14 +49,27 @@
 
 You can also override the strategy to be simulated from the config file using the `-s` or `--strategy` flag. For example:
 
 ```
 python run_simulator.py -c my_config.yml -s SSO-sync
 ```
 
+### Call the API
+
+The highest level API is the `SpeakerVerSim.simulate` function.
+It takes either the path to the config file or a dictionary of the configurations as its input, and outputs the simulation stats.
+
+Example usage:
+
+```
+import SpeakerVerSim
+
+stats = SpeakerVerSim.simulate("example_config.yml")
+```
+
 ### Reproduce experiments
 
 You can easily reproduce the experiments in our [paper](https://arxiv.org/abs/2007.12069) by running:
 
 ```
 python run_exp.py
 ```
```

### Comparing `SpeakerVerSim-0.1.0/README.md` & `SpeakerVerSim-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml)
+# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml) [![PyPI Version](https://img.shields.io/pypi/v/SpeakerVerSim.svg)](https://pypi.python.org/pypi/SpeakerVerSim) [![Python Versions](https://img.shields.io/pypi/pyversions/SpeakerVerSim.svg)](https://pypi.org/project/SpeakerVerSim) [![Downloads](https://pepy.tech/badge/SpeakerVerSim)](https://pepy.tech/project/SpeakerVerSim)
 
 
 ## Overview
 SpeakerVerSim is an easily-extensible Python-based simulation framework for different version control strategies of speaker recognition systems under different network configurations.
 
 These simulations are used in the paper [Version Control of Speaker Recognition Systems](https://arxiv.org/abs/2007.12069).
 
 ## How to use
 
+### Install
+
+The `SpeakerVerSim` library can be installed with:
+
+```
+pip install SpeakerVerSim
+```
+
 ### Run one simulation
 
 You can easily start a simulation by running:
 
 ```
 python run_simulator.py
 ```
@@ -26,14 +34,27 @@
 
 You can also override the strategy to be simulated from the config file using the `-s` or `--strategy` flag. For example:
 
 ```
 python run_simulator.py -c my_config.yml -s SSO-sync
 ```
 
+### Call the API
+
+The highest level API is the `SpeakerVerSim.simulate` function.
+It takes either the path to the config file or a dictionary of the configurations as its input, and outputs the simulation stats.
+
+Example usage:
+
+```
+import SpeakerVerSim
+
+stats = SpeakerVerSim.simulate("example_config.yml")
+```
+
 ### Reproduce experiments
 
 You can easily reproduce the experiments in our [paper](https://arxiv.org/abs/2007.12069) by running:
 
 ```
 python run_exp.py
 ```
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/__init__.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/__init__.py`

 * *Files identical despite different names*

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/common.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         # Set database.
         self.database = database
 
         # Config.
         self.config = self.client.config
 
         # Set worker model version.
-        self.set_worker_model_version(self.workers)
+        self.set_worker_model_version()
 
         # Build connections.
         self.client.set_frontend(self.frontend)
         self.frontend.set_client(self.client)
         self.frontend.set_workers(self.workers)
         self.frontend.set_database(self.database)
         for worker in self.workers:
@@ -366,16 +366,16 @@
 
         # Add processes.
         self.client.setup()
         self.frontend.setup()
         for worker in self.workers:
             worker.setup()
 
-    def set_worker_model_version(self, workers: list[BaseWorker]):
-        for worker in workers:
+    def set_worker_model_version(self):
+        for worker in self.workers:
             worker.set_model_version(1)
 
     def aggregate_metrics(self) -> GlobalStats:
         """Aggregate metrics, and maybe print."""
         stats = self.client.stats
         stats.total_num_messages = len(stats.final_messages)
         for msg in stats.final_messages:
@@ -395,7 +395,12 @@
             print("Global stats:")
             stats_short = copy.deepcopy(stats)
             stats_short.final_messages = None
             stats_short.workload = None
             print(stats_short)
 
         return stats
+
+    def simulate(self) -> GlobalStats:
+        """Run simulation."""
+        self.env.run(until=self.config["time_to_run"])
+        return self.aggregate_metrics()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/server_double.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/server_double.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 class DoubleVersionNetworkSystem(NetworkSystem):
     """Class for the entire network system.
 
     But each worker has two model versions.
     """
 
-    def set_worker_model_version(self, workers: list[BaseWorker]):
+    def set_worker_model_version(self):
         for worker in self.workers:
             worker.set_model_versions([1, 2])
 
 
 def simulate(config: dict[str, Any]) -> GlobalStats:
     """Run simulation."""
     if config["strategy"] != "SD":
@@ -156,10 +156,8 @@
     database.create(init_versions=[1, 2])
     netsys = DoubleVersionNetworkSystem(
         env,
         client,
         frontend,
         workers,
         database)
-
-    env.run(until=config["time_to_run"])
-    return netsys.aggregate_metrics()
+    return netsys.simulate()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_hash.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_hash.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,10 +39,8 @@
     database.create(init_version=1)
     netsys = NetworkSystem(
         env,
         client,
         frontend,
         workers,
         database)
-
-    env.run(until=config["time_to_run"])
-    return netsys.aggregate_metrics()
+    return netsys.simulate()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_multiprofile.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_multiprofile.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,10 +68,8 @@
     database.create(init_versions=[1])
     netsys = NetworkSystem(
         env,
         client,
         frontend,
         workers,
         database)
-
-    env.run(until=config["time_to_run"])
-    return netsys.aggregate_metrics()
+    return netsys.simulate()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_simple.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,10 +188,8 @@
     database.create(init_version=1)
     netsys = NetworkSystem(
         env,
         client,
         frontend,
         workers,
         database)
-
-    env.run(until=config["time_to_run"])
-    return netsys.aggregate_metrics()
+    return netsys.simulate()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/server_single_sync.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/server_single_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,10 +140,8 @@
     database.create(init_version=1)
     netsys = NetworkSystem(
         env,
         client,
         frontend,
         workers,
         database)
-
-    env.run(until=config["time_to_run"])
-    return netsys.aggregate_metrics()
+    return netsys.simulate()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim/test_simulation.py` & `SpeakerVerSim-0.1.1/SpeakerVerSim/test_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,10 +97,17 @@
         self.assertEqual(stats.forward_bounce_count, 0)
 
     def test_bad_strategy(self):
         self.config["strategy"] = ""
         with self.assertRaises(ValueError):
             simulate(self.config)
 
+    def test_simulator_file_input(self):
+        config_file = "example_config.yml"
+        stats = simulate(config_file)
+        self.assertEqual(len(stats.final_messages), 1080)
+        self.assertGreater(stats.backward_bounce_count, 1)
+        self.assertGreater(stats.forward_bounce_count, 1)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `SpeakerVerSim-0.1.0/SpeakerVerSim.egg-info/PKG-INFO` & `SpeakerVerSim-0.1.1/SpeakerVerSim.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: SpeakerVerSim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulation framework for version control strategies of speaker recognition systems.
 Home-page: https://github.com/wq2012/SpeakerVerSim
 Author: Quan Wang
 Author-email: quanw@google.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml)
+# SpeakerVerSim [![Python application](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml/badge.svg)](https://github.com/wq2012/SpeakerVerSim/actions/workflows/python-app.yml) [![PyPI Version](https://img.shields.io/pypi/v/SpeakerVerSim.svg)](https://pypi.python.org/pypi/SpeakerVerSim) [![Python Versions](https://img.shields.io/pypi/pyversions/SpeakerVerSim.svg)](https://pypi.org/project/SpeakerVerSim) [![Downloads](https://pepy.tech/badge/SpeakerVerSim)](https://pepy.tech/project/SpeakerVerSim)
 
 
 ## Overview
 SpeakerVerSim is an easily-extensible Python-based simulation framework for different version control strategies of speaker recognition systems under different network configurations.
 
 These simulations are used in the paper [Version Control of Speaker Recognition Systems](https://arxiv.org/abs/2007.12069).
 
 ## How to use
 
+### Install
+
+The `SpeakerVerSim` library can be installed with:
+
+```
+pip install SpeakerVerSim
+```
+
 ### Run one simulation
 
 You can easily start a simulation by running:
 
 ```
 python run_simulator.py
 ```
@@ -41,14 +49,27 @@
 
 You can also override the strategy to be simulated from the config file using the `-s` or `--strategy` flag. For example:
 
 ```
 python run_simulator.py -c my_config.yml -s SSO-sync
 ```
 
+### Call the API
+
+The highest level API is the `SpeakerVerSim.simulate` function.
+It takes either the path to the config file or a dictionary of the configurations as its input, and outputs the simulation stats.
+
+Example usage:
+
+```
+import SpeakerVerSim
+
+stats = SpeakerVerSim.simulate("example_config.yml")
+```
+
 ### Reproduce experiments
 
 You can easily reproduce the experiments in our [paper](https://arxiv.org/abs/2007.12069) by running:
 
 ```
 python run_exp.py
 ```
```

### Comparing `SpeakerVerSim-0.1.0/setup.py` & `SpeakerVerSim-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Setup script for the package."""
 
 import setuptools
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 DESCRIPTION = (
     "Simulation framework for version control strategies "
     "of speaker recognition systems.")
 
 with open("README.md", "r") as file_object:
     LONG_DESCRIPTION = file_object.read()
```

