# Comparing `tmp/automation-common-test-1.9.0.tar.gz` & `tmp/automation-common-test-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-common-test-1.9.0.tar", last modified: Mon May  8 15:44:42 2023, max compression
+gzip compressed data, was "automation-common-test-2.0.0.tar", last modified: Wed May 17 06:51:58 2023, max compression
```

## Comparing `automation-common-test-1.9.0.tar` & `automation-common-test-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 15:44:42.892399 automation-common-test-1.9.0/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 15:44:42.892208 automation-common-test-1.9.0/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-1.9.0/README.md
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 15:44:42.889469 automation-common-test-1.9.0/automation_common_test.egg-info/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-08 15:44:42.000000 automation-common-test-1.9.0/automation_common_test.egg-info/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      420 2023-05-08 15:44:42.000000 automation-common-test-1.9.0/automation_common_test.egg-info/SOURCES.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-08 15:44:42.000000 automation-common-test-1.9.0/automation_common_test.egg-info/dependency_links.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-08 15:44:42.000000 automation-common-test-1.9.0/automation_common_test.egg-info/top_level.txt
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 15:44:42.890573 automation-common-test-1.9.0/helpers/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-1.9.0/helpers/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-1.9.0/helpers/base_locator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     5510 2023-05-08 15:44:27.000000 automation-common-test-1.9.0/helpers/driver_manager.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-1.9.0/helpers/soft_check.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)    66006 2023-04-27 06:59:19.000000 automation-common-test-1.9.0/helpers/web_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-08 15:44:42.892456 automation-common-test-1.9.0/setup.cfg
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-08 15:44:40.000000 automation-common-test-1.9.0/setup.py
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-08 15:44:42.891872 automation-common-test-1.9.0/utils/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-1.9.0/utils/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-1.9.0/utils/config_parser.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-1.9.0/utils/encryption_decryption.py
--rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4591 2023-05-07 05:57:59.000000 automation-common-test-1.9.0/utils/post_results_teams.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.396601 automation-common-test-2.0.0/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-17 06:51:58.396368 automation-common-test-2.0.0/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-2.0.0/README.md
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.391125 automation-common-test-2.0.0/automation_common_test.egg-info/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      487 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-05-17 06:51:58.000000 automation-common-test-2.0.0/automation_common_test.egg-info/top_level.txt
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.393495 automation-common-test-2.0.0/helpers/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-2.0.0/helpers/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     2597 2023-05-16 05:29:45.000000 automation-common-test-2.0.0/helpers/api_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-2.0.0/helpers/base_locator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-05-17 01:07:02.000000 automation-common-test-2.0.0/helpers/decorator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     5157 2023-05-17 06:51:42.000000 automation-common-test-2.0.0/helpers/driver_manager.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-2.0.0/helpers/soft_check.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)    65913 2023-05-17 05:05:21.000000 automation-common-test-2.0.0/helpers/web_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-05-17 06:51:58.396649 automation-common-test-2.0.0/setup.cfg
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-05-17 06:51:42.000000 automation-common-test-2.0.0/setup.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-05-17 06:51:58.395851 automation-common-test-2.0.0/utils/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-2.0.0/utils/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-2.0.0/utils/config_parser.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-2.0.0/utils/encryption_decryption.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     4112 2023-05-17 05:11:54.000000 automation-common-test-2.0.0/utils/json_utils.py
+-rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4660 2023-05-09 03:29:52.000000 automation-common-test-2.0.0/utils/post_results_teams.py
```

### Comparing `automation-common-test-1.9.0/README.md` & `automation-common-test-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.9.0/helpers/driver_manager.py` & `automation-common-test-2.0.0/helpers/driver_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,75 +12,56 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.support.ui import WebDriverWait
 import logging
 from globals import browser
 
 driver_wait = 10
+current_os = platform.system()
 driver = None
-wait = None
-url = ""
-server = None
-
 logger = logging.getLogger(__name__)
 output_folder = os.path.join(os.getcwd(), "downloaded_files")
-current_os = platform.system()
 
 
-def create_driver():
-    web_driver = None
-    browser_type = browser.lower()
+
+def create_driver(browser_type, run_mode):
+    global driver
+    browser_type = browser_type
     if os.environ.get("Browser"):
         browser_type = os.environ.get("Browser").lower()
     if browser_type == "firefox":
         cap = DesiredCapabilities().FIREFOX
         cap["marionette"] = True
         firefox_options = webdriver.FirefoxOptions()
         firefox_options.set_preference("dom.disable_beforeunload", True)
-        web_driver = webdriver.Firefox(GeckoDriverManager.install(), options=firefox_options, capabilities=cap)
+        driver = webdriver.Firefox(GeckoDriverManager.install(), options=firefox_options, capabilities=cap)
     elif browser_type == "chrome":
         chrome_options = set_chrome_options()
-        if run_mode == "headless":
-            chrome_options.headless = True
+        if run_mode == "yes":
+            options.add_argument("--headless")
             chrome_options.add_argument("--window-size=1920,1080")
         warnings.filterwarnings(action="ignore", message="unclosed", category=ResourceWarning)
-        web_driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
+        driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
 
     elif browser_type == "ie":
         cap = DesiredCapabilities.INTERNETEXPLORER
         cap["NATIVE_EVENTS"] = False
-        web_driver = webdriver.Ie(IEDriverManager.install(), capabilities=cap)
+        driver = webdriver.Ie(IEDriverManager.install(), capabilities=cap)
     elif browser_type == "edge":
-        web_driver = webdriver.Edge(EdgeChromiumDriverManager.install())
-    web_driver.execute_script("document.body.style.zoom='100%'")
-    return web_driver
+        driver = webdriver.Edge(EdgeChromiumDriverManager.install())
+    driver.execute_script("document.body.style.zoom='100%'")
+    return driver
+
 
 
 def create_wait(timeout=driver_wait):
     web_driver_wait = WebDriverWait(driver, timeout)
     return web_driver_wait
 
 
-class create_driver_instance:
-
-    def get_driver(self):
-        global driver
-        global proxy_server
-        if not driver:
-            driver = create_driver()
-
-        return driver
-
-    def get_wait(self):
-        global wait
-        if not wait:
-            wait = create_wait()
-        return wait
-
-
 def capture_screenshot(image_name):
     driver.get_screenshot_as_file(image_name)
 
 
 def kill_driver_instance():
     global driver
     driver.close()
@@ -130,15 +111,15 @@
     options.add_argument("--disable-blink-features=AutomationControlled")
     options.add_argument("--disable-setuid-sandbox")
     options.add_argument("--disable-notifications")
     options.add_argument("--disable-popup-blocking")
     options.add_argument("--allow-insecure-localhost")
     options.add_argument('ignore-certificate-errors')
     options.add_experimental_option('excludeSwitches', ['enable-logging'])
-    options.addArguments("--headless")
+    # options.add_argument("--headless")
     preferences = {
         "profile.default_content_setting_values.automatic_downloads": 1,
         "download.default_directory": output_folder,
         "download.prompt_for_download": False,
         "download.directory_upgrade": True,
         "safebrowsing.enabled": True
     }
```

### Comparing `automation-common-test-1.9.0/helpers/soft_check.py` & `automation-common-test-2.0.0/helpers/soft_check.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.9.0/helpers/web_operations.py` & `automation-common-test-2.0.0/helpers/web_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.support import expected_conditions as EC
 import time
 import os
+import logging as logger
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import *
-from helpers.driver_manager import logger, driver, driver_wait, current_os, create_driver_instance
+from helpers.driver_manager import create_driver, create_wait, current_os
 
 """Class that wraps selenium functions to be used in UI automation tests
 """
 
 wait_msg = "Locator --> {}"
-driver = create_driver_instance().get_driver()
-_driver_wait = create_driver_instance().get_wait()
-wait = create_driver_instance().get_wait()
-
-
-# def __init__(driver: WebDriver, wait: WebDriverWait):
-#     driver: WebDriver = driver
-#     wait = wait
-#     _driver_wait: WebDriverWait = wait
+_driver_wait = None
 
 
+def create_driver_instance(browser_type, run_mode):
+    global driver
+    global _driver_wait
+    driver = create_driver(browser_type, run_mode)
+    _driver_wait = create_wait()
+    
+    
 class WaitForDocReady(object):
     """Class that allows to verify if the document (page) is loaded
     """
 
     def __call__(self, driver: WebDriver):
         """Execute a script to validate if the document is in ready state
 
@@ -43,22 +43,21 @@
 def _setup_wrapper(wait_time=None, wait_for_load=False):
     """Setup some internal functionalites to use in each selenium wrapper function
 
     Args:
         wait_time (float, optional): Optional wait time if the default wait want to be skipped. Defaults to None.
         wait_for_load (bool, optional): Allow to wait for the page to load. Defaults to False.
     """
+    global  _driver_wait
     # If wait time is specified it doesn't affect the wait for doc ready
     if wait_for_load:
-        wait.until(WaitForDocReady())
+        _driver_wait.until(WaitForDocReady())
     if wait_time:
         ignored_exceptions = (StaleElementReferenceException,)
         _driver_wait = WebDriverWait(driver, wait_time, ignored_exceptions=ignored_exceptions)
-    else:
-        _driver_wait = wait
 
 
 """
 ------------------------------------------------------------------------
 Elements Operations    
 ------------------------------------------------------------------------
 """
@@ -282,15 +281,15 @@
         actual_count = len(elems)
     except (NoSuchElementException, TimeoutException):
         return 0
     logger.info(f"Got number of elements of: {elem_name} with value {value} as: {len(elems)}")
     return actual_count
 
 
-def get_element_text(self, locator, elem_name, wait_time=None):
+def get_element_text(locator, elem_name, wait_time=None):
     """Allow to get the text of a element using selenium
 
     Args:
         locator (tuple): tuple with locator type and locator string
         elem_name (str): description of the element
         wait_time (float, optional): custom wait time for the elements, skips driver default wait time
 
@@ -1422,15 +1421,15 @@
 
     Args:
         locator (tuple): tuple with locator type and locator string
         elem_name (str): description of the element
         wait_time (float, optional): custom wait time for the elements, skips driver default wait time
     """
     _setup_wrapper(wait_time, wait_for_load=True)
-    elem = driver_wait.until(EC.visibility_of_element_located((locator[0], locator[1])),
+    elem = _driver_wait.until(EC.visibility_of_element_located((locator[0], locator[1])),
                              wait_msg.format(locator))
     elem.send_keys(Keys.ARROW_DOWN)
     logger.info(f"Arrow down was pressed on {elem_name}")
 
 
 def switch_to_iframe(locator, wait_time=None):
     """Allow to switch to an iframe using selenium
```

### Comparing `automation-common-test-1.9.0/utils/encryption_decryption.py` & `automation-common-test-2.0.0/utils/encryption_decryption.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-1.9.0/utils/post_results_teams.py` & `automation-common-test-2.0.0/utils/post_results_teams.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 -------------------------------------------------------------------
 """
 
 class_set = set()
 project_name = None
 
 
-def post_reports_to_teams(build_url, webhook_url):
+def post_reports_to_teams(env_url, webhook_url):
     global class_set
     result_dict = defaultdict(list)
     xml = get_xml_report()
     if xml.tests > 0:
         for suite in xml:
             for case in suite:
                 if case.classname and "tests" in case.classname:
                     class_set.add(case.classname)
                     result_dict[get_feature_name(case.classname)].append(translate_result(case.result))
-        create_payload(generate_result(result_dict), xml, build_url, webhook_url)
+        create_payload(generate_result(result_dict), xml, env_url, webhook_url)
 
 
 def translate_result(result):
     result_list = ['failure', 'skipped', 'error']
     if len(result) > 0:
         test = str(result).split(' ')[1].replace("'", "")
         if test in result_list:
@@ -59,25 +59,26 @@
         final_data = project_name.upper() + " - " + key.replace("_", " ").title() + " - " + "Passed: " + integer(
             res_dict.get('PASSED')) + " " + "Failed: " + integer(
             res_dict.get('FAILURE')) + " " + "Skipped: " + integer(res_dict.get('SKIPPED'))
         payload_data += final_data + '<br>'
     return payload_data
 
 
-def create_payload(final_payload, xml, build_url, webhook_url):
+def create_payload(final_payload, xml, env_url, webhook_url):
     total_tests = int(xml.tests)
     failed_error_skipped = xml.failures + xml.skipped + xml.errors
     failed_tests = xml.failures
     passed_tests = xml.tests - failed_error_skipped
+    build_url="https://dev.azure.com/Kyndryl-Sandbox/appmmm-automation/_build"
     if passed_tests > 0 or failed_tests > 0:
         pass_percent = round(float(passed_tests * 100 / total_tests), 2)
-        payload = f"**UI Automation Test Results:** <br><br>"f"**Project:** {project_name.upper()}<br>"f"**Environment:** {build_url}<br>" f"**Build:** {build_url}<br><br>"f"**Total TestCases Executed:** {total_tests}<br>" f"**Passed:** {passed_tests}<br>"f"**Failed:** {xml.failures}<br>"f"**Skipped:** {xml.skipped + xml.errors}<br>"f"**Pass Percentage:** {pass_percent}{'%'}<br><br>"f"**Feature-wise Summary:**<br> " + '<br>'
+        payload = f"**UI Automation Test Results:** <br><br>"f"**Project:** {project_name.upper()}<br>"f"**Environment:** {env_url}<br>" f"**Build:** {build_url}<br><br>"f"**Total TestCases Executed:** {total_tests}<br>" f"**Passed:** {passed_tests}<br>"f"**Failed:** {xml.failures}<br>"f"**Skipped:** {xml.skipped + xml.errors}<br>"f"**Pass Percentage:** {pass_percent}{'%'}<br><br>"f"**Feature-wise Summary:**<br> " + '<br>'
         payload += final_payload
     else:
-        payload = f"**UI Automation Test Results:** <br>"f"**Project:** {project_name.upper()}<br>"f"**Environment:** https://{build_url}<br>" f"**Build:** {build_url}<br><br>"f"All the test cases are skipped please look into it"
+        payload = f"**UI Automation Test Results:** <br>"f"**Project:** {project_name.upper()}<br>"f"**Environment:** https://{env_url}<br>" f"**Build:** {build_url}<br><br>"f"All the test cases are skipped please look into it"
     post_request(payload, webhook_url)
     print(payload)
 
 
 def post_request(payload, webhook_url):
     headers = {"Content-Type": "application/json"}
     team_response = requests.post(url=webhook_url, json={"text": payload}, headers=headers)
```

