# Comparing `tmp/duct-tape-0.25.2.tar.gz` & `tmp/duct-tape-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duct-tape-0.25.2.tar", last modified: Mon Jan  9 16:54:41 2023, max compression
+gzip compressed data, was "duct-tape-0.26.0.tar", last modified: Wed May 17 18:18:05 2023, max compression
```

## Comparing `duct-tape-0.25.2.tar` & `duct-tape-0.26.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-01-09 16:54:41.733733 duct-tape-0.25.2/
--rw-rw-rw-   0        0        0    35823 2022-11-28 16:24:33.000000 duct-tape-0.25.2/LICENSE
--rw-rw-rw-   0        0        0     4760 2023-01-09 16:54:41.734754 duct-tape-0.25.2/PKG-INFO
--rw-rw-rw-   0        0        0     4090 2023-01-06 21:33:19.000000 duct-tape-0.25.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-09 16:54:41.695280 duct-tape-0.25.2/duct_tape.egg-info/
--rw-rw-rw-   0        0        0     4760 2023-01-09 16:54:41.000000 duct-tape-0.25.2/duct_tape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-01-09 16:54:41.000000 duct-tape-0.25.2/duct_tape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-09 16:54:41.000000 duct-tape-0.25.2/duct_tape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-01-09 16:54:41.000000 duct-tape-0.25.2/duct_tape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-09 16:54:41.000000 duct-tape-0.25.2/duct_tape.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-09 16:54:41.706555 duct-tape-0.25.2/ducttape/
--rw-rw-rw-   0        0        0      110 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-09 16:54:41.732732 duct-tape-0.25.2/ducttape/data_sources/
--rw-rw-rw-   0        0        0       35 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/data_sources/__init__.py
--rw-rw-rw-   0        0        0     8944 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/data_sources/clever.py
--rw-rw-rw-   0        0        0    20902 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/data_sources/googlesheets.py
--rw-rw-rw-   0        0        0     8203 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/data_sources/informedk12.py
--rw-rw-rw-   0        0        0    20552 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/data_sources/lexia.py
--rw-rw-rw-   0        0        0     4073 2023-01-09 15:43:25.000000 duct-tape-0.25.2/ducttape/data_sources/mealtime.py
--rw-rw-rw-   0        0        0    26605 2023-01-09 15:49:23.000000 duct-tape-0.25.2/ducttape/data_sources/schoolmint.py
--rw-rw-rw-   0        0        0     3800 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/data_sources/seis.py
--rw-rw-rw-   0        0        0    11441 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/data_sources/summitlearning.py
--rw-rw-rw-   0        0        0    11018 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/data_sources/typingagent.py
--rw-rw-rw-   0        0        0     1205 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/exceptions.py
--rw-rw-rw-   0        0        0     2786 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/httpsession.py
--rw-rw-rw-   0        0        0    10045 2023-01-06 21:33:19.000000 duct-tape-0.25.2/ducttape/legacy.py
--rw-rw-rw-   0        0        0     8799 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/utils.py
--rw-rw-rw-   0        0        0     1606 2022-11-28 16:24:33.000000 duct-tape-0.25.2/ducttape/webui_datasource.py
--rw-rw-rw-   0        0        0      129 2023-01-09 16:54:41.735579 duct-tape-0.25.2/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-01-09 16:50:24.000000 duct-tape-0.25.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:18:05.451927 duct-tape-0.26.0/
+-rw-rw-rw-   0        0        0    35823 2022-11-28 16:24:33.000000 duct-tape-0.26.0/LICENSE
+-rw-rw-rw-   0        0        0     4760 2023-05-17 18:18:05.453430 duct-tape-0.26.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4090 2023-01-06 21:33:19.000000 duct-tape-0.26.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 18:18:05.390190 duct-tape-0.26.0/duct_tape.egg-info/
+-rw-rw-rw-   0        0        0     4760 2023-05-17 18:18:05.000000 duct-tape-0.26.0/duct_tape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-05-17 18:18:05.000000 duct-tape-0.26.0/duct_tape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 18:18:05.000000 duct-tape-0.26.0/duct_tape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-17 18:18:05.000000 duct-tape-0.26.0/duct_tape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 18:18:05.000000 duct-tape-0.26.0/duct_tape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 18:18:05.401189 duct-tape-0.26.0/ducttape/
+-rw-rw-rw-   0        0        0      110 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 18:18:05.449715 duct-tape-0.26.0/ducttape/data_sources/
+-rw-rw-rw-   0        0        0       35 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/data_sources/__init__.py
+-rw-rw-rw-   0        0        0     8944 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/data_sources/clever.py
+-rw-rw-rw-   0        0        0    20902 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/data_sources/googlesheets.py
+-rw-rw-rw-   0        0        0     8203 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/data_sources/informedk12.py
+-rw-rw-rw-   0        0        0    20552 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/data_sources/lexia.py
+-rw-rw-rw-   0        0        0     4169 2023-01-13 20:14:53.000000 duct-tape-0.26.0/ducttape/data_sources/mealtime.py
+-rw-rw-rw-   0        0        0    27182 2023-01-13 20:14:53.000000 duct-tape-0.26.0/ducttape/data_sources/schoolmint.py
+-rw-rw-rw-   0        0        0     3800 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/data_sources/seis.py
+-rw-rw-rw-   0        0        0    11441 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/data_sources/summitlearning.py
+-rw-rw-rw-   0        0        0    11018 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/data_sources/typingagent.py
+-rw-rw-rw-   0        0        0     1205 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/exceptions.py
+-rw-rw-rw-   0        0        0     2786 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/httpsession.py
+-rw-rw-rw-   0        0        0    10045 2023-01-06 21:33:19.000000 duct-tape-0.26.0/ducttape/legacy.py
+-rw-rw-rw-   0        0        0     8959 2023-05-17 18:17:34.000000 duct-tape-0.26.0/ducttape/utils.py
+-rw-rw-rw-   0        0        0     1606 2022-11-28 16:24:33.000000 duct-tape-0.26.0/ducttape/webui_datasource.py
+-rw-rw-rw-   0        0        0      131 2023-05-17 18:18:05.454432 duct-tape-0.26.0/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2023-05-17 18:17:34.000000 duct-tape-0.26.0/setup.py
```

### Comparing `duct-tape-0.25.2/LICENSE` & `duct-tape-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/PKG-INFO` & `duct-tape-0.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duct-tape
-Version: 0.25.2
+Version: 0.26.0
 Summary: Duct Tape is a Python interface for downloading data, uploading data, and controlling supported Ed-Tech software.
 Home-page: https://github.com/SummitPublicSchools/ducttape
 Download-URL: 
 Author: Patrick Yoho
 Author-email: trickyoho@gmail.com
 Keywords: automation,education,illuminate,selenium,etl
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `duct-tape-0.25.2/README.md` & `duct-tape-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/duct_tape.egg-info/PKG-INFO` & `duct-tape-0.26.0/duct_tape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duct-tape
-Version: 0.25.2
+Version: 0.26.0
 Summary: Duct Tape is a Python interface for downloading data, uploading data, and controlling supported Ed-Tech software.
 Home-page: https://github.com/SummitPublicSchools/ducttape
 Download-URL: 
 Author: Patrick Yoho
 Author-email: trickyoho@gmail.com
 Keywords: automation,education,illuminate,selenium,etl
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `duct-tape-0.25.2/duct_tape.egg-info/SOURCES.txt` & `duct-tape-0.26.0/duct_tape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/clever.py` & `duct-tape-0.26.0/ducttape/data_sources/clever.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/googlesheets.py` & `duct-tape-0.26.0/ducttape/data_sources/googlesheets.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/informedk12.py` & `duct-tape-0.26.0/ducttape/data_sources/informedk12.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/lexia.py` & `duct-tape-0.26.0/ducttape/data_sources/lexia.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/mealtime.py` & `duct-tape-0.26.0/ducttape/data_sources/mealtime.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support.ui import Select
-from selenium.common.exceptions import NoSuchElementException
-import pandas as pd
-
-# local import
-from ducttape.webui_datasource import WebUIDataSource
-from ducttape.utils import (
-    configure_selenium_chrome,
-    interpret_report_url,
-    wait_for_any_file_in_folder,
-    get_most_recent_file_in_dir,
-    delete_folder_contents,
-    DriverBuilder,
-)
-
-
-class Mealtime(WebUIDataSource):
-    """ Class for interacting with the web ui of Mealtime
-    """
-
-    def __init__(self, username, password, wait_time, hostname, temp_folder_path, headless=False):
-        super().__init__(username, password, wait_time, hostname, temp_folder_path, headless)
-        self.uri_scheme = 'https://'
-        self.base_url = self.uri_scheme + self.hostname
-
-    def _login(self):
-        """ Logs into the provided Mealtime instance.
-        """
-        self.driver.get(self.base_url + '/Base/SignIn.aspx')
-        elem = self.driver.find_element(By.ID, "username")
-        elem.clear()
-        elem.send_keys(self.username)
-        elem = self.driver.find_element(By.ID, "password")
-        elem.send_keys(self.password)
-        elem.send_keys(Keys.RETURN)
-
-    def download_url_report(self, report_url, temp_folder_name):
-        """ Downloads a MealTime report.
-
-        Args:
-            report_url (string): Information pertaining to the path and query
-                string for the report whose access is desired. Any filtering
-                that can be done with a stateful URL should be included.
-            temp_folder_name (string): The name of the folder in which this
-                specific report's download files should be stored.
-
-        Returns: A Pandas DataFrame of the report contents.
-        """
-        csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
-        # set up the driver for execution
-        self.driver = DriverBuilder().get_driver(csv_download_folder_path, self.headless)
-        self._login()
-
-        # get the report url
-        self.driver.get(interpret_report_url(self.base_url, report_url))
-
-        # select the download format (csv) and execute
-        export_format_select = Select(self.driver.find_element(By.ID, 'ctl00_ctl00_MainContent_reportViewer_ctl01_ctl05_ctl00'))
-        try:
-            export_format_select.select_by_value('CSV')
-            dl_type = 'csv'
-        except NoSuchElementException:
-            export_format_select.select_by_value('EXCELNoHeader')
-            dl_type = 'xls'
-        self.driver.find_element(By.ID, 'ctl00_ctl00_MainContent_reportViewer_ctl01_ctl05_ctl01').click()
-
-        # wait until file has downloaded to close the browser. We can do this
-        # because we delete the file before we return it, so the temp dir should
-        # always be empty when this command is run
-        # TODO add a try/except block here
-        wait_for_any_file_in_folder(csv_download_folder_path, dl_type)
-
-        # remove the header rows
-        #xlrd.open_workbook(utils.get_most_recent_file_in_dir(csv_download_folder_path), formatting_info=False)
-
-        if dl_type == 'csv':
-            report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
-                                      header=2)
-        else:
-            report_df = pd.read_excel(get_most_recent_file_in_dir(csv_download_folder_path),
-                                      header=3)
-
-        # delete any files in the mealtime temp folder; we don't need them now
-        # TODO: move this out of this function. It should happen as cleanup once
-        # the whole DAG has completed
-        delete_folder_contents(csv_download_folder_path)
-
-        self.driver.close()
-
-        # if the dataframe is empty (the report had no data), raise an error
-        if report_df.shape[0] == 0:
-            raise ValueError('No data in report for user {} at url: {}'.format(self.username, interpret_report_url(self.base_url, report_url)))
-
-        return report_df
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.ui import Select
+from selenium.common.exceptions import NoSuchElementException
+import pandas as pd
+
+# local import
+from ducttape.webui_datasource import WebUIDataSource
+from ducttape.utils import (
+    configure_selenium_chrome,
+    interpret_report_url,
+    wait_for_any_file_in_folder,
+    get_most_recent_file_in_dir,
+    delete_folder_contents,
+    DriverBuilder,
+)
+
+
+class Mealtime(WebUIDataSource):
+    """ Class for interacting with the web ui of Mealtime
+    """
+
+    def __init__(self, username, password, wait_time, hostname, temp_folder_path, headless=False):
+        super().__init__(username, password, wait_time, hostname, temp_folder_path, headless)
+        self.uri_scheme = 'https://'
+        self.base_url = self.uri_scheme + self.hostname
+
+    def _login(self):
+        """ Logs into the provided Mealtime instance.
+        """
+        self.driver.get(self.base_url + '/Base/SignIn.aspx')
+        elem = self.driver.find_element(By.ID, "username")
+        elem.clear()
+        elem.send_keys(self.username)
+        elem = self.driver.find_element(By.ID, "password")
+        elem.send_keys(self.password)
+        elem.send_keys(Keys.RETURN)
+
+    def download_url_report(self, report_url, temp_folder_name):
+        """ Downloads a MealTime report.
+
+        Args:
+            report_url (string): Information pertaining to the path and query
+                string for the report whose access is desired. Any filtering
+                that can be done with a stateful URL should be included.
+            temp_folder_name (string): The name of the folder in which this
+                specific report's download files should be stored.
+
+        Returns: A Pandas DataFrame of the report contents.
+        """
+        csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
+        # set up the driver for execution
+        self.driver = DriverBuilder().get_driver(csv_download_folder_path, self.headless)
+        self._login()
+
+        # get the report url
+        self.driver.get(interpret_report_url(self.base_url, report_url))
+
+        # select the download format (csv) and execute
+        export_format_select = Select(self.driver.find_element(By.ID, 'ctl00_ctl00_MainContent_reportViewer_ctl01_ctl05_ctl00'))
+        try:
+            export_format_select.select_by_value('CSV')
+            dl_type = 'csv'
+        except NoSuchElementException:
+            export_format_select.select_by_value('EXCELNoHeader')
+            dl_type = 'xls'
+        self.driver.find_element(By.ID, 'ctl00_ctl00_MainContent_reportViewer_ctl01_ctl05_ctl01').click()
+
+        # wait until file has downloaded to close the browser. We can do this
+        # because we delete the file before we return it, so the temp dir should
+        # always be empty when this command is run
+        # TODO add a try/except block here
+        wait_for_any_file_in_folder(csv_download_folder_path, dl_type)
+
+        # remove the header rows
+        #xlrd.open_workbook(utils.get_most_recent_file_in_dir(csv_download_folder_path), formatting_info=False)
+
+        if dl_type == 'csv':
+            report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
+                                      header=2)
+        else:
+            report_df = pd.read_excel(get_most_recent_file_in_dir(csv_download_folder_path),
+                                      header=3)
+
+        # delete any files in the mealtime temp folder; we don't need them now
+        # TODO: move this out of this function. It should happen as cleanup once
+        # the whole DAG has completed
+        delete_folder_contents(csv_download_folder_path)
+
+        self.driver.close()
+
+        # if the dataframe is empty (the report had no data), raise an error
+        if report_df.shape[0] == 0:
+            raise ValueError('No data in report for user {} at url: {}'.format(self.username, interpret_report_url(self.base_url, report_url)))
+
+        return report_df
```

### Comparing `duct-tape-0.25.2/ducttape/data_sources/schoolmint.py` & `duct-tape-0.26.0/ducttape/data_sources/schoolmint.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,577 +1,577 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
-from __future__ import absolute_import
-from builtins import super
-from builtins import int
-from builtins import str
-from future import standard_library
-from future.utils import raise_with_traceback
-standard_library.install_aliases()
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.common.exceptions import (
-    TimeoutException,
-    NoSuchElementException,
-    ElementNotVisibleException,
-)
-from selenium.webdriver.common.by import By
-import pandas as pd
-import time
-import datetime
-import os
-import glob
-import re
-import shutil
-from tempfile import mkdtemp
-
-# local import
-from ducttape.webui_datasource import WebUIDataSource
-from ducttape.utils import (
-    configure_selenium_chrome,
-    interpret_report_url,
-    wait_for_any_file_in_folder,
-    get_most_recent_file_in_dir,
-    delete_folder_contents,
-    DriverBuilder,
-    LoggingMixin,
-    ZipfileLongPaths,
-)
-from ducttape.exceptions import (
-    ReportNotReady,
-    NoDataError,
-    ReportNotFound,
-    InvalidLoginCredentials,
-)
-
-SCHOOLMINT_DEFAULT_EXPORT_ENCODING = 'utf-8-sig'
-WALKME_AND_SUPPORT_TIMEOUT = 5
-NUMBER_OF_RETRIES = 3
-
-GENERATE_REPORT_BUTTON_XPATH = (
-    "//tr[td[text() = '{report_name}' or text() = ' {report_name} ']]//button[contains(@class, 'export-data')]"
-)
-
-
-class SchoolMint(WebUIDataSource, LoggingMixin):
-    """ Class for interacting with SchoolMint
-    """
-
-    def __init__(self, username, password, wait_time, hostname, temp_folder_path, headless=False):
-        # try:
-        #     self.logger = logging.getLogger('sps-automation.data_sources.schoolmint.Schoolmint')
-        # except AttributeError:
-        #     self.log
-        super().__init__(username, password, wait_time, hostname, temp_folder_path, headless)
-        self.uri_scheme = 'https://'
-        self.base_url = self.uri_scheme + self.hostname
-
-    def _login(self):
-        """ Logs into the provided SchoolMint instance.
-        """
-        # 2019-01-16 SchoolMint seems to be having some issues with loading the login screen recently,
-        # so we'll add a retry here
-        count = 0
-        while count < NUMBER_OF_RETRIES:
-            self.log.debug('Logging into SchoolMint at, try {}: {}'.format(count, self.base_url))
-            self.driver.get(self.base_url + "/signin")
-            # wait until login form available
-            try:
-                elem = WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'login')))
-                elem.clear()
-                elem.send_keys(self.username)
-                elem = self.driver.find_element(By.ID, "password")
-                elem.send_keys(self.password)
-                elem.send_keys(Keys.RETURN)
-                break
-            except ElementNotVisibleException:
-                count += 1
-
-        # check that login succeeded by looking for the 'Student search' box
-        try:
-            elem = WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'student-lookup')))
-        except TimeoutException:
-            self.driver.close()
-            raise InvalidLoginCredentials
-
-        # wait for the page to fully load - the walk-me player is the last thing, but since it's a third
-        # party add-on we'll wait for the filters on the application index first
-        WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located(
-            (By.CLASS_NAME, 'report-filters')))
-        # now we'll wait for the walk "Walk Me Through" overlay in the bottom right
-        try:
-            WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'walkme-player')))
-        except TimeoutException:
-            pass
-
-        # deal with the walk_me announcement pop-ups overlays
-        try:
-            elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
-                EC.presence_of_element_located((By.CLASS_NAME, 'wm-shoutout'))
-            )
-            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-            elem = self.driver.find_element(By.ID, 'walkme-overlay-all')
-            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-        except TimeoutException:
-            self.log.debug('No wm-shoutout found')
-
-    def __remove_walk_me_and_support(self):
-        """Removes two third party overlays that can block buttons that selenium needs to click."""
-        self.log.info('Removing "Walk-Me" and "Support" overlays.')
-        walkme = True
-        # wait for walk-me to load
-        try:
-            WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'walkme-player')))
-        except TimeoutException:
-            self.log.info('Probably no Walk-Me found')
-            walkme = False
-
-        if walkme:
-            self.log.debug('Removing "Walk Me" overlay.')
-            try:
-                for id in ['walkme-player', 'walkme-overlay-all']:
-                    elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
-                        EC.presence_of_element_located((By.ID, id))
-                    )
-                    self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-                self.log.debug('Success')
-                self.log.debug('Removing "Walk Me" bouncing overlay.')
-                try:
-                    elem = self.driver.find_element(By.ID, 'walkme-attengrab')
-                    self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-                    self.log.debug('Success')
-                except NoSuchElementException:
-                    self.log.debug('No "Walk Me" bouncing overlay found.')
-            except TimeoutException:
-                self.log.debug('No "Walk Me" overlay found.')
-
-            # remove "Homeroom" announcement
-            self.log.debug('Removing "Homeroom" and other wm-shoutout modals.')
-            try:
-                elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
-                    # it turns out that the id can have numbers at the end (e.g. wm-shoutout-141590), so we need XPATH
-                    EC.presence_of_element_located((By.XPATH, "//*[starts-with(@id, 'wm-shoutout')]"))
-                )
-                self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-                self.log.debug('Success')
-            except TimeoutException:
-                self.log.debug('No "Homeroom" or other wm-shoutout modals found.')
-
-        # remove 'Support' button
-        self.log.debug('Trying to remove "Support" overlay.')
-        try:
-            elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
-                EC.presence_of_element_located((By.ID, 'launcher'))
-            )
-            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
-            self.log.debug('Success')
-        except TimeoutException:
-            self.log.debug('No "Support" overlay found.')
-            pass
-
-    def _set_year(self, school_year, driver=None):
-        """Sets the year for the SchoolMint interface.
-
-        Args:
-            school_year (string): The school year that should be selected. Use the format shown in the
-                SchoolMint interface. Example: '2016-2017'
-
-        :return: True if function succeeds
-        """
-        self.log.debug('Changing school year to: {}'.format(school_year))
-        if not driver:
-            self.driver = configure_selenium_chrome()
-            self._login()
-
-        # open the year selector menu
-        elem = WebDriverWait(self.driver, timeout=180).until(
-            EC.presence_of_element_located(
-                (By.XPATH, "//a[contains(@class,'dropdown-toggle enrollment')]")
-            )
-        )
-        elem.click()
-
-        # select the appropriate year
-        try:
-            year_xpath = "//*[@id='enrollment-selector']//a[contains(text(),'{}')]".format(school_year)
-            elem = self.driver.find_element(By.XPATH, year_xpath)
-            elem.click()
-        except NoSuchElementException as e:
-            self.driver.save_screenshot('cannot_find_year.png')
-            message = (
-                ' Check that the school_year variable is valid. '
-                'Passed value for school_year: {}'
-            ).format(school_year)
-
-            raise_with_traceback(type(e)(str(e) + message))
-
-        # wait for the page to be ready again
-        self.driver.get(self.base_url)
-        WebDriverWait(self.driver, timeout=180).until(
-            EC.presence_of_element_located((By.ID, 'student-lookup'))
-        )
-
-        if not driver:
-            self.driver.close()
-
-        return True
-
-    def check_school_year(self, school_year):
-        """Checks that the school year is set as expected in the UI."""
-        elem = self.driver.find_element(
-            By.XPATH, 
-            "//a[contains(@class,'dropdown-toggle enrollment')]/span[contains(@class,'current')]"
-        )
-        if school_year in elem.text:
-            return True
-        else:
-            return False
-
-    def download_url_report(self, report_url, school_year, temp_folder_name=None, pandas_read_csv_kwargs={}):
-        """ Downloads a SchoolMint data-stream-table report.
-
-        Args:
-            report_url (string): Information pertaining to the path and query
-                string for the report whose access is desired. Any filtering
-                that can be done with a stateful URL should be included.
-            school_year (string): The SchoolMint school year to download from (e.g. '2018-2019')
-            temp_folder_name (string): The name for a sub-directory in which the files from the
-                browser will be temporarily stored. If this directory does not exist, it will be
-                created. NOTE: This sub-directory will be
-            pandas_read_csv_kwargs: additional arguments to pass to Pandas read_csv
-
-        Returns: A Pandas DataFrame of the report contents.
-        """
-        if temp_folder_name:
-            csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
-        else:
-            csv_download_folder_path = mkdtemp(dir=self.temp_folder_path)
-
-        # set up the driver for execution
-        self.driver = DriverBuilder().get_driver(csv_download_folder_path, self.headless)
-        self._login()
-        # Clear pop-ups by reloading page
-        self.driver.get(self.base_url)
-        self._set_year(school_year, self.driver)
-
-        # get the report url
-        self.driver.get(interpret_report_url(self.base_url, report_url))
-        self.__remove_walk_me_and_support()
-
-        # wait until we have rows in the stream data table before starting to
-        # look for results
-        elem = WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.XPATH, "//*[@id='stream-table']/tbody/tr[1]/td[1]"))
-        )
-
-        if not self.check_school_year(school_year):
-            raise ReportNotFound("Wrong school detected prior to clicking generate.")
-
-        self.log.debug('Waiting for report-data-summary to load')
-        # wait until the stream table is fully loaded before downloading
-        prev_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
-        # print(prev_data_summary_elem)
-        time.sleep(1)
-        # we use the following count as a proxy for time elapsed, so we can
-        # use the class's wait_time as the number of retries
-        count = 0
-        while True:
-            # check id=report-data-summary
-            report_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
-
-            # if it matches, wait a little longer and double deck that it hasn't changed
-            if prev_data_summary_elem == report_data_summary_elem:
-                time.sleep(3)
-                count += 3
-                report_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
-                if prev_data_summary_elem == report_data_summary_elem:
-                    break
-            prev_data_summary_elem = report_data_summary_elem
-            time.sleep(1)
-
-            count += 1
-            if count >= self.wait_time:
-                raise TimeoutError('SchoolMint Report Data never did not fully load within %d' % self.wait_time)
-
-        # click the button to download the report
-        self.log.debug('Starting download...')
-        elem = self.driver.find_element(By.CLASS_NAME, "export-table")
-        elem.click()
-
-        # wait until file has downloaded to close the browser. We can do this
-        # because we delete the file before we return it, so the temp dir should
-        # always be empty when this command is run
-        wait_for_any_file_in_folder(csv_download_folder_path, "csv")
-
-        self.log.debug('Download finished.')
-        report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
-                                encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING, **pandas_read_csv_kwargs)
-
-        # TODO: move this out of this function. It should happen as cleanup once
-        # the whole DAG has completed
-        #delete_folder_contents(csv_download_folder_path)
-        shutil.rmtree(csv_download_folder_path)
-
-        # close the driver for this task
-        self.driver.close()
-
-        # if the dataframe is empty (the report had no data), raise an error
-        if report_df.shape[0] == 0:
-            #delete_folder_contents(csv_download_folder_path)
-            shutil.rmtree(csv_download_folder_path)
-            raise ValueError('No data in report for user {} at url: {}'.format(
-                self.username, interpret_report_url(self.base_url, report_url)))
-
-        return report_df
-
-    def __get_number_of_pages(self):
-        """Get the number of pages in a SchoolMint pagination."""
-        total_num_pages_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page][last()]'
-
-        elem = WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.XPATH, total_num_pages_xpath)))
-
-        num_pages = int(elem.get_attribute("data-page")) + 1
-
-        return num_pages
-
-    def __navigate_to_custom_report(self, report_name, school_year,
-                                    download_folder_path=None):
-        """Navigate to the page of the custom report tool that has the custom report on it"""
-        if not download_folder_path:
-            download_folder_path = self.temp_folder_path
-        self.driver = DriverBuilder().get_driver(
-            download_location=download_folder_path,
-            headless=self.headless
-        )
-        self._login()
-        # Clear pop-ups by reloading page
-        self.driver.get(self.base_url)
-        self._set_year(school_year, self.driver)
-
-        # get the custom reports page
-        custom_reports_url = 'report/customReports'
-        self.driver.get(interpret_report_url(self.base_url, custom_reports_url))
-        self.__remove_walk_me_and_support()
-
-        # wait for the page to load and get the maximum number of pages
-        total_num_pages_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page][last()]'
-
-        elem = WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.XPATH, total_num_pages_xpath)))
-
-        num_pages = int(elem.get_attribute("data-page")) + 1
-
-        current_page = 0
-        while current_page < num_pages:
-            report_name_xpath = "//tr[td//text()[contains(., '{}')]]".format(
-                report_name
-            )
-
-            try:
-                elem = self.driver.find_element(By.XPATH, report_name_xpath)
-                return current_page
-            except NoSuchElementException:
-                current_page += 1
-                if current_page < num_pages:
-                    next_page_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page={}]/a'.format(
-                        current_page
-                    )
-                    self.driver.find_element(By.XPATH, next_page_xpath).click()
-
-                    # scroll back to the top of the page, prevents selenium clicking errors
-                    self.driver.execute_script("window.scrollTo(0, 0);")
-
-        raise ReportNotFound
-
-    def generate_custom_report(self, report_name, school_year):
-        """
-        Clicks the generate button on a SchoolMint custom report.
-        :param report_name: The name of the report exactly as it is shown in the SchoolMint UI
-        :param school_year: The year in SchoolMint. Should be formatted as shown in the UI
-            (e.g. '2018-2019')
-        :return: True if the button was clicked. False if the button was not clicked because
-            the report is generating.
-        """
-        self.__navigate_to_custom_report(report_name, school_year)
-
-        if not self.check_school_year(school_year):
-            raise ReportNotFound("Wrong school detected prior to clicking generate.")
-
-        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
-        try:
-            generate_report_button = WebDriverWait(self.driver, self.wait_time).until(
-                EC.presence_of_element_located((By.XPATH, generate_report_button_xpath)))
-        except NoSuchElementException:
-            raise ReportNotFound
-
-        if generate_report_button.text == 'Generate Report':
-            generate_report_button.click()
-            self.driver.close()
-
-            return True
-        elif generate_report_button.text == 'Report in Progress':
-            self.driver.close()
-
-            return False
-        else:
-            raise ValueError("Unknown 'Generate Report' button text found")
-
-    def is_custom_report_generating(self, report_name, school_year):
-        """Checks if a SchoolMint Custom Report is generating or not"""
-        self.__navigate_to_custom_report(report_name, school_year)
-
-        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
-        try:
-            generate_report_button = WebDriverWait(self.driver, self.wait_time).until(
-                EC.presence_of_element_located((By.XPATH, generate_report_button_xpath)))
-        except NoSuchElementException:
-            raise ReportNotFound
-
-        if generate_report_button.text == 'Report in Progress':
-            return True
-        elif generate_report_button.text == 'Generate Report':
-            return False
-        else:
-            raise ValueError("Unknown 'Generate Report' button text found")
-
-    def get_last_custom_report_generation_datetime(self, report_name, school_year):
-        """Get's a report's generation timestamp in raw text"""
-        self.__navigate_to_custom_report(report_name, school_year)
-
-        try:
-            # old custom reports interface
-            report_generated_on_xpath = (
-                "//tr[td[./text()='{}']]/td[4]"
-            ).format(report_name)
-            report_generated_on_text = WebDriverWait(self.driver, self.wait_time).until(
-                EC.presence_of_element_located((By.XPATH, report_generated_on_xpath))).text
-        except TimeoutException:
-            try:
-                # new custom reports interface
-                report_generated_on_xpath = (
-                    "//tr[td[text()=' {} ']]/td[contains(@class,'last_generated_date-td')]"
-                ).format(report_name)
-                report_generated_on_text = WebDriverWait(self.driver, self.wait_time).until(
-                    EC.presence_of_element_located((By.XPATH, report_generated_on_xpath))).text
-            except TimeoutException:
-                raise ReportNotFound
-
-        return report_generated_on_text
-
-    def _download_custom_report(self, report_name, school_year, download_folder_path, download_if_generating=False):
-        """Protected function for clicking the download button on a report on the Custom Reports page"""
-        if not download_folder_path:
-            download_folder_path = self.temp_folder_path
-        self.__navigate_to_custom_report(report_name, school_year, download_folder_path)
-
-        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
-        generate_report_button_text = WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.XPATH, generate_report_button_xpath))).text
-
-        download_button_xpath = (
-            "//tr[td[text() = '{report_name}' or text() = ' {report_name} ']]//a[contains(text(), 'Download')]"
-        ).format(report_name=report_name)
-
-        elem = WebDriverWait(self.driver, self.wait_time).until(
-            EC.presence_of_element_located((By.XPATH, download_button_xpath)))
-
-        if generate_report_button_text == 'Generate Report':
-            elem.click()
-        elif generate_report_button_text == 'Report in Progress' and download_if_generating:
-            elem.click()
-        else:
-            raise ReportNotReady
-
-        return self.driver
-
-    def download_csv_custom_report(self, report_name, school_year, download_if_generating=False,
-                                   pandas_read_csv_kwargs={}):
-        """Download a SchoolMint Custom Report that downloads as a single CSV file"""
-        temp_folder_name = report_name.replace(" ", "_").lower()
-        csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
-        driver = self._download_custom_report(report_name, school_year, csv_download_folder_path,
-                                              download_if_generating)
-
-        # wait until file has downloaded to close the browser. We can do this
-        # because we delete the file before we return it, so the temp dir should
-        # always be empty when this command is run
-        wait_for_any_file_in_folder(csv_download_folder_path, "csv")
-
-        report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
-                                encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING, **pandas_read_csv_kwargs)
-
-        # delete any files in the mealtime temp folder; we don't need them now
-        # TODO: move this out of this function. It should happen as cleanup once
-        # the whole DAG has completed
-        delete_folder_contents(csv_download_folder_path)
-
-        # close the driver for this task
-        driver.close()
-
-        # if the dataframe is empty (the report had no data), raise an error
-        if report_df.shape[0] == 0:
-            raise NoDataError('No data for user {} in Custom Report: {}'.format(self.username, report_name))
-
-        return report_df
-
-    def download_zip_custom_report(self, report_name, school_year, download_folder_path=None,
-                                   download_if_generating=False, unzip=True,
-                                   pandas_read_csv_kwargs={}):
-        """
-        Downloads a SchoolMint Custom Report that downloads as a zipped set of CSVs
-        :param report_name: The name of the report exactly as it is shown in the SchoolMint UI
-        :param school_year: The year in SchoolMint. Should be formatted as shown in the UI
-            (e.g. '2018-2019')
-        :param download_folder_path: The path to where you want to store the zip file.
-        :param download_if_generating: Whether or not to download a custom report if the
-            report is currently generating.
-        :param unzip: Boolean. If True, not only downloads the file, but also unzips it and
-            returns each csv in a Pandas Dataframe in a dictionary.
-        :param pandas_read_csv_kwargs: Additional keyward arguments to pass to Panda's read_csv function.
-        :return: None or a dictionary of Pandas DataFrames representing each of the CSVs in
-            the zipped file.
-        """
-        # create a folder for this specific run
-        run_time = datetime.datetime.utcnow()
-        if not download_folder_path:
-            download_folder_path = self.temp_folder_path
-        download_dir_final = "{}/{}-{}-{}".format(download_folder_path, report_name,
-                                                   run_time.strftime('%Y%m%d'), run_time.strftime('%H%M%S'))
-        driver = self._download_custom_report(report_name, school_year, download_dir_final, download_if_generating)
-
-        # wait until file has downloaded to close the browser. We can do this
-        # because we delete the file before we return it, so the temp dir should
-        # always be empty when this command is run
-        # TODO add a try/except block here
-        wait_for_any_file_in_folder(download_dir_final, "zip")
-
-        driver.close()
-
-        if unzip:
-            # unzip the files
-            file_path = max(glob.iglob(download_dir_final + '/*.zip'), key=os.path.getctime)
-            ZipfileLongPaths(file_path).extractall(download_dir_final)
-
-            dfs = dict()
-            # iterate through the unzipped files and load them into dataframes
-            for csv_filepath in glob.iglob(download_dir_final + '/*.csv'):
-                csv_filename = os.path.basename(csv_filepath)
-                #print(csv_filename)
-                # find the files that start with a number, these are the custom forms files
-                if re.match("^(\d+)", csv_filename):
-                    num_beg = re.match("^(\d+)", csv_filename).group(0)
-                    words = re.findall("[A-Za-z]+", csv_filename)
-                    dict_key = csv_filename # "{}_{}".format(num_beg, '_'.join(words[0:3])).lower()
-                    dfs[dict_key] = pd.read_csv(csv_filepath, encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING,
-                                                skiprows=[0, 2], **pandas_read_csv_kwargs)
-                # otherwise it is the info file that comes along with the zip export (application-data-export, etc.)
-                else:
-                    words = re.findall("[A-Za-z]+", csv_filename)
-                    dict_key = csv_filename # "{}".format('_'.join(words[0:3])).lower()
-
-                    dfs[dict_key] = pd.read_csv(csv_filepath, encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING,
-                                                **pandas_read_csv_kwargs)
-
-            return dfs
+from __future__ import unicode_literals
+from __future__ import print_function
+from __future__ import division
+from __future__ import absolute_import
+from builtins import super
+from builtins import int
+from builtins import str
+from future import standard_library
+from future.utils import raise_with_traceback
+standard_library.install_aliases()
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.common.exceptions import (
+    TimeoutException,
+    NoSuchElementException,
+    ElementNotVisibleException,
+)
+from selenium.webdriver.common.by import By
+import pandas as pd
+import time
+import datetime
+import os
+import glob
+import re
+import shutil
+from tempfile import mkdtemp
+
+# local import
+from ducttape.webui_datasource import WebUIDataSource
+from ducttape.utils import (
+    configure_selenium_chrome,
+    interpret_report_url,
+    wait_for_any_file_in_folder,
+    get_most_recent_file_in_dir,
+    delete_folder_contents,
+    DriverBuilder,
+    LoggingMixin,
+    ZipfileLongPaths,
+)
+from ducttape.exceptions import (
+    ReportNotReady,
+    NoDataError,
+    ReportNotFound,
+    InvalidLoginCredentials,
+)
+
+SCHOOLMINT_DEFAULT_EXPORT_ENCODING = 'utf-8-sig'
+WALKME_AND_SUPPORT_TIMEOUT = 5
+NUMBER_OF_RETRIES = 3
+
+GENERATE_REPORT_BUTTON_XPATH = (
+    "//tr[td[text() = '{report_name}' or text() = ' {report_name} ']]//button[contains(@class, 'export-data')]"
+)
+
+
+class SchoolMint(WebUIDataSource, LoggingMixin):
+    """ Class for interacting with SchoolMint
+    """
+
+    def __init__(self, username, password, wait_time, hostname, temp_folder_path, headless=False):
+        # try:
+        #     self.logger = logging.getLogger('sps-automation.data_sources.schoolmint.Schoolmint')
+        # except AttributeError:
+        #     self.log
+        super().__init__(username, password, wait_time, hostname, temp_folder_path, headless)
+        self.uri_scheme = 'https://'
+        self.base_url = self.uri_scheme + self.hostname
+
+    def _login(self):
+        """ Logs into the provided SchoolMint instance.
+        """
+        # 2019-01-16 SchoolMint seems to be having some issues with loading the login screen recently,
+        # so we'll add a retry here
+        count = 0
+        while count < NUMBER_OF_RETRIES:
+            self.log.debug('Logging into SchoolMint at, try {}: {}'.format(count, self.base_url))
+            self.driver.get(self.base_url + "/signin")
+            # wait until login form available
+            try:
+                elem = WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'login')))
+                elem.clear()
+                elem.send_keys(self.username)
+                elem = self.driver.find_element(By.ID, "password")
+                elem.send_keys(self.password)
+                elem.send_keys(Keys.RETURN)
+                break
+            except ElementNotVisibleException:
+                count += 1
+
+        # check that login succeeded by looking for the 'Student search' box
+        try:
+            elem = WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'student-lookup')))
+        except TimeoutException:
+            self.driver.close()
+            raise InvalidLoginCredentials
+
+        # wait for the page to fully load - the walk-me player is the last thing, but since it's a third
+        # party add-on we'll wait for the filters on the application index first
+        WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located(
+            (By.CLASS_NAME, 'report-filters')))
+        # now we'll wait for the walk "Walk Me Through" overlay in the bottom right
+        try:
+            WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'walkme-player')))
+        except TimeoutException:
+            pass
+
+        # deal with the walk_me announcement pop-ups overlays
+        try:
+            elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
+                EC.presence_of_element_located((By.CLASS_NAME, 'wm-shoutout'))
+            )
+            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+            elem = self.driver.find_element(By.ID, 'walkme-overlay-all')
+            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+        except TimeoutException:
+            self.log.debug('No wm-shoutout found')
+
+    def __remove_walk_me_and_support(self):
+        """Removes two third party overlays that can block buttons that selenium needs to click."""
+        self.log.info('Removing "Walk-Me" and "Support" overlays.')
+        walkme = True
+        # wait for walk-me to load
+        try:
+            WebDriverWait(self.driver, self.wait_time).until(EC.presence_of_element_located((By.ID, 'walkme-player')))
+        except TimeoutException:
+            self.log.info('Probably no Walk-Me found')
+            walkme = False
+
+        if walkme:
+            self.log.debug('Removing "Walk Me" overlay.')
+            try:
+                for id in ['walkme-player', 'walkme-overlay-all']:
+                    elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
+                        EC.presence_of_element_located((By.ID, id))
+                    )
+                    self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+                self.log.debug('Success')
+                self.log.debug('Removing "Walk Me" bouncing overlay.')
+                try:
+                    elem = self.driver.find_element(By.ID, 'walkme-attengrab')
+                    self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+                    self.log.debug('Success')
+                except NoSuchElementException:
+                    self.log.debug('No "Walk Me" bouncing overlay found.')
+            except TimeoutException:
+                self.log.debug('No "Walk Me" overlay found.')
+
+            # remove "Homeroom" announcement
+            self.log.debug('Removing "Homeroom" and other wm-shoutout modals.')
+            try:
+                elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
+                    # it turns out that the id can have numbers at the end (e.g. wm-shoutout-141590), so we need XPATH
+                    EC.presence_of_element_located((By.XPATH, "//*[starts-with(@id, 'wm-shoutout')]"))
+                )
+                self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+                self.log.debug('Success')
+            except TimeoutException:
+                self.log.debug('No "Homeroom" or other wm-shoutout modals found.')
+
+        # remove 'Support' button
+        self.log.debug('Trying to remove "Support" overlay.')
+        try:
+            elem = WebDriverWait(self.driver, WALKME_AND_SUPPORT_TIMEOUT).until(
+                EC.presence_of_element_located((By.ID, 'launcher'))
+            )
+            self.driver.execute_script("""var elem=arguments[0];elem.parentNode.removeChild(elem);""", elem)
+            self.log.debug('Success')
+        except TimeoutException:
+            self.log.debug('No "Support" overlay found.')
+            pass
+
+    def _set_year(self, school_year, driver=None):
+        """Sets the year for the SchoolMint interface.
+
+        Args:
+            school_year (string): The school year that should be selected. Use the format shown in the
+                SchoolMint interface. Example: '2016-2017'
+
+        :return: True if function succeeds
+        """
+        self.log.debug('Changing school year to: {}'.format(school_year))
+        if not driver:
+            self.driver = configure_selenium_chrome()
+            self._login()
+
+        # open the year selector menu
+        elem = WebDriverWait(self.driver, timeout=180).until(
+            EC.presence_of_element_located(
+                (By.XPATH, "//a[contains(@class,'dropdown-toggle enrollment')]")
+            )
+        )
+        elem.click()
+
+        # select the appropriate year
+        try:
+            year_xpath = "//*[@id='enrollment-selector']//a[contains(text(),'{}')]".format(school_year)
+            elem = self.driver.find_element(By.XPATH, year_xpath)
+            elem.click()
+        except NoSuchElementException as e:
+            self.driver.save_screenshot('cannot_find_year.png')
+            message = (
+                ' Check that the school_year variable is valid. '
+                'Passed value for school_year: {}'
+            ).format(school_year)
+
+            raise_with_traceback(type(e)(str(e) + message))
+
+        # wait for the page to be ready again
+        self.driver.get(self.base_url)
+        WebDriverWait(self.driver, timeout=180).until(
+            EC.presence_of_element_located((By.ID, 'student-lookup'))
+        )
+
+        if not driver:
+            self.driver.close()
+
+        return True
+
+    def check_school_year(self, school_year):
+        """Checks that the school year is set as expected in the UI."""
+        elem = self.driver.find_element(
+            By.XPATH, 
+            "//a[contains(@class,'dropdown-toggle enrollment')]/span[contains(@class,'current')]"
+        )
+        if school_year in elem.text:
+            return True
+        else:
+            return False
+
+    def download_url_report(self, report_url, school_year, temp_folder_name=None, pandas_read_csv_kwargs={}):
+        """ Downloads a SchoolMint data-stream-table report.
+
+        Args:
+            report_url (string): Information pertaining to the path and query
+                string for the report whose access is desired. Any filtering
+                that can be done with a stateful URL should be included.
+            school_year (string): The SchoolMint school year to download from (e.g. '2018-2019')
+            temp_folder_name (string): The name for a sub-directory in which the files from the
+                browser will be temporarily stored. If this directory does not exist, it will be
+                created. NOTE: This sub-directory will be
+            pandas_read_csv_kwargs: additional arguments to pass to Pandas read_csv
+
+        Returns: A Pandas DataFrame of the report contents.
+        """
+        if temp_folder_name:
+            csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
+        else:
+            csv_download_folder_path = mkdtemp(dir=self.temp_folder_path)
+
+        # set up the driver for execution
+        self.driver = DriverBuilder().get_driver(csv_download_folder_path, self.headless)
+        self._login()
+        # Clear pop-ups by reloading page
+        self.driver.get(self.base_url)
+        self._set_year(school_year, self.driver)
+
+        # get the report url
+        self.driver.get(interpret_report_url(self.base_url, report_url))
+        self.__remove_walk_me_and_support()
+
+        # wait until we have rows in the stream data table before starting to
+        # look for results
+        elem = WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.XPATH, "//*[@id='stream-table']/tbody/tr[1]/td[1]"))
+        )
+
+        if not self.check_school_year(school_year):
+            raise ReportNotFound("Wrong school detected prior to clicking generate.")
+
+        self.log.debug('Waiting for report-data-summary to load')
+        # wait until the stream table is fully loaded before downloading
+        prev_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
+        # print(prev_data_summary_elem)
+        time.sleep(1)
+        # we use the following count as a proxy for time elapsed, so we can
+        # use the class's wait_time as the number of retries
+        count = 0
+        while True:
+            # check id=report-data-summary
+            report_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
+
+            # if it matches, wait a little longer and double deck that it hasn't changed
+            if prev_data_summary_elem == report_data_summary_elem:
+                time.sleep(3)
+                count += 3
+                report_data_summary_elem = self.driver.find_element(By.ID, 'report-data-summary').text
+                if prev_data_summary_elem == report_data_summary_elem:
+                    break
+            prev_data_summary_elem = report_data_summary_elem
+            time.sleep(1)
+
+            count += 1
+            if count >= self.wait_time:
+                raise TimeoutError('SchoolMint Report Data never did not fully load within %d' % self.wait_time)
+
+        # click the button to download the report
+        self.log.debug('Starting download...')
+        elem = self.driver.find_element(By.CLASS_NAME, "export-table")
+        elem.click()
+
+        # wait until file has downloaded to close the browser. We can do this
+        # because we delete the file before we return it, so the temp dir should
+        # always be empty when this command is run
+        wait_for_any_file_in_folder(csv_download_folder_path, "csv")
+
+        self.log.debug('Download finished.')
+        report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
+                                encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING, **pandas_read_csv_kwargs)
+
+        # TODO: move this out of this function. It should happen as cleanup once
+        # the whole DAG has completed
+        #delete_folder_contents(csv_download_folder_path)
+        shutil.rmtree(csv_download_folder_path)
+
+        # close the driver for this task
+        self.driver.close()
+
+        # if the dataframe is empty (the report had no data), raise an error
+        if report_df.shape[0] == 0:
+            #delete_folder_contents(csv_download_folder_path)
+            shutil.rmtree(csv_download_folder_path)
+            raise ValueError('No data in report for user {} at url: {}'.format(
+                self.username, interpret_report_url(self.base_url, report_url)))
+
+        return report_df
+
+    def __get_number_of_pages(self):
+        """Get the number of pages in a SchoolMint pagination."""
+        total_num_pages_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page][last()]'
+
+        elem = WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.XPATH, total_num_pages_xpath)))
+
+        num_pages = int(elem.get_attribute("data-page")) + 1
+
+        return num_pages
+
+    def __navigate_to_custom_report(self, report_name, school_year,
+                                    download_folder_path=None):
+        """Navigate to the page of the custom report tool that has the custom report on it"""
+        if not download_folder_path:
+            download_folder_path = self.temp_folder_path
+        self.driver = DriverBuilder().get_driver(
+            download_location=download_folder_path,
+            headless=self.headless
+        )
+        self._login()
+        # Clear pop-ups by reloading page
+        self.driver.get(self.base_url)
+        self._set_year(school_year, self.driver)
+
+        # get the custom reports page
+        custom_reports_url = 'report/customReports'
+        self.driver.get(interpret_report_url(self.base_url, custom_reports_url))
+        self.__remove_walk_me_and_support()
+
+        # wait for the page to load and get the maximum number of pages
+        total_num_pages_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page][last()]'
+
+        elem = WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.XPATH, total_num_pages_xpath)))
+
+        num_pages = int(elem.get_attribute("data-page")) + 1
+
+        current_page = 0
+        while current_page < num_pages:
+            report_name_xpath = "//tr[td//text()[contains(., '{}')]]".format(
+                report_name
+            )
+
+            try:
+                elem = self.driver.find_element(By.XPATH, report_name_xpath)
+                return current_page
+            except NoSuchElementException:
+                current_page += 1
+                if current_page < num_pages:
+                    next_page_xpath = '//*[@id="content"]//*[@class="pagination "]/li[@data-page={}]/a'.format(
+                        current_page
+                    )
+                    self.driver.find_element(By.XPATH, next_page_xpath).click()
+
+                    # scroll back to the top of the page, prevents selenium clicking errors
+                    self.driver.execute_script("window.scrollTo(0, 0);")
+
+        raise ReportNotFound
+
+    def generate_custom_report(self, report_name, school_year):
+        """
+        Clicks the generate button on a SchoolMint custom report.
+        :param report_name: The name of the report exactly as it is shown in the SchoolMint UI
+        :param school_year: The year in SchoolMint. Should be formatted as shown in the UI
+            (e.g. '2018-2019')
+        :return: True if the button was clicked. False if the button was not clicked because
+            the report is generating.
+        """
+        self.__navigate_to_custom_report(report_name, school_year)
+
+        if not self.check_school_year(school_year):
+            raise ReportNotFound("Wrong school detected prior to clicking generate.")
+
+        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
+        try:
+            generate_report_button = WebDriverWait(self.driver, self.wait_time).until(
+                EC.presence_of_element_located((By.XPATH, generate_report_button_xpath)))
+        except NoSuchElementException:
+            raise ReportNotFound
+
+        if generate_report_button.text == 'Generate Report':
+            generate_report_button.click()
+            self.driver.close()
+
+            return True
+        elif generate_report_button.text == 'Report in Progress':
+            self.driver.close()
+
+            return False
+        else:
+            raise ValueError("Unknown 'Generate Report' button text found")
+
+    def is_custom_report_generating(self, report_name, school_year):
+        """Checks if a SchoolMint Custom Report is generating or not"""
+        self.__navigate_to_custom_report(report_name, school_year)
+
+        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
+        try:
+            generate_report_button = WebDriverWait(self.driver, self.wait_time).until(
+                EC.presence_of_element_located((By.XPATH, generate_report_button_xpath)))
+        except NoSuchElementException:
+            raise ReportNotFound
+
+        if generate_report_button.text == 'Report in Progress':
+            return True
+        elif generate_report_button.text == 'Generate Report':
+            return False
+        else:
+            raise ValueError("Unknown 'Generate Report' button text found")
+
+    def get_last_custom_report_generation_datetime(self, report_name, school_year):
+        """Get's a report's generation timestamp in raw text"""
+        self.__navigate_to_custom_report(report_name, school_year)
+
+        try:
+            # old custom reports interface
+            report_generated_on_xpath = (
+                "//tr[td[./text()='{}']]/td[4]"
+            ).format(report_name)
+            report_generated_on_text = WebDriverWait(self.driver, self.wait_time).until(
+                EC.presence_of_element_located((By.XPATH, report_generated_on_xpath))).text
+        except TimeoutException:
+            try:
+                # new custom reports interface
+                report_generated_on_xpath = (
+                    "//tr[td[text()=' {} ']]/td[contains(@class,'last_generated_date-td')]"
+                ).format(report_name)
+                report_generated_on_text = WebDriverWait(self.driver, self.wait_time).until(
+                    EC.presence_of_element_located((By.XPATH, report_generated_on_xpath))).text
+            except TimeoutException:
+                raise ReportNotFound
+
+        return report_generated_on_text
+
+    def _download_custom_report(self, report_name, school_year, download_folder_path, download_if_generating=False):
+        """Protected function for clicking the download button on a report on the Custom Reports page"""
+        if not download_folder_path:
+            download_folder_path = self.temp_folder_path
+        self.__navigate_to_custom_report(report_name, school_year, download_folder_path)
+
+        generate_report_button_xpath = GENERATE_REPORT_BUTTON_XPATH.format(report_name=report_name)
+        generate_report_button_text = WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.XPATH, generate_report_button_xpath))).text
+
+        download_button_xpath = (
+            "//tr[td[text() = '{report_name}' or text() = ' {report_name} ']]//a[contains(text(), 'Download')]"
+        ).format(report_name=report_name)
+
+        elem = WebDriverWait(self.driver, self.wait_time).until(
+            EC.presence_of_element_located((By.XPATH, download_button_xpath)))
+
+        if generate_report_button_text == 'Generate Report':
+            elem.click()
+        elif generate_report_button_text == 'Report in Progress' and download_if_generating:
+            elem.click()
+        else:
+            raise ReportNotReady
+
+        return self.driver
+
+    def download_csv_custom_report(self, report_name, school_year, download_if_generating=False,
+                                   pandas_read_csv_kwargs={}):
+        """Download a SchoolMint Custom Report that downloads as a single CSV file"""
+        temp_folder_name = report_name.replace(" ", "_").lower()
+        csv_download_folder_path = self.temp_folder_path + '/' + temp_folder_name
+        driver = self._download_custom_report(report_name, school_year, csv_download_folder_path,
+                                              download_if_generating)
+
+        # wait until file has downloaded to close the browser. We can do this
+        # because we delete the file before we return it, so the temp dir should
+        # always be empty when this command is run
+        wait_for_any_file_in_folder(csv_download_folder_path, "csv")
+
+        report_df = pd.read_csv(get_most_recent_file_in_dir(csv_download_folder_path),
+                                encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING, **pandas_read_csv_kwargs)
+
+        # delete any files in the mealtime temp folder; we don't need them now
+        # TODO: move this out of this function. It should happen as cleanup once
+        # the whole DAG has completed
+        delete_folder_contents(csv_download_folder_path)
+
+        # close the driver for this task
+        driver.close()
+
+        # if the dataframe is empty (the report had no data), raise an error
+        if report_df.shape[0] == 0:
+            raise NoDataError('No data for user {} in Custom Report: {}'.format(self.username, report_name))
+
+        return report_df
+
+    def download_zip_custom_report(self, report_name, school_year, download_folder_path=None,
+                                   download_if_generating=False, unzip=True,
+                                   pandas_read_csv_kwargs={}):
+        """
+        Downloads a SchoolMint Custom Report that downloads as a zipped set of CSVs
+        :param report_name: The name of the report exactly as it is shown in the SchoolMint UI
+        :param school_year: The year in SchoolMint. Should be formatted as shown in the UI
+            (e.g. '2018-2019')
+        :param download_folder_path: The path to where you want to store the zip file.
+        :param download_if_generating: Whether or not to download a custom report if the
+            report is currently generating.
+        :param unzip: Boolean. If True, not only downloads the file, but also unzips it and
+            returns each csv in a Pandas Dataframe in a dictionary.
+        :param pandas_read_csv_kwargs: Additional keyward arguments to pass to Panda's read_csv function.
+        :return: None or a dictionary of Pandas DataFrames representing each of the CSVs in
+            the zipped file.
+        """
+        # create a folder for this specific run
+        run_time = datetime.datetime.utcnow()
+        if not download_folder_path:
+            download_folder_path = self.temp_folder_path
+        download_dir_final = "{}/{}-{}-{}".format(download_folder_path, report_name,
+                                                   run_time.strftime('%Y%m%d'), run_time.strftime('%H%M%S'))
+        driver = self._download_custom_report(report_name, school_year, download_dir_final, download_if_generating)
+
+        # wait until file has downloaded to close the browser. We can do this
+        # because we delete the file before we return it, so the temp dir should
+        # always be empty when this command is run
+        # TODO add a try/except block here
+        wait_for_any_file_in_folder(download_dir_final, "zip")
+
+        driver.close()
+
+        if unzip:
+            # unzip the files
+            file_path = max(glob.iglob(download_dir_final + '/*.zip'), key=os.path.getctime)
+            ZipfileLongPaths(file_path).extractall(download_dir_final)
+
+            dfs = dict()
+            # iterate through the unzipped files and load them into dataframes
+            for csv_filepath in glob.iglob(download_dir_final + '/*.csv'):
+                csv_filename = os.path.basename(csv_filepath)
+                #print(csv_filename)
+                # find the files that start with a number, these are the custom forms files
+                if re.match("^(\d+)", csv_filename):
+                    num_beg = re.match("^(\d+)", csv_filename).group(0)
+                    words = re.findall("[A-Za-z]+", csv_filename)
+                    dict_key = csv_filename # "{}_{}".format(num_beg, '_'.join(words[0:3])).lower()
+                    dfs[dict_key] = pd.read_csv(csv_filepath, encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING,
+                                                skiprows=[0, 2], **pandas_read_csv_kwargs)
+                # otherwise it is the info file that comes along with the zip export (application-data-export, etc.)
+                else:
+                    words = re.findall("[A-Za-z]+", csv_filename)
+                    dict_key = csv_filename # "{}".format('_'.join(words[0:3])).lower()
+
+                    dfs[dict_key] = pd.read_csv(csv_filepath, encoding=SCHOOLMINT_DEFAULT_EXPORT_ENCODING,
+                                                **pandas_read_csv_kwargs)
+
+            return dfs
```

### Comparing `duct-tape-0.25.2/ducttape/data_sources/seis.py` & `duct-tape-0.26.0/ducttape/data_sources/seis.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/summitlearning.py` & `duct-tape-0.26.0/ducttape/data_sources/summitlearning.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/data_sources/typingagent.py` & `duct-tape-0.26.0/ducttape/data_sources/typingagent.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/exceptions.py` & `duct-tape-0.26.0/ducttape/exceptions.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/httpsession.py` & `duct-tape-0.26.0/ducttape/httpsession.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/legacy.py` & `duct-tape-0.26.0/ducttape/legacy.py`

 * *Files identical despite different names*

### Comparing `duct-tape-0.25.2/ducttape/utils.py` & `duct-tape-0.26.0/ducttape/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,29 +87,33 @@
     elif report_url[0] == '/':
         return base_url + report_url
     else:
         return base_url + '/' + report_url
 
 
 def wait_for_any_file_in_folder(folder_path, file_format=None, timeout=60):
-    """ Waits until the first file shows up in a folder.
+    """
+    Waits until the first file shows up in a folder.
+    
+    Return:
+    file_found (bool): True if a file found; False if no file found.
     """
     count = 0
     if not file_format:
         file_found = False
         while count < timeout:
             for root, folders, files in os.walk(folder_path):
                 # break 'for' loop if files found
                 if files:
                     file_found = True
                     break
             print(files)
             # break 'while' loop if files found
             if file_found:
-                break
+                return True
             time.sleep(1)
     else:
         file_found = False
         while count < timeout:
             for root, folders, files in os.walk(folder_path):
                 for f in files:
                     if f.endswith(file_format):
@@ -120,16 +124,18 @@
                 # break 'for' loop if files found
                 if file_found:
                     print(files)
                     break
 
             # break 'while' loop if files found
             if file_found:
-                break
+                return True
             time.sleep(1)
+    # No file found before timeout
+    return False
 
 
 def correct_list_dataframe_dimensions(rows, columns):
 
     rows_modified = rows
 
     for row in rows_modified:
```

### Comparing `duct-tape-0.25.2/ducttape/webui_datasource.py` & `duct-tape-0.26.0/ducttape/webui_datasource.py`

 * *Files identical despite different names*

