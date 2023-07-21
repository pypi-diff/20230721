# Comparing `tmp/losscape-1.0.tar.gz` & `tmp/losscape-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.0.tar", last modified: Tue Jul 18 12:53:04 2023, max compression
+gzip compressed data, was "losscape-1.1.tar", last modified: Fri Jul 21 07:10:19 2023, max compression
```

## Comparing `losscape-1.0.tar` & `losscape-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 12:53:04.813786 losscape-1.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)      186 2023-07-18 12:53:04.813786 losscape-1.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2791 2023-07-18 12:47:42.000000 losscape-1.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 12:53:04.813786 losscape-1.0/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.0/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.0/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.0/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14961 2023-07-18 12:46:36.000000 losscape-1.0/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1767 2023-07-18 10:09:10.000000 losscape-1.0/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 12:53:04.813786 losscape-1.0/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      186 2023-07-18 12:53:04.000000 losscape-1.0/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-18 12:53:04.000000 losscape-1.0/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-18 12:53:04.000000 losscape-1.0/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-18 12:53:04.000000 losscape-1.0/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-18 12:53:04.000000 losscape-1.0/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-18 12:53:04.813786 losscape-1.0/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      354 2023-07-18 12:45:53.000000 losscape-1.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:10:19.579264 losscape-1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.1/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.1/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.1/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15665 2023-07-21 06:59:27.000000 losscape-1.1/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.1/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:10:19.579264 losscape-1.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:09:32.000000 losscape-1.1/setup.py
```

### Comparing `losscape-1.0/README.md` & `losscape-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,28 @@
 
 train(model, train_loader) # losscape can perform the training for you
 create_2D_losscape(model, train_loader, output_vtp=True)
 ```
 
 Typical results :
 
-
+<p float="left" align="center">
+  <img src="docs/1d_landscape.png" width="400" />
+  <img src="docs/2d_landscape.png" width="400" /> 
+</p>
 
 To visualize the loss landscape in 3D, use the `.vtp` file created by the library and simply drag-and-drop it in [a VTK viewer](https://kitware.github.io/itk-vtk-viewer/app/) :
 
+<p align="center">
+  <img src="docs/3d_landscape.png" width="300" />
+</p>
+
 ## Documentation 📖
 For more details, please refer to the documentation. It provides a global overview on how `losscape` works, and on how you can leverage it with your own model.
+(to be written).
 
 ## References 📚
 - [Visualizing the Loss Landscape of Neural Nets](https://arxiv.org/abs/1712.09913)
 - [Visualizing the Loss Landscape of Winning Lottery Tickets](https://arxiv.org/abs/2112.08538)
 
 
 ## Roadmap 🚀
```

### Comparing `losscape-1.0/losscape/compute_loss.py` & `losscape-1.1/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.0/losscape/create_directions.py` & `losscape-1.1/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.0/losscape/create_landscape.py` & `losscape-1.1/losscape/create_landscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 #todo : plot anim la traj d'une optim avec PCA
 #todo : losscape avec le test loss
 #todo pour la lib : possiblité de tout foutre dans un fichier, et il fait les exps automatiquement ? (genre on met model + dataloader + optim + loss et il loop sur les models + optims)
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
-def create_1D_losscape(model, train_loader_unshuffled, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '1d_losscape.png', x_min:float=-1., x_max:float=1., num_points:int=50):
+def create_2D_losscape(model, train_loader_unshuffled, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '1d_losscape.png', x_min:float=-1., x_max:float=1., num_points:int=50):
     """
-    Create a 1D losscape of the given model.
+    Create a 2D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
     optimizer : the optimizer used for training (should follow the same API as torch optimizers).(default to Adam)
     criterion : the criterion used to compute the loss. (default to F.cross_entropy)
@@ -29,14 +29,16 @@
     output_path : path where the plot will be saved. (default to '1d_losscape.png')
     x_min : min x value (that multiply the sampled direction). (default to -1.) 
     x_max : max x value (that multiply the sampled direction). (default to 1.)
     num_points : number of points to evaluate the loss, from x_min to x_max. (default to 50)
 
     Returns
     ----------
+    coords : numpy array containing the x coords used to create the landscape
+    losses : list of the losses computed
 
     """
 
     model.to(device)
 
     if direction is None:
         direction = create_random_direction(model)
@@ -58,36 +60,47 @@
     plt.savefig(output_path, dpi=300)
 
     if not save_only:
         plt.show()
     
     plt.clf()
 
-def create_2D_losscape(model, train_loader_unshuffled, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '2d_losscape.png', output_vtp:bool = False, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
+    return coords, losses
+
+def create_3D_losscape(model, train_loader_unshuffled, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '2d_losscape.png', output_vtp:bool = False, output_h5:bool = True, log_vtp:bool = True, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
     """
-    Create a 2D losscape of the given model.
+    Create a 3D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
     optimizer : the optimizer used for training (should follow the same API as torch optimizers).(default to Adam)
     criterion : the criterion used to compute the loss. (default to F.cross_entropy)
     num_batches : number of batches to evaluate the model with. (default to 8)
     save_only : only save the plot and don't display it. (default to False)
     output_path : path where the plot will be saved. (default to '1d_losscape.png')
     output_vpt : whether or not to also create a .vtp file, used to 3D visualize the losscape. (default to False)
+    output_h5 : whether or not to also create a .h5 file, containing the data generated by this function (default to True)
+    log_vtp : whether or not to visualize log values of loss in the vtp file (default to True)
     x_min : min x value (that multiply the first sampled direction). (default to -1.) 
     x_max : max x value (that multiply the first sampled direction). (default to 1.)
     y_min : min x value (that multiply the second sampled direction). (default to -1.) 
     y_max : max x value (that multiply the second sampled direction). (default to 1.)
     num_points : number of points to evaluate the loss, from x_min to x_max and y_min to y_max. (default to 50)
 
     Returns
     ----------
+    X : a (num_points, num_points) numpy array, the X meshgrid
+    Y : a (num_points, num_points) numpy array, the Y meshgrid
+    losses : a (num_points, num_points) numpy array containing all the losses computed
+
+    Notes
+    ----------
+    The h5 files is structured as follows :
 
     """
 
     model.to(device)
 
     if directions is None:
         directions = create_random_directions(model)
@@ -112,15 +125,15 @@
 
     if not save_only:
         plt.show()
     
     plt.clf()
 
     if output_vtp:
-        _create_vtp(X, Y, losses)
+        _create_vtp(X, Y, losses, log=log_vtp)
 
 def _set_weights(model, weights, directions, step):
     if len(directions) == 2:
         dx = directions[0]
         dy = directions[1]
         changes = [d0*step[0] + d1*step[1] for (d0, d1) in zip(dx, dy)]
```

### Comparing `losscape-1.0/losscape/train.py` & `losscape-1.1/losscape/train.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 #todo : accuracy + val loss + val acc a la fin ? ou a chaque epoch ?
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
-def train(model, train_loader, optimizer:torch.optim = None, criterion = F.cross_entropy, epochs:int = 50, verbose:int = 1):
+def train(model, train_loader, optimizer:torch.optim = None, criterion = F.cross_entropy, epochs:int = 50, decay_lr_epochs:int = 20, verbose:int = 1):
     """
     Train the provided model.
 
     Parameters
     ----------
     model : the torch model which will be trained.
     train_loader : the torch dataloader which gives training data.
     optimizer : the optimizer used for training (should follow the same API as torch optimizers).(default to Adam)
     criterion : the criterion used to compute the loss. (default to F.cross_entropy)
     epochs : the number of epochs (default to 50)
+    decay_lr_epochs : the lr will be divided by 10 every decay_lr_epochs epochs (default to 20)
     verbose : controls the printing during the training. (0 = print at the end only, 1 = print at 0,25,50,100%, 2 = print every epoch). (default to 1)
 
     Returns
     ----------
 
     """
 
     model.to(device)
 
     if criterion is None:
         criterion = F.cross_entropy
     
     if optimizer is None:
         optimizer = torch.optim.Adam(model.parameters(), lr=0.01)
+        
+    lr = optimizer.param_groups[0]['lr']
 
     for epoch in range(1, epochs+1):
         for batch_idx, (Xb, Yb) in enumerate(train_loader):
             Xb, Yb = Xb.to(device), Yb.to(device)
 
             logits = model(Xb)
             loss = criterion(logits, Yb)
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
+        if epoch%decay_lr_epochs == 0:
+            lr = 0.1 * lr
+            for param_group in optimizer.param_groups:
+                param_group['lr'] = lr
+
         if verbose == 2:
             print("Epoch {}/{}. Loss={}".format(epoch, epochs, loss.item()))
 
         if verbose == 1 and (epoch%(epochs/4) == 0):
             print("Epoch {}/{}. Loss={}".format(epoch, epochs, loss.item()))
 
     if verbose == 0:
```

