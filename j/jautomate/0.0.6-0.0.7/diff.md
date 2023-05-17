# Comparing `tmp/jautomate-0.0.6.tar.gz` & `tmp/jautomate-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jautomate-0.0.6.tar", last modified: Wed Mar 22 15:48:01 2023, max compression
+gzip compressed data, was "jautomate-0.0.7.tar", last modified: Wed May 17 18:42:58 2023, max compression
```

## Comparing `jautomate-0.0.6.tar` & `jautomate-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 15:48:01.466311 jautomate-0.0.6/
--rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-22 15:48:01.466396 jautomate-0.0.6/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)     2116 2023-03-17 14:27:58.000000 jautomate-0.0.6/README.md
--rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-03-16 19:32:05.000000 jautomate-0.0.6/pyproject.toml
--rw-r--r--   0 yoxall     (503) staff       (20)      804 2023-03-22 15:48:01.466793 jautomate-0.0.6/setup.cfg
--rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-03-15 18:48:35.000000 jautomate-0.0.6/setup.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 15:48:01.460336 jautomate-0.0.6/src/
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 15:48:01.463675 jautomate-0.0.6/src/jautomate/
--rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-03-22 15:47:55.000000 jautomate-0.0.6/src/jautomate/__init__.py
--rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-03-20 14:47:59.000000 jautomate-0.0.6/src/jautomate/__main__.py
--rw-r--r--   0 yoxall     (503) staff       (20)     7148 2023-03-13 15:40:58.000000 jautomate-0.0.6/src/jautomate/actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-03-13 19:41:21.000000 jautomate-0.0.6/src/jautomate/api.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1588 2023-03-15 18:11:11.000000 jautomate-0.0.6/src/jautomate/assets.py
--rw-r--r--   0 yoxall     (503) staff       (20)     4805 2023-03-16 19:29:53.000000 jautomate-0.0.6/src/jautomate/cli.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-03-22 15:47:15.000000 jautomate-0.0.6/src/jautomate/logger.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-03-16 18:53:21.000000 jautomate-0.0.6/src/jautomate/utils.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 15:48:01.465109 jautomate-0.0.6/src/jautomate.egg-info/
--rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/SOURCES.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/dependency_links.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/entry_points.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.6/src/jautomate.egg-info/not-zip-safe
--rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/requires.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-03-22 15:48:01.000000 jautomate-0.0.6/src/jautomate.egg-info/top_level.txt
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 15:48:01.465916 jautomate-0.0.6/tests/
--rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-03-16 19:08:13.000000 jautomate-0.0.6/tests/test_actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-03-16 15:17:54.000000 jautomate-0.0.6/tests/test_jautomate.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-03-16 19:12:12.000000 jautomate-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.147237 jautomate-0.0.7/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 18:42:58.147337 jautomate-0.0.7/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)     2372 2023-05-16 18:24:54.000000 jautomate-0.0.7/README.md
+-rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-05-05 12:20:37.000000 jautomate-0.0.7/pyproject.toml
+-rw-r--r--   0 yoxall     (503) staff       (20)      805 2023-05-17 18:42:58.147684 jautomate-0.0.7/setup.cfg
+-rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-05-05 12:20:37.000000 jautomate-0.0.7/setup.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.142417 jautomate-0.0.7/src/
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.145307 jautomate-0.0.7/src/jautomate/
+-rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-05-16 15:22:01.000000 jautomate-0.0.7/src/jautomate/__init__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/__main__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     8320 2023-05-17 15:53:41.000000 jautomate-0.0.7/src/jautomate/actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/api.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1768 2023-05-16 12:57:26.000000 jautomate-0.0.7/src/jautomate/assets.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     6023 2023-05-17 15:49:16.000000 jautomate-0.0.7/src/jautomate/cli.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/logger.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.146519 jautomate-0.0.7/src/jautomate.egg-info/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/SOURCES.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/dependency_links.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/entry_points.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.7/src/jautomate.egg-info/not-zip-safe
+-rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/requires.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/top_level.txt
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.147053 jautomate-0.0.7/tests/
+-rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_jautomate.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_utils.py
```

### Comparing `jautomate-0.0.6/PKG-INFO` & `jautomate-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: jautomate
-Version: 0.0.6
-Summary: Automates MDM tasks using the Jamf APIs
-Author: Dustin Yoxall
-Author-email: yoxall.dustin@ccpsstaff.org
-License: MIT
-Keywords: python,jamf
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Jautomate
 This tool automates MDM tasks on Jamf using the Jamf Pro and Jamf Classic API. For now there are only tasks focused on mobile devices. Computer versions of those tasks are in the works.
 
 ## Installation
 ---
 A pip installation will be set up once the build has been tested. For now you can install it from the testing PyPi server with this command:
 
@@ -86,7 +73,17 @@
 
 **Required arguments**
 
 | | |
 | --- | --- |
 DEVICE_TYPE | Type of devices being updated. {mobile / computer}
 FILE_PATH | The path to the csv file to be imported
+
+
+# Development
+References for dev/testing
+```bash
+# Run this line from the same directory as setup.py
+python -m build 
+# To test the build you can install/re-install with this line.
+pip install dist/jautomate-0.0.7-py3-none-any.whl --force-reinstall 
+```
```

### Comparing `jautomate-0.0.6/README.md` & `jautomate-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: jautomate
+Version: 0.0.7
+Summary: Automates MDM tasks using the Jamf APIs
+Author: Dustin Yoxall
+Author-email: yoxall.dustin@ccpsstaff.org
+License: MIT
+Keywords: python,jamf
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
 # Jautomate
 This tool automates MDM tasks on Jamf using the Jamf Pro and Jamf Classic API. For now there are only tasks focused on mobile devices. Computer versions of those tasks are in the works.
 
 ## Installation
 ---
 A pip installation will be set up once the build has been tested. For now you can install it from the testing PyPi server with this command:
 
@@ -72,8 +85,18 @@
 ```
 
 **Required arguments**
 
 | | |
 | --- | --- |
 DEVICE_TYPE | Type of devices being updated. {mobile / computer}
-FILE_PATH | The path to the csv file to be imported
+FILE_PATH | The path to the csv file to be imported
+
+
+# Development
+References for dev/testing
+```bash
+# Run this line from the same directory as setup.py
+python -m build 
+# To test the build you can install/re-install with this line.
+pip install dist/jautomate-0.0.7-py3-none-any.whl --force-reinstall 
+```
```

### Comparing `jautomate-0.0.6/setup.cfg` & `jautomate-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.11
 install_requires = 
 	jps_api_wrapper
 	typer
 	python-dotenv
 
 [options.packages.find]
 where = src
```

### Comparing `jautomate-0.0.6/src/jautomate/actions.py` & `jautomate-0.0.7/src/jautomate/actions.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 from typing import Dict, List
 from jautomate.api import jamf_p, jamf_c
 from jautomate.assets import Asset, Assets
 from jautomate.logger import j_logger
 from jautomate import utils
 
 
-def get_all_mobile_devices_modified() -> List[Dict]:
+class JautomateException(Exception):
+    """
+    Base Exception for Jautomate
+    """
+    pass
+
+
+def get_all_mobile_devices_pro() -> List[Dict]:
     """
     Returns dict of all mobile devices from Jamf using Pro API
 
     Returns:
         List[Dict]: List of all mobile devices from Jamf Pro API
     """
     # Pro API max page size is 2000
     page_size = 2000
     page = 0
+    # remaining_results needs to be higher than the total amount of devices
     remaining_results = 10000
     device_list = []
     while remaining_results > 0:
         response = jamf_p.get_mobile_devices(
             page=page, page_size=page_size)
 
         if remaining_results == 10000:
@@ -121,14 +129,18 @@
 
     Args:
         building_name (str): String abbreviation of building
 
     Returns:
         String: String representation of building ID number
     """
+    # We return 0 as an int to unset the building during unassign
+    if building_name == '0':
+        return None
+
     response = jamf_p.get_buildings()
     jamf_buildings = []
     jamf_buildings.extend(response['results'])
     return [building['id'] for building in jamf_buildings
             if building['name'] == building_name][0]
 
 
@@ -139,68 +151,86 @@
     Structure of payload can be found on Jamf's API doc:
     https://developer.jamf.com/jamf-pro/reference/patch_v2-mobile-devices-id
 
     Args:
         asset_list (Assets): Obj of assets being worked with. See Assets class for structure.
     """
     j_logger.debug('Syncing assets to Jamf')
+
     for asset in asset_list:
-        payload = {
-            "location": {
-                "realName": asset.student_name,
-                "room": asset.homeroom,
-                "buildingId": get_building_id(asset.building)
-            },
-            "updatedExtensionAttributes": [
-                {
-                    "value": [asset.student_grade],
-                    "name": "Grade"
+        # Process for mobile devices
+        if asset.device_type == 'mobile':
+            payload = {
+                "location": {
+                    "realName": asset.student_name,
+                    "room": asset.homeroom,
+                    "buildingId": get_building_id(asset.building)
                 },
-                {
-                    "value": ["prek-2"],
-                    "name": "Owner"
+                "updatedExtensionAttributes": [
+                    {
+                        "value": [asset.student_grade],
+                        "name": "Grade"
+                    },
+                    {
+                        "value": [asset.owner],
+                        "name": "Owner"
+                    }
+                ],
+                # This is set because it allows techs to see asset tag from settings on device
+                "name": asset.asset_tag,
+                "enforceName": True
+            }
+            jamf_p.update_mobile_device(payload, asset.jamf_id)
+            j_logger.debug("Asset: %s Ok", asset.asset_tag)
+
+        # Process for computers
+        if asset.device_type == 'computer':
+            payload = {
+                "general": {
+                    "extensionAttributes": [
+                        {
+                            "definitionId": "4",
+                            "name": "Grade",
+                            "values": [
+                                f"{asset.student_grade:02}"
+                            ]
+                        },
+                        {
+                            "definitionId": "3",
+                            "name": "GradYear",
+                            "values": [
+                                asset.grad_year
+                            ]
+                        }
+                    ]
+                },
+                "userAndLocation": {
+                    "realname": asset.student_name,
+                    "email": asset.email_address,
+                    "position": asset.position,
+                    "buildingId": get_building_id(asset.building),
+                    "room": asset.homeroom,
                 }
-            ],
-            # This is set because it allows techs to see asset tag from settings on device
-            "name": asset.asset_tag,
-            "enforceName": True
-        }
-        jamf_p.update_mobile_device(payload, asset.jamf_id)
-        j_logger.debug("Asset: %s Ok", asset.asset_tag)
-
-
-def unassign_devices_in_jamf(asset_list: List[Asset]) -> None:
-    """
-    Removes user and location info from asset in Jamf Pro
+            }
+            jamf_p.update_computer_inventory(payload, asset.jamf_id)
+            j_logger.debug("Asset: %s Ok", asset.asset_tag)
+
+
+def get_single_computer_record_by_asset_tag(asset_tag: str):
+    # This endpoint allows us to filter by asset tag so we only need to get the device we need
+    endpoint_filter = f'general.assetTag==\"{asset_tag}\"'
+    response = jamf_p.get_computer_inventories(
+        section=["GENERAL"], filter=endpoint_filter)
+    if response["totalCount"] >= 1:
+        return response["results"]
+    else:
+        raise JautomateException("Computer record could not be found.")
 
-    Most values passed as empty strings to clear them in Jamf Pro.
-    Structure of payload can be found on Jamf's API doc:
-    https://developer.jamf.com/jamf-pro/reference/patch_v2-mobile-devices-id
 
-    Args:
-        asset_list (Assets): Obj of assets being worked with. See Assets class for structure.
-    """
-    j_logger.debug('Unassigning assets in Jamf')
-    for asset in asset_list:
-        payload = {
-            "location": {
-                "realName": asset.student_name,
-                "room": asset.homeroom,
-                "buildingId": 0
-            },
-            "updatedExtensionAttributes": [
-                {
-                    "value": [asset.student_grade],
-                    "name": "Grade"
-                },
-                {
-                    "value": [""],
-                    "name": "Owner"
-                }
-            ],
-            # This is set because it allows techs to see asset tag from settings on device
-            "name": asset.asset_tag,
-            "enforceName": True
-        }
-        j_logger.debug(asset)
-        jamf_p.update_mobile_device(payload, asset.jamf_id)
-        j_logger.debug("Asset: %s Unassigned", asset.asset_tag)
+def update_computer_jamf_ids(asset_list: Assets):
+    for asset in asset_list.local:
+        matching_device = next(
+            (device for device in asset_list.remote
+                if device['general']['assetTag'] == asset.asset_tag), None)
+        if matching_device:
+            asset.jamf_id = matching_device['id']
+    return asset_list
```

### Comparing `jautomate-0.0.6/src/jautomate/assets.py` & `jautomate-0.0.7/src/jautomate/assets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module to handle asset structure and storage"""
 
 from abc import ABC
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 
 class AssetType(str, Enum):
     """
     Enum to assign asset type in standardized way.
 
     Used to define cli arguments for various commands and set as part of
@@ -35,17 +35,21 @@
     """
 
     asset_tag: str
     building: str
     homeroom: str
     student_grade: str
     student_name: str
-    owner: str = ''
-    serial_number: str = None
-    jamf_id: str = None
+    device_type: AssetType
+    email_address: Optional[str] = None
+    grad_year: Optional[str] = None
+    jamf_id: Optional[str] = None
+    owner: Optional[str] = None
+    position: Optional[str] = None
+    serial_number: Optional[str] = None
 
 
 @dataclass
 class MobileAsset(Asset):
     """Mobile Asset"""
```

### Comparing `jautomate-0.0.6/src/jautomate/cli.py` & `jautomate-0.0.7/src/jautomate/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,50 +74,63 @@
         ..., help='Asset tag should be a 6 digit number'),
     serial_number: str = typer.Argument(..., help='Serial Number of device'),
     student_name: str = typer.Argument(..., help=' Student full name'),
     homeroom: str = typer.Argument(..., help='Homeroom teachers last name'),
     student_grade: int = typer.Argument(..., help='Student grade as a number'),
     building: str = typer.Argument(
         ...,
-        help='Three letter building abbreviation. ex: COA')
-
-
-
-
+        help='Three letter building abbreviation. ex: COA'),
+    email_address: Optional[str] = typer.Argument(
+        default=None, help='Student email address'),
+    grad_year: Optional[str] = typer.Argument(
+        default=None, help='Year student graduates'),
+    owner: Optional[str] = typer.Argument(
+        default='', help='Owner of device, this was used in the past as a way to target devices but should be deprecated'),
+    position: Optional[str] = typer.Argument(
+        default=None, help='For now, this will also be the Graduation year, will be transitioned to Student or Staff'),
 ) -> None:
     """
     Assigns data to a single asset record in Jamf Pro.
 
     Args:
         device_type (str, required): Type of device being updated. mobile or computer
         asset_tag (str, required): Asset tag should be a 6 digit number
         serial_number (str, required): Serial Number of device
         student_name (str, required):  Student full name
         homeroom (str, required): Homeroom teachers last name
         student_grade (int, required): Student grade as a number
         building (_type_, required): Three letter building abbreviation. ex: COA
     """
-    if device_type.value == 'computer':
-        print('Computer functionality coming soon...')
-        return
+    j_logger.debug('%s asset assign is running...', device_type.value)
 
-    j_logger.debug('%s asset assign is running...', device_type)
+    # Create asset with all passed data
     asset = Asset(
         asset_tag=asset_tag,
         building=building,
+        device_type=device_type.value,
+        email_address=email_address,
+        grad_year=grad_year,
         homeroom=homeroom,
+        owner=owner,
+        position=position,
         serial_number=serial_number,
         student_grade=student_grade,
-        student_name=student_name
+        student_name=student_name,
     )
-    asset_list = Assets([asset], actions.get_all_mobile_devices())
-    asset_list = actions.get_mobile_device_jamf_ids_by_serial_number(
-        asset_list)
 
-    j_logger.debug(asset_list.local)
+    if asset.device_type == 'computer':
+        asset_list = Assets(
+            [asset],
+            actions.get_single_computer_record_by_asset_tag(asset.asset_tag))
+        asset_list = actions.update_computer_jamf_ids(asset_list)
+
+    if asset.device_type == 'mobile':
+        asset_list = Assets([asset], actions.get_all_mobile_devices())
+        asset_list = actions.get_mobile_device_jamf_ids_by_serial_number(
+            asset_list)
 
     actions.sync_assets_to_jamf(asset_list.local)
 
 
 @app.command()
 def unassign(
     device_type: AssetType = typer.Argument(
@@ -130,26 +143,35 @@
     """
     Unassigns data from a single asset record in Jamf Pro
 
     Args:
         device_type (str, required): Type of device being updated. mobile or computer
         asset_tag (str, required): Asset tag, should be a 6 digit number
     """
-    if device_type.value == 'computer':
-        print('Computer functionality coming soon...')
-        return
+    j_logger.debug('%s device unassign is running...', device_type.value)
 
-    j_logger.debug('%s device unassign is running...', device_type)
+    # Set all properties to empty str except asset_tag, building, device_type
     asset = Asset(
         asset_tag=asset_tag,
-        building='',
+        building='0',
+        device_type=device_type.value,
+        email_address='',
+        grad_year='',
         homeroom='',
+        owner='',
+        position='',
         student_grade='',
-        student_name=''
+        student_name='',
     )
-    asset_list = Assets([asset], actions.get_all_mobile_devices())
-    asset_list = actions.get_mobile_device_jamf_ids_by_asset_tag(
-        asset_list)
 
-    j_logger.debug(asset_list.local)
+    if device_type.value == 'computer':
+        asset_list = Assets(
+            [asset],
+            actions.get_single_computer_record_by_asset_tag(asset.asset_tag))
+        asset_list = actions.update_computer_jamf_ids(asset_list)
+
+    if asset.device_type == 'mobile':
+        asset_list = Assets([asset], actions.get_all_mobile_devices())
+        asset_list = actions.get_mobile_device_jamf_ids_by_asset_tag(
+            asset_list)
 
-    actions.unassign_devices_in_jamf(asset_list.local)
+    actions.sync_assets_to_jamf(asset_list.local)
```

### Comparing `jautomate-0.0.6/src/jautomate/logger.py` & `jautomate-0.0.7/src/jautomate/logger.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.6/src/jautomate/utils.py` & `jautomate-0.0.7/src/jautomate/utils.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.6/src/jautomate.egg-info/PKG-INFO` & `jautomate-0.0.7/src/jautomate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Jautomate
 This tool automates MDM tasks on Jamf using the Jamf Pro and Jamf Classic API. For now there are only tasks focused on mobile devices. Computer versions of those tasks are in the works.
 
 ## Installation
 ---
@@ -86,7 +86,17 @@
 
 **Required arguments**
 
 | | |
 | --- | --- |
 DEVICE_TYPE | Type of devices being updated. {mobile / computer}
 FILE_PATH | The path to the csv file to be imported
+
+
+# Development
+References for dev/testing
+```bash
+# Run this line from the same directory as setup.py
+python -m build 
+# To test the build you can install/re-install with this line.
+pip install dist/jautomate-0.0.7-py3-none-any.whl --force-reinstall 
+```
```

### Comparing `jautomate-0.0.6/src/jautomate.egg-info/SOURCES.txt` & `jautomate-0.0.7/src/jautomate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.6/tests/test_utils.py` & `jautomate-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

