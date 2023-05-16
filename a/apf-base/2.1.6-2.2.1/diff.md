# Comparing `tmp/apf_base-2.1.6.tar.gz` & `tmp/apf_base-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-zkh9oaqp/apf_base-2.1.6.tar", last modified: Tue May  2 21:09:17 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-3eop47oz/apf_base-2.2.1.tar", last modified: Tue May 16 22:51:12 2023, max compression
```

## Comparing `apf_base-2.1.6.tar` & `apf_base-2.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-02 21:08:24.000000 apf_base-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-02 21:09:17.000000 apf_base-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-02 21:08:24.000000 apf_base-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 21:08:24.000000 apf_base-2.1.6/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:09:17.000000 apf_base-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 21:08:24.000000 apf_base-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 22:50:42.000000 apf_base-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-16 22:51:12.000000 apf_base-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-16 22:50:42.000000 apf_base-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-16 22:50:42.000000 apf_base-2.2.1/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 22:51:12.000000 apf_base-2.2.1/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:51:12.000000 apf_base-2.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 22:50:42.000000 apf_base-2.2.1/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:51:12.000000 apf_base-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-16 22:50:42.000000 apf_base-2.2.1/setup.py
```

### Comparing `apf_base-2.1.6/LICENSE` & `apf_base-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/PKG-INFO` & `apf_base-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.1.6
+Version: 2.2.1
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.1.6/README.md` & `apf_base-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/consumers/avro_file.py` & `apf_base-2.2.1/apf/consumers/avro_file.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/consumers/csv.py` & `apf_base-2.2.1/apf/consumers/csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,22 +24,29 @@
     Parameters
     ----------
     FILE_PATH: path
         CSV path location
 
     OTHER_ARGS: dict
         Parameters passed to :func:`pandas.read_csv`
-        (reference `here <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_)
+        (reference `pandas documentation <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_)
 
     """
 
     def __init__(self, config):
         super().__init__(config)
         path = self.config.get("FILE_PATH", None)
         if path is None:
             raise Exception("FILE_PATH variable not set")
 
     def consume(self):
+        """Get a message from a csv file
+
+        Yields
+        ------
+        dict
+            Dictionary like message of an alert.
+        """
         df = pd.read_csv(self.config["FILE_PATH"], **self.config.get("OTHER_ARGS", {}))
         self.len = len(df)
         for index, row in df.iterrows():
             yield row.to_dict()
```

### Comparing `apf_base-2.1.6/apf/consumers/generic.py` & `apf_base-2.2.1/apf/consumers/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.config = config
 
     @abstractmethod
     def consume(self) -> Generator[Union[list, dict], None, None]:
         """Get a message from a data source
 
         Yields
-        -------
+        ------
         dict
             Dictionary like message of an alert.
         """
         yield {}
 
     def commit(self):
         """Post consume processing.
```

### Comparing `apf_base-2.1.6/apf/consumers/json.py` & `apf_base-2.2.1/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/consumers/kafka.py` & `apf_base-2.2.1/apf/consumers/kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         STEP_CONFIG = { ...
             "COMMIT": False #Disable commit
             #useful for testing/debugging.
         }
 
 
     Parameters
-    -----------
+    ----------
 
     TOPICS: list
 
         List of topics to consume.
 
         **Example:**
 
@@ -110,16 +110,17 @@
                     "group.id": "step_group",
                     'security.protocol': 'SSL',
                     'ssl.ca.location': '<ca-cert path>',
                     'ssl.keystore.location': '<keystore path>',
                     'ssl.keystore.password': '<keystore password>'
                 }
             }
+
         all supported `confluent_kafka` parameters can be found
-        `here <https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md>`_
+        `on the official library documentation <https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md>`_
     """
 
     consumer: Consumer
 
     def __init__(self, config):
         super().__init__(config)
         # Disable auto commit
@@ -200,15 +201,15 @@
         Will return a dictionary or a list, depending on the number of messages consumed.
 
         If num_messages > 1 then it returns list.
 
         If num_messages = 1 then it returns dict.
 
         Parameters
-        --------------
+        ----------
         num_messages: int
             Number of messages to be consumed
         timeout: int
             Seconds to wait when consuming messages. Raises exception if doesn't get the messages after
             specified time
         """
         num_messages, timeout = self.set_basic_config(num_messages, timeout)
```

### Comparing `apf_base-2.1.6/apf/core/__init__.py` & `apf_base-2.2.1/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/core/management/helpers.py` & `apf_base-2.2.1/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/core/secret_manager.py` & `apf_base-2.2.1/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/core/step.py` & `apf_base-2.2.1/apf/core/step.py`

 * *Files 10% similar despite different names*

```diff
@@ -160,14 +160,17 @@
             self.metrics_sender.send_metrics(metrics)
 
     def _pre_consume(self):
         self.logger.info("Starting step. Begin processing")
         self.pre_consume()
 
     def pre_consume(self):
+        """
+        Override this method to perform operations before the first message arrives.
+        """
         pass
 
     def _pre_execute(self, message: Union[dict, List[dict]]):
         self.logger.info("Received message. Begin preprocessing")
         self.metrics["timestamp_received"] = datetime.datetime.now(
             datetime.timezone.utc
         )
@@ -186,14 +189,21 @@
             # if tid:
             #     tid = str(tid).upper()
             #     self.prometheus_metrics.telescope_id.state(tid)
         preprocessed = self.pre_execute(self.message)
         return preprocessed
 
     def pre_execute(self, messages: List[dict]):
+        """
+        Override this method to perform operations on each batch of messages consumed.
+
+        Typically this method is used for pre processing operations such as parsing,
+        formatting and overall preparation for the execute method that handles
+        all the complex logic applied to the messages.
+        """
         return messages
 
     @abstractmethod
     def execute(
         self, messages: List[dict]
     ) -> Union[Iterable[Dict[str, Any]], Dict[str, Any]]:
         """Execute the logic of the step. This method has to be implemented by
@@ -224,31 +234,52 @@
             self.prometheus_metrics.processed_messages.observe(1)
         if isinstance(self.message, list):
             self.prometheus_metrics.processed_messages.observe(len(self.message))
         self.prometheus_metrics.execution_time.observe(time_difference.total_seconds())
         return final_result
 
     def post_execute(self, result: Union[Iterable[Dict[str, Any]], Dict[str, Any]]):
+        """
+        Override this method to perform additional operations on
+        the processed data coming from :py:func:`apf.core.step.GenericStep.execute`
+        method.
+
+        Typically used to do post processing, parsing, output formatting, etc.
+        """
         return result
 
     def _pre_produce(
         self, result: Union[Iterable[Dict[str, Any]], Dict[str, Any]]
     ) -> Union[Iterable[Dict[str, Any]], Dict[str, Any]]:
         self.logger.info("Finished all processing. Begin message production")
         message_to_produce = self.pre_produce(result)
         return message_to_produce
 
     def pre_produce(self, result: Union[Iterable[Dict[str, Any]], Dict[str, Any]]):
+        """
+        Override this method to perform additional operations on
+        the processed data coming from :py:func:`apf.core.step.GenericStep.post_execute`
+        method.
+
+        Typically used to format data output as described in the step producer's Schema
+        """
         return result
 
     def _post_produce(self):
         self.logger.info("Messages produced. Begin post production")
         self.post_produce()
 
     def post_produce(self):
+        """
+        Override this method to perform operations after data has been
+        produced by the producer.
+
+        You can use this lifecycle method to perform cleanup, send additional metrics,
+        notifications, etc.
+        """
         pass
 
     def get_value(self, message, params):
         """Get values from a massage and process it to create a new metric.
 
         Parameters
         ----------
@@ -383,8 +414,18 @@
         self._write_success()
 
     def _write_success(self):
         f = open("__SUCCESS__", "w")
         f.close()
 
     def tear_down(self):
+        """
+        Override this method to perform operations after the consumer
+        has stopped consuming data.
+
+        This method is called only once after processing messages and right before
+        the start method ends.
+
+        You can use this lifecycle method to perform cleanup, send additional metrics,
+        notifications, etc.
+        """
         pass
```

### Comparing `apf_base-2.1.6/apf/core/templates/step/package/step.py` & `apf_base-2.2.1/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.2.1/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/core/topic_management.py` & `apf_base-2.2.1/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/metrics/generic.py` & `apf_base-2.2.1/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/metrics/kafka.py` & `apf_base-2.2.1/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/metrics/log.py` & `apf_base-2.2.1/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/metrics/prometheus/prometheus.py` & `apf_base-2.2.1/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/producers/csv.py` & `apf_base-2.2.1/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/producers/generic.py` & `apf_base-2.2.1/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/producers/json_prod.py` & `apf_base-2.2.1/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf/producers/kafka.py` & `apf_base-2.2.1/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/apf_base.egg-info/PKG-INFO` & `apf_base-2.2.1/apf_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.1.6
+Version: 2.2.1
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.1.6/apf_base.egg-info/SOURCES.txt` & `apf_base-2.2.1/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.6/setup.py` & `apf_base-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.1.6",
+    version="2.2.1",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

