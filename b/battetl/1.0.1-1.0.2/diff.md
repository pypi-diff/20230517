# Comparing `tmp/battetl-1.0.1.tar.gz` & `tmp/battetl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.0.1.tar", last modified: Thu Apr 13 23:31:40 2023, max compression
+gzip compressed data, was "battetl-1.0.2.tar", last modified: Wed May 17 03:39:42 2023, max compression
```

## Comparing `battetl-1.0.1.tar` & `battetl-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.405179 battetl-1.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-04 20:46:42.000000 battetl-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    14919 2023-04-13 23:31:40.404173 battetl-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14366 2023-04-13 22:40:48.000000 battetl-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.378146 battetl-1.0.1/battetl/
--rw-rw-rw-   0        0        0     7291 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/BattETL.py
--rw-rw-rw-   0        0        0      116 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/__init__.py
--rw-rw-rw-   0        0        0     8243 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.392654 battetl-1.0.1/battetl/extract/
--rw-rw-rw-   0        0        0    27305 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/extract/Extractor.py
--rw-rw-rw-   0        0        0       34 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/extract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.397666 battetl-1.0.1/battetl/load/
--rw-rw-rw-   0        0        0    33698 2023-04-11 19:33:26.000000 battetl-1.0.1/battetl/load/Loader.py
--rw-rw-rw-   0        0        0       28 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/load/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.401142 battetl-1.0.1/battetl/transform/
--rw-rw-rw-   0        0        0    23437 2023-04-10 18:26:06.000000 battetl-1.0.1/battetl/transform/Transformer.py
--rw-rw-rw-   0        0        0       38 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/transform/__init__.py
--rw-rw-rw-   0        0        0    12219 2023-04-05 19:58:40.000000 battetl-1.0.1/battetl/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 23:31:40.388146 battetl-1.0.1/battetl.egg-info/
--rw-rw-rw-   0        0        0    14919 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 23:31:40.000000 battetl-1.0.1/battetl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 23:31:40.405179 battetl-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-04-13 23:21:25.000000 battetl-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.841215 battetl-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-04 20:46:42.000000 battetl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    15489 2023-05-17 03:39:42.839217 battetl-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14936 2023-05-10 20:47:12.000000 battetl-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.760103 battetl-1.0.2/battetl/
+-rw-rw-rw-   0        0        0     7350 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/BattETL.py
+-rw-rw-rw-   0        0        0      116 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/__init__.py
+-rw-rw-rw-   0        0        0     8802 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.802620 battetl-1.0.2/battetl/extract/
+-rw-rw-rw-   0        0        0    27305 2023-04-10 18:26:06.000000 battetl-1.0.2/battetl/extract/Extractor.py
+-rw-rw-rw-   0        0        0       34 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/extract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.813622 battetl-1.0.2/battetl/load/
+-rw-rw-rw-   0        0        0    36511 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/load/Loader.py
+-rw-rw-rw-   0        0        0       79 2023-04-26 18:52:26.000000 battetl-1.0.2/battetl/load/__init__.py
+-rw-rw-rw-   0        0        0     6816 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/load/batt_db_test_helper.py
+-rw-rw-rw-   0        0        0     1728 2023-05-10 20:47:12.000000 battetl-1.0.2/battetl/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.819625 battetl-1.0.2/battetl/transform/
+-rw-rw-rw-   0        0        0    26425 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/transform/Transformer.py
+-rw-rw-rw-   0        0        0       38 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/transform/__init__.py
+-rw-rw-rw-   0        0        0    12452 2023-04-26 18:52:26.000000 battetl-1.0.2/battetl/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.793621 battetl-1.0.2/battetl.egg-info/
+-rw-rw-rw-   0        0        0    15489 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:39:42.841215 battetl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-04-24 19:52:15.000000 battetl-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.836217 battetl-1.0.2/tests/
+-rw-rw-rw-   0        0        0     4494 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_BattETL.py
+-rw-rw-rw-   0        0        0    17547 2023-04-26 18:52:26.000000 battetl-1.0.2/tests/test_Extractor.py
+-rw-rw-rw-   0        0        0    26574 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_Loader.py
+-rw-rw-rw-   0        0        0    12554 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_Transformer.py
+-rw-rw-rw-   0        0        0     2532 2023-04-11 19:33:26.000000 battetl-1.0.2/tests/test_utils.py
```

### Comparing `battetl-1.0.1/LICENSE` & `battetl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `battetl-1.0.1/PKG-INFO` & `battetl-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1
-Name: battetl
-Version: 1.0.1
-Summary: A Python module for extracting, transforming, and loading battery data to a database.
-Home-page: https://github.com/BattGenie/battetl
-Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
-Author-email: info@battgenie.life
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
 
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
 <img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
@@ -70,34 +57,44 @@
 
 ## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
 ### Requirements
 
-BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
 
 ### Installation Instructions
 
-Install BattETL using pip:
+- Install BattETL using pip:
 
 ```sh
 pip install battetl
 ```
 
-Install BattETL from source code:
+- Install BattETL from source code:
 
 ```sh
 git clone https://github.com/BattGenie/battetl.git
 cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
 ## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
```

### Comparing `battetl-1.0.1/README.md` & `battetl-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: battetl
+Version: 1.0.2
+Summary: A Python module for extracting, transforming, and loading battery data to a database.
+Home-page: https://github.com/BattGenie/battetl
+Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
+Author-email: info@battgenie.life
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
+
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
 <img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
 ## Overview
@@ -55,34 +72,44 @@
 
 ## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
 ### Requirements
 
-BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
 
 ### Installation Instructions
 
-Install BattETL using pip:
+- Install BattETL using pip:
 
 ```sh
 pip install battetl
 ```
 
-Install BattETL from source code:
+- Install BattETL from source code:
 
 ```sh
 git clone https://github.com/BattGenie/battetl.git
 cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
 ## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
```

### Comparing `battetl-1.0.1/battetl/BattETL.py` & `battetl-1.0.2/battetl/BattETL.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         # Schedule
         if self.config.get('schedule_file_path'):
             try:
                 extractor.schedule_from_files(
                     self.config['schedule_file_path'])
                 self.schedule = extractor.schedule
-                self.config['meta_data']['schedule_meta']['schedule_files'] = json.dumps(extractor.schedule)
+                self.config['meta_data']['schedule_meta']['details'] = json.dumps(extractor.schedule)
             except Exception as e:
                 logger.error('Failed to extract schedule', exc_info=True)
                 logger.error(e)
         else:
             logger.warning('No schedule file path')
 
         return self
@@ -134,19 +134,19 @@
                 self.cycle_stats = transformer.cycle_stats
             except Exception as e:
                 logger.error('Failed to transform cycle stats', exc_info=True)
                 logger.error(e)
         else:
             logger.warning('No cycle stats to transform.')
 
-        if self.schedule and 'cv_voltage_thresh_mv' in self.config:
+        if self.schedule and 'cv_voltage_threshold_mv' in self.config['meta_data']['schedule_meta']:
             try:
                 transformer.calc_cycle_stats(
                     self.schedule['steps'],
-                    self.config['cv_voltage_thresh_mv'])
+                    self.config['meta_data']['schedule_meta']['cv_voltage_threshold_mv'])
                 self.cycle_stats = transformer.cycle_stats
             except Exception as e:
                 logger.error('Failed to calculate cycle stats', exc_info=True)
                 logger.error(e)
         else:
             logger.warning('Skipping cycle stats calculation.')
```

### Comparing `battetl-1.0.1/battetl/constants.py` & `battetl-1.0.2/battetl/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 class Constants:
     DEFAULT_TIME_ZONE = 'America/Los_Angeles'
 
+    DATABASE_MAX_RETRIES = 10
+    DATABASE_RETRY_DELAY = 10
+    DATABASE_MAX_RETRY_DELAY = 60
+
     MAKE_ARBIN = 'arbin'
     MAKE_MACCOR = 'maccor'
     DATA_TYPE_TEST_DATA = 'test_data'
     DATA_TYPE_CYCLE_STATS = 'cycle_stats'
 
     MACCOR_PROCEDURE_FILE_ENCODING = 'UTF-8'
 
@@ -26,15 +30,15 @@
         'test_time_s',
         'step_time_s',
         'current_ma',
         'voltage_mv',
         'recorded_datetime',
         'unixtime_s',
         'thermocouple_temp_c',
-        'other_detail',
+        'other_details',
     }
     COLUMNS_CYCLE_STATS = {
         'cycle_stats_id',
         'test_id',
         'cycle',
         'test_time_s',
         'reported_charge_capacity_mah',
@@ -53,15 +57,15 @@
         'calculated_cv_capacity_mah',
         'reported_coulombic_efficiency',
         'calculated_coulombic_efficiency',
         'calculated_fifty_percent_charge_time_s',
         'calculated_eighty_percent_charge_time_s',
         'calculated_charge_energy_mwh',
         'calculated_discharge_energy_mwh',
-        'other_detail',
+        'other_details',
     }
     COLUMNS_ARBIN_TEST_DATA_ONLY = {
         'Date Time',
         'ACR (Ohm)',
         'dQ/dV (Ah/V)',
         'Internal Resistance (Ohm)',
         'dV/dQ (V/Ah)',
@@ -84,14 +88,26 @@
         'Capacity(Ah)',
         'Step',
         'EV Temp',
         'Voltage(V)',
         'TestTime(s)',
         'Temp 1',
     }
+
+    COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY = {
+        'Rec',
+        'Cycle P',
+        'Cycle C',
+        'Capacity',
+        'Energy',
+        'MD',
+        'ES',
+        'DPT Time',
+    }
+
     COLUMNS_MACCOR_CYCLE_STATS_ONLY = {
         'T1_End',
         'T1_Max',
         'T1_Start',
         'T1_Min',
         'Cycle',
         'Date',
@@ -99,14 +115,16 @@
         'AH-IN',
     }
 
     COLUMNS_TO_MILLI = {
         # Test Data
         'voltage_v': 'voltage_mv',
         'current_a': 'current_ma',
+        'voltage': 'voltage_mv',
+        'current': 'current_ma',
         'charge_capacity_ah': 'charge_capacity_mah',
         'discharge_capacity_ah': 'discharge_capacity_mah',
         'charge_energy_wh': 'charge_energy_mwh',
         'discharge_energy_wh': 'discharge_energy_mwh',
         'power_w': 'power_mw',
         'impedance_ohm': 'impedance_mohm',
         'capacity_ah': 'capacity_mah',
@@ -114,14 +132,16 @@
         'arbin_charge_capacity_ah': 'arbin_charge_capacity_mah',
         'arbin_discharge_capacity_ah': 'arbin_discharge_capacity_mah',
         'arbin_charge_energy_wh': 'arbin_charge_energy_mwh',
         'arbin_discharge_energy_wh': 'arbin_discharge_energy_mwh',
         # Maccor Test Data
         'maccor_capacity_ah': 'maccor_capacity_mah',
         'maccor_energy_wh': 'maccor_energy_mwh',
+        'capacity': 'maccor_capacity_mah',
+        'energy': 'maccor_energy_mwh',
         # Arbin Cycle Stats
         'reported_charge_capacity_ah': 'reported_charge_capacity_mah',
         'reported_discharge_capacity_ah': 'reported_discharge_capacity_mah',
         'reported_charge_energy_wh': 'reported_charge_energy_mwh',
         'reported_discharge_energy_wh': 'reported_discharge_energy_mwh',
     }
 
@@ -184,17 +204,20 @@
         'Charge Energy (Wh)': 'reported_charge_energy_wh',
         'Charge_Energy(Wh)': 'reported_charge_energy_wh',
         'Discharge Energy (Wh)': 'reported_discharge_energy_wh',
         'Discharge Energy(Wh)': 'reported_discharge_energy_wh',
     }
     COLUMNS_MAPPING_MACCOR_TEST_DATA = {
         'Cyc#': 'cycle',
+        'Cycle P': 'cycle',
         'Step': 'step',
         'TestTime(s)': 'test_time_s',
+        'Test Time': 'test_time_s',
         'StepTime(s)': 'step_time_s',
+        'Step Time': 'step_time_s',
         'Capacity(Ah)': 'maccor_capacity_ah',
         'Watt-hr': 'maccor_energy_wh',
         'Current(A)': 'current_a',
         'Voltage(V)': 'voltage_v',
         'DPt Time': 'recorded_datetime',
         'EV Temp': 'ev_temp_c',
     }
```

### Comparing `battetl-1.0.1/battetl/extract/Extractor.py` & `battetl-1.0.2/battetl/extract/Extractor.py`

 * *Files identical despite different names*

### Comparing `battetl-1.0.1/battetl/load/Loader.py` & `battetl-1.0.2/battetl/load/Loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from battetl import logger, Constants, Utils
 import os
 import copy
 import json
+import time
 import psycopg2
 import psycopg2.pool
 import psycopg2.sql
 import sqlalchemy
 import sqlalchemy.orm
 import numpy as np
 import pandas as pd
-from schema import Schema, Use, Optional, SchemaError
+from schema import Schema, Use, Optional, And, SchemaError
 
 # progress bar
 from tqdm import tqdm
 # register the pandas extension
 tqdm.pandas()
 
-from battetl import logger, Constants, Utils
-
 
 class Loader:
     def __init__(
             self,
             config: dict,
             env_path: str = os.path.join(os.getcwd(), '.env')):
         """
@@ -82,21 +82,27 @@
                 Optional('lower_voltage_limit_v'): Use(float),
                 Optional('upper_voltage_limit_v'): Use(float),
             },
             'schedule_meta': {
                 'schedule_name': str,
                 'cycler_make': str,
                 Optional('schedule_id'): Use(int),
-                Optional('test_type'): str,
+                Optional('test_type'): And(
+                    str,
+                    lambda s: s in [
+                        'ICT', 'Characterization', 'Baseline life cycling',
+                        'MBC life cycling', 'MBC quick test', 'Pretest', 'HPPC'
+                    ]
+                ),
                 Optional('cycler_make'): str,
                 Optional('date_created'): str,
                 Optional('created_by'): str,
                 Optional('comments'): str,
                 Optional('cv_voltage_threshold_mv'): Use(float),
-                Optional('schedule_files'): str,
+                Optional('details'): str,
             },
             'cell': {
                 'manufacturer_sn': str,
                 Optional('cell_id'): Use(int),
                 Optional('cell_type_id'): Use(int),
                 Optional('batch_number'): str,
                 Optional('label'): str,
@@ -112,58 +118,90 @@
                 'manufacturer': str,
                 'manufacturer_pn': str,
                 Optional('cell_type_id'): Use(int),
                 Optional('form_factor'): str,
                 Optional('capacity_mah'): Use(float),
                 Optional('chemistry'): str,
                 Optional('dimensions'): str,
+                Optional('datasheet'): str,  # File path
             },
         })
 
         assert (self.__validate_config(config))
         assert (self.__create_connection())
 
-    def load_test_data(self, df: pd.DataFrame) -> int:
+    def load_test_data(self, df: pd.DataFrame, retry_cnt: int = 0) -> int:
         """
         Loads test data to the target database. Only loads data past the
         latest `unixtime_s` field that already exists in the `test_data` table.
 
         Parameters
         ----------
         df : pd.DataFrame
             Data Frame containing test data to load to database.
+        retry_cnt : int, optional
+            The number of times to retry loading data to the database.
 
         Returns
         -------
         num_rows_loaded : int
             The number of rows inserted into the `data` table.
         """
+        logger.info('Loading test data to database')
 
-        df_copy = df.copy(deep=True)
+        num_rows_loaded = 0
 
-        # Move fields to other_detail
-        df_copy = self.__create_other_detail(
-            df_copy, Constants.COLUMNS_TEST_DATA)
+        df_copy = df.copy(deep=True)
 
-        for column in df_copy.columns:
-            if column not in Constants.COLUMNS_TEST_DATA:
-                logger.debug(f'Dropping column {column} from DataFrame')
-                df_copy = df_copy.drop([column], axis=1)
+        try:
+            if retry_cnt > 0:
+                logger.info(f'Retry count: {retry_cnt}')
+                # Re-create connection
+                self.__create_connection()
+
+            latest_unixtime_s = self.__lookup_latest_unixtime()
+            if latest_unixtime_s:
+                df_copy = df_copy[df_copy['unixtime_s'] > latest_unixtime_s]
+
+            if df_copy.shape[0] > 0:
+                # Move fields to other_details
+                df_copy = self.__create_other_details(
+                    df_copy, Constants.COLUMNS_TEST_DATA)
+
+                for column in df_copy.columns:
+                    if column not in Constants.COLUMNS_TEST_DATA:
+                        logger.debug(
+                            f'Dropping column {column} from DataFrame')
+                        df_copy = df_copy.drop([column], axis=1)
+
+                test_id = self.__lookup_test_id()
+                if not test_id:
+                    test_id = self.__insert_test_meta()
+                df_copy['test_id'] = np.ones(
+                    df_copy.shape[0], dtype=np.uint16) * test_id
 
-        test_id = self.__lookup_test_id()
-        if not test_id:
-            test_id = self.__insert_test_meta()
-        df_copy['test_id'] = np.ones(
-            df_copy.shape[0], dtype=np.uint16) * test_id
+                num_rows_loaded += self.__load_dataframe(
+                    df=df_copy, target_table='test_data')
+        except Exception as e:
+            logger.error('Error loading test data')
+            if retry_cnt < Constants.DATABASE_MAX_RETRIES:
+                logger.info(
+                    f'Retrying load_test_data() {retry_cnt+1}/{Constants.DATABASE_MAX_RETRIES}')
+                retry_delay = min(Constants.DATABASE_RETRY_DELAY *
+                                  (retry_cnt+1), Constants.DATABASE_MAX_RETRY_DELAY)
+                logger.info(f'Retry delay: {retry_delay} seconds')
+                time.sleep(retry_delay)
 
-        latest_unixtime_s = self.__lookup_latest_unixtime()
-        if latest_unixtime_s:
-            df_copy = df_copy[df_copy['unixtime_s'] > latest_unixtime_s]
+                num_rows_loaded += self.load_test_data(
+                    df=df_copy, retry_cnt=retry_cnt+1)
+            else:
+                logger.error(f'Exceeded max retries for load_test_data()')
+                raise e
 
-        return self.__load_dataframe(df=df_copy, target_table='test_data')
+        return num_rows_loaded
 
     def load_cycle_stats(self, df: pd.DataFrame) -> int:
         """
         Loads cycle stats to the target database. Any cycles that already exist in the 
         database that overlap with the new cycle data will be overwritten. 
 
         Parameters
@@ -172,19 +210,20 @@
             Data Frame containing test data to load to database.
 
         Returns
         -------
         num_rows_loaded : int
             The number of rows inserted into the `test_data` table.
         """
+        logger.info('Loading cycle stats to database')
 
         df_copy = df.copy(deep=True)
 
-        # Move fields to other_detail
-        df_copy = self.__create_other_detail(
+        # Move fields to other_details
+        df_copy = self.__create_other_details(
             df_copy, Constants.COLUMNS_CYCLE_STATS)
 
         for column in df_copy.columns:
             if column not in Constants.COLUMNS_CYCLE_STATS:
                 logger.debug(f'Dropping column {column} from DataFrame')
                 df_copy = df_copy.drop([column], axis=1)
 
@@ -206,15 +245,16 @@
                 WHERE
                     test_id = {test_id}
                 AND 
                     cycle >= {newest_cycle}
                 ORDER BY cycle_stats_id ASC
             """).format(
                 test_id=psycopg2.sql.Literal(str(test_id)),
-                newest_cycle=psycopg2.sql.Literal(str(int(df_copy.cycle.iloc[0])))
+                newest_cycle=psycopg2.sql.Literal(
+                    str(int(df_copy.cycle.iloc[0])))
             )
             cursor.execute(stmt)
             result = cursor.fetchall()
         if result:
             duplicate_stats_id_bounds = [result[0][0], result[-1][0]]
             duplicate_cycle_range = [result[1][0], result[-1][0]]
             logger.info(
@@ -344,47 +384,45 @@
         except Exception as e:
             logger.error(f'Unexpected error creating connection to database {os.getenv("DB_TARGET")}!',
                          exc_info=True)
             logger.error(e)
 
         return success
 
-    def __create_other_detail(self, df: pd.DataFrame, table_columns: set) -> pd.DataFrame:
+    def __create_other_details(self, df: pd.DataFrame, table_columns: set) -> pd.DataFrame:
         """
-        Creates the other_detail column in the DataFrame. This column contains
+        Creates the other_details column in the DataFrame. This column contains
         all fields that are not in the target table.
 
         Parameters
         ----------
         df : pd.DataFrame
-            DataFrame to create other_detail column
+            DataFrame to create other_details column
         table_columns : set
             Set of columns in the target table
 
         Returns
         -------
         df : pd.DataFrame
-            DataFrame with other_detail column
+            DataFrame with other_details column
         """
-        other_detail_columns = set(df.columns) - set(table_columns)
+        other_details_columns = set(df.columns) - set(table_columns)
 
-        if other_detail_columns:
+        if other_details_columns:
             logger.info(
-                f'Move fields to other_detail: {", ".join(other_detail_columns)}')
-            df['other_detail'] = df.progress_apply(
+                f'Move fields to other_details: {", ".join(other_details_columns)}')
+            df['other_details'] = df.progress_apply(
                 lambda row: json.dumps({
-                    c: row[c] for c in other_detail_columns if not pd.isnull(row[c])
+                    c: row[c] for c in other_details_columns if not pd.isnull(row[c])
                 }),
                 axis=1,
             )
 
         return df
 
-    # TODO: Modify query so that test_name is used in conjunction with start_date
-
     def __lookup_test_id(self) -> int:
         """
         Looks up the test_id in the target database based on the test_name defined
         within the config. If no entry exists then None is returned.
 
         Returns
         -------
@@ -671,14 +709,27 @@
         -------
         cell_type_id : int
             The cell_type_id for the newly inserted cell_meta. None if the insert failed.
         """
         upload_dict = copy.deepcopy(self.config['cell_meta'])
 
         logger.debug(f'Inserting cell_meta: {json.dumps(upload_dict)}')
+
+        # Check if 'datasheet' key exists in upload_dict and the file exists
+        if 'datasheet' in upload_dict:
+            if os.path.exists(upload_dict['datasheet']):
+                logger.info(f'Found datasheet file: {upload_dict["datasheet"]}')
+                # Convert pdf file to binary data
+                with open(upload_dict['datasheet'], 'rb') as f:
+                    datasheet_data = f.read()
+                # Add binary data to upload_dict
+                upload_dict['datasheet'] = datasheet_data
+            else:
+                logger.error(f'Could not find datasheet file: {upload_dict["datasheet"]}')
+
         return self.__perform_insert(target_table='cells_meta', dict_to_load=upload_dict, pk_id_col='cell_type_id')
 
     def __insert_schedule_meta(self) -> int:
         """
         Inserts a new entry in `schedule_meta` table based on info in the config.
 
         Returns
@@ -743,15 +794,21 @@
         -------
         pk_id : int
             The primary key id for the newly inserted row. Returns None if issue with inserting rows.
         """
 
         # Remove any empty entries from upload dict
         dict_to_load = {k: v for k, v in dict_to_load.items() if v}
-        logger.debug(f'Inserting into {target_table} with {json.dumps(dict_to_load)}')
+        log_dict_to_load = dict(dict_to_load)
+        for k, v in log_dict_to_load.items():
+            # Convert binary data to string for logging
+            if isinstance(v, bytes):
+                log_dict_to_load[k] = '[binary data]'
+        logger.debug(
+            f'Inserting into {target_table} with {log_dict_to_load}')
         pk_id = None
 
         try:
             insert_statement = psycopg2.sql.SQL(
                 "INSERT INTO {table} ({cols}) VALUES ({vals}) RETURNING {pk_id}").format(
                 table=psycopg2.sql.Identifier(target_table),
                 cols=psycopg2.sql.SQL(', ').join(
@@ -771,15 +828,16 @@
                 logger.error(
                     f'No result returned when inserting into {target_table} with pk_id_col={pk_id_col}')
         except psycopg2.Error as e:
             logger.error(
                 f'Error inserting into {target_table} with pk_id_col={pk_id_col}')
             logger.error(e)
         except Exception as e:
-            logger.error(f'Unexpected error inserting into {target_table} with pk_id_col={pk_id_col}')
+            logger.error(
+                f'Unexpected error inserting into {target_table} with pk_id_col={pk_id_col}')
             logger.error(e)
 
         return pk_id
 
     def __lookup_latest_unixtime(self) -> int:
         """
         Looks up the latest `unixtime_s` loaded into the `test_data` table for the
@@ -790,16 +848,17 @@
         -------
         latest_unixtime_s : float
             The latest unixtime_s in the `test_data` table for the test.
         """
 
         test_id = self.__lookup_test_id()
         if not test_id:
+            test_name = self.config['test_meta']['test_name']
             logger.info(
-                f'No test data exists for {test_id}, OK to upload all data.')
+                f'No test data exists for "{test_name}", OK to upload all data.')
             return None
 
         with self.conn.cursor() as cursor:
             cursor.execute("""
                 SELECT
                     MAX(unixtime_s)
                 FROM
@@ -902,9 +961,11 @@
             logger.error(
                 f'Error inserting into {target_table} table')
             logger.error(e)
         except Exception as e:
             logger.error(
                 f'Unexpected error inserting into {target_table} table.')
             logger.error(e)
+            if target_table == 'test_data':
+                raise e
 
         return num_rows_inserted
```

### Comparing `battetl-1.0.1/battetl/logger.py` & `battetl-1.0.2/battetl/logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import datetime
 from dotenv import load_dotenv
 from logging.handlers import RotatingFileHandler
 
 load_dotenv()
 
 LOG_MAX_SIZE = 10 * 1024 * 1024  # 10 MB
+STREAM_LOG_MAX_LENGTH = 1000
 MODULE_DIR = os.path.abspath(os.path.dirname(__file__))
 LOG_DIR = os.path.join(MODULE_DIR, "logs")
 if not os.path.isdir(LOG_DIR):
     os.mkdir(LOG_DIR)
 LOG_FILE_NAME = 'battetl.log'
 LOG_FILE_PATH = os.path.join(LOG_DIR, LOG_FILE_NAME)
 
@@ -22,24 +23,24 @@
 # ----------
 # YYYY-MM-DD HH:MM:SS LEVEL [MODULE:LINENO] MESSAGE
 # asctime: Human-readable time when the LogRecord was created.
 # levelname: Text logging level for the message ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL').
 # module: The module (name portion of filename).
 # lineno: Source line number where the logging call was issued (if available).
 # message: The logged message.
-LOG_FORMAT = '%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message)s'
-
 logger = logging.getLogger('battetl')
 
-formatter_stream = logging.Formatter(fmt=LOG_FORMAT)
+log_format_stream = f'%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message).{STREAM_LOG_MAX_LENGTH}s'
+formatter_stream = logging.Formatter(fmt=log_format_stream)
 handler_stream = logging.StreamHandler()
 handler_stream.setFormatter(formatter_stream)
 logger.addHandler(handler_stream)
 
-formatter_file = logging.Formatter(fmt=LOG_FORMAT)
+log_format_file = '%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message)s'
+formatter_file = logging.Formatter(fmt=log_format_file)
 handler_file = RotatingFileHandler(
     LOG_FILE_PATH, maxBytes=LOG_MAX_SIZE, backupCount=10, delay=True)
 handler_file.setFormatter(formatter_file)
 logger.addHandler(handler_file)
 
 
 # Set log level to DEBUG if ENV is dev
```

### Comparing `battetl-1.0.1/battetl/transform/Transformer.py` & `battetl-1.0.2/battetl/transform/Transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -190,14 +190,19 @@
         """
         df = Utils.rename_df_columns(
             df, Constants.COLUMNS_MAPPING_MACCOR_TEST_DATA)
         df = Utils.convert_to_milli(df)
         df = self.__convert_datetime_unixtime(df)
         df = self.__convert_data_type(df)
 
+        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
+            df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
+        if 'step_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['step_time_s'][0]):
+            df = Utils.convert_timedelta_to_seconds(df, 'step_time_s')
+
         df = Utils.sort_dataframe(df, ['unixtime_s', 'step'])
 
         return df
 
     def __transform_maccor_cycle_stats(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transforms Maccor cycle to conform to BattETL naming and data conventions
@@ -218,27 +223,27 @@
             The transformed output DataFrame
         """
         df = Utils.rename_df_columns(
             df, Constants.COLUMNS_MAPPING_MACCOR_CYCLE_STATS)
         df = Utils.convert_to_milli(df)
         df = self.__convert_data_type(df)
 
-        def timedelta_validation_check(input_string):
-            # Check if it is like the format "1d 15:07:52.77"
-            regex = re.compile('\d+d \d+:\d+:\d+.\d+\Z', re.I)
-            match = regex.match(str(input_string))
-            return bool(match)
-
-        if 'test_time_s' in df.columns and len(df) > 0 and timedelta_validation_check(df['test_time_s'][0]):
+        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
             df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
 
         df = Utils.sort_dataframe(df, ['cycle'])
 
         return df
 
+    def __timedelta_validation_check(self, input_string):
+        # Check if it is like the format "1d 15:07:52.77" or "1d 15:07:52"
+        regex = re.compile(r'\d+d \d+:\d+:\d+(\.\d+)?\Z', re.I)
+        match = regex.match(str(input_string))
+        return bool(match)
+
     def __convert_datetime_unixtime(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Convert datetime to UTC format and add unixtime_s column
 
         Parameters
         ----------
         df : pandas.DataFrame
@@ -362,15 +367,15 @@
             return {}
 
         self.test_data = self.__harmonize_capacity(self.test_data, steps)
 
         # DataFrame where we will hold calculated cycle statistics for all cycles
         df_calced_stats = pd.DataFrame(columns=['cycle'])
 
-        for cycle in range(self.test_data.cycle.head(1).item(), self.test_data.cycle.tail(1).item()):
+        for cycle in range(self.test_data.cycle.head(1).item(), self.test_data.cycle.tail(1).item()+1):
 
             cycle_data = self.test_data[self.test_data.cycle == cycle]
             if cycle_data.empty:
                 logger.info("No cycle data for cycle " + str(cycle))
                 continue
 
             # Calculate various charge and discharge cycle statistics.
@@ -382,16 +387,16 @@
 
             discharge_metrics = self.__calc_discharge_stats(
                 cycle_data, steps['dsg'])
             stats.update(discharge_metrics)
 
             # Calculate coulombic efficiency from the charge and discharge stats.
             if (('calculated_charge_capacity_mah' not in stats) or
-                    ('calculated_discharge_capacity_mah' not in stats) or 
-                        (stats['calculated_charge_capacity_mah']==0)):
+                    ('calculated_discharge_capacity_mah' not in stats) or
+                    (stats['calculated_charge_capacity_mah'] == 0)):
                 ce = float("nan")
                 logger.info(
                     "Unable to calculate coulombic efficiency for cycle " + str(cycle))
             else:
                 ce = (discharge_metrics['calculated_discharge_capacity_mah']
                       / charge_metrics['calculated_charge_capacity_mah'])
             stats.update({'coulombic_efficiency': ce})
@@ -433,53 +438,40 @@
         # Define charge data to be where the step is a charge step.
         chg_data = cycle_data[cycle_data.step.isin(charge_steps)]
         if len(chg_data) < 2:
             logger.info("No charge data for cycle " +
                         str(cycle_data.cycle.iloc[0]))
             return stats
 
-        cumulative_tuple = self.__calc_cumulative_capacity(
-            chg_data, charge_steps, 'charge')
-        stats['calculated_charge_capacity_mah'] = cumulative_tuple[0]
-        stats['calculated_charge_energy_mwh'] = cumulative_tuple[1]
-        stats['calculated_charge_time_s'] = (chg_data.test_time_s.iloc[-1] -
-                                             chg_data.test_time_s.iloc[0])
-
-        # Calculate cc/cv time & capacity.
-        chg_data_cv = chg_data[chg_data.voltage_mv > cv_voltage_thresh_mv]
-        if chg_data_cv.empty:
-            logger.info("No CV data for cycle " +
-                        str(cycle_data.cycle.iloc[0]))
-            stats['calculated_cc_charge_time_s'] = stats['calculated_charge_time_s']
-            stats['calculated_cv_charge_time_s'] = float("nan")
-            stats['calculated_cc_capacity_mah'] = stats['calculated_charge_capacity_mah']
-            stats['calculated_cv_capacity_mah'] = float("nan")
-        else:
-            stats['calculated_cc_charge_time_s'] = (chg_data_cv.iloc[0].test_time_s
-                                                    - chg_data.iloc[0].test_time_s)
-            stats['calculated_cv_charge_time_s'] = (chg_data_cv.test_time_s.iloc[-1]
-                                                    - chg_data_cv.test_time_s.iloc[0])
-            stats['calculated_cc_capacity_mah'] = chg_data_cv.iloc[0].charge_capacity_mah
-            stats['calculated_cv_capacity_mah'] = (chg_data_cv.charge_capacity_mah.iloc[-1]
-                                                   - chg_data_cv.charge_capacity_mah.iloc[0])
+        ez_df = self.__ez_calc_df(
+            chg_data, charge_steps, 'charge', cv_voltage_thresh_mv)
+
+        stats['calculated_charge_capacity_mah'] = ez_df['charge_capacity_mah'].iloc[-1]
+        stats['calculated_charge_energy_mwh'] = ez_df['charge_energy_mwh'].iloc[-1]
+        stats['calculated_charge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
+
+        stats['calculated_cc_charge_time_s'] = ez_df.cc_time_s.sum()
+        stats['calculated_cv_charge_time_s'] = ez_df.cv_time_s.sum()
+        stats['calculated_cc_capacity_mah'] = ez_df.cc_capacity_mah.sum()
+        stats['calculated_cv_capacity_mah'] = ez_df.cv_capacity_mah.sum()
 
         # Calculate 50%/80% charge time & capacity.
         eighty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.8
         fifty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.5
         try:
-            eighty_percent_cap_time_s = (chg_data[chg_data.charge_capacity_mah > eighty_percent_cap_mah].test_time_s.iloc[0]
-                                        - chg_data.test_time_s.iloc[0])
-            half_percent_cap_time_s = (chg_data[chg_data.charge_capacity_mah > fifty_percent_cap_mah].test_time_s.iloc[0]
-                                    - chg_data.test_time_s.iloc[0])
+            eighty_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > eighty_percent_cap_mah].ellapsed_time_s.iloc[0]
+                                         - ez_df.ellapsed_time_s.iloc[0])
+            half_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > fifty_percent_cap_mah].ellapsed_time_s.iloc[0]
+                                       - ez_df.ellapsed_time_s.iloc[0])
         except:
             eighty_percent_cap_time_s = float('nan')
             half_percent_cap_time_s = float('nan')
             logger.warning(
                 f'Incomplete charge data for cycle {cycle_data.cycle.iloc[0]}')
-            
+
         stats['calculated_fifty_percent_charge_time_s'] = half_percent_cap_time_s
         stats['calculated_eighty_percent_charge_time_s'] = eighty_percent_cap_time_s
 
         return stats
 
     def __calc_discharge_stats(self, cycle_data: pd.DataFrame, discharge_steps: list) -> dict:
         """
@@ -503,73 +495,131 @@
         # Define discharge data to be where the step is a discharge step.
         dsg_data = cycle_data[cycle_data.step.isin(discharge_steps)]
         if len(dsg_data) < 2:
             logger.info("No discharge data for cycle " +
                         str(cycle_data.cycle.iloc[0]))
             return stats
 
-        cumulative_tuple = self.__calc_cumulative_capacity(
-            dsg_data, discharge_steps, 'discharge')
-        stats['calculated_discharge_capacity_mah'] = cumulative_tuple[0]
-        stats['calculated_discharge_energy_mwh'] = cumulative_tuple[1]
-        stats['calculated_discharge_time_s'] = dsg_data.test_time_s.iloc[-1] - \
-            dsg_data.test_time_s.iloc[0]
+        ez_df = self.__ez_calc_df(dsg_data, discharge_steps, 'discharge')
+
+        stats['calculated_discharge_capacity_mah'] = ez_df['discharge_capacity_mah'].iloc[-1]
+        stats['calculated_discharge_energy_mwh'] = ez_df['discharge_energy_mwh'].iloc[-1]
+        stats['calculated_discharge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
 
         return stats
 
-    def __calc_cumulative_capacity(self, df: pd.DataFrame, steps: list, step_type: str) -> tuple:
+    def __ez_calc_df(self, cycle_df: pd.DataFrame, steps: list, step_type: str, cv_voltage_thresh_mv=None) -> tuple:
         """
-        Calculates cumulative capacity from the dataframe from steps within 
-        the predefined list.
+        Creates a DataFrame we can easily use to calculate cycle statistics.
+
+        Modifies test_data to cummulative capacity in cases where capacity is reset at each step.
 
         Parameters
         ----------
         df : pd.DataFrame
-            A dataframe containing data to calculate capacity from. Will be modified
-            in place if capacity is reset after each step.
+            The DataFrame use to calculate cumulative capacity.
         steps : list
-            A list of the steps to calculate cumulative
+            A list of the steps to calculate cumulative capacity for. 
         step_type : str
-            The type of data we are calculating for. Can either be 'charge' or 'discharge'. If 
-            something else is passed an error is thrown.
+            Either 'charge' or 'discharge' depending on what type of steps we are calculating for.
+        cv_voltage_thresh_mv : float
+            The voltage threshold in mV above which charge is considered to be constant voltage.    
 
         Returns
         -------
-        (cumulative_capacity_mah, cumulative_energy_mwh): tuple
-            Tuple containing cumulative capacity and cumulative energy from the step data.
+        ez_df: pd.DataFrame
+            Dataframe containing values filtered to charge steps with cumulative capacity
+            and ellapsed time calculated.
         """
         logger.debug(f'Calculating cumulative {step_type} capacity')
 
+        time_col = 'ellapsed_time_s'
+        volt_col = 'voltage_mv'
+        cc_time = 'cc_time_s'
+        cv_time = 'cv_time_s'
+        cc_cap = 'cc_capacity_mah'
+        cv_cap = 'cv_capacity_mah'
         if step_type == 'charge':
-            capacity_column = 'charge_capacity_mah'
-            energy_column = 'charge_energy_mwh'
+            cap_col = 'charge_capacity_mah'
+            eng_col = 'charge_energy_mwh'
         elif step_type == 'discharge':
-            capacity_column = 'discharge_capacity_mah'
-            energy_column = 'discharge_energy_mwh'
+            cap_col = 'discharge_capacity_mah'
+            eng_col = 'discharge_energy_mwh'
+        else:
+            logger.error(f'Unknown step type {step_type}!')
+            return pd.DataFrame()
 
-        logger.debug(
-            f'Capacity column: {capacity_column}. Energy column: {energy_column}')
+        ez_df = pd.DataFrame(
+            columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
+
+        # Iterate through each charge step to calculate cumulative capacity
 
-        # Calculate cumulative capacity/energy from each of the steps.
-        cumulative_capacity_mah = 0
-        cumulative_energy_mwh = 0
         for i, step in enumerate(steps):
-            step_data = df[df.step == step]
-            if step_data.empty:
+
+            step_slice = cycle_df[cycle_df.step == step]
+            step_df = pd.DataFrame(
+                columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
+
+            if step_slice.empty:
                 continue
 
-            if i == 0:
-                cumulative_capacity_mah = step_data[capacity_column].iloc[-1] - \
-                    step_data[capacity_column].iloc[0]
-                cumulative_energy_mwh = step_data[energy_column].iloc[-1] - \
-                    step_data[energy_column].iloc[0]
+            if ez_df.empty:
+                ez_df[time_col] = step_slice['test_time_s'] - \
+                    step_slice['test_time_s'].iloc[0]
+                ez_df[volt_col] = step_slice['voltage_mv']
+                ez_df[eng_col] = step_slice[eng_col] - \
+                    step_slice[eng_col].iloc[0]
+                ez_df[cap_col] = step_slice[cap_col] - \
+                    step_slice[cap_col].iloc[0]
+                if step_type == 'charge':
+                    # if ez_df is empty, we're at beginning of a cycle and cap/step time should be reset to zero
+                    # TODO: add documentation for this
+                    delta_time = step_slice['step_time_s'] - \
+                        step_slice['step_time_s'].shift(1, fill_value=0)
+                    ez_df[cc_time] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
+                    ez_df[cv_time] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
+                    delta_cap = step_slice[cap_col] - \
+                        step_slice[cap_col].shift(1, fill_value=0)
+                    ez_df[cc_cap] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
+                    ez_df[cv_cap] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
+                # TODO: corner case of ICT will still need above logic for discharge
+                elif step_type == 'discharge':
+                    ez_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
             else:
-                # This check statement addresses instances where capacity was reset after each step.
-                if step_data[capacity_column].iloc[0] < cumulative_capacity_mah:
-                    step_data[capacity_column] += cumulative_capacity_mah
-                    step_data[energy_column] += cumulative_energy_mwh
-                cumulative_capacity_mah += step_data[capacity_column].iloc[-1] - \
-                    step_data[capacity_column].iloc[0]
-                cumulative_energy_mwh += step_data[energy_column].iloc[-1] - \
-                    step_data[energy_column].iloc[0]
-
-        return (cumulative_capacity_mah, cumulative_energy_mwh)
+                # This catches if capacity was reset after each step. Modifies test_data DF in place.
+                if step_slice[cap_col].iloc[0] < ez_df[cap_col].iloc[-1]:
+                    current_cycle = cycle_df.cycle.iloc[0]
+                    self.test_data.loc[self.test_data.cycle == current_cycle,
+                                       self.test_data.step == step, cap_col] += ez_df[cap_col]
+                    self.test_data.loc[self.test_data.cycle == current_cycle,
+                                       self.test_data.step == step, eng_col] += ez_df[eng_col]
+                if not ez_df.empty:
+                    # keeps running time across steps. ignoring time between steps
+                    step_df[time_col] = (
+                        step_slice['test_time_s'] - step_slice['test_time_s'].iloc[0]) + ez_df[time_col].iloc[-1]
+                # step_slice is updated with above updates to test_data because it's a slice, not copy, of test_data
+                step_df[volt_col] = step_slice[volt_col]
+                step_df[cap_col] = step_slice[cap_col]
+                step_df[eng_col] = step_slice[eng_col]
+                if step_type == 'charge':
+                    # calculate the delta time/cap for each step, sum the deltas in calc_stats() to get cycle time/cap
+                    delta_time = step_slice['step_time_s'] - \
+                        step_slice['step_time_s'].shift(1, fill_value=0)
+                    step_df[cc_time] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
+                    step_df[cv_time] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
+                    delta_cap = step_slice[cap_col] - step_slice[cap_col].shift(
+                        1, fill_value=ez_df[cap_col].iloc[-1])
+                    step_df[cc_cap] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
+                    step_df[cv_cap] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
+                elif step_type == 'discharge':
+                    step_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
+                ez_df = pd.concat([ez_df, step_df])
+        logger.debug(f'Finished calculating cumulative {step_type} capacity')
+        return ez_df
```

### Comparing `battetl-1.0.1/battetl/utils.py` & `battetl-1.0.2/battetl/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,26 +134,31 @@
         columnsSet = Utils.get_lower_strip_set(columns)
         arbinTestDataSet = Utils.get_lower_strip_set(
             Constants.COLUMNS_ARBIN_TEST_DATA_ONLY)
         arbinCycleStatsSet = Utils.get_lower_strip_set(
             Constants.COLUMNS_ARBIN_CYCLE_STATS_ONLY)
         maccorTestDataSet = Utils.get_lower_strip_set(
             Constants.COLUMNS_MACCOR_TEST_DATA_ONLY)
+        maccorTestDataSetType2 = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY)
         maccorCycleStatsSet = Utils.get_lower_strip_set(
             Constants.COLUMNS_MACCOR_CYCLE_STATS_ONLY)
 
         if len(columnsSet & arbinTestDataSet) >= (len(arbinTestDataSet) / 2):
             return Constants.MAKE_ARBIN, Constants.DATA_TYPE_TEST_DATA
 
         if len(columnsSet & arbinCycleStatsSet) >= (len(arbinCycleStatsSet) / 2):
             return Constants.MAKE_ARBIN, Constants.DATA_TYPE_CYCLE_STATS
 
         if len(columnsSet & maccorTestDataSet) >= (len(maccorTestDataSet) / 2):
             return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
 
+        if len(columnsSet & maccorTestDataSetType2) >= (len(maccorTestDataSetType2) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
+
         if len(columnsSet & maccorCycleStatsSet) >= (len(maccorCycleStatsSet) / 2):
             return Constants.MAKE_MACCOR, Constants.DATA_TYPE_CYCLE_STATS
 
         return None, None
 
     def get_lower_strip_set(data: list[str]) -> set:
         """
@@ -282,18 +287,15 @@
             Converted data
         """
         logger.info(f'Convert {column} to seconds')
 
         if column not in df.columns:
             raise NameError(f'Can not find {column}')
 
-        def conv(row):
-            return pd.Timedelta(row[column]).total_seconds()
-
-        df[column] = df.apply(conv, axis=1)
+        df[column] = round(pd.to_timedelta(df[column]).dt.total_seconds(), 3)
 
         return df
 
     def convert_datetime(df: pd.DataFrame, column: str, timezone: str) -> pd.DataFrame:
         """
         Convert datetime to UTC format with time zone
```

### Comparing `battetl-1.0.1/battetl.egg-info/PKG-INFO` & `battetl-1.0.2/battetl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
+
 # BattETL
 
 BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
 
 <img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
 
 ## Overview
@@ -70,34 +72,44 @@
 
 ## Installation
 
 A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
 
 ### Requirements
 
-BattETL requires Python 3.9 or 3.10. The specific package requirements are detailed in the `requirements.txt` file.
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
 
 ### Installation Instructions
 
-Install BattETL using pip:
+- Install BattETL using pip:
 
 ```sh
 pip install battetl
 ```
 
-Install BattETL from source code:
+- Install BattETL from source code:
 
 ```sh
 git clone https://github.com/BattGenie/battetl.git
 cd battetl
 pip install -r requirements.txt
 pip install .
 ```
 
-Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
 
 ## Usage
 
 A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
 
 Using BattETL as an all-in-one ETL function is as easy as:
```

### Comparing `battetl-1.0.1/setup.py` & `battetl-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import os
 import setuptools
-from pip._internal.req import parse_requirements
-from pip._internal.network.session import PipSession
 
-this_dir = os.path.dirname(os.path.abspath(__file__))
-pip_requirements = parse_requirements(
-    os.path.join(this_dir, "requirements.txt"), PipSession())
-reqs = [pii.requirement for pii in pip_requirements]
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="battetl",
-    version="1.0.1",
+    version="1.0.2",
     author="Zander Nevitt, Bing Syuan Wang and Chintan Pathak",
     author_email="info@battgenie.life",
     description="A Python module for extracting, transforming, and loading battery data to a database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BattGenie/battetl",
     packages=setuptools.find_packages(),
-    install_requires=reqs,
+    install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9, <3.11',
     license='MIT',
```

