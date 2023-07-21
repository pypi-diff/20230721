# Comparing `tmp/fsrs4anki_optimizer-4.2.1.tar.gz` & `tmp/fsrs4anki_optimizer-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.2.1.tar", last modified: Thu Jul 20 14:40:08 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.3.0.tar", last modified: Fri Jul 21 04:19:01 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.2.1.tar` & `fsrs4anki_optimizer-4.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.442014 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51551 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/setup.py
```

### Comparing `fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,31 +474,18 @@
             tqdm.write("Analysis saved!")
             caption = "1:again, 2:hard, 3:good, 4:easy\n"
             analysis = df[df['r_history'].str.contains(r'^[1-4][^124]*$', regex=True)][['r_history', 'avg_interval', 'avg_retention', 'stability', 'factor', 'group_cnt']].to_string(index=False)
             return caption + analysis
 
     def define_model(self):
         """Step 3"""
-        self.init_w = [1, 2, 3, 4, 5, 0.5, 0.5, 0.2, 1.4, 0.2, 0.8, 2, 0.2, 0.2, 1, 0.5, 2]
+        self.init_w = [0.4, 0.6, 2.4, 5.8, 4.93, 0.94, 0.86, 0.01, 1.49, 0.14, 0.94, 2.18, 0.05, 0.34, 1.26, 0.29, 2.61]
         '''
-        w[0]: initial_stability_for_again_answer
-        w[1]: initial_stability_step_per_rating
-        w[2]: initial_difficulty_for_good_answer
-        w[3]: initial_difficulty_step_per_rating
-        w[4]: next_difficulty_step_per_rating
-        w[5]: next_difficulty_reversion_to_mean_speed (used to avoid ease hell)
-        w[6]: next_stability_factor_after_success
-        w[7]: next_stability_stabilization_decay_after_success
-        w[8]: next_stability_retrievability_gain_after_success
-        w[9]: next_stability_factor_after_failure
-        w[10]: next_stability_difficulty_decay_after_success
-        w[11]: next_stability_stability_gain_after_failure
-        w[12]: next_stability_retrievability_gain_after_failure
-        For more details about the parameters, please see: 
-        https://github.com/open-spaced-repetition/fsrs4anki/wiki/Free-Spaced-Repetition-Scheduler
+        For details about the parameters, please see: 
+        https://github.com/open-spaced-repetition/fsrs4anki/wiki/The-Algorithm
         '''
 
     def pretrain(self, verbose=True):
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         if self.dataset.empty:
             raise ValueError('Training data is inadequate.')
```

