# Comparing `tmp/deepliif-1.1.6.tar.gz` & `tmp/deepliif-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepliif-1.1.6.tar", last modified: Mon Mar 20 19:47:47 2023, max compression
+gzip compressed data, was "deepliif-1.1.7.tar", last modified: Fri Jul 21 03:54:16 2023, max compression
```

## Comparing `deepliif-1.1.6.tar` & `deepliif-1.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:47.082852 deepliif-1.1.6/
--rw-rw-rw-   0        0        0      956 2022-11-10 15:00:10.000000 deepliif-1.1.6/LICENSE.md
--rw-rw-rw-   0        0        0    22991 2023-03-20 19:47:47.083852 deepliif-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    22552 2023-03-13 14:58:54.000000 deepliif-1.1.6/README.md
--rw-rw-rw-   0        0        0    40524 2023-03-13 14:59:00.000000 deepliif-1.1.6/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:46.332809 deepliif-1.1.6/deepliif/
--rw-rw-rw-   0        0        0        0 2022-03-16 15:16:26.000000 deepliif-1.1.6/deepliif/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:46.584824 deepliif-1.1.6/deepliif/data/
--rw-rw-rw-   0        0        0     5281 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/__init__.py
--rw-rw-rw-   0        0        0     3045 2023-03-13 14:58:54.000000 deepliif-1.1.6/deepliif/data/aligned_dataset.py
--rw-rw-rw-   0        0        0     5564 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/base_dataset.py
--rw-rw-rw-   0        0        0     2808 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/colorization_dataset.py
--rw-rw-rw-   0        0        0     2006 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/image_folder.py
--rw-rw-rw-   0        0        0     1553 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/single_dataset.py
--rw-rw-rw-   0        0        0     3592 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/template_dataset.py
--rw-rw-rw-   0        0        0     3393 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/data/unaligned_dataset.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:46.749833 deepliif-1.1.6/deepliif/models/
--rw-rw-rw-   0        0        0    20669 2023-03-13 14:58:54.000000 deepliif-1.1.6/deepliif/models/DeepLIIF_model.py
--rw-rw-rw-   0        0        0    17765 2023-03-15 22:08:44.000000 deepliif-1.1.6/deepliif/models/__init__.py
--rw-rw-rw-   0        0        0    12951 2023-03-13 14:59:00.000000 deepliif-1.1.6/deepliif/models/base_model.py
--rw-rw-rw-   0        0        0    32177 2023-03-13 14:58:54.000000 deepliif-1.1.6/deepliif/models/networks.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:46.877841 deepliif-1.1.6/deepliif/options/
--rw-rw-rw-   0        0        0      137 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/options/__init__.py
--rw-rw-rw-   0        0        0     9794 2023-03-13 14:58:54.000000 deepliif-1.1.6/deepliif/options/base_options.py
--rw-rw-rw-   0        0        0     2947 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/options/processing_options.py
--rw-rw-rw-   0        0        0     1114 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/options/test_options.py
--rw-rw-rw-   0        0        0     3580 2023-03-13 14:58:54.000000 deepliif-1.1.6/deepliif/options/train_options.py
--rw-rw-rw-   0        0        0    16985 2023-03-13 14:58:41.000000 deepliif-1.1.6/deepliif/postprocessing.py
--rw-rw-rw-   0        0        0    15757 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/train.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:47.078852 deepliif-1.1.6/deepliif/util/
--rw-rw-rw-   0        0        0    16924 2023-03-15 11:44:25.000000 deepliif-1.1.6/deepliif/util/__init__.py
--rw-rw-rw-   0        0        0     3749 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/util/get_data.py
--rw-rw-rw-   0        0        0     3309 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/util/html.py
--rw-rw-rw-   0        0        0     2280 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/util/image_pool.py
--rw-rw-rw-   0        0        0     4636 2023-03-13 14:58:41.000000 deepliif-1.1.6/deepliif/util/util.py
--rw-rw-rw-   0        0        0    15636 2022-11-10 15:00:10.000000 deepliif-1.1.6/deepliif/util/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:47:46.372812 deepliif-1.1.6/deepliif.egg-info/
--rw-rw-rw-   0        0        0    22991 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      182 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-20 19:47:46.000000 deepliif-1.1.6/deepliif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      230 2023-03-20 19:47:47.094853 deepliif-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-03-20 19:41:59.000000 deepliif-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:16.572807 deepliif-1.1.7/
+-rw-rw-rw-   0        0        0      956 2022-11-10 15:00:10.000000 deepliif-1.1.7/LICENSE.md
+-rw-rw-rw-   0        0        0    23773 2023-07-21 03:54:16.572807 deepliif-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    23334 2023-06-12 15:46:02.000000 deepliif-1.1.7/README.md
+-rw-rw-rw-   0        0        0    40524 2023-03-13 14:59:00.000000 deepliif-1.1.7/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:15.683756 deepliif-1.1.7/deepliif/
+-rw-rw-rw-   0        0        0        0 2022-03-16 15:16:26.000000 deepliif-1.1.7/deepliif/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:16.047777 deepliif-1.1.7/deepliif/data/
+-rw-rw-rw-   0        0        0     5281 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/__init__.py
+-rw-rw-rw-   0        0        0     3045 2023-03-13 14:58:54.000000 deepliif-1.1.7/deepliif/data/aligned_dataset.py
+-rw-rw-rw-   0        0        0     5564 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/base_dataset.py
+-rw-rw-rw-   0        0        0     2808 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/colorization_dataset.py
+-rw-rw-rw-   0        0        0     2006 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/image_folder.py
+-rw-rw-rw-   0        0        0     1553 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/single_dataset.py
+-rw-rw-rw-   0        0        0     3592 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/template_dataset.py
+-rw-rw-rw-   0        0        0     3393 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/data/unaligned_dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:16.146783 deepliif-1.1.7/deepliif/models/
+-rw-rw-rw-   0        0        0    20669 2023-03-13 14:58:54.000000 deepliif-1.1.7/deepliif/models/DeepLIIF_model.py
+-rw-rw-rw-   0        0        0    17778 2023-07-21 03:45:52.000000 deepliif-1.1.7/deepliif/models/__init__.py
+-rw-rw-rw-   0        0        0    12951 2023-03-13 14:59:00.000000 deepliif-1.1.7/deepliif/models/base_model.py
+-rw-rw-rw-   0        0        0    32177 2023-03-13 14:58:54.000000 deepliif-1.1.7/deepliif/models/networks.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:16.312792 deepliif-1.1.7/deepliif/options/
+-rw-rw-rw-   0        0        0      137 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/options/__init__.py
+-rw-rw-rw-   0        0        0     9794 2023-03-13 14:58:54.000000 deepliif-1.1.7/deepliif/options/base_options.py
+-rw-rw-rw-   0        0        0     2947 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/options/processing_options.py
+-rw-rw-rw-   0        0        0     1114 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/options/test_options.py
+-rw-rw-rw-   0        0        0     3580 2023-03-13 14:58:54.000000 deepliif-1.1.7/deepliif/options/train_options.py
+-rw-rw-rw-   0        0        0    16985 2023-03-13 14:58:41.000000 deepliif-1.1.7/deepliif/postprocessing.py
+-rw-rw-rw-   0        0        0    15757 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/train.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:16.567807 deepliif-1.1.7/deepliif/util/
+-rw-rw-rw-   0        0        0    16924 2023-03-15 11:44:25.000000 deepliif-1.1.7/deepliif/util/__init__.py
+-rw-rw-rw-   0        0        0     3749 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/util/get_data.py
+-rw-rw-rw-   0        0        0     3309 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/util/html.py
+-rw-rw-rw-   0        0        0     2280 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/util/image_pool.py
+-rw-rw-rw-   0        0        0     4636 2023-03-13 14:58:41.000000 deepliif-1.1.7/deepliif/util/util.py
+-rw-rw-rw-   0        0        0    15636 2022-11-10 15:00:10.000000 deepliif-1.1.7/deepliif/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:54:15.737759 deepliif-1.1.7/deepliif.egg-info/
+-rw-rw-rw-   0        0        0    23773 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      182 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 03:54:14.000000 deepliif-1.1.7/deepliif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      230 2023-07-21 03:54:16.576808 deepliif-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-07-21 03:50:48.000000 deepliif-1.1.7/setup.py
```

### Comparing `deepliif-1.1.6/LICENSE.md` & `deepliif-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/PKG-INFO` & `deepliif-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepliif
-Version: 1.1.6
+Version: 1.1.7
 Summary: DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification
 Home-page: https://github.com/nadeemlab/DeepLIIF
 Author: Parmida93
 Author-email: ghahremani.parmida@gmail.com
 Keywords: DeepLIIF,IHC,Segmentation,Classification
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,28 +12,24 @@
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
     <img src="./images/DeepLIIF_logo.png" width="50%">
     <h3 align="center"><strong>Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification</strong></h3>
     <p align="center">
-    <a href="https://doi.org/10.1101/2021.05.01.442219">Journal Preprint</a>
+    <a href="https://rdcu.be/cKSBz">Nature MI'22 Link</a>
     |
-    <a href="https://rdcu.be/cKSBz">Journal Link</a>
+    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR'22 Link</a>
     |
-    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR Link</a>
+    <a href="https://arxiv.org/abs/2305.16465">MICCAI'23 link</a>
     |
     <a href="https://deepliif.org/">Cloud Deployment</a>
     |
     <a href="https://nadeemlab.github.io/DeepLIIF/">Documentation</a>
     |
-    <a href="#docker">Docker</a>
-    |
-    <a href="https://github.com/nadeemlab/DeepLIIF/tree/main/ImageJ_Plugin">ImageJ Plugin</a>
-    |
     <a href="#support">Support</a>
   </p>
 </p>
 
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of tissue is broadly used in diagnostic 
 pathology laboratories for patient care. To date, clinical reporting is predominantly qualitative or semi-quantitative. 
 By creating a multitask deep learning framework referred to as DeepLIIF, we present a single-step solution to stain 
@@ -352,28 +348,31 @@
 
 We are also creating a self-configurable version of DeepLIIF which will take as input any co-registered H&E/IHC and 
 multiplex images and produce the optimal output. If you are generating or have generated H&E/IHC and multiplex staining 
 for the same slide (de novo staining) and would like to contribute that data for DeepLIIF, we can perform 
 co-registration, whole-cell multiplex segmentation via [ImPartial](https://github.com/nadeemlab/ImPartial), train the 
 DeepLIIF model and release back to the community with full credit to the contributors.
 
+- [x] **Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and multiplex immunofluorescence dataset](https://zenodo.org/record/4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine Intelligence'22**)
+- [x] **Moffitt Cancer Center** AI-ready multiplex immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck squamous cell carcinoma (**MICCAI'23**)   
+
 ## Support
 Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif) for discussion and questions related to DeepLIIF.
 
 Bugs can be reported in the [GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab.
 
 ## License
 Â© [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons Clause** license, 
 and is available for non-commercial academic purposes. 
 
 ## Acknowledgments
 * This code is inspired by [CycleGAN and pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
 
 ## Reference
-If you find our work useful in your research or if you use parts of this code, please cite our paper:
+If you find our work useful in your research or if you use parts of this code or our released dataset, please cite the following papers:
 ```
 @article{ghahremani2022deep,
   title={Deep learning-inferred multiplex immunofluorescence for immunohistochemical image quantification},
   author={Ghahremani, Parmida and Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann, Travis J and Nadeem, Saad},
   journal={Nature Machine Intelligence},
   volume={4},
   number={4},
@@ -386,8 +385,14 @@
   title={DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
   author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem, Saad},
   journal={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
   pages={21399--21405},
   year={2022}
 }
 
+@article{ghahremani2023deepliifdataset,
+  title={An AI-Ready Multiplex Staining Dataset for Reproducible and Accurate Characterization of Tumor Immune Microenvironment},
+  author={Ghahremani, Parmida and Marino, Joseph and Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H. Chung, Christine and Nadeem, Saad},
+  journal={International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI)},
+  year={2023}
+}
 ```
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: deepliif Version: 1.1.6 Summary: DeepLIIF: Deep-
+Metadata-Version: 2.1 Name: deepliif Version: 1.1.7 Summary: DeepLIIF: Deep-
 Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image
 Quantification Home-page: https://github.com/nadeemlab/DeepLIIF Author:
 Parmida93 Author-email: ghahremani.parmida@gmail.com Keywords:
 DeepLIIF,IHC,Segmentation,Classification Description-Content-Type: text/
 markdown License-File: LICENSE.md
                          [./images/DeepLIIF_logo.png]
          **** Deep-Learning Inferred Multiplex Immunofluorescence for
                  Immunohistochemical Image Quantification ****
-Journal_Preprint | Journal_Link | CVPR_Link | Cloud_Deployment | Documentation
-                      | Docker | ImageJ_Plugin | Support
+    Nature_MI'22_Link | CVPR'22_Link | MICCAI'23_link | Cloud_Deployment |
+                            Documentation | Support
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of
 tissue is broadly used in diagnostic pathology laboratories for patient care.
 To date, clinical reporting is predominantly qualitative or semi-quantitative.
 By creating a multitask deep learning framework referred to as DeepLIIF, we
 present a single-step solution to stain deconvolution/separation, cell
 segmentation, and quantitative single-cell IHC scoring. Leveraging a unique de
 novo dataset of co-registered IHC and multiplex immunofluorescence (mpIF)
@@ -258,27 +258,40 @@
 this dataset [here](https://zenodo.org/record/4751737#.YKRTS0NKhH4). We are
 also creating a self-configurable version of DeepLIIF which will take as input
 any co-registered H&E/IHC and multiplex images and produce the optimal output.
 If you are generating or have generated H&E/IHC and multiplex staining for the
 same slide (de novo staining) and would like to contribute that data for
 DeepLIIF, we can perform co-registration, whole-cell multiplex segmentation via
 [ImPartial](https://github.com/nadeemlab/ImPartial), train the DeepLIIF model
-and release back to the community with full credit to the contributors. ##
-Support Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif)
-for discussion and questions related to DeepLIIF. Bugs can be reported in the
-[GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab. ## License
-ÃÂ© [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under
-**Apache 2.0 with Commons Clause** license, and is available for non-commercial
-academic purposes. ## Acknowledgments * This code is inspired by [CycleGAN and
-pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
-## Reference If you find our work useful in your research or if you use parts
-of this code, please cite our paper: ``` @article{ghahremani2022deep, title=
-{Deep learning-inferred multiplex immunofluorescence for immunohistochemical
-image quantification}, author={Ghahremani, Parmida and Li, Yanyun and Kaufman,
-Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann,
-Travis J and Nadeem, Saad}, journal={Nature Machine Intelligence}, volume={4},
-number={4}, pages={401--412}, year={2022}, publisher={Nature Publishing Group}
-} @article{ghahremani2022deepliifui, title={DeepLIIF: An Online Platform for
-Quantification of Clinical Pathology Slides}, author={Ghahremani, Parmida and
-Marino, Joseph and Dodds, Ricardo and Nadeem, Saad}, journal={Proceedings of
-the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
-pages={21399--21405}, year={2022} } ```
+and release back to the community with full credit to the contributors. - [x]
+**Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and
+multiplex immunofluorescence dataset](https://zenodo.org/record/
+4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine
+Intelligence'22**) - [x] **Moffitt Cancer Center** AI-ready multiplex
+immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck
+squamous cell carcinoma (**MICCAI'23**) ## Support Please use the [Image.sc
+Forum](https://forum.image.sc/tag/deepliif) for discussion and questions
+related to DeepLIIF. Bugs can be reported in the [GitHub Issues](https://
+github.com/nadeemlab/DeepLIIF/issues) tab. ## License ÃÂ© [Nadeem Lab](https:/
+/nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons
+Clause** license, and is available for non-commercial academic purposes. ##
+Acknowledgments * This code is inspired by [CycleGAN and pix2pix in PyTorch]
+(https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix). ## Reference If you
+find our work useful in your research or if you use parts of this code or our
+released dataset, please cite the following papers: ``` @article
+{ghahremani2022deep, title={Deep learning-inferred multiplex immunofluorescence
+for immunohistochemical image quantification}, author={Ghahremani, Parmida and
+Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo,
+Michael and Hollmann, Travis J and Nadeem, Saad}, journal={Nature Machine
+Intelligence}, volume={4}, number={4}, pages={401--412}, year={2022},
+publisher={Nature Publishing Group} } @article{ghahremani2022deepliifui, title=
+{DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
+author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem,
+Saad}, journal={Proceedings of the IEEE/CVF Conference on Computer Vision and
+Pattern Recognition (CVPR)}, pages={21399--21405}, year={2022} } @article
+{ghahremani2023deepliifdataset, title={An AI-Ready Multiplex Staining Dataset
+for Reproducible and Accurate Characterization of Tumor Immune
+Microenvironment}, author={Ghahremani, Parmida and Marino, Joseph and
+Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H.
+Chung, Christine and Nadeem, Saad}, journal={International Conference on
+Medical Image Computing and Computer-Assisted Intervention (MICCAI)}, year=
+{2023} } ```
```

### Comparing `deepliif-1.1.6/README.md` & `deepliif-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
     <img src="./images/DeepLIIF_logo.png" width="50%">
     <h3 align="center"><strong>Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification</strong></h3>
     <p align="center">
-    <a href="https://doi.org/10.1101/2021.05.01.442219">Journal Preprint</a>
+    <a href="https://rdcu.be/cKSBz">Nature MI'22 Link</a>
     |
-    <a href="https://rdcu.be/cKSBz">Journal Link</a>
+    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR'22 Link</a>
     |
-    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR Link</a>
+    <a href="https://arxiv.org/abs/2305.16465">MICCAI'23 link</a>
     |
     <a href="https://deepliif.org/">Cloud Deployment</a>
     |
     <a href="https://nadeemlab.github.io/DeepLIIF/">Documentation</a>
     |
-    <a href="#docker">Docker</a>
-    |
-    <a href="https://github.com/nadeemlab/DeepLIIF/tree/main/ImageJ_Plugin">ImageJ Plugin</a>
-    |
     <a href="#support">Support</a>
   </p>
 </p>
 
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of tissue is broadly used in diagnostic 
 pathology laboratories for patient care. To date, clinical reporting is predominantly qualitative or semi-quantitative. 
 By creating a multitask deep learning framework referred to as DeepLIIF, we present a single-step solution to stain 
@@ -341,28 +337,31 @@
 
 We are also creating a self-configurable version of DeepLIIF which will take as input any co-registered H&E/IHC and 
 multiplex images and produce the optimal output. If you are generating or have generated H&E/IHC and multiplex staining 
 for the same slide (de novo staining) and would like to contribute that data for DeepLIIF, we can perform 
 co-registration, whole-cell multiplex segmentation via [ImPartial](https://github.com/nadeemlab/ImPartial), train the 
 DeepLIIF model and release back to the community with full credit to the contributors.
 
+- [x] **Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and multiplex immunofluorescence dataset](https://zenodo.org/record/4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine Intelligence'22**)
+- [x] **Moffitt Cancer Center** AI-ready multiplex immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck squamous cell carcinoma (**MICCAI'23**)   
+
 ## Support
 Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif) for discussion and questions related to DeepLIIF.
 
 Bugs can be reported in the [GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab.
 
 ## License
 © [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons Clause** license, 
 and is available for non-commercial academic purposes. 
 
 ## Acknowledgments
 * This code is inspired by [CycleGAN and pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
 
 ## Reference
-If you find our work useful in your research or if you use parts of this code, please cite our paper:
+If you find our work useful in your research or if you use parts of this code or our released dataset, please cite the following papers:
 ```
 @article{ghahremani2022deep,
   title={Deep learning-inferred multiplex immunofluorescence for immunohistochemical image quantification},
   author={Ghahremani, Parmida and Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann, Travis J and Nadeem, Saad},
   journal={Nature Machine Intelligence},
   volume={4},
   number={4},
@@ -375,8 +374,14 @@
   title={DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
   author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem, Saad},
   journal={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
   pages={21399--21405},
   year={2022}
 }
 
+@article{ghahremani2023deepliifdataset,
+  title={An AI-Ready Multiplex Staining Dataset for Reproducible and Accurate Characterization of Tumor Immune Microenvironment},
+  author={Ghahremani, Parmida and Marino, Joseph and Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H. Chung, Christine and Nadeem, Saad},
+  journal={International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI)},
+  year={2023}
+}
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
                          [./images/DeepLIIF_logo.png]
          **** Deep-Learning Inferred Multiplex Immunofluorescence for
                  Immunohistochemical Image Quantification ****
-Journal_Preprint | Journal_Link | CVPR_Link | Cloud_Deployment | Documentation
-                      | Docker | ImageJ_Plugin | Support
+    Nature_MI'22_Link | CVPR'22_Link | MICCAI'23_link | Cloud_Deployment |
+                            Documentation | Support
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of
 tissue is broadly used in diagnostic pathology laboratories for patient care.
 To date, clinical reporting is predominantly qualitative or semi-quantitative.
 By creating a multitask deep learning framework referred to as DeepLIIF, we
 present a single-step solution to stain deconvolution/separation, cell
 segmentation, and quantitative single-cell IHC scoring. Leveraging a unique de
 novo dataset of co-registered IHC and multiplex immunofluorescence (mpIF)
@@ -252,27 +252,40 @@
 this dataset [here](https://zenodo.org/record/4751737#.YKRTS0NKhH4). We are
 also creating a self-configurable version of DeepLIIF which will take as input
 any co-registered H&E/IHC and multiplex images and produce the optimal output.
 If you are generating or have generated H&E/IHC and multiplex staining for the
 same slide (de novo staining) and would like to contribute that data for
 DeepLIIF, we can perform co-registration, whole-cell multiplex segmentation via
 [ImPartial](https://github.com/nadeemlab/ImPartial), train the DeepLIIF model
-and release back to the community with full credit to the contributors. ##
-Support Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif)
-for discussion and questions related to DeepLIIF. Bugs can be reported in the
-[GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab. ## License
-Â© [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under
-**Apache 2.0 with Commons Clause** license, and is available for non-commercial
-academic purposes. ## Acknowledgments * This code is inspired by [CycleGAN and
-pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
-## Reference If you find our work useful in your research or if you use parts
-of this code, please cite our paper: ``` @article{ghahremani2022deep, title=
-{Deep learning-inferred multiplex immunofluorescence for immunohistochemical
-image quantification}, author={Ghahremani, Parmida and Li, Yanyun and Kaufman,
-Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann,
-Travis J and Nadeem, Saad}, journal={Nature Machine Intelligence}, volume={4},
-number={4}, pages={401--412}, year={2022}, publisher={Nature Publishing Group}
-} @article{ghahremani2022deepliifui, title={DeepLIIF: An Online Platform for
-Quantification of Clinical Pathology Slides}, author={Ghahremani, Parmida and
-Marino, Joseph and Dodds, Ricardo and Nadeem, Saad}, journal={Proceedings of
-the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
-pages={21399--21405}, year={2022} } ```
+and release back to the community with full credit to the contributors. - [x]
+**Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and
+multiplex immunofluorescence dataset](https://zenodo.org/record/
+4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine
+Intelligence'22**) - [x] **Moffitt Cancer Center** AI-ready multiplex
+immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck
+squamous cell carcinoma (**MICCAI'23**) ## Support Please use the [Image.sc
+Forum](https://forum.image.sc/tag/deepliif) for discussion and questions
+related to DeepLIIF. Bugs can be reported in the [GitHub Issues](https://
+github.com/nadeemlab/DeepLIIF/issues) tab. ## License Â© [Nadeem Lab](https://
+nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons
+Clause** license, and is available for non-commercial academic purposes. ##
+Acknowledgments * This code is inspired by [CycleGAN and pix2pix in PyTorch]
+(https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix). ## Reference If you
+find our work useful in your research or if you use parts of this code or our
+released dataset, please cite the following papers: ``` @article
+{ghahremani2022deep, title={Deep learning-inferred multiplex immunofluorescence
+for immunohistochemical image quantification}, author={Ghahremani, Parmida and
+Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo,
+Michael and Hollmann, Travis J and Nadeem, Saad}, journal={Nature Machine
+Intelligence}, volume={4}, number={4}, pages={401--412}, year={2022},
+publisher={Nature Publishing Group} } @article{ghahremani2022deepliifui, title=
+{DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
+author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem,
+Saad}, journal={Proceedings of the IEEE/CVF Conference on Computer Vision and
+Pattern Recognition (CVPR)}, pages={21399--21405}, year={2022} } @article
+{ghahremani2023deepliifdataset, title={An AI-Ready Multiplex Staining Dataset
+for Reproducible and Accurate Characterization of Tumor Immune
+Microenvironment}, author={Ghahremani, Parmida and Marino, Joseph and
+Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H.
+Chung, Christine and Nadeem, Saad}, journal={International Conference on
+Medical Image Computing and Computer-Assisted Intervention (MICCAI)}, year=
+{2023} } ```
```

### Comparing `deepliif-1.1.6/cli.py` & `deepliif-1.1.7/cli.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/__init__.py` & `deepliif-1.1.7/deepliif/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/aligned_dataset.py` & `deepliif-1.1.7/deepliif/data/aligned_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/base_dataset.py` & `deepliif-1.1.7/deepliif/data/base_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/colorization_dataset.py` & `deepliif-1.1.7/deepliif/data/colorization_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/image_folder.py` & `deepliif-1.1.7/deepliif/data/image_folder.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/single_dataset.py` & `deepliif-1.1.7/deepliif/data/single_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/template_dataset.py` & `deepliif-1.1.7/deepliif/data/template_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/data/unaligned_dataset.py` & `deepliif-1.1.7/deepliif/data/unaligned_dataset.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/models/DeepLIIF_model.py` & `deepliif-1.1.7/deepliif/models/DeepLIIF_model.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/models/__init__.py` & `deepliif-1.1.7/deepliif/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     images['Lap2'] = create_image_for_stitching(tile_size, rows, cols)
     images['Marker'] = create_image_for_stitching(tile_size, rows, cols)
     images['Seg'] = create_image_for_stitching(tile_size, rows, cols)
 
     for i in range(cols):
         for j in range(rows):
             tile = extract_tile(rescaled, tile_size, overlap_size, i, j)
-            res = run_fn(tile, model_path, eager_mode)
+            res = run_wrapper(tile, run_fn, model_path, eager_mode)
 
             stitch_tile(images['Hema'], res['G1'], tile_size, overlap_size, i, j)
             stitch_tile(images['DAPI'], res['G2'], tile_size, overlap_size, i, j)
             stitch_tile(images['Lap2'], res['G3'], tile_size, overlap_size, i, j)
             stitch_tile(images['Marker'], res['G4'], tile_size, overlap_size, i, j)
             stitch_tile(images['Seg'], res['G5'], tile_size, overlap_size, i, j)
```

### Comparing `deepliif-1.1.6/deepliif/models/base_model.py` & `deepliif-1.1.7/deepliif/models/base_model.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/models/networks.py` & `deepliif-1.1.7/deepliif/models/networks.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/options/base_options.py` & `deepliif-1.1.7/deepliif/options/base_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/options/processing_options.py` & `deepliif-1.1.7/deepliif/options/processing_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/options/test_options.py` & `deepliif-1.1.7/deepliif/options/test_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/options/train_options.py` & `deepliif-1.1.7/deepliif/options/train_options.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/postprocessing.py` & `deepliif-1.1.7/deepliif/postprocessing.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/train.py` & `deepliif-1.1.7/deepliif/train.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/__init__.py` & `deepliif-1.1.7/deepliif/util/__init__.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/get_data.py` & `deepliif-1.1.7/deepliif/util/get_data.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/html.py` & `deepliif-1.1.7/deepliif/util/html.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/image_pool.py` & `deepliif-1.1.7/deepliif/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/util.py` & `deepliif-1.1.7/deepliif/util/util.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif/util/visualizer.py` & `deepliif-1.1.7/deepliif/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/deepliif.egg-info/PKG-INFO` & `deepliif-1.1.7/deepliif.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepliif
-Version: 1.1.6
+Version: 1.1.7
 Summary: DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification
 Home-page: https://github.com/nadeemlab/DeepLIIF
 Author: Parmida93
 Author-email: ghahremani.parmida@gmail.com
 Keywords: DeepLIIF,IHC,Segmentation,Classification
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -12,28 +12,24 @@
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
     <img src="./images/DeepLIIF_logo.png" width="50%">
     <h3 align="center"><strong>Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification</strong></h3>
     <p align="center">
-    <a href="https://doi.org/10.1101/2021.05.01.442219">Journal Preprint</a>
+    <a href="https://rdcu.be/cKSBz">Nature MI'22 Link</a>
     |
-    <a href="https://rdcu.be/cKSBz">Journal Link</a>
+    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR'22 Link</a>
     |
-    <a href="https://openaccess.thecvf.com/content/CVPR2022/html/Ghahremani_DeepLIIF_An_Online_Platform_for_Quantification_of_Clinical_Pathology_Slides_CVPR_2022_paper.html">CVPR Link</a>
+    <a href="https://arxiv.org/abs/2305.16465">MICCAI'23 link</a>
     |
     <a href="https://deepliif.org/">Cloud Deployment</a>
     |
     <a href="https://nadeemlab.github.io/DeepLIIF/">Documentation</a>
     |
-    <a href="#docker">Docker</a>
-    |
-    <a href="https://github.com/nadeemlab/DeepLIIF/tree/main/ImageJ_Plugin">ImageJ Plugin</a>
-    |
     <a href="#support">Support</a>
   </p>
 </p>
 
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of tissue is broadly used in diagnostic 
 pathology laboratories for patient care. To date, clinical reporting is predominantly qualitative or semi-quantitative. 
 By creating a multitask deep learning framework referred to as DeepLIIF, we present a single-step solution to stain 
@@ -352,28 +348,31 @@
 
 We are also creating a self-configurable version of DeepLIIF which will take as input any co-registered H&E/IHC and 
 multiplex images and produce the optimal output. If you are generating or have generated H&E/IHC and multiplex staining 
 for the same slide (de novo staining) and would like to contribute that data for DeepLIIF, we can perform 
 co-registration, whole-cell multiplex segmentation via [ImPartial](https://github.com/nadeemlab/ImPartial), train the 
 DeepLIIF model and release back to the community with full credit to the contributors.
 
+- [x] **Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and multiplex immunofluorescence dataset](https://zenodo.org/record/4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine Intelligence'22**)
+- [x] **Moffitt Cancer Center** AI-ready multiplex immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck squamous cell carcinoma (**MICCAI'23**)   
+
 ## Support
 Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif) for discussion and questions related to DeepLIIF.
 
 Bugs can be reported in the [GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab.
 
 ## License
 Â© [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons Clause** license, 
 and is available for non-commercial academic purposes. 
 
 ## Acknowledgments
 * This code is inspired by [CycleGAN and pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
 
 ## Reference
-If you find our work useful in your research or if you use parts of this code, please cite our paper:
+If you find our work useful in your research or if you use parts of this code or our released dataset, please cite the following papers:
 ```
 @article{ghahremani2022deep,
   title={Deep learning-inferred multiplex immunofluorescence for immunohistochemical image quantification},
   author={Ghahremani, Parmida and Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann, Travis J and Nadeem, Saad},
   journal={Nature Machine Intelligence},
   volume={4},
   number={4},
@@ -386,8 +385,14 @@
   title={DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
   author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem, Saad},
   journal={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
   pages={21399--21405},
   year={2022}
 }
 
+@article{ghahremani2023deepliifdataset,
+  title={An AI-Ready Multiplex Staining Dataset for Reproducible and Accurate Characterization of Tumor Immune Microenvironment},
+  author={Ghahremani, Parmida and Marino, Joseph and Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H. Chung, Christine and Nadeem, Saad},
+  journal={International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI)},
+  year={2023}
+}
 ```
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: deepliif Version: 1.1.6 Summary: DeepLIIF: Deep-
+Metadata-Version: 2.1 Name: deepliif Version: 1.1.7 Summary: DeepLIIF: Deep-
 Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image
 Quantification Home-page: https://github.com/nadeemlab/DeepLIIF Author:
 Parmida93 Author-email: ghahremani.parmida@gmail.com Keywords:
 DeepLIIF,IHC,Segmentation,Classification Description-Content-Type: text/
 markdown License-File: LICENSE.md
                          [./images/DeepLIIF_logo.png]
          **** Deep-Learning Inferred Multiplex Immunofluorescence for
                  Immunohistochemical Image Quantification ****
-Journal_Preprint | Journal_Link | CVPR_Link | Cloud_Deployment | Documentation
-                      | Docker | ImageJ_Plugin | Support
+    Nature_MI'22_Link | CVPR'22_Link | MICCAI'23_link | Cloud_Deployment |
+                            Documentation | Support
 *Reporting biomarkers assessed by routine immunohistochemical (IHC) staining of
 tissue is broadly used in diagnostic pathology laboratories for patient care.
 To date, clinical reporting is predominantly qualitative or semi-quantitative.
 By creating a multitask deep learning framework referred to as DeepLIIF, we
 present a single-step solution to stain deconvolution/separation, cell
 segmentation, and quantitative single-cell IHC scoring. Leveraging a unique de
 novo dataset of co-registered IHC and multiplex immunofluorescence (mpIF)
@@ -258,27 +258,40 @@
 this dataset [here](https://zenodo.org/record/4751737#.YKRTS0NKhH4). We are
 also creating a self-configurable version of DeepLIIF which will take as input
 any co-registered H&E/IHC and multiplex images and produce the optimal output.
 If you are generating or have generated H&E/IHC and multiplex staining for the
 same slide (de novo staining) and would like to contribute that data for
 DeepLIIF, we can perform co-registration, whole-cell multiplex segmentation via
 [ImPartial](https://github.com/nadeemlab/ImPartial), train the DeepLIIF model
-and release back to the community with full credit to the contributors. ##
-Support Please use the [Image.sc Forum](https://forum.image.sc/tag/deepliif)
-for discussion and questions related to DeepLIIF. Bugs can be reported in the
-[GitHub Issues](https://github.com/nadeemlab/DeepLIIF/issues) tab. ## License
-ÃÂ© [Nadeem Lab](https://nadeemlab.org/) - DeepLIIF code is distributed under
-**Apache 2.0 with Commons Clause** license, and is available for non-commercial
-academic purposes. ## Acknowledgments * This code is inspired by [CycleGAN and
-pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
-## Reference If you find our work useful in your research or if you use parts
-of this code, please cite our paper: ``` @article{ghahremani2022deep, title=
-{Deep learning-inferred multiplex immunofluorescence for immunohistochemical
-image quantification}, author={Ghahremani, Parmida and Li, Yanyun and Kaufman,
-Arie and Vanguri, Rami and Greenwald, Noah and Angelo, Michael and Hollmann,
-Travis J and Nadeem, Saad}, journal={Nature Machine Intelligence}, volume={4},
-number={4}, pages={401--412}, year={2022}, publisher={Nature Publishing Group}
-} @article{ghahremani2022deepliifui, title={DeepLIIF: An Online Platform for
-Quantification of Clinical Pathology Slides}, author={Ghahremani, Parmida and
-Marino, Joseph and Dodds, Ricardo and Nadeem, Saad}, journal={Proceedings of
-the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
-pages={21399--21405}, year={2022} } ```
+and release back to the community with full credit to the contributors. - [x]
+**Memorial Sloan Kettering Cancer Center** [AI-ready immunohistochemistry and
+multiplex immunofluorescence dataset](https://zenodo.org/record/
+4751737#.YKRTS0NKhH4) for breast, lung, and bladder cancers (**Nature Machine
+Intelligence'22**) - [x] **Moffitt Cancer Center** AI-ready multiplex
+immunofluorescence and multiplex immunohistochemistry dataset for head-and-neck
+squamous cell carcinoma (**MICCAI'23**) ## Support Please use the [Image.sc
+Forum](https://forum.image.sc/tag/deepliif) for discussion and questions
+related to DeepLIIF. Bugs can be reported in the [GitHub Issues](https://
+github.com/nadeemlab/DeepLIIF/issues) tab. ## License ÃÂ© [Nadeem Lab](https:/
+/nadeemlab.org/) - DeepLIIF code is distributed under **Apache 2.0 with Commons
+Clause** license, and is available for non-commercial academic purposes. ##
+Acknowledgments * This code is inspired by [CycleGAN and pix2pix in PyTorch]
+(https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix). ## Reference If you
+find our work useful in your research or if you use parts of this code or our
+released dataset, please cite the following papers: ``` @article
+{ghahremani2022deep, title={Deep learning-inferred multiplex immunofluorescence
+for immunohistochemical image quantification}, author={Ghahremani, Parmida and
+Li, Yanyun and Kaufman, Arie and Vanguri, Rami and Greenwald, Noah and Angelo,
+Michael and Hollmann, Travis J and Nadeem, Saad}, journal={Nature Machine
+Intelligence}, volume={4}, number={4}, pages={401--412}, year={2022},
+publisher={Nature Publishing Group} } @article{ghahremani2022deepliifui, title=
+{DeepLIIF: An Online Platform for Quantification of Clinical Pathology Slides},
+author={Ghahremani, Parmida and Marino, Joseph and Dodds, Ricardo and Nadeem,
+Saad}, journal={Proceedings of the IEEE/CVF Conference on Computer Vision and
+Pattern Recognition (CVPR)}, pages={21399--21405}, year={2022} } @article
+{ghahremani2023deepliifdataset, title={An AI-Ready Multiplex Staining Dataset
+for Reproducible and Accurate Characterization of Tumor Immune
+Microenvironment}, author={Ghahremani, Parmida and Marino, Joseph and
+Hernandez-Prera, Juan and V. de la Iglesia, Janis and JC Slebos, Robbert and H.
+Chung, Christine and Nadeem, Saad}, journal={International Conference on
+Medical Image Computing and Computer-Assisted Intervention (MICCAI)}, year=
+{2023} } ```
```

### Comparing `deepliif-1.1.6/deepliif.egg-info/SOURCES.txt` & `deepliif-1.1.7/deepliif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepliif-1.1.6/setup.py` & `deepliif-1.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='deepliif',
-    version='1.1.6',
+    version='1.1.7',
     packages=['deepliif', 'deepliif.data', 'deepliif.models', 'deepliif.util', 'deepliif.options'],
 
     description='DeepLIIF: Deep-Learning Inferred Multiplex Immunofluorescence for Immunohistochemical Image Quantification',
     author='Parmida93',
     author_email='ghahremani.parmida@gmail.com',
     url='https://github.com/nadeemlab/DeepLIIF',
     long_description=README,
```

