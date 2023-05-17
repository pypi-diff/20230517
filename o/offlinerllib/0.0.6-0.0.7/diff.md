# Comparing `tmp/offlinerllib-0.0.6.tar.gz` & `tmp/offlinerllib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinerllib-0.0.6.tar", last modified: Wed Apr 12 12:38:51 2023, max compression
+gzip compressed data, was "offlinerllib-0.0.7.tar", last modified: Wed May 17 07:14:54 2023, max compression
```

## Comparing `offlinerllib-0.0.6.tar` & `offlinerllib-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/d4rl_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/module/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/policy/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/policy/model_free/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/awac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/bppo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/edac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/inac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/iql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/sacn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/td3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/td3bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/xql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.017917 offlinerllib-0.0.7/offlinerllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/buffer/d4rl_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/d4rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/env/mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32225 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/module/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/module/net/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib/policy/model_free/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/awac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/edac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/inac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/iql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/sacn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/td3bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/xql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/offlinerllib/policy/model_free/xsac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:14:54.021917 offlinerllib-0.0.7/offlinerllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 07:14:54.000000 offlinerllib-0.0.7/offlinerllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:14:54.025917 offlinerllib-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-17 07:14:45.000000 offlinerllib-0.0.7/setup.py
```

### Comparing `offlinerllib-0.0.6/LICENSE` & `offlinerllib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.6/PKG-INFO` & `offlinerllib-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.6/README.md` & `offlinerllib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.6/offlinerllib/buffer/d4rl_buffer.py` & `offlinerllib-0.0.7/offlinerllib/buffer/d4rl_buffer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from torch.utils.data import Dataset, IterableDataset
 
 from offlinerllib.buffer.base import Buffer
 from offlinerllib.utils.functional import discounted_cum_sum
 
-
 def pad_along_axis(
     arr: np.ndarray, pad_to: int, axis: int = 0, fill_value: float = 0.0
 ) -> np.ndarray:
     pad_size = pad_to - arr.shape[axis]
     if pad_size <= 0:
         return arr
 
@@ -47,67 +46,91 @@
         
     def random_batch(self, batch_size: int):
         idx = np.random.randint(self.size, size=batch_size)
         return self.__getitem__(idx)
         
 
 class D4RLTrajectoryBuffer(Buffer, IterableDataset):
-    def __init__(self, dataset, seq_len: int, discount: float=1.0, return_scale: float=1.0):
-        # fetch data from dataset
+    def __init__(
+        self, 
+        dataset, 
+        seq_len: int, 
+        discount: float=1.0, 
+        return_scale: float=1.0,
+    ) -> None:
         converted_dataset = {
             "observations": dataset["observations"].astype(np.float32), 
             "actions": dataset["actions"].astype(np.float32), 
             "rewards": dataset["rewards"][:, None].astype(np.float32), 
             "terminals": dataset["terminals"][:, None].astype(np.float32), 
             "next_observations": dataset["next_observations"].astype(np.float32)
         }
-
         traj, traj_len = [], []
         self.seq_len = seq_len
+        self.discount = discount
+        self.return_scale = return_scale
         traj_start = 0
         for i in range(dataset["rewards"].shape[0]):
             if dataset["ends"][i]:
                 episode_data = {k: v[traj_start:i+1] for k, v in converted_dataset.items()}
-                episode_data["returns"] = discounted_cum_sum(episode_data["rewards"], discount=discount) / return_scale
+                episode_data["returns"] = discounted_cum_sum(episode_data["rewards"], discount=discount) * self.return_scale
                 traj.append(episode_data)
                 traj_len.append(i+1-traj_start)
                 traj_start = i+1
-        self.traj = np.array(traj, dtype=object)
         self.traj_len = np.array(traj_len)
-        self.traj_num = len(self.traj_len)
         self.size = self.traj_len.sum()
+        self.traj_num = len(self.traj_len)
         self.sample_prob = self.traj_len / self.size
-
-        del converted_dataset
         
+        # pad trajs to have the same mask len
+        self.max_len = self.traj_len.max() + self.seq_len - 1  # this is for the convenience of sampling
+        for i_traj in range(self.traj_num):
+            this_len = self.traj_len[i_traj]
+            for _key, _value in traj[i_traj].items():
+                traj[i_traj][_key] = pad_along_axis(_value, pad_to=self.max_len)
+            traj[i_traj]["masks"] = np.hstack([np.ones(this_len), np.zeros(self.max_len-this_len)])
+        
+        # register all entries
+        self.observations = np.asarray([t["observations"] for t in traj])
+        self.actions = np.asarray([t["actions"] for t in traj])
+        self.rewards = np.asarray([t["rewards"] for t in traj])
+        self.terminals = np.asarray([t["terminals"] for t in traj])
+        self.next_observations = np.asarray([t["next_observations"] for t in traj])
+        self.returns = np.asarray([t["returns"] for t in traj])
+        self.masks = np.asarray([t["masks"] for t in traj])
+        self.timesteps = np.arange(self.max_len)
+
+    def __len__(self):
+        return self.size
+
     def __prepare_sample(self, traj_idx, start_idx):
-        traj = self.traj[traj_idx]
-        sample = {k: v[start_idx:start_idx+self.seq_len] for k, v in traj.items()}
-        sample_len = len(sample["observations"])
-        if sample_len < self.seq_len:
-            sample = {k: pad_along_axis(v, pad_to=self.seq_len) for k, v in sample.items()}
-        masks = np.hstack([np.ones(sample_len), np.zeros(self.seq_len-sample_len)])
-        sample["masks"] = masks
-        sample["timesteps"] = np.arange(start_idx, start_idx+self.seq_len)
-        return sample
+        return {
+            "observations": self.observations[traj_idx, start_idx:start_idx+self.seq_len], 
+            "actions": self.actions[traj_idx, start_idx:start_idx+self.seq_len], 
+            "rewards": self.rewards[traj_idx, start_idx:start_idx+self.seq_len], 
+            "terminals": self.terminals[traj_idx, start_idx:start_idx+self.seq_len], 
+            "next_observations": self.next_observations[traj_idx, start_idx:start_idx+self.seq_len], 
+            "returns": self.returns[traj_idx, start_idx:start_idx+self.seq_len], 
+            "masks": self.masks[traj_idx, start_idx:start_idx+self.seq_len], 
+            "timesteps": self.timesteps[start_idx:start_idx+self.seq_len]
+        }
     
     def __iter__(self):
         while True:
             traj_idx = np.random.choice(self.traj_num, p=self.sample_prob)
             start_idx = np.random.choice(self.traj_len[traj_idx])
             yield self.__prepare_sample(traj_idx, start_idx)
-        
+            
     def random_batch(self, batch_size: int):
         batch_data = {}
         traj_idxs = np.random.choice(self.traj_num, size=batch_size, p=self.sample_prob)
         for i in range(batch_size):
             traj_idx = traj_idxs[i]
             start_idx = np.random.choice(self.traj_len[traj_idx])
             sample = self.__prepare_sample(traj_idx, start_idx)
             for _key, _value in sample.items():
                 if not _key in batch_data:
                     batch_data[_key] = []
                 batch_data[_key].append(_value)
         for _key, _value in batch_data.items():
             batch_data[_key] = np.vstack(_value)
-        return batch_data
-            
+        return batch_data
```

### Comparing `offlinerllib-0.0.6/offlinerllib/module/actor.py` & `offlinerllib-0.0.7/offlinerllib/module/actor.py`

 * *Files 17% similar despite different names*

```diff
@@ -262,27 +262,29 @@
     input_dim :  The dimensions of input (the output of backend module). 
     output_dim :  The dimension of actor's output. 
     reparameterize : Whether to use the reparameterization trick when sampling. 
     conditioned_logstd :  Whether the logstd is conditioned on the observation. 
     fix_logstd :  If not None, the logstd will be set to this value and fixed (un-learnable). 
     logstd_min: The minimum value of logstd. Default is -20. 
     logstd_max: The maximum value of logstd. Default is 2. 
+    logstd_hard_clip: Whether or not to hard-clip the logstd. If True, then logstd = clip(logstd_out, logstd_min, logstd_max); otherwise logstd = frac{tanh(logstd_out)+1}{2}*(logstd_max-logstd_min) + logstd_min. 
     device :  The device which the model runs on. Default is cpu. 
     ***(any args of MLP or EnsembleMLP)
     """
     def __init__(
         self, 
         backend: nn.Module, 
         input_dim: int, 
         output_dim: int, 
         reparameterize: bool=True, 
         conditioned_logstd: bool=True, 
         fix_logstd: Optional[float]=None, 
         logstd_min: int = -20, 
         logstd_max: int = 2,
+        logstd_hard_clip: bool=True, 
         device: Union[str, int, torch.device]="cpu", 
         *, 
         ensemble_size: int = 1, 
         hidden_dims: Union[int, Sequence[int]]=[],
         norm_layer: Optional[Union[ModuleType, Sequence[ModuleType]]] = None, 
         activation: Optional[Union[ModuleType, Sequence[ModuleType]]] = nn.ReLU, 
         dropout: Optional[Union[float, Sequence[float]]] = None, 
@@ -292,14 +294,15 @@
         
         self.actor_type = "GaussianActor"
         self.input_dim = input_dim
         self.output_dim = output_dim
         self.reparameterize = reparameterize
         self.device = device
         self.backend = backend
+        self.logstd_hard_clip = logstd_hard_clip
         
         if fix_logstd is not None:
             self._logstd_is_layer = False
             self.register_buffer("logstd", torch.tensor(fix_logstd))
         elif not conditioned_logstd:
             self._logstd_is_layer = False
             self.logstd = nn.Parameter(torch.zeros([self.output_dim]), requires_grad=True)
@@ -340,15 +343,18 @@
     def forward(self, input: torch.Tensor):
         out = self.output_layer(self.backend(input))
         if self._logstd_is_layer:
             mean, logstd = torch.split(out, self.output_dim // 2, dim=-1)
         else:
             mean = out
             logstd = self.logstd.broadcast_to(mean.shape)
-        logstd = torch.clip(logstd, min=self.logstd_min, max=self.logstd_max)
+        if self.logstd_hard_clip:
+            logstd = torch.clip(logstd, min=self.logstd_min, max=self.logstd_max)
+        else:
+            logstd = self.logstd_min + (torch.tanh(logstd)+1)/2*(self.logstd_max - self.logstd_min)
         return mean, logstd
     
     def sample(self, obs: torch.Tensor, deterministic: bool=False, return_mean_logstd: bool=False, *args, **kwargs) -> Tuple[torch.Tensor, torch.Tensor, Dict]:
         """Sampling procedure. The action is sampled from a Gaussian distribution.
 
         Parameters
         ----------
@@ -414,38 +420,40 @@
     input_dim :  The dimensions of input (the output of backend module). 
     output_dim :  The dimension of actor's output. 
     reparameterize : Whether to use the reparameterization trick when sampling. 
     conditioned_logstd :  Whether the logstd is conditioned on the observation. 
     fix_logstd :  If not None, the logstd will be set to this value and fixed (un-learnable). 
     logstd_min: The minimum value of logstd. Default is -20. 
     logstd_max: The maximum value of logstd. Default is 2. 
+    logstd_hard_clip: Whether or not to hard-clip the logstd. If True, then logstd = clip(logstd_out, logstd_min, logstd_max); otherwise logstd = frac{tanh(logstd_out)+1}{2}*(logstd_max-logstd_min) + logstd_min. 
     device :  The device which the model runs on. Default is cpu. 
     ***(any args of MLP or EnsembleMLP)
     """
     def __init__(
         self, 
         backend: nn.Module, 
         input_dim: int, 
         output_dim: int, 
         reparameterize: bool = True, 
         conditioned_logstd: bool = True, 
         fix_logstd: Optional[float] = None, 
         logstd_min: int = -20, 
         logstd_max: int = 2, 
+        logstd_hard_clip: bool=True, 
         device: Union[str, int, torch.device]="cpu",
         *, 
         ensemble_size: int = 1, 
         hidden_dims: Union[int, Sequence[int]]=[],
         norm_layer: Optional[Union[ModuleType, Sequence[ModuleType]]] = None, 
         activation: Optional[Union[ModuleType, Sequence[ModuleType]]] = nn.ReLU, 
         dropout: Optional[Union[float, Sequence[float]]] = None, 
         share_hidden_layer: Union[Sequence[bool], bool] = False, 
     ) -> None:
         super().__init__(
-            backend, input_dim, output_dim, reparameterize, conditioned_logstd, fix_logstd, logstd_min, logstd_max, device,  
+            backend, input_dim, output_dim, reparameterize, conditioned_logstd, fix_logstd, logstd_min, logstd_max, logstd_hard_clip, device,  
             ensemble_size=ensemble_size, 
             hidden_dims=hidden_dims, 
             norm_layer=norm_layer, 
             activation=activation, 
             dropout=dropout, 
             share_hidden_layer=share_hidden_layer
         )
@@ -490,15 +498,15 @@
         Returns
         -------
         (torch.Tensor, Dict) :  The log-probability of action at obs and the info dict. 
 
         :param state: state of the environment.
         :param action: action to be evaluated.
         """
-        mean, logstd = self(obs)
+        mean, logstd = self.forward(obs)
         dist = TanhNormal(mean, logstd.exp())
         info = {"dist": dist} if return_dist else False
         return dist.log_prob(action).sum(-1, keepdim=True), info
     
     
 class ClippedGaussianActor(GaussianActor):
     """
@@ -518,38 +526,40 @@
     input_dim :  The dimensions of input (the output of backend module). 
     output_dim :  The dimension of actor's output. 
     reparameterize : Whether to use the reparameterization trick when sampling. 
     conditioned_logstd :  Whether the logstd is conditioned on the observation. 
     fix_logstd :  If not None, the logstd will be set to this value and fixed (un-learnable). 
     logstd_min: The minimum value of logstd. Default is -20. 
     logstd_max: The maximum value of logstd. Default is 2. 
+    logstd_hard_clip: Whether or not to hard-clip the logstd. If True, then logstd = clip(logstd_out, logstd_min, logstd_max); otherwise logstd = frac{tanh(logstd_out)+1}{2}*(logstd_max-logstd_min) + logstd_min. 
     device :  The device which the model runs on. Default is cpu. 
     ***(any args of MLP or EnsembleMLP)
     """
     def __init__(
         self, 
         backend: nn.Module, 
         input_dim: int, 
         output_dim: int, 
         reparameterize: bool = True, 
         conditioned_logstd: bool = True, 
         fix_logstd: Optional[float] = None, 
         logstd_min: int = -20, 
         logstd_max: int = 2, 
+        logstd_hard_clip: bool=True, 
         device: Union[str, int, torch.device]="cpu",
         *, 
         ensemble_size: int = 1, 
         hidden_dims: Union[int, Sequence[int]]=[],
         norm_layer: Optional[Union[ModuleType, Sequence[ModuleType]]] = None, 
         activation: Optional[Union[ModuleType, Sequence[ModuleType]]] = nn.ReLU, 
         dropout: Optional[Union[float, Sequence[float]]] = None, 
         share_hidden_layer: Union[Sequence[bool], bool] = False, 
     ) -> None:
         super().__init__(
-            backend, input_dim, output_dim, reparameterize, conditioned_logstd, fix_logstd, logstd_min, logstd_max, device,  
+            backend, input_dim, output_dim, reparameterize, conditioned_logstd, fix_logstd, logstd_min, logstd_max, logstd_hard_clip, device,  
             ensemble_size=ensemble_size, 
             hidden_dims=hidden_dims, 
             norm_layer=norm_layer, 
             activation=activation, 
             dropout=dropout, 
             share_hidden_layer=share_hidden_layer
         )
@@ -597,15 +607,15 @@
         Returns
         -------
         (torch.Tensor, Dict) :  The log-probability of action at obs and the info dict. 
 
         :param state: state of the environment.
         :param action: action to be evaluated.
         """
-        mean, logstd = self(obs)
+        mean, logstd = self.forward(obs)
         mean = torch.tanh(mean)
         dist = Normal(mean, logstd.exp())
         info = {"dist": dist} if return_dist else {}
         return dist.log_prob(action).sum(-1, keepdim=True), info
 
 
 class CategoricalActor(BaseActor):
```

### Comparing `offlinerllib-0.0.6/offlinerllib/module/critic.py` & `offlinerllib-0.0.7/offlinerllib/module/critic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.6/offlinerllib/module/net/basic.py` & `offlinerllib-0.0.7/offlinerllib/module/net/basic.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.6/offlinerllib/module/net/mlp.py` & `offlinerllib-0.0.7/offlinerllib/module/net/mlp.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/awac.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/awac.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,35 +17,33 @@
     Advantage Weighted Actor Critic <Ref: https://arxiv.org/abs/2006.09359>
     """
     
     def __init__(
         self, 
         actor: nn.Module, 
         critic: nn.Module, 
-        actor_optim: torch.optim.Optimizer, 
-        critic_optim: torch.optim.Optimizer, 
         aw_lambda: float = 1.0, 
         discount: float = 0.99, 
         tau: float = 5e-3, 
         exp_adv_max: float = 100.0, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__(
             actor=actor, 
             critic=critic, 
-            actor_optim=actor_optim, 
-            critic_optim=critic_optim, 
             tau=tau, 
             discount=discount, 
             alpha=0.0, 
             device=device
         )
         self._exp_adv_max = exp_adv_max
         self._aw_lambda = aw_lambda
-        
+
+    def configure_optimizers(self, actor_lr, critic_lr):
+        return super().configure_optimizers(actor_lr, critic_lr)
         
     def _actor_loss(self, batch: Dict[str, Any]) -> Dict[str, Any]:
         obss, actions = itemgetter("observations", "actions")(batch)
         with torch.no_grad():
             baseline_actions, *_ = self.actor.sample(obss)
             v = self.critic(obss, baseline_actions).min(0)[0]
             q = self.critic(obss, actions).min(0)[0]
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/dt.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/dt.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,31 +11,37 @@
 class DecisionTransformerPolicy(BasePolicy):
     """
     Decision Transformer: Reinforcement Learning via Sequence Modeling <Ref: https://arxiv.org/abs/2106.01345>
     """
     def __init__(
         self, 
         dt: DecisionTransformer, 
-        dt_optim: torch.optim, 
         state_dim: int, 
         action_dim: int, 
         seq_len: int, 
         episode_len: int, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__()
         self.dt = dt
-        self.dt_optim = dt_optim
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.seq_len = seq_len
         self.episode_len = episode_len
         
         self.to(device)
 
+    def configure_optimizers(self, lr, weight_decay, betas, warmup_steps):
+        decay, no_decay = self.dt.configure_params()
+        self.dt_optim = torch.optim.AdamW([
+            {"params": decay, "weight_decay": weight_decay}, 
+            {"params": no_decay, "weight_decay": 0.0}
+        ], lr=lr, betas=betas)
+        self.dt_optim_scheduler = torch.optim.lr_scheduler.LambdaLR(self.dt_optim, lambda step: min((step+1)/warmup_steps, 1))
+
     @torch.no_grad()
     def select_action(self, states, actions, returns_to_go, timesteps, **kwargs):
         states = torch.from_numpy(states).float().reshape(1, -1, self.state_dim)[:, -self.seq_len:]
         actions = torch.from_numpy(actions).float().reshape(1, -1, self.action_dim)[:, -self.seq_len:]
         returns_to_go = torch.from_numpy(returns_to_go).float().reshape(1, -1, 1)[:, -self.seq_len:]
         timesteps = torch.from_numpy(timesteps).reshape(1, -1)[:, -self.seq_len:]
         
@@ -79,13 +85,15 @@
         mse_loss = torch.nn.functional.mse_loss(action_pred, actions.detach(), reduction="none")
         mse_loss = (mse_loss * masks.unsqueeze(-1)).mean()
         self.dt_optim.zero_grad()
         mse_loss.backward()
         if clip_grad is not None:
             torch.nn.utils.clip_grad_norm_(self.dt.parameters(), clip_grad)
         self.dt_optim.step()
+        self.dt_optim_scheduler.step()
         
         return {
             "loss/mse_loss": mse_loss.item(), 
+            "misc/learning_rate": self.dt_optim_scheduler.get_last_lr()[0]
         }
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/edac.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/edac.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,27 +14,35 @@
     Uncertainty-Based Offline Reinforcement Learning with Diversified Q-Ensemble <Ref: https://arxiv.org/abs/2110.01548>
     """
 
     def __init__(
         self,
         actor: BaseActor,
         critic: Critic,
-        actor_optim: optim.Optimizer,
-        critic_optim: optim.Optimizer,
         tau: float = 0.005,
         eta: float = 1.0,
         discount: float = 0.99,
         alpha: Union[float, Tuple[float, float]] = 0.2,
         do_reverse_update: bool = False,
         device: Union[str, torch.device] = "cpu"
     ) -> None:
-        super().__init__(actor, critic, actor_optim, critic_optim, tau, discount,
-                         alpha, do_reverse_update, device)
+        super().__init__(
+            actor, 
+            critic, 
+            tau, 
+            discount,
+            alpha, 
+            do_reverse_update, 
+            device
+        )
         self.eta = eta
 
+    def configure_optimizers(self, actor_lr, critic_lr):
+        return super().configure_optimizers(actor_lr, critic_lr)
+
     def _critic_loss(self, batch: Dict[str, torch.Tensor]) -> Tuple[Dict[str, torch.Tensor], Dict[str, float]]:
         critic_loss, critic_loss_metrics = super()._critic_loss(batch)
         obss, actions, next_obss, rewards, terminals = itemgetter("observations", "actions", "next_observations", "rewards", "terminals")(batch)
         ensemble_size = self.critic.ensemble_size
         assert (ensemble_size > 1)
         diversity_loss = None
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/inac.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/inac.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,42 +16,40 @@
     """
     def __init__(
         self, 
         actor: BaseActor, 
         behavior: BaseActor, 
         critic_q: Critic,
         critic_v: Critic,
-        actor_optim: torch.optim.Optimizer, 
-        behavior_optim: torch.optim.Optimizer,
-        critic_q_optim: torch.optim.Optimizer, 
-        critic_v_optim: torch.optim.Optimizer, 
         temperature: float = 0.01, 
         discount: float = 0.99, 
         tau: float = 5e-3, 
         adv_min: float = 1e-8, 
         adv_max: float = 1e4, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__()
         self.actor = actor
         self.behavior = behavior
         self.critic_q = critic_q
         self.critic_v = critic_v
         self.critic_q_target = make_target(critic_q)
-        self.actor_optim = actor_optim
-        self.critic_q_optim = critic_q_optim
-        self.critic_v_optim = critic_v_optim
-        self.behavior_optim = behavior_optim
         self._temperature = temperature
         self._tau = tau
         self._discount = discount
         self._adv_min = adv_min
         self._adv_max = adv_max
         
         self.to(device)
+
+    def configure_optimizers(self, actor_lr, critic_q_lr, critic_v_lr, behavior_lr):
+        self.actor_optim = torch.optim.Adam(self.actor.parameters(), lr=actor_lr)
+        self.critic_q_optim = torch.optim.Adam(self.critic_q.parameters(), lr=critic_q_lr)
+        self.critic_v_optim = torch.optim.Adam(self.critic_v.parameters(), lr=critic_v_lr)
+        self.behavior_optim = torch.optim.Adam(self.behavior.parameters(), lr=behavior_lr)
         
     @torch.no_grad()
     def select_action(
         self,
         obs: np.ndarray,
         deterministic: bool = False
     ) -> np.ndarray:
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/iql.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/iql.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,43 +18,45 @@
     """
 
     def __init__(
         self,
         actor: nn.Module,
         critic_q: nn.Module, 
         critic_v: nn.Module,
-        actor_optim: torch.optim.Optimizer,
-        critic_q_optim: torch.optim.Optimizer, 
-        critic_v_optim: torch.optim.Optimizer,
         expectile: float = 0.7,
         temperature: float = 3.0, 
         tau: float = 0.005,
         discount: float = 0.99,
         max_action: float = 1.0, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__()
 
         self.actor = actor
         self.critic_q = critic_q
         self.critic_q_old = make_target(self.critic_q)
         self.critic_v = critic_v
 
-        self.actor_optim = actor_optim
-        self.critic_q_optim = critic_q_optim
-        self.critic_v_optim = critic_v_optim
-
         self._max_action = max_action
         self._tau = tau
         self._discount = discount
         self._expectile = expectile
         self._temperature = temperature
         
         self.to(device)
     
+    def configure_optimizers(self, actor_lr, critic_v_lr, critic_q_lr, actor_opt_scheduler_steps=None):
+        self.actor_optim = torch.optim.Adam(self.actor.parameters(), lr=actor_lr)
+        self.critic_v_optim = torch.optim.Adam(self.critic_v.parameters(), lr=critic_v_lr)
+        self.critic_q_optim = torch.optim.Adam(self.critic_q.parameters(), lr=critic_q_lr)
+        if actor_opt_scheduler_steps is not None:
+            self.actor_lr_scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(self.actor_optim, actor_opt_scheduler_steps)
+        else:
+            self.actor_lr_scheduler = None
+    
     @torch.no_grad()
     def select_action(self, obs: np.ndarray, deterministic: bool = False) -> np.ndarray:
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
         action, *_ = self.actor.sample(obs, deterministic)
         return action.squeeze().cpu().numpy()
     
     def update(self, batch: Dict) -> Dict[str, float]:
@@ -93,14 +95,16 @@
         elif isinstance(self.actor, GaussianActor):
             policy_out = - self.actor.evaluate(obss, actions)[0]
         actor_loss = (exp_advanrage * policy_out).mean()
 
         self.actor_optim.zero_grad()
         actor_loss.backward()
         self.actor_optim.step()
+        if self.actor_lr_scheduler is not None:
+            self.actor_lr_scheduler.step()
 
         self._sync_weight()
 
         return {
             "loss/actor": actor_loss.item(),
             "loss/q": critic_q_loss.item(),
             "loss/v": critic_v_loss.item()
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/sac.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/sac.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,46 +16,48 @@
     Soft Actor Critic <Ref: https://arxiv.org/abs/1801.01290>
     """
 
     def __init__(
         self,
         actor: BaseActor,
         critic: Critic,
-        actor_optim: torch.optim.Optimizer,
-        critic_optim: torch.optim.Optimizer,
         tau: float = 0.005,
         discount: float = 0.99,
         alpha: Union[float, Tuple[float, float]] = 0.2,
+        target_update_freq: int=1, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__()
 
         self.actor = actor
         self.critic = critic
         self.critic_target = make_target(self.critic)
 
-        self.actor_optim = actor_optim
-        self.critic_optim = critic_optim
-
         self._is_auto_alpha = False
         if isinstance(alpha, tuple):
             self._is_auto_alpha = True
             target_entropy, alpha_lr = alpha
             self._log_alpha = nn.Parameter(torch.tensor([0.0], dtype=torch.float32, device=device), requires_grad=True)
             self._target_entropy = target_entropy
             self.alpha_optim = torch.optim.Adam([self._log_alpha], lr=alpha_lr)
             self._alpha = self._log_alpha.detach().exp()
         else:
             self._alpha = torch.tensor([alpha], dtype=torch.float32, device=device, requires_grad=False)
 
         self._tau = tau
         self._discount = discount
+        self._target_update_freq = target_update_freq
+        self._steps = 0
 
         self.to(device)
 
+    def configure_optimizers(self, actor_lr, critic_lr):
+        self.actor_optim = torch.optim.Adam(self.actor.parameters(), lr=actor_lr)
+        self.critic_optim = torch.optim.Adam(self.critic.parameters(), lr=critic_lr)
+
     @torch.no_grad()
     def select_action(
         self,
         obs: np.ndarray,
         deterministic: bool = False
     ) -> np.ndarray:
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
@@ -127,17 +129,19 @@
             alpha_loss.backward()
             self.alpha_optim.step()
             self._alpha = self._log_alpha.exp().detach()
         else:
             alpha_loss = 0
         metrics["misc/alpha"] = self._alpha.item()
 
-        self._sync_weight()
+        if self._steps % self._target_update_freq == 0:
+            self._sync_weight()
 
         # update info
+        self._steps += 1
         metrics.update({
             "loss/actor": actor_loss.item(),
             "loss/critic": critic_loss.item(),
             "loss/alpha": alpha_loss
         })
         return metrics
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/sacn.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/sacn.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 
 
 class SACNPolicy(SACPolicy):
     def __init__(
         self, 
         actor: BaseActor, 
         critic: Critic, 
-        actor_optim: nn.Module, 
-        critic_optim: nn.Module, 
         tau: float = 0.005, 
         discount: float = 0.99, 
         alpha: Union[float, Tuple[float, float]] = 0.2, 
         do_reverse_update: bool = False, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
-        super().__init__(actor, critic, actor_optim, critic_optim, tau, discount, alpha, device)
+        super().__init__(actor, critic, tau, discount, alpha, device)
         self.do_reverse_update = do_reverse_update
+
+    def configure_optimizers(self, actor_lr, critic_lr):
+        return super().configure_optimizers(actor_lr, critic_lr)
     
     def update(self, batch: Dict[str, torch.Tensor]) -> Dict[str, float]:
         if self.do_reverse_update:
             return self.reverse_update(batch)
         else:
             return super().update(batch)
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/td3.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/td3.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     Twin Delayed Deep Deterministic Policy Gradient <Ref: https://arxiv.org/abs/1802.09477>
     """
 
     def __init__(
         self,
         actor: BaseActor,
         critic: Critic, 
-        actor_optim: torch.optim.Optimizer,
-        critic_optim: torch.optim.Optimizer,
         actor_update_interval: int = 2, 
         policy_noise: float = 0.2, 
         noise_clip: float = 0.5,
         exploration_noise: Any = None, 
         tau: float = 0.005,
         discount: float = 0.99,
         max_action: float = 1.0, 
@@ -32,28 +30,30 @@
     ) -> None:
         super().__init__()
 
         self.actor = actor
         self.actor_target = make_target(self.actor)
         self.critic = critic
         self.critic_target = make_target(self.critic)
-        self.actor_optim = actor_optim
-        self.critic_optim = critic_optim
 
         self._tau = tau
         self._discount = discount
         self._actor_update_interval = actor_update_interval
         self._policy_noise = policy_noise
         self._noise_clip = noise_clip
         self._exploration_noise = exploration_noise
         self._max_action = max_action
 
         self._update_cnt = 0
         
         self.to(device)
+
+    def configure_optimizers(self, actor_lr, critic_lr):
+        self.actor_optim = torch.optim.Adam(self.actor.parameters(), lr=actor_lr)
+        self.critic_optim = torch.optim.Adam(self.critic.parameters(), lr=critic_lr)
         
     @torch.no_grad()
     def select_action(
         self, 
         obs: np.ndarray, 
         deterministic: bool=False
     ) -> np.ndarray:
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/td3bc.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/td3bc.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,40 +14,39 @@
     """
     TD3 with Behaviour Cloning <Ref: https://arxiv.org/pdf/2106.06860.pdf>
     """
     def __init__(
         self, 
         actor: BaseActor, 
         critic: Critic, 
-        actor_optim: torch.optim.Optimizer, 
-        critic_optim: torch.optim.Optimizer, 
         alpha: float = 0.2, 
         actor_update_interval: int = 2, 
         policy_noise: float = 0.2, 
         noise_clip: float = 0.5, 
         tau: float = 0.005, 
         discount: float = 0.99, 
         max_action: float = 1.0, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__(
             actor=actor, 
             critic=critic, 
-            actor_optim=actor_optim, 
-            critic_optim=critic_optim, 
             actor_update_interval=actor_update_interval, 
             policy_noise=policy_noise, 
             noise_clip=noise_clip, 
             exploration_noise=None, 
             tau=tau, 
             discount=discount, 
             max_action=max_action, 
             device=device
         )
         self.alpha = alpha
+
+    def configure_optimizers(self, actor_lr, critic_lr):
+        return super().configure_optimizers(actor_lr, critic_lr)
         
     def actor_loss(self, batch: Dict[str, Any]) -> Tuple[torch.Tensor, Dict[str, Any]]:
         obss, actions = itemgetter("observations", "actions")(batch)
         new_actions, *_ = self.actor.sample(obss)
         new_q1 = self.critic(obss, new_actions)[0, ...]
         bc_loss = F.mse_loss(new_actions, actions)
         q_loss = -self.alpha / (new_q1.abs().mean().detach()) * new_q1.mean()
```

### Comparing `offlinerllib-0.0.6/offlinerllib/policy/model_free/xql.py` & `offlinerllib-0.0.7/offlinerllib/policy/model_free/xql.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from operator import itemgetter
 from typing import Dict, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from offlinerllib.module.actor import DeterministicActor, GaussianActor
+from offlinerllib.module.actor import DeterministicActor, GaussianActor, CategoricalActor
 from offlinerllib.policy import BasePolicy
 from offlinerllib.utils.functional import gumbel_log_loss, gumbel_rescale_loss
 from offlinerllib.utils.misc import convert_to_tensor, make_target
 
 
 class XQLPolicy(BasePolicy):
     """
@@ -17,50 +17,54 @@
     """
     
     def __init__(
         self, 
         actor: nn.Module, 
         critic_q: nn.Module, 
         critic_v: nn.Module, 
-        actor_optim: torch.optim.Optimizer, 
-        critic_q_optim: torch.optim.Optimizer, 
-        critic_v_optim: torch.optim.Optimizer, 
         num_v_update: int=1, 
         scale_random_sample: int=0, 
         loss_temperature: float=1.0, 
         aw_temperature: float=0.1, 
         use_log_loss: bool=False, 
         noise_std: float=0,
         tau: float = 0.005, 
         discount: float = 0.99, 
         max_action: float = 1.0, 
+        max_clip: float = 1.0, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
         super().__init__()
         self.actor = actor
         self.critic_q = critic_q
         self.critic_q_target = make_target(self.critic_q)
         self.critic_v = critic_v
         
-        self.actor_optim = actor_optim
-        self.critic_q_optim = critic_q_optim
-        self.critic_v_optim = critic_v_optim
-        
         self.num_v_update = num_v_update
         self.scale_random_sample = scale_random_sample
         
         self.tau = tau
         self.discount = discount
         self.loss_temperature = loss_temperature
         self.aw_temperature = aw_temperature
         self.use_log_loss = use_log_loss
         self.max_action = max_action
+        self.max_clip = max_clip
         self.noise_std = noise_std
 
         self.to(device)
+        
+    def configure_optimizers(self, actor_lr, critic_v_lr, critic_q_lr, actor_opt_scheduler_steps=None):
+        self.actor_optim = torch.optim.Adam(self.actor.parameters(), lr=actor_lr)
+        self.critic_v_optim = torch.optim.Adam(self.critic_v.parameters(), lr=critic_v_lr)
+        self.critic_q_optim = torch.optim.Adam(self.critic_q.parameters(), lr=critic_q_lr)
+        if actor_opt_scheduler_steps is not None:
+            self.actor_lr_scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(self.actor_optim, actor_opt_scheduler_steps)
+        else:
+            self.actor_lr_scheduler = None
 
     @torch.no_grad()   
     def select_action(self, obs: np.ndarray, deterministic: bool=False):
         obs = torch.from_numpy(obs).float().unsqueeze(0).to(self.device)
         action, *_ = self.actor.sample(obs, deterministic)
         return action.squeeze().cpu().numpy()
         
@@ -83,36 +87,39 @@
                 noise = (torch.randn_like(v_actions)*self.noise_std).clamp(-0.5*self.max_action, 0.5*self.max_action)
                 v_actions = (v_actions + noise).clamp(-self.max_action, self.max_action)
                 
             with torch.no_grad():
                 q = self.critic_q_target(v_obss, v_actions)
             v = self.critic_v(v_obss)
             if self.use_log_loss:
-                value_loss = gumbel_log_loss(v, q, alpha=self.loss_temperature).mean()
+                value_loss = gumbel_log_loss(v, q, alpha=self.loss_temperature, clip_max=self.max_clip).mean()
             else:
-                value_loss = gumbel_rescale_loss(v, q, alpha=self.loss_temperature).mean()
+                value_loss = gumbel_rescale_loss(v, q, alpha=self.loss_temperature, clip_max=self.max_clip).mean()
+            clip_ratio = (((q-v)/self.loss_temperature) > self.max_clip).float().mean().item()
             self.critic_v_optim.zero_grad()
             value_loss.backward()
             self.critic_v_optim.step()
             v_loss_value += value_loss.detach().cpu().item()
         v_loss_value /= self.num_v_update
             
         # update actor network
         with torch.no_grad():
             v = self.critic_v(obss)
             q = self.critic_q_target(obss, actions)
             exp_advantage = torch.exp((q-v)*self.aw_temperature).clamp(max=100.0)
         if isinstance(self.actor, DeterministicActor):
             policy_out = torch.sum((self.actor.sample(obss)[0] - actions)**2, dim=1)
-        elif isinstance(self.actor, GaussianActor):
+        elif isinstance(self.actor, (GaussianActor, CategoricalActor)):
             policy_out = - self.actor.evaluate(obss, actions)[0]
         actor_loss = (exp_advantage * policy_out).mean()
         self.actor_optim.zero_grad()
         actor_loss.backward()
         self.actor_optim.step()
+        if self.actor_lr_scheduler is not None:
+            self.actor_lr_scheduler.step()
         actor_loss_value = actor_loss.detach().cpu().item()
         
         # update q network
         with torch.no_grad():
             next_v = self.critic_v(next_obss)
             target_q = rewards + self.discount * (1-terminals) * next_v
         q = self.critic_q(obss, actions, reduce=False)
@@ -123,14 +130,15 @@
         q_loss_value = q_loss.detach().cpu().item()
         
         self._sync_weight()
         
         return {
             "loss/q_loss": q_loss_value, 
             "loss/actor_loss": actor_loss_value, 
-            "loss/v_loss": v_loss_value
+            "loss/v_loss": v_loss_value, 
+            "misc/clip_ratio": clip_ratio
         }
                 
     def _sync_weight(self) -> None:
         for o, n in zip(self.critic_q_target.parameters(), self.critic_q.parameters()):
             o.data.copy_(o.data * (1.0 - self.tau) + n.data * self.tau)
```

### Comparing `offlinerllib-0.0.6/offlinerllib.egg-info/PKG-INFO` & `offlinerllib-0.0.7/offlinerllib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.6/offlinerllib.egg-info/SOURCES.txt` & `offlinerllib-0.0.7/offlinerllib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 offlinerllib.egg-info/SOURCES.txt
 offlinerllib.egg-info/dependency_links.txt
 offlinerllib.egg-info/requires.txt
 offlinerllib.egg-info/top_level.txt
 offlinerllib/buffer/__init__.py
 offlinerllib/buffer/base.py
 offlinerllib/buffer/d4rl_buffer.py
+offlinerllib/env/__init__.py
+offlinerllib/env/d4rl.py
+offlinerllib/env/mixed.py
 offlinerllib/module/__init__.py
 offlinerllib/module/actor.py
 offlinerllib/module/critic.py
 offlinerllib/module/net/__init__.py
 offlinerllib/module/net/basic.py
 offlinerllib/module/net/mlp.py
 offlinerllib/policy/__init__.py
 offlinerllib/policy/base.py
 offlinerllib/policy/model_free/__init__.py
 offlinerllib/policy/model_free/awac.py
-offlinerllib/policy/model_free/bppo.py
 offlinerllib/policy/model_free/dt.py
 offlinerllib/policy/model_free/edac.py
 offlinerllib/policy/model_free/inac.py
 offlinerllib/policy/model_free/iql.py
 offlinerllib/policy/model_free/sac.py
 offlinerllib/policy/model_free/sacn.py
 offlinerllib/policy/model_free/td3.py
 offlinerllib/policy/model_free/td3bc.py
-offlinerllib/policy/model_free/xql.py
+offlinerllib/policy/model_free/xql.py
+offlinerllib/policy/model_free/xsac.py
```

### Comparing `offlinerllib-0.0.6/setup.py` & `offlinerllib-0.0.7/setup.py`

 * *Files identical despite different names*

