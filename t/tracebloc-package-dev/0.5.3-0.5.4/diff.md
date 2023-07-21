# Comparing `tmp/tracebloc_package-dev-0.5.3.tar.gz` & `tmp/tracebloc_package-dev-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.3.tar", last modified: Thu Jul 13 07:56:19 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.4.tar", last modified: Fri Jul 21 14:53:11 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.3.tar` & `tracebloc_package-dev-0.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.517095 tracebloc_package-dev-0.5.3/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.3/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-07-13 07:56:19.517203 tracebloc_package-dev-0.5.3/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.3/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-07-13 07:56:19.517907 tracebloc_package-dev-0.5.3/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-07-13 07:56:12.000000 tracebloc_package-dev-0.5.3/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.515689 tracebloc_package-dev-0.5.3/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.3/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.3/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    24334 2023-07-04 07:32:00.000000 tracebloc_package-dev-0.5.3/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    59195 2023-07-13 07:56:12.000000 tracebloc_package-dev-0.5.3/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.5.3/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10936 2023-06-23 11:15:51.000000 tracebloc_package-dev-0.5.3/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.3/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     6712 2023-06-23 11:15:51.000000 tracebloc_package-dev-0.5.3/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.3/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.516931 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.395840 tracebloc_package-dev-0.5.4/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.4/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-21 14:53:11.395934 tracebloc_package-dev-0.5.4/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.4/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-07-21 14:53:11.396320 tracebloc_package-dev-0.5.4/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-07-21 14:48:57.000000 tracebloc_package-dev-0.5.4/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.394341 tracebloc_package-dev-0.5.4/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.4/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.4/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    26592 2023-07-21 14:48:29.000000 tracebloc_package-dev-0.5.4/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    58421 2023-07-19 08:56:18.000000 tracebloc_package-dev-0.5.4/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.4/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    11021 2023-07-21 14:48:30.000000 tracebloc_package-dev-0.5.4/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.4/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     6857 2023-07-21 14:48:30.000000 tracebloc_package-dev-0.5.4/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.4/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.395642 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.3/LICENSE.txt` & `tracebloc_package-dev-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.3/PKG-INFO` & `tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: tracebloc_package-dev
-Version: 0.5.3
+Name: tracebloc-package-dev
+Version: 0.5.4
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
+
```

### Comparing `tracebloc_package-dev-0.5.3/setup.py` & `tracebloc_package-dev-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.3",
+    version="0.5.4",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/functional_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -365,22 +365,25 @@
             {
                 "model",
                 "model_name",
                 "message",
                 "progress_bar",
                 "image_size",
                 "batch_size",
+                "tmp_path",
             },
         )
         self.message = kwargs["message"]
         self.model = kwargs["model"]
         self.model_name = kwargs["model_name"]
         self.progress_bar = kwargs["progress_bar"]
         self.image_size = kwargs["image_size"]
         self.batch_size = kwargs["batch_size"]
+        self.tmp_path = kwargs["tmp_path"]
+        self.average_weights_file_path = None
 
     def progress_bar_update(self):
         if self.progress_bar is not None:
             self.progress_bar.update(1)
 
     def is_model_supported(self):
         """
@@ -420,14 +423,21 @@
             else:
                 loss = tf.keras.losses.CategoricalCrossentropy()
             self.model.compile(
                 optimizer=tf.keras.optimizers.Adam(),
                 loss=loss,
             )
             self.model.fit(training_dataset, epochs=1, verbose=0)
+            # dump weights from trained model will be used in averaging check
+            get_model_parameters(
+                model=self.model,
+                weight_file_path=self.tmp_path,
+                weights_file_name=TRAINED_WEIGHTS_FILENAME,
+                framework=TENSORFLOW_FRAMEWORK,
+            )
             self.progress_bar_update()
         except Exception as e:  # pragma: no cover
             self.message = (
                 "\nModel not support training on image classification dataset."
             )
             raise
 
@@ -439,20 +449,73 @@
         if model_channel.input_shape[3] != 3:
             self.message = (
                 "\nPlease provide model input shape with 3 channels"  # pragma: no cover
             )
             raise Exception("invalid input shape")  # pragma: no cover
         self.progress_bar_update()
 
+    def average_weights(self):
+        weights = []
+        new_weights = []
+        no_images_array = [20, 20]
+        weights_file_path_1 = os.path.join(
+            self.tmp_path, f"{UNTRAINED_WEIGHTS_FILENAME}.pkl"
+        )
+        weights_file_path_2 = os.path.join(
+            self.tmp_path, f"{TRAINED_WEIGHTS_FILENAME}.pkl"
+        )
+        self.average_weights_file_path = os.path.join(
+            self.tmp_path, f"{AVERAGED_WEIGHTS_PATH}.pkl"
+        )
+        try:
+            with open(weights_file_path_1, "rb") as pkl_file, open(
+                weights_file_path_2, "rb"
+            ) as pkl_file2:
+                weights.append(pickle.load(pkl_file))
+                weights.append(pickle.load(pkl_file2))
+        except Exception as e:
+            raise
+        try:
+            new_weights = [
+                np.array(
+                    [
+                        np.average(np.array(w), weights=no_images_array, axis=0)
+                        for w in zip(*weights_list_tuple)
+                    ]
+                )
+                for weights_list_tuple in zip(*weights)
+            ]
+            del weights
+            del no_images_array
+        except Exception as e:
+            raise
+        try:
+            with open(self.average_weights_file_path, "wb") as f:
+                pickle.dump(new_weights, f)
+            del new_weights
+        except Exception as e:
+            raise
+
+    def load_averaged_weights(self):
+        try:
+            with open(self.average_weights_file_path, "rb") as f:
+                parameters = pickle.load(f)
+            self.model.set_weights(parameters)
+            del parameters
+        except Exception as e:
+            raise
+
     def is_model_eligible(self):
         try:
             self.is_model_supported()
             self.check_original_model_channels()
             self.layer_instance_check()
             self.small_training_loop()
+            self.average_weights()
+            self.load_averaged_weights()
             self.message = "all check passed"
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel checks failed with error as {e}"
             return False, self.message
         return True, self.message
 
     def model_func_checks(self):
@@ -536,14 +599,15 @@
                     # print statistics
                     running_loss += loss.item()
             # dump weights from trained model will be used in averaging check
             get_model_parameters(
                 model=self.model,
                 weight_file_path=self.tmp_path,
                 weights_file_name=TRAINED_WEIGHTS_FILENAME,
+                framework=PYTORCH_FRAMEWORK,
             )
             self.progress_bar.update(1)
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel not support training on image classification dataset as there is error {e} "
             raise
 
     def average_weights(self):
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,104 +715,90 @@
             self.__not_supported_parameters("layersFreeze")
 
     def terminateOnNaNCallback(self):
         """
         Callback that terminates training when a NaN loss is encountered.
         example: trainingObject.terminateOnNaNCallback()
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            c = [""]
-            self.__terminateOnNaNCallback["terminateOnNaN"] = c
-        else:
-            self.__not_supported_parameters("terminateOnNaNCallback")
+        c = [""]
+        self.__terminateOnNaNCallback["terminateOnNaN"] = c
 
     def modelCheckpointCallback(self, monitor: str, save_best_only: bool):
         """
         Callback to save the model weights. parameters: monitor: Quantity to be monitored, save_best_only:  if
         save_best_only=True, it only saves when the model is considered the "best" and the latest best model
         according to the quantity monitored will not be overwritten. example: trainingObject.modelCheckpointCallback(
         'val_loss', True)
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-            try:
-                f.index(monitor.lower())
-                if type(save_best_only) == bool:
-                    c = [monitor, save_best_only]
-                    self.__modelCheckpointCallback["modelCheckpoint"] = c
-                    self.__remove_error_method()
-                else:
-                    error_msg = (
-                        "Invalid datatype for arguments given for save_best_only\n"
-                    )
-                    self.__print_error(error_msg)
-            except:
-                error_msg = f"Please provide supported monitor values: {f}\n"
+        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+        try:
+            f.index(monitor.lower())
+            if type(save_best_only) == bool:
+                c = [monitor, save_best_only]
+                self.__modelCheckpointCallback["modelCheckpoint"] = c
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid datatype for arguments given for save_best_only\n"
                 self.__print_error(error_msg)
-        else:
-            self.__not_supported_parameters("modelCheckpointCallback")
+        except:
+            error_msg = f"Please provide supported monitor values: {f}\n"
+            self.__print_error(error_msg)
 
     def earlystopCallback(self, monitor: str, patience: int):
         """
         Stop training when a monitored metric has stopped improving.
         parameters: monitor: Quantity to be monitored,
                                 patience: Number of epochs with no improvement after which training will be stopped.
         example: trainingObject.earlystopCallback('loss', 10)
 
 
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-            try:
-                f.index(monitor.lower())
-                if type(patience) == int:
-                    c = [monitor, patience]
-                    self.__earlystopCallback["earlystopping"] = c
-                    self.__remove_error_method()
-                else:
-                    error_msg = "Invalid datatype for arguments given for patience\n"
-                    self.__print_error(error_msg)
-            except:
-                error_msg = f"Please provide supported monitor values: {f}\n"
+        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+        try:
+            f.index(monitor.lower())
+            if type(patience) == int:
+                c = [monitor, patience]
+                self.__earlystopCallback["earlystopping"] = c
+                self.__remove_error_method()
+            else:
+                error_msg = "Invalid datatype for arguments given for patience\n"
                 self.__print_error(error_msg)
-        else:
-            self.__not_supported_parameters("earlystopCallback")
+        except:
+            error_msg = f"Please provide supported monitor values: {f}\n"
+            self.__print_error(error_msg)
 
     def reducelrCallback(
         self, monitor: str, factor: float, patience: int, min_delta: float
     ):
         """
         Reduce learning rate when a metric has stopped improving. parameters: monitor: Quantity to be monitored,
         factor: factor by which the learning rate will be reduced. new_lr = lr * factor. patience: number of epochs
         with no improvement after which learning rate will be reduced. min_delta: threshold for measuring the new
         optimum, to only focus on significant changes.
         example: trainingObject.reducelrCallback('loss', 0.1, 10, 0.0001)
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            f = ["accuracy", "loss", "val_loss", "val_accuracy"]
-            try:
-                f.index(monitor.lower())
-                if (
-                    type(factor) == float
-                    and type(patience) == int
-                    and type(min_delta) == float
-                ):
-                    c = [monitor, factor, patience, min_delta]
-                    self.__reducelrCallback["reducelr"] = c
-                    self.__remove_error_method()
-                else:
-                    error_msg = (
-                        "Invalid datatype for arguments given for reducelrCallback\n"
-                    )
-                    self.__print_error(error_msg)
-            except:
-                error_msg = f"Please provide supported monitor values: {f}\n"
+        f = ["accuracy", "loss", "val_loss", "val_accuracy"]
+        try:
+            f.index(monitor.lower())
+            if (
+                type(factor) == float
+                and type(patience) == int
+                and type(min_delta) == float
+            ):
+                c = [monitor, factor, patience, min_delta]
+                self.__reducelrCallback["reducelr"] = c
+                self.__remove_error_method()
+            else:
+                error_msg = (
+                    "Invalid datatype for arguments given for reducelrCallback\n"
+                )
                 self.__print_error(error_msg)
-        else:
-            self.__not_supported_parameters("reducelrCallback")
+        except:
+            error_msg = f"Please provide supported monitor values: {f}\n"
+            self.__print_error(error_msg)
 
     def __setCallbacks(self):
         """
         List of dictionaries.
         List of tensorflow callbacks for training.
         default: []
         """
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,21 +119,22 @@
                 print(text, "\n")
                 self.progress_bar.close()
                 return None
             loaded_model = model_checks_generic.model
             self.__framework = model_checks_generic.framework
             self.__image_size = int(model_checks_generic.image_size)
             self.__batch_size = int(model_checks_generic.batch_size)
+            # dump weights from non-trained model will be used in averaging check
+            get_model_parameters(
+                model=loaded_model,
+                weight_file_path=model_checks_generic.tmp_file_path,
+                weights_file_name=UNTRAINED_WEIGHTS_FILENAME,
+                framework=self.__framework,
+            )
             if self.__framework == PYTORCH_FRAMEWORK:
-                # dump weights from non-trained model will be used in averaging check
-                get_model_parameters(
-                    model=loaded_model,
-                    weight_file_path=model_checks_generic.tmp_file_path,
-                    weights_file_name=UNTRAINED_WEIGHTS_FILENAME,
-                )
                 self.model_check_class = TorchChecks(
                     model=loaded_model,
                     model_name=model_name,
                     message=message,
                     progress_bar=self.progress_bar,
                     image_size=self.__image_size,
                     batch_size=self.__batch_size,
@@ -143,14 +144,15 @@
                 self.model_check_class = TensorflowChecks(
                     model=loaded_model,
                     model_name=model_name,
                     message=message,
                     progress_bar=self.progress_bar,
                     image_size=self.__image_size,
                     batch_size=self.__batch_size,
+                    tmp_path=model_checks_generic.tmp_file_path,
                 )
             (
                 status,
                 message,
                 model_name,
                 progress_bar,
             ) = self.model_check_class.model_func_checks()
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,17 +195,25 @@
         multi_disease_model.add(base_mobilenet_model)
         multi_disease_model.add(GlobalAveragePooling2D())
         multi_disease_model.add(Dropout(0.5))
         multi_disease_model.add(Dense(output_classes, activation="sigmoid"))
         return multi_disease_model
 
 
-def get_model_parameters(model, weight_file_path: str, weights_file_name: str) -> None:
-    parameters = [val.cpu().numpy() for _, val in model.state_dict().items()]
-    with open(os.path.join(weight_file_path, f"{weights_file_name}.pkl"), "wb") as f:
+def get_model_parameters(**kwargs) -> None:
+    if kwargs["framework"] == PYTORCH_FRAMEWORK:
+        parameters = [
+            val.cpu().numpy() for _, val in kwargs["model"].state_dict().items()
+        ]
+    else:
+        parameters = kwargs["model"].get_weights()
+    with open(
+        os.path.join(kwargs["weight_file_path"], f"{kwargs['weights_file_name']}.pkl"),
+        "wb",
+    ) as f:
         pickled = pickle.dumps(parameters)
         optimized_pickle = pickletools.optimize(pickled)
         f.write(optimized_pickle)
     del parameters
 
 
 def validate_kwargs(
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.4/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: tracebloc-package-dev
-Version: 0.5.3
+Name: tracebloc_package-dev
+Version: 0.5.4
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
+
```

### Comparing `tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

