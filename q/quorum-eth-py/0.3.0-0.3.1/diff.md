# Comparing `tmp/quorum_eth_py-0.3.0.tar.gz` & `tmp/quorum_eth_py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.3.0.tar", last modified: Wed May 17 04:47:48 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.3.1.tar", last modified: Wed May 17 05:09:41 2023, max compression
```

## Comparing `quorum_eth_py-0.3.0.tar` & `quorum_eth_py-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 04:47:48.784939 quorum_eth_py-0.3.0/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-17 04:47:48.783942 quorum_eth_py-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 04:47:48.723453 quorum_eth_py-0.3.0/quorum_eth_py/
--rw-rw-rw-   0        0        0      445 2023-05-17 04:45:58.000000 quorum_eth_py-0.3.0/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1746 2023-05-17 04:45:00.000000 quorum_eth_py-0.3.0/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0     7528 2023-05-17 04:42:24.000000 quorum_eth_py-0.3.0/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.3.0/quorum_eth_py/_gateway.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.3.0/quorum_eth_py/_http.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:47:48.780952 quorum_eth_py-0.3.0/quorum_eth_py/contract/
--rw-rw-rw-   0        0        0    23212 2023-05-14 05:42:29.000000 quorum_eth_py-0.3.0/quorum_eth_py/contract/RumERC20.py
--rw-rw-rw-   0        0        0      138 2023-05-15 07:09:49.000000 quorum_eth_py-0.3.0/quorum_eth_py/contract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 04:47:48.737170 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-17 04:47:48.000000 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-17 04:47:48.000000 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 04:47:48.000000 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 04:47:48.000000 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-17 04:47:48.000000 quorum_eth_py-0.3.0/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 04:47:48.784939 quorum_eth_py-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-05-17 04:45:58.000000 quorum_eth_py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.871835 quorum_eth_py-0.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-17 05:09:41.869862 quorum_eth_py-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.809709 quorum_eth_py-0.3.1/quorum_eth_py/
+-rw-rw-rw-   0        0        0      445 2023-05-17 05:09:03.000000 quorum_eth_py-0.3.1/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-05-17 04:45:00.000000 quorum_eth_py-0.3.1/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0     7497 2023-05-17 05:08:52.000000 quorum_eth_py-0.3.1/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.3.1/quorum_eth_py/_gateway.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.3.1/quorum_eth_py/_http.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.867841 quorum_eth_py-0.3.1/quorum_eth_py/contract/
+-rw-rw-rw-   0        0        0    23212 2023-05-14 05:42:29.000000 quorum_eth_py-0.3.1/quorum_eth_py/contract/RumERC20.py
+-rw-rw-rw-   0        0        0      138 2023-05-15 07:09:49.000000 quorum_eth_py-0.3.1/quorum_eth_py/contract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.861251 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:09:41.871835 quorum_eth_py-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2023-05-17 05:09:03.000000 quorum_eth_py-0.3.1/setup.py
```

### Comparing `quorum_eth_py-0.3.0/LICENSE` & `quorum_eth_py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.0/PKG-INFO` & `quorum_eth_py-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_eth_py
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.3.0/quorum_eth_py/_browser.py` & `quorum_eth_py-0.3.1/quorum_eth_py/_browser.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.0/quorum_eth_py/_eth.py` & `quorum_eth_py-0.3.1/quorum_eth_py/_eth.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,44 +31,44 @@
         status = self.w3.is_connected()
         logger.info("connected to rum-eth-chain: %s", status)
         return status
 
     def get_balance(self, address: str = None):
         """get the balance of address, default is the account address"""
         address = address or self.account.address
-        address = self.w3.is_checksum_address(address)
+        address = self.w3.to_checksum_address(address)
         balance_wei = self.w3.eth.get_balance(address)
         balance = self.w3.from_wei(balance_wei, "ether")
         return balance
 
     def _transction(self, tx: dict):
         signed_tx = self.w3.eth.account.sign_transaction(
-            tx, private_key=self.account.privateKey
+            tx, private_key=self.account.key
         )
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         return tx_receipt
 
     def transfer(self, to_address: str, num):
         """transfer rum to address, the rum is origin token of poa chain, used as gas feed"""
         # check balance of account
         if num <= 0:
             raise Exception("transfer num must be positive")
-        to_address = self.w3.is_checksum_address(to_address)
+        to_address = self.w3.to_checksum_address(to_address)
         if self.get_balance() < num:
             raise Exception(f"balance not enough {self.get_balance()}")
         tx = {
             "nonce": self.w3.eth.get_transaction_count(self.account.address),
             "to": to_address,
             "value": self.w3.to_wei(num, "ether"),
             "gasPrice": self.w3.to_wei("10", "gwei"),
             "gas": 50000,
             "chainId": RUM_ETH_CHAINID,
         }
-        gas_limit = self.w3.eth.estimateGas(tx)
+        gas_limit = self.w3.eth.estimate_gas(tx)
         if gas_limit > tx["gas"]:
             tx["gas"] = gas_limit
         tx_receipt = self._transction(tx)
         tid = tx_receipt.transactionHash.hex()
         return tid
 
     def contract_instance(self, abi, contract_address):
@@ -79,35 +79,35 @@
         self, name, symbol, total_supply, minter_address=None, abi=None, bytecode=None
     ):
         """deploy new erc20 contract"""
         abi = abi or RumERC20_abi
         bytecode = bytecode or RumERC20_bytecode
         contract = self.w3.eth.contract(abi=abi, bytecode=bytecode)
         cap = self.w3.to_wei(total_supply, "ether")
-        minter = self.w3.is_checksum_address(minter_address or self.account.address)
+        minter = self.w3.to_checksum_address(minter_address or self.account.address)
 
         tx = {
             "from": self.account.address,
             "nonce": self.w3.eth.get_transaction_count(self.account.address),
             "gasPrice": self.w3.to_wei("10", "gwei"),
             "gas": 50000,
             "chainId": RUM_ETH_CHAINID,
         }
         gas_limit = contract.constructor(
             cap=cap, name_=name, symbol_=symbol, minter=minter
-        ).estimateGas()
+        ).estimate_gas()
         if gas_limit > tx["gas"]:
             tx["gas"] = gas_limit
 
         if self.get_balance() < self.w3.from_wei(tx["gas"], "ether"):
             raise Exception(f"not enough for gas fee {self.get_balance()}")
 
         build_tx = contract.constructor(
             cap=cap, name_=name, symbol_=symbol, minter=minter
-        ).buildTransaction(tx)
+        ).build_transaction(tx)
         tx_receipt = self._transction(build_tx)
         contract_address = tx_receipt.contractAddress
         logger.info("deploy new erc20 contract: %s", contract_address)
         return contract_address
 
     def get_trx(self, tx_id_hex: str):
         receipt = self.w3.eth.get_transaction_receipt(tx_id_hex)
@@ -162,41 +162,39 @@
 
     def total_supply(self):
         unit256 = self.funcs.totalSupply().call()
         return self.w3.from_wei(unit256, "ether")
 
     def get_balance(self, address=None):
         address = address or self.account.address
-        address = self.w3.is_checksum_address(address)
+        address = self.w3.to_checksum_address(address)
         unit256 = self.funcs.balanceOf(address).call()
         return self.w3.from_wei(unit256, "ether")
 
     def get_rum_balance(self, address=None):
         address = address or self.account.address
         return self.chain.get_balance(address)
 
     def transfer(self, to_address, num):
         """transfter num of token to address"""
-        to_address = self.w3.is_checksum_address(to_address)
+        to_address = self.w3.to_checksum_address(to_address)
         amount = self.w3.to_wei(num, "ether")
 
         options = {
             "gas": 53000,
             "gasPrice": self.w3.to_wei("1", "gwei"),
             "from": self.account.address,
             "nonce": self.w3.eth.get_transaction_count(self.account.address),
         }
-        gas_limit = self.w3.eth.estimateGas(options)
+        gas_limit = self.w3.eth.estimate_gas(options)
         if gas_limit > options["gas"]:
             options["gas"] = gas_limit
 
-        tx = self.funcs.transfer(to_address, amount).buildTransaction(options)
-        signed = self.w3.eth.account.sign_transaction(
-            tx, private_key=self.account.privateKey
-        )
+        tx = self.funcs.transfer(to_address, amount).build_transaction(options)
+        signed = self.w3.eth.account.sign_transaction(tx, private_key=self.account.key)
         tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         tid = tx_receipt.transactionHash.hex()
         logger.info("transfer to %s is done by trx: %s", to_address, tid)
         return tid
 
     def get_trx(self, tx_id_hex: str):
```

### Comparing `quorum_eth_py-0.3.0/quorum_eth_py/_http.py` & `quorum_eth_py-0.3.1/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.0/quorum_eth_py/contract/RumERC20.py` & `quorum_eth_py-0.3.1/quorum_eth_py/contract/RumERC20.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.0/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.3.1/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-eth-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.3.0/setup.py` & `quorum_eth_py-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.3.0",
+    version="0.3.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

