# Comparing `tmp/scvi-tools-0.9.0b1.tar.gz` & `tmp/scvi-tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scvi-tools-0.9.0b1.tar", last modified: Wed Feb 24 05:11:14 2021, max compression
+gzip compressed data, was "scvi-tools-0.9.1.tar", last modified: Sat Mar 20 18:55:24 2021, max compression
```

## Comparing `scvi-tools-0.9.0b1.tar` & `scvi-tools-0.9.1.tar`

### file list

```diff
@@ -1,89 +1,94 @@
--rw-r--r--   0        0        0     1547 2021-01-20 23:18:59.370998 scvi-tools-0.9.0b1/LICENSE
--rw-r--r--   0        0        0     4096 2021-02-23 23:57:00.742574 scvi-tools-0.9.0b1/README.md
--rw-r--r--   0        0        0     3272 2021-02-24 05:10:20.144932 scvi-tools-0.9.0b1/pyproject.toml
--rw-r--r--   0        0        0      741 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/__init__.py
--rw-r--r--   0        0        0      439 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/_compat.py
--rw-r--r--   0        0        0      271 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/_constants.py
--rw-r--r--   0        0        0     2149 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/_docs.py
--rw-r--r--   0        0        0     5426 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/_settings.py
--rw-r--r--   0        0        0      302 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/_utils.py
--rw-r--r--   0        0        0      659 2021-02-22 04:33:13.557258 scvi-tools-0.9.0b1/scvi/compose/__init__.py
--rw-r--r--   0        0        0    33227 2021-02-04 17:26:16.093070 scvi-tools-0.9.0b1/scvi/compose/_base_components.py
--rw-r--r--   0        0        0     9786 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/compose/_base_module.py
--rw-r--r--   0        0        0     3725 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/compose/_decorators.py
--rw-r--r--   0        0        0      227 2021-02-21 18:26:57.235150 scvi-tools-0.9.0b1/scvi/compose/_pyro.py
--rw-r--r--   0        0        0      198 2021-02-22 04:31:34.533637 scvi-tools-0.9.0b1/scvi/compose/_utils.py
--rw-r--r--   0        0        0     1395 2021-02-23 22:45:19.178918 scvi-tools-0.9.0b1/scvi/data/__init__.py
--rw-r--r--   0        0        0    44059 2021-02-23 22:45:19.178918 scvi-tools-0.9.0b1/scvi/data/_anndata.py
--rw-r--r--   0        0        0        0 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/data/_built_in_data/__init__.py
--rw-r--r--   0        0        0     4505 2021-02-04 22:55:03.671635 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_brain_large.py
--rw-r--r--   0        0        0     4773 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_cite_seq.py
--rw-r--r--   0        0        0     2135 2021-02-04 22:55:03.747632 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_cortex.py
--rw-r--r--   0        0        0     1988 2021-02-04 22:55:03.763631 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_csv.py
--rw-r--r--   0        0        0     5775 2021-02-04 22:55:04.115615 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_dataset_10x.py
--rw-r--r--   0        0        0     1426 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_download.py
--rw-r--r--   0        0        0     5749 2021-02-04 22:55:04.115615 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_loom.py
--rw-r--r--   0        0        0     4405 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_pbmc.py
--rw-r--r--   0        0        0     3538 2021-02-04 22:55:03.735632 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_seqfish.py
--rw-r--r--   0        0        0     3427 2021-02-04 22:55:03.747632 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_smfish.py
--rw-r--r--   0        0        0     1438 2021-02-23 22:45:19.178918 scvi-tools-0.9.0b1/scvi/data/_built_in_data/_synthetic.py
--rw-r--r--   0        0        0    19491 2021-02-16 00:32:19.280019 scvi-tools-0.9.0b1/scvi/data/_datasets.py
--rw-r--r--   0        0        0    10206 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/data/_preprocessing.py
--rw-r--r--   0        0        0     1258 2021-01-28 20:54:18.604884 scvi-tools-0.9.0b1/scvi/data/_read.py
--rw-r--r--   0        0        0     4078 2021-02-23 22:45:19.178918 scvi-tools-0.9.0b1/scvi/data/_utils.py
--rw-r--r--   0        0        0      432 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/dataloaders/__init__.py
--rw-r--r--   0        0        0     4954 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/dataloaders/_ann_dataloader.py
--rw-r--r--   0        0        0     3970 2021-02-23 22:45:19.178918 scvi-tools-0.9.0b1/scvi/dataloaders/_anntorchdataset.py
--rw-r--r--   0        0        0     2416 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/dataloaders/_concat_dataloader.py
--rw-r--r--   0        0        0    10567 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/dataloaders/_data_splitting.py
--rw-r--r--   0        0        0     3694 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/dataloaders/_semi_dataloader.py
--rw-r--r--   0        0        0      227 2021-02-15 23:47:10.057336 scvi-tools-0.9.0b1/scvi/distributions/__init__.py
--rw-r--r--   0        0        0    16964 2021-02-15 23:47:10.057336 scvi-tools-0.9.0b1/scvi/distributions/_negative_binomial.py
--rw-r--r--   0        0        0      177 2021-02-21 06:14:45.185834 scvi-tools-0.9.0b1/scvi/external/__init__.py
--rw-r--r--   0        0        0       47 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/external/gimvi/__init__.py
--rw-r--r--   0        0        0    19466 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/external/gimvi/_model.py
--rw-r--r--   0        0        0    15980 2021-01-23 02:47:42.247935 scvi-tools-0.9.0b1/scvi/external/gimvi/_module.py
--rw-r--r--   0        0        0     4977 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/external/gimvi/_task.py
--rw-r--r--   0        0        0       45 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/external/solo/__init__.py
--rw-r--r--   0        0        0     9250 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/external/solo/_model.py
--rw-r--r--   0        0        0      107 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/external/stereoscope/__init__.py
--rw-r--r--   0        0        0     9063 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/external/stereoscope/_model.py
--rw-r--r--   0        0        0     7938 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/external/stereoscope/_module.py
--rw-r--r--   0        0        0      360 2021-02-22 04:33:13.557258 scvi-tools-0.9.0b1/scvi/lightning/__init__.py
--rw-r--r--   0        0        0     3330 2021-02-22 04:33:13.557258 scvi-tools-0.9.0b1/scvi/lightning/_callbacks.py
--rw-r--r--   0        0        0     1584 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/lightning/_logger.py
--rw-r--r--   0        0        0     3226 2021-02-22 04:33:13.561258 scvi-tools-0.9.0b1/scvi/lightning/_progress.py
--rw-r--r--   0        0        0     5072 2021-02-22 04:33:13.561258 scvi-tools-0.9.0b1/scvi/lightning/_trainer.py
--rw-r--r--   0        0        0    24720 2021-02-23 16:22:33.196244 scvi-tools-0.9.0b1/scvi/lightning/_trainingplans.py
--rw-r--r--   0        0        0      277 2021-01-28 20:54:18.604884 scvi-tools-0.9.0b1/scvi/model/__init__.py
--rw-r--r--   0        0        0     9790 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/_autozi.py
--rw-r--r--   0        0        0     3924 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/_linear_scvi.py
--rw-r--r--   0        0        0     4320 2021-02-04 22:55:03.735632 scvi-tools-0.9.0b1/scvi/model/_metrics.py
--rw-r--r--   0        0        0    16996 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/model/_peakvi.py
--rw-r--r--   0        0        0    12971 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/_scanvi.py
--rw-r--r--   0        0        0     3937 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/_scvi.py
--rw-r--r--   0        0        0    43282 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/model/_totalvi.py
--rw-r--r--   0        0        0     6989 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/_utils.py
--rw-r--r--   0        0        0      381 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/base/__init__.py
--rw-r--r--   0        0        0     7505 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/base/_archesmixin.py
--rw-r--r--   0        0        0    12742 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/base/_base_model.py
--rw-r--r--   0        0        0     1894 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/model/base/_log_likelihood.py
--rw-r--r--   0        0        0    19919 2021-02-21 06:14:45.185834 scvi-tools-0.9.0b1/scvi/model/base/_rnamixin.py
--rw-r--r--   0        0        0     2389 2021-02-24 05:03:06.764172 scvi-tools-0.9.0b1/scvi/model/base/_training_mixin.py
--rw-r--r--   0        0        0     2778 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/base/_trainrunner.py
--rw-r--r--   0        0        0     6191 2021-02-23 23:40:25.378776 scvi-tools-0.9.0b1/scvi/model/base/_utils.py
--rw-r--r--   0        0        0     6495 2021-02-21 06:14:45.185834 scvi-tools-0.9.0b1/scvi/model/base/_vaemixin.py
--rw-r--r--   0        0        0      280 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/modules/__init__.py
--rw-r--r--   0        0        0    15630 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/modules/_autozivae.py
--rw-r--r--   0        0        0     1651 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/modules/_classifier.py
--rw-r--r--   0        0        0    11790 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/modules/_peakvae.py
--rw-r--r--   0        0        0    10613 2021-01-23 02:47:42.251935 scvi-tools-0.9.0b1/scvi/modules/_scanvae.py
--rw-r--r--   0        0        0    26808 2021-01-23 02:47:42.251935 scvi-tools-0.9.0b1/scvi/modules/_totalvae.py
--rw-r--r--   0        0        0     1275 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/modules/_utils.py
--rw-r--r--   0        0        0    21353 2021-02-15 23:47:10.057336 scvi-tools-0.9.0b1/scvi/modules/_vae.py
--rw-r--r--   0        0        0     5223 2021-01-20 23:18:59.378998 scvi-tools-0.9.0b1/scvi/modules/_vaec.py
--rw-r--r--   0        0        0      125 2021-02-22 04:30:49.731617 scvi-tools-0.9.0b1/scvi/utils/__init__.py
--rw-r--r--   0        0        0    22011 2021-02-04 22:55:04.155613 scvi-tools-0.9.0b1/scvi/utils/_differential.py
--rw-r--r--   0        0        0     1744 2021-02-21 01:46:37.994429 scvi-tools-0.9.0b1/scvi/utils/_track.py
--rw-r--r--   0        0        0     6301 2021-02-24 05:11:14.751399 scvi-tools-0.9.0b1/setup.py
--rw-r--r--   0        0        0     6988 2021-02-24 05:11:14.751766 scvi-tools-0.9.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1547 2021-01-20 23:18:59.370998 scvi-tools-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4612 2021-03-03 20:28:45.785192 scvi-tools-0.9.1/README.md
+-rw-r--r--   0        0        0     3373 2021-03-20 18:46:54.374129 scvi-tools-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      763 2021-03-06 17:06:46.262941 scvi-tools-0.9.1/scvi/__init__.py
+-rw-r--r--   0        0        0      439 2021-01-20 23:18:59.378998 scvi-tools-0.9.1/scvi/_compat.py
+-rw-r--r--   0        0        0      271 2021-01-20 23:18:59.378998 scvi-tools-0.9.1/scvi/_constants.py
+-rw-r--r--   0        0        0     2212 2021-03-03 18:42:32.748579 scvi-tools-0.9.1/scvi/_docs.py
+-rw-r--r--   0        0        0     5861 2021-03-16 18:04:26.750512 scvi-tools-0.9.1/scvi/_settings.py
+-rw-r--r--   0        0        0      302 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/_utils.py
+-rw-r--r--   0        0        0     1463 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/data/__init__.py
+-rw-r--r--   0        0        0    44059 2021-03-03 21:42:15.295079 scvi-tools-0.9.1/scvi/data/_anndata.py
+-rw-r--r--   0        0        0        0 2021-01-20 23:18:59.378998 scvi-tools-0.9.1/scvi/data/_built_in_data/__init__.py
+-rw-r--r--   0        0        0     4505 2021-02-04 22:55:03.671635 scvi-tools-0.9.1/scvi/data/_built_in_data/_brain_large.py
+-rw-r--r--   0        0        0     4773 2021-03-02 16:45:08.820252 scvi-tools-0.9.1/scvi/data/_built_in_data/_cite_seq.py
+-rw-r--r--   0        0        0     2135 2021-02-04 22:55:03.747632 scvi-tools-0.9.1/scvi/data/_built_in_data/_cortex.py
+-rw-r--r--   0        0        0     1988 2021-02-04 22:55:03.763631 scvi-tools-0.9.1/scvi/data/_built_in_data/_csv.py
+-rw-r--r--   0        0        0     5775 2021-02-04 22:55:04.115615 scvi-tools-0.9.1/scvi/data/_built_in_data/_dataset_10x.py
+-rw-r--r--   0        0        0     1426 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/data/_built_in_data/_download.py
+-rw-r--r--   0        0        0     1702 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/data/_built_in_data/_heartcellatlas.py
+-rw-r--r--   0        0        0     5749 2021-02-04 22:55:04.115615 scvi-tools-0.9.1/scvi/data/_built_in_data/_loom.py
+-rw-r--r--   0        0        0     4405 2021-01-20 23:18:59.378998 scvi-tools-0.9.1/scvi/data/_built_in_data/_pbmc.py
+-rw-r--r--   0        0        0     3538 2021-02-04 22:55:03.735632 scvi-tools-0.9.1/scvi/data/_built_in_data/_seqfish.py
+-rw-r--r--   0        0        0     3427 2021-02-04 22:55:03.747632 scvi-tools-0.9.1/scvi/data/_built_in_data/_smfish.py
+-rw-r--r--   0        0        0     1438 2021-02-25 16:29:29.288706 scvi-tools-0.9.1/scvi/data/_built_in_data/_synthetic.py
+-rw-r--r--   0        0        0    20922 2021-03-02 16:45:08.820252 scvi-tools-0.9.1/scvi/data/_datasets.py
+-rw-r--r--   0        0        0    10206 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/data/_preprocessing.py
+-rw-r--r--   0        0        0     1258 2021-01-28 20:54:18.604884 scvi-tools-0.9.1/scvi/data/_read.py
+-rw-r--r--   0        0        0     4078 2021-03-03 02:56:25.450296 scvi-tools-0.9.1/scvi/data/_utils.py
+-rw-r--r--   0        0        0      432 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/dataloaders/__init__.py
+-rw-r--r--   0        0        0     4954 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/dataloaders/_ann_dataloader.py
+-rw-r--r--   0        0        0     3970 2021-02-25 16:29:29.288706 scvi-tools-0.9.1/scvi/dataloaders/_anntorchdataset.py
+-rw-r--r--   0        0        0     2416 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/dataloaders/_concat_dataloader.py
+-rw-r--r--   0        0        0    10567 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/dataloaders/_data_splitting.py
+-rw-r--r--   0        0        0     3694 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/dataloaders/_semi_dataloader.py
+-rw-r--r--   0        0        0      227 2021-02-15 23:47:10.057336 scvi-tools-0.9.1/scvi/distributions/__init__.py
+-rw-r--r--   0        0        0    16964 2021-02-15 23:47:10.057336 scvi-tools-0.9.1/scvi/distributions/_negative_binomial.py
+-rw-r--r--   0        0        0      226 2021-03-08 03:05:36.724282 scvi-tools-0.9.1/scvi/external/__init__.py
+-rw-r--r--   0        0        0      115 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/external/cellassign/__init__.py
+-rw-r--r--   0        0        0     8082 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/external/cellassign/_model.py
+-rw-r--r--   0        0        0     8725 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/external/cellassign/_module.py
+-rw-r--r--   0        0        0       81 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/external/gimvi/__init__.py
+-rw-r--r--   0        0        0    19465 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/external/gimvi/_model.py
+-rw-r--r--   0        0        0    15970 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/external/gimvi/_module.py
+-rw-r--r--   0        0        0     4972 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/external/gimvi/_task.py
+-rw-r--r--   0        0        0       45 2021-02-21 01:46:37.994429 scvi-tools-0.9.1/scvi/external/solo/__init__.py
+-rw-r--r--   0        0        0     9250 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/external/solo/_model.py
+-rw-r--r--   0        0        0      183 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/external/stereoscope/__init__.py
+-rw-r--r--   0        0        0     9118 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/external/stereoscope/_model.py
+-rw-r--r--   0        0        0     7942 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/external/stereoscope/_module.py
+-rw-r--r--   0        0        0      277 2021-01-28 20:54:18.604884 scvi-tools-0.9.1/scvi/model/__init__.py
+-rw-r--r--   0        0        0     9783 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/model/_autozi.py
+-rw-r--r--   0        0        0     3922 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/model/_linear_scvi.py
+-rw-r--r--   0        0        0     4320 2021-02-04 22:55:03.735632 scvi-tools-0.9.1/scvi/model/_metrics.py
+-rw-r--r--   0        0        0    17156 2021-03-03 19:42:59.696669 scvi-tools-0.9.1/scvi/model/_peakvi.py
+-rw-r--r--   0        0        0    13482 2021-03-02 16:45:08.820252 scvi-tools-0.9.1/scvi/model/_scanvi.py
+-rw-r--r--   0        0        0     3935 2021-03-20 17:43:27.364121 scvi-tools-0.9.1/scvi/model/_scvi.py
+-rw-r--r--   0        0        0    43291 2021-03-03 18:42:32.748579 scvi-tools-0.9.1/scvi/model/_totalvi.py
+-rw-r--r--   0        0        0     6989 2021-03-01 22:16:53.854085 scvi-tools-0.9.1/scvi/model/_utils.py
+-rw-r--r--   0        0        0      324 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/model/base/__init__.py
+-rw-r--r--   0        0        0     7546 2021-03-03 06:17:06.248449 scvi-tools-0.9.1/scvi/model/base/_archesmixin.py
+-rw-r--r--   0        0        0    12795 2021-03-03 06:17:06.248449 scvi-tools-0.9.1/scvi/model/base/_base_model.py
+-rw-r--r--   0        0        0     1894 2021-01-20 23:18:59.378998 scvi-tools-0.9.1/scvi/model/base/_log_likelihood.py
+-rw-r--r--   0        0        0    20122 2021-03-03 18:42:32.748579 scvi-tools-0.9.1/scvi/model/base/_rnamixin.py
+-rw-r--r--   0        0        0     2776 2021-03-03 06:17:06.248449 scvi-tools-0.9.1/scvi/model/base/_training_mixin.py
+-rw-r--r--   0        0        0     6262 2021-03-03 23:57:15.577159 scvi-tools-0.9.1/scvi/model/base/_utils.py
+-rw-r--r--   0        0        0     6529 2021-03-03 06:17:06.248449 scvi-tools-0.9.1/scvi/model/base/_vaemixin.py
+-rw-r--r--   0        0        0      280 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/__init__.py
+-rw-r--r--   0        0        0    15653 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/_autozivae.py
+-rw-r--r--   0        0        0     1646 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/_classifier.py
+-rw-r--r--   0        0        0    11788 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/_peakvae.py
+-rw-r--r--   0        0        0    11373 2021-03-03 02:56:54.241626 scvi-tools-0.9.1/scvi/module/_scanvae.py
+-rw-r--r--   0        0        0    26802 2021-03-02 16:45:08.820252 scvi-tools-0.9.1/scvi/module/_totalvae.py
+-rw-r--r--   0        0        0     1270 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/_utils.py
+-rw-r--r--   0        0        0    21343 2021-03-20 17:43:27.364121 scvi-tools-0.9.1/scvi/module/_vae.py
+-rw-r--r--   0        0        0     5216 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/_vaec.py
+-rw-r--r--   0        0        0      205 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/base/__init__.py
+-rw-r--r--   0        0        0    10950 2021-03-16 18:04:26.750512 scvi-tools-0.9.1/scvi/module/base/_base_module.py
+-rw-r--r--   0        0        0     3725 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/base/_decorators.py
+-rw-r--r--   0        0        0      227 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/module/base/_pyro.py
+-rw-r--r--   0        0        0      422 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/nn/__init__.py
+-rw-r--r--   0        0        0    33146 2021-03-04 00:21:54.151886 scvi-tools-0.9.1/scvi/nn/_base_components.py
+-rw-r--r--   0        0        0      275 2021-03-03 06:17:06.248449 scvi-tools-0.9.1/scvi/nn/_utils.py
+-rw-r--r--   0        0        0      417 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/train/__init__.py
+-rw-r--r--   0        0        0     3322 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/train/_callbacks.py
+-rw-r--r--   0        0        0     1584 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/train/_logger.py
+-rw-r--r--   0        0        0     3226 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/train/_progress.py
+-rw-r--r--   0        0        0     6332 2021-03-02 16:45:08.820252 scvi-tools-0.9.1/scvi/train/_trainer.py
+-rw-r--r--   0        0        0    27024 2021-03-16 18:04:26.750512 scvi-tools-0.9.1/scvi/train/_trainingplans.py
+-rw-r--r--   0        0        0     2770 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/train/_trainrunner.py
+-rw-r--r--   0        0        0      125 2021-02-22 04:30:49.731617 scvi-tools-0.9.1/scvi/utils/__init__.py
+-rw-r--r--   0        0        0    22011 2021-03-03 18:42:32.748579 scvi-tools-0.9.1/scvi/utils/_differential.py
+-rw-r--r--   0        0        0     1743 2021-03-01 23:15:51.996897 scvi-tools-0.9.1/scvi/utils/_track.py
+-rw-r--r--   0        0        0     6882 2021-03-20 18:55:25.156503 scvi-tools-0.9.1/setup.py
+-rw-r--r--   0        0        0     7482 2021-03-20 18:55:25.156904 scvi-tools-0.9.1/PKG-INFO
```

### Comparing `scvi-tools-0.9.0b1/LICENSE` & `scvi-tools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/README.md` & `scvi-tools-0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Downloads](https://pepy.tech/badge/scvi-tools)](https://pepy.tech/project/scvi-tools)
 [![Join the chat at https://gitter.im/scvi-tools/development](https://badges.gitter.im/scvi-tools/development.svg)](https://gitter.im/scvi-tools/development?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [scvi-tools](https://scvi-tools.org/) (single-cell variational inference
 tools) is a package for probabilistic modeling of single-cell omics
 data, built on top of [PyTorch](https://pytorch.org) and
-[Anndata](https://anndata.readthedocs.io/en/latest/).
+[AnnData](https://anndata.readthedocs.io/en/latest/).
 
 # Available implementations of single-cell omics models
 
 scvi-tools contains scalable implementations of several models that
 facilitate a broad number of tasks across many omics, including:
 
 -   [scVI](https://rdcu.be/bdHYQ) for analysis of single-cell RNA-seq
@@ -37,35 +37,51 @@
     for an interpretable linear factor model version of scVI.
 -   [Stereoscope](https://www.nature.com/articles/s42003-020-01247-y)
     for deconvolution of spatial transcriptomics data.
 -   peakVI for analysis of ATAC-seq data.
 -   [scArches](https://www.biorxiv.org/content/10.1101/2020.07.16.205997v1)
     for transfer learning from one single-cell atlas to a query dataset
     (currently supports scVI, scANVI and TotalVI).
+-   [CellAssign](https://www.nature.com/articles/s41592-019-0529-1) for
+    reference-based annotation of scRNA-seq data.
+-   [Solo](https://www.sciencedirect.com/science/article/pii/S2405471220301952) 
+    for doublet detection in scRNA-seq data.
 
 All these implementations have a high-level API that interacts with
 [scanpy](http://scanpy.readthedocs.io/), standard save/load functions,
 and support GPU acceleration.
 
 # Fast prototyping of novel probabilistic models
 
 scvi-tools contains the building blocks to prototype novel probablistic
 models. These building blocks are powered by popular probabilistic and
 machine learning frameworks such as [PyTorch
-lightning](https://www.pytorchlightning.ai/), and
+Lightning](https://www.pytorchlightning.ai/), and
 [Pyro](https://pyro.ai/).
 
 We recommend checking out the [skeleton
 repository](https://github.com/YosefLab/scvi-tools-skeleton), as a
 starting point for developing new models into scvi-tools.
 
+# Basic installation
+
+For conda, 
+```
+conda install scvi-tools -c bioconda -c conda-forge
+```
+and for pip,
+```
+pip install scvi-tools
+```
+Please be sure to install a version of [PyTorch](https://pytorch.org/) that is compatible with your GPU (if applicable).
+
 # Resources
 
 -   Tutorials, API reference, and installation guides are available in
     the [documentation](https://docs.scvi-tools.org/).
 -   For discussion of usage, checkout out our
     [forum](https://discourse.scvi-tools.org).
 -   Please use the issues here to submit bug reports.
--   If you\'d like to contribute, check out our [development
-    guide](https://docs.scvi-tools.org/en/stable/development.html).
+-   If you\'d like to contribute, check out our [contributing
+    guide](https://docs.scvi-tools.org/en/stable/contributing/index.html).
 -   If you find a model useful for your research, please consider citing
     the corresponding publication (linked above).
```

### Comparing `scvi-tools-0.9.0b1/pyproject.toml` & `scvi-tools-0.9.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 
 [tool.poetry]
 authors = ["Romain Lopez <romain_lopez@gmail.com>", "Adam Gayoso <adamgayoso@berkeley.edu>", "Galen Xing <gx2113@columbia.edu>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Science/Research",
   "Natural Language :: English",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
-description = "Deep generative models for end-to-end analysis of single-cell omics data."
+description = "Deep probabilistic analysis of single-cell omics data."
 documentation = "https://scvi-tools.org"
 homepage = "https://github.com/YosefLab/scvi-tools"
 license = "BSD-3-Clause"
 name = "scvi-tools"
 packages = [
   {include = "scvi"},
 ]
 readme = "README.md"
-version = "0.9.0-beta.1"
+version = "0.9.1"
 
 [tool.poetry.dependencies]
 anndata = ">=0.7.5"
 black = {version = ">=20.8b1", optional = true}
 codecov = {version = ">=2.0.8", optional = true}
 flake8 = {version = ">=3.7.7", optional = true}
-furo = {version = ">=2020.12.30b24", optional = true}
 h5py = ">=2.9.0"
 importlib-metadata = {version = "^1.0", python = "<3.8"}
 ipython = {version = ">=7.20", optional = true, python = ">=3.7"}
 ipywidgets = "*"
 isort = {version = ">=5.7", optional = true}
 jupyter = {version = ">=1.0", optional = true}
 leidenalg = {version = "*", optional = true}
@@ -47,45 +47,48 @@
 nbsphinx = {version = "*", optional = true}
 nbsphinx-link = {version = "*", optional = true}
 numba = ">=0.41.0"
 numpy = ">=1.17.0"
 openpyxl = ">=3.0"
 pandas = ">=1.0"
 pre-commit = {version = ">=2.7.1", optional = true}
-pyro-ppl = ">=1.1.0"
+pydata-sphinx-theme = {version = ">=0.4.3", optional = true}
+pyro-ppl = ">=1.5.0"
 pytest = {version = ">=4.4", optional = true}
-python = ">=3.6.2,<4.0"
+python = ">=3.7,<4.0"
 python-igraph = {version = "*", optional = true}
 pytorch-lightning = ">=1.2"
 rich = ">=9.1.0"
 scanpy = {version = ">=1.6", optional = true}
 scanpydoc = {version = ">=0.5", optional = true}
 scikit-learn = ">=0.21.2"
 scikit-misc = {version = ">=0.1.3", optional = true}
 sphinx = {version = ">=3.4", optional = true}
 sphinx-autodoc-typehints = {version = "*", optional = true}
 sphinx-gallery = {version = ">0.6", optional = true}
+sphinx-tabs = {version = "*", optional = true}
 sphinx_copybutton = {version = "*", optional = true}
 torch = ">=1.7.1"
 tqdm = ">=4.56.0"
 typing_extensions = {version = "*", python = "<3.8"}
 
 [tool.poetry.extras]
 dev = ["black", "pytest", "flake8", "codecov", "scanpy", "loompy", "jupyter", "nbformat", "nbconvert", "pre-commit", "isort"]
 docs = [
   "sphinx",
   "scanpydoc",
   "nbsphinx",
   "nbsphinx-link",
   "ipython",
-  "furo",
+  "pydata-sphinx-theme",
   "typing_extensions",
   "sphinx-autodoc-typehints",
   "sphinx_copybutton",
   "sphinx_gallery",
+  "sphinx-tabs",
 ]
 tutorials = ["scanpy", "leidenalg", "python-igraph", "loompy", "scikit-misc"]
 
 [tool.poetry.dev-dependencies]
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `scvi-tools-0.9.0b1/scvi/__init__.py` & `scvi-tools-0.9.1/scvi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # Set default logging handler to avoid logging with logging.lastResort logger.
 import logging
 
 from ._constants import _CONSTANTS
 from ._settings import settings
 
 # this import needs to come after prior imports to prevent circular import
-from . import data, model
+from . import data, model, external
 
 # https://github.com/python-poetry/poetry/pull/2366#issuecomment-652418094
 # https://github.com/python-poetry/poetry/issues/144#issuecomment-623927302
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 package_name = "scvi-tools"
 __version__ = importlib_metadata.version(package_name)
 
 settings.verbosity = logging.INFO
 test_var = "test"
 
-__all__ = ["settings", "_CONSTANTS", "data", "model"]
+__all__ = ["settings", "_CONSTANTS", "data", "model", "external"]
```

### Comparing `scvi-tools-0.9.0b1/scvi/_docs.py` & `scvi-tools-0.9.1/scvi/_docs.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,8 +38,10 @@
 batchid2
     Same as `batchid1` for group2. `batchid2` must either have null intersection with `batchid1`,
     or be exactly equal to `batchid1`. When the two sets are exactly equal, cells are compared by
     decoding on the same batch. When sets have null intersection, cells from `group1` and `group2`
     are decoded on each group in `group1` and `group2`, respectively.
 fdr_target
     Tag features as DE based on posterior expected false discovery rate.
+silent
+    If True, disables the progress bar. Default: False.
 """
```

### Comparing `scvi-tools-0.9.0b1/scvi/_settings.py` & `scvi-tools-0.9.1/scvi/_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
     >>> scvi.settings.progress_bar_style = "rich"
 
     To set the verbosity
 
     >>> import logging
     >>> scvi.settings.verbosity = logging.INFO
+
+    To set the number of threads PyTorch will use
+
+    >>> scvi.settings.num_threads = 2
     """
 
     def __init__(
         self,
         verbosity: int = logging.INFO,
         progress_bar_style: Literal["rich", "tqdm"] = "tqdm",
         batch_size: int = 128,
@@ -52,14 +56,15 @@
         self.batch_size = batch_size
         if progress_bar_style not in ["rich", "tqdm"]:
             raise ValueError("Progress bar style must be in ['rich', 'tqdm']")
         self.progress_bar_style = progress_bar_style
         self.logging_dir = logging_dir
         self.dl_num_workers = dl_num_workers
         self.dl_pin_memory_gpu_training = dl_pin_memory_gpu_training
+        self._num_threads = None
 
     @property
     def batch_size(self) -> int:
         """
         Minibatch size for loading data into the model.
 
         This is only used after a model is trained. Trainers have specific
@@ -103,14 +108,25 @@
         return self._logging_dir
 
     @logging_dir.setter
     def logging_dir(self, logging_dir: Union[str, Path]):
         self._logging_dir = Path(logging_dir).resolve()
 
     @property
+    def num_threads(self) -> None:
+        """Number of threads PyTorch will use."""
+        return self._num_threads
+
+    @num_threads.setter
+    def num_threads(self, num: int):
+        """Number of threads PyTorch will use."""
+        self._num_threads = num
+        torch.set_num_threads(num)
+
+    @property
     def progress_bar_style(self) -> str:
         """Library to use for progress bar."""
         return self._pbar_style
 
     @progress_bar_style.setter
     def progress_bar_style(self, pbar_style: Literal["tqdm", "rich"]):
         """Library to use for progress bar."""
```

### Comparing `scvi-tools-0.9.0b1/scvi/compose/_base_components.py` & `scvi-tools-0.9.1/scvi/nn/_base_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             self.n_cat_list = []
 
         cat_dim = sum(self.n_cat_list)
         self.fc_layers = nn.Sequential(
             collections.OrderedDict(
                 [
                     (
-                        "Layer_{}".format(i),
+                        "Layer {}".format(i),
                         nn.Sequential(
                             nn.Linear(
                                 n_in + cat_dim * self.inject_into_layer(i),
                                 n_out,
                                 bias=bias,
                             ),
                             # non-default params come from defaults in original Tensorflow implementation
@@ -121,16 +121,14 @@
                 new_grad[:, -categorical_dims:] = grad[:, -categorical_dims:]
             return new_grad
 
         def _hook_fn_zero_out(grad):
             return grad * 0
 
         for i, layers in enumerate(self.fc_layers):
-            # if i > 0 and not self.inject_covariates:
-            #     break
             for layer in layers:
                 if i == 0 and not hook_first_layer:
                     continue
                 if isinstance(layer, nn.Linear):
                     if self.inject_into_layer(i):
                         w = layer.weight.register_hook(_hook_fn_weight)
                     else:
@@ -220,15 +218,15 @@
     n_hidden
         The number of nodes per hidden layer
     dropout_rate
         Dropout rate to apply to each of the hidden layers
     distribution
         Distribution of z
     **kwargs
-        Keyword args for :class:`~scvi.modules._base.FCLayers`
+        Keyword args for :class:`~scvi.module._base.FCLayers`
     """
 
     def __init__(
         self,
         n_input: int,
         n_output: int,
         n_cat_list: Iterable[int] = None,
@@ -471,15 +469,15 @@
     n_layers
         The number of fully-connected hidden layers
     n_hidden
         The number of nodes per hidden layer
     dropout_rate
         Dropout rate to apply to each of the hidden layers
     kwargs
-        Keyword args for :class:`~scvi.modules._base.FCLayers`
+        Keyword args for :class:`~scvi.module._base.FCLayers`
     """
 
     def __init__(
         self,
         n_input: int,
         n_output: int,
         n_cat_list: Iterable[int] = None,
```

### Comparing `scvi-tools-0.9.0b1/scvi/compose/_base_module.py` & `scvi-tools-0.9.1/scvi/module/base/_base_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class LossRecorder:
     """
     Loss signature for models.
 
     This class provides an organized way to record the model loss, as well as
     the components of the ELBO. This may also be used in MLE, MAP, EM methods.
-    The loss is used for backpropagation during infernce. The other parameters
+    The loss is used for backpropagation during inference. The other parameters
     are used for logging/early stopping during inference.
 
     Parameters
     ----------
     loss
         Tensor with loss for minibatch. Should be one dimensional with one value.
         Note that loss should be a :class:`~torch.Tensor` and not the result of `.item()`.
@@ -29,31 +29,34 @@
         KL divergence associated with each observation in the minibatch.
     kl_global
         Global kl divergence term. Should be one dimensional with one value.
     """
 
     def __init__(
         self,
-        loss: torch.Tensor,
-        reconstruction_loss: torch.Tensor,
-        kl_local: torch.Tensor,
-        kl_global: torch.Tensor = torch.Tensor([0]),
+        loss: Union[Dict[str, torch.Tensor], torch.Tensor],
+        reconstruction_loss: Union[Dict[str, torch.Tensor], torch.Tensor],
+        kl_local: Union[Dict[str, torch.Tensor], torch.Tensor],
+        kl_global: Union[Dict[str, torch.Tensor], torch.Tensor] = torch.Tensor([0]),
+        **kwargs,
     ):
         self._loss = loss if isinstance(loss, dict) else dict(loss=loss)
         self._reconstruction_loss = (
             reconstruction_loss
             if isinstance(reconstruction_loss, dict)
             else dict(reconstruction_loss=reconstruction_loss)
         )
         self._kl_local = (
             kl_local if isinstance(kl_local, dict) else dict(kl_local=kl_local)
         )
         self._kl_global = (
             kl_global if isinstance(kl_global, dict) else dict(kl_global=kl_global)
         )
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
     @staticmethod
     def _get_dict_sum(dictionary):
         total = 0.0
         for value in dictionary.values():
             total += value
         return total
@@ -70,20 +73,18 @@
     def kl_local(self) -> torch.Tensor:
         return self._get_dict_sum(self._kl_local)
 
     @property
     def kl_global(self) -> torch.Tensor:
         return self._get_dict_sum(self._kl_global)
 
-    @property
-    def elbo(self):
-        return
-
 
 class BaseModuleClass(nn.Module):
+    """Abstract class for scvi-tools modules."""
+
     def __init__(
         self,
     ):
         super().__init__()
 
     @auto_move_data
     def forward(
@@ -149,46 +150,52 @@
     @abstractmethod
     def _get_generative_input(
         self,
         tensors: Dict[str, torch.Tensor],
         inference_outputs: Dict[str, torch.Tensor],
         **kwargs,
     ):
-        """Parse tensors dictionary for inference related values."""
+        """Parse tensors dictionary for generative related values."""
 
     @abstractmethod
     def inference(
         self,
         *args,
         **kwargs,
     ) -> dict:
         """
         Run the inference (recognition) model.
 
         In the case of variational inference, this function will perform steps related to
         computing variational distribution parameters. In a VAE, this will involve running
         data through encoder networks.
+
+        This function should return a dictionary with str keys and :class:`~torch.Tensor` values.
         """
 
     @abstractmethod
     def generative(self, *args, **kwargs) -> dict:
         """
         Run the generative model.
 
         This function should return the parameters associated with the likelihood of the data.
         This is typically written as :math:`p(x|z)`.
+
+        This function should return a dictionary with str keys and :class:`~torch.Tensor` values.
         """
 
     @abstractmethod
     def loss(self, *args, **kwargs) -> LossRecorder:
         """
         Compute the loss for a minibatch of data.
 
         This function uses the outputs of the inference and generative functions to compute
         a loss. This many optionally include other penalty terms, which should be computed here.
+
+        This function should return an object of type :class:`~scvi.module.base.LossRecorder`.
         """
 
     @abstractmethod
     def sample(self, *args, **kwargs):
         """Generate samples from the learned model."""
 
 
@@ -203,16 +210,23 @@
     Base module class for Pyro models.
 
     In Pyro, `model` and `guide` should have the same signature. Out of convenience,
     the forward function of this class passes through to the forward of the `model`.
 
     There are two ways this class can be equipped with a model and a guide. First,
     `model` and `guide` can be class attributes that are :class:`~pyro.nn.PyroModule`
-    instances. Second, `model` and `guide` methods can be written (see Pyro scANVI example)
-    https://pyro.ai/examples/scanvi.html
+    instances. The implemented `model` and `guide` class method can then return the (private) attributes.
+    Second, `model` and `guide` methods can be written directly (see Pyro scANVI example)
+    https://pyro.ai/examples/scanvi.html.
+
+    The `model` and `guide` may also be equipped with `n_obs` attributes, which can be set
+    to `None` (e.g., `self.n_obs = None`). This attribute may be helpful in designating the
+    size of observation-specific Pyro plates. The value will be updated automatically by
+    :class:`~scvi.train.PyroTrainingPlan`, provided that it is given the number of training examples
+    upon initialization.
     """
 
     def __init__(self):
         super().__init__()
 
     @staticmethod
     @abstractmethod
@@ -228,14 +242,24 @@
         :class:`~scvi.dataloaders.AnnDataLoader`.
 
         Returns
         -------
         args and kwargs for the functions, args should be an Iterable and kwargs a dictionary.
         """
 
+    @property
+    @abstractmethod
+    def model(self):
+        pass
+
+    @property
+    @abstractmethod
+    def guide(self):
+        pass
+
     def create_predictive(
         self,
         model: Optional[Callable] = None,
         posterior_samples: Optional[dict] = None,
         guide: Optional[Callable] = None,
         num_samples: Optional[int] = None,
         return_sites: Tuple[str] = (),
```

### Comparing `scvi-tools-0.9.0b1/scvi/compose/_decorators.py` & `scvi-tools-0.9.1/scvi/module/base/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/__init__.py` & `scvi-tools-0.9.1/scvi/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ._datasets import (
     annotation_simulation,
     brainlarge_dataset,
     breast_cancer_dataset,
     cortex,
     dataset_10x,
     frontalcortex_dropseq,
+    heart_cell_atlas_subsampled,
     mouse_ob_dataset,
     pbmc_dataset,
     pbmcs_10x_cite_seq,
     prefrontalcortex_starmap,
     purified_pbmc_dataset,
     retina,
     seqfish,
@@ -55,8 +56,9 @@
     "transfer_anndata_setup",
     "register_tensor_from_anndata",
     "read_h5ad",
     "read_csv",
     "read_loom",
     "read_text",
     "read_10x_atac",
+    "heart_cell_atlas_subsampled",
 ]
```

### Comparing `scvi-tools-0.9.0b1/scvi/data/_anndata.py` & `scvi-tools-0.9.1/scvi/data/_anndata.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     protein_expression_obsm_key: Optional[str] = None,
     protein_names_uns_key: Optional[str] = None,
     categorical_covariate_keys: Optional[List[str]] = None,
     continuous_covariate_keys: Optional[List[str]] = None,
     copy: bool = False,
 ) -> Optional[anndata.AnnData]:
     """
-    Sets up :class:`~anndata.AnnData` object for `scvi` models.
+    Sets up :class:`~anndata.AnnData` object for models.
 
-    A mapping will be created between data fields used by `scvi` to their respective locations in adata.
+    A mapping will be created between data fields used by models to their respective locations in adata.
     This method will also compute the log mean and log variance per batch for the library size prior.
 
     None of the data in adata are modified. Only adds fields to adata.
 
     Parameters
     ----------
     adata
@@ -109,17 +109,17 @@
         if not `None`, uses this as the key in `adata.layers` for raw count data.
     protein_expression_obsm_key
         key in `adata.obsm` for protein expression data, Required for :class:`~scvi.model.TOTALVI`.
     protein_names_uns_key
         key in `adata.uns` for protein names. If None, will use the column names of `adata.obsm[protein_expression_obsm_key]`
         if it is a DataFrame, else will assign sequential names to proteins. Only relevant but not required for :class:`~scvi.model.TOTALVI`.
     categorical_covariate_keys
-        keys in `adata.obs` that correspond to categorical data. Used in some `scvi` models.
+        keys in `adata.obs` that correspond to categorical data. Used in some models.
     continuous_covariate_keys
-        keys in `adata.obs` that correspond to continuous data. Used in some `scvi` models.
+        keys in `adata.obs` that correspond to continuous data. Used in some models.
     copy
         if `True`, a copy of adata is returned.
 
     Returns
     -------
     If ``copy``,  will return :class:`~anndata.AnnData`.
     Adds the following fields to adata:
@@ -350,14 +350,17 @@
     adata_alternate_key_name
         Added key in adata_attr_name for categorical codes if `is_categorical` is True
     """
     if is_categorical is True:
         if adata_attr_name != "obs":
             raise ValueError("categorical handling only implemented for data in `.obs`")
 
+    if adata_alternate_key_name is None:
+        adata_alternate_key_name = adata_key_name + "_scvi"
+
     if is_categorical is True and adata_attr_name == "obs":
         adata_key_name = _make_obs_column_categorical(
             adata,
             column_key=adata_key_name,
             alternate_column_key=adata_alternate_key_name,
         )
     new_dict = {
@@ -953,15 +956,15 @@
     mappings = setup_dict["categorical_mappings"]
     version = setup_dict["scvi_version"]
 
     rich.print("Anndata setup with scvi-tools version {}.".format(version))
 
     n_cat = 0
     n_covs = 0
-    if "extra_categorical_mappings" in setup_dict.keys():
+    if "extra_categoricals" in setup_dict.keys():
         n_cat = len(setup_dict["extra_categoricals"]["mappings"])
     if "extra_continuous_keys" in setup_dict.keys():
         n_covs = len(setup_dict["extra_continuous_keys"])
 
     in_colab = "google.colab" in sys.modules
     force_jupyter = None if not in_colab else True
     console = Console(force_jupyter=force_jupyter)
@@ -1176,41 +1179,39 @@
     adata_labels_mapping = adata_categoricals["_scvi_labels"]["mapping"]
 
     transfer_setup = transfer_setup or _needs_transfer(
         self_labels_mapping, adata_labels_mapping, "label"
     )
 
     # validate any extra categoricals
+    error_msg = (
+        "Registered categorical key order mismatch between "
+        + "the anndata used to train and the anndata passed in."
+        + "Expected categories & order {}. Received {}.\n"
+    )
     if "extra_categoricals" in _scvi_dict.keys():
         target_dict = adata.uns["_scvi"]["extra_categoricals"]
         source_dict = _scvi_dict["extra_categoricals"]
         # check that order of keys setup is same
         if not np.array_equal(target_dict["keys"], source_dict["keys"]):
-            error_msg = (
-                "Registered categorical key order mismatch between "
-                + "the anndata used to train and the anndata passed in."
-                + "Expected categories & order {}. Received {}.\n"
-            )
             raise ValueError(error_msg.format(source_dict["keys"], target_dict["keys"]))
         # check mappings are equivalent
         target_extra_cat_maps = adata.uns["_scvi"]["extra_categoricals"]["mappings"]
         for key, val in source_dict["mappings"].items():
             target_map = target_extra_cat_maps[key]
             transfer_setup = transfer_setup or _needs_transfer(val, target_map, key)
     # validate any extra continuous covs
     if "extra_continuous_keys" in _scvi_dict.keys():
         if "extra_continuous_keys" not in adata.uns["_scvi"].keys():
             raise ValueError('extra_continuous_keys not in adata.uns["_scvi"]')
         target_cont_keys = adata.uns["_scvi"]["extra_continuous_keys"]
         source_cont_keys = _scvi_dict["extra_continuous_keys"]
-        n_keys = len(target_cont_keys)
-        if np.sum(source_cont_keys == target_cont_keys) != n_keys:
-            raise ValueError(
-                "extra_continous_keys are not the same between source and target"
-            )
+        # check that order of keys setup is same
+        if not np.array_equal(target_cont_keys, source_cont_keys):
+            raise ValueError(error_msg.format(source_cont_keys, target_cont_keys))
 
     return transfer_setup
 
 
 def _needs_transfer(mapping1, mapping2, category):
     needs_transfer = False
     error_msg = (
```

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_brain_large.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_brain_large.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_cite_seq.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_cite_seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 def _load_spleen_lymph_cite_seq(
     save_path: str = "data/",
     protein_join: str = "inner",
     remove_outliers: bool = True,
     run_setup_anndata: bool = True,
 ):
     """
-    Immune cells from the murine spleen and lymph nodes [GayosoSteier20]_.
+    Immune cells from the murine spleen and lymph nodes [GayosoSteier21]_.
 
     This dataset was used throughout the totalVI manuscript, and named SLN-all.
 
     Parameters
     ----------
     save_path
         Location to use when saving/loading the data.
```

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_cortex.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_cortex.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_csv.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_csv.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_dataset_10x.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_dataset_10x.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_download.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_download.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_loom.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_loom.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_pbmc.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_pbmc.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_seqfish.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_seqfish.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_smfish.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_smfish.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_built_in_data/_synthetic.py` & `scvi-tools-0.9.1/scvi/data/_built_in_data/_synthetic.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_datasets.py` & `scvi-tools-0.9.1/scvi/data/_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ._built_in_data._cite_seq import (
     _load_pbmcs_10x_cite_seq,
     _load_spleen_lymph_cite_seq,
 )
 from ._built_in_data._cortex import _load_cortex
 from ._built_in_data._csv import _load_breast_cancer_dataset, _load_mouse_ob_dataset
 from ._built_in_data._dataset_10x import _load_dataset_10x
+from ._built_in_data._heartcellatlas import _load_heart_cell_atlas_subsampled
 from ._built_in_data._loom import (
     _load_annotation_simulation,
     _load_frontalcortex_dropseq,
     _load_prefrontalcortex_starmap,
     _load_retina,
 )
 from ._built_in_data._pbmc import _load_pbmc_dataset, _load_purified_pbmc_dataset
@@ -466,15 +467,15 @@
 def spleen_lymph_cite_seq(
     save_path: str = "data/",
     protein_join: str = "inner",
     remove_outliers: bool = True,
     run_setup_anndata: bool = True,
 ) -> anndata.AnnData:
     """
-    Immune cells from the murine spleen and lymph nodes [GayosoSteier20]_.
+    Immune cells from the murine spleen and lymph nodes [GayosoSteier21]_.
 
     This dataset was used throughout the totalVI manuscript, and named SLN-all.
 
     Parameters
     ----------
     save_path
         Location to use when saving/loading the data.
@@ -628,7 +629,52 @@
         batch_size=batch_size,
         n_genes=n_genes,
         n_proteins=n_proteins,
         n_batches=n_batches,
         n_labels=n_labels,
         run_setup_anndata=run_setup_anndata,
     )
+
+
+def heart_cell_atlas_subsampled(
+    save_path: str = "data/",
+    remove_nuisance_clusters: bool = True,
+    run_setup_anndata: bool = True,
+) -> anndata.AnnData:
+    """
+    Combined single cell and single nuclei RNA-Seq data of 485K cardiac cells with annotations.
+
+    Dataset was filtered down randomly to 20k cells using :func:`~scanpy.pp.subsample`. The original
+    data can be downloaded from https://www.heartcellatlas.org/#DataSources.
+
+    Parameters
+    ----------
+    save_path
+        Location to use when saving/loading the data.
+    remove_nuisance_clusters
+        Remove doublets and unsassigned cells
+    run_setup_anndata
+        If true, runs setup_anndata() on dataset before returning
+
+    Returns
+    -------
+    AnnData
+
+    Notes
+    -----
+    The data were filtered using the following sequence::
+
+        >>> adata = anndata.read_h5ad(path_to_anndata)
+        >>> bdata = sc.pp.subsample(adata, n_obs=20000, copy=True)
+        >>> sc.pp.filter_genes(bdata, min_counts=3)
+        >>> bdata.write_h5ad(path, compression="gzip")
+
+    Examples
+    --------
+    >>> import scvi
+    >>> adata = scvi.data.heart_cell_atlas_subsampled()
+    """
+    return _load_heart_cell_atlas_subsampled(
+        save_path=save_path,
+        remove_nuisance_clusters=remove_nuisance_clusters,
+        run_setup_anndata=run_setup_anndata,
+    )
```

### Comparing `scvi-tools-0.9.0b1/scvi/data/_preprocessing.py` & `scvi-tools-0.9.1/scvi/data/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_read.py` & `scvi-tools-0.9.1/scvi/data/_read.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/data/_utils.py` & `scvi-tools-0.9.1/scvi/data/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/dataloaders/_ann_dataloader.py` & `scvi-tools-0.9.1/scvi/dataloaders/_ann_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/dataloaders/_anntorchdataset.py` & `scvi-tools-0.9.1/scvi/dataloaders/_anntorchdataset.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/dataloaders/_concat_dataloader.py` & `scvi-tools-0.9.1/scvi/dataloaders/_concat_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/dataloaders/_data_splitting.py` & `scvi-tools-0.9.1/scvi/dataloaders/_data_splitting.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/dataloaders/_semi_dataloader.py` & `scvi-tools-0.9.1/scvi/dataloaders/_semi_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/distributions/_negative_binomial.py` & `scvi-tools-0.9.1/scvi/distributions/_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/external/gimvi/_model.py` & `scvi-tools-0.9.1/scvi/external/gimvi/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import torch
 from anndata import AnnData, read
 from torch.utils.data import DataLoader
 
 from scvi import _CONSTANTS
 from scvi.data import transfer_anndata_setup
 from scvi.dataloaders import DataSplitter
-from scvi.lightning import Trainer
 from scvi.model._utils import _get_var_names_from_setup_anndata, parse_use_gpu_arg
 from scvi.model.base import BaseModelClass, VAEMixin
+from scvi.train import Trainer
 
 from ._module import JVAE
 from ._task import GIMVITrainingPlan
 
 logger = logging.getLogger(__name__)
 
 
@@ -48,15 +48,15 @@
     generative_distributions
         List of generative distribution for adata_seq data and adata_spatial data.
     model_library_size
         List of bool of whether to model library size for adata_seq and adata_spatial.
     n_latent
         Dimensionality of the latent space.
     **model_kwargs
-        Keyword args for :class:`~scvi.modules.JVAE`
+        Keyword args for :class:`~scvi.external.gimvi.JVAE`
 
     Examples
     --------
     >>> adata_seq = anndata.read_h5ad(path_to_anndata_seq)
     >>> adata_spatial = anndata.read_h5ad(path_to_anndata_spatial)
     >>> scvi.data.setup_anndata(adata_seq)
     >>> scvi.data.setup_anndata(adata_spatial)
@@ -157,15 +157,15 @@
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         batch_size
             Minibatch size to use during training.
         plan_kwargs
             Keyword args for model-specific Pytorch Lightning task. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         gpus, device = parse_use_gpu_arg(use_gpu)
 
         self.trainer = Trainer(
             max_epochs=max_epochs,
             gpus=gpus,
             **kwargs,
```

### Comparing `scvi-tools-0.9.0b1/scvi/external/gimvi/_module.py` & `scvi-tools-0.9.1/scvi/external/gimvi/_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,17 @@
 import torch
 import torch.nn.functional as F
 from torch.distributions import Normal, Poisson
 from torch.distributions import kl_divergence as kl
 from torch.nn import ModuleList
 
 from scvi import _CONSTANTS
-from scvi.compose import (
-    BaseModuleClass,
-    Encoder,
-    LossRecorder,
-    MultiDecoder,
-    MultiEncoder,
-    auto_move_data,
-    one_hot,
-)
 from scvi.distributions import NegativeBinomial, ZeroInflatedNegativeBinomial
+from scvi.module.base import BaseModuleClass, LossRecorder, auto_move_data
+from scvi.nn import Encoder, MultiDecoder, MultiEncoder, one_hot
 
 torch.backends.cudnn.benchmark = True
 
 
 class JVAE(BaseModuleClass):
     """
     Joint variational auto-encoder for imputing missing genes in spatial data.
```

### Comparing `scvi-tools-0.9.0b1/scvi/external/gimvi/_task.py` & `scvi-tools-0.9.1/scvi/external/gimvi/_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
 from scvi import _CONSTANTS
-from scvi.lightning import AdversarialTrainingPlan
-from scvi.modules import Classifier
+from scvi.module import Classifier
+from scvi.train import AdversarialTrainingPlan
 
 
 class GIMVITrainingPlan(AdversarialTrainingPlan):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if kwargs["adversarial_classifier"] is True:
             self.n_output_classifier = 2
```

### Comparing `scvi-tools-0.9.0b1/scvi/external/solo/_model.py` & `scvi-tools-0.9.1/scvi/external/solo/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 import numpy as np
 import torch
 from anndata import AnnData
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
 from scvi import _CONSTANTS
-from scvi.compose import auto_move_data
 from scvi.data import get_from_registry, setup_anndata
 from scvi.dataloaders import DataSplitter
-from scvi.lightning import ClassifierTrainingPlan
 from scvi.model import SCVI
-from scvi.model.base import BaseModelClass, TrainRunner
-from scvi.modules import Classifier
+from scvi.model.base import BaseModelClass
+from scvi.module import Classifier
+from scvi.module.base import auto_move_data
+from scvi.train import ClassifierTrainingPlan, TrainRunner
 
 logger = logging.getLogger(__name__)
 
 LABELS_KEY = "_solo_doub_sim"
 
 
 class SOLO(BaseModelClass):
@@ -34,15 +34,15 @@
     Parameters
     ----------
     adata
         AnnData object that has been registered via :func:`~scvi.data.setup_anndata`.
         Object should contain latent representation of real cells and doublets as `adata.X`.
         Object should also be registered, using `.X` and `labels_key="_solo_doub_sim"`.
     **classifier_kwargs
-        Keyword args for :class:`~scvi.modules.Classifier`
+        Keyword args for :class:`~scvi.module.Classifier`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata)
     >>> vae = scvi.model.SCVI(adata)
     >>> vae.train()
@@ -50,25 +50,25 @@
     >>> solo.train()
     >>> solo.predict()
     """
 
     def __init__(
         self,
         adata: AnnData,
-        **model_kwargs,
+        **classifier_kwargs,
     ):
         # TODO, catch user warning here and logger warning
         # about non count data
         super().__init__(adata)
 
         self.module = Classifier(
             n_input=self.summary_stats["n_vars"],
             n_labels=2,
             logits=True,
-            **model_kwargs,
+            **classifier_kwargs,
         )
         self._model_summary_string = "Solo model"
         self.init_params_ = self._get_init_params(locals())
 
     @classmethod
     def from_scvi_model(cls, scvi_model: SCVI, adata: Optional[AnnData] = None):
         """
@@ -171,24 +171,24 @@
             Size of training set in the range [0.0, 1.0].
         validation_size
             Size of the test set. If `None`, defaults to 1 - `train_size`. If
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         batch_size
             Minibatch size to use during training.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.ClassifierTrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.ClassifierTrainingPlan`. Keyword arguments passed to
         early_stopping
             Adds callback for early stopping on validation_loss
         early_stopping_patience
             Number of times early stopping metric can not improve over early_stopping_min_delta
         early_stopping_min_delta
             Threshold for counting an epoch torwards patience
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         update_dict = {
             "lr": lr,
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
```

### Comparing `scvi-tools-0.9.0b1/scvi/external/stereoscope/_model.py` & `scvi-tools-0.9.1/scvi/external/stereoscope/_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     https://github.com/almaan/stereoscope.
 
     Parameters
     ----------
     sc_adata
         single-cell AnnData object that has been registered via :func:`~scvi.data.setup_anndata`.
     **model_kwargs
-        Keyword args for :class:`~scvi.external.RNADeconv`
+        Keyword args for :class:`~scvi.external.stereoscope.RNADeconv`
 
     Examples
     --------
     >>> sc_adata = anndata.read_h5ad(path_to_sc_anndata)
-    >>> scvi.data.setup_anndata(sc_adata, label_key="labels")
-    >>> stereo = scvi.external.RNAStereoscope(sc_adata)
+    >>> scvi.data.setup_anndata(sc_adata, labels_key="labels")
+    >>> stereo = scvi.external.stereoscope.RNAStereoscope(sc_adata)
     >>> stereo.train()
     """
 
     def __init__(
         self,
         sc_adata: AnnData,
         **model_kwargs,
@@ -80,18 +80,18 @@
             Size of training set in the range [0.0, 1.0].
         validation_size
             Size of the test set. If `None`, defaults to 1 - `train_size`. If
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         batch_size
             Minibatch size to use during training.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.TrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         update_dict = {
             "lr": lr,
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
@@ -121,33 +121,33 @@
         parameters of the model learned from the single-cell RNA seq data for deconvolution.
     cell_type_mapping
         numpy array mapping for the cell types used in the deconvolution
     prior_weight
         how to reweight the minibatches for stochastic optimization. "n_obs" is the valid
         procedure, "minibatch" is the procedure implemented in Stereoscope.
     **model_kwargs
-        Keyword args for :class:`~scvi.external.SpatialDeconv`
+        Keyword args for :class:`~scvi.external.stereoscope.SpatialDeconv`
 
     Examples
     --------
     >>> sc_adata = anndata.read_h5ad(path_to_sc_anndata)
-    >>> scvi.data.setup_anndata(sc_adata, label_key="labels")
-    >>> sc_model = scvi.external.RNAStereoscope(sc_adata)
+    >>> scvi.data.setup_anndata(sc_adata, labels_key="labels")
+    >>> sc_model = scvi.external.stereoscope.RNAStereoscope(sc_adata)
     >>> sc_model.train()
     >>> st_adata = anndata.read_h5ad(path_to_st_anndata)
     >>> scvi.data.setup_anndata(st_adata)
-    >>> stereo = scvi.external.SpatialStereoscope.from_rna_model(st_adata, sc_model)
+    >>> stereo = scvi.external.stereoscope.SpatialStereoscope.from_rna_model(st_adata, sc_model)
     >>> stereo.train()
-    >>> st_adata.obs["deconv"] = stereo.get_proportions()
+    >>> st_adata.obsm["deconv"] = stereo.get_proportions()
 
     Notes
     -----
     See further usage examples in the following tutorials:
 
-    1. :doc:`/user_guide/notebooks/stereoscope_public_LV`
+    1. :doc:`/user_guide/notebooks/stereoscope_heart_LV_tutorial`
     """
 
     def __init__(
         self,
         st_adata: AnnData,
         sc_params: Tuple[np.ndarray],
         cell_type_mapping: np.ndarray,
@@ -244,18 +244,18 @@
             Learning rate for optimization.
         use_gpu
             Use default GPU if available (if None or True), or index of GPU to use (if int),
             or name of GPU (if str), or use CPU (if False).
         batch_size
             Minibatch size to use during training.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.TrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         update_dict = {
             "lr": lr,
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
```

### Comparing `scvi-tools-0.9.0b1/scvi/external/stereoscope/_module.py` & `scvi-tools-0.9.1/scvi/external/stereoscope/_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import torch
 from torch.distributions import NegativeBinomial, Normal
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import BaseModuleClass, LossRecorder, auto_move_data
+from scvi.module.base import BaseModuleClass, LossRecorder, auto_move_data
 
 
 class RNADeconv(BaseModuleClass):
     """
     Model of single-cell RNA-sequencing data for deconvolution of spatial transriptomics.
 
     Reimplementation of the ScModel module of Stereoscope [Andersson20]_:
```

### Comparing `scvi-tools-0.9.0b1/scvi/lightning/_callbacks.py` & `scvi-tools-0.9.1/scvi/train/_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     mode
         one of ["min", "max"].
     period
         Interval (number of epochs) between checkpoints.
 
     Examples
     --------
-    from scvi.lightning import Trainer
-    from scvi.lightning import SaveBestState
+    from scvi.train import Trainer
+    from scvi.train import SaveBestState
     """
 
     def __init__(
         self,
         monitor: str = "elbo_validation",
         mode: str = "min",
         verbose=False,
```

### Comparing `scvi-tools-0.9.0b1/scvi/lightning/_logger.py` & `scvi-tools-0.9.1/scvi/train/_logger.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/lightning/_progress.py` & `scvi-tools-0.9.1/scvi/train/_progress.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/lightning/_trainer.py` & `scvi-tools-0.9.1/scvi/train/_trainer.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,14 +40,30 @@
         If `True`, enable checkpointing. It will configure a default ModelCheckpoint
         callback if there is no user-defined ModelCheckpoint in `callbacks`.
     num_sanity_val_steps
         Sanity check runs n validation batches before starting the training routine.
         Set it to -1 to run all batches in all validation dataloaders.
     weights_summary
         Prints a summary of the weights when training begins.
+    early_stopping
+        Whether to perform early stopping with respect to the validation set. This
+        automatically adds a :class:`~pytorch_lightning.callbacks.early_stopping.EarlyStopping`
+        instance. A custom instance can be passed by using the callbacks argument and
+        setting this to `False`.
+    early_stopping_monitor
+        Metric logged during validation set epoch. The available metrics will depend on
+        the training plan class used. We list the most common options here in the typing.
+    early_stopping_min_delta
+        Minimum change in the monitored quantity to qualify as an improvement,
+        i.e. an absolute change of less than min_delta, will count as no improvement.
+    early_stopping_patience
+        Number of validation epochs with no improvement after which training will be stopped.
+    early_stopping_mode
+            In 'min' mode, training will stop when the quantity monitored has stopped decreasing
+            and in 'max' mode it will stop when the quantity monitored has stopped increasing.
     progress_bar_refresh_rate
         How often to refresh progress bar (in steps). Value 0 disables progress bar.
     simple_progress_bar
         Use custom scvi-tools simple progress bar (per epoch rather than per batch)
     logger
         A valid pytorch lightning logger. Defaults to a simple dictionary logger.
         If `True`, defaults to the default pytorch lightning logger.
@@ -124,8 +140,13 @@
 
     def fit(self, *args, **kwargs):
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 action="ignore", category=UserWarning, message="The dataloader,"
             )
+            warnings.filterwarnings(
+                action="ignore",
+                category=UserWarning,
+                message="you defined a validation_step but have no val_dataloader",
+            )
             super().fit(*args, **kwargs)
```

### Comparing `scvi-tools-0.9.0b1/scvi/lightning/_trainingplans.py` & `scvi-tools-0.9.1/scvi/train/_trainingplans.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import pyro
 import pytorch_lightning as pl
 import torch
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import BaseModuleClass, PyroBaseModuleClass, one_hot
-from scvi.modules import Classifier
+from scvi.module import Classifier
+from scvi.module.base import BaseModuleClass, PyroBaseModuleClass
+from scvi.nn import one_hot
 
 
 class TrainingPlan(pl.LightningModule):
     """
     Lightning module task to train scvi-tools modules.
 
     Parameters
     ----------
-    vae_model
-        A model instance from class ``BaseModuleClass``.
+    module
+        A module instance from class ``BaseModuleClass``.
     n_obs_training
         Number of observations in the training set.
     lr
         Learning rate used for optimization.
     weight_decay
         Weight decay used in optimizatoin.
     eps
@@ -46,21 +47,21 @@
     lr_threshold
         Threshold for measuring the new optimum.
     lr_scheduler_metric
         Which metric to track for learning rate reduction.
     lr_min
         Minimum learning rate allowed
     **loss_kwargs
-        Keyword args to pass to the loss method of the `vae_model`.
+        Keyword args to pass to the loss method of the `module`.
         `kl_weight` should not be passed here and is handled automatically.
     """
 
     def __init__(
         self,
-        vae_model: BaseModuleClass,
+        module: BaseModuleClass,
         n_obs_training: int,
         lr: float = 1e-3,
         weight_decay: float = 1e-6,
         eps: float = 0.01,
         optimizer: Literal["Adam", "AdamW"] = "Adam",
         n_steps_kl_warmup: Union[int, None] = None,
         n_epochs_kl_warmup: Union[int, None] = 400,
@@ -71,15 +72,15 @@
         lr_scheduler_metric: Literal[
             "elbo_validation", "reconstruction_loss_validation", "kl_local_validation"
         ] = "elbo_validation",
         lr_min: float = 0,
         **loss_kwargs,
     ):
         super(TrainingPlan, self).__init__()
-        self.module = vae_model
+        self.module = module
         self.n_obs_training = n_obs_training
         self.lr = lr
         self.weight_decay = weight_decay
         self.eps = eps
         self.optimizer_name = optimizer
         self.n_steps_kl_warmup = n_steps_kl_warmup
         self.n_epochs_kl_warmup = n_epochs_kl_warmup
@@ -204,16 +205,16 @@
 
 class AdversarialTrainingPlan(TrainingPlan):
     """
     Train vaes with adversarial loss option to encourage latent space mixing.
 
     Parameters
     ----------
-    vae_model
-        A model instance from class ``BaseModuleClass``.
+    module
+        A module instance from class ``BaseModuleClass``.
     n_obs_training
         Number of observations in the training set.
     lr
         Learning rate used for optimization :class:`~torch.optim.Adam`.
     weight_decay
         Weight decay used in :class:`~torch.optim.Adam`.
     n_steps_kl_warmup
@@ -238,21 +239,21 @@
     adversarial_classifier
         Whether to use adversarial classifier in the latent space
     scale_adversarial_loss
         Scaling factor on the adversarial components of the loss.
         By default, adversarial loss is scaled from 1 to 0 following opposite of
         kl warmup.
     **loss_kwargs
-        Keyword args to pass to the loss method of the `vae_model`.
+        Keyword args to pass to the loss method of the `module`.
         `kl_weight` should not be passed here and is handled automatically.
     """
 
     def __init__(
         self,
-        vae_model: BaseModuleClass,
+        module: BaseModuleClass,
         n_obs_training,
         lr=1e-3,
         weight_decay=1e-6,
         n_steps_kl_warmup: Union[int, None] = None,
         n_epochs_kl_warmup: Union[int, None] = 400,
         reduce_lr_on_plateau: bool = False,
         lr_factor: float = 0.6,
@@ -263,15 +264,15 @@
         ] = "elbo_validation",
         lr_min: float = 0,
         adversarial_classifier: Union[bool, Classifier] = False,
         scale_adversarial_loss: Union[float, Literal["auto"]] = "auto",
         **loss_kwargs,
     ):
         super().__init__(
-            vae_model=vae_model,
+            module=module,
             n_obs_training=n_obs_training,
             lr=lr,
             weight_decay=weight_decay,
             n_steps_kl_warmup=n_steps_kl_warmup,
             n_epochs_kl_warmup=n_epochs_kl_warmup,
             reduce_lr_on_plateau=reduce_lr_on_plateau,
             lr_factor=lr_factor,
@@ -404,16 +405,16 @@
 
 class SemiSupervisedTrainingPlan(TrainingPlan):
     """
     Lightning module task for SemiSupervised Training.
 
     Parameters
     ----------
-    vae_model
-        A model instance from class ``BaseModuleClass``.
+    module
+        A module instance from class ``BaseModuleClass``.
     classification_ratio
         Weight of the classification_loss in loss function
     lr
         Learning rate used for optimization :class:`~torch.optim.Adam`.
     weight_decay
         Weight decay used in :class:`~torch.optim.Adam`.
     n_steps_kl_warmup
@@ -430,21 +431,21 @@
     lr_patience
         Number of epochs with no improvement after which learning rate will be reduced.
     lr_threshold
         Threshold for measuring the new optimum.
     lr_scheduler_metric
         Which metric to track for learning rate reduction.
     **loss_kwargs
-        Keyword args to pass to the loss method of the `vae_model`.
+        Keyword args to pass to the loss method of the `module`.
         `kl_weight` should not be passed here and is handled automatically.
     """
 
     def __init__(
         self,
-        vae_model: BaseModuleClass,
+        module: BaseModuleClass,
         classification_ratio: int = 50,
         lr=1e-3,
         weight_decay=1e-6,
         n_steps_kl_warmup: Union[int, None] = None,
         n_epochs_kl_warmup: Union[int, None] = 400,
         reduce_lr_on_plateau: bool = False,
         lr_factor: float = 0.6,
@@ -452,15 +453,15 @@
         lr_threshold: float = 0.0,
         lr_scheduler_metric: Literal[
             "elbo_validation", "reconstruction_loss_validation", "kl_local_validation"
         ] = "elbo_validation",
         **loss_kwargs,
     ):
         super(SemiSupervisedTrainingPlan, self).__init__(
-            vae_model=vae_model,
+            module=module,
             n_obs_training=1,  # no impact with choice
             lr=lr,
             weight_decay=weight_decay,
             n_steps_kl_warmup=n_steps_kl_warmup,
             n_epochs_kl_warmup=n_epochs_kl_warmup,
             reduce_lr_on_plateau=reduce_lr_on_plateau,
             lr_factor=lr_factor,
@@ -486,21 +487,25 @@
             feed_labels=False,
             labelled_tensors=labelled_dataset,
         )
         input_kwargs.update(self.loss_kwargs)
         _, _, scvi_losses = self.forward(full_dataset, loss_kwargs=input_kwargs)
         loss = scvi_losses.loss
         reconstruction_loss = scvi_losses.reconstruction_loss
-        return {
+        loss_dict = {
             "loss": loss,
             "reconstruction_loss_sum": reconstruction_loss.sum(),
             "kl_local_sum": scvi_losses.kl_local.sum(),
             "kl_global": scvi_losses.kl_global,
             "n_obs": reconstruction_loss.shape[0],
         }
+        if hasattr(scvi_losses, "classification_loss"):
+            loss_dict["classification_loss"] = scvi_losses.classification_loss
+            loss_dict["n_labelled_tensors"] = scvi_losses.n_labelled_tensors
+        return loss_dict
 
     def validation_step(self, batch, batch_idx, optimizer_idx=0):
         # Potentially dangerous if batch is from a single dataloader with two keys
         if len(batch) == 2:
             full_dataset = batch[0]
             labelled_dataset = batch[1]
         else:
@@ -511,21 +516,59 @@
             feed_labels=False,
             labelled_tensors=labelled_dataset,
         )
         input_kwargs.update(self.loss_kwargs)
         _, _, scvi_losses = self.forward(full_dataset, loss_kwargs=input_kwargs)
         loss = scvi_losses.loss
         reconstruction_loss = scvi_losses.reconstruction_loss
-        return {
+
+        loss_dict = {
             "loss": loss,
             "reconstruction_loss_sum": reconstruction_loss.sum(),
             "kl_local_sum": scvi_losses.kl_local.sum(),
             "kl_global": scvi_losses.kl_global,
             "n_obs": reconstruction_loss.shape[0],
         }
+        if hasattr(scvi_losses, "classification_loss"):
+            loss_dict["classification_loss"] = scvi_losses.classification_loss
+            loss_dict["n_labelled_tensors"] = scvi_losses.n_labelled_tensors
+        return loss_dict
+
+    def training_epoch_end(self, outputs):
+        super().training_epoch_end(outputs)
+        classifier_loss, total_labelled_tensors = 0, 0
+
+        for tensors in outputs:
+            if "classification_loss" in tensors.keys():
+                n_labelled = tensors["n_labelled_tensors"]
+                total_labelled_tensors += n_labelled
+                classification_loss = tensors["classification_loss"]
+                classifier_loss += classification_loss * n_labelled
+
+        if total_labelled_tensors > 0:
+            self.log(
+                "classification_loss_train", classifier_loss / total_labelled_tensors
+            )
+
+    def validation_epoch_end(self, outputs):
+        super().validation_epoch_end(outputs)
+        classifier_loss, total_labelled_tensors = 0, 0
+
+        for tensors in outputs:
+            if "classification_loss" in tensors.keys():
+                n_labelled = tensors["n_labelled_tensors"]
+                total_labelled_tensors += n_labelled
+                classification_loss = tensors["classification_loss"]
+                classifier_loss += classification_loss * n_labelled
+
+        if total_labelled_tensors > 0:
+            self.log(
+                "classification_loss_validation",
+                classifier_loss / total_labelled_tensors,
+            )
 
 
 class PyroTrainingPlan(pl.LightningModule):
     """
     Lightning module task to train Pyro scvi-tools modules.
 
     Parameters
@@ -535,24 +578,36 @@
         should have callable `model` and `guide` attributes or methods.
     loss_fn
         A Pyro loss. Should be a subclass of :class:`~pyro.infer.ELBO`.
         If `None`, defaults to :class:`~pyro.infer.Trace_ELBO`.
     optim
         A Pyro optimizer, e.g., :class:`~pyro.optim.Adam`. If `None`,
         defaults to Adam optimizer with a learning rate of `1e-3`.
+    n_obs
+        Number of training examples. If not `None`, updates the `n_obs` attr
+        of the Pyro module's `model` and `guide`, if they exist.
     """
 
     def __init__(
         self,
         pyro_module: PyroBaseModuleClass,
         loss_fn: Optional[pyro.infer.ELBO] = None,
         optim: Optional[pyro.optim.PyroOptim] = None,
+        n_obs: Optional[int] = None,
     ):
         super().__init__()
         self.module = pyro_module
+        self.n_obs = n_obs
+
+        # important for scaling log prob in Pyro plates
+        if n_obs is not None:
+            if hasattr(self.module.model, "n_obs"):
+                setattr(self.module.model, "n_obs", n_obs)
+            if hasattr(self.module.guide, "n_obs"):
+                setattr(self.module.guide, "n_obs", n_obs)
 
         self.loss_fn = pyro.infer.Trace_ELBO() if loss_fn is None else loss_fn
         self.optim = pyro.optim.Adam({"lr": 1e-3}) if optim is None else optim
 
         self.automatic_optimization = False
         self.pyro_guide = self.module.guide
         self.pyro_model = self.module.model
@@ -586,15 +641,15 @@
 class ClassifierTrainingPlan(pl.LightningModule):
     """
     Lightning module task to train a simple MLP classifier.
 
     Parameters
     ----------
     classifier
-        A model instance from :class:`~scvi.modules.Classifier`.
+        A model instance from :class:`~scvi.module.Classifier`.
     lr
         Learning rate used for optimization.
     weight_decay
         Weight decay used in optimizatoin.
     eps
         eps used for optimization.
     optimizer
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_autozi.py` & `scvi-tools-0.9.1/scvi/model/_autozi.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from anndata import AnnData
 from torch import logsumexp
 from torch.distributions import Beta, Normal
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
 from scvi.model.base import UnsupervisedTrainingMixin
-from scvi.modules import AutoZIVAE
+from scvi.module import AutoZIVAE
 
 from .base import BaseModelClass, VAEMixin
 
 logger = logging.getLogger(__name__)
 
 # register buffer
 
@@ -64,15 +64,15 @@
     zero_inflation: One of the following
 
         * ``'gene'`` - zero-inflation Bernoulli parameter of AutoZI is constant per gene across cells
         * ``'gene-batch'`` - zero-inflation Bernoulli parameter can differ between different batches
         * ``'gene-label'`` - zero-inflation Bernoulli parameter can differ between different labels
         * ``'gene-cell'`` - zero-inflation Bernoulli parameter can differ for every gene in every cell
     **model_kwargs
-        Keyword args for :class:`~scvi.core.modules.AutoZIVAE`
+        Keyword args for :class:`~scvi.module.AutoZIVAE`
 
     Examples
     --------
 
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata, batch_key="batch")
     >>> vae = scvi.model.AutoZIVAE(adata)
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_linear_scvi.py` & `scvi-tools-0.9.1/scvi/model/_linear_scvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 from anndata import AnnData
 
 from scvi._compat import Literal
 from scvi.model._utils import _get_var_names_from_setup_anndata
 from scvi.model.base import UnsupervisedTrainingMixin
-from scvi.modules import LDVAE
+from scvi.module import LDVAE
 
 from .base import BaseModelClass, RNASeqMixin, VAEMixin
 
 logger = logging.getLogger(__name__)
 
 
 class LinearSCVI(RNASeqMixin, VAEMixin, UnsupervisedTrainingMixin, BaseModelClass):
@@ -44,15 +44,15 @@
         * ``'poisson'`` - Poisson distribution
     latent_distribution
         One of:
 
         * ``'normal'`` - Normal distribution
         * ``'ln'`` - Logistic normal distribution (Normal(0, I) transformed by softmax)
     **model_kwargs
-        Keyword args for :class:`~scvi.modules.LDVAE`
+        Keyword args for :class:`~scvi.module.LDVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata, batch_key="batch")
     >>> vae = scvi.model.LinearSCVI(adata)
     >>> vae.train()
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_metrics.py` & `scvi-tools-0.9.1/scvi/model/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/model/_peakvi.py` & `scvi-tools-0.9.1/scvi/model/_peakvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import torch
 from anndata import AnnData
 from scipy.sparse import csr_matrix, vstack
 
 from scvi._compat import Literal
 from scvi._docs import doc_differential_expression
 from scvi._utils import _doc_params
-from scvi.lightning._callbacks import SaveBestState
 from scvi.model._utils import (
     _get_batch_code_from_category,
     _get_var_names_from_setup_anndata,
     scatac_raw_counts_properties,
 )
 from scvi.model.base import UnsupervisedTrainingMixin
-from scvi.modules import PEAKVAE
+from scvi.module import PEAKVAE
+from scvi.train._callbacks import SaveBestState
 
 from .base import ArchesMixin, BaseModelClass, VAEMixin
 from .base._utils import _de_core
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,14 +54,16 @@
         One of
 
         * ``'normal'`` - Normal distribution (Default)
         * ``'ln'`` - Logistic normal distribution (Normal(0, I) transformed by softmax)
     deeply_inject_covariates
         Whether to deeply inject covariates into all layers of the decoder. If False (default),
         covairates will only be included in the input layer.
+    **model_kwargs
+        Keyword args for :class:`~scvi.module.PEAKVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.dataset.setup_anndata(adata, batch_key="batch")
     >>> vae = scvi.model.PEAKVI(adata)
     >>> vae.train()
@@ -177,18 +179,18 @@
             Number of training steps (minibatches) to scale weight on KL divergences from 0 to 1.
             Only activated when `n_epochs_kl_warmup` is set to None. If `None`, defaults
             to `floor(0.75 * adata.n_obs)`.
         n_epochs_kl_warmup
             Number of epochs to scale weight on KL divergences from 0 to 1.
             Overrides `n_steps_kl_warmup` when both are not `None`.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.VAETask`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         update_dict = dict(
             lr=lr,
             weight_decay=weight_decay,
             eps=eps,
             n_epochs_kl_warmup=n_epochs_kl_warmup,
             n_steps_kl_warmup=n_steps_kl_warmup,
@@ -340,18 +342,20 @@
         group1: Optional[Iterable[str]] = None,
         group2: Optional[str] = None,
         idx1: Optional[Union[Sequence[int], Sequence[bool]]] = None,
         idx2: Optional[Union[Sequence[int], Sequence[bool]]] = None,
         mode: Literal["vanilla", "change"] = "change",
         delta: float = 0.1,
         batch_size: Optional[int] = None,
+        all_stats: bool = True,
         batch_correction: bool = False,
         batchid1: Optional[Iterable[str]] = None,
         batchid2: Optional[Iterable[str]] = None,
         fdr_target: float = 0.05,
+        silent: bool = False,
         two_sided: bool = True,
         **kwargs,
     ) -> pd.DataFrame:
         r"""
         A unified method for differential accessibility analysis.
 
         Implements `"vanilla"` DE [Lopez18]_ and `"change"` mode DE [Boyeau19]_.
@@ -413,25 +417,26 @@
             adata=adata,
             model_fn=model_fn,
             groupby=groupby,
             group1=group1,
             group2=group2,
             idx1=idx1,
             idx2=idx2,
-            all_stats=True,
+            all_stats=all_stats,
             all_stats_fn=scatac_raw_counts_properties,
             col_names=col_names,
             mode=mode,
             batchid1=batchid1,
             batchid2=batchid2,
             delta=delta,
             batch_correction=batch_correction,
             fdr=fdr_target,
             change_fn=change_fn,
             m1_domain_fn=m1_domain_fn,
+            silent=silent,
             **kwargs,
         )
 
         # manually change the results DataFrame to fit a PeakVI differential accessibility results
         result = pd.DataFrame(
             {
                 "prob_da": result.proba_de,
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_scanvi.py` & `scvi-tools-0.9.1/scvi/model/_scanvi.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 from scvi._compat import Literal
 from scvi.data._anndata import _make_obs_column_categorical
 from scvi.dataloaders import (
     AnnDataLoader,
     SemiSupervisedDataLoader,
     SemiSupervisedDataSplitter,
 )
-from scvi.lightning import SemiSupervisedTrainingPlan
-from scvi.lightning._callbacks import SubSampleLabels
-from scvi.modules import SCANVAE
+from scvi.module import SCANVAE
+from scvi.train import SemiSupervisedTrainingPlan, TrainRunner
+from scvi.train._callbacks import SubSampleLabels
 
 from ._scvi import SCVI
-from .base import ArchesMixin, BaseModelClass, RNASeqMixin, TrainRunner, VAEMixin
+from .base import ArchesMixin, BaseModelClass, RNASeqMixin, VAEMixin
 
 logger = logging.getLogger(__name__)
 
 
 class SCANVI(RNASeqMixin, VAEMixin, ArchesMixin, BaseModelClass):
     """
-    Single-cell annotation using variational inference [Xu20]_.
+    Single-cell annotation using variational inference [Xu21]_.
 
     Inspired from M1 + M2 model, as described in (https://arxiv.org/pdf/1406.5298.pdf).
 
     Parameters
     ----------
     adata
         AnnData object that has been registered via :func:`~scvi.data.setup_anndata`.
@@ -55,15 +55,15 @@
     gene_likelihood
         One of:
 
         * ``'nb'`` - Negative binomial distribution
         * ``'zinb'`` - Zero-inflated negative binomial distribution
         * ``'poisson'`` - Poisson distribution
     **model_kwargs
-        Keyword args for :class:`~scvi.modules.SCANVAE`
+        Keyword args for :class:`~scvi.module.SCANVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata, batch_key="batch", labels_key="labels")
     >>> vae = scvi.model.SCANVI(adata, "Unknown")
     >>> vae.train()
@@ -72,14 +72,15 @@
 
     Notes
     -----
     See further usage examples in the following tutorials:
 
     1. :doc:`/user_guide/notebooks/harmonization`
     2. :doc:`/user_guide/notebooks/scarches_scvi_tools`
+    3. :doc:`/user_guide/notebooks/seed_labeling`
     """
 
     def __init__(
         self,
         adata: AnnData,
         unlabeled_category: Union[str, int, float],
         n_hidden: int = 128,
@@ -165,20 +166,33 @@
             AnnData object that has been registered via :func:`~scvi.data.setup_anndata`.
         scanvi_kwargs
             kwargs for scanVI model
         """
         if scvi_model.is_trained_ is False:
             logger.warning("Passed in scvi model hasn't been trained yet.")
 
+        scanvi_kwargs = dict(scanvi_kwargs)
         init_params = scvi_model.init_params_
         non_kwargs = init_params["non_kwargs"]
+        kwargs = init_params["kwargs"]
+        kwargs = {k: v for (i, j) in kwargs.items() for (k, v) in j.items()}
+        for k, v in {**non_kwargs, **kwargs}.items():
+            if k in scanvi_kwargs.keys():
+                logger.warning(
+                    "Ignoring param '{}' as it was already passed in to ".format(k)
+                    + "pretrained scvi model with value {}.".format(v)
+                )
+                del scanvi_kwargs[k]
+
         if adata is None:
             adata = scvi_model.adata
 
-        scanvi_model = cls(adata, unlabeled_category, **non_kwargs, **scanvi_kwargs)
+        scanvi_model = cls(
+            adata, unlabeled_category, **non_kwargs, **kwargs, **scanvi_kwargs
+        )
         scvi_state_dict = scvi_model.module.state_dict()
         scanvi_model.module.load_state_dict(scvi_state_dict, strict=False)
 
         return scanvi_model
 
     def _set_indices_and_labels(self):
         """
@@ -314,18 +328,18 @@
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         batch_size
             Minibatch size to use during training.
         use_gpu
             Use default GPU if available (if None or True), or index of GPU to use (if int),
             or name of GPU (if str), or use CPU (if False).
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.SemiSupervisedTrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.SemiSupervisedTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
 
         if max_epochs is None:
             n_cells = self.adata.n_obs
             max_epochs = np.min([round((20000 / n_cells) * 400), 400])
 
         logger.info("Training for {} epochs.".format(max_epochs))
@@ -342,17 +356,15 @@
             unlabeled_category=self.unlabeled_category_,
             train_size=train_size,
             validation_size=validation_size,
             n_samples_per_label=n_samples_per_label,
             batch_size=batch_size,
             use_gpu=use_gpu,
         )
-        training_plan = SemiSupervisedTrainingPlan(
-            self.module, len(data_splitter.train_idx), **plan_kwargs
-        )
+        training_plan = SemiSupervisedTrainingPlan(self.module, **plan_kwargs)
         if "callbacks" in trainer_kwargs.keys():
             trainer_kwargs["callbacks"].concatenate(sampler_callback)
         else:
             trainer_kwargs["callbacks"] = sampler_callback
 
         runner = TrainRunner(
             self,
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_scvi.py` & `scvi-tools-0.9.1/scvi/model/_scvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from anndata import AnnData
 
 from scvi._compat import Literal
 from scvi.model.base import UnsupervisedTrainingMixin
-from scvi.modules import VAE
+from scvi.module import VAE
 
 from .base import ArchesMixin, BaseModelClass, RNASeqMixin, VAEMixin
 
 logger = logging.getLogger(__name__)
 
 
 class SCVI(
@@ -44,15 +44,15 @@
         * ``'poisson'`` - Poisson distribution
     latent_distribution
         One of:
 
         * ``'normal'`` - Normal distribution
         * ``'ln'`` - Logistic normal distribution (Normal(0, I) transformed by softmax)
     **model_kwargs
-        Keyword args for :class:`~scvi.modules.VAE`
+        Keyword args for :class:`~scvi.module.VAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata, batch_key="batch")
     >>> vae = scvi.model.SCVI(adata)
     >>> vae.train()
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_totalvi.py` & `scvi-tools-0.9.1/scvi/model/_totalvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 from scvi import _CONSTANTS
 from scvi._compat import Literal
 from scvi._docs import doc_differential_expression
 from scvi._utils import _doc_params
 from scvi.data import get_from_registry
 from scvi.data._utils import _check_nonnegative_integers
 from scvi.dataloaders import DataSplitter
-from scvi.lightning import AdversarialTrainingPlan
 from scvi.model._utils import (
     _get_batch_code_from_category,
     _get_var_names_from_setup_anndata,
     cite_seq_raw_counts_properties,
 )
-from scvi.model.base import TrainRunner
 from scvi.model.base._utils import _de_core
-from scvi.modules import TOTALVAE
+from scvi.module import TOTALVAE
+from scvi.train import AdversarialTrainingPlan, TrainRunner
 
 from .base import ArchesMixin, BaseModelClass, RNASeqMixin, VAEMixin
 
 logger = logging.getLogger(__name__)
 Number = TypeVar("Number", int, float)
 
 
 class TOTALVI(RNASeqMixin, VAEMixin, ArchesMixin, BaseModelClass):
     """
-    total Variational Inference [GayosoSteier20]_.
+    total Variational Inference [GayosoSteier21]_.
 
     Parameters
     ----------
     adata
         AnnData object that has been registered via :func:`~scvi.data.setup_anndata`.
     n_latent
         Dimensionality of the latent space.
@@ -64,15 +63,15 @@
         * ``'normal'`` - Normal distribution
         * ``'ln'`` - Logistic normal distribution (Normal(0, I) transformed by softmax)
     empirical_protein_background_prior
         Set the initialization of protein background prior empirically. This option fits a GMM for each of
         100 cells per batch and averages the distributions. Note that even with this option set to `True`,
         this only initializes a parameter that is learned during inference. If `False`, randomly initializes.
     **model_kwargs
-        Keyword args for :class:`~scvi.modules.TOTALVAE`
+        Keyword args for :class:`~scvi.module.TOTALVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.data.setup_anndata(adata, batch_key="batch", protein_expression_obsm_key="protein_expression")
     >>> vae = scvi.model.TOTALVI(adata)
     >>> vae.train()
@@ -197,18 +196,18 @@
             Number of epochs to scale weight on KL divergences from 0 to 1.
             Overrides `n_steps_kl_warmup` when both are not `None`.
         adversarial_classifier
             Whether to use adversarial classifier in the latent space. This helps mixing when
             there are missing proteins in any of the batches. Defaults to `True` is missing proteins
             are detected.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.AdversarialTrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.AdversarialTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if adversarial_classifier is None:
             imputation = (
                 True if "totalvi_batch_mask" in self.scvi_setup_dict_.keys() else False
             )
             adversarial_classifier = True if imputation else False
         n_steps_kl_warmup = (
@@ -654,14 +653,15 @@
         delta: float = 0.25,
         batch_size: Optional[int] = None,
         all_stats: bool = True,
         batch_correction: bool = False,
         batchid1: Optional[Iterable[str]] = None,
         batchid2: Optional[Iterable[str]] = None,
         fdr_target: float = 0.05,
+        silent: bool = False,
         protein_prior_count: float = 0.1,
         scale_protein: bool = False,
         sample_protein_mixing: bool = False,
         include_protein_background: bool = False,
         **kwargs,
     ) -> pd.DataFrame:
         r"""
@@ -716,14 +716,15 @@
             col_names,
             mode,
             batchid1,
             batchid2,
             delta,
             batch_correction,
             fdr_target,
+            silent,
             **kwargs,
         )
 
         return result
 
     @torch.no_grad()
     def posterior_predictive_sample(
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/_utils.py` & `scvi-tools-0.9.1/scvi/model/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_archesmixin.py` & `scvi-tools-0.9.1/scvi/model/base/_archesmixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 from typing import Optional, Union
 
 import torch
 from anndata import AnnData
 
-from scvi.compose import FCLayers
 from scvi.data import transfer_anndata_setup
 from scvi.model._utils import parse_use_gpu_arg
+from scvi.nn import FCLayers
 
 from ._base_model import BaseModelClass
 from ._utils import _initialize_model, _load_saved_files, _validate_var_names
 
 logger = logging.getLogger(__name__)
 
 
 class ArchesMixin:
+    """Universal scArches implementation."""
+
     @classmethod
     def load_query_data(
         cls,
         adata: AnnData,
         reference_model: Union[str, BaseModelClass],
         inplace_subset_query_vars: bool = False,
         use_gpu: Optional[Union[str, int, bool]] = None,
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_base_model.py` & `scvi-tools-0.9.1/scvi/model/base/_base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 import pyro
 import rich
 import torch
 from anndata import AnnData
 from rich.text import Text
 
 from scvi import _CONSTANTS, settings
-from scvi.compose import PyroBaseModuleClass
 from scvi.data import get_from_registry, transfer_anndata_setup
 from scvi.data._anndata import _check_anndata_setup_equivalence
 from scvi.data._utils import _check_nonnegative_integers
 from scvi.dataloaders import AnnDataLoader
 from scvi.model._utils import parse_use_gpu_arg
+from scvi.module.base import PyroBaseModuleClass
 
 from ._utils import _initialize_model, _load_saved_files, _validate_var_names
 
 logger = logging.getLogger(__name__)
 
 
 class BaseModelClass(ABC):
+    """Abstract class for scvi-tools models."""
+
     def __init__(self, adata: Optional[AnnData] = None):
         if adata is not None:
             if "_scvi" not in adata.uns.keys():
                 raise ValueError(
                     "Please setup your AnnData with scvi.data.setup_anndata(adata) first"
                 )
             self.adata = adata
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_log_likelihood.py` & `scvi-tools-0.9.1/scvi/model/base/_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_rnamixin.py` & `scvi-tools-0.9.1/scvi/model/base/_rnamixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 logger = logging.getLogger(__name__)
 
 Number = Union[int, float]
 
 
 class RNASeqMixin:
+    """General purpose methods for RNA-seq analysis."""
+
     @torch.no_grad()
     def get_normalized_expression(
         self,
         adata: Optional[AnnData] = None,
         indices: Optional[Sequence[int]] = None,
         transform_batch: Optional[Sequence[Union[Number, str]]] = None,
         gene_list: Optional[Sequence[str]] = None,
@@ -165,14 +167,15 @@
         delta: float = 0.25,
         batch_size: Optional[int] = None,
         all_stats: bool = True,
         batch_correction: bool = False,
         batchid1: Optional[Iterable[str]] = None,
         batchid2: Optional[Iterable[str]] = None,
         fdr_target: float = 0.05,
+        silent: bool = False,
         **kwargs,
     ) -> pd.DataFrame:
         r"""
         A unified method for differential expression analysis.
 
         Implements `"vanilla"` DE [Lopez18]_ and `"change"` mode DE [Boyeau19]_.
 
@@ -208,14 +211,15 @@
             col_names,
             mode,
             batchid1,
             batchid2,
             delta,
             batch_correction,
             fdr_target,
+            silent,
             **kwargs,
         )
 
         return result
 
     @torch.no_grad()
     def posterior_predictive_sample(
@@ -474,17 +478,20 @@
                 compute_loss=False,
             )
             px_r = generative_outputs["px_r"]
             px_rate = generative_outputs["px_rate"]
             px_dropout = generative_outputs["px_dropout"]
 
             n_batch = px_rate.size(0) if n_samples == 1 else px_rate.size(1)
-            dispersion_list += [
-                np.repeat(np.array(px_r.cpu())[np.newaxis, :], n_batch, axis=0)
-            ]
+
+            px_r = np.array(px_r.cpu())
+            if len(px_r.shape) == 1:
+                dispersion_list += [np.repeat(px_r[np.newaxis, :], n_batch, axis=0)]
+            else:
+                dispersion_list += [px_r]
             mean_list += [np.array(px_rate.cpu())]
             dropout_list += [np.array(px_dropout.cpu())]
 
         dropout = np.concatenate(dropout_list)
         means = np.concatenate(mean_list)
         dispersions = np.concatenate(dispersion_list)
         if give_mean and n_samples > 1:
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_training_mixin.py` & `scvi-tools-0.9.1/scvi/model/base/_training_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Optional, Union
 
 import numpy as np
 
 from scvi.dataloaders import DataSplitter
-from scvi.lightning import TrainingPlan
-
-from ._trainrunner import TrainRunner
+from scvi.train import TrainingPlan, TrainRunner
 
 
 class UnsupervisedTrainingMixin:
+    """General purpose unsupervised train method."""
+
     def train(
         self,
         max_epochs: Optional[int] = None,
         use_gpu: Optional[Union[str, int, bool]] = None,
         train_size: float = 0.9,
         validation_size: Optional[float] = None,
         batch_size: int = 128,
+        early_stopping: bool = False,
         plan_kwargs: Optional[dict] = None,
         **trainer_kwargs,
     ):
         """
         Train the model.
 
         Parameters
@@ -33,19 +34,22 @@
         train_size
             Size of training set in the range [0.0, 1.0].
         validation_size
             Size of the test set. If `None`, defaults to 1 - `train_size`. If
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         batch_size
             Minibatch size to use during training.
+        early_stopping
+            Perform early stopping. Additional arguments can be passed in `**kwargs`.
+            See :class:`~scvi.train.Trainer` for further options.
         plan_kwargs
-            Keyword args for :class:`~scvi.lightning.TrainingPlan`. Keyword arguments passed to
+            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
-            Other keyword args for :class:`~scvi.lightning.Trainer`.
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
             n_cells = self.adata.n_obs
             max_epochs = np.min([round((20000 / n_cells) * 400), 400])
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else dict()
 
@@ -55,14 +59,19 @@
             validation_size=validation_size,
             batch_size=batch_size,
             use_gpu=use_gpu,
         )
         training_plan = TrainingPlan(
             self.module, len(data_splitter.train_idx), **plan_kwargs
         )
+
+        es = "early_stopping"
+        trainer_kwargs[es] = (
+            early_stopping if es not in trainer_kwargs.keys() else trainer_kwargs[es]
+        )
         runner = TrainRunner(
             self,
             training_plan=training_plan,
             data_splitter=data_splitter,
             max_epochs=max_epochs,
             use_gpu=use_gpu,
             **trainer_kwargs,
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_trainrunner.py` & `scvi-tools-0.9.1/scvi/train/_trainrunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from typing import Optional, Union
 
 import pytorch_lightning as pl
 
 from scvi.dataloaders import DataSplitter, SemiSupervisedDataSplitter
-from scvi.lightning import Trainer
 from scvi.model._utils import parse_use_gpu_arg
 from scvi.model.base import BaseModelClass
+from scvi.train import Trainer
 
 logger = logging.getLogger(__name__)
 
 
 class TrainRunner:
     """
     TrainRunner calls Trainer.fit() and handles pre and post training procedures.
@@ -26,15 +26,15 @@
         :class:`~scvi.dataloaders.DataSplitter`
     max_epochs
         max_epochs to train for
     use_gpu
         Use default GPU if available (if None or True), or index of GPU to use (if int),
         or name of GPU (if str), or use CPU (if False).
     trainer_kwargs
-        Extra kwargs for :class:`~scvi.lightning.Trainer`
+        Extra kwargs for :class:`~scvi.train.Trainer`
 
     Examples
     --------
     >>> # Following code should be within a subclass of BaseModelClass
     >>> data_splitter = DataSplitter(self.adata)
     >>> training_plan = TrainingPlan(self.module, len(data_splitter.train_idx))
     >>> runner = TrainRunner(
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_utils.py` & `scvi-tools-0.9.1/scvi/model/base/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         # expand out kwargs
         kwargs = {k: v for (i, j) in kwargs.items() for (k, v) in j.items()}
     else:
         # grab all the parameters execept for kwargs (is a dict)
         non_kwargs = {k: v for k, v in init_params.items() if not isinstance(v, dict)}
         kwargs = {k: v for k, v in init_params.items() if isinstance(v, dict)}
         kwargs = {k: v for (i, j) in kwargs.items() for (k, v) in j.items()}
+        non_kwargs.pop("use_cuda")
 
     model = cls(adata, **non_kwargs, **kwargs)
     return model
 
 
 def _validate_var_names(adata, source_var_names):
 
@@ -97,14 +98,15 @@
     col_names,
     mode,
     batchid1,
     batchid2,
     delta,
     batch_correction,
     fdr,
+    silent,
     **kwargs
 ):
     """Internal function for DE interface."""
     if group1 is None and idx1 is None:
         group1 = adata.obs[groupby].astype("category").cat.categories.tolist()
         if len(group1) == 1:
             raise ValueError(
@@ -131,14 +133,15 @@
         group1 = [g1_key]
 
     df_results = []
     dc = DifferentialComputation(model_fn, adata)
     for g1 in track(
         group1,
         description="DE...",
+        disable=silent,
     ):
         cell_idx1 = (adata.obs[groupby] == g1).to_numpy().ravel()
         if group2 is None:
             cell_idx2 = ~cell_idx1
         else:
             cell_idx2 = (adata.obs[groupby] == group2).to_numpy().ravel()
```

### Comparing `scvi-tools-0.9.0b1/scvi/model/base/_vaemixin.py` & `scvi-tools-0.9.1/scvi/model/base/_vaemixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from ._log_likelihood import compute_elbo, compute_reconstruction_error
 
 logger = logging.getLogger(__name__)
 
 
 class VAEMixin:
+    """Univseral VAE methods."""
+
     @torch.no_grad()
     def get_elbo(
         self,
         adata: Optional[AnnData] = None,
         indices: Optional[Sequence[int]] = None,
         batch_size: Optional[int] = None,
     ) -> float:
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_autozivae.py` & `scvi-tools-0.9.1/scvi/module/_autozivae.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import torch
 import torch.nn.functional as F
 from scipy.special import logit
 from torch.distributions import Beta, Gamma, Normal
 from torch.distributions import kl_divergence as kl
 
 from scvi import _CONSTANTS
-from scvi.compose import LossRecorder, auto_move_data, one_hot
 from scvi.distributions import NegativeBinomial, ZeroInflatedNegativeBinomial
+from scvi.module.base import LossRecorder, auto_move_data
+from scvi.nn import one_hot
 
 from ._vae import VAE
 
 torch.backends.cudnn.benchmark = True
 
 
 class AutoZIVAE(VAE):
@@ -391,16 +392,16 @@
 
         # Reconstruction loss
         reconst_loss = self.get_reconstruction_loss(
             x, px_rate, px_r, px_dropout, bernoulli_params
         )
 
         kl_global = kl_divergence_bernoulli
-        kl_local_for_warmup = kl_divergence_l
-        kl_local_no_warmup = kl_divergence_z
+        kl_local_for_warmup = kl_divergence_z
+        kl_local_no_warmup = kl_divergence_l
 
         weighted_kl_local = kl_weight * kl_local_for_warmup + kl_local_no_warmup
         loss = n_obs * torch.mean(reconst_loss + weighted_kl_local) + kl_global
         kl_local = dict(
             kl_divergence_l=kl_divergence_l, kl_divergence_z=kl_divergence_z
         )
         return LossRecorder(loss, reconst_loss, kl_local, kl_global)
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_classifier.py` & `scvi-tools-0.9.1/scvi/module/_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch import nn as nn
 
-from scvi.compose import FCLayers
+from scvi.nn import FCLayers
 
 
 class Classifier(nn.Module):
     """
     Basic fully-connected NN classifier.
 
     Parameters
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_peakvae.py` & `scvi-tools-0.9.1/scvi/module/_peakvae.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 
 import numpy as np
 import torch
 from torch.distributions import Normal, kl_divergence
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import (
-    BaseModuleClass,
-    Encoder,
-    FCLayers,
-    LossRecorder,
-    auto_move_data,
-)
+from scvi.module.base import BaseModuleClass, LossRecorder, auto_move_data
+from scvi.nn import Encoder, FCLayers
 
 
 class Decoder(torch.nn.Module):
     """
     Decodes data from latent space of ``n_input`` dimensions ``n_output``dimensions.
 
     Uses a fully-connected neural network of ``n_hidden`` layers.
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_scanvae.py` & `scvi-tools-0.9.1/scvi/module/_scanvae.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import torch
 from torch.distributions import Categorical, Normal
 from torch.distributions import kl_divergence as kl
 from torch.nn import functional as F
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import Decoder, Encoder, LossRecorder, auto_move_data
+from scvi.module.base import LossRecorder, auto_move_data
+from scvi.nn import Decoder, Encoder
 
 from ._classifier import Classifier
 from ._utils import broadcast_labels
 from ._vae import VAE
 
 
 class SCANVAE(VAE):
     """
     Single-cell annotation using variational inference.
 
-    This is an implementation of the scANVI model described in [Xu20]_,
+    This is an implementation of the scANVI model described in [Xu21]_,
     inspired from M1 + M2 model, as described in (https://arxiv.org/pdf/1406.5298.pdf).
 
     Parameters
     ----------
     n_input
         Number of input genes
     n_batch
@@ -63,15 +64,15 @@
     use_labels_groups
         Whether to use the label groups
     use_batch_norm
         Whether to use batch norm in layers
     use_layer_norm
         Whether to use layer norm in layers
     **kwargs
-        Keyword args for :class:`~scvi.modules.VAE`
+        Keyword args for :class:`~scvi.module.VAE`
     """
 
     def __init__(
         self,
         n_input: int,
         n_batch: int = 0,
         n_labels: int = 0,
@@ -206,16 +207,15 @@
 
     @auto_move_data
     def classification_loss(self, labelled_dataset):
         x = labelled_dataset[_CONSTANTS.X_KEY]
         y = labelled_dataset[_CONSTANTS.LABELS_KEY]
         batch_idx = labelled_dataset[_CONSTANTS.BATCH_KEY]
         classification_loss = F.cross_entropy(
-            self.classify(x, batch_idx),
-            y.view(-1).long(),
+            self.classify(x, batch_idx), y.view(-1).long()
         )
         return classification_loss
 
     def loss(
         self,
         tensors,
         inference_outputs,
@@ -270,18 +270,30 @@
         if is_labelled:
             loss = reconst_loss + loss_z1_weight + loss_z1_unweight
             kl_locals = {
                 "kl_divergence_z2": kl_divergence_z2,
                 "kl_divergence_l": kl_divergence_l,
             }
             if labelled_tensors is not None:
-                loss += (
-                    self.classification_loss(labelled_tensors) * classification_ratio
+                classifier_loss = self.classification_loss(labelled_tensors)
+                loss += classifier_loss * classification_ratio
+                return LossRecorder(
+                    loss,
+                    reconst_loss,
+                    kl_locals,
+                    kl_global=0.0,
+                    classification_loss=classifier_loss,
+                    n_labelled_tensors=labelled_tensors[_CONSTANTS.X_KEY].shape[0],
                 )
-            return LossRecorder(loss, reconst_loss, kl_locals, kl_global=0.0)
+            return LossRecorder(
+                loss,
+                reconst_loss,
+                kl_locals,
+                kl_global=0.0,
+            )
 
         probs = self.classifier(z1)
         reconst_loss += loss_z1_weight + (
             (loss_z1_unweight).view(self.n_labels, -1).t() * probs
         ).sum(dim=1)
 
         kl_divergence = (kl_divergence_z2.view(self.n_labels, -1).t() * probs).sum(
@@ -292,9 +304,18 @@
             Categorical(probs=self.y_prior.repeat(probs.size(0), 1)),
         )
         kl_divergence += kl_divergence_l
 
         loss = torch.mean(reconst_loss + kl_divergence * kl_weight)
 
         if labelled_tensors is not None:
-            loss += self.classification_loss(labelled_tensors) * classification_ratio
+            classifier_loss = self.classification_loss(labelled_tensors)
+            loss += classifier_loss * classification_ratio
+            return LossRecorder(
+                loss,
+                reconst_loss,
+                kl_divergence,
+                kl_global=0.0,
+                classification_loss=classifier_loss,
+                n_labelled_tensors=labelled_tensors[_CONSTANTS.X_KEY].shape[0],
+            )
         return LossRecorder(loss, reconst_loss, kl_divergence, kl_global=0.0)
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_totalvae.py` & `scvi-tools-0.9.1/scvi/module/_totalvae.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,37 +6,31 @@
 import torch
 import torch.nn.functional as F
 from torch.distributions import Normal
 from torch.distributions import kl_divergence as kl
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import (
-    BaseModuleClass,
-    DecoderTOTALVI,
-    EncoderTOTALVI,
-    LossRecorder,
-    auto_move_data,
-    one_hot,
-)
 from scvi.distributions import (
     NegativeBinomial,
     NegativeBinomialMixture,
     ZeroInflatedNegativeBinomial,
 )
+from scvi.module.base import BaseModuleClass, LossRecorder, auto_move_data
+from scvi.nn import DecoderTOTALVI, EncoderTOTALVI, one_hot
 
 torch.backends.cudnn.benchmark = True
 
 
 # VAE model
 class TOTALVAE(BaseModuleClass):
     """
     Total variational inference for CITE-seq data.
 
-    Implements the totalVI model of [GayosoSteier20]_.
+    Implements the totalVI model of [GayosoSteier21]_.
 
     Parameters
     ----------
     n_input_genes
         Number of input genes
     n_input_proteins
         Number of input proteins
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_utils.py` & `scvi-tools-0.9.1/scvi/module/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from scvi.compose import one_hot
+from scvi.nn import one_hot
 
 
 def iterate(obj, func):
     t = type(obj)
     if t is list or t is tuple:
         return t([iterate(o, func) for o in obj])
     else:
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_vae.py` & `scvi-tools-0.9.1/scvi/module/_vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 import torch.nn.functional as F
 from torch import logsumexp
 from torch.distributions import Normal, Poisson
 from torch.distributions import kl_divergence as kl
 
 from scvi import _CONSTANTS
 from scvi._compat import Literal
-from scvi.compose import (
-    BaseModuleClass,
-    DecoderSCVI,
-    Encoder,
-    LinearDecoderSCVI,
-    LossRecorder,
-    auto_move_data,
-    one_hot,
-)
 from scvi.distributions import NegativeBinomial, ZeroInflatedNegativeBinomial
+from scvi.module.base import BaseModuleClass, LossRecorder, auto_move_data
+from scvi.nn import DecoderSCVI, Encoder, LinearDecoderSCVI, one_hot
 
 torch.backends.cudnn.benchmark = True
 
 
 # VAE model
 class VAE(BaseModuleClass):
     """
@@ -322,16 +315,16 @@
                 Normal(local_l_mean, torch.sqrt(local_l_var)),
             ).sum(dim=1)
         else:
             kl_divergence_l = 0.0
 
         reconst_loss = self.get_reconstruction_loss(x, px_rate, px_r, px_dropout)
 
-        kl_local_for_warmup = kl_divergence_l
-        kl_local_no_warmup = kl_divergence_z
+        kl_local_for_warmup = kl_divergence_z
+        kl_local_no_warmup = kl_divergence_l
 
         weighted_kl_local = kl_weight * kl_local_for_warmup + kl_local_no_warmup
 
         loss = torch.mean(reconst_loss + weighted_kl_local)
 
         kl_local = dict(
             kl_divergence_l=kl_divergence_l, kl_divergence_z=kl_divergence_z
```

### Comparing `scvi-tools-0.9.0b1/scvi/modules/_vaec.py` & `scvi-tools-0.9.1/scvi/module/_vaec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from torch.distributions import Categorical, Normal
 from torch.distributions import kl_divergence as kl
 
-from scvi.compose import DecoderSCVI, Encoder
-from scvi.modules import Classifier
-from scvi.modules._utils import broadcast_labels
+from scvi.module import Classifier
+from scvi.module._utils import broadcast_labels
+from scvi.nn import DecoderSCVI, Encoder
 
 from ._vae import VAE
 
 
 class VAEC(VAE):
     r"""
     A semi-supervised Variational auto-encoder model - inspired from M2 model.
```

### Comparing `scvi-tools-0.9.0b1/scvi/utils/_differential.py` & `scvi-tools-0.9.1/scvi/utils/_differential.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class DifferentialComputation:
     """
     Unified class for differential computation.
 
     This class takes a function from a model like `SCVI` or `TOTALVI` and takes outputs
     from this function with respect to the adata input and computed Bayes factors as
-    described in [Lopez18]_, [Xu20]_, or [Boyeau19]_.
+    described in [Lopez18]_, [Xu21]_, or [Boyeau19]_.
 
     Parameters
     ----------
     model_fn
         Function in model API to get values from.
     adata
         AnnData setup with scvi
@@ -51,15 +51,15 @@
         cred_interval_lvls: Optional[Union[List[float], np.ndarray]] = None,
     ) -> Dict[str, np.ndarray]:
         r"""
         A unified method for differential expression inference.
 
         Two modes coexist:
 
-        - the `"vanilla"` mode follows protocol described in [Lopez18]_ and [Xu20]_
+        - the `"vanilla"` mode follows protocol described in [Lopez18]_ and [Xu21]_
         In this case, we perform hypothesis testing based on the hypotheses
 
         .. math::
             M_1: h_1 > h_2 ~\text{and}~ M_2: h_1 \leq h_2.
 
         DE can then be based on the study of the Bayes factors
```

### Comparing `scvi-tools-0.9.0b1/scvi/utils/_track.py` & `scvi-tools-0.9.1/scvi/utils/_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,11 +49,11 @@
         # fixes repeated pbar in jupyter
         # see https://github.com/tqdm/tqdm/issues/375
         if hasattr(tqdm_base, "_instances"):
             for instance in list(tqdm_base._instances):
                 tqdm_base._decr_instances(instance)
         return tqdm_base(sequence, desc=description, file=sys.stdout, **kwargs)
     else:
-        in_colab = "google.colab" in sys.modules
+        in_colab = "google.colab" in sys.module
         force_jupyter = None if not in_colab else True
         console = Console(force_jupyter=force_jupyter)
         return track_base(sequence, description=description, console=console, **kwargs)
```

### Comparing `scvi-tools-0.9.0b1/setup.py` & `scvi-tools-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['scvi',
- 'scvi.compose',
  'scvi.data',
  'scvi.data._built_in_data',
  'scvi.dataloaders',
  'scvi.distributions',
  'scvi.external',
+ 'scvi.external.cellassign',
  'scvi.external.gimvi',
  'scvi.external.solo',
  'scvi.external.stereoscope',
- 'scvi.lightning',
  'scvi.model',
  'scvi.model.base',
- 'scvi.modules',
+ 'scvi.module',
+ 'scvi.module.base',
+ 'scvi.nn',
+ 'scvi.train',
  'scvi.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['anndata>=0.7.5',
  'h5py>=2.9.0',
  'ipywidgets',
  'numba>=0.41.0',
  'numpy>=1.17.0',
  'openpyxl>=3.0',
  'pandas>=1.0',
- 'pyro-ppl>=1.1.0',
+ 'pyro-ppl>=1.5.0',
  'pytorch-lightning>=1.2',
  'rich>=9.1.0',
  'scikit-learn>=0.21.2',
  'torch>=1.7.1',
  'tqdm>=4.56.0']
 
 extras_require = \
@@ -46,41 +48,42 @@
          'jupyter>=1.0',
          'loompy>=3.0.6',
          'nbconvert>=5.4.0',
          'nbformat>=4.4.0',
          'pre-commit>=2.7.1',
          'pytest>=4.4',
          'scanpy>=1.6'],
- 'docs': ['furo>=2020.12.30b24',
-          'nbsphinx',
+ 'docs': ['nbsphinx',
           'nbsphinx-link',
+          'pydata-sphinx-theme>=0.4.3',
           'scanpydoc>=0.5',
           'sphinx>=3.4',
           'sphinx-autodoc-typehints',
           'sphinx-gallery>0.6',
+          'sphinx-tabs',
           'sphinx_copybutton'],
  'docs:python_version >= "3.7"': ['ipython>=7.20'],
  'tutorials': ['leidenalg',
                'loompy>=3.0.6',
                'python-igraph',
                'scanpy>=1.6',
                'scikit-misc>=0.1.3']}
 
 setup_kwargs = {
     'name': 'scvi-tools',
-    'version': '0.9.0b1',
-    'description': 'Deep generative models for end-to-end analysis of single-cell omics data.',
-    'long_description': '<img src="https://github.com/YosefLab/scvi-tools/blob/master/docs/_static/scvi-tools-horizontal.svg?raw=true" width="400" alt="scvi-tools">\n\n[![Stars](https://img.shields.io/github/stars/YosefLab/scvi-tools?logo=GitHub&color=yellow)](https://github.com/YosefLab/scvi-tools/stargazers)\n[![PyPI](https://img.shields.io/pypi/v/scvi-tools.svg)](https://pypi.org/project/scvi-tools)\n[![Documentation Status](https://readthedocs.org/projects/scvi/badge/?version=latest)](https://scvi.readthedocs.io/en/stable/?badge=stable)\n![Build\nStatus](https://github.com/YosefLab/scvi-tools/workflows/scvi-tools/badge.svg)\n[![Coverage](https://codecov.io/gh/YosefLab/scvi-tools/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/scvi-tools)\n[![Code\nStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![Downloads](https://pepy.tech/badge/scvi-tools)](https://pepy.tech/project/scvi-tools)\n[![Join the chat at https://gitter.im/scvi-tools/development](https://badges.gitter.im/scvi-tools/development.svg)](https://gitter.im/scvi-tools/development?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n\n[scvi-tools](https://scvi-tools.org/) (single-cell variational inference\ntools) is a package for probabilistic modeling of single-cell omics\ndata, built on top of [PyTorch](https://pytorch.org) and\n[Anndata](https://anndata.readthedocs.io/en/latest/).\n\n# Available implementations of single-cell omics models\n\nscvi-tools contains scalable implementations of several models that\nfacilitate a broad number of tasks across many omics, including:\n\n-   [scVI](https://rdcu.be/bdHYQ) for analysis of single-cell RNA-seq\n    data, as well as its improved differential expression\n    [framework](https://www.biorxiv.org/content/biorxiv/early/2019/10/04/794289.full.pdf).\n-   [scANVI](https://www.biorxiv.org/content/biorxiv/early/2019/01/29/532895.full.pdf)\n    for cell annotation of scRNA-seq data using semi-labeled examples.\n-   [totalVI](https://www.biorxiv.org/content/10.1101/2020.05.08.083337v1.full.pdf)\n    for analysis of CITE-seq data.\n-   [gimVI](https://arxiv.org/pdf/1905.02269.pdf) for imputation of\n    missing genes in spatial transcriptomics from scRNA-seq data.\n-   [AutoZI](https://www.biorxiv.org/content/biorxiv/early/2019/10/10/794875.full.pdf)\n    for assessing gene-specific levels of zero-inflation in scRNA-seq\n    data.\n-   [LDVAE](https://www.biorxiv.org/content/10.1101/737601v1.full.pdf)\n    for an interpretable linear factor model version of scVI.\n-   [Stereoscope](https://www.nature.com/articles/s42003-020-01247-y)\n    for deconvolution of spatial transcriptomics data.\n-   peakVI for analysis of ATAC-seq data.\n-   [scArches](https://www.biorxiv.org/content/10.1101/2020.07.16.205997v1)\n    for transfer learning from one single-cell atlas to a query dataset\n    (currently supports scVI, scANVI and TotalVI).\n\nAll these implementations have a high-level API that interacts with\n[scanpy](http://scanpy.readthedocs.io/), standard save/load functions,\nand support GPU acceleration.\n\n# Fast prototyping of novel probabilistic models\n\nscvi-tools contains the building blocks to prototype novel probablistic\nmodels. These building blocks are powered by popular probabilistic and\nmachine learning frameworks such as [PyTorch\nlightning](https://www.pytorchlightning.ai/), and\n[Pyro](https://pyro.ai/).\n\nWe recommend checking out the [skeleton\nrepository](https://github.com/YosefLab/scvi-tools-skeleton), as a\nstarting point for developing new models into scvi-tools.\n\n# Resources\n\n-   Tutorials, API reference, and installation guides are available in\n    the [documentation](https://docs.scvi-tools.org/).\n-   For discussion of usage, checkout out our\n    [forum](https://discourse.scvi-tools.org).\n-   Please use the issues here to submit bug reports.\n-   If you\\\'d like to contribute, check out our [development\n    guide](https://docs.scvi-tools.org/en/stable/development.html).\n-   If you find a model useful for your research, please consider citing\n    the corresponding publication (linked above).\n',
+    'version': '0.9.1',
+    'description': 'Deep probabilistic analysis of single-cell omics data.',
+    'long_description': '<img src="https://github.com/YosefLab/scvi-tools/blob/master/docs/_static/scvi-tools-horizontal.svg?raw=true" width="400" alt="scvi-tools">\n\n[![Stars](https://img.shields.io/github/stars/YosefLab/scvi-tools?logo=GitHub&color=yellow)](https://github.com/YosefLab/scvi-tools/stargazers)\n[![PyPI](https://img.shields.io/pypi/v/scvi-tools.svg)](https://pypi.org/project/scvi-tools)\n[![Documentation Status](https://readthedocs.org/projects/scvi/badge/?version=latest)](https://scvi.readthedocs.io/en/stable/?badge=stable)\n![Build\nStatus](https://github.com/YosefLab/scvi-tools/workflows/scvi-tools/badge.svg)\n[![Coverage](https://codecov.io/gh/YosefLab/scvi-tools/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/scvi-tools)\n[![Code\nStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![Downloads](https://pepy.tech/badge/scvi-tools)](https://pepy.tech/project/scvi-tools)\n[![Join the chat at https://gitter.im/scvi-tools/development](https://badges.gitter.im/scvi-tools/development.svg)](https://gitter.im/scvi-tools/development?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n\n[scvi-tools](https://scvi-tools.org/) (single-cell variational inference\ntools) is a package for probabilistic modeling of single-cell omics\ndata, built on top of [PyTorch](https://pytorch.org) and\n[AnnData](https://anndata.readthedocs.io/en/latest/).\n\n# Available implementations of single-cell omics models\n\nscvi-tools contains scalable implementations of several models that\nfacilitate a broad number of tasks across many omics, including:\n\n-   [scVI](https://rdcu.be/bdHYQ) for analysis of single-cell RNA-seq\n    data, as well as its improved differential expression\n    [framework](https://www.biorxiv.org/content/biorxiv/early/2019/10/04/794289.full.pdf).\n-   [scANVI](https://www.biorxiv.org/content/biorxiv/early/2019/01/29/532895.full.pdf)\n    for cell annotation of scRNA-seq data using semi-labeled examples.\n-   [totalVI](https://www.biorxiv.org/content/10.1101/2020.05.08.083337v1.full.pdf)\n    for analysis of CITE-seq data.\n-   [gimVI](https://arxiv.org/pdf/1905.02269.pdf) for imputation of\n    missing genes in spatial transcriptomics from scRNA-seq data.\n-   [AutoZI](https://www.biorxiv.org/content/biorxiv/early/2019/10/10/794875.full.pdf)\n    for assessing gene-specific levels of zero-inflation in scRNA-seq\n    data.\n-   [LDVAE](https://www.biorxiv.org/content/10.1101/737601v1.full.pdf)\n    for an interpretable linear factor model version of scVI.\n-   [Stereoscope](https://www.nature.com/articles/s42003-020-01247-y)\n    for deconvolution of spatial transcriptomics data.\n-   peakVI for analysis of ATAC-seq data.\n-   [scArches](https://www.biorxiv.org/content/10.1101/2020.07.16.205997v1)\n    for transfer learning from one single-cell atlas to a query dataset\n    (currently supports scVI, scANVI and TotalVI).\n-   [CellAssign](https://www.nature.com/articles/s41592-019-0529-1) for\n    reference-based annotation of scRNA-seq data.\n-   [Solo](https://www.sciencedirect.com/science/article/pii/S2405471220301952) \n    for doublet detection in scRNA-seq data.\n\nAll these implementations have a high-level API that interacts with\n[scanpy](http://scanpy.readthedocs.io/), standard save/load functions,\nand support GPU acceleration.\n\n# Fast prototyping of novel probabilistic models\n\nscvi-tools contains the building blocks to prototype novel probablistic\nmodels. These building blocks are powered by popular probabilistic and\nmachine learning frameworks such as [PyTorch\nLightning](https://www.pytorchlightning.ai/), and\n[Pyro](https://pyro.ai/).\n\nWe recommend checking out the [skeleton\nrepository](https://github.com/YosefLab/scvi-tools-skeleton), as a\nstarting point for developing new models into scvi-tools.\n\n# Basic installation\n\nFor conda, \n```\nconda install scvi-tools -c bioconda -c conda-forge\n```\nand for pip,\n```\npip install scvi-tools\n```\nPlease be sure to install a version of [PyTorch](https://pytorch.org/) that is compatible with your GPU (if applicable).\n\n# Resources\n\n-   Tutorials, API reference, and installation guides are available in\n    the [documentation](https://docs.scvi-tools.org/).\n-   For discussion of usage, checkout out our\n    [forum](https://discourse.scvi-tools.org).\n-   Please use the issues here to submit bug reports.\n-   If you\\\'d like to contribute, check out our [contributing\n    guide](https://docs.scvi-tools.org/en/stable/contributing/index.html).\n-   If you find a model useful for your research, please consider citing\n    the corresponding publication (linked above).\n',
     'author': 'Romain Lopez',
     'author_email': 'romain_lopez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/YosefLab/scvi-tools',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `scvi-tools-0.9.0b1/PKG-INFO` & `scvi-tools-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: scvi-tools
-Version: 0.9.0b1
-Summary: Deep generative models for end-to-end analysis of single-cell omics data.
+Version: 0.9.1
+Summary: Deep probabilistic analysis of single-cell omics data.
 Home-page: https://github.com/YosefLab/scvi-tools
 License: BSD-3-Clause
 Author: Romain Lopez
 Author-email: romain_lopez@gmail.com
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tutorials
 Requires-Dist: anndata (>=0.7.5)
 Requires-Dist: black (>=20.8b1); extra == "dev"
 Requires-Dist: codecov (>=2.0.8); extra == "dev"
 Requires-Dist: flake8 (>=3.7.7); extra == "dev"
-Requires-Dist: furo (>=2020.12.30b24); extra == "docs"
 Requires-Dist: h5py (>=2.9.0)
 Requires-Dist: importlib-metadata (>=1.0,<2.0); python_version < "3.8"
 Requires-Dist: ipython (>=7.20); (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: ipywidgets
 Requires-Dist: isort (>=5.7); extra == "dev"
 Requires-Dist: jupyter (>=1.0); extra == "dev"
 Requires-Dist: leidenalg; extra == "tutorials"
@@ -41,26 +39,28 @@
 Requires-Dist: nbsphinx-link; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: numba (>=0.41.0)
 Requires-Dist: numpy (>=1.17.0)
 Requires-Dist: openpyxl (>=3.0)
 Requires-Dist: pandas (>=1.0)
 Requires-Dist: pre-commit (>=2.7.1); extra == "dev"
-Requires-Dist: pyro-ppl (>=1.1.0)
+Requires-Dist: pydata-sphinx-theme (>=0.4.3); extra == "docs"
+Requires-Dist: pyro-ppl (>=1.5.0)
 Requires-Dist: pytest (>=4.4); extra == "dev"
 Requires-Dist: python-igraph; extra == "tutorials"
 Requires-Dist: pytorch-lightning (>=1.2)
 Requires-Dist: rich (>=9.1.0)
 Requires-Dist: scanpy (>=1.6); extra == "dev" or extra == "tutorials"
 Requires-Dist: scanpydoc (>=0.5); extra == "docs"
 Requires-Dist: scikit-learn (>=0.21.2)
 Requires-Dist: scikit-misc (>=0.1.3); extra == "tutorials"
 Requires-Dist: sphinx (>=3.4); extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-gallery (>0.6); extra == "docs"
+Requires-Dist: sphinx-tabs; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
 Requires-Dist: torch (>=1.7.1)
 Requires-Dist: tqdm (>=4.56.0)
 Requires-Dist: typing_extensions; (python_version < "3.8") and (extra == "docs")
 Project-URL: Documentation, https://scvi-tools.org
 Description-Content-Type: text/markdown
 
@@ -76,15 +76,15 @@
 Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Downloads](https://pepy.tech/badge/scvi-tools)](https://pepy.tech/project/scvi-tools)
 [![Join the chat at https://gitter.im/scvi-tools/development](https://badges.gitter.im/scvi-tools/development.svg)](https://gitter.im/scvi-tools/development?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [scvi-tools](https://scvi-tools.org/) (single-cell variational inference
 tools) is a package for probabilistic modeling of single-cell omics
 data, built on top of [PyTorch](https://pytorch.org) and
-[Anndata](https://anndata.readthedocs.io/en/latest/).
+[AnnData](https://anndata.readthedocs.io/en/latest/).
 
 # Available implementations of single-cell omics models
 
 scvi-tools contains scalable implementations of several models that
 facilitate a broad number of tasks across many omics, including:
 
 -   [scVI](https://rdcu.be/bdHYQ) for analysis of single-cell RNA-seq
@@ -103,36 +103,52 @@
     for an interpretable linear factor model version of scVI.
 -   [Stereoscope](https://www.nature.com/articles/s42003-020-01247-y)
     for deconvolution of spatial transcriptomics data.
 -   peakVI for analysis of ATAC-seq data.
 -   [scArches](https://www.biorxiv.org/content/10.1101/2020.07.16.205997v1)
     for transfer learning from one single-cell atlas to a query dataset
     (currently supports scVI, scANVI and TotalVI).
+-   [CellAssign](https://www.nature.com/articles/s41592-019-0529-1) for
+    reference-based annotation of scRNA-seq data.
+-   [Solo](https://www.sciencedirect.com/science/article/pii/S2405471220301952) 
+    for doublet detection in scRNA-seq data.
 
 All these implementations have a high-level API that interacts with
 [scanpy](http://scanpy.readthedocs.io/), standard save/load functions,
 and support GPU acceleration.
 
 # Fast prototyping of novel probabilistic models
 
 scvi-tools contains the building blocks to prototype novel probablistic
 models. These building blocks are powered by popular probabilistic and
 machine learning frameworks such as [PyTorch
-lightning](https://www.pytorchlightning.ai/), and
+Lightning](https://www.pytorchlightning.ai/), and
 [Pyro](https://pyro.ai/).
 
 We recommend checking out the [skeleton
 repository](https://github.com/YosefLab/scvi-tools-skeleton), as a
 starting point for developing new models into scvi-tools.
 
+# Basic installation
+
+For conda, 
+```
+conda install scvi-tools -c bioconda -c conda-forge
+```
+and for pip,
+```
+pip install scvi-tools
+```
+Please be sure to install a version of [PyTorch](https://pytorch.org/) that is compatible with your GPU (if applicable).
+
 # Resources
 
 -   Tutorials, API reference, and installation guides are available in
     the [documentation](https://docs.scvi-tools.org/).
 -   For discussion of usage, checkout out our
     [forum](https://discourse.scvi-tools.org).
 -   Please use the issues here to submit bug reports.
--   If you\'d like to contribute, check out our [development
-    guide](https://docs.scvi-tools.org/en/stable/development.html).
+-   If you\'d like to contribute, check out our [contributing
+    guide](https://docs.scvi-tools.org/en/stable/contributing/index.html).
 -   If you find a model useful for your research, please consider citing
     the corresponding publication (linked above).
```

