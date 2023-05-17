# Comparing `tmp/vl_datasets-0.0.6-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.7-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15132 bytes, number of entries: 10
--rw-r--r--  2.0 unx      141 b- defN 23-May-16 11:04 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     4734 b- defN 23-May-16 11:04 vl_datasets/food101.py
--rw-r--r--  2.0 unx     2352 b- defN 23-May-16 11:04 vl_datasets/image_folder.py
--rw-r--r--  2.0 unx     4823 b- defN 23-May-16 11:04 vl_datasets/oxford_pet.py
--rw-r--r--  2.0 unx     1056 b- defN 23-May-16 11:04 vl_datasets/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    17100 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-May-16 11:04 vl_datasets-0.0.6.dist-info/RECORD
-10 files, 42493 bytes uncompressed, 13758 bytes compressed:  67.6%
+Zip file size: 15231 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      141 b- defN 23-May-17 06:35 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     4734 b- defN 23-May-17 06:35 vl_datasets/food101.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-17 06:35 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx     4867 b- defN 23-May-17 06:35 vl_datasets/oxford_pet.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-17 06:35 vl_datasets/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17772 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-May-17 06:35 vl_datasets-0.0.7.dist-info/RECORD
+10 files, 43209 bytes uncompressed, 13857 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: vl_datasets/oxford_pet.py
 Comment: 
 
 Filename: vl_datasets/utils.py
 Comment: 
 
-Filename: vl_datasets-0.0.6.dist-info/LICENSE
+Filename: vl_datasets-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.6.dist-info/METADATA
+Filename: vl_datasets-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.6.dist-info/WHEEL
+Filename: vl_datasets-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.6.dist-info/top_level.txt
+Filename: vl_datasets-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.6.dist-info/RECORD
+Filename: vl_datasets-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 from .image_folder import CleanImageFolder
 from .food101 import CleanFood101
 from .oxford_pet import CleanOxfordIIITPet
```

## vl_datasets/oxford_pet.py

```diff
@@ -33,29 +33,30 @@
         root: str,
         split: str = "trainval",
         target_types: Union[Sequence[str], str] = "category",
         transforms: Optional[Callable] = None,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         exclude_csv: Optional[str] = None,
-        download: bool = False,
+        download: bool = True,
     ):
         self._split = verify_str_arg(split, "split", ("trainval", "test"))
         if isinstance(target_types, str):
             target_types = [target_types]
         self._target_types = [
             verify_str_arg(target_type, "target_types", self._VALID_TARGET_TYPES)
             for target_type in target_types
         ]
 
         super().__init__(
             root,
             transforms=transforms,
             transform=transform,
             target_transform=target_transform,
+            download=download
         )
 
         self._base_folder = pathlib.Path(self.root) / "oxford-iiit-pet"
         self._images_folder = self._base_folder / "images"
         self._anns_folder = self._base_folder / "annotations"
         self._segs_folder = self._anns_folder / "trimaps"
 
@@ -102,15 +103,15 @@
                 print(e)
 
         image_ids = []
         self._labels = []
 
         # A copy of self.exclude_set but without file extension
         exclude_set_filenames = {
-            filename.split(".")[0] for filename in self.exclude_set
+            filename.split("/")[-1].split(".")[0] for filename in self.exclude_set
         }
 
         with open(self._anns_folder / f"{self._split}.txt") as file:
             for line in file:
                 image_id, label, *_ = line.strip().split()
 
                 # if filename found in exclude set continue
```

## Comparing `vl_datasets-0.0.6.dist-info/LICENSE` & `vl_datasets-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.6.dist-info/METADATA` & `vl_datasets-0.0.7.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.6
+Version: 0.0.7
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -138,28 +138,28 @@
 
 We're offering select `.csv` files completely free with no strings attached. 
 For access to our complete dataset and exclusive beta features, all we ask is that you [sign up](https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
 
 Here is a table of widely used computer vision datasets, issues we found and a link to access the `.csv` file.
 
 
-| Dataset                                                                 | Issues (WIP)                                                                                                                                                                                 | CSV            |
-|-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
-| [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). |
-| [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). |
-| [Imagenette](https://github.com/fastai/imagenette)                      | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download here. |
-| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
-| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
+| Dataset                                                                 | Issues (WIP)                                                                                                                                                                                 | CSV                                                                                                | Class                |
+|-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------|
+| [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `CleanFood101`       |
+| [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 1.021% (75)</li><li>Outliers - 0.095% (7)</li><li>Broken - 0.000% (0)</li><li>Blur - 0.000% (0)</li><li>Dark - 0.054% (4)</li><li>Bright - 0.000% (0)</li></ul>         | Download [here](https://drive.google.com/uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | `CleanOxfordIIITPet` |
+| [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [Places365](https://github.com/CSAILVision/places365)                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)           | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+| [COCO](https://cocodataset.org/#home)                                   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Request access [here](https://forms.gle/8jxPkyzeKj82kPed8).                                        | WIP                  |
+
 
 
 Learn more on how we clean the datasets using our profilling tool [here](https://visual-layer.link).
 
 
 ## Installation
 
@@ -205,88 +205,99 @@
 > **NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for free to be our beta testers and get full access to the all the `.csv` files for the dataset listed in this repo. 
 
 With the dataset loaded you can train a model using PyTorch training loop.
 
 ## Learn from Examples
 
 <table>
-  <tr>
-      <td rowspan="3" width="160">
-      <a href="https://visual-layer.readme.io/docs/getting-started">
-              <img src="./imgs/food.jpg" width="256">
-      </a>
-      </td>    
-      <td rowspan="3">
-        <ul>
-            <li> <b>Dataset:</b> <code>CleanFood101</code></li>
-            <li> <b>Framework:</b> PyTorch.</li>
-            <li> <b>Description:</b> Load a dataset and train a PyTorch model.</li>
-        </ul>
-      </td>
-      <td align="center" width="80">
-          <a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
-              <img src="./imgs/nbviewer_logo.svg" height="34">
-          </a>
-      </td>
-  </tr>
-  <tr>
-      <td align="center">
-          <a href="https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
-              <img src="./imgs/github_logo.png" height="32">
-          </a>
-      </td>
-  </tr>
-  <tr>
-      <td align="center">
-          <a href="https://colab.research.google.com/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
-              <img src="./imgs/colab_logo.png" height="28">
-          </a>
-      </td>
-  </tr>
-
-  <!-- ------------------------------------------------------------------- -->
-
-  <tr>
-      <td rowspan="3" width="160">
-      <a href="https://visual-layer.readme.io/docs/objects-and-bounding-boxes">
-              <img src="./imgs/pet.jpg" width="256">
-      </a>
-      </td>    
-      <td rowspan="3">
-        <ul>
-            <li> <b>Dataset:</b> <code>CleanOxfordIIITPet</code></li>
-            <li> <b>Framework:</b> fast.ai.</li>
-            <li> <b>Description:</b> Finetune a pretrained TIMM model using fastai.</li>
-        </ul>
-      </td>
-      <td align="center" width="80">
-          <a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
-              <img src="./imgs/nbviewer_logo.svg" height="34">
-          </a>
-      </td>
-  </tr>
-  <tr>
-      <td align="center">
-          <a href="https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
-              <img src="./imgs/github_logo.png" height="32">
-          </a>
-      </td>
-  </tr>
-  <tr>
-      <td align="center">
-          <a href="https://colab.research.google.com/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
-              <img src="./imgs/colab_logo.png" height="28">
-          </a>
-      </td>
-  </tr>
-
-  <!-- ------------------------------------------------------------------- -->
-  
+	<tr>
+		<td rowspan="4" width="160">
+			<a href="https://visual-layer.readme.io/docs/getting-started">
+				<img src="./imgs/food.jpg" width="256" />
+			</a>
+		</td>
+		<td rowspan="4">
+			<ul>
+				<li><b>Dataset:</b> <code>CleanFood101</code></li>
+				<li><b>Framework:</b> PyTorch.</li>
+				<li><b>Description:</b> Load a dataset and train a PyTorch model.</li>
+			</ul>
+		</td>
+		<td align="center" width="80">
+			<a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
+				<img src="./imgs/nbviewer_logo.svg" height="34" />
+			</a>
+		</td>
+	</tr>
+	<tr>
+		<td align="center">
+			<a href="https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
+				<img src="./imgs/github_logo.png" height="32" />
+			</a>
+		</td>
+	</tr>
+	<tr>
+		<td align="center">
+			<a href="https://colab.research.google.com/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
+				<img src="./imgs/colab_logo.png" height="28" />
+			</a>
+		</td>
+	</tr>
+    <tr>
+		<td align="center">
+			<a href="https://kaggle.com/kernels/welcome?src=https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
+				<img src="./imgs/kaggle_logo.png" height="28" />
+			</a>
+		</td>
+	</tr>
+	<!-- ------------------------------------------------------------------- -->
+	<tr>
+		<td rowspan="4" width="160">
+			<a href="https://visual-layer.readme.io/docs/objects-and-bounding-boxes">
+				<img src="./imgs/pet.jpg" width="256" />
+			</a>
+		</td>
+		<td rowspan="4">
+			<ul>
+				<li><b>Dataset:</b> <code>CleanOxfordIIITPet</code></li>
+				<li><b>Framework:</b> fast.ai.</li>
+				<li><b>Description:</b> Finetune a pretrained TIMM model using fastai.</li>
+			</ul>
+		</td>
+		<td align="center" width="80">
+			<a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
+				<img src="./imgs/nbviewer_logo.svg" height="34" />
+			</a>
+		</td>
+	</tr>
+	<tr>
+		<td align="center">
+			<a href="https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
+				<img src="./imgs/github_logo.png" height="32" />
+			</a>
+		</td>
+	</tr>
+	<tr>
+		<td align="center">
+			<a href="https://colab.research.google.com/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
+				<img src="./imgs/colab_logo.png" height="28" />
+			</a>
+		</td>
+	</tr>
+    <tr>
+		<td align="center">
+			<a href="https://kaggle.com/kernels/welcome?src=https://github.com/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
+				<img src="./imgs/kaggle_logo.png" height="28" />
+			</a>
+		</td>
+	</tr>
+	<!-- ------------------------------------------------------------------- -->
 </table>
 
+
 ## License
 `vl-datasets` is licensed under the Apache 2.0 License. See [LICENSE](./LICENSE).
 
 However, you are bound to the usage license of the original dataset. It is your responsibility to determine whether you have permission to use the dataset under the dataset's license. We provide no warranty or guarantee of accuracy or completeness.
 
 ## Getting Help
 Get help from the Visual Layer team or community members via the following channels -
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.6 Summary: Open, Clean
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.7 Summary: Open, Clean
 Datasets for Computer Vision. Home-page: https://github.com/visual-layer/vl-
 datasets Author: Visual Layer Author-email: info@visual-layer.com License:
 Apache-2.0 Keywords: machine learning,computer vision,data-centric Platform:
 UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
@@ -54,143 +54,137 @@
 a startup and we'd like to offer free access to the datasets as much as we can
 afford to. But in doing so, we'd also need your support. We're offering select
 `.csv` files completely free with no strings attached. For access to our
 complete dataset and exclusive beta features, all we ask is that you [sign up]
 (https://forms.gle/8jxPkyzeKj82kPed8) to be a beta tester â it's completely
 free and your feedback will help shape the future of our platform. Here is a
 table of widely used computer vision datasets, issues we found and a link to
-access the `.csv` file. | Dataset | Issues (WIP) | CSV | |---------------------
-----------------------------------------------------|--------------------------
+access the `.csv` file. | Dataset | Issues (WIP) | CSV | Class | |-------------
+------------------------------------------------------------|------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------|----------------| | [Food-101](https://data.vision.ee.ethz.ch/cvl/
-datasets_extra/food-101/) |
+--------------|----------------------------------------------------------------
+------------------------------------|----------------------| | [Food-101]
+(https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
 | Download [here](https://drive.google.com/
-uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | | [Oxford-IIIT Pet]
-(https://www.robots.ox.ac.uk/~vgg/data/pets/) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
+uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | `CleanFood101` | |
+[Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/) |
+    * Duplicates - 1.021% (75)
+    * Outliers - 0.095% (7)
+    * Broken - 0.000% (0)
+    * Blur - 0.000% (0)
+    * Dark - 0.054% (4)
+    * Bright - 0.000% (0)
 | Download [here](https://drive.google.com/
-uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). | | [Imagenette]
-(https://github.com/fastai/imagenette) |
-    * Duplicates - 0.24% (12,345)
-    * Outliers - 0.85% (456)
-    * Broken - 0.85% (456)
-    * Blur - 0.85% (456)
-    * Dark - 0.85% (456)
-    * Bright - 0.85% (456)
-| Download here. | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
+uc?export=download&id=1OLa8k4NITnmCHjeByzvGaWt3W7k6R1QL). |
+`CleanOxfordIIITPet` | | [LAION-1B](https://laion.ai/blog/laion-5b/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-
-21k](https://www.image-net.org/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[Imagenet-21k](https://www.image-net.org/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Imagenet-1k]
-(https://www.image-net.org/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[Imagenet-1k](https://www.image-net.org/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [KITTI]
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [KITTI]
 (https://www.cvlibs.net/datasets/kitti/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [DeepFashion]
-(http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [Places365]
-(https://github.com/CSAILVision/places365) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[Places365](https://github.com/CSAILVision/places365) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [CelebA-HQ]
-(http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[CelebA-HQ](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [ADE20K]
-(https://groups.csail.mit.edu/vision/datasets/ADE20K/) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | |
+[ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | | [COCO](https:
-//cocodataset.org/#home) |
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | | [COCO]
+(https://cocodataset.org/#home) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | Learn more on
-how we clean the datasets using our profilling tool [here](https://visual-
-layer.link). ## Installation **Option 1** - Install `vl_datasets` package from
-PyPI: ```shell pip install vl-datasets ``` **Option 2** - Install the bleeding
-edge version on GitHub: ``` pip install git+https://github.com/visual-layer/vl-
-datasets.git@main --upgrade ``` ## Usage To start using `vl-datasets`, import
-the clean version of the dataset with: ```python from vl_datasets import
-CleanFood101 ``` This should import the clean version of the `Food101` dataset.
-Next, you can load the dataset as a PyTorch `Dataset`. ```python train_dataset
-= CleanFood101('./', split='train') valid_dataset = CleanFood101('./',
-split='test') ``` If you have a custom `.csv` file you can optionally pass in
-the file: ```python train_dataset = CleanFood101('./', split='train',
-exclude_csv='my-file.csv') ``` The filenames listed in the `.csv` will be
-excluded in the dataset. Next, you can load the train and validation datasets
-in a PyTorch training loop. See the [Learn from Examples](#learn-from-examples)
-section to learn more. > **NOTE**: Sign up [here](https://forms.gle/
-8jxPkyzeKj82kPed8) for free to be our beta testers and get full access to the
-all the `.csv` files for the dataset listed in this repo. With the dataset
-loaded you can train a model using PyTorch training loop. ## Learn from
-Examples
+| Request access [here](https://forms.gle/8jxPkyzeKj82kPed8). | WIP | Learn
+more on how we clean the datasets using our profilling tool [here](https://
+visual-layer.link). ## Installation **Option 1** - Install `vl_datasets`
+package from PyPI: ```shell pip install vl-datasets ``` **Option 2** - Install
+the bleeding edge version on GitHub: ``` pip install git+https://github.com/
+visual-layer/vl-datasets.git@main --upgrade ``` ## Usage To start using `vl-
+datasets`, import the clean version of the dataset with: ```python from
+vl_datasets import CleanFood101 ``` This should import the clean version of the
+`Food101` dataset. Next, you can load the dataset as a PyTorch `Dataset`.
+```python train_dataset = CleanFood101('./', split='train') valid_dataset =
+CleanFood101('./', split='test') ``` If you have a custom `.csv` file you can
+optionally pass in the file: ```python train_dataset = CleanFood101('./',
+split='train', exclude_csv='my-file.csv') ``` The filenames listed in the
+`.csv` will be excluded in the dataset. Next, you can load the train and
+validation datasets in a PyTorch training loop. See the [Learn from Examples]
+(#learn-from-examples) section to learn more. > **NOTE**: Sign up [here](https:
+//forms.gle/8jxPkyzeKj82kPed8) for free to be our beta testers and get full
+access to the all the `.csv` files for the dataset listed in this repo. With
+the dataset loaded you can train a model using PyTorch training loop. ## Learn
+from Examples
                       * Dataset: CleanFood101       [./imgs/nbviewer_logo.svg]
 [./imgs/food.jpg]     * Framework: PyTorch.          [./imgs/github_logo.png]
                       * Description: Load a dataset   [./imgs/colab_logo.png]
-                        and train a PyTorch model.
+                        and train a PyTorch model.   [./imgs/kaggle_logo.png]
                       * Dataset: CleanOxfordIIITPet [./imgs/nbviewer_logo.svg]
                       * Framework: fast.ai.          [./imgs/github_logo.png]
-[./imgs/pet.jpg]      * Description: Finetune a
-                        pretrained TIMM model using   [./imgs/colab_logo.png]
+[./imgs/pet.jpg]      * Description: Finetune a       [./imgs/colab_logo.png]
+                        pretrained TIMM model using  [./imgs/kaggle_logo.png]
                         fastai.
 ## License `vl-datasets` is licensed under the Apache 2.0 License. See
 [LICENSE](./LICENSE). However, you are bound to the usage license of the
 original dataset. It is your responsibility to determine whether you have
 permission to use the dataset under the dataset's license. We provide no
 warranty or guarantee of accuracy or completeness. ## Getting Help Get help
 from the Visual Layer team or community members via the following channels - +
```

## Comparing `vl_datasets-0.0.6.dist-info/RECORD` & `vl_datasets-0.0.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-vl_datasets/__init__.py,sha256=50SEBWz4pZFQVYwU5ajqPr4DP7M7uFYx1EV8aZiajP4,141
+vl_datasets/__init__.py,sha256=yv-iuT9v_UIquIEFyOlnCbn6fCGpZNoaVYdsGdZbYoo,141
 vl_datasets/food101.py,sha256=JX3uO3J234GIHFRZlBfg0Qt74AXqbbD0yCVErFZa1Gs,4734
 vl_datasets/image_folder.py,sha256=qjhkPSbGeK5pcYL7t1md5b4RDUPUuo5MrCdtt0LrNYQ,2352
-vl_datasets/oxford_pet.py,sha256=DyiYytV0ri6QFcJ4m4FsfJeixmHJrQiDilNa2IPI_bM,4823
+vl_datasets/oxford_pet.py,sha256=8MwaNtwVqNSbxYMqgaEcVMw09n5qwYu3hHsrLnJDfis,4867
 vl_datasets/utils.py,sha256=JXQ9pMvbIwr92FYlNEZJXuScF9OkBrE8Bs8faWQoj_w,1056
-vl_datasets-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vl_datasets-0.0.6.dist-info/METADATA,sha256=wUZ8QV6KGXQD0zl7lsxvxs_AbH-ttJt_2-GZB29HIsU,17100
-vl_datasets-0.0.6.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-vl_datasets-0.0.6.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
-vl_datasets-0.0.6.dist-info/RECORD,,
+vl_datasets-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vl_datasets-0.0.7.dist-info/METADATA,sha256=WsQPccBqbgjlm2D-wyUnxvsaRqc5GNg7gEz_yxrcY2g,17772
+vl_datasets-0.0.7.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
+vl_datasets-0.0.7.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
+vl_datasets-0.0.7.dist-info/RECORD,,
```

