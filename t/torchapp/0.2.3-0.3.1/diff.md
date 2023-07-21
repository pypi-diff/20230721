# Comparing `tmp/torchapp-0.2.3.tar.gz` & `tmp/torchapp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchapp-0.2.3.tar", max compression
+gzip compressed data, was "torchapp-0.3.1.tar", max compression
```

## Comparing `torchapp-0.2.3.tar` & `torchapp-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    11345 2022-09-12 15:06:53.693505 torchapp-0.2.3/LICENSE
--rw-r--r--   0        0        0     6537 2022-09-12 15:06:53.693505 torchapp-0.2.3/README.rst
--rw-r--r--   0        0        0     2101 2022-09-12 15:06:53.697506 torchapp-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       53 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/__init__.py
--rw-r--r--   0        0        0    32749 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/apps.py
--rw-r--r--   0        0        0     2141 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/fastai.bib
--rw-r--r--   0        0        0      633 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/mlflow.bib
--rw-r--r--   0        0        0      426 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/optuna.bib
--rw-r--r--   0        0        0      474 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/skopt.bib
--rw-r--r--   0        0        0      244 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/torchapp.bib
--rw-r--r--   0        0        0      185 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/bibtex/wandb.bib
--rw-r--r--   0        0        0      420 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/blocks.py
--rw-r--r--   0        0        0       84 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/callbacks/__init__.py
--rw-r--r--   0        0        0     4116 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/callbacks/mlflow.py
--rw-r--r--   0        0        0      717 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/callbacks/wandb.py
--rw-r--r--   0        0        0     1891 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/citations.py
--rw-r--r--   0        0        0     1292 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/download.py
--rw-r--r--   0        0        0     1703 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/enums.py
--rw-r--r--   0        0        0        0 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/examples/__init__.py
--rw-r--r--   0        0        0     4287 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/examples/image_classifier.py
--rw-r--r--   0        0        0      738 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/examples/iris.bib
--rw-r--r--   0        0        0     1512 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/examples/iris.py
--rwxr-xr-x   0        0        0     1809 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/examples/logistic_regression.py
--rw-r--r--   0        0        0     2435 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/main.py
--rw-r--r--   0        0        0      638 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/metrics.py
--rw-r--r--   0        0        0      856 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/params.py
--rw-r--r--   0        0        0    14506 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/testing.py
--rw-r--r--   0        0        0        0 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/tuning/__init__.py
--rw-r--r--   0        0        0     2492 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/tuning/optuna.py
--rw-r--r--   0        0        0     2925 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/tuning/skopt.py
--rw-r--r--   0        0        0     3903 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/tuning/wandb.py
--rw-r--r--   0        0        0     3704 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/util.py
--rw-r--r--   0        0        0     3282 2022-09-12 15:06:53.701506 torchapp-0.2.3/torchapp/vision.py
--rw-r--r--   0        0        0     8332 1970-01-01 00:00:00.000000 torchapp-0.2.3/setup.py
--rw-r--r--   0        0        0     8396 1970-01-01 00:00:00.000000 torchapp-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-07-21 01:01:15.382093 torchapp-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6537 2023-07-21 01:01:15.382093 torchapp-0.3.1/README.rst
+-rw-r--r--   0        0        0     2142 2023-07-21 01:01:15.386093 torchapp-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/__init__.py
+-rw-r--r--   0        0        0    33403 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/apps.py
+-rw-r--r--   0        0        0     2141 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/fastai.bib
+-rw-r--r--   0        0        0      633 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/mlflow.bib
+-rw-r--r--   0        0        0      426 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/optuna.bib
+-rw-r--r--   0        0        0      470 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/skopt.bib
+-rw-r--r--   0        0        0      244 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/torchapp.bib
+-rw-r--r--   0        0        0      185 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/wandb.bib
+-rw-r--r--   0        0        0      420 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/blocks.py
+-rw-r--r--   0        0        0       84 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/__init__.py
+-rw-r--r--   0        0        0     4116 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/mlflow.py
+-rw-r--r--   0        0        0      717 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/wandb.py
+-rw-r--r--   0        0        0     1937 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/citations.py
+-rw-r--r--   0        0        0     2215 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/download.py
+-rw-r--r--   0        0        0     1904 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/enums.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/__init__.py
+-rw-r--r--   0        0        0    12563 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/diffusion.py
+-rw-r--r--   0        0        0     6750 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/image_classifier.py
+-rw-r--r--   0        0        0      738 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/iris.bib
+-rw-r--r--   0        0        0     1512 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/iris.py
+-rwxr-xr-x   0        0        0     1809 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/logistic_regression.py
+-rw-r--r--   0        0        0     1053 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/mlp.py
+-rw-r--r--   0        0        0     2435 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/main.py
+-rw-r--r--   0        0        0      638 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/metrics.py
+-rw-r--r--   0        0        0     1161 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/params.py
+-rw-r--r--   0        0        0    15279 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/testing.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/tuning/__init__.py
+-rw-r--r--   0        0        0     2763 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/tuning/optuna.py
+-rw-r--r--   0        0        0     5376 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/tuning/skopt.py
+-rw-r--r--   0        0        0     3794 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/tuning/wandb.py
+-rw-r--r--   0        0        0     3704 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/util.py
+-rw-r--r--   0        0        0     3384 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/vision.py
+-rw-r--r--   0        0        0     8479 1970-01-01 00:00:00.000000 torchapp-0.3.1/PKG-INFO
```

### Comparing `torchapp-0.2.3/LICENSE` & `torchapp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/README.rst` & `torchapp-0.3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :target: https://rbturnbull.github.io/torchapp/coverage/
 
 .. |git3moji badge| image:: https://img.shields.io/badge/git3moji-%E2%9A%A1%EF%B8%8F%F0%9F%90%9B%F0%9F%93%BA%F0%9F%91%AE%F0%9F%94%A4-fffad8.svg
     :target: https://robinpokorny.github.io/git3moji/
 
 .. end-badges
 
-A wrapper for PyTorch projects to create easy command-line inferfaces and manage hyper-parameter tuning.
+A wrapper for PyTorch projects to create easy command-line interfaces and manage hyper-parameter tuning.
 
 Documentation at https://rbturnbull.github.io/torchapp/
 
 .. start-quickstart
 
 Installation
 =======================
```

### Comparing `torchapp-0.2.3/pyproject.toml` & `torchapp-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torchapp"
-version = "0.2.3"
+version = "0.3.1"
 description = "A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning."
 authors = ["Robert Turnbull <robert.turnbull@unimelb.edu.au>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/rbturnbull/torchapp"
 documentation = "https://rbturnbull.github.io/torchapp/"
 homepage = "https://github.com/rbturnbull/torchapp"
@@ -15,35 +15,36 @@
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-torch = "^1.12.1"
-numpy = "^1.22.0"
+torch = ">=1.12.1"
+numpy = ">=1.22.0,<1.24.0"
 typer = "^0.4.0"
 rich = "^10.16.1"
 fastai = "^2.5.3"
 pandas = "^1.3.5"
 wandb = "^0.12.9"
 cookiecutter = "^2.1.1"
-scikit-learn = "^1.0.2"
+scikit-learn = ">=1.0.2,<1.2.0"
 Pillow = "^9.0.1"
 PyYAML = "^6.0"
 click = "8.0.4"
-torchvision = "^0.13.1"
+torchvision = ">=0.13.0"
 pybtex = "^0.24.0"
 pyjwt = ">=2.4.0"
 mlflow = "^1.25.1"
 optuna = "^2.10.0"
 pybtexnbib = "^0.1.1"
 scikit-optimize = "^0.9.0"
 scipy = "^1.9.1"
 appdirs = "^1.4.4"
+certifi = "^2023.5.7"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 ipython = "^8.1.1"
 ipykernel = "^6.6.1"
 coverage = "^5.5"
```

### Comparing `torchapp-0.2.3/torchapp/apps.py` & `torchapp-0.3.1/torchapp/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import typer
 from typer.main import get_params_convertors_ctx_param_name_from_function
 from rich.console import Console
 from rich.traceback import install
 from rich.table import Table
 from rich.box import SIMPLE
 
+
+
 install()
 console = Console()
 
 from .citations import Citable
 from .util import copy_func, call_func, change_typer_to_defaults, add_kwargs
 from .params import Param
 from .callbacks import TorchAppWandbCallback, TorchAppMlflowCallback
@@ -117,20 +119,24 @@
         change_typer_to_defaults(self.inference_dataloader)
         change_typer_to_defaults(self.output_results)
 
         # Store a bool to let the app know later on (in self.assert_initialized)
         # that __init__ has been called on this parent class
         self.torchapp_initialized = True
         self.learner_obj = None
+        # self.console = console
 
     def __str__(self):
         return self.__class__.__name__
 
     def get_bibtex_files(self):
-        return [bibtex_dir / "fastai.bib", bibtex_dir / "torchapp.bib"]
+        return [
+            bibtex_dir / "fastai.bib", 
+            bibtex_dir / "torchapp.bib",
+        ]
 
     def copy_method(self, method):
         return MethodType(copy_func(method.__func__), self)
 
     def pretrained_location(self) -> Union[str, Path]:
         """
         The location of a pretrained model.
@@ -206,32 +212,33 @@
             raise FileNotFoundError(f"Cannot find pretrained model at '{path}'")
 
         return path
 
     def prepare_source(self, data):
         return data
 
-    def output_results(self, results, **kwargs):
-        print(results)
-
     def inference_dataloader(self, learner, **kwargs):
         dataloader = learner.dls.test_dl(**kwargs)
         return dataloader
 
     def validate(
         self,
         gpu: bool = Param(True, help="Whether or not to use a GPU for processing if available."),
         **kwargs,
     ):
         path = call_func(self.pretrained_local_path, **kwargs)
 
         # Check if CUDA is available
         gpu = gpu and torch.cuda.is_available()
 
-        learner = load_learner(path, cpu=not gpu)
+        try:
+            learner = load_learner(path, cpu=not gpu)
+        except Exception:
+            import dill
+            learner = load_learner(path, cpu=not gpu, pickle_module=dill)
 
         # Create a dataloader for inference
         dataloaders = call_func(self.dataloaders, **kwargs)
 
         table = Table(title="Validation", box=SIMPLE)
 
         values = learner.validate(dl=dataloaders.valid)
@@ -259,20 +266,23 @@
         # Open the exported learner from a pickle file
         path = call_func(self.pretrained_local_path, **kwargs)
         learner = self.learner_obj = load_learner(path, cpu=not gpu)
 
         # Create a dataloader for inference
         dataloader = call_func(self.inference_dataloader, learner, **kwargs)
 
-        results = learner.get_preds(dl=dataloader, reorder=False, with_decoded=False, act=self.activation())
+        results = learner.get_preds(dl=dataloader, reorder=False, with_decoded=False, act=self.activation(), cbs=self.inference_callbacks())
 
         # Output results
         output_results = call_func(self.output_results, results, **kwargs)
         return output_results if output_results is not None else results
 
+    def inference_callbacks(self):
+        return None
+
     @classmethod
     def main(cls, inference_only:bool=False):
         """
         Creates an instance of this class and runs the command-line interface.
         """
         cli = cls.click(inference_only=inference_only)
         return cli()
@@ -454,15 +464,18 @@
             default_value = value.default
             if isinstance(default_value, Param) and default_value.tune == True:
 
                 # Override annotation if given in typing hints
                 if value.annotation:
                     default_value.annotation = value.annotation
 
+                default_value.check_choices()
+
                 tuning_params[key] = default_value
+                
         return tuning_params
 
     def dataloaders(self):
         raise NotImplementedError(
             f"Please ensure that the 'dataloaders' method is implemented in {self.__class__.__name__}."
         )
 
@@ -518,21 +531,21 @@
         output_dir: Path = Param("./outputs", help="The location of the output directory."),
         weight_decay: float = Param(
             None, help="The amount of weight decay. If None then it uses the default amount of weight decay in fastai."
         ),
         # l2_regularization: bool = Param(False, help="Whether to add decay to the gradients (L2 regularization) instead of to the weights directly (weight decay)."),
         **kwargs,
     ):
-        output_dir = Path(output_dir)
-        output_dir.mkdir(exist_ok=True, parents=True)
+        self.output_dir = Path(output_dir)
+        self.output_dir.mkdir(exist_ok=True, parents=True)
 
         return dict(
             loss_func=call_func(self.loss_func, **kwargs),
             metrics=call_func(self.metrics, **kwargs),
-            path=output_dir,
+            path=self.output_dir,
             wd=weight_decay,
         )
 
     def loss_func(self, **kwargs):
         """The loss function. If None, then fastai will use the default loss function if it exists for this model."""
         return None
 
@@ -625,16 +638,23 @@
             callbacks.append(callback)
             self.add_bibtex_file(bibtex_dir / "wandb.bib")  # this should be in the callback
 
         if mlflow:
             callbacks.append(TorchAppMlflowCallback(app=self, experiment_name=project_name))
             self.add_bibtex_file(bibtex_dir / "mlflow.bib")  # this should be in the callback
 
+        extra_callbacks = self.extra_callbacks()
+        if extra_callbacks:
+            callbacks += extra_callbacks
+
         return callbacks
 
+    def extra_callbacks(self):
+        return None
+
     def show_batch(
         self, output_path: Path = Param(None, help="A location to save the HTML which summarizes the batch."), **kwargs
     ):
         dataloaders = call_func(self.dataloaders, **kwargs)
 
         # patch the display function of ipython so we can capture the HTML
         def mock_display(html_object):
@@ -725,30 +745,30 @@
         """
         return self.__class__.__name__
 
     def tune(
         self,
         runs: int = Param(default=1, help="The number of runs to attempt to train the model."),
         engine: str = Param(
-            default="wandb",
+            default="skopt",
             help="The optimizer to use to perform the hyperparameter tuning. Options: wandb, optuna, skopt.",
         ),  # should be enum
         id: str = Param(
             default="",
             help="The ID of this hyperparameter tuning job. "
             "If using wandb, then this is the sweep id. "
             "If using optuna, then this is the storage. "
             "If using skopt, then this is the file to store the results. ",
         ),
         name: str = Param(
             default="",
             help="An informative name for this hyperparameter tuning job. If empty, then it creates a name from the project name.",
         ),
         method: str = Param(
-            default="random", help="The sampling method to use to perform the hyperparameter tuning."
+            default="", help="The sampling method to use to perform the hyperparameter tuning. By default it chooses the default method of the engine."
         ),  # should be enum
         min_iter: int = Param(
             default=None,
             help="The minimum number of iterations if using early termination. If left empty, then early termination is not used.",
         ),
         seed: int = Param(
             default=None,
@@ -879,7 +899,15 @@
         return result
 
     def cache_dir(self) -> Path:
         """ Returns a path to a directory where data files for this app can be cached. """
         cache_dir = Path(user_cache_dir("torchapps"))/self.__class__.__name__
         cache_dir.mkdir(exist_ok=True, parents=True)
         return cache_dir
+
+    def output_results(
+        self, 
+        results, 
+        **kwargs
+    ):
+        print(results)
+        return results
```

### Comparing `torchapp-0.2.3/torchapp/bibtex/fastai.bib` & `torchapp-0.3.1/torchapp/bibtex/fastai.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/bibtex/mlflow.bib` & `torchapp-0.3.1/torchapp/bibtex/mlflow.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/callbacks/mlflow.py` & `torchapp-0.3.1/torchapp/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/callbacks/wandb.py` & `torchapp-0.3.1/torchapp/callbacks/wandb.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/citations.py` & `torchapp-0.3.1/torchapp/citations.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     def get_bibtex_files(self) -> List:
         return []
 
     def add_bibtex_file(self, file):
         if not self.bibtex_files:
             self.set_bibtext_files()
 
-        self.bibtex_files.append(file)
+        if file not in self.bibtex_files:
+            self.bibtex_files.append(file)
 
     def set_bibtex_files(self):
         self.bibtex_files = self.get_bibtex_files()
 
     def bibtex(self) -> str:
         bibtex_strings = []
         for bibtex_file in self.bibtex_files:
```

### Comparing `torchapp-0.2.3/torchapp/enums.py` & `torchapp-0.3.1/torchapp/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,7 +57,17 @@
         Returns:
             nn.Module: The pytorch module for this activation function.
         """
         if not hasattr(nn, self.value):
             raise ActivationError(f"Activation function '{self.value}' not available.")
 
         return getattr(nn, self.value)(*args, **kwargs)
+
+    @classmethod
+    def default_tune_choices(cls):
+        return [
+            cls.ReLU,
+            cls.LeakyReLU,
+            cls.RReLU,
+            cls.ELU,
+            cls.Hardsigmoid,
+        ]
```

### Comparing `torchapp-0.2.3/torchapp/examples/image_classifier.py` & `torchapp-0.3.1/torchapp/examples/image_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List
 from pathlib import Path
 import torch
 from fastai.data.block import DataBlock, CategoryBlock
-from fastai.data.transforms import ColReader, RandomSplitter, DisplayedTransform, ColSplitter
+from fastai.data.transforms import ColReader, RandomSplitter, DisplayedTransform, ColSplitter, get_image_files
 from fastai.metrics import accuracy
 from fastai.vision.data import ImageBlock
 from fastai.vision.augment import Resize, ResizeMethod
 import pandas as pd
 import torchapp as ta
+from fastai.vision.augment import aug_transforms
 
 from torchapp.vision import VisionApp
 from rich.console import Console
 console = Console()
 
 
 class PathColReader(DisplayedTransform):
@@ -36,78 +37,135 @@
     def dataloaders(
         self,
         csv: Path = ta.Param(default=None, help="A CSV with image paths and categories."),
         image_column: str = ta.Param(default="image", help="The name of the column with the image paths."),
         category_column: str = ta.Param(
             default="category", help="The name of the column with the category of the image."
         ),
-        base_dir: Path = ta.Param(default="./", help="The base directory for images with relative paths."),
+        base_dir: Path = ta.Param(default=None, help="The base directory for images with relative paths. If not given, then it is relative to the csv directory."),
         validation_column: str = ta.Param(
             default="validation",
             help="The column in the dataset to use for validation. "
             "If the column is not in the dataset, then a validation set will be chosen randomly according to `validation_proportion`.",
         ),
+        validation_value: str = ta.Param(
+            default=None,
+            help="If set, then the value in the `validation_column` must equal this string for the item to be in the validation set. "
+        ),
         validation_proportion: float = ta.Param(
             default=0.2,
             help="The proportion of the dataset to keep for validation. Used if `validation_column` is not in the dataset.",
         ),
         batch_size: int = ta.Param(default=16, help="The number of items to use in each batch."),
         width: int = ta.Param(default=224, help="The width to resize all the images to."),
         height: int = ta.Param(default=224, help="The height to resize all the images to."),
         resize_method: str = ta.Param(default="squish", help="The method to resize images."),
+        max_lighting:float=0.0,
+        max_rotate:float=0.0,
+        max_warp:float=0.0,
+        max_zoom:float=1.0,
+        do_flip:bool=False,
+        p_affine:float=0.75,
+        p_lighting:float=0.75,
     ):
         df = pd.read_csv(csv)
 
+        base_dir = base_dir or Path(csv).parent
+        
         # Create splitter for training/validation images
+        if validation_value is not None:
+            validation_column_new = f"{validation_column} is {validation_value}"
+            df[validation_column_new] = df[validation_column].astype(str) == validation_value
+            validation_column = validation_column_new
+            
         if validation_column and validation_column in df:
             splitter = ColSplitter(validation_column)
         else:
             splitter = RandomSplitter(validation_proportion)
 
+        batch_transforms = aug_transforms(
+            p_lighting=p_lighting,
+            p_affine=p_affine,
+            max_rotate=max_rotate, 
+            do_flip=do_flip, 
+            max_lighting=max_lighting, 
+            max_zoom=max_zoom,
+            max_warp=max_warp,
+            pad_mode='zeros',
+        )
+
         datablock = DataBlock(
             blocks=[ImageBlock, CategoryBlock],
             get_x=PathColReader(column_name=image_column, base_dir=base_dir),
             get_y=ColReader(category_column),
             splitter=splitter,
             item_tfms=Resize((height, width), method=resize_method),
+            batch_tfms=batch_transforms,
         )
 
         return datablock.dataloaders(df, bs=batch_size)
 
     def metrics(self):
         return [accuracy]
 
     def monitor(self):
         return "accuracy"
 
     def inference_dataloader(
         self, 
         learner, 
         items:List[Path] = None, 
+        csv: Path = ta.Param(default=None, help="A CSV with image paths."),
+        image_column: str = ta.Param(default="image", help="The name of the column with the image paths."),
+        base_dir: Path = ta.Param(default="./", help="The base directory for images with relative paths."),
         **kwargs
     ):
-        if not items:
-            items = []
+        self.items = []
         if isinstance(items, (Path, str)):
-            items = [items]
+            self.items.append(Path(items))
+        else:
+            try:
+                for item in items:
+                    item = Path(item)
+                    # If the item is a directory then get all images in that directory
+                    if item.is_dir():
+                        self.items.extend( get_image_files(item) )
+                    else:
+                        self.items.append(item)
+            except:
+                raise ValueError(f"Cannot interpret list of items.")
+
+        # Read CSV if available
+        if csv is not None:
+            df = pd.read_csv(csv)
+            for _, row in df.iterrows():
+                self.items.append(Path(row[image_column]))
+
+        if not self.items:
+            raise ValueError(f"No items found.")
+
+        # Set relative to base dir
+        if base_dir:
+            base_dir = Path(base_dir)
+        
+            self.items = [base_dir / item if not item.is_absolute() else item for item in self.items]
 
-        items = [Path(item) for item in items]
-        self.items = items
-        return learner.dls.test_dl(items, **kwargs)
+        return learner.dls.test_dl(self.items, **kwargs)
 
     def output_results(
         self, 
         results, 
         output_csv:Path = ta.Param(None, help="Path to write predictions in CSV format"), 
         verbose:bool = True, 
         **kwargs
     ):
         data = []
         vocab = self.learner_obj.dls.vocab
-        for item, probabilities in zip(self.items, results[0]):            
+        for item, scores in zip(self.items, results[0]): 
+            probabilities = torch.softmax(torch.as_tensor(scores), dim=-1)           
             prediction = vocab[torch.argmax(probabilities)]
             if verbose:
                 console.print(f"'{item}': '{prediction}'")
             data.append( [item,prediction] + probabilities.tolist() )
 
         df = pd.DataFrame(data, columns=["path","prediction"]+list(vocab))
         if output_csv:
```

### Comparing `torchapp-0.2.3/torchapp/examples/iris.bib` & `torchapp-0.3.1/torchapp/examples/iris.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/examples/iris.py` & `torchapp-0.3.1/torchapp/examples/iris.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/examples/logistic_regression.py` & `torchapp-0.3.1/torchapp/examples/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/main.py` & `torchapp-0.3.1/torchapp/main.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/metrics.py` & `torchapp-0.3.1/torchapp/metrics.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/params.py` & `torchapp-0.3.1/torchapp/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-import math
 from typer.models import OptionInfo
-from typing import NamedTuple, List
-from numbers import Number
+from .enums import Activation
 
 
 class Param(OptionInfo):
     def __init__(
         self,
         default=None,
         tune=False,
         tune_min=None,
         tune_max=None,
         tune_choices=None,
-        log=False,
+        log=False, # deprecated. use tune_log
+        tune_log=False,
         distribution=None,
         annotation=None,
         **kwargs,
     ):
         super().__init__(default=default, **kwargs)
         self.tune = tune
-        self.log = log
+        self.tune_log = tune_log or log
         self.tune_min = tune_min if tune_min is not None else self.min
         self.tune_max = tune_max if tune_max is not None else self.max
         self.annotation = annotation
         self.distribution = distribution
         self.tune_choices = tune_choices
+        
         if distribution:
             raise NotImplementedError("Distribution for parameters not implemented yet")
+
+    def check_choices(self):
+        if self.tune_choices:
+            return
+
+        if self.annotation == bool:
+            self.tune_choices = [False, True]
+
+        elif self.annotation == Activation:
+            self.tune_choices = Activation.default_tune_choices()
```

### Comparing `torchapp-0.2.3/torchapp/testing.py` & `torchapp-0.3.1/torchapp/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,28 +82,49 @@
     if isinstance(output, (TensorBase, torch.Tensor)):
         output = f"{type(output)} {tuple(output.shape)}"
     output = str(output)
     output = re.sub(r"0[xX][0-9a-fA-F]+", "<HEX>", output)
     return output
 
 
+def strip_whitespace_recursive(obj):
+    if isinstance(obj, str):
+        obj = obj.replace("\n", " ").strip()
+        return re.sub(r"\s+", " ", obj)
+    if isinstance(obj, dict):
+        return {k:strip_whitespace_recursive(v) for k,v in obj.items()}
+
+    return obj
+
+
 def assert_output(file: Path, interactive: bool, params: dict, output, expected, regenerate: bool = False):
     """
     Tests to see if the output is the same as the expected data and allows for saving a new version of the expected files if needed.
 
     Args:
         file (Path): The path to the expected file in yaml format.
         interactive (bool): Whether or not to prompt for replacing the expected file.
         params (dict): The dictionary of parameters to store in the expected file.
         output (str): The string representation of the output from the app.
         expected (str): The expected output from the yaml file.
     """
     if expected == output:
         return
 
+    # if expected and output are both strings, check to see if they are equal when normalizing whitespace
+    expected_cleaned = strip_whitespace_recursive(expected)
+    output_cleaned = strip_whitespace_recursive(output)
+    if expected_cleaned == output_cleaned:
+        return
+
+    print(' ----------------------\n')
+    print('expected_cleaned ----------------------\n', expected_cleaned)
+    print('output_cleaned ----------------------\n', output_cleaned)
+    print(' ----------------------\n')
+
     if isinstance(expected, dict) and isinstance(output, dict):
         keys = set(expected.keys()) | set(output.keys())
         diff = {}
         for key in keys:
             diff[key] = get_diff(expected.get(key, ""), output.get(key, ""))
             if diff[key]:
                 console.print(diff[key])
```

### Comparing `torchapp-0.2.3/torchapp/tuning/optuna.py` & `torchapp-0.3.1/torchapp/tuning/optuna.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     )
 
 from ..util import call_func
 
 
 def get_sampler(method, seed=0):
     method = method.lower()
-    if method.startswith("tpe"):
+    if method.startswith("tpe") or not method:
         return samplers.TPESampler(seed=seed)
     elif method.startswith("cma"):
         return samplers.CmaEsSampler(seed=seed)
     # elif method.startswith("grid"):
     #     return samplers.GridSampler()
     elif method.startswith("random"):
         return samplers.RandomSampler(seed=seed)
@@ -26,30 +26,33 @@
     raise NotImplementedError(f"Cannot interpret sampling method '{method}' using Optuna.")
 
 
 def suggest(trial, name, param):
     if param.tune_choices:
         return trial.suggest_categorical(name, param.tune_choices)
     elif param.annotation == float:
-        return trial.suggest_float(name, param.tune_min, param.tune_max, log=param.log)
+        return trial.suggest_float(name, param.tune_min, param.tune_max, log=param.tune_log)
     elif param.annotation == int:
-        return trial.suggest_int(name, param.tune_min, param.tune_max, log=param.log)
+        return trial.suggest_int(name, param.tune_min, param.tune_max, log=param.tune_log)
 
     raise NotImplementedError("Optuna Tuning Engine cannot understand param '{name}': {param}")
 
 
 def optuna_tune(
     app,
     storage: str = "",
     name: str = None,
     method: str = "tpe",  # Should be enum
     runs: int = 1,
     seed: int = None,
     **kwargs,
 ):
+    output_dir = Path(kwargs.get("output_dir", "."))
+    output_dir.mkdir(parents=True, exist_ok=True)
+
     def objective(trial: optuna.Trial):
         run_kwargs = dict(kwargs)
 
         tuning_params = app.tuning_params()
 
         for key, value in tuning_params.items():
             if key not in kwargs or kwargs[key] is None:
@@ -66,14 +69,18 @@
         learner = call_func(app.train, **run_kwargs)
 
         # Return metric from recorder
         return app.get_best_metric(learner)
 
     if not storage:
         storage = None
+    elif "://" not in storage:
+        storage_path = output_dir/f"{storage}.sqlite3"
+        storage = f"sqlite:///{storage_path.resolve()}"
+
     study = optuna.create_study(
         study_name=name,
         storage=storage,
         sampler=get_sampler(method, seed=seed),
         load_if_exists=True,
         direction=app.goal(),
     )
```

### Comparing `torchapp-0.2.3/torchapp/tuning/wandb.py` & `torchapp-0.3.1/torchapp/tuning/wandb.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,19 @@
 def get_parameter_config(param) -> dict:
     if param.tune_choices:
         return dict(
             distribution="categorical",
             values=param.tune_choices,
         )
 
-    if param.annotation == bool:
-        return dict(
-            distribution="categorical",
-            values=[False, True],
-        )
-
     if param.annotation in [int, float]:
         assert param.tune_min is not None
         assert param.tune_max is not None
 
-        distribution = "log_uniform_values" if param.log else "uniform"
+        distribution = "log_uniform_values" if param.tune_log else "uniform"
         if param.annotation == int:
             distribution = f"q_{distribution}"
 
         return dict(
             distribution=distribution,
             min=param.tune_min,
             max=param.tune_max,
@@ -37,25 +31,26 @@
 
     raise NotImplementedError
 
 
 def get_sweep_config(
     app,
     name: str = None,
-    method: str = "random",  # Should be enum
+    method: str = "",  # Should be enum
     min_iter: int = None,
     **kwargs,
 ):
     parameters_config = dict()
     tuning_params = app.tuning_params()
 
     for key, value in tuning_params.items():
         if key not in kwargs or kwargs[key] is None:
             parameters_config[key] = get_parameter_config(value)
 
+    method = method or "bayes"
     if method not in ["grid", "random", "bayes"]:
         raise NotImplementedError(f"Cannot interpret sampling method '{method}' using wandb.")
 
     sweep_config = {
         "name": name,
         "method": method,
         "parameters": parameters_config,
```

### Comparing `torchapp-0.2.3/torchapp/util.py` & `torchapp-0.3.1/torchapp/util.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.2.3/torchapp/vision.py` & `torchapp-0.3.1/torchapp/vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,22 @@
 
         # Only accept functions
         if isinstance(obj, types.FunctionType):
 
             # Only accept if the return value is a pytorch module
             hints = get_type_hints(obj)
             return_value = hints.get("return", "")
-            if nn.Module in return_value.mro():
-                model_choices.append(item)
-    return model_choices
+            try:
+                mro = return_value.mro()
+                if nn.Module in mro:
+                    model_choices.append(item)
+            except TypeError:
+                pass
 
+    return model_choices
 
 TorchvisionModelEnum = enum.Enum(
     "TorchvisionModelName",
     {model_name if model_name else "default": model_name for model_name in torchvision_model_choices()},
 )
```

### Comparing `torchapp-0.2.3/PKG-INFO` & `torchapp-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: torchapp
-Version: 0.2.3
+Version: 0.3.1
 Summary: A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning.
 Home-page: https://github.com/rbturnbull/torchapp
 License: Apache-2.0
 Keywords: fastai,pytorch,deep learning,command-line interface
 Author: Robert Turnbull
 Author-email: robert.turnbull@unimelb.edu.au
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Pillow (>=9.0.1,<10.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: click (==8.0.4)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: fastai (>=2.5.3,<3.0.0)
 Requires-Dist: mlflow (>=1.25.1,<2.0.0)
-Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Requires-Dist: numpy (>=1.22.0,<1.24.0)
 Requires-Dist: optuna (>=2.10.0,<3.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: pybtex (>=0.24.0,<0.25.0)
 Requires-Dist: pybtexnbib (>=0.1.1,<0.2.0)
 Requires-Dist: pyjwt (>=2.4.0)
 Requires-Dist: rich (>=10.16.1,<11.0.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.0.2,<1.2.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
-Requires-Dist: torch (>=1.12.1,<2.0.0)
-Requires-Dist: torchvision (>=0.13.1,<0.14.0)
+Requires-Dist: torch (>=1.12.1)
+Requires-Dist: torchvision (>=0.13.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Requires-Dist: wandb (>=0.12.9,<0.13.0)
 Project-URL: Documentation, https://rbturnbull.github.io/torchapp/
 Project-URL: Repository, https://github.com/rbturnbull/torchapp
 Description-Content-Type: text/x-rst
 
 ==========
@@ -68,15 +70,15 @@
     :target: https://rbturnbull.github.io/torchapp/coverage/
 
 .. |git3moji badge| image:: https://img.shields.io/badge/git3moji-%E2%9A%A1%EF%B8%8F%F0%9F%90%9B%F0%9F%93%BA%F0%9F%91%AE%F0%9F%94%A4-fffad8.svg
     :target: https://robinpokorny.github.io/git3moji/
 
 .. end-badges
 
-A wrapper for PyTorch projects to create easy command-line inferfaces and manage hyper-parameter tuning.
+A wrapper for PyTorch projects to create easy command-line interfaces and manage hyper-parameter tuning.
 
 Documentation at https://rbturnbull.github.io/torchapp/
 
 .. start-quickstart
 
 Installation
 =======================
```

