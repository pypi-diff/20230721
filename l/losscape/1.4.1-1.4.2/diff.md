# Comparing `tmp/losscape-1.4.1.tar.gz` & `tmp/losscape-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.4.1.tar", last modified: Fri Jul 21 13:38:24 2023, max compression
+gzip compressed data, was "losscape-1.4.2.tar", last modified: Fri Jul 21 13:44:15 2023, max compression
```

## Comparing `losscape-1.4.1.tar` & `losscape-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3293 2023-07-21 13:38:24.643021 losscape-1.4.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.4.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.1/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.1/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.1/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.4.1/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.1/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3293 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 13:38:24.643021 losscape-1.4.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-21 13:37:59.000000 losscape-1.4.1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.164334 losscape-1.4.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-21 13:44:15.164334 losscape-1.4.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.160334 losscape-1.4.2/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.2/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.2/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.2/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.4.2/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.2/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.164334 losscape-1.4.2/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 13:44:15.164334 losscape-1.4.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-21 13:44:09.000000 losscape-1.4.2/setup.py
```

### Comparing `losscape-1.4.1/PKG-INFO` & `losscape-1.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.1
+Version: 1.4.2
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
 
-This is the official repository for `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
+This is `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
 
-`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and lightning-fast rendering speed over other comparable libraries.
+`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and fast rendering speed.
 
 ## Key Features ✨
 
 - 🏃 **Fast Rendering**: Leveraging PyTorch's `torch.no_grad()` feature and controlling the number of examples to compute the loss, `losscape` speeds up the visualization process dramatically, thus saving valuable wall time.
-- 📊 **Flexible Plotting**: Supports both 1D and 2D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
+- 📊 **Flexible Plotting**: Supports both 2D and 3D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
 - 🔌 **Plug and Play**: Easy to integrate with your existing PyTorch models. No substantial modifications to your codebase are needed!
 
 ## Installation 📦
 
 You can install `losscape` via pip:
 
 ```
@@ -41,27 +41,27 @@
 train(model, train_loader) # losscape can perform the training for you
 create_2D_losscape(model, train_loader, output_vtp=True)
 ```
 
 Typical results :
 
 <p float="left" align="center">
-  <img src="docs/1d_landscape.png" width="400" />
-  <img src="docs/2d_landscape.png" width="400" /> 
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/1d_landscape.png?raw=true" width="400" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/2d_landscape.png?raw=true" width="400" /> 
 </p>
 
 To visualize the loss landscape in 3D, use the `.vtp` file created by the library and simply drag-and-drop it in [a VTK viewer](https://kitware.github.io/itk-vtk-viewer/app/) :
 
 <p align="center">
-  <img src="docs/3d_landscape.png" width="300" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/3d_landscape.png?raw=true" width="300" />
 </p>
 
 ## Documentation 📖
 For more details, please refer to the documentation. It provides a global overview on how `losscape` works, and on how you can leverage it with your own model.
-(to be written).
+(to be written : for now you can refer to the code, its simple enough to understand the structure of the library, and you can spin up using the juypter notebook example, all available on the Github repo).
 
 ## References 📚
 - [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913)
 - [Visualizing the Loss Landscape of Winning Lottery Tickets](https://arxiv.org/abs/2112.08538)
 
 
 ## Roadmap 🚀
```

### Comparing `losscape-1.4.1/README.md` & `losscape-1.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # loss + landscape = `losscape` 🌄
 
-This is the official repository for `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
+This is `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
 
-`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and lightning-fast rendering speed over other comparable libraries.
+`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and fast rendering speed.
 
 ## Key Features ✨
 
 - 🏃 **Fast Rendering**: Leveraging PyTorch's `torch.no_grad()` feature and controlling the number of examples to compute the loss, `losscape` speeds up the visualization process dramatically, thus saving valuable wall time.
-- 📊 **Flexible Plotting**: Supports both 1D and 2D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
+- 📊 **Flexible Plotting**: Supports both 2D and 3D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
 - 🔌 **Plug and Play**: Easy to integrate with your existing PyTorch models. No substantial modifications to your codebase are needed!
 
 ## Installation 📦
 
 You can install `losscape` via pip:
 
 ```
@@ -32,27 +32,27 @@
 train(model, train_loader) # losscape can perform the training for you
 create_2D_losscape(model, train_loader, output_vtp=True)
 ```
 
 Typical results :
 
 <p float="left" align="center">
-  <img src="docs/1d_landscape.png" width="400" />
-  <img src="docs/2d_landscape.png" width="400" /> 
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/1d_landscape.png?raw=true" width="400" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/2d_landscape.png?raw=true" width="400" /> 
 </p>
 
 To visualize the loss landscape in 3D, use the `.vtp` file created by the library and simply drag-and-drop it in [a VTK viewer](https://kitware.github.io/itk-vtk-viewer/app/) :
 
 <p align="center">
-  <img src="docs/3d_landscape.png" width="300" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/3d_landscape.png?raw=true" width="300" />
 </p>
 
 ## Documentation 📖
 For more details, please refer to the documentation. It provides a global overview on how `losscape` works, and on how you can leverage it with your own model.
-(to be written).
+(to be written : for now you can refer to the code, its simple enough to understand the structure of the library, and you can spin up using the juypter notebook example, all available on the Github repo).
 
 ## References 📚
 - [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913)
 - [Visualizing the Loss Landscape of Winning Lottery Tickets](https://arxiv.org/abs/2112.08538)
 
 
 ## Roadmap 🚀
```

### Comparing `losscape-1.4.1/losscape/compute_loss.py` & `losscape-1.4.2/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.1/losscape/create_directions.py` & `losscape-1.4.2/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.1/losscape/create_landscape.py` & `losscape-1.4.2/losscape/create_landscape.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.1/losscape/train.py` & `losscape-1.4.2/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.1/losscape.egg-info/PKG-INFO` & `losscape-1.4.2/losscape.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.1
+Version: 1.4.2
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
 
-This is the official repository for `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
+This is `losscape`, a lightweight, modular, and straightforward Python library that empowers you to visualize the loss landscape of your neural networks, as in [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913).
 
-`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and lightning-fast rendering speed over other comparable libraries.
+`losscape` is designed as a plug-and-play extension for your existing PyTorch models. It boasts its simplicity, modularity, and fast rendering speed.
 
 ## Key Features ✨
 
 - 🏃 **Fast Rendering**: Leveraging PyTorch's `torch.no_grad()` feature and controlling the number of examples to compute the loss, `losscape` speeds up the visualization process dramatically, thus saving valuable wall time.
-- 📊 **Flexible Plotting**: Supports both 1D and 2D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
+- 📊 **Flexible Plotting**: Supports both 2D and 3D plotting options for your loss landscapes, giving you the power to choose based on your requirements and computational constraints.
 - 🔌 **Plug and Play**: Easy to integrate with your existing PyTorch models. No substantial modifications to your codebase are needed!
 
 ## Installation 📦
 
 You can install `losscape` via pip:
 
 ```
@@ -41,27 +41,27 @@
 train(model, train_loader) # losscape can perform the training for you
 create_2D_losscape(model, train_loader, output_vtp=True)
 ```
 
 Typical results :
 
 <p float="left" align="center">
-  <img src="docs/1d_landscape.png" width="400" />
-  <img src="docs/2d_landscape.png" width="400" /> 
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/1d_landscape.png?raw=true" width="400" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/2d_landscape.png?raw=true" width="400" /> 
 </p>
 
 To visualize the loss landscape in 3D, use the `.vtp` file created by the library and simply drag-and-drop it in [a VTK viewer](https://kitware.github.io/itk-vtk-viewer/app/) :
 
 <p align="center">
-  <img src="docs/3d_landscape.png" width="300" />
+  <img src="https://github.com/Procuste34/losscape/blob/main/docs/3d_landscape.png?raw=true" width="300" />
 </p>
 
 ## Documentation 📖
 For more details, please refer to the documentation. It provides a global overview on how `losscape` works, and on how you can leverage it with your own model.
-(to be written).
+(to be written : for now you can refer to the code, its simple enough to understand the structure of the library, and you can spin up using the juypter notebook example, all available on the Github repo).
 
 ## References 📚
 - [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913)
 - [Visualizing the Loss Landscape of Winning Lottery Tickets](https://arxiv.org/abs/2112.08538)
 
 
 ## Roadmap 🚀
```

### Comparing `losscape-1.4.1/setup.py` & `losscape-1.4.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.4.1',
+    version='1.4.2',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

