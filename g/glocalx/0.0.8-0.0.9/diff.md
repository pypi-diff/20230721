# Comparing `tmp/glocalx-0.0.8.tar.gz` & `tmp/glocalx-0.0.9.tar.gz`

## Comparing `glocalx-0.0.8.tar` & `glocalx-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 glocalx-0.0.8/PKG-INFO
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/__init__.py
--rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/api.py
--rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/callbacks.py
--rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/evaluators.py
--rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/generators.py
--rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/glocalx.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/glocax_probabilistic.py
--rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/models.py
--rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/requirements.txt
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/serialization.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_dataset.csv
--rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_model.h5
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/dummy/dummy_rules.json
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/data/loaders/adult_info.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.8/src/glocalx/loaders/lore.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.8/LICENSE
--rwxr-xr-x   0        0        0    11369 2020-02-02 00:00:00.000000 glocalx-0.0.8/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 glocalx-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 glocalx-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 glocalx-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.9/data/dummy/dummy_dataset.csv
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.9/data/dummy/dummy_model.h5
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.9/data/dummy/dummy_rules.json
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.9/data/loaders/adult_info.json
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/__init__.py
+-rwxr-xr-x   0        0        0     9644 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/api.py
+-rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/callbacks.py
+-rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/evaluators.py
+-rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/generators.py
+-rwxr-xr-x   0        0        0    24488 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/glocalx.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/glocax_probabilistic.py
+-rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/models.py
+-rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/requirements.txt
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/serialization.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/data/dummy/dummy_dataset.csv
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/data/dummy/dummy_model.h5
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/data/dummy/dummy_rules.json
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/data/loaders/adult_info.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.9/src/glocalx/loaders/lore.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0    11318 2020-02-02 00:00:00.000000 glocalx-0.0.9/README.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 glocalx-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 glocalx-0.0.9/PKG-INFO
```

### Comparing `glocalx-0.0.8/PKG-INFO` & `glocalx-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glocalx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generating global explanations from local ones.
 Project-URL: Homepage, https://github.com/msetzu/glocalx
 Project-URL: Bug Tracker, https://github.com/msetzu/glocalx/issues
 Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,14 @@
 Requires-Python: <3.11,>=3.8
 Requires-Dist: click
 Requires-Dist: logzero==1.6.2
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: tensorflow==2.8
 Description-Content-Type: text/markdown
 
 # GLocalX - Global through Local Explainability
 
 Explanations come in two forms: local, explaining a single model prediction, and global, explaining all model predictions. The Local to Global (L2G) problem consists in bridging these two family of explanations. Simply put, we generate global explanations by merging local ones.
 
 ## The algorithm
@@ -55,30 +54,29 @@
 
 Installing from pypi does not give direct access to quickstart data, first download the `data/` folder from the [original repository](https://github.com/msetzu/glocalx/tree/main).
 
 ### Python interface
 
 ```python
 from tensorflow.keras.models import load_model
-from numpy import genfromtxt, float as np_float
 import logzero
 
 from glocalx.glocalx import GLocalX, shut_up_tensorflow
 from glocalx.models import Rule
 
 # Set log profile: INFO for normal logging, DEBUG for verbosity
 logzero.loglevel(logzero.logging.INFO)
 shut_up_tensorflow()
 
 # Load black box: optional! Use black_box = None to use the dataset labels
 black_box = load_model('data/dummy/dummy_model.h5')
 # Load data and header
 data = genfromtxt('data/dummy/dummy_dataset.csv', delimiter=',', names=True)
 features_names = data.dtype.names
-tr_set = data.view(np_float).reshape(data.shape + (-1,))
+tr_set = data.view(float).reshape(data.shape + (-1,))
 
 # Load local explanations
 local_explanations = Rule.from_json('data/dummy/dummy_rules.json', names=features_names)
 
 # Create a GLocalX instance for `black_box`
 glocalx = GLocalX(oracle=black_box)
 # Fit the model, use batch_size=128 for larger datasets
```

### Comparing `glocalx-0.0.8/src/glocalx/.gitignore` & `glocalx-0.0.9/src/glocalx/.gitignore`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/api.py` & `glocalx-0.0.9/src/glocalx/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 import pickle
 import json
 
 from .callbacks import print_cb, full_cb, final_rule_dump_cb
 from .glocalx import GLocalX
 from .generators import TrePanGenerator, BudgedExhaustedException
 
-# Shut up, tensorflow!
-os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 import click
 import logzero
 import numpy as np
-from tensorflow.keras.models import load_model as load_tf_model
 
 from logzero import logger
 
 from .models import Rule
 
 
 @click.command()
@@ -157,17 +154,15 @@
         sample_indices_space = range(n)
         sample_size = int(undersample * n)
         sample_indices = np.random.choice(sample_indices_space, (sample_size,))
         rules = [rules[i] for i in sample_indices]
 
     logger.info('Loading oracle...')
     if oracle is not None:
-        if oracle.endswith('.h5'):
-            oracle = load_tf_model(oracle)
-        elif oracle.endswith('.pickle'):
+        if oracle.endswith('.pickle'):
             with open(oracle, 'rb') as log:
                 oracle = pickle.load(log)
         else:
             return
         oracle_predictions = oracle.predict(tr_set[1:, :-1]).round().reshape((tr_set.shape[0] - 1, 1))
         tr_set = np.hstack((tr_set[1:, :-1], oracle_predictions))
```

### Comparing `glocalx-0.0.8/src/glocalx/callbacks.py` & `glocalx-0.0.9/src/glocalx/callbacks.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/evaluators.py` & `glocalx-0.0.9/src/glocalx/evaluators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/generators.py` & `glocalx-0.0.9/src/glocalx/generators.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/glocalx.py` & `glocalx-0.0.9/src/glocalx/glocalx.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 from logzero import logger
 
 from sklearn.model_selection import train_test_split
-import tensorflow as tf
 import numpy as np
 
 from .evaluators import MemEvaluator
 from .callbacks import final_rule_dump_cb as final_rule_dump_callback
 from .models import Rule
 
 
@@ -33,22 +32,14 @@
             x (np.array): The instance(s) to predict
         Returns:
             numpy.array: Array of predictions
         """
         pass
 
 
-def shut_up_tensorflow():
-    """Silences tensorflow warnings."""
-    os.environ["KMP_AFFINITY"] = "noverbose"
-    os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
-    tf.get_logger().setLevel('ERROR')
-    tf.autograph.set_verbosity(3)
-
-
 class GLocalX:
     """
     GLocalX instance. Aggregates local explanations into global ones.
 
     Attributes:
         oracle (Predictor): The black box to explain
         evaluator (MemEvaluator): Evaluator used to evaluate merges and distances
```

### Comparing `glocalx-0.0.8/src/glocalx/glocax_probabilistic.py` & `glocalx-0.0.9/src/glocalx/glocax_probabilistic.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/models.py` & `glocalx-0.0.9/src/glocalx/models.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/requirements.txt` & `glocalx-0.0.9/src/glocalx/requirements.txt`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/serialization.py` & `glocalx-0.0.9/src/glocalx/serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Serialize and deserialize objects and rules."""
 import pickle
 
-from tensorflow.keras.models import load_model as load_tf_model
 import numpy as np
 
 import json
 import os
 
 from .glocalx import GLocalX
 from .models import Rule
@@ -43,17 +42,15 @@
     premises = [{int(k): v for k, v in d.items() if k != 'consequence' and k != 'label'} for d in rules]
     consequences = [dic['consequence'] if 'consequence' in dic else dic['label'] for dic in rules]
     rules = [Rule(premises=premise, consequence=consequence, names=names)
              for premise, consequence in zip(premises, consequences)]
 
     # Load oracle
     oracle = dic['oracle']
-    if oracle.endswith('.h5'):
-        oracle = load_tf_model(oracle)
-    elif oracle.endswith('.pickle'):
+    if oracle.endswith('.pickle'):
         with open(oracle, 'rb') as log:
             oracle = pickle.load(log)
     else:
         return
 
     # Load undersample
     undersample = dic['undersample']
```

### Comparing `glocalx-0.0.8/src/glocalx/data/dummy/dummy_model.h5` & `glocalx-0.0.9/data/dummy/dummy_model.h5`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/data/loaders/adult_info.json` & `glocalx-0.0.9/data/loaders/adult_info.json`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/src/glocalx/loaders/lore.py` & `glocalx-0.0.9/src/glocalx/loaders/lore.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/LICENSE` & `glocalx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.8/README.md` & `glocalx-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,30 +32,29 @@
 
 Installing from pypi does not give direct access to quickstart data, first download the `data/` folder from the [original repository](https://github.com/msetzu/glocalx/tree/main).
 
 ### Python interface
 
 ```python
 from tensorflow.keras.models import load_model
-from numpy import genfromtxt, float as np_float
 import logzero
 
 from glocalx.glocalx import GLocalX, shut_up_tensorflow
 from glocalx.models import Rule
 
 # Set log profile: INFO for normal logging, DEBUG for verbosity
 logzero.loglevel(logzero.logging.INFO)
 shut_up_tensorflow()
 
 # Load black box: optional! Use black_box = None to use the dataset labels
 black_box = load_model('data/dummy/dummy_model.h5')
 # Load data and header
 data = genfromtxt('data/dummy/dummy_dataset.csv', delimiter=',', names=True)
 features_names = data.dtype.names
-tr_set = data.view(np_float).reshape(data.shape + (-1,))
+tr_set = data.view(float).reshape(data.shape + (-1,))
 
 # Load local explanations
 local_explanations = Rule.from_json('data/dummy/dummy_rules.json', names=features_names)
 
 # Create a GLocalX instance for `black_box`
 glocalx = GLocalX(oracle=black_box)
 # Fit the model, use batch_size=128 for larger datasets
```

### Comparing `glocalx-0.0.8/pyproject.toml` & `glocalx-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "glocalx"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Generating global explanations from local ones."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 classifiers = [
@@ -22,14 +22,13 @@
 ]
 dependencies = [
     "click",
     "logzero==1.6.2",
     "numpy",
     "pandas",
     "scikit-learn",
-    "scipy",
-    "tensorflow==2.8",
+    "scipy"
 ]
 
 [project.urls]
 	"Homepage" = "https://github.com/msetzu/glocalx"
 	"Bug Tracker" = "https://github.com/msetzu/glocalx/issues"
```

