# Comparing `tmp/vl_datasets-0.0.5-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.6-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 12624 bytes, number of entries: 8
--rw-r--r--  2.0 unx       99 b- defN 23-May-15 06:06 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     4734 b- defN 23-May-15 06:06 vl_datasets/food101.py
--rw-r--r--  2.0 unx     2352 b- defN 23-May-15 06:06 vl_datasets/image_folder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    16358 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      650 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/RECORD
-8 files, 35670 bytes uncompressed, 11492 bytes compressed:  67.8%
+Zip file size: 15132 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      141 b- defN 23-May-16 11:04 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     4734 b- defN 23-May-16 11:04 vl_datasets/food101.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-16 11:04 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx     4823 b- defN 23-May-16 11:04 vl_datasets/oxford_pet.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-16 11:04 vl_datasets/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17100 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/RECORD
+10 files, 42493 bytes uncompressed, 13758 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -3,23 +3,29 @@
 
 Filename: vl_datasets/food101.py
 Comment: 
 
 Filename: vl_datasets/image_folder.py
 Comment: 
 
-Filename: vl_datasets-0.0.5.dist-info/LICENSE
+Filename: vl_datasets/oxford_pet.py
 Comment: 
 
-Filename: vl_datasets-0.0.5.dist-info/METADATA
+Filename: vl_datasets/utils.py
 Comment: 
 
-Filename: vl_datasets-0.0.5.dist-info/WHEEL
+Filename: vl_datasets-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.5.dist-info/top_level.txt
+Filename: vl_datasets-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.5.dist-info/RECORD
+Filename: vl_datasets-0.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: vl_datasets-0.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: vl_datasets-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,3 +1,4 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 from .image_folder import CleanImageFolder
 from .food101 import CleanFood101
+from .oxford_pet import CleanOxfordIIITPet
```

## Comparing `vl_datasets-0.0.5.dist-info/LICENSE` & `vl_datasets-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.5.dist-info/METADATA` & `vl_datasets-0.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -55,15 +55,15 @@
 <br />
 <div align="center">
 
 <a href="https://www.visual-layer.com">
   <img alt="Visual Layer Logo" src="https://raw.githubusercontent.com/visual-layer/fastdup/main/gallery/visual_layer_logo.png" alt="Logo" width="400">
 </a>
 
-<h3 align="center">Open, Clean Datasets for Computer Vision</h3>
+<h3 align="center">Open, Clean, Curated Datasets for Computer Vision</h3>
 
   <p align="center">
   <br />
     🔥 We use
     <a href="https://github.com/visual-layer/fastdup">fastdup</a> - a free tool to clean all datasets shared in this repo.
     <br />
     <a href="https://visual-layer.readme.io/" target="_blank" rel="noopener noreferrer"><strong>Explore the docs »</strong></a>
@@ -93,24 +93,39 @@
     <img src="https://img.shields.io/badge/-YouTube-black.svg?style=for-the-badge&logo=youtube&colorB=red" alt="Logo">
     </a>
   </p>
 </div>
 
 ## Description
 
-`vl-datasets` is a collection of clean computer vision datasets, carefully analyzed and processed to avoid common image dataset issues such as:
+`vl-datasets` is a Python package that provides access to clean computer vision datasets with only 2 lines of code.
+
+For example, to get access to the clean version of the [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) dataset simply run:
+
+![image](./imgs/usage.png)
+
+We support some of the most widely used computer vision datasets.
+[Let us know](https://forms.gle/8jxPkyzeKj82kPed8) if you have additional request to support a new dataset.
+
+All the datasets are analyzed for issues such as: 
 
 + Duplicates.
 + Broken images.
 + Outliers.
 + Dark/Bright/Blurry images.
 
-For each dataset in this repo, we provide a `.csv` file that lists the problematic images from the dataset.
+![image](./imgs/issues.png)
+
+`vl-datasets` provides a convenient way to access these cleaned datasets in Python.
+
+Alternatively, for each dataset in this repo, we provide a `.csv` file that lists the problematic images from the dataset.
+
 You can use the listed images in the `.csv` to improve the model by re-labeling the them or just simply remove it from the dataset.
 
+
 ## Why?
 
 Computer vision is an exciting and rapidly advancing field, with new techniques and models emerging now and then. 
 However, to develop and evaluate these models, it's essential to have reliable and standardized datasets to work with.
 
 Even with the recent success of generative models, data quality remains an issue that's [mainly overlooked](https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-e3ea4c9e8d22).
 Training models will erroneours data impacts model accuracy, incurs costs in time, storage and computational resources.
@@ -118,81 +133,78 @@
 We believe that access to clean and high-quality computer vision datasets leads to accurate, non-biased, and efficient model.
 By providing public access to `vl-datasets` we hope it helps advance the field of computer vision.
 
 ## Datasets & Access
 We're a startup and we'd like to offer free access to the datasets as much as we can afford to. But in doing so, we'd also need your support.
 
 We're offering select `.csv` files completely free with no strings attached. 
-For access to our complete dataset and exclusive beta features, all we ask is that you [sign up]((https://forms.gle/8jxPkyzeKj82kPed8)) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
-
-Join us in unlocking the full potential of our data and revolutionizing the industry!
+For access to our complete dataset and exclusive beta features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
 
 Here is a table of widely used computer vision datasets, issues we found and a link to access the `.csv` file.
 
 
 | Dataset                                                                 | Issues (WIP)                                                                                                                                                                                 | CSV            |
 |-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
 | [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). |
-| [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download here. |
+| [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). |
 | [Imagenette](https://github.com/fastai/imagenette)                      | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download here. |
-| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-
-
-<!-- ## Setting Up
+| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
 
-### Prerequisites 
 
-Supported `Python` versions:
-
-
-![Supported Python: Ubuntu](https://img.shields.io/badge/Python-3.9%20%7C%203.10-blue?style=for-the-badge)
-
-
-Supported operating systems:
-
-![Supported OS: Ubuntu](https://img.shields.io/badge/Supported%20OS-Ubuntu-orange.svg?style=for-the-badge) -->
+Learn more on how we clean the datasets using our profilling tool [here](https://visual-layer.link).
 
 
 ## Installation
 
-**Option 1** - Install `vl_datasets` package from PyPI.
+**Option 1** - Install `vl_datasets` package from PyPI:
 
 ```shell
 pip install vl-datasets
 ```
 
-**Option 2** - Install the bleeding edge version on GitHub
+**Option 2** - Install the bleeding edge version on GitHub:
 ```
 pip install git+https://github.com/visual-layer/vl-datasets.git@main --upgrade
 ```
 
 ## Usage
-To start using `vl-datasets`, you can import the clean version of the dataset with:
+To start using `vl-datasets`, import the clean version of the dataset with:
 
 ```python
 from vl_datasets import CleanFood101
 ```
 
 This should import the clean version of the `Food101` dataset.
 
 Next, you can load the dataset as a PyTorch `Dataset`.
 
 ```python
 train_dataset = CleanFood101('./', split='train')
 valid_dataset = CleanFood101('./', split='test')
 ```
 
+If you have a custom `.csv` file you can optionally pass in the file:
+
+```python
+train_dataset = CleanFood101('./', split='train', exclude_csv='my-file.csv')
+```
+The filenames listed in the `.csv` will be excluded in the dataset.
+
+Next, you can load the train and validation datasets in a PyTorch training loop.
+
+See the [Learn from Examples](#learn-from-examples) section to learn more.
+
 
 > **NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for free to be our beta testers and get full access to the all the `.csv` files for the dataset listed in this repo. 
 
 With the dataset loaded you can train a model using PyTorch training loop.
 
 ## Learn from Examples
 
@@ -237,17 +249,17 @@
       <td rowspan="3" width="160">
       <a href="https://visual-layer.readme.io/docs/objects-and-bounding-boxes">
               <img src="./imgs/pet.jpg" width="256">
       </a>
       </td>    
       <td rowspan="3">
         <ul>
-            <li> <b>Dataset:</b> <code>CleanPets</code></li>
+            <li> <b>Dataset:</b> <code>CleanOxfordIIITPet</code></li>
             <li> <b>Framework:</b> fast.ai.</li>
-            <li> <b>Description:</b> Finetune a pretrained DINOv2 model using fastai.</li>
+            <li> <b>Description:</b> Finetune a pretrained TIMM model using fastai.</li>
         </ul>
       </td>
       <td align="center" width="80">
           <a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
               <img src="./imgs/nbviewer_logo.svg" height="34">
           </a>
       </td>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.5 Summary: Open, Clean
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.6 Summary: Open, Clean
 Datasets for Computer Vision. Home-page: https://github.com/visual-layer/vl-
 datasets Author: Visual Layer Author-email: info@visual-layer.com License:
 Apache-2.0 Keywords: machine learning,computer vision,data-centric Platform:
 UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
@@ -17,52 +17,57 @@
 dynamic/json?style=for-the-
 badge&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fvl-
 datasets&color=lightblue [downloads-url]: https://pypi.org/project/vl-datasets/
 [license-shield]: https://img.shields.io/badge/License-Apache%202.0-
 purple.svg?style=for-the-badge [license-url]: https://github.com/visual-layer/
 vl-datasets/blob/main/LICENSE
                               [Visual_Layer_Logo]
-              **** Open, Clean Datasets for Computer Vision ****
+          **** Open, Clean, Curated Datasets for Computer Vision ****
 
  ð¥ We use fastdup - a free tool to clean all datasets shared in this repo.
                              Explore_the_docs_Â»
             Report_Issues Â· Read_Blog Â· Get_In_Touch Â· About_Us
 
                       [Logo] [Logo] [Logo] [Logo] [Logo]
-## Description `vl-datasets` is a collection of clean computer vision datasets,
-carefully analyzed and processed to avoid common image dataset issues such as:
-+ Duplicates. + Broken images. + Outliers. + Dark/Bright/Blurry images. For
-each dataset in this repo, we provide a `.csv` file that lists the problematic
-images from the dataset. You can use the listed images in the `.csv` to improve
-the model by re-labeling the them or just simply remove it from the dataset. ##
-Why? Computer vision is an exciting and rapidly advancing field, with new
-techniques and models emerging now and then. However, to develop and evaluate
-these models, it's essential to have reliable and standardized datasets to work
-with. Even with the recent success of generative models, data quality remains
-an issue that's [mainly overlooked](https://medium.com/@amiralush/large-image-
-datasets-today-are-a-mess-e3ea4c9e8d22). Training models will erroneours data
-impacts model accuracy, incurs costs in time, storage and computational
-resources. We believe that access to clean and high-quality computer vision
-datasets leads to accurate, non-biased, and efficient model. By providing
-public access to `vl-datasets` we hope it helps advance the field of computer
-vision. ## Datasets & Access We're a startup and we'd like to offer free access
-to the datasets as much as we can afford to. But in doing so, we'd also need
-your support. We're offering select `.csv` files completely free with no
-strings attached. For access to our complete dataset and exclusive beta
-features, all we ask is that you [sign up]((https://forms.gle/
-8jxPkyzeKj82kPed8)) to be a beta tester â it's completely free and your
-feedback will help shape the future of our platform. Join us in unlocking the
-full potential of our data and revolutionizing the industry! Here is a table of
-widely used computer vision datasets, issues we found and a link to access the
-`.csv` file. | Dataset | Issues (WIP) | CSV | |--------------------------------
------------------------------------------|-------------------------------------
+## Description `vl-datasets` is a Python package that provides access to clean
+computer vision datasets with only 2 lines of code. For example, to get access
+to the clean version of the [Food-101](https://data.vision.ee.ethz.ch/cvl/
+datasets_extra/food-101/) dataset simply run: ![image](./imgs/usage.png) We
+support some of the most widely used computer vision datasets. [Let us know]
+(https://forms.gle/8jxPkyzeKj82kPed8) if you have additional request to support
+a new dataset. All the datasets are analyzed for issues such as: + Duplicates.
++ Broken images. + Outliers. + Dark/Bright/Blurry images. ![image](./imgs/
+issues.png) `vl-datasets` provides a convenient way to access these cleaned
+datasets in Python. Alternatively, for each dataset in this repo, we provide a
+`.csv` file that lists the problematic images from the dataset. You can use the
+listed images in the `.csv` to improve the model by re-labeling the them or
+just simply remove it from the dataset. ## Why? Computer vision is an exciting
+and rapidly advancing field, with new techniques and models emerging now and
+then. However, to develop and evaluate these models, it's essential to have
+reliable and standardized datasets to work with. Even with the recent success
+of generative models, data quality remains an issue that's [mainly overlooked]
+(https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-
+e3ea4c9e8d22). Training models will erroneours data impacts model accuracy,
+incurs costs in time, storage and computational resources. We believe that
+access to clean and high-quality computer vision datasets leads to accurate,
+non-biased, and efficient model. By providing public access to `vl-datasets` we
+hope it helps advance the field of computer vision. ## Datasets & Access We're
+a startup and we'd like to offer free access to the datasets as much as we can
+afford to. But in doing so, we'd also need your support. We're offering select
+`.csv` files completely free with no strings attached. For access to our
+complete dataset and exclusive beta features, all we ask is that you [sign up]
+(https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester â it's completely
+free and your feedback will help shape the future of our platform. Here is a
+table of widely used computer vision datasets, issues we found and a link to
+access the `.csv` file. | Dataset | Issues (WIP) | CSV | |---------------------
+----------------------------------------------------|--------------------------
 -------------------------------------------------------------------------------
---------------------------------------------------------------------------|----
-------------| | [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/
-food-101/) |
+-------------------------------------------------------------------------------
+------|----------------| | [Food-101](https://data.vision.ee.ethz.ch/cvl/
+datasets_extra/food-101/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
 | Download [here](https://drive.google.com/
@@ -70,114 +75,123 @@
 (https://www.robots.ox.ac.uk/~vgg/data/pets/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Download here. | | [Imagenette](https://github.com/fastai/imagenette) |
+| Download [here](https://drive.google.com/
+uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | | [Imagenette]
+(https://github.com/fastai/imagenette) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
 | Download here. | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-21k]
-(https://www.image-net.org/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-
+21k](https://www.image-net.org/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-1k](https:
-//www.image-net.org/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-1k]
+(https://www.image-net.org/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [KITTI](https://
-www.cvlibs.net/datasets/kitti/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [KITTI]
+(https://www.cvlibs.net/datasets/kitti/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [DeepFashion](http:/
-/mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [DeepFashion]
+(http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Places365](https://
-github.com/CSAILVision/places365) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Places365]
+(https://github.com/CSAILVision/places365) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [CelebA-HQ](http://
-mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [CelebA-HQ]
+(http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [ADE20K](https://
-groups.csail.mit.edu/vision/datasets/ADE20K/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [ADE20K]
+(https://groups.csail.mit.edu/vision/datasets/ADE20K/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [COCO](https://
-cocodataset.org/#home) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [COCO](https:
+//cocodataset.org/#home) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). |  ## Installation
-**Option 1** - Install `vl_datasets` package from PyPI. ```shell pip install
-vl-datasets ``` **Option 2** - Install the bleeding edge version on GitHub ```
-pip install git+https://github.com/visual-layer/vl-datasets.git@main --upgrade
-``` ## Usage To start using `vl-datasets`, you can import the clean version of
-the dataset with: ```python from vl_datasets import CleanFood101 ``` This
-should import the clean version of the `Food101` dataset. Next, you can load
-the dataset as a PyTorch `Dataset`. ```python train_dataset = CleanFood101('./
-', split='train') valid_dataset = CleanFood101('./', split='test') ``` >
-**NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for free to be
-our beta testers and get full access to the all the `.csv` files for the
-dataset listed in this repo. With the dataset loaded you can train a model
-using PyTorch training loop. ## Learn from Examples
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | Learn more on
+how we clean the datasets using our profilling tool [here](https://visual-
+layer.link). ## Installation **Option 1** - Install `vl_datasets` package from
+PyPI: ```shell pip install vl-datasets ``` **Option 2** - Install the bleeding
+edge version on GitHub: ``` pip install git+https://github.com/visual-layer/vl-
+datasets.git@main --upgrade ``` ## Usage To start using `vl-datasets`, import
+the clean version of the dataset with: ```python from vl_datasets import
+CleanFood101 ``` This should import the clean version of the `Food101` dataset.
+Next, you can load the dataset as a PyTorch `Dataset`. ```python train_dataset
+= CleanFood101('./', split='train') valid_dataset = CleanFood101('./',
+split='test') ``` If you have a custom `.csv` file you can optionally pass in
+the file: ```python train_dataset = CleanFood101('./', split='train',
+exclude_csv='my-file.csv') ``` The filenames listed in the `.csv` will be
+excluded in the dataset. Next, you can load the train and validation datasets
+in a PyTorch training loop. See the [Learn from Examples](#learn-from-examples)
+section to learn more. > **NOTE**: Sign up [here](https://forms.gle/
+8jxPkyzeKj82kPed8) for free to be our beta testers and get full access to the
+all the `.csv` files for the dataset listed in this repo. With the dataset
+loaded you can train a model using PyTorch training loop. ## Learn from
+Examples
                       * Dataset: CleanFood101       [./imgs/nbviewer_logo.svg]
 [./imgs/food.jpg]     * Framework: PyTorch.          [./imgs/github_logo.png]
                       * Description: Load a dataset   [./imgs/colab_logo.png]
                         and train a PyTorch model.
-                      * Dataset: CleanPets          [./imgs/nbviewer_logo.svg]
+                      * Dataset: CleanOxfordIIITPet [./imgs/nbviewer_logo.svg]
                       * Framework: fast.ai.          [./imgs/github_logo.png]
 [./imgs/pet.jpg]      * Description: Finetune a
-                        pretrained DINOv2 model       [./imgs/colab_logo.png]
-                        using fastai.
+                        pretrained TIMM model using   [./imgs/colab_logo.png]
+                        fastai.
 ## License `vl-datasets` is licensed under the Apache 2.0 License. See
 [LICENSE](./LICENSE). However, you are bound to the usage license of the
 original dataset. It is your responsibility to determine whether you have
 permission to use the dataset under the dataset's license. We provide no
 warranty or guarantee of accuracy or completeness. ## Getting Help Get help
 from the Visual Layer team or community members via the following channels - +
 [Slack](https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-
```

## Comparing `vl_datasets-0.0.5.dist-info/RECORD` & `vl_datasets-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-vl_datasets/__init__.py,sha256=dujkobmbbGaxbOqGb4EtWbn_Cr_duOBvEYwcWYsOr2I,99
+vl_datasets/__init__.py,sha256=50SEBWz4pZFQVYwU5ajqPr4DP7M7uFYx1EV8aZiajP4,141
 vl_datasets/food101.py,sha256=JX3uO3J234GIHFRZlBfg0Qt74AXqbbD0yCVErFZa1Gs,4734
 vl_datasets/image_folder.py,sha256=qjhkPSbGeK5pcYL7t1md5b4RDUPUuo5MrCdtt0LrNYQ,2352
-vl_datasets-0.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vl_datasets-0.0.5.dist-info/METADATA,sha256=17LxWayakIpIpQyhNDc6dOAg16RZTUJwYsYN1iwuYK8,16358
-vl_datasets-0.0.5.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-vl_datasets-0.0.5.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
-vl_datasets-0.0.5.dist-info/RECORD,,
+vl_datasets/oxford_pet.py,sha256=DyiYytV0ri6QFcJ4m4FsfJeixmHJrQiDilNa2IPI_bM,4823
+vl_datasets/utils.py,sha256=JXQ9pMvbIwr92FYlNEZJXuScF9OkBrE8Bs8faWQoj_w,1056
+vl_datasets-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vl_datasets-0.0.6.dist-info/METADATA,sha256=wUZ8QV6KGXQD0zl7lsxvxs_AbH-ttJt_2-GZB29HIsU,17100
+vl_datasets-0.0.6.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
+vl_datasets-0.0.6.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
+vl_datasets-0.0.6.dist-info/RECORD,,
```

