# Comparing `tmp/torch_uncertainty-0.1.0.tar.gz` & `tmp/torch_uncertainty-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_uncertainty-0.1.0.tar", max compression
+gzip compressed data, was "torch_uncertainty-0.1.1.tar", max compression
```

## Comparing `torch_uncertainty-0.1.0.tar` & `torch_uncertainty-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,66 @@
--rw-r--r--   0        0        0    11363 2023-02-15 16:35:44.883384 torch_uncertainty-0.1.0/LICENSE
--rw-r--r--   0        0        0     2721 2023-02-15 16:35:44.883384 torch_uncertainty-0.1.0/README.md
--rw-r--r--   0        0        0     1682 2023-02-15 16:35:44.883384 torch_uncertainty-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3331 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/__init__.py
--rw-r--r--   0        0        0       48 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/__init__.py
--rw-r--r--   0        0        0       49 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/batched/__init__.py
--rw-r--r--   0        0        0     6501 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/batched/resnet.py
--rw-r--r--   0        0        0       48 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/masked/__init__.py
--rw-r--r--   0        0        0     6156 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/masked/resnet.py
--rw-r--r--   0        0        0        0 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/mimo/__init__.py
--rw-r--r--   0        0        0       48 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/packed/__init__.py
--rw-r--r--   0        0        0     6114 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/packed/resnet.py
--rw-r--r--   0        0        0       42 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/standard/__init__.py
--rw-r--r--   0        0        0     2237 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/baselines/standard/resnet.py
--rw-r--r--   0        0        0      221 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/__init__.py
--rw-r--r--   0        0        0     7843 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/cifar10.py
--rw-r--r--   0        0        0     7253 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/cifar100.py
--rw-r--r--   0        0        0     6598 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/imagenet.py
--rw-r--r--   0        0        0     4706 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/mnist.py
--rw-r--r--   0        0        0     4437 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datamodules/tiny_imagenet.py
--rw-r--r--   0        0        0      216 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/__init__.py
--rw-r--r--   0        0        0      771 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/aggregated_dataset.py
--rw-r--r--   0        0        0     4036 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/cifar_c.py
--rw-r--r--   0        0        0      559 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/imagenet_o.py
--rw-r--r--   0        0        0     1048 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/imagenet_r.py
--rw-r--r--   0        0        0      789 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/mixing_set.py
--rw-r--r--   0        0        0     4976 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/datasets/tiny_imagenet.py
--rw-r--r--   0        0        0      182 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/layers/__init__.py
--rw-r--r--   0        0        0    15133 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/layers/batchens_layers.py
--rw-r--r--   0        0        0     9725 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/layers/masksembles_layers.py
--rw-r--r--   0        0        0     6503 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/layers/packed_layers.py
--rw-r--r--   0        0        0      340 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/__init__.py
--rw-r--r--   0        0        0     6091 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/brier_score.py
--rw-r--r--   0        0        0     5264 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/disagreement.py
--rw-r--r--   0        0        0     6559 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/entropy.py
--rw-r--r--   0        0        0     4060 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/fpr95.py
--rw-r--r--   0        0        0     4917 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/jensen_shannon_divergence.py
--rw-r--r--   0        0        0     5852 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/mutual_information.py
--rw-r--r--   0        0        0     4296 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/nll.py
--rw-r--r--   0        0        0     2656 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/metrics/variation_ratio.py
--rw-r--r--   0        0        0        0 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/__init__.py
--rw-r--r--   0        0        0      101 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/__init__.py
--rw-r--r--   0        0        0    10797 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/batched.py
--rw-r--r--   0        0        0    12789 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/masked.py
--rw-r--r--   0        0        0    12733 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/packed.py
--rw-r--r--   0        0        0     9906 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/std.py
--rw-r--r--   0        0        0        0 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/wideresnet/__init__.py
--rw-r--r--   0        0        0     4993 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/wideresnet/packed.py
--rw-r--r--   0        0        0     4392 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/models/wideresnet/std.py
--rw-r--r--   0        0        0     4557 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/optimization_procedures.py
--rw-r--r--   0        0        0        0 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/routines/__init__.py
--rw-r--r--   0        0        0    10628 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/routines/classification.py
--rw-r--r--   0        0        0       42 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/transforms/__init__.py
--rw-r--r--   0        0        0      815 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/transforms/cutout.py
--rw-r--r--   0        0        0     1301 2023-02-15 16:35:44.887384 torch_uncertainty-0.1.0/torch_uncertainty/utils.py
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.0/setup.py
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11363 2023-05-17 14:21:25.756706 torch_uncertainty-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2996 2023-05-17 14:21:25.756706 torch_uncertainty-0.1.1/README.md
+-rw-r--r--   0        0        0     2002 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3838 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/__init__.py
+-rw-r--r--   0        0        0      212 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/__init__.py
+-rw-r--r--   0        0        0     6909 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/resnet.py
+-rw-r--r--   0        0        0     6111 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/wideresnet.py
+-rw-r--r--   0        0        0       89 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/__init__.py
+-rw-r--r--   0        0        0     6564 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/resnet.py
+-rw-r--r--   0        0        0     5443 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/wideresnet.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/mimo/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/__init__.py
+-rw-r--r--   0        0        0     7688 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/resnet.py
+-rw-r--r--   0        0        0     5317 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/wideresnet.py
+-rw-r--r--   0        0        0       77 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/__init__.py
+-rw-r--r--   0        0        0     4800 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/resnet.py
+-rw-r--r--   0        0        0     3891 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/wideresnet.py
+-rw-r--r--   0        0        0      221 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/__init__.py
+-rw-r--r--   0        0        0     6647 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar10.py
+-rw-r--r--   0        0        0     7007 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar100.py
+-rw-r--r--   0        0        0     6404 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/imagenet.py
+-rw-r--r--   0        0        0     4649 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/mnist.py
+-rw-r--r--   0        0        0     4437 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/tiny_imagenet.py
+-rw-r--r--   0        0        0      247 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/__init__.py
+-rw-r--r--   0        0        0      771 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/aggregated_dataset.py
+-rw-r--r--   0        0        0     4036 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_c.py
+-rw-r--r--   0        0        0     2528 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_h.py
+-rw-r--r--   0        0        0      559 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_o.py
+-rw-r--r--   0        0        0     1048 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_r.py
+-rw-r--r--   0        0        0      789 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/mixing_set.py
+-rw-r--r--   0        0        0     5007 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/tiny_imagenet.py
+-rw-r--r--   0        0        0      182 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/__init__.py
+-rw-r--r--   0        0        0    15133 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/batchens_layers.py
+-rw-r--r--   0        0        0     9725 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/masksembles_layers.py
+-rw-r--r--   0        0        0     8318 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/packed_layers.py
+-rw-r--r--   0        0        0      340 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/__init__.py
+-rw-r--r--   0        0        0     4042 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/brier_score.py
+-rw-r--r--   0        0        0     3456 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/disagreement.py
+-rw-r--r--   0        0        0     3098 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/entropy.py
+-rw-r--r--   0        0        0     4060 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/fpr95.py
+-rw-r--r--   0        0        0     3829 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/jensen_shannon_divergence.py
+-rw-r--r--   0        0        0     3376 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/mutual_information.py
+-rw-r--r--   0        0        0     3149 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/nll.py
+-rw-r--r--   0        0        0     2656 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/variation_ratio.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/__init__.py
+-rw-r--r--   0        0        0    11032 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/batched.py
+-rw-r--r--   0        0        0    12641 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/masked.py
+-rw-r--r--   0        0        0    13476 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/packed.py
+-rw-r--r--   0        0        0    10540 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/std.py
+-rw-r--r--   0        0        0      101 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/__init__.py
+-rw-r--r--   0        0        0     5704 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/batched.py
+-rw-r--r--   0        0        0     6386 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/masked.py
+-rw-r--r--   0        0        0     7010 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/packed.py
+-rw-r--r--   0        0        0     5420 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/std.py
+-rw-r--r--   0        0        0     4791 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/optimization_procedures.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/routines/__init__.py
+-rw-r--r--   0        0        0    10576 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/routines/classification.py
+-rw-r--r--   0        0        0       42 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/transforms/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/transforms/cutout.py
+-rw-r--r--   0        0        0       77 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/__init__.py
+-rw-r--r--   0        0        0     1313 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/checkpoints.py
+-rw-r--r--   0        0        0      210 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/hub.py
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.1/setup.py
+-rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.1/PKG-INFO
```

### Comparing `torch_uncertainty-0.1.0/LICENSE` & `torch_uncertainty-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/README.md` & `torch_uncertainty-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-# Torch Uncertainty
+Metadata-Version: 2.1
+Name: torch-uncertainty
+Version: 0.1.1
+Summary: A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.
+License: Apache-2.0
+Keywords: deep-learning,pytorch,uncertainty,ensembles,uncertainty-quantification,predictive-uncertainty,reliable-ai,deep-learning-uncertainty
+Author: ENSTA U2IS
+Author-email: olivier.laurent@ensta-paris.fr
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: einops (>=0.6.0,<0.7.0)
+Requires-Dist: huggingface-hub (>=0.14.1,<0.15.0)
+Requires-Dist: pytorch-lightning (>=1.9.0,<2.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
+Requires-Dist: timm (>=0.6.12,<0.7.0)
+Requires-Dist: torchinfo (>=1.7.1,<2.0.0)
+Requires-Dist: torchvision (>=0.14.1,<0.15.0)
+Description-Content-Type: text/markdown
 
-[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+<div align="center">
 
-_Torch Uncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.
+![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)
+
+[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty) [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+</div>
+
+_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.
 
 ---
 
 This package provides a multi-level API, including:
-- ready-to-train baselines on research datasets, such as CIFAR and ImageNet
+- ready-to-train baselines on research datasets, such as ImageNet and CIFAR
 - baselines available for training on your datasets
+- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR.
 - layers available for use in your networks
 
 ## Installation
 
-The package can be installed from PyPI or from source.
-
-### From PyPI (available soon)
-
-Install the package via pip: `pip install torch-uncertainty`
-
-### From source
-
-#### Installing Poetry
-
-Installation guidelines for poetry are available on <https://python-poetry.org/docs/>. They boil down to executing the following command:
-
-`curl -sSL https://install.python-poetry.org | python3 -`
-
-#### Installing the package
-
-Clone the repository:
+The package can be installed from PyPI:
 
-`git clone https://github.com/ENSTA-U2IS/torch-uncertainty.git`
+```sh
+pip install torch-uncertainty
+```
 
-Create a new conda environment and activate it with:
-
-`conda create -n uncertainty && conda activate uncertainty`
-
-Install the package using poetry:
-
-`poetry install torch-uncertainty` or, for development, `poetry install torch-uncertainty --with dev`
-
-Depending on your system, you may encounter errors. If so, kill the process and add `PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring` at the beginning of every `poetry install` commands.
-
-#### Contributing
-
-In case that you would like to contribute, install from source and add the pre-commit hooks with `pre-commit install`
+To contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.
 
 ## Getting Started and Documentation
 
 Please find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).
 
 A quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).
 
@@ -57,14 +59,27 @@
 
 To date, the following baselines are implemented:
 
 - Deep Ensembles
 - Masksembles
 - Packed-Ensembles
 
+## Tutorials
+
 
-## Awesome Torch repositories
+## Awesome Uncertainty repositories
 
 You may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
 
-## References
+## Other References
+
+This package also contains the official implementation of Packed-Ensembles.
+
+If you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):
+	
+    @inproceedings{laurent2023packed,
+        title={Packed-Ensembles for Efficient Uncertainty Estimation},
+        author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},
+        booktitle={ICLR},
+        year={2023}
+    }
```

### Comparing `torch_uncertainty-0.1.0/pyproject.toml` & `torch_uncertainty-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 [tool.poetry]
 name = "torch_uncertainty"
-version = "0.1.0"
+version = "0.1.1"
 description = "A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques."
 authors = [
     "ENSTA U2IS <olivier.laurent@ensta-paris.fr>",
     "Adrien Lafage <adrienlafage@outlook.com>",
     "Olivier Laurent <olivier.ar.laurent@gmail.com>",
 ]
 license = "Apache-2.0"
-keywords = ["deep-learning", "pytorch", "uncertainty-quantification"]
+keywords = ["deep-learning", "pytorch", "uncertainty", "ensembles", "uncertainty-quantification", "predictive-uncertainty", "reliable-ai", "deep-learning-uncertainty"]
 readme = "README.md"
 packages = [{include = "torch_uncertainty"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pytorch-lightning = "^1.9.0"
 tensorboard = "^2.11.2"
 einops = "^0.6.0"
 torchinfo = "^1.7.1"
 torchvision = "^0.14.1"
 timm = "^0.6.12"
 scipy = "^1.10.0"
+huggingface-hub = "^0.14.1"
 
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^0.991"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.0.4"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.3"
-sphinx-rtd-theme = "^1.2.0"
+sphinx = "^5.1.3"
+pytorch-sphinx-theme = {git = "https://github.com/torch-uncertainty/pytorch_sphinx_theme"}
+sphinx-copybutton = "^0.5.1"
+sphinx-gallery = "^0.12.2"
+matplotlib = "^3.7.1"
+sphinx-design = "^0.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
@@ -47,14 +52,15 @@
 /(
     __pycache__
   | \.git
   | \.mypy_cache
   | \.ipynb_checkpoints
   | build
   | dist
+  | auto_tutorials_source/*
 )/
 '''
 
 [tool.isort]
 line_length = 80
 profile = "black"
 known_first_party = ["numpy"]
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/__init__.py` & `torch_uncertainty-0.1.1/torch_uncertainty/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # fmt: off
+# flake8: noqa
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Callable, Type, Union
 
 import pytorch_lightning as pl
+import torch
 from pytorch_lightning.callbacks import LearningRateMonitor
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint
 from pytorch_lightning.loggers.tensorboard import TensorBoardLogger
 from torch.nn import Module
 from torchinfo import summary
 
@@ -43,14 +45,17 @@
         loss=loss,
         optimization_procedure=optimization_procedure,
         num_classes=dm.num_classes,
         in_channels=dm.num_channels,
         **vars(args),
     )
 
+    if args.channels_last:
+        model = model.to(memory_format=torch.channels_last)
+
     # logger
     tb_logger = TensorBoardLogger(
         str(root / "logs"),
         name=net_name,
         default_hp_metric=False,
         log_graph=args.log_graph,
         version=args.test,
@@ -97,18 +102,35 @@
     datamodule: Type[pl.LightningDataModule],
     loss: Module,
     optimization_procedure: Callable[[Module], dict],
     root: Union[Path, str],
     net_name: str,
 ) -> None:
     parser = ArgumentParser("torch-uncertainty")
-    parser.add_argument("--seed", type=int, default=None)
-    parser.add_argument("--test", type=int, default=None)
-    parser.add_argument("--summary", dest="summary", action="store_true")
-    parser.add_argument("--log_graph", dest="log_graph", action="store_true")
+    parser.add_argument(
+        "--seed",
+        type=int,
+        default=None,
+        help="Set the random seed to some value for reproducibility",
+    )
+    parser.add_argument(
+        "--test",
+        type=int,
+        default=None,
+        help="Test a specific version of the model. The checkpoint must be available in the logs folder.",
+    )
+    parser.add_argument(
+        "--summary", action="store_true", help="Print a summary of the model"
+    )
+    parser.add_argument("--log_graph", action="store_true")
+    parser.add_argument(
+        "--channels_last",
+        action="store_true",
+        help="Use channels last memory format",
+    )
 
     parser = pl.Trainer.add_argparse_args(parser)
     parser = datamodule.add_argparse_args(parser)
     parser = network.add_model_specific_args(parser)
     args = parser.parse_args()
     main(
         network, datamodule, loss, optimization_procedure, root, net_name, args
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/baselines/batched/resnet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/wideresnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,27 @@
 # fmt: off
-from argparse import ArgumentParser
-from typing import Any, Dict, Literal
+from argparse import ArgumentParser, BooleanOptionalAction
+from typing import Any, Dict
 
 import torch
 import torch.nn as nn
 from torch import optim
 
-from torch_uncertainty.models.resnet import (
-    batched_resnet18,
-    batched_resnet34,
-    batched_resnet50,
-    batched_resnet101,
-    batched_resnet152,
-)
+from torch_uncertainty.models.wideresnet.batched import batched_wideresnet28x10
 from torch_uncertainty.routines.classification import ClassificationEnsemble
 
-# fmt: on
-archs = [
-    batched_resnet18,
-    batched_resnet34,
-    batched_resnet50,
-    batched_resnet101,
-    batched_resnet152,
-]
-choices = [18, 34, 50, 101, 152]
-
 
-class BatchedResNet(ClassificationEnsemble):
-    r"""LightningModule for BatchEnsembles ResNet.
+# fmt: on
+class BatchedWideResNet(ClassificationEnsemble):
+    r"""LightningModule for BatchEnsembles WideResNet.
 
     Args:
         num_classes (int): Number of classes to predict.
         num_estimators (int): Number of estimators in the ensemble.
         in_channels (int): Number of input channels.
-        arch (int):
-            Determines which ResNet architecture to use:
-
-            - ``18``: ResNet-18
-            - ``32``: ResNet-32
-            - ``50``: ResNet-50
-            - ``101``: ResNet-101
-            - ``152``: ResNet-152
-
         loss (torch.nn.Module): Training loss.
         optimization_procedure (Any): Optimization procedure, corresponds to
             what expect the `LightningModule.configure_optimizers()
             <https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#configure-optimizers>`_
             method.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
@@ -66,21 +42,21 @@
     """
 
     def __init__(
         self,
         num_classes: int,
         num_estimators: int,
         in_channels: int,
-        arch: Literal[18, 34, 50, 101, 152],
         loss: nn.Module,
         optimization_procedure: Any,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
+        imagenet_structure: bool = True,
         **kwargs: Dict[str, Any],
     ) -> None:
         super().__init__(
             num_classes=num_classes,
             num_estimators=num_estimators,
             use_entropy=use_entropy,
             use_logits=use_logits,
@@ -90,18 +66,19 @@
 
         # construct config
         self.save_hyperparameters(ignore=["loss", "optimization_procedure"])
 
         self.loss = loss
         self.optimization_procedure = optimization_procedure
 
-        self.model = archs[choices.index(arch)](
+        self.model = batched_wideresnet28x10(
             in_channels=in_channels,
             num_estimators=num_estimators,
             num_classes=num_classes,
+            imagenet_structure=imagenet_structure,
         )
 
         # to log the graph
         self.example_input_array = torch.randn(1, in_channels, 32, 32)
 
     def configure_optimizers(self) -> dict:
         param_optimizer = self.optimization_procedure(self)["optimizer"]
@@ -146,42 +123,42 @@
 
     @staticmethod
     def add_model_specific_args(
         parent_parser: ArgumentParser,
     ) -> ArgumentParser:
         """Defines the model's attributes via command-line options:
 
-        - ``--arch [int]``: defines :attr:`arch`. Defaults to ``18``.
         - ``--num_estimators [int]``: defines :attr:`num_estimators`. Defaults
           to ``1``.
+        - ``--imagenet_structure``: sets :attr:`imagenet_structure`. Defaults
+          to ``True``.
         - ``--entropy``: sets :attr:`use_entropy` to ``True``.
         - ``--logits``: sets :attr:`use_logits` to ``True``.
         - ``--mutual_information``: sets :attr:`use_mi` to ``True``.
         - ``--variation_ratio``: sets :attr:`use_variation_ratio` to ``True``.
 
         Example:
 
             .. parsed-literal::
 
-                python script.py --arch 18 --num_estimators 4 --alpha 2
+                python script.py --num_estimators 4
         """
+        parent_parser.add_argument("--num_estimators", type=int, default=4)
         parent_parser.add_argument(
-            "--arch",
-            type=int,
-            default=18,
-            choices=choices,
-            help="Type of ResNet",
+            "--imagenet_structure",
+            action=BooleanOptionalAction,
+            default=True,
+            help="Use imagenet structure",
         )
-        parent_parser.add_argument("--num_estimators", type=int, default=4)
         parent_parser.add_argument(
             "--entropy", dest="use_entropy", action="store_true"
         )
         parent_parser.add_argument(
             "--logits", dest="use_logits", action="store_true"
         )
         parent_parser.add_argument(
-            "--mutual_information", dest="uses_mi", action="store_true"
+            "--mutual_information", dest="use_mi", action="store_true"
         )
         parent_parser.add_argument(
             "--variation_ratio", dest="use_variation_ratio", action="store_true"
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/baselines/masked/resnet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/resnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fmt: off
-from argparse import ArgumentParser
+from argparse import ArgumentParser, BooleanOptionalAction
 from typing import Any, Dict, Literal
 
 import torch
 import torch.nn as nn
 
 from torch_uncertainty.models.resnet import (
     masked_resnet18,
@@ -82,14 +82,15 @@
         arch: Literal[18, 34, 50, 101, 152],
         loss: nn.Module,
         optimization_procedure: Any,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
+        imagenet_structure: bool = True,
         **kwargs: Dict[str, Any],
     ) -> None:
         super().__init__(
             num_classes=num_classes,
             num_estimators=num_estimators,
             use_entropy=use_entropy,
             use_logits=use_logits,
@@ -112,14 +113,15 @@
 
         self.model = archs[choices.index(arch)](
             in_channels=in_channels,
             num_estimators=num_estimators,
             scale=scale,
             groups=groups,
             num_classes=num_classes,
+            imagenet_structure=imagenet_structure,
         )
 
         # to log the graph
         self.example_input_array = torch.randn(1, in_channels, 32, 32)
 
     def configure_optimizers(self) -> dict:
         return self.optimization_procedure(self)
@@ -138,14 +140,16 @@
     ) -> ArgumentParser:
         """Defines the model's attributes via command-line options:
 
         - ``--arch [int]``: defines :attr:`arch`. Defaults to ``18``.
         - ``--num_estimators [int]``: defines :attr:`num_estimators`. Defaults
           to ``1``.
         - ``--scale [int]``: defines :attr:`scale`. Defaults to ``1``.
+        - ``--imagenet_structure``: sets :attr:`imagenet_structure`. Defaults
+          to ``True``.
         - ``--groups [int]``: defines :attr:`groups`. Defaults to ``1``.
         - ``--entropy``: sets :attr:`use_entropy` to ``True``.
         - ``--logits``: sets :attr:`use_logits` to ``True``.
         - ``--mutual_information``: sets :attr:`use_mi` to ``True``.
         - ``--variation_ratio``: sets :attr:`use_variation_ratio` to ``True``.
 
         Example:
@@ -157,23 +161,29 @@
         parent_parser.add_argument(
             "--arch",
             type=int,
             default=18,
             choices=choices,
             help="Type of ResNet",
         )
+        parent_parser.add_argument(
+            "--imagenet_structure",
+            action=BooleanOptionalAction,
+            default=True,
+            help="Use imagenet structure",
+        )
         parent_parser.add_argument("--scale", type=float, default=2.0)
         parent_parser.add_argument(
             "--entropy", dest="use_entropy", action="store_true"
         )
         parent_parser.add_argument("--groups", type=int, default=1)
         parent_parser.add_argument(
             "--logits", dest="use_logits", action="store_true"
         )
         parent_parser.add_argument(
-            "--mutual_information", dest="uses_mi", action="store_true"
+            "--mutual_information", dest="use_mi", action="store_true"
         )
         parent_parser.add_argument("--num_estimators", type=int, default=4)
         parent_parser.add_argument(
             "--variation_ratio", dest="use_variation_ratio", action="store_true"
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/baselines/packed/resnet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/wideresnet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,29 @@
 # fmt: off
-from argparse import ArgumentParser
-from typing import Any, Dict, Literal
+from argparse import ArgumentParser, BooleanOptionalAction
+from typing import Any, Dict
 
 import torch
 import torch.nn as nn
 
-from torch_uncertainty.models.resnet import (
-    packed_resnet18,
-    packed_resnet34,
-    packed_resnet50,
-    packed_resnet101,
-    packed_resnet152,
-)
+from torch_uncertainty.models.wideresnet.masked import masked_wideresnet28x10
 from torch_uncertainty.routines.classification import ClassificationEnsemble
 
 # fmt: on
-archs = [
-    packed_resnet18,
-    packed_resnet34,
-    packed_resnet50,
-    packed_resnet101,
-    packed_resnet152,
-]
-choices = [18, 34, 50, 101, 152]
 
 
-class PackedResNet(ClassificationEnsemble):
-    r"""LightningModule for Packed-Ensembles ResNet.
+class MaskedWideResNet(ClassificationEnsemble):
+    r"""LightningModule for Masksembles WideResNet.
 
     Args:
         num_classes (int): Number of classes to predict.
         num_estimators (int): Number of estimators in the ensemble.
         in_channels (int): Number of input channels.
-        alpha (int): Expansion factor affecting the width of the estimators.
-        gamma (int): Number of groups within each estimator.
-        arch (int):
-            Determines which ResNet architecture to use:
-
-            - ``18``: ResNet-18
-            - ``32``: ResNet-32
-            - ``50``: ResNet-50
-            - ``101``: ResNet-101
-            - ``152``: ResNet-152
-
+        scale (int): Expansion factor affecting the width of the estimators.
+        groups (int): Number of groups within each estimator.
         loss (torch.nn.Module): Training loss.
         optimization_procedure (Any): Optimization procedure, corresponds to
             what expect the `LightningModule.configure_optimizers()
             <https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#configure-optimizers>`_
             method.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
@@ -54,124 +31,114 @@
             OOD criterion or not. Defaults to ``False``.
         use_mi (bool, optional): Indicates whether to use the mutual
             information as the OOD criterion or not. Defaults to ``False``.
         use_variation_ratio (bool, optional): Indicates whether to use the
             variation ratio as the OOD criterion or not. Defaults to ``False``.
 
     Note:
-
         The OOD criterion is by defaults the confidence score.
 
     Warning:
-
         Make sure at most only one of :attr:`use_entropy`, :attr:`use_logits`,
         :attr:`use_mi` and :attr:`use_variation_ratio` attributes is set to
         ``True``. Otherwise a :class:`ValueError()` will be raised.
-
-    Raises:
-            ValueError: If :attr:`alpha`:math:`<1`.
-            ValueError: If :attr:`gamma`:math:`<1`.
     """
 
     def __init__(
         self,
         num_classes: int,
         num_estimators: int,
         in_channels: int,
-        alpha: int,
-        gamma: int,
-        arch: Literal[18, 34, 50, 101, 152],
+        scale: int,
+        groups: int,
         loss: nn.Module,
         optimization_procedure: Any,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
+        imagenet_structure: bool = True,
         **kwargs: Dict[str, Any],
     ) -> None:
         super().__init__(
             num_classes=num_classes,
             num_estimators=num_estimators,
             use_entropy=use_entropy,
             use_logits=use_logits,
             use_mi=use_mi,
             use_variation_ratio=use_variation_ratio,
         )
 
-        if alpha <= 0:
-            raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
-        if gamma < 1:
-            raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
-
         # construct config
         self.save_hyperparameters(ignore=["loss", "optimization_procedure"])
 
         self.loss = loss
         self.optimization_procedure = optimization_procedure
 
-        self.model = archs[choices.index(arch)](
+        self.model = masked_wideresnet28x10(
             in_channels=in_channels,
             num_estimators=num_estimators,
-            alpha=alpha,
-            gamma=gamma,
+            scale=scale,
+            groups=groups,
             num_classes=num_classes,
+            imagenet_structure=imagenet_structure,
         )
 
         # to log the graph
         self.example_input_array = torch.randn(1, in_channels, 32, 32)
 
     def configure_optimizers(self) -> dict:
         return self.optimization_procedure(self)
 
     @property
     def criterion(self) -> nn.Module:
         return self.loss()
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # type: ignore
-        input = input.repeat(1, self.num_estimators, 1, 1)
+        input = input.repeat(self.num_estimators, 1, 1, 1)
         return self.model.forward(input)
 
     @staticmethod
     def add_model_specific_args(
         parent_parser: ArgumentParser,
     ) -> ArgumentParser:
         """Defines the model's attributes via command-line options:
 
-        - ``--arch [int]``: defines :attr:`arch`. Defaults to ``18``.
         - ``--num_estimators [int]``: defines :attr:`num_estimators`. Defaults
           to ``1``.
-        - ``--alpha [int]``: defines :attr:`alpha`. Defaults to ``1``.
-        - ``--gamma [int]``: defines :attr:`gamma`. Defaults to ``1``.
         - ``--entropy``: sets :attr:`use_entropy` to ``True``.
         - ``--logits``: sets :attr:`use_logits` to ``True``.
         - ``--mutual_information``: sets :attr:`use_mi` to ``True``.
         - ``--variation_ratio``: sets :attr:`use_variation_ratio` to ``True``.
+        - ``--scale [float]``: defines :attr:`scale`. Defaults to ``2.0``.
+        - ``--imagenet_structure``: sets :attr:`imagenet_structure`. Defaults
+          to ``True``.
+        - ``--groups [int]``: defines :attr:`groups`. Defaults to ``1``.
 
         Example:
 
             .. parsed-literal::
 
-                python script.py --arch 18 --num_estimators 4 --alpha 2
+                python script.py --num_estimators 4 --scale 2.0 --groups 1
         """
+        parent_parser.add_argument("--num_estimators", type=int, default=4)
         parent_parser.add_argument(
-            "--arch",
-            type=int,
-            default=18,
-            choices=choices,
-            help="Type of ResNet",
+            "--imagenet_structure",
+            action=BooleanOptionalAction,
+            default=True,
+            help="Use imagenet structure",
         )
-        parent_parser.add_argument("--alpha", type=int, default=2)
         parent_parser.add_argument(
             "--entropy", dest="use_entropy", action="store_true"
         )
-        parent_parser.add_argument("--gamma", type=int, default=1)
         parent_parser.add_argument(
             "--logits", dest="use_logits", action="store_true"
         )
         parent_parser.add_argument(
-            "--mutual_information", dest="uses_mi", action="store_true"
+            "--mutual_information", dest="use_mi", action="store_true"
         )
-        parent_parser.add_argument("--num_estimators", type=int, default=4)
         parent_parser.add_argument(
             "--variation_ratio", dest="use_variation_ratio", action="store_true"
         )
+        parent_parser.add_argument("--scale", type=float, default=2.0)
+        parent_parser.add_argument("--groups", type=int, default=1)
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datamodules/cifar10.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar10.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,124 +6,107 @@
 import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
 from torch.utils.data import DataLoader, Dataset, random_split
 from torchvision.datasets import CIFAR10, SVHN
 
-from ..datasets import CIFAR10_C, AggregatedDataset
+from ..datasets import CIFAR10_C, CIFAR10_H, AggregatedDataset
 from ..transforms import Cutout
 
 
 # fmt: on
 class CIFAR10DataModule(LightningDataModule):
+    num_classes = 10
+    num_channels = 3
+
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
-        enable_cutout: bool = False,
+        cutout: int = None,
         auto_augment: str = None,
-        use_cifar_c: str = None,
+        test_alt: str = None,
         corruption_severity: int = 1,
         num_dataloaders: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
         self.root: Path = root
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
-        self.enable_cutout = enable_cutout
-        self.auto_augment = auto_augment
         self.num_dataloaders = num_dataloaders
-        self.num_classes = 10
-        self.num_channels = 3
 
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
 
-        if use_cifar_c is None:
-            self.dataset = CIFAR10
-        else:
+        if test_alt == "c":
             self.dataset = CIFAR10_C
+        elif test_alt == "h":
+            self.dataset = CIFAR10_H
+        else:
+            self.dataset = CIFAR10
 
-        self.use_cifar_c = use_cifar_c
+        self.test_alt = test_alt
         self.corruption_severity = corruption_severity
         self.ood_dataset = SVHN
 
-        if enable_cutout:
-            main_transform = Cutout(16)
+        if cutout:
+            main_transform = Cutout(cutout)
         elif auto_augment:
-            main_transform = rand_augment_transform(self.auto_augment, {})
+            main_transform = rand_augment_transform(auto_augment, {})
         else:
             main_transform = nn.Identity()
 
         self.transform_train = T.Compose(
             [
                 T.RandomCrop(32, padding=4),
                 T.RandomHorizontalFlip(),
-                T.ToTensor(),
-                T.Normalize(
-                    (0.4914, 0.4822, 0.4465),
-                    (0.2023, 0.1994, 0.2010),
-                ),
                 main_transform,
-            ]
-        )
-
-        self.transform_test = T.Compose(
-            [
                 T.ToTensor(),
                 T.Normalize(
                     (0.4914, 0.4822, 0.4465),
                     (0.2023, 0.1994, 0.2010),
                 ),
             ]
         )
 
-        self.transform_test_imagenet = T.Compose(
+        self.transform_test = T.Compose(
             [
                 T.ToTensor(),
-                T.RandomCrop(32),
-                T.RandomHorizontalFlip(),
                 T.Normalize(
                     (0.4914, 0.4822, 0.4465),
                     (0.2023, 0.1994, 0.2010),
                 ),
             ]
         )
 
     def prepare_data(self) -> None:
-        if self.use_cifar_c is None:
+        if self.test_alt != "c":
             self.dataset(self.root, train=True, download=True)
             self.dataset(self.root, train=False, download=True)
         else:
             self.dataset(
                 self.root,
-                subset=self.use_cifar_c,
                 severity=self.corruption_severity,
             )
 
-        # if self.use_imagenet_o:
-        #     self.ood_dataset(self.root)
-        # else:
         self.ood_dataset(self.root, split="test", download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
-            assert (
-                self.use_cifar_c is None
-            ), "CIFAR-C can only be used in testing."
+            assert self.test_alt != "c", "CIFAR-C can only be used in testing."
             full = self.dataset(
                 self.root,
                 train=True,
                 download=False,
                 transform=self.transform_train,
             )
             self.train, self.val = random_split(
@@ -139,30 +122,23 @@
         elif stage == "test" or stage is None:
             self.test = self.dataset(
                 self.root,
                 train=False,
                 download=False,
                 transform=self.transform_test,
             )
-            # if self.use_imagenet_o:
-            #     self.ood = self.ood_dataset(
-            #         self.root,
-            #         transform=self.transform_test_imagenet,
-            #     )
-            # else:
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
                 download=False,
                 transform=self.transform_test,
             )
         else:
             self.test = self.dataset(
                 self.root,
-                subset=self.use_cifar_c,
                 severity=self.corruption_severity,
                 transform=self.transform_test,
             )
 
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
@@ -186,21 +162,14 @@
     def val_dataloader(self) -> DataLoader:
         r"""Gets the validation dataloader for CIFAR10.
         Returns:
             DataLoader: CIFAR10 validation dataloader.
         """
         return self._data_loader(self.val)
 
-    def predict_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for CIFAR10.
-        Returns:
-            DataLoader: CIFAR10 validation dataloader.
-        """
-        return self._data_loader(self.val)
-
     def test_dataloader(self) -> List[DataLoader]:
         r"""Gets the test dataloaders for CIFAR10.
         Returns:
             List[DataLoader]: Dataloaders of the CIFAR10 test set (in
                 distribution data) and SVHN test split (out-of-distribution
                 data).
         """
@@ -225,17 +194,14 @@
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=128)
         p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
-        p.add_argument("--cutout", dest="enable_cutout", action="store_true")
+        p.add_argument("--cutout", type=int, default=0)
         p.add_argument("--auto_augment", type=str)
-        # p.add_argument(
-        #     "--imagenet-o", dest="use_imagenet_o", action="store_true"
-        # )
-        p.add_argument("--cifar-c", dest="use_cifar_c", type=str, default=None)
+        p.add_argument("--test_alt", choices=["c", "h"], default=None)
         p.add_argument(
             "--severity", dest="corruption_severity", type=int, default=None
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datamodules/cifar100.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/imagenet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,191 +1,173 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
-import torch
-import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
-from torch.utils.data import DataLoader, Dataset, random_split
-from torchvision.datasets import CIFAR100, SVHN
+from torch.utils.data import DataLoader, Dataset
+from torchvision.datasets import DTD, SVHN, ImageNet, INaturalist
 
-from ..datasets import CIFAR100_C, AggregatedDataset
-from ..transforms import Cutout
+from ..datasets import ImageNetO, ImageNetR
 
 
 # fmt: on
-class CIFAR100DataModule(LightningDataModule):
+class ImageNetDataModule(LightningDataModule):
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
-        enable_cutout: bool = False,
-        enable_randaugment: bool = False,
-        auto_augment: str = None,
-        use_cifar_c: str = None,
-        corrupution_severity: int = 1,
-        num_dataloaders: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
+        ood_name: str = "svhn",
+        test_option: str = None,
+        # num_ops: int = 2,
+        # magnitude: float = 15,
+        procedure: str = "A3",
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
-        self.enable_cutout = enable_cutout
-        self.enable_randaugment = enable_randaugment
-        self.auto_augment = auto_augment
-        self.num_dataloaders = num_dataloaders
-        self.num_classes = 100
-        self.num_channels = 3
-
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
+        self.ood_name = ood_name
+        self.num_classes = 1000
+        self.num_channels = 3
 
-        if use_cifar_c is None:
-            self.dataset = CIFAR100
+        if test_option is None:
+            self.dataset = ImageNet
+        elif test_option == "imagenet-r":
+            self.dataset = ImageNetR
         else:
-            self.dataset = CIFAR100_C
+            raise ValueError(f"Error, {test_option} not taken in charge.")
 
-        self.ood_dataset = SVHN
+        if ood_name == "inaturalist":
+            self.ood_dataset = INaturalist
+        elif ood_name == "imagenet-o":
+            self.ood_dataset = ImageNetO
+        elif ood_name == "svhn":
+            self.ood_dataset = SVHN
+        elif ood_name == "textures":
+            self.ood_dataset = DTD
+        else:
+            raise ValueError(f"The dataset {ood_name} is not supported.")
 
-        self.use_cifar_c = use_cifar_c
-        self.corruption_severity = corrupution_severity
+        self.procedure = procedure
 
-        assert (
-            self.enable_cutout
-            + self.enable_randaugment
-            + int(self.auto_augment is not None)
-            <= 1
-        ), "Only one data augmentation can be chosen at a time."
-
-        if enable_cutout:
-            main_transform = Cutout(8)
-        elif enable_randaugment:
-            main_transform = T.RandAugment(num_ops=2, magnitude=20)
-        elif auto_augment:
-            main_transform = rand_augment_transform(self.auto_augment, {})
+        if self.procedure == "Classic":
+            print("Classic Procedure")
+            train_size = 224
+        elif self.procedure == "A3":
+            print("Procedure A3")
+            train_size = 160
         else:
-            main_transform = nn.Identity()
+            raise ValueError("The procedure is unknown")
 
         self.transform_train = T.Compose(
             [
-                T.RandomCrop(32, padding=4),
+                T.RandomResizedCrop(train_size),
                 T.RandomHorizontalFlip(),
-                main_transform,
+                rand_augment_transform("rand-m6-mstd0.5-inc1", {}),
                 T.ToTensor(),
-                T.ConvertImageDtype(torch.float32),
-                T.Normalize(
-                    (0.5071, 0.4867, 0.4408),
-                    (0.2675, 0.2565, 0.2761),
-                ),
+                T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
             ]
         )
+
         self.transform_test = T.Compose(
             [
+                T.Resize(256),
+                T.CenterCrop(224),
                 T.ToTensor(),
-                T.Normalize(
-                    (0.5071, 0.4867, 0.4408),
-                    (0.2675, 0.2565, 0.2761),
-                ),
+                T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
             ]
         )
 
+    def _verify_splits(self, split: str) -> None:
+        if split not in list(self.root.iterdir()):
+            raise FileNotFoundError(
+                f"a {split} Imagenet split was not found in {self.root},"
+                f" make sure the folder contains a subfolder named {split}"
+            )
+
     def prepare_data(self) -> None:
-        if self.use_cifar_c is None:
-            self.dataset(self.root, train=True, download=True)
-            self.dataset(self.root, train=False, download=True)
-
-        self.ood_dataset(
-            self.root,
-            split="test",
-            download=True,
-            transform=self.transform_test,
-        )
+        if self.ood_name == "inaturalist":
+            self.ood = self.ood_dataset(
+                self.root,
+                version="2021_valid",
+                download=True,
+                transform=self.transform_test,
+            )
+        elif self.ood_name != "textures":
+            self.ood = self.ood_dataset(
+                self.root,
+                split="test",
+                download=True,
+                transform=self.transform_test,
+            )
+        else:
+            self.ood = self.ood_dataset(
+                self.root,
+                split="train",
+                download=True,
+                transform=self.transform_test,
+            )
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
-            assert (
-                self.use_cifar_c is None
-            ), "CIFAR-C can only be used in testing."
-            full = self.dataset(
+            self.train = self.dataset(
                 self.root,
-                train=True,
-                download=False,
+                split="train",
                 transform=self.transform_train,
             )
-            self.train, self.val = random_split(
-                full, [len(full) - self.val_split, self.val_split]
+            self.val = self.dataset(
+                self.root,
+                split="val",
+                transform=self.transform_test,
             )
-            if self.val_split == 0:
-                self.val = self.dataset(
-                    self.root,
-                    train=False,
-                    download=False,
-                    transform=self.transform_test,
-                )
-        elif stage == "test":
-            if self.use_cifar_c is None:
-                self.test = self.dataset(
+        if stage == "test" or stage is None:
+            self.test = self.dataset(
+                self.root,
+                split="val",
+                transform=self.transform_test,
+            )
+            if self.ood_name == "inaturalist":
+                self.ood = self.ood_dataset(
                     self.root,
-                    train=False,
-                    download=False,
+                    version="2021_valid",
                     transform=self.transform_test,
                 )
             else:
-                self.test = self.dataset(
+                self.ood = self.ood_dataset(
                     self.root,
                     transform=self.transform_test,
-                    subset=self.use_cifar_c,
-                    severity=self.corruption_severity,
+                    download=True,
                 )
-            self.ood = self.ood_dataset(
-                self.root,
-                split="test",
-                download=False,
-                transform=self.transform_test,
-            )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for CIFAR10.
-        Returns:
-            DataLoader: CIFAR10 training dataloader.
-        """
-        if self.num_dataloaders > 1:
-            return self._data_loader(
-                AggregatedDataset(self.train, self.num_dataloaders),
-                shuffle=True,
-            )
-        else:
-            return self._data_loader(self.train, shuffle=True)
+        return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for CIFAR100.
-        Returns:
-            DataLoader: CIFAR100 validation dataloader.
-        """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets the test dataloaders for CIFAR100.
+        r"""Gets test dataloaders for ImageNet.
         Returns:
-            List[DataLoader]: Dataloaders of the CIFAR100 test set (in
-                distribution data) and SVHN test split (out-of-distribution
-                data).
+            List[DataLoader]: ImageNet test set (in distribution data) and
+            Textures test split (out-of-distribution data).
         """
         return [self._data_loader(self.test), self._data_loader(self.ood)]
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
         return DataLoader(
@@ -201,20 +183,13 @@
     def add_argparse_args(
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
-        p.add_argument("--batch_size", type=int, default=128)
+        p.add_argument("--batch_size", type=int, default=256)
         p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
-        p.add_argument("--cutout", dest="enable_cutout", action="store_true")
-        p.add_argument(
-            "--randaugment", dest="enable_randaugment", action="store_true"
-        )
-        p.add_argument("--auto_augment", type=str)
-        p.add_argument("--cifar-c", dest="use_cifar_c", type=str, default=None)
-        p.add_argument(
-            "--severity", dest="corrupution_severity", type=int, default=1
-        )
+        p.add_argument("--ood_name", type=str, default="svhn")
+        p.add_argument("--test_option", type=str)
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datamodules/imagenet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar100.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,188 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
+import torch
+import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
 from torch.utils.data import DataLoader, Dataset, random_split
-from torchvision.datasets import DTD, SVHN, ImageNet, INaturalist
+from torchvision.datasets import CIFAR100, SVHN
 
-from ..datasets import ImageNetO, ImageNetR
+from ..datasets import CIFAR100_C, AggregatedDataset
+from ..transforms import Cutout
 
 
 # fmt: on
-class ImageNetDataModule(LightningDataModule):
+class CIFAR100DataModule(LightningDataModule):
+    num_classes = 100
+    num_channels = 3
+
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
+        cutout: int = None,
+        enable_randaugment: bool = False,
+        auto_augment: str = None,
+        test_alt: str = None,
+        corruption_severity: int = 1,
+        num_dataloaders: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
-        ood_name: str = "svhn",
-        test_option: str = None,
-        # num_ops: int = 2,
-        # magnitude: float = 15,
-        procedure: str = "A3",
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
+        self.num_dataloaders = num_dataloaders
+
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
-        self.ood_name = ood_name
-        self.num_classes = 1000
-        self.num_channels = 3
-
-        if test_option is None:
-            self.dataset = ImageNet
-        elif test_option == "imagenet-r":
-            self.dataset = ImageNetR
-        else:
-            raise ValueError(f"Error, {test_option} not taken in charge.")
 
-        if ood_name == "inaturalist":
-            self.ood_dataset = INaturalist
-        elif ood_name == "imagenet-o":
-            self.ood_dataset = ImageNetO
-        elif ood_name == "svhn":
-            self.ood_dataset = SVHN
-        elif ood_name == "textures":
-            self.ood_dataset = DTD
+        if test_alt == "c":
+            self.dataset = CIFAR100_C
         else:
-            raise ValueError(f"The dataset {ood_name} is not supported.")
+            self.dataset = CIFAR100
 
-        self.procedure = procedure
+        self.test_alt = test_alt
 
-        if self.procedure == "Classic":
-            print("Classic Procedure")
-            train_size = 224
-        elif self.procedure == "A3":
-            print("Procedure A3")
-            train_size = 160
+        self.ood_dataset = SVHN
+
+        self.corruption_severity = corruption_severity
+
+        if (cutout is not None) + enable_randaugment + int(
+            auto_augment is not None
+        ) > 1:
+            raise ValueError(
+                "Only one data augmentation can be chosen at a time. Raise a "
+                "GitHub issue if needed."
+            )
+
+        if cutout:
+            main_transform = Cutout(cutout)
+        elif enable_randaugment:
+            main_transform = T.RandAugment(num_ops=2, magnitude=20)
+        elif auto_augment:
+            main_transform = rand_augment_transform(auto_augment, {})
         else:
-            raise ValueError("The procedure is unknown")
+            main_transform = nn.Identity()
 
         self.transform_train = T.Compose(
             [
-                T.RandomResizedCrop(train_size),
+                T.RandomCrop(32, padding=4),
                 T.RandomHorizontalFlip(),
-                rand_augment_transform("rand-m6-mstd0.5-inc1", {}),
+                main_transform,
                 T.ToTensor(),
-                T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
+                T.ConvertImageDtype(torch.float32),
+                T.Normalize(
+                    (0.5071, 0.4867, 0.4408),
+                    (0.2675, 0.2565, 0.2761),
+                ),
             ]
         )
-
         self.transform_test = T.Compose(
             [
-                T.Resize(256),
-                T.CenterCrop(224),
                 T.ToTensor(),
-                T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
+                T.Normalize(
+                    (0.5071, 0.4867, 0.4408),
+                    (0.2675, 0.2565, 0.2761),
+                ),
             ]
         )
 
-    def _verify_splits(self, split: str) -> None:
-        if split not in list(self.root.iterdir()):
-            raise FileNotFoundError(
-                f"a {split} Imagenet split was not found in {self.root},"
-                f" make sure the folder contains a subfolder named {split}"
-            )
-
     def prepare_data(self) -> None:
-        if self.ood_name == "inaturalist":
-            self.ood = self.ood_dataset(
-                self.root,
-                version="2021_valid",
-                download=True,
-                transform=self.transform_test,
-            )
-        elif self.ood_name != "textures":
-            self.ood = self.ood_dataset(
-                self.root,
-                split="test",
-                download=True,
-                transform=self.transform_test,
-            )
-        else:
-            self.ood = self.ood_dataset(
-                self.root,
-                split="train",
-                download=True,
-                transform=self.transform_test,
-            )
+        if self.test_alt is None:
+            self.dataset(self.root, train=True, download=True)
+            self.dataset(self.root, train=False, download=True)
+
+        self.ood_dataset(
+            self.root,
+            split="test",
+            download=True,
+            transform=self.transform_test,
+        )
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
+            assert self.test_alt != "c", "CIFAR-C can only be used in testing."
             full = self.dataset(
                 self.root,
-                split="train",
+                train=True,
+                download=False,
                 transform=self.transform_train,
             )
             self.train, self.val = random_split(
                 full, [len(full) - self.val_split, self.val_split]
             )
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
-                    split="val",
+                    train=False,
+                    download=False,
                     transform=self.transform_test,
                 )
-        if stage == "test" or stage is None:
-            self.test = self.dataset(
-                self.root,
-                split="val",
-                transform=self.transform_test,
-            )
-            if self.ood_name == "inaturalist":
-                self.ood = self.ood_dataset(
+        elif stage == "test":
+            if self.test_alt is None:
+                self.test = self.dataset(
                     self.root,
-                    version="2021_valid",
+                    train=False,
+                    download=False,
                     transform=self.transform_test,
                 )
             else:
-                self.ood = self.ood_dataset(
+                self.test = self.dataset(
                     self.root,
                     transform=self.transform_test,
-                    download=True,
+                    severity=self.corruption_severity,
                 )
+            self.ood = self.ood_dataset(
+                self.root,
+                split="test",
+                download=False,
+                transform=self.transform_test,
+            )
 
     def train_dataloader(self) -> DataLoader:
-        return self._data_loader(self.train, shuffle=True)
+        r"""Gets the training dataloader for CIFAR100.
+        Returns:
+            DataLoader: CIFAR100 training dataloader.
+        """
+        if self.num_dataloaders > 1:
+            return self._data_loader(
+                AggregatedDataset(self.train, self.num_dataloaders),
+                shuffle=True,
+            )
+        else:
+            return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
+        r"""Gets the validation dataloader for CIFAR100.
+        Returns:
+            DataLoader: CIFAR100 validation dataloader.
+        """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets test dataloaders for ImageNet.
+        r"""Gets the test dataloaders for CIFAR100.
         Returns:
-            List[DataLoader]: ImageNet test set (in distribution data) and SVHN
-                test split (out-of-distribution data).
+            List[DataLoader]: Dataloaders of the CIFAR100 test set (in
+                distribution data) and SVHN test split (out-of-distribution
+                data).
         """
         return [self._data_loader(self.test), self._data_loader(self.ood)]
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
         return DataLoader(
@@ -187,13 +198,20 @@
     def add_argparse_args(
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
-        p.add_argument("--batch_size", type=int, default=256)
+        p.add_argument("--batch_size", type=int, default=128)
         p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
-        p.add_argument("--ood_name", type=str, default="svhn")
-        p.add_argument("--test_option", type=str)
+        p.add_argument("--cutout", type=int, default=0)
+        p.add_argument(
+            "--randaugment", dest="enable_randaugment", action="store_true"
+        )
+        p.add_argument("--auto_augment", type=str)
+        p.add_argument("--test_alt", choices=["c"], default=None)
+        p.add_argument(
+            "--severity", dest="corruption_severity", type=int, default=1
+        )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datamodules/mnist.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/mnist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
+from torch import nn
 from torch.utils.data import DataLoader, Dataset, random_split
 from torchvision.datasets import MNIST, FashionMNIST
 
+from torch_uncertainty.transforms import Cutout
+
 
 # fmt: on
 class MNISTDataModule(LightningDataModule):
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
-        enable_cutout: bool = False,
+        cutout: int = None,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
-        self.enable_cutout = enable_cutout
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
         self.dataset = MNIST
         self.ood_dataset = FashionMNIST
         self.num_classes = 10
 
+        if cutout:
+            main_transform = Cutout(cutout)
+        else:
+            main_transform = nn.Identity()
+
         self.transform_train = T.Compose(
             [
+                main_transform,
                 T.ToTensor(),
                 T.RandomCrop(28, padding=4),
                 T.Normalize((0.1307,), (0.3081,)),
             ]
         )
         self.transform_test = T.Compose(
             [
@@ -99,21 +107,14 @@
     def val_dataloader(self) -> DataLoader:
         r"""Gets the validation dataloader for MNIST.
         Returns:
             DataLoader: MNIST validation dataloader.
         """
         return self._data_loader(self.val)
 
-    def predict_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for MNIST.
-        Returns:
-            DataLoader: MNIST validation dataloader.
-        """
-        return self._data_loader(self.val)
-
     def test_dataloader(self) -> List[DataLoader]:
         r"""Gets the test dataloaders for MNIST.
         Returns:
             List[DataLoader]: Dataloaders of the MNIST test set (in
                 distribution data) and FashionMNIST test split
                 (out-of-distribution data).
         """
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datamodules/tiny_imagenet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/aggregated_dataset.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/aggregated_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/cifar_c.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_c.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/imagenet_o.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_o.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/imagenet_r.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_r.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/mixing_set.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/mixing_set.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/datasets/tiny_imagenet.py` & `torch_uncertainty-0.1.1/torch_uncertainty/datasets/tiny_imagenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # fmt:off
 import os
 from collections import defaultdict
+from pathlib import Path
 from typing import Callable, Optional
 
 from PIL import Image
 from torch.utils.data import Dataset
 
 import numpy as np
 
@@ -84,15 +85,15 @@
         target_transform: Optional[Callable] = None,
         max_samples=None,
     ):
         self.split = split
         self.label_idx = 1  # from [image, id, nid, box]
         self.transform = transform
         self.target_transform = target_transform
-        self.root = root
+        self.root = Path(root)
 
         self.IMAGE_SHAPE = (64, 64, 3)
 
         self.samples = []
         self.label_data = []
 
         self.max_samples = max_samples
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/layers/batchens_layers.py` & `torch_uncertainty-0.1.1/torch_uncertainty/layers/batchens_layers.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/layers/masksembles_layers.py` & `torch_uncertainty-0.1.1/torch_uncertainty/layers/masksembles_layers.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/metrics/disagreement.py` & `torch_uncertainty-0.1.1/torch_uncertainty/metrics/jensen_shannon_divergence.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# fmt: off
-from typing import Any, List, Literal, Optional
+# fmt:off
+from typing import Any, Literal, Optional
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 from torchmetrics import Metric
-from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.data import dim_zero_cat
 
 
-# fmt: on
-class Disagreement(Metric):
-    """The Disagreement Metric to estimate the confidence of an ensemble of
-    estimators.
+# fmt:on
+class JensenShannonDivergence(Metric):
+    """The Generalized Jensen Shannon Divergence Metric to estimate the
+    epistemic uncertainty of an ensemble of estimators.
 
     Args:
         reduction (str, optional): Determines how to reduce over the
             :math:`B`/batch dimension:
 
             - ``'mean'`` [default]: Averages score across samples
             - ``'sum'``: Sum score across samples
@@ -27,28 +26,36 @@
 
     Inputs:
         - :attr:`probs`: :math:`(B, N, C)`
 
         where :math:`B` is the batch size, :math:`C` is the number of classes
         and :math:`N` is the number of estimators.
 
+    See also:
+        The Jensen-Shannon Divergence on wikipedia
+        <https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence>`_.
+
+    Note:
+        A higher Jensen-Shannon divergence means a higher uncertainty.
+
     Note:
-        A higher disagreement means a lower confidence.
+        The generalized Jensen-Shannon divergence is computationnally
+            equivalent to the Mutual-Information.
 
     Warning:
         Make sure that the probabilities in :attr:`probs` are normalized to sum
         to one.
 
     Raises:
         ValueError:
             If :attr:`reduction` is not one of ``'mean'``, ``'sum'``,
             ``'none'`` or ``None``.
     """
 
-    is_differentiable: bool = False
+    full_state_update: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     def __init__(
         self,
         reduction: Literal["mean", "sum", "none", None] = "mean",
         **kwargs: Any,
@@ -70,89 +77,45 @@
                 default=torch.tensor(0.0),
                 dist_reduce_fx="sum",
             )
         else:
             self.add_state("values", default=[], dist_reduce_fx="cat")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
-    def _compute_disagreement(self, preds: Tensor) -> Tensor:
-        num_estimators = preds.size(-1)
-        counts = torch.sum(F.one_hot(preds), dim=1)
-        max_counts = num_estimators * (num_estimators - 1) / 2
-        return 1 - (counts * (counts - 1) / 2).sum(dim=1) / max_counts
-
-    def update(self, probs: Tensor) -> None:
-        """Update state with prediction probabilities and targets.
+    def update(self, probs: Tensor) -> None:  # type: ignore
+        """Update state with new data.
 
         Args:
             probs (torch.Tensor): Probabilities from the model.
         """
-        preds = probs.argmax(dim=-1)
+        batch_size = probs.size(0)
+        num_estimators = probs.size(1)
+        mean_probs = probs.mean(dim=1, keepdim=True).repeat(
+            1, probs.shape[1], 1
+        )
+        jsd = (
+            F.kl_div(
+                mean_probs.log(),
+                probs.log(),
+                log_target=True,
+                reduction="none",
+            ).sum(dim=(1, 2))
+            / num_estimators
+        )
+
         if self.reduction is None or self.reduction == "none":
-            self.values.append(self._compute_disagreement(preds))
+            self.values.append(jsd)
         else:
-            self.values += self._compute_disagreement(preds).sum(dim=-1)
-            self.total += probs.size(0)
+            self.values += jsd.sum()
+            self.total += batch_size
 
     def compute(self) -> Tensor:
-        """Compute Disagreement based on inputs passed in to ``update``."""
+        """Compute Jensen Shannon Divergence based on inputs passed in to
+        ``update``.
+        """
         values = dim_zero_cat(self.values)
         if self.reduction == "sum":
             return values.sum(dim=-1)
         elif self.reduction == "mean":
             return values.sum(dim=-1) / self.total
         else:  # reduction is None or "none"
             return values
-
-
-# TODO: Check dimension
-class Disagreement_old(Metric):
-    full_state_update: bool = False
-    probs: List[Tensor]
-
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
-
-        self.add_state("probs", [], dist_reduce_fx="cat")
-
-        rank_zero_warn(
-            "Metric `Disagreement` will save all targets and predictions"
-            " in buffer. For large datasets this may lead to large memory"
-            " footprint."
-        )
-
-    def update(self, probs: Tensor) -> None:  # type: ignore
-        # store data as (example, estimator, class)
-        self.probs.append(probs.transpose(0, 1))
-
-    def _compute_disagreement(self, classes: Tensor) -> Tensor:
-        r"""Computes the disagreement between the predicted classes among
-        all pairs of estimators.
-        Args:
-            classes (Tensor): Classes predicted by the `n_estimators`
-                estimators.
-        Returns:
-            Tensor: Mean disagreement between estimators.
-        """
-        # TODO: Using onehot might be memory intensive
-        n_estimators = classes.shape[-1]
-        counts = torch.sum(F.one_hot(classes), dim=1)
-        max_counts = n_estimators * (n_estimators - 1) / 2
-        return torch.mean(
-            1 - (counts * (counts - 1) / 2).sum(dim=1) / max_counts
-        )
-
-    def compute(self) -> Tensor:
-        probs = dim_zero_cat(self.probs)
-        classes = probs.argmax(dim=-1)
-        return self._compute_disagreement(classes)
-
-
-if __name__ == "__main__":
-    input = torch.softmax(torch.randn(8, 5, 4), dim=-1)  # (B, N, C)
-
-    disagreement_old = Disagreement_old()
-    disagreement = Disagreement()
-
-    assert disagreement_old(input.transpose(0, 1)) == disagreement(input)
-
-    print("All good!")
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/metrics/fpr95.py` & `torch_uncertainty-0.1.1/torch_uncertainty/metrics/fpr95.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/metrics/jensen_shannon_divergence.py` & `torch_uncertainty-0.1.1/torch_uncertainty/metrics/brier_score.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,119 @@
-# fmt:off
-from typing import Any, Literal, Optional
+# fmt: off
+from typing import Literal, Optional
 
 import torch
 import torch.nn.functional as F
-from torch import Tensor
 from torchmetrics import Metric
-from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.data import dim_zero_cat
 
 
 # fmt:on
-class JensenShannonDivergence(Metric):
-    """The Jensen Shannon Divergence Metric to estimate the epistemic
-    uncertainty of an ensemble of estimators.
+class BrierScore(Metric):
+    r"""The Brier Score Metric.
 
     Args:
         reduction (str, optional): Determines how to reduce over the
             :math:`B`/batch dimension:
 
             - ``'mean'`` [default]: Averages score across samples
             - ``'sum'``: Sum score across samples
             - ``'none'`` or ``None``: Returns score per sample
 
         kwargs: Additional keyword arguments, see `Advanced metric settings
             <https://torchmetrics.readthedocs.io/en/stable/pages/overview.html#metric-kwargs>`_.
 
     Inputs:
-        - :attr:`probs`: :math:`(B, N, C)`
+        - :attr:`probs`: :math:`(B, C)` or :math:`(B, N, C)`
+        - :attr:`target`: :math:`(B)` or :math:`(B, C)`
 
         where :math:`B` is the batch size, :math:`C` is the number of classes
         and :math:`N` is the number of estimators.
 
     Note:
-        A higher Jensen-Shannon divergence means a higher uncertainty.
+        If :attr:`probs` is a 3D tensor, then the metrics computes the mean of
+        the Brier score over the estimators ie. :math:`t = \frac{1}{N}
+        \sum_{i=0}^{N-1} BrierScore(probs[:,i,:], target)`.
 
     Warning:
         Make sure that the probabilities in :attr:`probs` are normalized to sum
         to one.
 
     Raises:
         ValueError:
             If :attr:`reduction` is not one of ``'mean'``, ``'sum'``,
             ``'none'`` or ``None``.
     """
 
-    full_state_update: bool = False
-    higher_is_better: Optional[bool] = None
+    is_differentiable: bool = False
+    higher_is_better: Optional[bool] = False
     full_state_update: bool = False
 
     def __init__(
         self,
+        num_classes: int,
         reduction: Literal["mean", "sum", "none", None] = "mean",
-        **kwargs: Any,
+        **kwargs,
     ) -> None:
         super().__init__(**kwargs)
 
         allowed_reduction = ("sum", "mean", "none", None)
         if reduction not in allowed_reduction:
             raise ValueError(
                 "Expected argument `reduction` to be one of ",
                 f"{allowed_reduction} but got {reduction}",
             )
 
+        self.num_classes = num_classes
         self.reduction = reduction
+        self.num_estimators = 1
 
         if self.reduction in ["mean", "sum"]:
             self.add_state(
-                "values",
-                default=torch.tensor(0.0),
-                dist_reduce_fx="sum",
+                "values", default=torch.tensor(0.0), dist_reduce_fx="sum"
             )
         else:
             self.add_state("values", default=[], dist_reduce_fx="cat")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
-    def update(self, probs: Tensor) -> None:  # type: ignore
-        """Update state with new data.
+    def update(self, probs: torch.Tensor, target: torch.Tensor) -> None:
+        """
+        Update the current Brier score with a new tensor of probabilities.
 
         Args:
-            probs (torch.Tensor): Probabilities from the model.
+            probs (torch.Tensor): A probability tensor of shape
+                (num_estimators, batch, num_classes) or
+                (batch, num_classes)
         """
-        batch_size = probs.size(0)
-        num_estimators = probs.size(1)
-        mean_probs = probs.mean(dim=1, keepdim=True).repeat(
-            1, probs.shape[1], 1
-        )
-        jsd = (
-            F.kl_div(
-                mean_probs.log(),
-                probs.log(),
-                log_target=True,
-                reduction="none",
-            ).sum(dim=(1, 2))
-            / num_estimators
-        )
+        if len(target.shape) == 1:
+            target = F.one_hot(target, self.num_classes)
+
+        print("target", target.shape, "probs", probs.shape)
+        if len(probs.shape) == 2:
+            batch_size = probs.size(0)
+        else:
+            batch_size = probs.size(0)
+            self.num_estimators = probs.size(1)
+            target = target.unsqueeze(1).repeat(1, self.num_estimators, 1)
+
+        brier_score = F.mse_loss(probs, target, reduction="none").sum(dim=-1)
 
         if self.reduction is None or self.reduction == "none":
-            self.values.append(jsd)
+            self.values.append(brier_score)
         else:
-            self.values += jsd.sum()
+            self.values += brier_score.sum()
             self.total += batch_size
 
-    def compute(self) -> Tensor:
-        """Compute Jensen Shannon Divergence based on inputs passed in to
-        ``update``.
+    def compute(self) -> torch.Tensor:
+        """
+        Compute the final Brier score based on inputs passed to ``update``.
+
+        Returns:
+            torch.Tensor: The final value(s) for the Brier score
         """
         values = dim_zero_cat(self.values)
         if self.reduction == "sum":
-            return values.sum(dim=-1)
+            return values.sum(dim=-1) / self.num_estimators
         elif self.reduction == "mean":
-            return values.sum(dim=-1) / self.total
-        else:  # reduction is None or "none"
+            return values.sum(dim=-1) / self.total / self.num_estimators
+        else:  # reduction is None
             return values
-
-
-class JensenShannonDivergence_old(Metric):
-    full_state_update: bool = False
-
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
-
-        self.add_state("probs", [], dist_reduce_fx="cat")
-
-        rank_zero_warn(
-            "Metric `JensenShannonDivergence` will save all "
-            "predictions in buffer. For large datasets this may lead to large "
-            "memory footprint."
-        )
-
-    def update(self, probs: Tensor) -> None:  # type: ignore
-        # store data as (example, estimator, class)
-        self.probs.append(probs.transpose(0, 1))
-
-    def compute(self) -> Tensor:
-        probs = dim_zero_cat(self.probs)
-        mean_proba = probs.mean(1, keepdim=True).repeat(1, probs.shape[1], 1)
-
-        return (
-            F.kl_div(
-                mean_proba.log(),
-                probs.log(),
-                log_target=True,
-                reduction="batchmean",
-            )
-            / probs.shape[1]
-        )
-
-
-if __name__ == "__main__":
-    import pytest
-
-    input = torch.softmax(torch.randn(8, 5, 4), dim=-1)  # (B, N, C)
-
-    mi_old = JensenShannonDivergence_old()
-    mi = JensenShannonDivergence()
-
-    print(mi_old(input.transpose(0, 1)))
-    print(mi(input))
-
-    assert mi_old(input.transpose(0, 1)) == pytest.approx(mi(input))
-
-    print("All good!")
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/metrics/nll.py` & `torch_uncertainty-0.1.1/torch_uncertainty/metrics/nll.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,17 @@
 # fmt: off
 from typing import Any, Literal, Optional
 
 import torch
 import torch.nn.functional as F
 from torchmetrics import Metric
-from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.data import dim_zero_cat
 
 
 # fmt: on
-class NegativeLogLikelihood_old(Metric):
-    full_state_update: bool = False
-
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
-
-        self.add_state("log_probs", [], dist_reduce_fx="cat")
-        self.add_state("targets", [], dist_reduce_fx="cat")
-
-        rank_zero_warn(
-            "Metric `NLLMetric` will save all targets and predictions"
-            " in buffer. For large datasets this may lead to large memory"
-            " footprint."
-        )
-
-    def update(self, probs: torch.Tensor, target: torch.Tensor) -> None:
-        self.log_probs.append(torch.log(probs))
-        self.targets.append(target)
-
-    def compute(self) -> torch.Tensor:
-        log_probs = dim_zero_cat(self.log_probs)
-        targets = dim_zero_cat(self.targets)
-        return F.nll_loss(log_probs, targets)
-
-
 class NegativeLogLikelihood(Metric):
     """The Negative Log Likelihood Metric.
 
     Args:
         reduction (str, optional): Determines how to reduce over the
             :math:`B`/batch dimension:
 
@@ -116,19 +90,7 @@
 
         if self.reduction == "sum":
             return values.sum(dim=-1)
         elif self.reduction == "mean":
             return values.sum(dim=-1) / self.total
         else:  # reduction is None or "none"
             return values
-
-
-if __name__ == "__main__":
-    input = torch.softmax(torch.randn(8, 4), dim=-1)
-    target = torch.randint(4, (8,))
-
-    nll = NegativeLogLikelihood_old()
-    nllv2 = NegativeLogLikelihood()
-
-    assert nll(input, target) == nllv2(input, target)
-
-    print("All good!")
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/metrics/variation_ratio.py` & `torch_uncertainty-0.1.1/torch_uncertainty/metrics/variation_ratio.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/batched.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/batched.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,55 +140,48 @@
         self,
         block,
         num_blocks,
         in_channels: int,
         num_estimators,
         num_classes=10,
         width_multiplier: int = 1,
-        # dataset: str = "cifar",
+        imagenet_structure: bool = True,
     ):
         super().__init__()
         self.in_planes = 64 * width_multiplier
-        # self.dataset = dataset
 
         self.width_multiplier = width_multiplier
-        # if dataset == "imagenet":
-        #     self.conv1 = BatchConv2d(
-        #         3,
-        #         64 * self.width_multiplier,
-        #         kernel_size=7,
-        #         stride=2,
-        #         padding=3,
-        #         bias=False,
-        #         num_estimators=num_estimators,
-        #     )
-
-        # elif dataset == "mnist":
-        #     self.conv1 = BatchConv2d(
-        #         1,
-        #         64 * self.width_multiplier,
-        #         kernel_size=3,
-        #         stride=1,
-        #         padding=1,
-        #         bias=False,
-        #         num_estimators=num_estimators,
-        #     )
-        # else:
-        self.conv1 = BatchConv2d(
-            in_channels,
-            64 * self.width_multiplier,
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            bias=False,
-            num_estimators=num_estimators,
-        )
+        if imagenet_structure:
+            self.conv1 = BatchConv2d(
+                3,
+                64 * self.width_multiplier,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                bias=False,
+                num_estimators=num_estimators,
+            )
+        else:
+            self.conv1 = BatchConv2d(
+                in_channels,
+                64 * self.width_multiplier,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                bias=False,
+                num_estimators=num_estimators,
+            )
         self.bn1 = nn.BatchNorm2d(64 * self.width_multiplier)
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
             block,
             64 * width_multiplier,
             num_blocks[0],
             stride=1,
             num_estimators=num_estimators,
@@ -229,142 +222,160 @@
         for stride in strides:
             layers.append(block(self.in_planes, planes, stride, num_estimators))
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x):
         out = F.relu(self.bn1(self.conv1(x)))
-        # if self.dataset == "imagenet" or self.dataset == "tinyimagenet":
-        #     out = F.max_pool2d(out, kernel_size=3, stride=2, padding=1)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
         return out
 
 
 def batched_resnet18(
-    in_channels: int, num_estimators: int, num_classes: int
+    in_channels: int,
+    num_estimators: int,
+    num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _BatchedResNet:
-    """BatchEnsembles of ResNet-18 from `Deep Residual Learning for Image
+    """BatchEnsemble of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
-        _BatchedResNet: A BatchEnsembles-style ResNet-18.
+        _BatchedResNet: A BatchEnsemble-style ResNet-18.
     """
     return _BatchedResNet(
         BasicBlock,
         [2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet34(
-    in_channels: int, num_estimators: int, num_classes: int
+    in_channels: int,
+    num_estimators: int,
+    num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _BatchedResNet:
-    """BatchEnsembles of ResNet-18 from `Deep Residual Learning for Image
+    """BatchEnsemble of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
-        _BatchedResNet: A BatchEnsembles-style ResNet-34.
+        _BatchedResNet: A BatchEnsemble-style ResNet-34.
     """
     return _BatchedResNet(
         BasicBlock,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet50(
     in_channels: int,
     num_estimators: int,
     num_classes: int,
     width_multiplier: int = 1,
+    imagenet_structure: bool = True,
 ) -> _BatchedResNet:
-    """BatchEnsembles of ResNet-18 from `Deep Residual Learning for Image
+    """BatchEnsemble of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
-        _BatchedResNet: A BatchEnsembles-style ResNet-50.
+        _BatchedResNet: A BatchEnsemble-style ResNet-50.
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         width_multiplier=width_multiplier,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet101(
-    in_channels: int, num_estimators: int, num_classes: int
+    in_channels: int,
+    num_estimators: int,
+    num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _BatchedResNet:
-    """BatchEnsembles of ResNet-18 from `Deep Residual Learning for Image
+    """BatchEnsemble of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
-        _BatchedResNet: A BatchEnsembles-style ResNet-101.
+        _BatchedResNet: A BatchEnsemble-style ResNet-101.
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet152(
-    in_channels: int, num_estimators: int, num_classes: int
+    in_channels: int,
+    num_estimators: int,
+    num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _BatchedResNet:
-    """BatchEnsembles of ResNet-18 from `Deep Residual Learning for Image
+    """BatchEnsemble of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _BatchedResNet: A BatchEnsembles-style ResNet-152.
+        _BatchedResNet: A BatchEnsemble-style ResNet-152.
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/masked.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/masked.py`

 * *Files 10% similar despite different names*

```diff
@@ -158,71 +158,56 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         scale: float = 2.0,
         groups: int = 1,
-        # dataset: str = "cifar",
+        imagenet_structure: bool = True,
     ) -> None:
         super().__init__()
-        # assert dataset in [
-        #     "cifar",
-        #     "mnist",
-        #     "tinyimagenet",
-        #     "imagenet",
-        # ], "The dataset is not taken in charge by this implementation."
-        # self.dataset = dataset
 
         self.in_channels = in_channels
         self.num_estimators = num_estimators
         self.in_planes = 64
         if self.in_planes % self.num_estimators:
             self.in_planes += (
                 self.num_estimators - self.in_planes % self.num_estimators
             )
         block_planes = self.in_planes
 
-        # No subgroups in the first layer
-        # if self.dataset == "imagenet":
-        #     self.conv1 = MaskedConv2d(
-        #         3 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=7,
-        #         stride=2,
-        #         padding=3,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # elif self.dataset == "mnist":
-        #     self.conv1 = MaskedConv2d(
-        #         1 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=3,
-        #         stride=1,
-        #         padding=1,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # else:
-        self.conv1 = nn.Conv2d(
-            self.in_channels,
-            block_planes,
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            groups=1,
-            bias=False,
-        )
+        if imagenet_structure:
+            self.conv1 = nn.Conv2d(
+                self.in_channels,
+                block_planes,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                groups=1,  # No groups for the first layer
+                bias=False,
+            )
+        else:
+            self.conv1 = nn.Conv2d(
+                self.in_channels,
+                block_planes,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                groups=1,
+                bias=False,
+            )
 
         self.bn1 = nn.BatchNorm2d(block_planes)
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
             block,
             block_planes,
             num_blocks[0],
             stride=1,
             num_estimators=num_estimators,
@@ -291,16 +276,14 @@
                 )
             )
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
         out = F.relu(self.bn1(self.conv1(x)))
-        # if self.dataset == "imagenet" or self.dataset == "tinyimagenet":
-        # out = F.max_pool2d(out, kernel_size=3, stride=2, padding=1)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
 
         out = self.pool(out)
@@ -311,14 +294,15 @@
 
 def masked_resnet18(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _MaskedResNet:
     """Masksembles of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -332,23 +316,25 @@
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def masked_resnet34(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _MaskedResNet:
     """Masksembles of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -362,23 +348,25 @@
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def masked_resnet50(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _MaskedResNet:
     """Masksembles of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -392,23 +380,25 @@
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def masked_resnet101(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _MaskedResNet:
     """Masksembles of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -422,38 +412,42 @@
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def masked_resnet152(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _MaskedResNet:
     """Masksembles of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
+        scale (float): Expansion factor affecting the width of the estimators.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
         _MaskedResNet: A Masksembles-style ResNet-152.
     """
     return _MaskedResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/packed.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/packed.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,114 +22,132 @@
     expansion = 1
 
     def __init__(
         self,
         in_planes: int,
         planes: int,
         stride: int = 1,
+        alpha: float = 2,
         num_estimators: int = 4,
         gamma: int = 1,
     ):
         super(BasicBlock, self).__init__()
 
         # No subgroups for the first layer
         self.conv1 = PackedConv2d(
             in_planes,
             planes,
             kernel_size=3,
+            alpha=alpha,
             num_estimators=num_estimators,
             stride=stride,
             padding=1,
             bias=False,
         )
-        self.bn1 = nn.BatchNorm2d(planes)
+        self.bn1 = nn.BatchNorm2d(planes * alpha)
         self.conv2 = PackedConv2d(
             planes,
             planes,
             kernel_size=3,
+            alpha=alpha,
             num_estimators=num_estimators,
+            gamma=gamma,
             stride=1,
             padding=1,
-            groups=gamma,
             bias=False,
         )
-        self.bn2 = nn.BatchNorm2d(planes)
+        self.bn2 = nn.BatchNorm2d(planes * alpha)
 
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != self.expansion * planes:
             self.shortcut = nn.Sequential(
                 PackedConv2d(
                     in_planes,
                     self.expansion * planes,
                     kernel_size=1,
+                    alpha=alpha,
                     num_estimators=num_estimators,
+                    gamma=gamma,
                     stride=stride,
-                    groups=gamma,
                     bias=False,
                 ),
-                nn.BatchNorm2d(self.expansion * planes),
+                nn.BatchNorm2d(self.expansion * planes * alpha),
             )
 
     def forward(self, x: Tensor) -> Tensor:
         out = F.relu(self.bn1(self.conv1(x)))
         out = self.bn2(self.conv2(out))
         out += self.shortcut(x)
         out = F.relu(out)
         return out
 
 
 class Bottleneck(nn.Module):
     expansion = 4
 
-    def __init__(self, in_planes, planes, stride=1, num_estimators=4, gamma=1):
+    def __init__(
+        self,
+        in_planes: int,
+        planes: int,
+        stride: int = 1,
+        alpha: float = 2,
+        num_estimators: int = 4,
+        gamma: int = 1,
+    ):
         super(Bottleneck, self).__init__()
 
         # No subgroups for the first layer
         self.conv1 = PackedConv2d(
             in_planes,
             planes,
             kernel_size=1,
+            alpha=alpha,
             num_estimators=num_estimators,
+            gamma=1,  # No groups in the first layer
             bias=False,
         )
-        self.bn1 = nn.BatchNorm2d(planes)
+        self.bn1 = nn.BatchNorm2d(planes * alpha)
         self.conv2 = PackedConv2d(
             planes,
             planes,
             kernel_size=3,
+            alpha=alpha,
             num_estimators=num_estimators,
+            gamma=gamma,
             stride=stride,
             padding=1,
-            groups=gamma,
+            groups=1,
             bias=False,
         )
-        self.bn2 = nn.BatchNorm2d(planes)
+        self.bn2 = nn.BatchNorm2d(planes * alpha)
         self.conv3 = PackedConv2d(
             planes,
             self.expansion * planes,
             kernel_size=1,
+            alpha=alpha,
             num_estimators=num_estimators,
-            groups=gamma,
+            gamma=gamma,
             bias=False,
         )
-        self.bn3 = nn.BatchNorm2d(self.expansion * planes)
+        self.bn3 = nn.BatchNorm2d(self.expansion * planes * alpha)
 
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != self.expansion * planes:
             self.shortcut = nn.Sequential(
                 PackedConv2d(
                     in_planes,
                     self.expansion * planes,
                     kernel_size=1,
+                    alpha=alpha,
                     num_estimators=num_estimators,
+                    gamma=gamma,
                     stride=stride,
-                    groups=gamma,
                     bias=False,
                 ),
-                nn.BatchNorm2d(self.expansion * planes),
+                nn.BatchNorm2d(self.expansion * planes * alpha),
             )
 
     def forward(self, x: Tensor) -> Tensor:
         out = F.relu(self.bn1(self.conv1(x)))
         out = F.relu(self.bn2(self.conv2(out)))
         out = self.bn3(self.conv3(out))
         out += self.shortcut(x)
@@ -143,157 +161,160 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         alpha: int = 2,
         gamma: int = 1,
-        # dataset: str = "cifar",
+        imagenet_structure: bool = True,
     ) -> None:
         super().__init__()
-        # assert dataset in [
-        #     "cifar",
-        #     "mnist",
-        #     "tinyimagenet",
-        #     "imagenet",
-        # ], "The dataset is not taken in charge by this implementation."
-        # self.dataset = dataset
 
         self.in_channels = in_channels
         self.num_estimators = num_estimators
-        self.in_planes = int(64 * alpha)
-        if self.in_planes % self.num_estimators:
-            self.in_planes += (
-                self.num_estimators - self.in_planes % self.num_estimators
-            )
+        self.in_planes = 64
         block_planes = self.in_planes
 
-        # No subgroups in the first layer
-        # if self.dataset == "imagenet":
-        #     self.conv1 = PackedConv2d(
-        #         3 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=7,
-        #         stride=2,
-        #         padding=3,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # elif self.dataset == "mnist":
-        #     self.conv1 = PackedConv2d(
-        #         1 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=3,
-        #         stride=1,
-        #         padding=1,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # else:
-        self.conv1 = PackedConv2d(
-            self.in_channels * self.num_estimators,
-            block_planes,
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            num_estimators=num_estimators,
-            groups=1,
-            bias=False,
-        )
+        if imagenet_structure:
+            self.conv1 = PackedConv2d(
+                self.in_channels,
+                block_planes,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                alpha=alpha,
+                num_estimators=num_estimators,
+                gamma=1,  # No groups for the first layer
+                groups=1,
+                bias=False,
+                first=True,
+            )
+        else:
+            self.conv1 = PackedConv2d(
+                self.in_channels,
+                block_planes,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                alpha=alpha,
+                num_estimators=num_estimators,
+                gamma=1,  # No groups for the first layer
+                groups=1,
+                bias=False,
+                first=True,
+            )
 
-        self.bn1 = nn.BatchNorm2d(block_planes)
+        self.bn1 = nn.BatchNorm2d(block_planes * alpha)
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
             block,
             block_planes,
             num_blocks[0],
             stride=1,
+            alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
         )
         self.layer2 = self._make_layer(
             block,
             block_planes * 2,
             num_blocks[1],
             stride=2,
+            alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
         )
         self.layer3 = self._make_layer(
             block,
             block_planes * 4,
             num_blocks[2],
             stride=2,
+            alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
         )
         self.layer4 = self._make_layer(
             block,
             block_planes * 8,
             num_blocks[3],
             stride=2,
+            alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
         )
 
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
         self.linear = PackedLinear(
             block_planes * 8 * block.expansion,
-            num_classes * num_estimators,
-            num_estimators,
+            num_classes,
+            alpha=alpha,
+            num_estimators=num_estimators,
+            last=True,
         )
 
     def _make_layer(
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         planes: int,
         num_blocks: int,
         stride: int,
+        alpha: float,
         num_estimators: int,
         gamma: int,
     ) -> nn.Module:
         strides = [stride] + [1] * (num_blocks - 1)
         layers = []
         for stride in strides:
             layers.append(
-                block(self.in_planes, planes, stride, num_estimators, gamma)
+                block(
+                    self.in_planes,
+                    planes,
+                    stride,
+                    alpha=alpha,
+                    num_estimators=num_estimators,
+                    gamma=gamma,
+                )
             )
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
         out = F.relu(self.bn1(self.conv1(x)))
-        # if self.dataset == "imagenet" or self.dataset == "tinyimagenet":
-        # out = F.max_pool2d(out, kernel_size=3, stride=2, padding=1)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
+
         out = rearrange(
             out, "e (m c) h w -> (m e) c h w", m=self.num_estimators
         )
+
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
         return out
 
 
 def packed_resnet18(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -308,23 +329,25 @@
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def packed_resnet34(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -339,23 +362,25 @@
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def packed_resnet50(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -370,23 +395,25 @@
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def packed_resnet101(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -401,39 +428,44 @@
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def packed_resnet152(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    imagenet_structure: bool = True,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-152.
     """
     return _PackedResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/resnet/std.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/std.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,65 +130,50 @@
     def __init__(
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         groups: int,
-        # dataset: str = "cifar",
+        imagenet_structure: bool = True,
     ) -> None:
         super().__init__()
-        # assert dataset in [
-        #     "cifar",
-        #     "mnist",
-        #     "tinyimagenet",
-        #     "imagenet",
-        # ], "The dataset is not taken in charge by this implementation."
-        # self.dataset = dataset
+
         self.in_planes = 64
         block_planes = self.in_planes
 
-        # if self.dataset == "imagenet":
-        #     self.conv1 = nn.Conv2d(
-        #         3 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=7,
-        #         stride=2,
-        #         padding=3,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # elif self.dataset == "mnist":
-        #     self.conv1 = nn.Conv2d(
-        #         1 * self.num_estimators,
-        #         block_planes,
-        #         kernel_size=3,
-        #         stride=1,
-        #         padding=1,
-        #         groups=1,
-        #         num_estimators=num_estimators,
-        #         bias=False,
-        #     )
-        # else:
-
-        # No groups in the first layer
-        self.conv1 = nn.Conv2d(
-            in_channels,
-            block_planes,
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            groups=1,
-            bias=False,
-        )
+        if imagenet_structure:
+            self.conv1 = nn.Conv2d(
+                in_channels,
+                block_planes,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                groups=1,  # No groups in the first layer
+                bias=False,
+            )
+        else:
+            self.conv1 = nn.Conv2d(
+                in_channels,
+                block_planes,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                groups=1,  # No groups in the first layer
+                bias=False,
+            )
 
         self.bn1 = nn.BatchNorm2d(block_planes)
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
             block,
             block_planes,
             num_blocks[0],
             stride=1,
             groups=groups,
@@ -257,127 +242,148 @@
         out = self.linear(out)
         return out
 
 
 def resnet18(
     in_channels: int,
     num_classes: int,
-    groups: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> _ResNet:
     """ResNet-18 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
-        groups (int): Number of groups in convolutions.
+        groups (int): Number of groups in convolutions. Defaults to 1.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _PackedResNet: A ResNet-18.
+        _ResNet: A ResNet-18.
     """
     return _ResNet(
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_classes=num_classes,
         groups=groups,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def resnet34(
     in_channels: int,
     num_classes: int,
-    groups: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> _ResNet:
     """ResNet-34 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
-        groups (int): Number of groups in convolutions.
+        groups (int): Number of groups in convolutions. Defaults to 1.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _PackedResNet: A ResNet-34.
+        _ResNet: A ResNet-34.
     """
     return _ResNet(
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def resnet50(
     in_channels: int,
     num_classes: int,
-    groups: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> _ResNet:
     """ResNet-50 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
-        groups (int): Number of groups in convolutions.
+        groups (int): Number of groups in convolutions. Defaults to 1.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _PackedResNet: A ResNet-50.
+        _ResNet: A ResNet-50.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def resnet101(
     in_channels: int,
     num_classes: int,
-    groups: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> _ResNet:
     """ResNet-101 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
-        groups (int): Number of groups in convolutions.
+        groups (int): Number of groups in convolutions. Defaults to 1.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _PackedResNet: A ResNet-101.
+        _ResNet: A ResNet-101.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
+        imagenet_structure=imagenet_structure,
     )
 
 
 def resnet152(
     in_channels: int,
     num_classes: int,
-    groups: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> _ResNet:
     """ResNet-152 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
-        groups (int): Number of groups in convolutions.
+        groups (int, optional): Number of groups in convolutions. Defaults to
+            ``1``.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
 
     Returns:
-        _PackedResNet: A ResNet-152.
+        _ResNet: A ResNet-152.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
-        groups=groups,
         num_classes=num_classes,
+        groups=groups,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/wideresnet/packed.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/batched.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,193 +1,217 @@
 # fmt: off
 import torch.nn as nn
 import torch.nn.functional as F
-from einops import rearrange
-
-from ...layers import PackedConv2d, PackedLinear
 
+from ...layers import BatchConv2d, BatchLinear
 
 # fmt: on
+__all__ = [
+    "batched_wideresnet28x10",
+]
+
+
 class WideBasicBlock(nn.Module):
     def __init__(
         self,
         in_planes,
         planes,
         dropout_rate,
         stride=1,
         num_estimators=4,
-        gamma=1,
     ):
         super().__init__()
         self.bn1 = nn.BatchNorm2d(in_planes)
-        self.conv1 = PackedConv2d(
+        self.conv1 = BatchConv2d(
             in_planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
             padding=1,
-            groups=gamma,
             bias=False,
         )
         self.dropout = nn.Dropout(p=dropout_rate)
         self.bn2 = nn.BatchNorm2d(planes)
-        self.conv2 = PackedConv2d(
+        self.conv2 = BatchConv2d(
             planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
             stride=stride,
             padding=1,
-            groups=gamma,
             bias=False,
         )
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != planes:
             self.shortcut = nn.Sequential(
-                PackedConv2d(
+                BatchConv2d(
                     in_planes,
                     planes,
                     kernel_size=1,
                     num_estimators=num_estimators,
                     stride=stride,
-                    groups=gamma,
                     bias=True,
                 ),
             )
 
     def forward(self, x):
         out = self.dropout(self.conv1(F.relu(self.bn1(x))))
         out = self.conv2(F.relu(self.bn2(out)))
         out += self.shortcut(x)
         return out
 
 
-class _PackedWide(nn.Module):
+class _BatchedWide(nn.Module):
     def __init__(
         self,
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         num_estimators: int,
-        dropout_rate: float,
-        alpha: int = 2,
-        gamma: int = 1,
+        dropout_rate: float = 0.0,
+        imagenet_structure: bool = True,
     ):
         super().__init__()
         self.num_estimators = num_estimators
-        self.in_planes = 16 * alpha
+        self.in_planes = 16
 
-        assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4"
+        assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         n = (depth - 4) / 6
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        self.conv1 = PackedConv2d(
-            in_channels * self.num_estimators,
-            nStages[0] * alpha,
-            kernel_size=3,
-            num_estimators=self.num_estimators,
-            stride=1,
-            padding=1,
-            groups=gamma,
-            bias=True,
-        )
+        if imagenet_structure:
+            self.conv1 = BatchConv2d(
+                in_channels,
+                nStages[0],
+                num_estimators=self.num_estimators,
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                bias=True,
+                groups=1,
+            )
+        else:
+            self.conv1 = BatchConv2d(
+                in_channels,
+                nStages[0],
+                num_estimators=self.num_estimators,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                bias=True,
+                groups=1,
+            )
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
             WideBasicBlock,
-            nStages[1] * alpha,
+            nStages[1],
             n,
             dropout_rate,
             stride=1,
             num_estimators=self.num_estimators,
-            gamma=gamma,
         )
         self.layer2 = self._wide_layer(
             WideBasicBlock,
-            nStages[2] * alpha,
+            nStages[2],
             n,
             dropout_rate,
             stride=2,
             num_estimators=self.num_estimators,
-            gamma=gamma,
         )
         self.layer3 = self._wide_layer(
             WideBasicBlock,
-            nStages[3] * alpha,
+            nStages[3],
             n,
             dropout_rate,
             stride=2,
             num_estimators=self.num_estimators,
-            gamma=gamma,
         )
-        self.bn1 = nn.BatchNorm2d(nStages[3] * alpha, momentum=0.9)
+        self.bn1 = nn.BatchNorm2d(nStages[3])
 
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
-        self.linear = PackedLinear(
-            nStages[3] * alpha,
-            num_classes * num_estimators,
+        self.linear = BatchLinear(
+            nStages[3],
+            num_classes,
             num_estimators,
         )
 
     def _wide_layer(
         self,
         block: nn.Module,
         planes: int,
         num_blocks: int,
         dropout_rate: float,
         stride: int,
         num_estimators: int,
-        gamma,
     ):
         strides = [stride] + [1] * (int(num_blocks) - 1)
         layers = []
 
         for stride in strides:
             layers.append(
                 block(
                     self.in_planes,
                     planes,
                     dropout_rate,
                     stride,
                     num_estimators,
-                    gamma,
                 )
             )
             self.in_planes = planes
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
         out = self.conv1(x)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = F.relu(self.bn1(out))
-        out = rearrange(
-            out, "e (m c) h w -> (m e) c h w", m=self.num_estimators
-        )
+
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
 
         return out
 
 
-def packed_wideresnet28x10(
-    num_estimators: int, alpha: int, gamma: int, num_classes: int
-) -> nn.Module:
-    return _PackedWide(
+def batched_wideresnet28x10(
+    in_channels: int,
+    num_estimators: int,
+    num_classes: int,
+    imagenet_structure: bool = True,
+) -> _BatchedWide:
+    """BatchEnsemble of Wide-ResNet-28x10 from `Wide Residual Networks
+    <https://arxiv.org/pdf/1605.07146.pdf>`_.
+
+    Args:
+        in_channels (int): Number of input channels.
+        num_estimators (int): Number of estimators in the ensemble.
+        num_classes (int): Number of classes to predict.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
+
+    Returns:
+        _BatchedWide: A BatchEnsemble-style Wide-ResNet-28x10.
+    """
+    return _BatchedWide(
+        in_channels=in_channels,
         depth=28,
         widen_factor=10,
         dropout_rate=0.3,
         num_classes=num_classes,
         num_estimators=num_estimators,
-        alpha=alpha,
-        gamma=gamma,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/models/wideresnet/std.py` & `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/std.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # fmt: off
 from typing import Type
 
 import torch.nn as nn
 import torch.nn.functional as F
-from einops import rearrange
-
 
 # fmt: on
+__all__ = [
+    "wideresnet28x10",
+]
+
+
 class WideBasicBlock(nn.Module):
     def __init__(
         self,
         in_planes,
         planes,
         dropout_rate,
         stride=1,
@@ -62,35 +65,52 @@
         self,
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         dropout_rate: float,
         groups: int = 1,
+        imagenet_structure: bool = True,
     ):
         super().__init__()
         self.in_planes = 16
 
-        assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4"
+        assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         num_blocks = int((depth - 4) / 6)
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        self.conv1 = nn.Conv2d(
-            in_channels,
-            nStages[0],
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            groups=groups,
-            bias=True,
-        )
+        if imagenet_structure:
+            self.conv1 = nn.Conv2d(
+                in_channels,
+                nStages[0],
+                kernel_size=7,
+                stride=2,
+                padding=3,
+                groups=groups,
+                bias=True,
+            )
+        else:
+            self.conv1 = nn.Conv2d(
+                in_channels,
+                nStages[0],
+                kernel_size=3,
+                stride=1,
+                padding=1,
+                groups=groups,
+                bias=True,
+            )
 
-        self.optional_pool = nn.Identity()
+        if imagenet_structure:
+            self.optional_pool = nn.MaxPool2d(
+                kernel_size=3, stride=2, padding=1
+            )
+        else:
+            self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
             WideBasicBlock,
             nStages[1],
             num_blocks=num_blocks,
             dropout_rate=dropout_rate,
             stride=1,
@@ -151,28 +171,43 @@
     def forward(self, x):
         out = self.conv1(x)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = F.relu(self.bn1(out))
-        out = rearrange(
-            out, "e (m c) h w -> (m e) c h w", m=self.num_estimators
-        )
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
 
         return out
 
 
 def wideresnet28x10(
-    in_channels: int, groups: int, num_classes: int
+    in_channels: int,
+    num_classes: int,
+    groups: int = 1,
+    imagenet_structure: bool = True,
 ) -> nn.Module:
+    """Wide-ResNet-28x10 from `Wide Residual Networks
+    <https://arxiv.org/pdf/1605.07146.pdf>`_.
+
+    Args:
+        in_channels (int): Number of input channels
+        num_classes (int): Number of classes to predict.
+        groups (int, optional): Number of groups in convolutions. Defaults to
+            ``1``.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
+
+    Returns:
+        _Wide: A Wide-ResNet-28x10.
+    """
     return _Wide(
         depth=28,
         widen_factor=10,
         in_channels=in_channels,
         dropout_rate=0.3,
         num_classes=num_classes,
         groups=groups,
+        imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/optimization_procedures.py` & `torch_uncertainty-0.1.1/torch_uncertainty/optimization_procedures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # fmt: off
 import torch.nn as nn
 import torch.optim as optim
 from timm.optim import Lamb
 
-
 # fmt:on
+__all__ = [
+    "optim_cifar10_resnet18",
+    "optim_cifar10_resnet50",
+    "optim_cifar10_wideresnet",
+    "optim_cifar100_resnet18",
+    "optim_cifar100_resnet50",
+    "optim_imagenet_resnet50",
+    "optim_imagenet_resnet50_A3",
+]
+
+
 def optim_cifar10_resnet18(model: nn.Module) -> dict:
     """optimizer to train a ResNet18 on CIFAR-10"""
     optimizer = optim.SGD(
         model.parameters(),
         lr=0.05,
         momentum=0.9,
         weight_decay=5e-4,
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/routines/classification.py` & `torch_uncertainty-0.1.1/torch_uncertainty/routines/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,16 @@
         self,
         num_classes: int,
         use_entropy: bool = False,
         use_logits: bool = False,
     ) -> None:
         super().__init__()
 
-        # FIXME: use ValueError instead
-        assert (
-            use_logits + use_entropy
-        ) <= 1, "You cannot choose more than one OOD criterion."
+        if (use_logits + use_entropy) > 1:
+            raise ValueError("You cannot choose more than one OOD criterion.")
 
         self.num_classes = num_classes
         self.use_logits = use_logits
         self.use_entropy = use_entropy
 
         # metrics
         cls_metrics = MetricCollection(
@@ -195,21 +193,21 @@
         )
 
         self.num_estimators = num_estimators
 
         self.use_mi = use_mi
         self.use_variation_ratio = use_variation_ratio
 
-        # FIXME: use ValueError instead
-        assert (
+        if (
             self.use_logits
             + self.use_entropy
             + self.use_mi
             + self.use_variation_ratio
-        ) <= 1, "You cannot choose more than one OOD criterion."
+        ) > 1:
+            raise ValueError("You cannot choose more than one OOD criterion.")
 
         # metrics for ensembles only
         ens_metrics = MetricCollection(
             {
                 "disagreement": Disagreement(),
                 "mi": MutualInformation(),
                 "entropy": Entropy(),
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/transforms/cutout.py` & `torch_uncertainty-0.1.1/torch_uncertainty/transforms/cutout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # fmt: off
 import torch
 
 import numpy as np
 
-# fmt: on
-
 
+# fmt: on
 class Cutout:
     """
     Reference : https://github.com/quark0/darts/blob/master/cnn/utils.py
     """
 
-    def __init__(self, length: int):
-        self.length = length
+    def __init__(self, length: int, value: int = 0):
+        if length <= 0:
+            raise ValueError("Cutout length must be positive.")
+        else:
+            self.length = length
+
+        self.value = value
 
     def __call__(self, img: torch.Tensor):
-        if self.length <= 0:
-            return img
+        if len(img.shape) == 2:
+            img = img.unsqueeze(0)
         h, w = img.size(1), img.size(2)
         mask = np.ones((h, w), np.float32)
         y = np.random.randint(h)
         x = np.random.randint(w)
 
         y1 = np.clip(y - self.length // 2, 0, h)
         y2 = np.clip(y + self.length // 2, 0, h)
         x1 = np.clip(x - self.length // 2, 0, w)
         x2 = np.clip(x + self.length // 2, 0, w)
 
-        mask[y1:y2, x1:x2] = 0.0
+        mask[y1:y2, x1:x2] = self.value
         mask = torch.from_numpy(mask)
         mask = mask.expand_as(img)
         img *= mask
         return img
```

### Comparing `torch_uncertainty-0.1.0/torch_uncertainty/utils.py` & `torch_uncertainty-0.1.1/torch_uncertainty/utils/checkpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # fmt: off
 from pathlib import Path
 from typing import Tuple, Union
 
 
 # fmt: on
 def get_version(
-    root: Union[str, Path], version: int, checkpoint: int = None
+    root: Union[str, Path], version: int, checkpoint: Union[int, None] = None
 ) -> Tuple[Path, Path]:
     """
     Find a compute the path to the checkpoint corresponding to the input
         parameters
 
-
     Args:
         root (Union[str, Path]): The root of the dataset containing the
             checkpoints.
         version (int): The version of the checkpoint
         checkpoint (int, optional): The number of the checkpoint. Defaults
             to None.
```

### Comparing `torch_uncertainty-0.1.0/setup.py` & `torch_uncertainty-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,33 +13,35 @@
  'torch_uncertainty.datasets',
  'torch_uncertainty.layers',
  'torch_uncertainty.metrics',
  'torch_uncertainty.models',
  'torch_uncertainty.models.resnet',
  'torch_uncertainty.models.wideresnet',
  'torch_uncertainty.routines',
- 'torch_uncertainty.transforms']
+ 'torch_uncertainty.transforms',
+ 'torch_uncertainty.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['einops>=0.6.0,<0.7.0',
+ 'huggingface-hub>=0.14.1,<0.15.0',
  'pytorch-lightning>=1.9.0,<2.0.0',
  'scipy>=1.10.0,<2.0.0',
  'tensorboard>=2.11.2,<3.0.0',
  'timm>=0.6.12,<0.7.0',
  'torchinfo>=1.7.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'torch-uncertainty',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.',
-    'long_description': '# Torch Uncertainty\n\n[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n\n_Torch Uncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.\n\n---\n\nThis package provides a multi-level API, including:\n- ready-to-train baselines on research datasets, such as CIFAR and ImageNet\n- baselines available for training on your datasets\n- layers available for use in your networks\n\n## Installation\n\nThe package can be installed from PyPI or from source.\n\n### From PyPI (available soon)\n\nInstall the package via pip: `pip install torch-uncertainty`\n\n### From source\n\n#### Installing Poetry\n\nInstallation guidelines for poetry are available on <https://python-poetry.org/docs/>. They boil down to executing the following command:\n\n`curl -sSL https://install.python-poetry.org | python3 -`\n\n#### Installing the package\n\nClone the repository:\n\n`git clone https://github.com/ENSTA-U2IS/torch-uncertainty.git`\n\nCreate a new conda environment and activate it with:\n\n`conda create -n uncertainty && conda activate uncertainty`\n\nInstall the package using poetry:\n\n`poetry install torch-uncertainty` or, for development, `poetry install torch-uncertainty --with dev`\n\nDepending on your system, you may encounter errors. If so, kill the process and add `PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring` at the beginning of every `poetry install` commands.\n\n#### Contributing\n\nIn case that you would like to contribute, install from source and add the pre-commit hooks with `pre-commit install`\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- Masksembles\n- Packed-Ensembles\n\n\n## Awesome Torch repositories\n\nYou may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## References\n\n',
+    'long_description': '<div align="center">\n\n![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)\n\n[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty) [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n</div>\n\n_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.\n\n---\n\nThis package provides a multi-level API, including:\n- ready-to-train baselines on research datasets, such as ImageNet and CIFAR\n- baselines available for training on your datasets\n- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR.\n- layers available for use in your networks\n\n## Installation\n\nThe package can be installed from PyPI:\n\n```sh\npip install torch-uncertainty\n```\n\nTo contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- Masksembles\n- Packed-Ensembles\n\n## Tutorials\n\n\n## Awesome Uncertainty repositories\n\nYou may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## Other References\n\nThis package also contains the official implementation of Packed-Ensembles.\n\nIf you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):\n\t\n    @inproceedings{laurent2023packed,\n        title={Packed-Ensembles for Efficient Uncertainty Estimation},\n        author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},\n        booktitle={ICLR},\n        year={2023}\n    }\n',
     'author': 'ENSTA U2IS',
     'author_email': 'olivier.laurent@ensta-paris.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

