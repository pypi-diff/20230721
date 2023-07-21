# Comparing `tmp/perming-1.3.1-py3-none-any.whl.zip` & `tmp/perming-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13221 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-13 03:59 perming/__init__.py
+Zip file size: 13772 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-21 13:32 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    21066 b- defN 23-Jul-13 04:36 perming/_utils.py
+-rw-rw-rw-  2.0 fat    22794 b- defN 23-Jul-21 15:04 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
 -rw-rw-rw-  2.0 fat    13988 b- defN 23-Jul-13 04:45 perming/common.py
--rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 04:43 perming/general.py
--rw-rw-rw-  2.0 fat     8772 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      746 b- defN 23-Jul-13 04:47 perming-1.3.1.dist-info/RECORD
-10 files, 51908 bytes uncompressed, 11967 bytes compressed:  76.9%
+-rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 07:33 perming/general.py
+-rw-rw-rw-  2.0 fat    10926 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      747 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/RECORD
+10 files, 55791 bytes uncompressed, 12518 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.3.1.dist-info/METADATA
+Filename: perming-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.3.1.dist-info/WHEEL
+Filename: perming-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.3.1.dist-info/top_level.txt
+Filename: perming-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.3.1.dist-info/RECORD
+Filename: perming-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -23,8 +23,8 @@
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
     'Multi-outputs': Ranker
 }
 
-__version__ = '1.3.1'
+__version__ = '1.4.0'
```

## perming/_utils.py

```diff
@@ -155,57 +155,66 @@
         :param features: TabularData, composed of n-row samples and m-column features: (n_samples, n_features).
         :param target: TabularData, consists of correct labels or values: (n_samples,) or (n_samples, n_outputs).
         :param ratio_set: Dict[str, int], stores the proportion of train-set, test-set and val-set. default: {'train': 8, 'test': 1, 'val': 1}.
         :param worker_set: Dict[str, int], load the configuration of DataLoader with multi-threaded. default: {'train': 8, 'test': 2, 'val': 1}.
         :param random_seed: int | None, random.seed(random_seed) used for fixed random datasets. default: None.
         '''
         assert ratio_set['train'] > 0 and ratio_set['test'] > 0 and ratio_set['val'] > 0
-        assert ratio_set['train'] > 4 * ratio_set['test'], "The training set needs to be larger than the test set."
-        assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, "The sum of 3 datasets' ratio needs to be 10."
+        assert ratio_set['train'] > 4 * ratio_set['test'], 'The training set needs to be larger than the test set.'
+        assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, 'The sum of 3 datasets ratio needs to be 10.'
         assert isinstance(features, TabularData) and features.ndim == 2, 'Please ensure features with dimension at (n_samples, n_features).'
-        assert features.shape[1] == self.input, "Please ensure `input_` is equal to `features.shape[1]`."
-        assert isinstance(target, TabularData), "Please ensure target format at numpy.ndarray noted as TabularData."
+        assert features.shape[1] == self.input, 'Please ensure `input_` is equal to `features.shape[1]`.'
+        assert isinstance(target, TabularData), 'Please ensure target format at numpy.ndarray noted as TabularData.'
         target_dtype = str(target.dtype) # __str__
-        is_int_type, is_float_type = "int" in target_dtype, "float" in target_dtype
+        is_int_type, is_float_type = 'int' in target_dtype, 'float' in target_dtype
         self.is_target_2d = isinstance(target[0], TabularData) # judge target is 2d matrix.
         if self.is_target_2d: # (n_samples, n_outputs)
-            assert target.shape[1] == self.num_classes, "Please ensure target with (n_samples, n_outputs=num_classes)."
-            assert is_int_type or is_float_type, "Please ensure target.dtype in any int or float type of numpy.dtype."
+            assert target.shape[1] == self.num_classes, 'Please ensure target with (n_samples, n_outputs=num_classes).'
+            assert is_int_type or is_float_type, 'Please ensure target.dtype in any int or float type of numpy.dtype.'
             roc: bool = not is_int_type and is_float_type
         else: # (n_samples,)
             if self.num_classes >= 2:
                 self.unique = numpy.unique(target) # int indexes -> any class with single value noted
-                assert len(self.unique) == self.num_classes, "Please ensure `num_classes` is equal to `len(numpy.unique(labels))`."
+                assert len(self.unique) == self.num_classes, 'Please ensure `num_classes` is equal to `len(numpy.unique(labels))`.'
                 self.indices = dict(zip(self.unique, range(self.num_classes))) # original classes -> int indexes
                 target = numpy.array([self.indices[value] for value in target], dtype=numpy.int8) # adjust int8 -> any int dtype
             else:
-                assert is_float_type, "Please ensure target.dtype in any float type of numpy.dtype." # continuous
+                assert is_float_type, 'Please ensure target.dtype in any float type of numpy.dtype.' # continuous
             roc: bool = self.model.squeeze
         train_, test_, val_ = train_test_val_split(features, target, ratio_set, random_seed)
         self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'])
         self.test_loader = torch.utils.data.DataLoader(TabularDataset(test_['features'], test_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['test'])
         self.val_loader = torch.utils.data.DataLoader(TabularDataset(val_['features'], val_['target'], roc), batch_size=self.batch_size, shuffle=False, num_workers=worker_set['val'])
 
     def train_val(self, 
-                  num_epochs: int=2, 
-                  interval: int=100, 
-                  backend: str="threading", 
-                  n_jobs: int=-1) -> None:
+                  num_epochs: int=2,
+                  interval: int=100,
+                  tolerance: float=1e-3,
+                  patience: int=10, 
+                  backend: str='threading', 
+                  n_jobs: int=-1,
+                  early_stop: bool=False) -> None:
         '''
         Training and Validation with `train_loader` and `val_container`.
         :param num_epochs: int, training epochs for `self.model`. default: 2.
         :param interval: int, console output interval. default: 100.
-        :param backend: str, "threading", "multiprocessing, "locky". default: "threading".
+        :param tolerance: float, tolerance set to judge difference in val_loss. default: 1e-3
+        :param patience: int, patience of no improvement waiting for training to stop. default: 10.
+        :param backend: str, 'threading', 'multiprocessing', 'locky'. default: 'threading'.
         :param n_jobs: int, accelerate processing of validation. default: -1.
+        :param early_stop: bool, whether to enable early_stop in train_val. default: False
         '''
         assert num_epochs > 0 and interval > 0, 'With num_epochs > 0 and interval > 0 to train parameters into outputs.'
+        assert tolerance > 1e-9 and tolerance < 1.0, 'Set tolerance to early stop training and validation process within patience.'
+        assert patience >= 10 and patience <= 100, 'Value coordinate with tolerance should fit about num_epochs and batch_size.' 
         assert n_jobs == -1 or n_jobs > 0, 'Take full jobs with setting n_jobs=-1 or manually set nums of jobs.'
         total_step = len(self.train_loader)
         self._set_container(backend, n_jobs)
         val_length = len(self.val_container)
+        self.stop_iter: bool = False # init state of train_val
         for epoch in range(num_epochs):
             gc.collect()
             torch.cuda.empty_cache()
             for i, (features, target) in enumerate(self.train_loader):
                 features = features.to(self.device)
                 target = target.to(self.device)
 
@@ -221,18 +230,37 @@
                 # validation with val_container
                 self.val_loss = 0 # int value at cpu
                 with parallel_backend(backend, n_jobs=n_jobs):
                     for val_set in self.val_container:
                         outputs_val = self.model(val_set[0].to(self.device)) # return value from cuda
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
                 self.val_loss /= val_length
+                val_counts = i + 1 + total_step * epoch
 
+                # early stop
+                if early_stop:
+                    bool_val_first: bool = i == 0 and epoch == 0
+                    if bool_val_first: # record first time of val_loss
+                        val_loss_pre = self.val_loss
+                    else:
+                        if val_loss_pre < self.val_loss:
+                            val_loss_pre = self.val_loss
+                        else:
+                            if val_counts % patience == 0:
+                                if val_loss_pre - self.val_loss < tolerance:
+                                    self.stop_iter: bool = True
+                                else:
+                                    val_loss_pre = self.val_loss
                 # console print
                 if (i + 1) % interval == 0:
-                    print ('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
+                    print('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
+
+            if self.stop_iter:
+                print('Process stop at epoch [{}/{}] with patience {} within tolerance {}'.format(epoch+1, num_epochs, patience, tolerance))
+                break
 
     def test(self, 
              sort_by: str='accuracy',
              sort_state: bool=True):
         '''
         Test with Initialized Configuration. `accuracy > 0`, 'correct_class != None'
         Configured keywords only work when `not self.is_target_2d and num_classes >= 2`.
```

## Comparing `perming-1.3.1.dist-info/METADATA` & `perming-1.4.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.3.1
+Version: 1.4.0
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
@@ -47,65 +47,71 @@
 ## general model
 
 |GENERAL_BOX(Box)|Parameters|Meaning|
 |--|--|--|
 |`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />device: str="cuda"<br />*<br />activation: str="relu"<br />inplace_on: bool=True<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier or Regressier Based on Basic Information of the Dataset Obtained through Data Preprocessing and Feature Engineering.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Numpy Dataset into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `num_epochs` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|train_val|num_epochs: int=2<br />tolerance: float=1e-3<br />patience: int=10<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 ## common models (cuda first)
 
 - Regression
 
 |Regressier|Parameters|Meaning|
 |--|--|--|
 |`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MSELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Regressier Based on Basic Information of the Regression Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=1`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|/|Test Module Only Show with Loss at 3 Stages: Train, Test, Val|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 - Binary-classification
 
 |Binarier|Parameters|Meaning|
 |--|--|--|
 |`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="BCELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=2`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Binary-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|sort_by: str="accuracy"<br />sort_state: bool=True|Test Module Show with Correct Class and Loss at 3 Stages: Train, Test, Val|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 - Multi-classification
 
 |Multipler|Parameters|Meaning|
 |--|--|--|
 |`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 - Multi-outputs
 
 |Ranker|Parameters|Meaning|
 |--|--|--|
 |`__init__`|input_: int<br />num_outputs: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MultiLabelSoftMarginLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Ranker Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with (n_samples, n_outputs).|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-outputs Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
+> prefer replace shape *(n,1)* with shape *(n,)* using `numpy.squeeze(input_matrix)`
+
 ## pip install
 
 download latest version:
 ```text
 git clone https://github.com/linjing-lab/easy-pytorch.git
 cd easy-pytorch/released_box
 pip install -e . --verbose
```

## Comparing `perming-1.3.1.dist-info/RECORD` & `perming-1.4.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perming/__init__.py,sha256=rL_phPpO1ftL_MoZLxTY0HwDkbrxLpoOwUm5S57ebLE,887
+perming/__init__.py,sha256=8Lz5WwpKYk2lLFHoif2LCuw9zlicEaLqzvmR5GOc2us,887
 perming/_typing.py,sha256=SGQP3QKfMZr-ciHT6jIrv4NUDmgqkx-RhYxIQloBSC4,176
-perming/_utils.py,sha256=vGOP8DKHvt7t5Iu35VnVRQ5un23uHTIEPByb97S1P1k,21066
+perming/_utils.py,sha256=y1IfBSyEYwGDHTNwRRvT2txih67v3Iob4ddG4RUgNB8,22794
 perming/_version.py,sha256=K3CPQxLgHmXPNpNWlhpnrp6Bt8v5rU9wZyVRBsRTI3E,568
 perming/common.py,sha256=_-wi8gZFYCtO81XNvu8y-WLJQiZj1-IJ9Ipr2YHWlYw,13988
 perming/general.py,sha256=sUjieRqdWa3o6PXdici5ABarVHcBTCVuv1Wg2K1kggI,5605
-perming-1.3.1.dist-info/METADATA,sha256=9qnNk_Vy8xrOXZ62pj8gm5nWkNJnxcFowZXdQujHGUM,8772
-perming-1.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-perming-1.3.1.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
-perming-1.3.1.dist-info/RECORD,,
+perming-1.4.0.dist-info/METADATA,sha256=n2vgTmwTVUH-23kPlE6tLBOW_SHyBlY6ZtKtAZdOD-8,10926
+perming-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+perming-1.4.0.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
+perming-1.4.0.dist-info/RECORD,,
```

