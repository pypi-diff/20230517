# Comparing `tmp/btcs_crypto_systems-0.0.4.tar.gz` & `tmp/btcs_crypto_systems-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btcs_crypto_systems-0.0.4.tar", last modified: Fri Feb 17 09:10:48 2023, max compression
+gzip compressed data, was "btcs_crypto_systems-0.0.5.tar", last modified: Wed May 17 06:44:09 2023, max compression
```

## Comparing `btcs_crypto_systems-0.0.4.tar` & `btcs_crypto_systems-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 09:10:48.273747 btcs_crypto_systems-0.0.4/
--rw-rw-rw-   0        0        0      908 2023-02-17 09:10:48.269808 btcs_crypto_systems-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-02-17 09:02:19.000000 btcs_crypto_systems-0.0.4/README.md
--rw-rw-rw-   0        0        0      176 2023-02-17 09:09:07.000000 btcs_crypto_systems-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-17 09:10:48.274746 btcs_crypto_systems-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-17 09:10:48.222489 btcs_crypto_systems-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-02-17 09:10:48.244491 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/
--rw-rw-rw-   0        0        0        0 2023-02-17 07:54:17.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/__init__.py
--rw-rw-rw-   0        0        0     1267 2023-02-17 09:08:56.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/ams.py
--rw-rw-rw-   0        0        0    10991 2023-02-17 08:04:32.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/token_master.py
--rw-rw-rw-   0        0        0      348 2023-02-17 08:38:32.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-17 09:10:48.265797 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/
--rw-rw-rw-   0        0        0      908 2023-02-17 09:10:48.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-02-17 09:10:48.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 09:10:48.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-02-17 09:10:48.000000 btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.501103 btcs_crypto_systems-0.0.5/
+-rw-rw-rw-   0        0        0     1338 2023-05-17 06:44:09.499101 btcs_crypto_systems-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-02-17 09:17:57.000000 btcs_crypto_systems-0.0.5/README.md
+-rw-rw-rw-   0        0        0      176 2023-05-17 06:43:55.000000 btcs_crypto_systems-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:44:09.501103 btcs_crypto_systems-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.455122 btcs_crypto_systems-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.480104 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/
+-rw-rw-rw-   0        0        0        0 2023-05-17 06:42:37.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/__init__.py
+-rw-rw-rw-   0        0        0     1267 2023-02-17 09:08:56.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/address_manangement_service.py
+-rw-rw-rw-   0        0        0     9621 2023-05-17 06:43:30.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/token_master.py
+-rw-rw-rw-   0        0        0      348 2023-02-17 08:38:32.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:44:09.496104 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/
+-rw-rw-rw-   0        0        0     1338 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-17 06:44:09.000000 btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/top_level.txt
```

### Comparing `btcs_crypto_systems-0.0.4/PKG-INFO` & `btcs_crypto_systems-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-Metadata-Version: 2.1
-Name: btcs_crypto_systems
-Version: 0.0.4
-Summary: To interact with BTCS crypto systems.
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # crypto systems package for BTCS crypto business systems
 
 
 ### Install
-```shell
+```bash
 pip install btcs_crypto_systems
 ```
 
 ### Update
-```shell
+```bash
 pip install btcs_crypto_systems --upgrade
 ```
+## Usage
 
 ### TokenMaster
 ```python
 from btcs_crypto_systems import token_master
 
 tm = token_master.TokenMaster(env="test")
 print(tm.assets[7].symbol)
@@ -34,10 +28,25 @@
 csv_writer.writerow(["0x8c8d7c46219d9205f056f28fee5950ad564d7465","1.001"])
 
 #creates a file called 20230217_0853_example_output_file.csv
 ```
 
 ### AMS
 ```python
-from btcs_crypto_systems import ams
+from btcs_crypto_systems import address_manangement_service
+
+ams = address_manangement_service.AMS(env="test")
+addresses = ams.get_addresses(account="200065621002")
+print(addresses)
+```
 
+
+## Update the package
+Navigate to the folder where the pyproject.toml file is.
+```bash
+python3 -m build
+python3 -m twine upload --repository pypi dist/*
+```
+```
+username: __token__
+password: get an API key from here https://pypi.org/manage/account/token/ 
 ```
```

### Comparing `btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/ams.py` & `btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/address_manangement_service.py`

 * *Files identical despite different names*

### Comparing `btcs_crypto_systems-0.0.4/src/btcs_crypto_systems/token_master.py` & `btcs_crypto_systems-0.0.5/src/btcs_crypto_systems/token_master.py`

 * *Files 20% similar despite different names*

```diff
@@ -78,46 +78,30 @@
         return "('tokenId':{}, 'blockchainId':{}, 'assetId':{})".format(self.id, self.blockchain_id, self.asset_id)
 
 class Asset:
     id: int
     name: str
     amount_precision: int
     asset_type: str
-    can_be_traded_online: bool
-    can_be_traded_internal: bool
     bancs_currency_id: str
-    can_be_deposited_from_online: bool
-    can_be_withdrawn_from_online: bool
     symbol: str
-    can_be_deposited: bool
-    can_be_withdrawn: bool
-    is_deposit_automated: bool
     automatic_withdrawal_limit: int
     automatic_withdrawal_limit_in_chf: int
-    can_create_account_in_online: bool
     is_active: bool
     token_ids: List[int]
 
-    def __init__(self, id: int, name: str, amount_precision: int, asset_type: str, can_be_traded_online: bool, can_be_traded_internal: bool, bancs_currency_id: str, can_be_deposited_from_online: bool, can_be_withdrawn_from_online: bool, symbol: str, can_be_deposited: bool, can_be_withdrawn: bool, is_deposit_automated: bool, automatic_withdrawal_limit: int, automatic_withdrawal_limit_in_chf: int, can_create_account_in_online: bool, is_active: bool, token_ids: List[int]) -> None:
+    def __init__(self, id: int, name: str, amount_precision: int, asset_type: str, bancs_currency_id: str, symbol: str, automatic_withdrawal_limit: int, automatic_withdrawal_limit_in_chf: int, is_active: bool, token_ids: List[int]) -> None:
         self.id = id
         self.name = name
         self.amount_precision = amount_precision
         self.asset_type = asset_type
-        self.can_be_traded_online = can_be_traded_online
-        self.can_be_traded_internal = can_be_traded_internal
         self.bancs_currency_id = bancs_currency_id
-        self.can_be_deposited_from_online = can_be_deposited_from_online
-        self.can_be_withdrawn_from_online = can_be_withdrawn_from_online
         self.symbol = symbol
-        self.can_be_deposited = can_be_deposited
-        self.can_be_withdrawn = can_be_withdrawn
-        self.is_deposit_automated = is_deposit_automated
         self.automatic_withdrawal_limit = automatic_withdrawal_limit
         self.automatic_withdrawal_limit_in_chf = automatic_withdrawal_limit_in_chf
-        self.can_create_account_in_online = can_create_account_in_online
         self.is_active = is_active
         self.token_ids = token_ids
 
     def __str__(self):
         return "({}, {}, {})".format(self.id, self.symbol, self.token_ids)
 
     def __repr__(self):
@@ -154,26 +138,18 @@
                     trs.append(tr["id"])
 
             self.assets[a["id"]] = Asset( 
                 a["id"], 
                 a["name"], 
                 a["amountPrecision"], 
                 a["assetType"], 
-                a["canBeTradedOnline"], 
-                a["canBeTradedInternal"], 
                 a["bancsCurrencyId"], 
-                a["canBeDepositedFromOnline"], 
-                a["canBeWithdrawnFromOnline"], 
                 a["symbol"], 
-                a["canBeDeposited"], 
-                a["canBeWithdrawn"], 
-                a["isDepositAutomated"], 
                 a["automaticWithdrawalLimit"], 
                 a["automaticWithdrawalLimitInChf"], 
-                a["canCreateAccountInOnline"], 
                 a["isActive"], 
                 trs
             )
     
         # ----------------------- load blockchains -----------------------
         loaded_blockchains = TokenMaster.get_all("{}/blockchains".format(self.base_url))
         for b in loaded_blockchains:
```

### Comparing `btcs_crypto_systems-0.0.4/src/btcs_crypto_systems.egg-info/PKG-INFO` & `btcs_crypto_systems-0.0.5/src/btcs_crypto_systems.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: btcs-crypto-systems
-Version: 0.0.4
+Version: 0.0.5
 Summary: To interact with BTCS crypto systems.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # crypto systems package for BTCS crypto business systems
 
 
 ### Install
-```shell
+```bash
 pip install btcs_crypto_systems
 ```
 
 ### Update
-```shell
+```bash
 pip install btcs_crypto_systems --upgrade
 ```
+## Usage
 
 ### TokenMaster
 ```python
 from btcs_crypto_systems import token_master
 
 tm = token_master.TokenMaster(env="test")
 print(tm.assets[7].symbol)
@@ -34,10 +35,25 @@
 csv_writer.writerow(["0x8c8d7c46219d9205f056f28fee5950ad564d7465","1.001"])
 
 #creates a file called 20230217_0853_example_output_file.csv
 ```
 
 ### AMS
 ```python
-from btcs_crypto_systems import ams
+from btcs_crypto_systems import address_manangement_service
 
+ams = address_manangement_service.AMS(env="test")
+addresses = ams.get_addresses(account="200065621002")
+print(addresses)
+```
+
+
+## Update the package
+Navigate to the folder where the pyproject.toml file is.
+```bash
+python3 -m build
+python3 -m twine upload --repository pypi dist/*
+```
+```
+username: __token__
+password: get an API key from here https://pypi.org/manage/account/token/ 
 ```
```

