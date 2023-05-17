# Comparing `tmp/torch4keras-0.0.7.tar.gz` & `tmp/torch4keras-0.0.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.0.7.tar", last modified: Fri May  5 14:04:39 2023, max compression
+gzip compressed data, was "dist/torch4keras-0.0.7.post2.tar", last modified: Wed May 17 03:08:54 2023, max compression
```

## Comparing `torch4keras-0.0.7.tar` & `torch4keras-0.0.7.post2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.916319 torch4keras-0.0.7/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     6453 2023-05-05 14:04:39.915318 torch4keras-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6199 2023-05-05 13:57:27.000000 torch4keras-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 14:04:39.916319 torch4keras-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-04-24 15:56:30.000000 torch4keras-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.896319 torch4keras-0.0.7/torch4keras/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:52:53.000000 torch4keras-0.0.7/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    42265 2023-04-24 15:56:30.000000 torch4keras-0.0.7/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    22581 2023-05-03 05:20:41.000000 torch4keras-0.0.7/torch4keras/model.py
--rw-rw-rw-   0        0        0     8167 2023-04-24 15:56:30.000000 torch4keras-0.0.7/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.914316 torch4keras-0.0.7/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     6453 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/top_level.txt
+drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/
+-rw-r--r--   0 lb         (501) staff       (20)     7400 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/PKG-INFO
+drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras/
+-rw-r--r--   0 lb         (501) staff       (20)        0 2022-10-21 08:10:37.000000 torch4keras-0.0.7.post2/torch4keras/__init__.py
+-rw-r--r--   0 lb         (501) staff       (20)    22806 2023-05-17 01:26:05.000000 torch4keras-0.0.7.post2/torch4keras/model.py
+-rw-r--r--   0 lb         (501) staff       (20)    41281 2023-04-24 03:19:19.000000 torch4keras-0.0.7.post2/torch4keras/callbacks.py
+-rw-r--r--   0 lb         (501) staff       (20)     7956 2023-04-24 01:52:03.000000 torch4keras-0.0.7.post2/torch4keras/snippets.py
+-rw-r--r--   0 lb         (501) staff       (20)     6437 2023-05-17 02:57:10.000000 torch4keras-0.0.7.post2/README.md
+-rw-r--r--   0 lb         (501) staff       (20)      491 2023-05-17 03:08:52.000000 torch4keras-0.0.7.post2/setup.py
+-rw-r--r--   0 lb         (501) staff       (20)       38 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/setup.cfg
+drwxr-xr-x   0 lb         (501) staff       (20)        0 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/
+-rw-r--r--   0 lb         (501) staff       (20)     7400 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/PKG-INFO
+-rw-r--r--   0 lb         (501) staff       (20)      252 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/SOURCES.txt
+-rw-r--r--   0 lb         (501) staff       (20)       12 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/top_level.txt
+-rw-r--r--   0 lb         (501) staff       (20)        1 2023-05-17 03:08:54.000000 torch4keras-0.0.7.post2/torch4keras.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `torch4keras-0.0.7/PKG-INFO` & `torch4keras-0.0.7.post2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,88 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.7
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# torch4keras
-**Use torch like keras**
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本说明
-- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **v0.0.3.post2**：20221107 修复DDP下打印的bug
-- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **v0.0.1**：20221019 初始版本
-
-## 5. 更新：
-- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **20221019**：初版提交
+# torch4keras
+**Use torch like keras**
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+
+[Documentation](https://torch4keras.readthedocs.io) |
+[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+[Source code](https://github.com/Tongjilibo/torch4keras)
+
+## 1. 下载安装
+安装稳定版
+```shell
+pip install torch4keras
+```
+安装最新版
+```shell
+pip install git+https://github.com/Tongjilibo/torch4keras.git
+```
+
+## 2. 功能
+- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+- 训练：
+
+    ```text
+    2022-10-28 23:16:10 - Start Training
+    2022-10-28 23:16:10 - Epoch: 1/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+    test_acc: 0.98045. best_test_acc: 0.98045
+
+    2022-10-28 23:16:27 - Epoch: 2/5
+    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+    test_acc: 0.98280. best_test_acc: 0.98280
+
+    2022-10-28 23:16:44 - Epoch: 3/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+    test_acc: 0.98365. best_test_acc: 0.98365
+
+    2022-10-28 23:17:03 - Epoch: 4/5
+    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+    test_acc: 0.98265. best_test_acc: 0.98365
+
+    2022-10-28 23:17:21 - Epoch: 5/5
+    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+    test_acc: 0.98585. best_test_acc: 0.98585
+
+    2022-10-28 23:17:37 - Finish Training
+    ```
+
+## 3. 快速上手
+- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+
+## 4. 版本说明
+- **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **v0.0.3.post2**：20221107 修复DDP下打印的bug
+- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **v0.0.1**：20221019 初始版本
+
+## 5. 更新：
+- **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+- **20221019**：初版提交
```

### Comparing `torch4keras-0.0.7/README.md` & `torch4keras-0.0.7.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,98 @@
-# torch4keras
-**Use torch like keras**
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本说明
-- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **v0.0.3.post2**：20221107 修复DDP下打印的bug
-- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **v0.0.1**：20221019 初始版本
-
-## 5. 更新：
-- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **20221019**：初版提交
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.7.post2
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description: # torch4keras
+        **Use torch like keras**
+        
+        [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+        [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+        [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+        [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+        [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+        
+        [Documentation](https://torch4keras.readthedocs.io) |
+        [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+        [Source code](https://github.com/Tongjilibo/torch4keras)
+        
+        ## 1. 下载安装
+        安装稳定版
+        ```shell
+        pip install torch4keras
+        ```
+        安装最新版
+        ```shell
+        pip install git+https://github.com/Tongjilibo/torch4keras.git
+        ```
+        
+        ## 2. 功能
+        - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+        - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+        - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+        - 训练：
+        
+            ```text
+            2022-10-28 23:16:10 - Start Training
+            2022-10-28 23:16:10 - Epoch: 1/5
+            5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+            test_acc: 0.98045. best_test_acc: 0.98045
+        
+            2022-10-28 23:16:27 - Epoch: 2/5
+            5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+            test_acc: 0.98280. best_test_acc: 0.98280
+        
+            2022-10-28 23:16:44 - Epoch: 3/5
+            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+            test_acc: 0.98365. best_test_acc: 0.98365
+        
+            2022-10-28 23:17:03 - Epoch: 4/5
+            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+            test_acc: 0.98265. best_test_acc: 0.98365
+        
+            2022-10-28 23:17:21 - Epoch: 5/5
+            5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+            test_acc: 0.98585. best_test_acc: 0.98585
+        
+            2022-10-28 23:17:37 - Finish Training
+            ```
+        
+        ## 3. 快速上手
+        - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+        - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+        
+        ## 4. 版本说明
+        - **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+        - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+        - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+        - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+        - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+        - **v0.0.3.post2**：20221107 修复DDP下打印的bug
+        - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+        - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+        - **v0.0.1**：20221019 初始版本
+        
+        ## 5. 更新：
+        - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+        - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+        - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+        - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+        - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+        - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+        - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+        - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+        - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+        - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+        - **20221019**：初版提交
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `torch4keras-0.0.7/torch4keras/model.py` & `torch4keras-0.0.7.post2/torch4keras/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,473 +1,488 @@
-from torch import nn
-import torch
-from torch4keras.snippets import metric_mapping
-from torch4keras.callbacks import ProgbarLogger, Callback, CallbackList, BaseLogger, History, TqdmProgressBar
-from collections import OrderedDict
-from inspect import isfunction
-import os
-
-
-class Trainer:
-    """Trainer, 传入Module实例
-
-    :param module: None/nn.Module，nn.Module()的模型实例
-    """
-    def __init__(self, module=None):
-        super(Trainer, self).__init__()
-        self.initialize(module)
-    
-    def initialize(self, module=None):
-        # 这里主要是为了外面调用用到
-        self.global_step, self.local_step, self.total_steps, self.epoch, self.steps_per_epoch, self.train_dataloader = 0, 0, 0, 0, None, None
-        self.resume_step, self.resume_epoch = 0, 0
-        self.retain_graph = False  # loss.backward()是否保留计算图
-        self.callbacks = []
-        # 传入Module实例方式
-        if module is not None:
-            assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
-            self.module = module
-        # 是否运行Callbacks，目前主要是在DDP模式下运用
-        self.run_callbacks = True
-        # loss是否立即backward
-        self.loss_backward = True
-
-    def compile(self, loss, optimizer, scheduler=None, clip_grad_norm=None, mixed_precision=False, metrics=None, 
-                stateful_metrics=None, grad_accumulation_steps=1, **kwargs):
-        '''complile: 定义loss, optimizer, metrics等参数
-        
-        :param loss: loss
-        :param optimizer: 优化器
-        :param scheduler: scheduler
-        :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
-        :param mixed_precision: bool, 是否使用混合精度，默认为False
-        :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
-        :param stateful_metrics: List[str], 不滑动平均仅进行状态记录的metric，指标抖动会更加明显
-        :param grad_accumulation_steps: int, 梯度累积步数，默认为1
-        :param tqdmbar: bool, 是否使用tqdm进度条，从kwargs中解析，默认为False
-        :return: None
-        '''
-        self.criterion = loss
-        self.optimizer = optimizer
-        self.scheduler = scheduler
-        self.clip_grad_norm = clip_grad_norm
-        assert mixed_precision in {True, False, 'fp16', 'bf16'}
-        self.mixed_precision = 'fp16' if mixed_precision is True else mixed_precision
-        if self.mixed_precision:
-            self.autocast = torch.cuda.amp.autocast
-            self.scaler = torch.cuda.amp.GradScaler()
-
-        # 训练过程观测的指标
-        self.metrics = OrderedDict({'loss': None})
-        if metrics is None:
-            metrics = []
-        elif isinstance(metrics, (str, dict)) or isfunction(metrics):
-            metrics = [metrics]
-
-        for metric in metrics:
-            # 字符类型，目前仅支持accuracy
-            if isinstance(metric, str) and metric != 'loss':
-                self.metrics[metric] = None
-            # 字典形式 {metric: func}
-            elif isinstance(metric, dict):
-                self.metrics.update(metric)
-            # 函数形式，key和value都赋值metric
-            elif isfunction(metric):
-                self.metrics.update({metric: metric})
-            else:
-                raise ValueError('Args metrics only support `String, Dict, Callback, List[String, Dict, Callback]` format')
-        self.stateful_metrics = stateful_metrics
-
-        # 梯度累积
-        self.grad_accumulation_steps = grad_accumulation_steps
-
-        # 进度条参数
-        self.tqdmbar = kwargs.get('tqdmbar', False)
-    
-    def _forward(self, train_X):
-        # 如果传入了网络结构module，则调用module的forward
-        # 如果是继承方式，则调用自身的forward
-        if isinstance(train_X, torch.Tensor):  # tensor不展开
-            return self.get_module().forward(train_X)
-        elif isinstance(train_X, (tuple, list)):
-            return self.get_module().forward(*train_X)
-        elif isinstance(train_X, dict):
-            return self.get_module().forward(**train_X)
-        else:
-            return self.get_module().forward(train_X)
-
-    def train_step(self, train_X, train_y):
-        '''forward并返回loss
-
-        :param train_X: List[torch.Tensor], 训练数据
-        :param train_y: torch.Tensor/List[torch.Tensor], 标签信息
-        :return: [output, loss, loss_detail] output: torch.Tensor/List[torch.Tensor], 模型输出; loss: nn.Tensor, 计算得到的loss; loss_detail: dict[nn.Tensor], 具体的各个loss
-        '''
-        # 计算loss
-        if self.mixed_precision:
-            with self.autocast(dtype=torch.float16 if self.mixed_precision=='fp16' else torch.bfloat16):
-                output = self._forward(train_X)
-                loss_detail = self.criterion(output, train_y)
-        else:
-            output = self._forward(train_X)
-            loss_detail = self.criterion(output, train_y)
-
-        # 整理loss
-        if isinstance(loss_detail, torch.Tensor):
-            loss = loss_detail
-            loss_detail = {}
-        elif isinstance(loss_detail, dict):
-            loss = loss_detail['loss']  # 还存在其他loss，仅用于打印
-            del loss_detail['loss']
-        elif isinstance(loss_detail, (tuple, list)):
-            loss = loss_detail[0]
-            loss_detail = {f'loss{i}':v for i, v in enumerate(loss_detail[1:], start=1)}
-        else:
-            raise ValueError('Return loss only support `Tensor/dict/tuple/list` format')
-
-        # 梯度累积
-        loss = loss / self.grad_accumulation_steps if self.grad_accumulation_steps > 1 else loss
-
-        # loss.backward
-        if self.loss_backward:
-            self.scale_before_step = 0
-            if self.mixed_precision:  # 混合精度
-                self.scale_before_step = self.scaler.get_scale()
-                self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
-            else:
-                loss.backward(retain_graph=self.retain_graph)
-                
-        return output, loss, loss_detail
-
-    def fit(self, train_dataloader, steps_per_epoch=None, epochs=1, callbacks=None, verbose=1):
-        '''模型训练
-        
-        :param train_dataloader: Dataloader, 训练数据集
-        :param steps_per_epoch: int, 每个epoch训练的steps，默认为None表示自行计算 
-        :param epochs: int, 训练的轮次, 默认为1
-        :param callbacks: Callback/List[Callback], 回调函数，可调用预制的Callback或者自定义，默认为None 
-        :param verbose: int, 是否打印，默认为1表示打印
-        :return: None
-        '''
-        if not hasattr(train_dataloader, '__len__'):
-            assert steps_per_epoch is not None, 'Either train_dataloader has attr `__len__` or steps_per_epoch is not None'
-
-        self.steps_per_epoch = len(train_dataloader) if steps_per_epoch is None else steps_per_epoch
-        self.total_steps = self.steps_per_epoch * epochs
-        self.train_dataloader = train_dataloader  # 设置为成员变量，可由外部的callbacks进行修改
-        train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
-        verbose = self.verbose if hasattr(self, 'verbose') else verbose
-
-        # callbacks设置
-        if callbacks is None:
-            callbacks = []
-        elif isinstance(callbacks, Callback):
-            callbacks = [callbacks]
-        for callback in callbacks:
-            assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
-
-        history = History()
-        callbacks_ = [BaseLogger(self.stateful_metrics)]
-
-        # 进度条
-        if verbose:
-            if self.tqdmbar:
-                progbarlogger = TqdmProgressBar(stateful_metrics=self.stateful_metrics)
-            else:
-                progbarlogger = ProgbarLogger(stateful_metrics=self.stateful_metrics)
-            callbacks_.append(progbarlogger)
-        callbacks_  += callbacks + [history]
-        self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
-        callback_trainer = self
-        callback_model = self.get_module()
-        self.callbacks.set_trainer(callback_trainer)
-        self.callbacks.set_model(callback_model)
-        self.callbacks.set_optimizer(self.optimizer)
-        self.callbacks.set_params({
-            'epochs': epochs,
-            'steps': self.steps_per_epoch,
-            'verbose': verbose,
-            'metrics': [i for i in self.metrics.keys() if isinstance(i, str)],
-        })
-        logs = {}
-        self.callbacks.on_train_begin(logs)
-        callback_trainer.stop_training = False  # 在EarlyStopping中会重新设置
-
-        # epoch：当前epoch
-        # global_step：当前全局训练步数
-        # local_step: 当前epoch内的训练步数，不同epoch中相同local_step对应的batch数据不一定相同，在steps_per_epoch=None时相同
-        # bti：在dataloader中的index，不同epoch中相同的bti对应的batch数据一般相同，除非重新生成dataloader
-        self.bti = 0
-        for epoch in range(self.resume_epoch, epochs):
-            self.epoch = epoch
-            # resume_step：判断local_step的起点，以及进度条的起始位置
-            resume_step = self.resume_step if epoch==self.resume_epoch else 0
-            self.callbacks.on_epoch_begin(self.global_step, self.epoch)
-            if verbose:
-                progbarlogger.seen = resume_step  # 这里设置进度条的seen，在callbacks中也会修改
-            
-            for local_step in range(resume_step, self.steps_per_epoch):
-                self.local_step = local_step
-                self.global_step = self.epoch * self.steps_per_epoch + self.local_step
-                # 循环dataloader, 不要试用itertools的cycle，遇到过变量不释放的问题
-                try:
-                    batch = next(train_dataloader_iter)
-                except StopIteration:
-                    self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
-                    train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
-                    self.bti = 0
-                    batch = next(train_dataloader_iter)
-                self.train_X, self.train_y = batch
-
-                logs = self.get_batch_size()
-                self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
-
-                self.get_module().train()  # 设置为train模式
-
-                # 入参个数判断，如果入参>=3表示是多个入参，如果=2则表示是一个入参
-                self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
-                self.callbacks.on_train_step_end()
-                                
-                # 参数更新, 真实的参数更新次数要除以grad_accumulation_steps，注意调整总的训练步数
-                if (self.global_step+1) % self.grad_accumulation_steps == 0:
-                    skip_scheduler = False
-                    # 混合精度
-                    if self.mixed_precision:
-                        self.scaler.unscale_(self.optimizer)
-                        if self.clip_grad_norm is not None:  # 梯度裁剪
-                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
-                        self.scaler.step(self.optimizer)
-                        self.scaler.update()
-                        skip_scheduler = self.scaler.get_scale() != self.scale_before_step
-                    else:
-                        if self.clip_grad_norm is not None:  # 梯度裁剪
-                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
-                        self.optimizer.step()
-
-                    self.optimizer.zero_grad()  # 清梯度
-                    if (self.scheduler is not None) and not skip_scheduler:
-                        if isinstance(self.scheduler, (tuple, list)):
-                            for scheduler in self.scheduler:
-                                scheduler.step()
-                        else:
-                            self.scheduler.step()
-
-                # 添加loss至log打印
-                logs.update({'loss': self.loss.item()})
-                logs_loss_detail = {k: v.item() if isinstance(v, torch.Tensor) else v for k, v in self.loss_detail.items()}
-                logs.update(logs_loss_detail)
-                if verbose and (self.global_step == resume_step):
-                    progbarlogger.add_metrics(list(logs_loss_detail.keys()), add_position=1)
-                    
-                # 添加metrics至log打印
-                for metric, func in self.metrics.items():
-                    perf = metric_mapping(metric, func, self.output, self.train_y)  # 内置的一些accuracy指标
-                    if perf is not None:
-                        if isfunction(metric):  # 直接传入回调函数(无key)
-                            if verbose and (self.global_step == resume_step):
-                                progbarlogger.add_metrics(list(perf.keys()))
-                            logs.update(perf)
-                        elif isinstance(metric, str):  # 直接传入回调函数(有key)
-                            logs[metric] = perf
-
-                self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
-
-                self.bti += 1
-            self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
-            # TerminateOnNaN、EarlyStopping等停止训练策略
-            if callback_trainer.stop_training:
-                break
-        self.callbacks.on_train_end(logs)
-        return history
-
-    def get_batch_size(self):
-        '''获取batch_size，主要是用于callback中的BaseLogger和Callback
-        '''
-        # 从train_X中取batch_size，最多允许嵌套两层，即encoder和decoder的((token_ids1, mask1), (token_ids2, mask2))
-        if isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], (list, tuple)):
-            btz = self.train_X[0][0].size(0)
-        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], torch.Tensor):
-            btz = self.train_X[0].size(0)
-        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], dict):
-            btz = self.train_X[0].get('batch_size', 0)
-        elif isinstance(self.train_X, dict):
-            btz = self.train_X.get('batch_size', 0)
-        elif isinstance(self.train_X, torch.Tensor):
-            btz = self.train_X.size(0)
-        else:
-            raise ValueError('Input only support `[list, tuple, tensor]`')
-        return {'size': btz}
-
-    @torch.no_grad()
-    def predict(self, train_X, return_all=None):
-        '''模型预测，调用forward()
-
-        :param train_X: torch.Tensor, 预测用的数据集
-        :param return_all: None/int, 若返回为多个时候指定仅返回第几个，默认为None表示全部返回
-        :return: Any, 预测输出
-        '''
-        self.get_module().eval()
-        output = self._forward(train_X)
-        if return_all is None:
-            return output
-        elif isinstance(output, (tuple, list)) and isinstance(return_all, int) and return_all < len(output):
-            return output[return_all]
-        else:
-            raise ValueError('Return format error')
-
-    def load_steps_params(self, save_path):
-        '''导入训练过程参数
-        
-        :param save_path: str, 训练过程参数保存路径
-        '''
-        step_params = torch.load(save_path)
-        self.resume_step = step_params['resume_step'] 
-        self.resume_epoch = step_params['resume_epoch']
-        return step_params
-
-    def save_steps_params(self, save_path):
-        '''保存训练过程参数
-
-        :param save_path: str, 训练过程参数保存路径
-        '''
-        step_params = {'resume_step': (self.local_step+1) % self.steps_per_epoch, 
-                       'resume_epoch': self.epoch + (self.local_step+1) // self.steps_per_epoch}
-        torch.save(step_params, save_path)
-
-    def load_weights(self, load_path, strict=True, mapping={}):
-        '''加载模型权重, 支持加载权重文件list
-
-        :param save_path: str/tuple/list, 权重加载路径
-        :param strict: bool, torch.load()是否严格加载
-        :param mapping: dict, 指定key的映射
-        '''
-        state_dict_raw = {}
-        if isinstance(load_path, (tuple, list)):
-            strict = False  # 加载多个权重文件时候，strict设置为False
-        elif isinstance(load_path, str):
-            load_path = [load_path]
-        else:
-            raise ValueError('Args `load_path` only support str/tuple/list format')
-        
-        for load_path_i in load_path:
-            state_dict = torch.load(load_path_i, map_location='cpu')
-            for k, v in state_dict.items():
-                k = mapping.get(k, k)
-                state_dict_raw[k] = v
-            self.get_module().load_state_dict(state_dict_raw, strict=strict)
-
-    def save_weights(self, save_path, mapping={}, trainable_only=False, verbose=1):
-        '''保存模型权重
-
-        :param save_path: str, 权重保存路径
-        :param mapping: dict, 指定key的映射
-        :param trainable_only: bool, 指定仅保存可训练参数
-        '''
-        state_dict_raw = {}
-        state_dict = self.get_module().state_dict()
-        trainable_parameters = set(p for p,v in self.get_module().named_parameters() if v.requires_grad)
-        for k, v in state_dict.items():
-            # 只保存可训练的模型部分
-            if trainable_only and (k not in trainable_parameters):
-                continue
-            k = mapping.get(k, k)
-            state_dict_raw[k] = v
-        torch.save(state_dict_raw, save_path)
-        if trainable_only and (verbose > 0):
-            params_all = sum(p.numel() for p in self.get_module().parameters())
-            params_trainable = sum(p.numel() for p in self.get_module().parameters() if p.requires_grad)
-            print(f"[INFO] Only trainable parameters saved and occupy {params_trainable}/{params_all} {params_trainable/params_all:.2f}%")
-
-    def resume_from_checkpoint(self, model_path=None, optimizer_path=None, step_params_path=None):
-        '''同时加载模型、优化器、训练过程参数
-
-        :param model_path: str, 模型文件路径
-        :param optimizer_path: str, 优化器文件路径
-        :param step_params_path: str, 训练过程参数保存路径
-        '''
-        # 加载模型权重
-        if model_path:
-            self.load_weights(model_path)
-        # 加载优化器，断点续训使用
-        if optimizer_path:
-            state_dict = torch.load(optimizer_path, map_location='cpu')
-            self.optimizer.load_state_dict(state_dict)
-        # 加载训练进度参数，断点续训使用
-        self.load_steps_params(step_params_path)
-
-    def save_to_checkpoint(self, model_path=None, optimizer_path=None, step_params_path=None):
-        '''同时保存模型、优化器、训练过程参数
-
-        :param model_path: str, 模型文件路径
-        :param optimizer_path: str, 优化器文件路径
-        :param step_params_path: str, 训练过程参数保存路径
-        '''
-        if model_path:
-            save_dir = os.path.dirname(model_path)
-            os.makedirs(save_dir, exist_ok=True)
-            self.save_weights(model_path)
-        if optimizer_path:
-            save_dir = os.path.dirname(optimizer_path)
-            os.makedirs(save_dir, exist_ok=True)
-            torch.save(self.optimizer.state_dict(), optimizer_path)
-        if step_params_path:
-            save_dir = os.path.dirname(step_params_path)
-            os.makedirs(save_dir, exist_ok=True)
-            self.save_steps_params(step_params_path)
-
-    def get_module(self):
-        '''返回nn.Module模块
-        '''
-        if isinstance(self, nn.Module): return self
-        return self.module if hasattr(self, 'module') else self
-
-
-class BaseModel(Trainer, nn.Module):
-    """BaseModel, 使用继承的方式来使用
-    """
-    def __init__(self, *args, **kwargs):
-        nn.Module.__init__(self)
-        Trainer.__init__(self, *args, **kwargs)
-        
-
-class BaseModelDP(nn.DataParallel, BaseModel):
-    '''DataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
-    '''
-    def __init__(self, *args, **kwargs):
-        BaseModel.__init__(self)
-        nn.DataParallel.__init__(self, *args, **kwargs)
-
-
-class BaseModelDDP(nn.parallel.DistributedDataParallel, BaseModel):
-    '''DistributedDataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
-    '''
-    def __init__(self, *args, master_rank=0, **kwargs):
-        BaseModel.__init__(self)
-        nn.parallel.DistributedDataParallel.__init__(self, *args, **kwargs)
-
-        # 默认仅对master_rank=0打印信息
-        assert isinstance(master_rank, (int, list, tuple)), 'Args `master_rank` only supoorts int, list, tuple'
-        if isinstance(master_rank, int):
-            master_rank = [master_rank]
-        self.verbose = (torch.distributed.get_rank() in master_rank)
-
-
-TrainerDP = BaseModelDP
-TrainerDDP = BaseModelDDP
-
-
-def add_trainer(obj):
-    '''为对象添加Triner对应的方法
-    '''
-    if isinstance(obj, (Trainer, TrainerDP, TrainerDDP, BaseModel, BaseModelDP, BaseModelDDP)):
-        return obj
-    
-    if isinstance(obj, nn.Module):
-        import types
-        for k in dir(Trainer):
-            if k.startswith('__') and k.endswith('__'):
-                continue
-            elif (k == 'forward') and hasattr(obj, 'forward'):
-                continue
-            exec(f'obj.{k} = types.MethodType(Trainer.{k}, obj)')
-        obj.initialize()
+from torch import nn
+import torch
+from torch4keras.snippets import metric_mapping
+from torch4keras.callbacks import ProgbarLogger, Callback, CallbackList, BaseLogger, History, TqdmProgressBar
+from collections import OrderedDict
+from inspect import isfunction
+import os
+
+
+class Trainer:
+    """Trainer, 传入Module实例
+
+    :param module: None/nn.Module，nn.Module()的模型实例
+    """
+    def __init__(self, module=None):
+        super(Trainer, self).__init__()
+        self.initialize(module)
+    
+    def initialize(self, module=None):
+        # 这里主要是为了外面调用用到
+        self.global_step, self.local_step, self.total_steps, self.epoch, self.steps_per_epoch, self.train_dataloader = 0, 0, 0, 0, None, None
+        self.resume_step, self.resume_epoch = 0, 0
+        self.retain_graph = False  # loss.backward()是否保留计算图
+        self.callbacks = []
+        # 传入Module实例方式
+        if module is not None:
+            assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
+            self.module = module
+        # 是否运行Callbacks，目前主要是在DDP模式下运用
+        self.run_callbacks = True
+        # loss是否立即backward
+        self.loss_backward = True
+
+    def compile(self, loss, optimizer, scheduler=None, clip_grad_norm=None, mixed_precision=False, metrics=None, 
+                stateful_metrics=None, grad_accumulation_steps=1, **kwargs):
+        '''complile: 定义loss, optimizer, metrics等参数
+        
+        :param loss: loss
+        :param optimizer: 优化器
+        :param scheduler: scheduler
+        :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
+        :param mixed_precision: bool, 是否使用混合精度，默认为False
+        :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
+        :param stateful_metrics: List[str], 不滑动平均仅进行状态记录的metric，指标抖动会更加明显
+        :param grad_accumulation_steps: int, 梯度累积步数，默认为1
+        :param tqdmbar: bool, 是否使用tqdm进度条，从kwargs中解析，默认为False
+        :return: None
+        '''
+        self.criterion = loss
+        self.optimizer = optimizer
+        self.scheduler = scheduler
+        self.clip_grad_norm = clip_grad_norm
+        assert mixed_precision in {True, False, 'fp16', 'bf16'}
+        self.mixed_precision = 'fp16' if mixed_precision is True else mixed_precision
+        if self.mixed_precision:
+            self.autocast = torch.cuda.amp.autocast
+            self.scaler = torch.cuda.amp.GradScaler()
+
+        # 训练过程观测的指标
+        self.metrics = OrderedDict({'loss': None})
+        if metrics is None:
+            metrics = []
+        elif isinstance(metrics, (str, dict)) or isfunction(metrics):
+            metrics = [metrics]
+
+        for metric in metrics:
+            # 字符类型，目前仅支持accuracy
+            if isinstance(metric, str) and metric != 'loss':
+                self.metrics[metric] = None
+            # 字典形式 {metric: func}
+            elif isinstance(metric, dict):
+                self.metrics.update(metric)
+            # 函数形式，key和value都赋值metric
+            elif isfunction(metric):
+                self.metrics.update({metric: metric})
+            else:
+                raise ValueError('Args metrics only support `String, Dict, Callback, List[String, Dict, Callback]` format')
+        self.stateful_metrics = stateful_metrics
+
+        # 梯度累积
+        self.grad_accumulation_steps = grad_accumulation_steps
+
+        # 进度条参数
+        self.tqdmbar = kwargs.get('tqdmbar', False)
+    
+    def _forward(self, *inputs, **input_kwargs):
+        # 如果传入了网络结构module，则调用module的forward
+        # 如果是继承方式，则调用自身的forward
+        if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):
+            inputs = inputs[0]
+        if isinstance(inputs, torch.Tensor):  # tensor不展开
+            return self.get_module().forward(inputs, **input_kwargs)
+        elif isinstance(inputs, (tuple, list)):
+            return self.get_module().forward(*inputs, **input_kwargs)
+        else:
+            return self.get_module().forward(inputs, **input_kwargs)
+
+    def train_step(self, train_X, train_y):
+        '''forward并返回loss
+
+        :param train_X: List[torch.Tensor], 训练数据
+        :param train_y: torch.Tensor/List[torch.Tensor], 标签信息
+        :return: [output, loss, loss_detail] output: torch.Tensor/List[torch.Tensor], 模型输出; loss: nn.Tensor, 计算得到的loss; loss_detail: dict[nn.Tensor], 具体的各个loss
+        '''
+        # 计算loss
+        if self.mixed_precision:
+            with self.autocast(dtype=torch.float16 if self.mixed_precision=='fp16' else torch.bfloat16):
+                output = self._forward(train_X)
+                loss_detail = self.criterion(output, train_y)
+        else:
+            output = self._forward(train_X)
+            loss_detail = self.criterion(output, train_y)
+
+        # 整理loss
+        if isinstance(loss_detail, torch.Tensor):
+            loss = loss_detail
+            loss_detail = {}
+        elif isinstance(loss_detail, dict):
+            loss = loss_detail['loss']  # 还存在其他loss，仅用于打印
+            del loss_detail['loss']
+        elif isinstance(loss_detail, (tuple, list)):
+            loss = loss_detail[0]
+            loss_detail = {f'loss{i}':v for i, v in enumerate(loss_detail[1:], start=1)}
+        else:
+            raise ValueError('Return loss only support `Tensor/dict/tuple/list` format')
+
+        # 梯度累积
+        loss = loss / self.grad_accumulation_steps if self.grad_accumulation_steps > 1 else loss
+
+        # loss.backward
+        if self.loss_backward:
+            self.scale_before_step = 0
+            if self.mixed_precision:  # 混合精度
+                self.scale_before_step = self.scaler.get_scale()
+                self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
+            else:
+                loss.backward(retain_graph=self.retain_graph)
+                
+        return output, loss, loss_detail
+
+    def fit(self, train_dataloader, steps_per_epoch=None, epochs=1, callbacks=None, verbose=1):
+        '''模型训练
+        
+        :param train_dataloader: Dataloader, 训练数据集
+        :param steps_per_epoch: int, 每个epoch训练的steps，默认为None表示自行计算 
+        :param epochs: int, 训练的轮次, 默认为1
+        :param callbacks: Callback/List[Callback], 回调函数，可调用预制的Callback或者自定义，默认为None 
+        :param verbose: int, 是否打印，默认为1表示打印
+        :return: None
+        '''
+        if not hasattr(train_dataloader, '__len__'):
+            assert steps_per_epoch is not None, 'Either train_dataloader has attr `__len__` or steps_per_epoch is not None'
+
+        self.steps_per_epoch = len(train_dataloader) if steps_per_epoch is None else steps_per_epoch
+        self.total_steps = self.steps_per_epoch * epochs
+        self.train_dataloader = train_dataloader  # 设置为成员变量，可由外部的callbacks进行修改
+        train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
+        verbose = self.verbose if hasattr(self, 'verbose') else verbose
+
+        # callbacks设置
+        if callbacks is None:
+            callbacks = []
+        elif isinstance(callbacks, Callback):
+            callbacks = [callbacks]
+        for callback in callbacks:
+            assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
+
+        history = History()
+        callbacks_ = [BaseLogger(self.stateful_metrics)]
+
+        # 进度条
+        if verbose:
+            if self.tqdmbar:
+                progbarlogger = TqdmProgressBar(stateful_metrics=self.stateful_metrics)
+            else:
+                progbarlogger = ProgbarLogger(stateful_metrics=self.stateful_metrics)
+            callbacks_.append(progbarlogger)
+        callbacks_  += callbacks + [history]
+        self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
+        callback_trainer = self
+        callback_model = self.get_module()
+        self.callbacks.set_trainer(callback_trainer)
+        self.callbacks.set_model(callback_model)
+        self.callbacks.set_optimizer(self.optimizer)
+        self.callbacks.set_params({
+            'epochs': epochs,
+            'steps': self.steps_per_epoch,
+            'verbose': verbose,
+            'metrics': [i for i in self.metrics.keys() if isinstance(i, str)],
+        })
+        logs = {}
+        self.callbacks.on_train_begin(logs)
+        callback_trainer.stop_training = False  # 在EarlyStopping中会重新设置
+
+        # epoch：当前epoch
+        # global_step：当前全局训练步数
+        # local_step: 当前epoch内的训练步数，不同epoch中相同local_step对应的batch数据不一定相同，在steps_per_epoch=None时相同
+        # bti：在dataloader中的index，不同epoch中相同的bti对应的batch数据一般相同，除非重新生成dataloader
+        self.bti = 0
+        for epoch in range(self.resume_epoch, epochs):
+            self.epoch = epoch
+            # resume_step：判断local_step的起点，以及进度条的起始位置
+            resume_step = self.resume_step if epoch==self.resume_epoch else 0
+            self.callbacks.on_epoch_begin(self.global_step, self.epoch)
+            if verbose:
+                progbarlogger.seen = resume_step  # 这里设置进度条的seen，在callbacks中也会修改
+            
+            for local_step in range(resume_step, self.steps_per_epoch):
+                self.local_step = local_step
+                self.global_step = self.epoch * self.steps_per_epoch + self.local_step
+                # 循环dataloader, 不要试用itertools的cycle，遇到过变量不释放的问题
+                try:
+                    batch = next(train_dataloader_iter)
+                except StopIteration:
+                    self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
+                    train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
+                    self.bti = 0
+                    batch = next(train_dataloader_iter)
+                self.train_X, self.train_y = batch
+
+                logs = self.log_init()
+                self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
+
+                self.get_module().train()  # 设置为train模式
+
+                # 入参个数判断，如果入参>=3表示是多个入参，如果=2则表示是一个入参
+                self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
+                self.callbacks.on_train_step_end()
+                                
+                # 参数更新, 真实的参数更新次数要除以grad_accumulation_steps，注意调整总的训练步数
+                if (self.global_step+1) % self.grad_accumulation_steps == 0:
+                    skip_scheduler = False
+                    # 混合精度
+                    if self.mixed_precision:
+                        self.scaler.unscale_(self.optimizer)
+                        if self.clip_grad_norm is not None:  # 梯度裁剪
+                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
+                        self.scaler.step(self.optimizer)
+                        self.scaler.update()
+                        skip_scheduler = self.scaler.get_scale() != self.scale_before_step
+                    else:
+                        if self.clip_grad_norm is not None:  # 梯度裁剪
+                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
+                        self.optimizer.step()
+
+                    self.optimizer.zero_grad()  # 清梯度
+                    if (self.scheduler is not None) and not skip_scheduler:
+                        if isinstance(self.scheduler, (tuple, list)):
+                            for scheduler in self.scheduler:
+                                scheduler.step()
+                        else:
+                            self.scheduler.step()
+
+                # 添加loss至log打印
+                logs.update({'loss': self.loss.item()})
+                logs_loss_detail = {k: v.item() if isinstance(v, torch.Tensor) else v for k, v in self.loss_detail.items()}
+                logs.update(logs_loss_detail)
+                if verbose and (self.global_step == resume_step):
+                    progbarlogger.add_metrics(list(logs_loss_detail.keys()), add_position=1)
+                    
+                # 添加metrics至log打印
+                for metric, func in self.metrics.items():
+                    perf = metric_mapping(metric, func, self.output, self.train_y)  # 内置的一些accuracy指标
+                    if perf is not None:
+                        if isfunction(metric):  # 直接传入回调函数(无key)
+                            if verbose and (self.global_step == resume_step):
+                                progbarlogger.add_metrics(list(perf.keys()))
+                            logs.update(perf)
+                        elif isinstance(metric, str):  # 直接传入回调函数(有key)
+                            logs[metric] = perf
+
+                self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
+
+                self.bti += 1
+            self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
+            # TerminateOnNaN、EarlyStopping等停止训练策略
+            if callback_trainer.stop_training:
+                break
+        self.callbacks.on_train_end(logs)
+        return history
+
+    def log_init(self):
+        '''获取batch_size，主要是用于callback中的BaseLogger和Callback
+        '''
+        # 从train_X中取batch_size，最多允许嵌套两层，即encoder和decoder的((token_ids1, mask1), (token_ids2, mask2))
+        if isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], (list, tuple)):
+            btz = self.train_X[0][0].size(0)
+        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], torch.Tensor):
+            btz = self.train_X[0].size(0)
+        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], dict):
+            btz = self.train_X[0].get('batch_size', 0)
+        elif isinstance(self.train_X, dict):
+            btz = self.train_X.get('batch_size', 0)
+        elif isinstance(self.train_X, torch.Tensor):
+            btz = self.train_X.size(0)
+        else:
+            raise ValueError('Input only support `[list, tuple, tensor]`')
+        logs ={'size': btz}
+
+        # 添加lr
+        try:
+            logs['lr'] = self.optimizer.param_groups[0]["lr"]
+        except:
+            pass
+        return logs
+
+    @torch.no_grad()
+    def predict(self, *inputs, **input_kwargs):
+        '''模型预测，调用forward()'''
+        self.get_module().eval()
+        return self._forward(*inputs, **input_kwargs)
+        
+    def load_steps_params(self, save_path):
+        '''导入训练过程参数
+        
+        :param save_path: str, 训练过程参数保存路径
+        '''
+        step_params = torch.load(save_path)
+        self.resume_step = step_params['resume_step'] 
+        self.resume_epoch = step_params['resume_epoch']
+        return step_params
+
+    def save_steps_params(self, save_path):
+        '''保存训练过程参数
+
+        :param save_path: str, 训练过程参数保存路径
+        '''
+        step_params = {'resume_step': (self.local_step+1) % self.steps_per_epoch, 
+                       'resume_epoch': self.epoch + (self.local_step+1) // self.steps_per_epoch}
+        save_dir = os.path.dirname(save_path)
+        os.makedirs(save_dir, exist_ok=True)
+        torch.save(step_params, save_path)
+
+    def load_weights(self, load_path, strict=True, mapping={}):
+        '''加载模型权重, 支持加载权重文件list
+
+        :param save_path: str/tuple/list, 权重加载路径
+        :param strict: bool, torch.load()是否严格加载
+        :param mapping: dict, 指定key的映射
+        '''
+        state_dict_raw = {}
+        if isinstance(load_path, (tuple, list)):
+            strict = False  # 加载多个权重文件时候，strict设置为False
+        elif isinstance(load_path, str):
+            load_path = [load_path]
+        else:
+            raise ValueError('Args `load_path` only support str/tuple/list format')
+        
+        for load_path_i in load_path:
+            state_dict = torch.load(load_path_i, map_location='cpu')
+            for k, v in state_dict.items():
+                k = mapping.get(k, k)
+                state_dict_raw[k] = v
+            self.get_module().load_state_dict(state_dict_raw, strict=strict)
+
+    def save_weights(self, save_path, mapping={}, trainable_only=False, verbose=1):
+        '''保存模型权重
+
+        :param save_path: str, 权重保存路径
+        :param mapping: dict, 指定key的映射
+        :param trainable_only: bool, 指定仅保存可训练参数
+        '''
+        state_dict_raw = {}
+        state_dict = self.get_module().state_dict()
+        trainable_parameters = set(p for p,v in self.get_module().named_parameters() if v.requires_grad)
+        for k, v in state_dict.items():
+            # 只保存可训练的模型部分
+            if trainable_only and (k not in trainable_parameters):
+                continue
+            k = mapping.get(k, k)
+            state_dict_raw[k] = v
+        
+        save_dir = os.path.dirname(save_path)
+        os.makedirs(save_dir, exist_ok=True)
+        torch.save(state_dict_raw, save_path)
+        if trainable_only and (verbose > 0):
+            params_all = sum(p.numel() for p in self.get_module().parameters())
+            params_trainable = sum(p.numel() for p in self.get_module().parameters() if p.requires_grad)
+            print(f"[INFO] Only trainable parameters saved and occupy {params_trainable}/{params_all} {params_trainable/params_all:.2f}%")
+
+    def resume_from_checkpoint(self, model_path=None, optimizer_path=None, step_params_path=None):
+        '''同时加载模型、优化器、训练过程参数
+
+        :param model_path: str, 模型文件路径
+        :param optimizer_path: str, 优化器文件路径
+        :param step_params_path: str, 训练过程参数保存路径
+        '''
+        # 加载模型权重
+        if model_path:
+            self.load_weights(model_path)
+        # 加载优化器，断点续训使用
+        if optimizer_path:
+            state_dict = torch.load(optimizer_path, map_location='cpu')
+            self.optimizer.load_state_dict(state_dict)
+        # 加载训练进度参数，断点续训使用
+        self.load_steps_params(step_params_path)
+
+    def save_to_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None, verbose=0):
+        '''同时保存模型、优化器、训练过程参数、scheduler
+
+        :param model_path: str, 模型文件路径
+        :param optimizer_path: str, 优化器文件路径
+        :param scheduler_path: str, scheduler文件路径
+        :param step_params_path: str, 训练过程参数保存路径
+        '''
+        verbose_str = ''
+        if model_path:
+            self.save_weights(model_path)
+            verbose_str += f'Model weights successfuly saved to {model_path}.\n'
+        if optimizer_path:
+            save_dir = os.path.dirname(optimizer_path)
+            os.makedirs(save_dir, exist_ok=True)
+            torch.save(self.optimizer.state_dict(), optimizer_path)
+            verbose_str += f'Optimizer successfuly saved to {optimizer_path}.\n'
+        if scheduler_path and (self.scheduler is not None):
+            save_dir = os.path.dirname(scheduler_path)
+            os.makedirs(save_dir, exist_ok=True)
+            torch.save(self.scheduler.state_dict(), scheduler_path)
+            verbose_str += f'Scheduler successfuly saved to {scheduler_path}.\n'
+        if step_params_path:
+            self.save_steps_params(step_params_path)
+            verbose_str += f'Steps_params successfuly saved to {step_params_path}.\n'
+        if verbose != 0:
+            print(verbose_str)
+
+    def get_module(self):
+        '''返回nn.Module模块
+        '''
+        if isinstance(self, nn.Module): return self
+        return self.module if hasattr(self, 'module') else self
+
+
+class BaseModel(Trainer, nn.Module):
+    """BaseModel, 使用继承的方式来使用
+    """
+    def __init__(self, *args, **kwargs):
+        nn.Module.__init__(self)
+        Trainer.__init__(self, *args, **kwargs)
+        
+
+class BaseModelDP(nn.DataParallel, BaseModel):
+    '''DataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
+    '''
+    def __init__(self, *args, **kwargs):
+        BaseModel.__init__(self)
+        nn.DataParallel.__init__(self, *args, **kwargs)
+
+
+class BaseModelDDP(nn.parallel.DistributedDataParallel, BaseModel):
+    '''DistributedDataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
+    '''
+    def __init__(self, *args, master_rank=0, **kwargs):
+        BaseModel.__init__(self)
+        nn.parallel.DistributedDataParallel.__init__(self, *args, **kwargs)
+
+        # 默认仅对master_rank=0打印信息
+        assert isinstance(master_rank, (int, list, tuple)), 'Args `master_rank` only supoorts int, list, tuple'
+        if isinstance(master_rank, int):
+            master_rank = [master_rank]
+        self.verbose = (torch.distributed.get_rank() in master_rank)
+
+
+TrainerDP = BaseModelDP
+TrainerDDP = BaseModelDDP
+
+
+def add_trainer(obj, include=None, exclude=None):
+    '''为对象添加Triner对应的方法
+    '''
+    include = include or []
+    exclude = exclude or []
+    if isinstance(obj, (Trainer, TrainerDP, TrainerDDP, BaseModel, BaseModelDP, BaseModelDDP)):
+        return obj
+    
+    if isinstance(obj, nn.Module):
+        import types
+        for k in dir(Trainer):
+            if k in include:  # 必须包含的
+                pass
+            elif k in exclude:  # 必须屏蔽的
+                continue
+            elif k.startswith('__') and k.endswith('__'):
+                continue
+            elif hasattr(obj, k):  # 如果下游重新定义，则不继承
+                continue
+            exec(f'obj.{k} = types.MethodType(Trainer.{k}, obj)')
+        obj.initialize()
     return obj
```

### Comparing `torch4keras-0.0.7/torch4keras/snippets.py` & `torch4keras-0.0.7.post2/torch4keras/snippets.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-import numpy as np
-import torch
-import time
-import inspect
-from packaging import version
-from torch.utils.data import Dataset, IterableDataset
-import os
-import random
-
-try:
-    from sklearn.metrics import roc_auc_score
-except ImportError:
-    roc_auc_score = None
-        
-def take_along_dim(input_tensor, indices, dim=None):
-    '''兼容部分低版本pytorch没有torch.take_along_dim
-    '''
-    if version.parse(torch.__version__) > version.parse('1.8.1'):
-        return torch.take_along_dim(input_tensor, indices, dim)
-    else:
-        # 该逻辑仅在少量数据上测试，如有bug，欢迎反馈
-        if dim is None:
-            res = input_tensor.flatten()[indices]
-        else:
-            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
-            res = torch.from_numpy(res).to(input_tensor.device)
-        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
-        return res
-
-
-def torch_div(input, other, rounding_mode=None):
-    ''' torch.div兼容老版本
-    '''
-    if version.parse(torch.__version__) < version.parse('1.7.2'):
-        indices = input // other  # 兼容老版本
-    else:
-        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
-    return indices
-
-
-def softmax(x, axis=-1):
-    """numpy版softmax
-    """
-    x = x - x.max(axis=axis, keepdims=True)
-    x = np.exp(x)
-    return x / x.sum(axis=axis, keepdims=True)
-
-
-def search_layer(model, layer_name, retrun_first=True):
-    '''根据layer_name搜索并返回参数/参数list
-    '''
-    return_list = []
-    for name, param in model.named_parameters():
-        if param.requires_grad and layer_name in name:
-            return_list.append(param)
-    if len(return_list) == 0:
-        return None
-    if retrun_first:
-        return return_list[0]
-    else:
-        return return_list
-
-
-class ListDataset(Dataset):
-    '''数据是List格式Dataset，支持传入file_path或者外部已读入的data(List格式)
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    :param data: List[Any], list格式的数据，和file_path至少有一个不为None
-    '''
-    def __init__(self, file_path=None, data=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.data = self.load_data(file_path)
-        elif isinstance(data, list):
-            self.data = data
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        return self.data[index]
-
-    @staticmethod
-    def load_data(file_path):
-        return file_path
-
-
-class IterDataset(IterableDataset):
-    '''流式读取文件，用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    '''
-    def __init__(self, file_path=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.file_path = file_path
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-    
-    def __iter__(self):
-        return self.load_data(self.file_path)
-
-    @staticmethod
-    def load_data(file_path, verbose=0):
-        if isinstance(file_path, (tuple, list)):
-            for file in file_path:
-                if verbose != 0:
-                    print("Load data: ", file)
-                with open(file, 'r') as file_obj:
-                    for line in file_obj:
-                        yield line
-        elif isinstance(file_path, str):
-            with open(file_path, 'r') as file_obj:
-                for line in file_obj:
-                    yield line
-
-
-def metric_mapping(metric, func, y_pred, y_true):
-    '''metric的计算
-
-    :param metric: str, 自带metrics的名称
-    :param func: function, 透传的用户自定的计算指标的函数
-    :param y_pred: torch.Tensor, 样本的预测结果
-    :param y_true: torch.Tensor, 样本的真实结果
-    '''
-    # 自定义metrics
-    if inspect.isfunction(func):
-        metric_res = func(y_pred, y_true)
-        if inspect.isfunction(metric):
-            # 如果直接传入回调函数（无key），要求回调函数返回Dict[String: Int/Float]类型
-            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
-        elif isinstance(metric, str):
-            # 如果直接传入回调函数（有key），要求回调函数返回Int/Float类型
-            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
-        return metric_res
-    elif metric == 'loss':
-        pass
-    # 自带metrics
-    elif isinstance(metric, str):
-        # 如果forward返回了list, tuple，则选取第一项
-        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
-        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
-        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估，detach不进入计算图
-
-        # 根据shape做预处理
-        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
-            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
-        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
-            pass
-        else:
-            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
-
-        # 执行内置的metric
-        if metric in {'accuracy', 'acc'}:
-            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
-        elif metric in {'auc'}:
-            if roc_auc_score is None:
-                raise ImportError('roc_auc_score requires the `sklearn` library.')
-            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
-        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
-            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
-            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
-            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
-            return 100. * torch.mean(diff).item()
-        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
-            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
-            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
-            return torch.mean(torch.square(first_log - second_log)).item()
-
-    return None
-
-
-def seed_everything(seed=None):
-    '''固定seed
-    
-    :param seed: int, 随机种子
-    '''
-    max_seed_value = np.iinfo(np.uint32).max
-    min_seed_value = np.iinfo(np.uint32).min
-
-    if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
-        seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
-    print(f"Global seed set to {seed}")
-    os.environ["PYTHONHASHSEED"] = str(seed)
-    random.seed(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-    torch.backends.cudnn.benchmark = False
-    torch.backends.cudnn.deterministic = True
-    return seed
-
-
-def spend_time(func):
-    '''装饰器，计算函数消耗的时间
-    '''
-    start = time.time()
-    def warpper(*args, **kwargs):
-        res = func(*args, **kwargs)
-        end = time.time()
-        consume = end - start
-        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
-        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
-        print(f'{start1} ~ {end1}  spent {consume:.2f}s')
-        return res
-    return warpper
+import numpy as np
+import torch
+import time
+import inspect
+from packaging import version
+from torch.utils.data import Dataset, IterableDataset
+import os
+import random
+
+try:
+    from sklearn.metrics import roc_auc_score
+except ImportError:
+    roc_auc_score = None
+        
+def take_along_dim(input_tensor, indices, dim=None):
+    '''兼容部分低版本pytorch没有torch.take_along_dim
+    '''
+    if version.parse(torch.__version__) > version.parse('1.8.1'):
+        return torch.take_along_dim(input_tensor, indices, dim)
+    else:
+        # 该逻辑仅在少量数据上测试，如有bug，欢迎反馈
+        if dim is None:
+            res = input_tensor.flatten()[indices]
+        else:
+            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
+            res = torch.from_numpy(res).to(input_tensor.device)
+        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
+        return res
+
+
+def torch_div(input, other, rounding_mode=None):
+    ''' torch.div兼容老版本
+    '''
+    if version.parse(torch.__version__) < version.parse('1.7.2'):
+        indices = input // other  # 兼容老版本
+    else:
+        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
+    return indices
+
+
+def softmax(x, axis=-1):
+    """numpy版softmax
+    """
+    x = x - x.max(axis=axis, keepdims=True)
+    x = np.exp(x)
+    return x / x.sum(axis=axis, keepdims=True)
+
+
+def search_layer(model, layer_name, retrun_first=True):
+    '''根据layer_name搜索并返回参数/参数list
+    '''
+    return_list = []
+    for name, param in model.named_parameters():
+        if param.requires_grad and layer_name in name:
+            return_list.append(param)
+    if len(return_list) == 0:
+        return None
+    if retrun_first:
+        return return_list[0]
+    else:
+        return return_list
+
+
+class ListDataset(Dataset):
+    '''数据是List格式Dataset，支持传入file_path或者外部已读入的data(List格式)
+
+    :param file_path: str, 待读取的文件的路径，若无可以为None
+    :param data: List[Any], list格式的数据，和file_path至少有一个不为None
+    '''
+    def __init__(self, file_path=None, data=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.data = self.load_data(file_path)
+        elif isinstance(data, list):
+            self.data = data
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        return self.data[index]
+
+    @staticmethod
+    def load_data(file_path):
+        return file_path
+
+
+class IterDataset(IterableDataset):
+    '''流式读取文件，用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
+
+    :param file_path: str, 待读取的文件的路径，若无可以为None
+    '''
+    def __init__(self, file_path=None, **kwargs):
+        self.kwargs = kwargs
+        if isinstance(file_path, (str, tuple, list)):
+            self.file_path = file_path
+        else:
+            raise ValueError('The input args shall be str format file_path / list format dataset')
+    
+    def __iter__(self):
+        return self.load_data(self.file_path)
+
+    @staticmethod
+    def load_data(file_path, verbose=0):
+        if isinstance(file_path, (tuple, list)):
+            for file in file_path:
+                if verbose != 0:
+                    print("Load data: ", file)
+                with open(file, 'r') as file_obj:
+                    for line in file_obj:
+                        yield line
+        elif isinstance(file_path, str):
+            with open(file_path, 'r') as file_obj:
+                for line in file_obj:
+                    yield line
+
+
+def metric_mapping(metric, func, y_pred, y_true):
+    '''metric的计算
+
+    :param metric: str, 自带metrics的名称
+    :param func: function, 透传的用户自定的计算指标的函数
+    :param y_pred: torch.Tensor, 样本的预测结果
+    :param y_true: torch.Tensor, 样本的真实结果
+    '''
+    # 自定义metrics
+    if inspect.isfunction(func):
+        metric_res = func(y_pred, y_true)
+        if inspect.isfunction(metric):
+            # 如果直接传入回调函数（无key），要求回调函数返回Dict[String: Int/Float]类型
+            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
+        elif isinstance(metric, str):
+            # 如果直接传入回调函数（有key），要求回调函数返回Int/Float类型
+            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
+        return metric_res
+    elif metric == 'loss':
+        pass
+    # 自带metrics
+    elif isinstance(metric, str):
+        # 如果forward返回了list, tuple，则选取第一项
+        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
+        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
+        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估，detach不进入计算图
+
+        # 根据shape做预处理
+        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
+            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
+        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
+            pass
+        else:
+            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
+
+        # 执行内置的metric
+        if metric in {'accuracy', 'acc'}:
+            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
+        elif metric in {'auc'}:
+            if roc_auc_score is None:
+                raise ImportError('roc_auc_score requires the `sklearn` library.')
+            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
+        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
+            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
+            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
+        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
+            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
+            return 100. * torch.mean(diff).item()
+        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
+            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
+            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
+            return torch.mean(torch.square(first_log - second_log)).item()
+
+    return None
+
+
+def seed_everything(seed=None):
+    '''固定seed
+    
+    :param seed: int, 随机种子
+    '''
+    max_seed_value = np.iinfo(np.uint32).max
+    min_seed_value = np.iinfo(np.uint32).min
+
+    if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
+        seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
+    print(f"Global seed set to {seed}")
+    os.environ["PYTHONHASHSEED"] = str(seed)
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.deterministic = True
+    return seed
+
+
+def spend_time(func):
+    '''装饰器，计算函数消耗的时间
+    '''
+    start = time.time()
+    def warpper(*args, **kwargs):
+        res = func(*args, **kwargs)
+        end = time.time()
+        consume = end - start
+        start1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(start))
+        end1 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(end))
+        print(f'{start1} ~ {end1}  spent {consume:.2f}s')
+        return res
+    return warpper
```

### Comparing `torch4keras-0.0.7/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.0.7.post2/torch4keras.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,98 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.7
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# torch4keras
-**Use torch like keras**
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
-[![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
-
-[Documentation](https://torch4keras.readthedocs.io) |
-[Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
-[Source code](https://github.com/Tongjilibo/torch4keras)
-
-## 1. 下载安装
-安装稳定版
-```shell
-pip install torch4keras
-```
-安装最新版
-```shell
-pip install git+https://github.com/Tongjilibo/torch4keras.git
-```
-
-## 2. 功能
-- 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
-- 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
-- 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
-- 训练：
-
-    ```text
-    2022-10-28 23:16:10 - Start Training
-    2022-10-28 23:16:10 - Epoch: 1/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-    test_acc: 0.98045. best_test_acc: 0.98045
-
-    2022-10-28 23:16:27 - Epoch: 2/5
-    5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-    test_acc: 0.98280. best_test_acc: 0.98280
-
-    2022-10-28 23:16:44 - Epoch: 3/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
-    test_acc: 0.98365. best_test_acc: 0.98365
-
-    2022-10-28 23:17:03 - Epoch: 4/5
-    5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
-    test_acc: 0.98265. best_test_acc: 0.98365
-
-    2022-10-28 23:17:21 - Epoch: 5/5
-    5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
-    Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
-    test_acc: 0.98585. best_test_acc: 0.98585
-
-    2022-10-28 23:17:37 - Finish Training
-    ```
-
-## 3. 快速上手
-- 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
-- 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
-
-## 4. 版本说明
-- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
-- **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **v0.0.3.post2**：20221107 修复DDP下打印的bug
-- **v0.0.3**：20221106 参考Keras修改了callback的逻辑
-- **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **v0.0.1**：20221019 初始版本
-
-## 5. 更新：
-- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
-- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
-- **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
-- **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
-- **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
-- **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
-- **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
-- **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
-- **20221019**：初版提交
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.7.post2
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description: # torch4keras
+        **Use torch like keras**
+        
+        [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
+        [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
+        [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
+        [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
+        [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
+        [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
+        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
+        
+        [Documentation](https://torch4keras.readthedocs.io) |
+        [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
+        [Source code](https://github.com/Tongjilibo/torch4keras)
+        
+        ## 1. 下载安装
+        安装稳定版
+        ```shell
+        pip install torch4keras
+        ```
+        安装最新版
+        ```shell
+        pip install git+https://github.com/Tongjilibo/torch4keras.git
+        ```
+        
+        ## 2. 功能
+        - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
+        - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
+        - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
+        - 训练：
+        
+            ```text
+            2022-10-28 23:16:10 - Start Training
+            2022-10-28 23:16:10 - Epoch: 1/5
+            5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+            test_acc: 0.98045. best_test_acc: 0.98045
+        
+            2022-10-28 23:16:27 - Epoch: 2/5
+            5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+            test_acc: 0.98280. best_test_acc: 0.98280
+        
+            2022-10-28 23:16:44 - Epoch: 3/5
+            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0284 - acc: 0.9915
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 673.60it/s] 
+            test_acc: 0.98365. best_test_acc: 0.98365
+        
+            2022-10-28 23:17:03 - Epoch: 4/5
+            5000/5000 [==============================] - 15s 3ms/step - loss: 0.0179 - acc: 0.9948
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 692.34it/s] 
+            test_acc: 0.98265. best_test_acc: 0.98365
+        
+            2022-10-28 23:17:21 - Epoch: 5/5
+            5000/5000 [==============================] - 14s 3ms/step - loss: 0.0129 - acc: 0.9958
+            Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 701.77it/s] 
+            test_acc: 0.98585. best_test_acc: 0.98585
+        
+            2022-10-28 23:17:37 - Finish Training
+            ```
+        
+        ## 3. 快速上手
+        - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
+        - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
+        
+        ## 4. 版本说明
+        - **v0.0.7.post2**20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+        - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+        - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
+        - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+        - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+        - **v0.0.3.post2**：20221107 修复DDP下打印的bug
+        - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
+        - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+        - **v0.0.1**：20221019 初始版本
+        
+        ## 5. 更新：
+        - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
+        - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+        - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+        - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
+        - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
+        - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
+        - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
+        - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
+        - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
+        - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
+        - **20221019**：初版提交
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

