# Comparing `tmp/banditcoot-0.1.7.tar.gz` & `tmp/banditcoot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banditcoot-0.1.7.tar", max compression
+gzip compressed data, was "banditcoot-0.1.8.tar", max compression
```

## Comparing `banditcoot-0.1.7.tar` & `banditcoot-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      703 2023-02-24 03:42:56.784428 banditcoot-0.1.7/README.md
--rw-r--r--   0        0        0      496 2023-07-20 22:44:21.182539 banditcoot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 03:42:56.785625 banditcoot-0.1.7/src/banditcoot/__init__.py
--rw-r--r--   0        0        0      220 2023-07-20 22:43:03.554510 banditcoot-0.1.7/src/banditcoot/algorithms/__init__.py
--rw-r--r--   0        0        0     3466 2023-07-20 22:42:15.415831 banditcoot-0.1.7/src/banditcoot/algorithms/_epsilon_greedy.py
--rw-r--r--   0        0        0     1834 2023-02-24 03:42:56.786032 banditcoot-0.1.7/src/banditcoot/algorithms/_softmax.py
--rw-r--r--   0        0        0       70 2023-07-20 22:43:03.555420 banditcoot-0.1.7/src/banditcoot/arms/__init__.py
--rw-r--r--   0        0        0      299 2023-06-21 17:11:07.648470 banditcoot-0.1.7/src/banditcoot/arms/_bernoulli.py
--rw-r--r--   0        0        0       82 2023-02-24 03:42:56.786425 banditcoot-0.1.7/src/banditcoot/utility/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-03 17:51:34.210403 banditcoot-0.1.7/src/banditcoot/utility/_batch_monte_carlo_sim.py
--rw-r--r--   0        0        0     1514 2023-06-21 17:11:07.648711 banditcoot-0.1.7/src/banditcoot/utility/_monte_carlo_sim.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.7/setup.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      703 2023-02-24 03:42:56.784428 banditcoot-0.1.8/README.md
+-rw-r--r--   0        0        0      496 2023-07-20 23:10:02.033907 banditcoot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-24 03:42:56.785625 banditcoot-0.1.8/src/banditcoot/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-20 22:43:03.554510 banditcoot-0.1.8/src/banditcoot/algorithms/__init__.py
+-rw-r--r--   0        0        0     3636 2023-07-20 23:09:12.542997 banditcoot-0.1.8/src/banditcoot/algorithms/_epsilon_greedy.py
+-rw-r--r--   0        0        0     1834 2023-02-24 03:42:56.786032 banditcoot-0.1.8/src/banditcoot/algorithms/_softmax.py
+-rw-r--r--   0        0        0       70 2023-07-20 22:43:03.555420 banditcoot-0.1.8/src/banditcoot/arms/__init__.py
+-rw-r--r--   0        0        0      299 2023-06-21 17:11:07.648470 banditcoot-0.1.8/src/banditcoot/arms/_bernoulli.py
+-rw-r--r--   0        0        0       82 2023-02-24 03:42:56.786425 banditcoot-0.1.8/src/banditcoot/utility/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-03 17:51:34.210403 banditcoot-0.1.8/src/banditcoot/utility/_batch_monte_carlo_sim.py
+-rw-r--r--   0        0        0     1514 2023-06-21 17:11:07.648711 banditcoot-0.1.8/src/banditcoot/utility/_monte_carlo_sim.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.8/setup.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.8/PKG-INFO
```

### Comparing `banditcoot-0.1.7/README.md` & `banditcoot-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.7/src/banditcoot/algorithms/_epsilon_greedy.py` & `banditcoot-0.1.8/src/banditcoot/algorithms/_epsilon_greedy.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,12 +77,12 @@
         self.conv_rates[chosen_arm] = ((prev_conv_rates[chosen_arm] * prev_counts[chosen_arm]) + num_successes) / self.counts[chosen_arm]
 
         # calculate new average reward for chosen arm
         observed_reward = prev_rewards[chosen_arm] if observed_reward is None else observed_reward
         prev_total_rewards = (prev_rewards[chosen_arm] * prev_conv_rates[chosen_arm] * prev_counts[chosen_arm])
         new_total_rewards  = num_successes * observed_reward
         self.rewards[chosen_arm] = (prev_total_rewards + new_total_rewards) / self.counts[chosen_arm]
-        
+        self.rewards[chosen_arm] = (prev_rewards[chosen_arm] * prev_counts[chosen_arm] / self.counts[chosen_arm]) + (observed_reward * num_times_chosen / self.counts[chosen_arm])
         # calculate new average value for chosen arm
         self.values[chosen_arm] = (self.conv_rates[chosen_arm] * self.counts[chosen_arm] * self.rewards[chosen_arm])/self.counts[chosen_arm]
         return
```

### Comparing `banditcoot-0.1.7/src/banditcoot/algorithms/_softmax.py` & `banditcoot-0.1.8/src/banditcoot/algorithms/_softmax.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.7/src/banditcoot/utility/_batch_monte_carlo_sim.py` & `banditcoot-0.1.8/src/banditcoot/utility/_batch_monte_carlo_sim.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.7/src/banditcoot/utility/_monte_carlo_sim.py` & `banditcoot-0.1.8/src/banditcoot/utility/_monte_carlo_sim.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.7/setup.py` & `banditcoot-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'banditcoot',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Python module for developing and testing multi-armed bandits',
     'long_description': 'Banditcoot\n====================\n\n<img align="left" width="75" src="https://github.com/dan-kwon/banditcoot/blob/master/resources/Banditcoot.png"/> \n\n**banditcoot** is a Python module is intended for my own personal use when developing and testing multi-armed bandit algorithms. Forked from the accompanying [code repository](https://github.com/johnmyleswhite/BanditsBook) for [Bandit Algorithms for Website Optimization](https://www.oreilly.com/library/view/bandit-algorithms-for/9781449341565/).\n\n*Any use of this code is at your own risk.*\n</br>\n\n## Installation\n--------------------\nRecommended method of installation is to use pip \n```\npip install banditcoot\n```\n\n\n## Quickstart\n--------------------\n',
     'author': 'dan-kwon',
     'author_email': 'danielkwon02@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `banditcoot-0.1.7/PKG-INFO` & `banditcoot-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banditcoot
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python module for developing and testing multi-armed bandits
 License: MIT
 Author: dan-kwon
 Author-email: danielkwon02@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

