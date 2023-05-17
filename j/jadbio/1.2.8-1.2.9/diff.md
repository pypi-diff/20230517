# Comparing `tmp/jadbio-1.2.8.tar.gz` & `tmp/jadbio-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadbio-1.2.8.tar", last modified: Thu Mar  2 10:34:14 2023, max compression
+gzip compressed data, was "jadbio-1.2.9.tar", last modified: Wed May 17 08:54:40 2023, max compression
```

## Comparing `jadbio-1.2.8.tar` & `jadbio-1.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-03-02 10:34:14.711225 jadbio-1.2.8/
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)    35149 2023-03-02 10:34:07.000000 jadbio-1.2.8/LICENSE
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1574 2023-03-02 10:34:14.711225 jadbio-1.2.8/PKG-INFO
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)     2169 2023-03-02 10:34:07.000000 jadbio-1.2.8/README.md
-drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-03-02 10:34:14.710225 jadbio-1.2.8/jadbio/
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)       22 2023-03-02 10:34:07.000000 jadbio-1.2.8/jadbio/__init__.py
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)    86717 2023-03-02 10:34:07.000000 jadbio-1.2.8/jadbio/client.py
-drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-03-02 10:34:14.711225 jadbio-1.2.8/jadbio.egg-info/
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1574 2023-03-02 10:34:14.000000 jadbio-1.2.8/jadbio.egg-info/PKG-INFO
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)      236 2023-03-02 10:34:14.000000 jadbio-1.2.8/jadbio.egg-info/SOURCES.txt
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)        1 2023-03-02 10:34:14.000000 jadbio-1.2.8/jadbio.egg-info/dependency_links.txt
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)      100 2023-03-02 10:34:14.000000 jadbio-1.2.8/jadbio.egg-info/requires.txt
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)        7 2023-03-02 10:34:14.000000 jadbio-1.2.8/jadbio.egg-info/top_level.txt
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)      107 2023-03-02 10:34:07.000000 jadbio-1.2.8/pyproject.toml
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)      948 2023-03-02 10:34:14.711225 jadbio-1.2.8/setup.cfg
--rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1159 2023-03-02 10:34:07.000000 jadbio-1.2.8/setup.py
+drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-05-17 08:54:40.259869 jadbio-1.2.9/
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)    35149 2023-05-17 08:54:33.000000 jadbio-1.2.9/LICENSE
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1574 2023-05-17 08:54:40.259869 jadbio-1.2.9/PKG-INFO
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)     2169 2023-05-17 08:54:33.000000 jadbio-1.2.9/README.md
+drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-05-17 08:54:40.258869 jadbio-1.2.9/jadbio/
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)       22 2023-05-17 08:54:33.000000 jadbio-1.2.9/jadbio/__init__.py
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)    87589 2023-05-17 08:54:33.000000 jadbio-1.2.9/jadbio/client.py
+drwxr-xr-x   0 jadbio    (1000) jadbio    (1000)        0 2023-05-17 08:54:40.259869 jadbio-1.2.9/jadbio.egg-info/
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1574 2023-05-17 08:54:40.000000 jadbio-1.2.9/jadbio.egg-info/PKG-INFO
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)      236 2023-05-17 08:54:40.000000 jadbio-1.2.9/jadbio.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)        1 2023-05-17 08:54:40.000000 jadbio-1.2.9/jadbio.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)      100 2023-05-17 08:54:40.000000 jadbio-1.2.9/jadbio.egg-info/requires.txt
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)        7 2023-05-17 08:54:40.000000 jadbio-1.2.9/jadbio.egg-info/top_level.txt
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)      107 2023-05-17 08:54:33.000000 jadbio-1.2.9/pyproject.toml
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)      948 2023-05-17 08:54:40.259869 jadbio-1.2.9/setup.cfg
+-rw-r--r--   0 jadbio    (1000) jadbio    (1000)     1159 2023-05-17 08:54:33.000000 jadbio-1.2.9/setup.py
```

### Comparing `jadbio-1.2.8/LICENSE` & `jadbio-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jadbio-1.2.8/PKG-INFO` & `jadbio-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jadbio
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python wrapper for the public JADBio REST API.
 Home-page: https://github.com/JADBio/JADBioPythonClient
 Author: JADBio
 Author-email: support@jadbio.com
 License: GPL3.0
 Project-URL: Homepage, https://jadbio.com
-Project-URL: Documentation, https://support.jadbio.com/pythonclient/1.2.8
+Project-URL: Documentation, https://support.jadbio.com/pythonclient/1.2.9
 Project-URL: Source code, https://github.com/JADBio/JADBioPythonClient
 Keywords: jadbio automl machine-learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jadbio-1.2.8/README.md` & `jadbio-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `jadbio-1.2.8/jadbio/client.py` & `jadbio-1.2.9/jadbio/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import ntpath
 
 import requests
 from requests import Session
+from requests.adapters import HTTPAdapter
+from urllib3 import Retry
 from requests_toolbelt import MultipartEncoder
 from typing import List, Tuple
 
 API_VERSION = 'v1'
 
-
 class RequestFailed(Exception):
     pass
 
 
 class JadRequestResponseError(Exception):
     """
     Exception raised when sth goes wrong with a request
@@ -69,16 +70,15 @@
             self.__session.close()
             self.logout()
         except:
             pass
 
     def get_version(self):
         """
-        Provides access to the full version number of the currently deployed API.
-        The major version number is always implied by the request URL.
+        Returns the full version number of the currently deployed API.
 
         :return: public api version
         :rtype: str
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
 
@@ -87,14 +87,33 @@
         1.0-beta
         """
 
         url = self.__base_url + 'version'
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get Version')['version']
 
+    def get_jadbio_version(self):
+        """
+        Returns the full version number of the currently deployed JADBio.
+
+        :return: JADBio version
+        :rtype: str
+        :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
+
+        :Example:
+
+        >>> client = JadbioClient('juser@gmail.com', 'a password')
+        >>> print(client.get_jadbio_version())
+        1.4.101
+        """
+
+        url = self.__base_url + 'version'
+        ret = self.__session.get(url, headers=self.__token)
+        return JadbioClient.__parse_response__(ret, 'Get Version')['jadbioVersion']
+
     def login(self, username: str, password: str):
         """
         Login user, and store credentials in current session (previous credentials if any, are overwritten).
         Creates a session in the current client instance.
 
         :param str username: Jad account username or email.
         :param str password: Jad account password.
@@ -104,14 +123,26 @@
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
         >>> client.login('anothermail@gmail.com', 'another password')
         """
 
         self.__session = Session()
 
+        # Enable retries to avoid common HTTP errors.
+        # The delay between retries is defined as: backoff_factor * [0s, 2s, 4s, 8s, 16s, ...].
+        #
+        # See https://stackoverflow.com/a/35504626 for more details.
+        adapter = HTTPAdapter(max_retries = Retry(
+            total = 5, 
+            backoff_factor = 0.2,
+            status_forcelist = [500, 502, 503, 504]
+        ))
+        self.__session.mount("http://", adapter)
+        self.__session.mount("https://", adapter)
+
         url = self.__base_url + 'login'
         loginRequest = {'usernameOrEmail': username, 'password': password}
         res = self.__session.post(url, json=loginRequest)
 
         login = JadbioClient.__parse_response__(res, 'Login')
 
         self.__token = {'Authorization': ' '.join(['Bearer', login['token']])}
@@ -156,15 +187,15 @@
             JadbioClient.__parse_response__(res,
                                             'Create project')['projectId'])
 
     def get_project(self, project_id: str):
         """
         Returns a project.
 
-        :param str project_id: identifies the project to which the user must have read access.
+        :param str project_id: The id of the project. The user must have read permissions to the project.
         :return: { projectId: string, name: string, description?: string }
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
@@ -174,25 +205,23 @@
 
         url = self.__base_url + 'project/{}'.format(project_id)
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get project')
 
     def get_projects(self, offset: int = 0, count: int = 10):
         """
-        Projects form an ordered list from which the request extracts the sublist starting at offset and containing at
-        most count elements.
+        Returns a sublist of projects of a user.
 
-        :param int offset: project list offset.
-        :param int count: max number of projects to get.
+        :param int offset: Project list offset. The first element starts at offset 0.
+        :param int count: Limit on the number of projects to return. No limit is applied if count is negative.
         :return: {offset: number, totalCount: number, data: [{ projectId: string, name: string, description?: string }]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
-        The list uses zero-based indexing, meaning the first element is at offset 0.
-        Constraints: Both offset and count must be non-negative integers and count can be at most 100.
+        Constraints: Offset must be a non-negative integer.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
         >>> client.get_projects()
         {'offset': 0, 'totalCount': 1,
             'data': [{'projectId': '462', 'name': 'test'}]}
@@ -203,15 +232,15 @@
         return JadbioClient.__parse_response__(ret, 'Get projects')
 
     def delete_project(self, project_id: str):
         """
         Allows clients to delete a specified project.
         **Beware** This operation silently deletes all contained datasets, analyses and models used inside that project.
 
-        :param str project_id: Identifies the project. It must be owned by the user.
+        :param str project_id: The id of the project. It must be owned by the user.
         :return: { projectId: string, name: string, description?: string }
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
@@ -298,15 +327,16 @@
                        has_sample_headers: bool = True,
                        description: str = ''):
         """
         Create a dataset from an uploaded file.
 
         :param str name: Name of the dataset (must have at least 3 and at most 60 characters and must be unique within
             the target project).
-        :param str project_id: Id of the project to which the dataset will be created.
+        :param str project_id: The id of the project. The dataset will be added to this project. 
+            The user must have write permissions to the project.
         :param int file_id: Id provided by the client when the file was uploaded.
         :param int file_size_in_bytes: must match the actual size of the uploaded file.
             (e.g. len(open("pth/to/file.csv",'r').read()))
         :param str separator: specifies the characters used to separate values in the file.
         :param bool has_samples_in_rows: must be true iff rows of the uploaded file correspond to samples.
         :param bool has_feature_headers_name: True if dataset contains feature names.
         :param bool has_sample_headers: True if dataset contains sample names.
@@ -368,16 +398,16 @@
 
     def attach_dataset(self, name: str, project_id: str, dataset_id: str):
         """
         Attach a dataset from another project, to a destination project.
 
         :param str name: Used to name the new dataset. It must have at least 3 and at most 60 characters and must
             be unique within the target project.
-        :param str project_id: The destination project where the specified dataset will be attached to. The user should
-            have read and write permissions for that project.
+        :param str project_id: The id of the project. The dataset will be attached to this project. 
+            The user must have write permissions to the project.
         :param str dataset_id:  Identifies the source dataset. It must belong to a project to which the user has read
             permissions.
         :return: {datasetId: string, projectId: string, name: string, description?: string, sampleCount: number,
             featureCount: number, sizeInBytes: number}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
@@ -391,35 +421,31 @@
 
         url = self.__base_url + 'dataset/{}/attachToProject/{}'.format(dataset_id, project_id)
         ret = self.__session.post(url, data=name, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Attach dataset')
 
     def get_datasets(self, project_id: str, offset: int = 0, count: int = 10):
         """
-        The projectId identifies the project to which the user must have read permissions.
-        Datasets form an ordered list from which the request extracts the sublist starting at offset and containing at
-        most count elements.
-        The list uses zero-based indexing, meaning the first element is at offset 0.
-
-        :param str project_id: Id of the project to get datasets from.
-        :param int offset: Start index.
-        :param int count: Number of datasets to retrieve.
+        Returns a sublist of datasets contained in a project.
+
+        :param str project_id: The id of the project. The user must have read permissions to the project.
+        :param int offset: Dataset list offset. The first element starts at offset 0.
+        :param int count: Limit on the number of datasets to analysis. No limit is applied if count is negative.
         :return: { projectId: string, offset: number, totalCount: number,\
             data: [{projectId: string,
                 datasetId: string,
                 name: string,
                 description?: string,
                 sampleCount: number,
                 featureCount: number,
                 sizeInBytes: number}]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
-        The list uses zero-based indexing, meaning the first element is at offset 0.
-        Constraints: Both offset and count must be non-negative integers and count can be at most 100.
+        Constraints: Offset must be a non-negative integer.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
         >>> client.get_datasets('462')
         {'projectId': '462', 'offset': 0, 'totalCount': 2, 'data': [
                 {'projectId': '462', 'datasetId': '6065', 'name': 'file',
@@ -1074,16 +1100,15 @@
         return JadbioClient.__parse_response__(
             ret, 'Get Extra FS')['extraFeatureSelectors']
 
     def get_analysis(self, analysis_id: str):
         """
         Returns an analysis.
 
-        :param str analysis_id: Identifies the analysis which must belong to a project to which the user must
-            have read access.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :return: {analysisId: string, projectId: string, parameters: object, state: string}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
@@ -1107,28 +1132,25 @@
 
         url = self.__base_url + 'analysis/{}'.format(analysis_id)
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get analysis')
 
     def get_analyses(self, project_id: str, offset: int = 0, count: int = 10):
         """
-        Returns a sublist of all analyses in a project.
+        Returns a sublist of analyses contained in a project.
 
-        :param str project_id: Identifies the project to which the user must have read permission.
-        :param int offset: Request extracts the sublist starting at offset.
-        :param int count: max number of analyses to get.
+        :param str project_id: The id of the project. The user must have read permissions to the project.
+        :param int offset: Analysis list offset. The first element starts at offset 0.
+        :param int count: Limit on the number of analyses to analysis. No limit is applied if count is negative.
         :return: {projectId: string, offset: number, totalCount: number, \
             data: [{analysisId: string, parameters: object, state: string}]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
-        The list uses zero-based indexing, meaning the first element is at offset 0.
-        Constraints: Both offset and count must be non-negative integers and count can be at most 100.
-        The parameters object has the same fields as specified when each analysis was created,
-        including the dataset identifier and optional values.
+        Constraints: Offset must be a non-negative integer.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
         >>> client.get_analyses('462')
         {'projectId': '462', 'offset': 0, 'totalCount': 1, 'data': [{
             'analysisId': '5219',
@@ -1151,16 +1173,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get analyses')
 
     def get_analysis_status(self, analysis_id: str):
         """
         Returns the status of an analysis.
 
-        :param str analysis_id: Identifies the analysis. It must belong to a project to which the user has read
-            permissions.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :return: {analysisId: string, parameters: object, state: string, startTime?: timestamp, \
             executionTimeInSeconds?: number, progress?: number}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The nested parameters object has the same fields as specified when the analysis was created,
         including the dataset identifier and optional values.
@@ -1191,15 +1212,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get analysis status')
 
     def get_analysis_result(self, analysis_id: str):
         """
         Returns the result of a finished analysis.
 
-        :param str analysis_id: Identifies the analysis.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :return: {analysisId: string, parameters: object, mlEngine: string, startTime: timestamp,\
             executionTimeInSeconds: number, models: { model_key1?: model1, model_key2?: model2}}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The nested parameters object has the same fields as specified when the analysis was created,
         including the identity of the dataset and optional values.
@@ -1266,15 +1287,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get analysis result')
 
     def download_analysis_model_predictions(self, analysis_id: str, model_id: str):
         """
         Returns the out-of-sample predictions for the specified model of a finished analysis.
 
-        :param str analysis_id: Identifies the analysis.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :param str model_id: Identifies the model.
         :return: {analysisId: string, parameters: object, mlEngine: string, startTime: timestamp,\
             executionTimeInSeconds: number, models: { model_key1?: model1, model_key2?: model2}}
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
 
@@ -1288,16 +1309,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get analysis model predictions')
 
     def delete_analysis(self, analysis_id: str):
         """
         Allows clients to delete a specified analysis.
 
-        :param str analysis_id: Identifies the analysis. It must belong to a project to which the user has
-            write permissions.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :return: {analysisId: string, parameters: object, state: string}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The parameters object has the same fields as specified when each analysis was created,
         including the dataset identifier and optional values.
 
@@ -1323,15 +1343,15 @@
         ret = self.__session.post(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Delete analysis')
 
     def available_plots(self, analysis_id: str, model_key: str):
         """
         Retrieves the plot names of the computed plots for a given model in an analysis.
 
-        :param str analysis_id: Identifies the analysis.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :param str model_key: A key present in analysis_result['models'] (e.g. 'best' or 'interpretable')
         :return: {analysisId: string, modelKey: string, plots: string[]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The analysisId, modelKey is the same as in the request. The plots array contains the plot names that are
         available for the current modelKey.
@@ -1349,15 +1369,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Available analysis')
 
     def get_plot(self, analysis_id: str, model_key: str, plot_key: str):
         """
         Retrieves the raw values of a plot for a modelKey - analysis pair.
 
-        :param str analysis_id: Identifies the analysis.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :param str model_key: A key present in analysis_result['models'] (e.g. 'best' or 'interpretable')
         :param str plot_key: A key present in available_plots['plots'] (e.g. 'Feature Importance')
         :return: {analysis_id: string, modelKey: string, plot: {plot_key: object}}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The analysisId, model_key are the same as in the request. The plot object contains the raw values of the
@@ -1387,15 +1407,15 @@
         ret = self.__session.get(url, headers=self.__token)
         return JadbioClient.__parse_response__(ret, 'Get plot')
 
     def get_plots(self, analysis_id: str, model_key: str):
         """
         Retrieves the raw values of all the available plots for a modelKey - analysis pair.
 
-        :param str analysis_id: Identifies the analysis.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
         :param str model_key: A key present in analysis_result['models'] (e.g. 'best' or 'interpretable')
         :return: {analysis_id: string, model_key: string, plots: {plot_key: object}[]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         The analysisId, model_key are the same as in the request. The plots array contains the raw values of plot
         objects per plotKey present in the request.
@@ -1434,17 +1454,16 @@
                         model_key: str,
                         signature_index: int = 0):
         """
         Launches a task that predicts outcome for an unlabeled dataset using a model found by a finished analysis.
         (User must have read and execute permissions to the project that contains the analysis and the dataset to be
         predicted.)
 
-        :param str analysis_id: Identifies the analysis, must belong to the same project as the dataset_id.
-        :param str dataset_id: Identifies a dataset containing unlabeled data, must belong to the same project as
-            analysis_id.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project
+        :param str dataset_id: The id of the dataset to predict. This must belong to the same project as the analysis.
         :param str model_key: A key present in analysis_result['models'] (e.g. 'best' or 'interpretable')
         :param int signature_index: zero-based index of the model signature to use for the predictions.
         :return: predictionId
         :rtype: str
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
         :Example:
@@ -1473,15 +1492,15 @@
                               model_key: str,
                               signature_index: int = 0):
         """
         Launches a task that predicts outcome for an unlabeled dataset using a model found by a finished analysis.
         (User must have read and execute permissions to the project that contains the analysis and the dataset to be
         predicted.)
 
-        :param str analysis_id: Identifies the analysis, must belong to the same project as the dataset_id.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project
         :param str dataset_id: Identifies a dataset containing unlabeled data, must belong to the same project as
             analysis_id.
         :param str model_key: A key present in analysis_result['models'] (e.g. 'best' or 'interpretable')
         :param int signature_index: zero-based index of the model signature to use for the predictions.
         :return: {errors?: [string], warnings?: [string], suggestions?: [string]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
@@ -1537,27 +1556,25 @@
         return JadbioClient.__parse_response__(ret, 'Get prediction')
 
     def get_predictions(self,
                         analysis_id: str,
                         offset: int = 0,
                         count: int = 10):
         """
-        Returns a sublist of the predictions created using an analysis result.
+        Returns a sublist of the predictions from an analysis.
 
-        :param str analysis_id: Identifies the analysis which must belong to a project to which the user has
-            read permissions.
-        :param int offset: predictions list offset.
-        :param count: max number of predictions to get.
+        :param str analysis_id: The id of the analysis. The user must have read permissions to the corresponding project.
+        :param int offset: Predictions list offset. The first element starts at offset 0.
+        :param int count: Limit on the number of predictions to return. No limit is applied if count is negative.
         :return: {analysisId: string, offset: number, totalCount: number,
             data: [{predictionId: string, projectId: string, parameters: object, state: string}]}
         :rtype: dict
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
 
-        The list uses zero-based indexing, meaning the first element is at offset 0.
-        Constraints: Both offset and count must be non-negative integers and count can be at most 100.
+        Constraints: Offset must be a non-negative integer.
 
         :Example:
 
         >>> client = JadbioClient('juser@gmail.com', 'a password')
         >>> client.get_predictions('5219')
         {
             'analysisId': '5219'
@@ -1662,15 +1679,15 @@
     def image_upload_init(self,
                           project_id: str,
                           name: str,
                           data_path: str,
                           has_feature_names: bool = True,
                           description: str = None):
         """
-        :param str project_id: project id
+        :param str project_id: The id of the project. The user must have write permissions to the project.
         :param str name: image name (should be unique per project)
         :param str data_path: csv file containing sample names, target, other features, if None it defaults to 'target.csv'
         :param bool has_feature_names:
         :param str description: dataset description (optional)
         :return: {taskId: string}
         :raises RequestFailed, JadRequestResponseError: Exception in case sth goes wrong with a request.
```

### Comparing `jadbio-1.2.8/jadbio.egg-info/PKG-INFO` & `jadbio-1.2.9/jadbio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jadbio
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python wrapper for the public JADBio REST API.
 Home-page: https://github.com/JADBio/JADBioPythonClient
 Author: JADBio
 Author-email: support@jadbio.com
 License: GPL3.0
 Project-URL: Homepage, https://jadbio.com
-Project-URL: Documentation, https://support.jadbio.com/pythonclient/1.2.8
+Project-URL: Documentation, https://support.jadbio.com/pythonclient/1.2.9
 Project-URL: Source code, https://github.com/JADBio/JADBioPythonClient
 Keywords: jadbio automl machine-learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jadbio-1.2.8/setup.cfg` & `jadbio-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jadbio-1.2.8/setup.py` & `jadbio-1.2.9/setup.py`

 * *Files identical despite different names*

