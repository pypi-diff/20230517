# Comparing `tmp/dctrackclient-0.2.4.tar.gz` & `tmp/dctrackclient-0.3.0.tar.gz`

## Comparing `dctrackclient-0.2.4.tar` & `dctrackclient-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.github/workflows/doc.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/LICENSE
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/api.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/schema.json
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.github/workflows/gen.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dctrackclient-0.3.0/PKG-INFO
```

### Comparing `dctrackclient-0.2.4/.github/workflows/python-publish.yml` & `dctrackclient-0.3.0/.github/workflows/python-publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -26,16 +26,17 @@
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
-    - name: Write documentation
-      run: python .github/workflows/doc.py >> README.md
+        pip install jsonschema
+    - name: Generate code
+      run: python .github/workflows/gen.py
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dctrackclient-0.2.4/LICENSE` & `dctrackclient-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.4/pyproject.toml` & `dctrackclient-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.2.4"
+version = "0.3.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.2.4/PKG-INFO` & `dctrackclient-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dcTrackClient
-Version: 0.2.4
-Summary: Sunbird dcTrack API client in Python
-Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
-Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
-Author-email: Nicolas Ventura <ventura@lbl.gov>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/python-publish.yml?label=publish&logo=pypi) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API client in Python
 
 ## Initialize a connection to the dcTrack API
 
 Import the class:
@@ -78,165 +64,229 @@
 ```
 
 ## Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
 https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm
-## Module Documentation
-### class Client:
-```py
-def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = ''):
+
+## getItem(id)
+> Get item details using the item ID.
 ```
-> Provide either a username and password, or an API token to access the dcTrack database with Python.
-```py
-def createItem(self, data: dict, returnDetails: bool = True):
+GET api/v2/dcimoperations/items/{id}
 ```
-> Create a new item.
-```py
-def modifyItem(self, id: int, data: dict, returnDetails: bool = True):
+|Parameter|Type|
+|---|---|
+|id|number|
+
+## createItem(returnDetails, payload)
+> Create a new item. When returnDetails is set to true, the API call will return the full json payload. If set to false, the call returns only the "id" and "tiName".
 ```
-> Update an existing item.
-```py
-def deleteItem(self, id: int):
+POST api/v2/dcimoperations/items payload
+```
+|Parameter|Type|
+|---|---|
+|returnDetails|boolean|
+|payload|object|
+
+## updateItem(id, returnDetails, payload)
+> Update an existing item. When returnDetails is set to true, the API call will return the full json payload. If set to false, the call returns only the "id" and "tiName".
 ```
+PUT api/v2/dcimoperations/items/{id} payload
+```
+|Parameter|Type|
+|---|---|
+|id|number|
+|returnDetails|boolean|
+|payload|object|
+
+## deleteItem(id)
 > Delete an item using the item ID.
-```py
-def getItem(self, id: int):
 ```
-> Get item details using the item ID.
-```py
-def searchItems(self, data: dict, pageNumber: int, pageSize: int):
+DELETE api/v2/dcimoperations/items/{id}
 ```
-> Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination.
-```py
-def getCabinetItems(self, cabId: int):
+|Parameter|Type|
+|---|---|
+|id|number|
+
+## searchItems(pageNumber, pageSize, payload)
+> Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination. Returns a list of items with the specified information.
+```
+POST api/v2/quicksearch/items payload
 ```
+|Parameter|Type|
+|---|---|
+|pageNumber|number|
+|pageSize|number|
+|payload|object|
+
+## cabinetItems(CabinetId)
 > Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items.
-```py
-def manageItemsBulk(self, cabId: int):
 ```
-> Retrieve a list of Items contained in a Cabinet including Passive Items.
-```py
-def getAllMakes(self):
+GET api/v2/items/cabinetItems/{CabinetId}
 ```
-> Retrieve a list of all Makes.
-```py
-def addMake(self, data: dict):
+|Parameter|Type|
+|---|---|
+|CabinetId|number|
+
+## manageItemsBulk(payload)
+> Add/Update/Delete Items.
 ```
-> Add a new Make.
-```py
-def modifyMake(self, id: int, data: dict):
+POST api/v2/dcimoperations/items/bulk payload
 ```
-> Modify a Make.
-```py
-def deleteMake(self, id: int):
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## getMakes()
+> Returns a list of makes with basic information.
 ```
-> Delete a Make.
-```py
-def getMakesByName(self, name: str, usingSpecialChars: bool = False):
+GET api/v2/makes
 ```
-> Search for one or more makes using the make name. You also can search using special characters.
-```py
-def getModel(self, id: int, usedCounts: bool = False):
+*No parameters.*
+
+## createMake(payload)
+> Add a new Make. Returns JSON entity containing Make information that was passed in from the Request payload.
 ```
-> Get Model fields for the specified Model ID.
-```py
-def addModel(self, data: dict, returnDetails: bool = True, proceedOnWarning: bool = False):
+POST api/v2/makes payload
 ```
-> Add a new Model.
-```py
-def modifyModel(self, id: int, data: dict, returnDetails: bool = True, proceedOnWarning: bool = False):
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## updateMake(makeId, payload)
+> Modify a Make. Returns JSON entity containing Make information that was passed in from the Request payload.
 ```
-> Modify an existing Model.
-```py
-def deleteModel(self, id: int):
+PUT api/v2/makes/{makeId} payload
 ```
-> Delete a Model using the Model ID.
-```py
-def searchModels(self, data: dict, pageNumber: int, pageSize: int):
+|Parameter|Type|
+|---|---|
+|makeId|number|
+|payload|object|
+
+## deleteMake(makeId)
+> Delete a Make.
 ```
-> Search for models by user supplied search criteria.
-```py
-def getConnector(self, id: int, usedCount: bool = False):
+DELETE api/v2/makes/{makeId}
 ```
-> Get a Connector record by ID.
-```py
-def addConnector(self, data: dict):
+|Parameter|Type|
+|---|---|
+|makeId|number|
+
+## searchMakes(makeName)
+> Search for a make using the make name. Returns a list of makes with basic information.
 ```
-> Add a new Connector.
-```py
-def updateConnector(self, id: int, data: dict):
+GET api/v2/dcimoperations/search/makes/{makeName}
 ```
-> Update an existing Connector.
-```py
-def deleteConnector(self, ids: list[int]):
+|Parameter|Type|
+|---|---|
+|makeName|string|
+
+## getModel(modelId, usedCounts)
+> Get Model fields for the specified Model ID. usedCounts is an optional parameter that determines if the count of Items for the specified model is returned in the response. If set to "true" the counts will be included in the response, if omitted or set to "false" the item count will not be included in the response.
 ```
-> Delete one or more Connector records.
-```py
-def searchConnectors(self, data: dict, pageNumber: int, pageSize: int, usedCount: bool):
+GET api/v2/models/{modelId}
 ```
-> Retrieve a List of Connectors.
-```py
-def createDataPorts(self, itemId: int, data: dict):
+|Parameter|Type|
+|---|---|
+|modelId|number|
+|usedCounts|number|
+
+## createModel(returnDetails, proceedOnWarning, payload)
+> Add a new Model. Returns JSON entity containing Make information that was passed in from the Request payload. "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored. Fields that are not in the payload will remain unchanged.
 ```
-> Use the REST API to create data ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
-```py
-def updateDataPorts(self, itemId: int, portId: int, data: dict):
+POST api/v2/models payload
 ```
-> Update an item's data port details using the REST API. To do this, specify the item and data port ID, and provide the updated parameter value(s).
-```py
-def deleteDataPorts(self, itemId: int, portId: int):
+|Parameter|Type|
+|---|---|
+|returnDetails|boolean|
+|proceedOnWarning|boolean|
+|payload|object|
+
+## deleteModel(id)
+> Delete a Model using the Model ID.
 ```
-> Delete an item's data port using the REST API by specifying the item ID and data port ID.
-```py
-def getDataPorts(self, itemId: int):
+DELETE api/v2/models/{id}
 ```
-> Use the REST API to retrieve details from all data ports on an item.
-```py
-def getDataPort(self, itemId: int, portId: int):
+|Parameter|Type|
+|---|---|
+|id|number|
+
+## searchModels(pageNumber, pageSize, payload)
+> Search for models by user supplied search criteria. Returns a list of models with the "selectedColumns" returned in the payload. Search by Alias is not supported.
 ```
-> Use the REST API to read the details of an item's data port. To do this, specify the item and item data port ID.
-```py
-def getPowerPorts(self, itemId: int):
+POST api/v2/quicksearch/models payload
 ```
-> Use the REST API to retrieve details from all power ports on an item.
-```py
-def getPowerPort(self, itemId: int, portId: int):
+|Parameter|Type|
+|---|---|
+|pageNumber|number|
+|pageSize|number|
+|payload|object|
+
+## deleteModelImage(id, orientation)
+> Delete a Mode Image using the Model ID and the Image Orientation, where id is the Model Id and orientation is either front or back
 ```
-> Use the REST API to retrieve details from one power port on an item.
-```py
-def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
+DELETE api/v2/models/images/{id}/{orientation}
 ```
-> Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
-```py
-def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
+|Parameter|Type|
+|---|---|
+|id|number|
+|orientation|string|
+
+## getConnector(connectorId, usedCount)
+> Get a Connector record by ID. Returns a Connector with all information including Compatible Connectors. The usedCount parameter is optional. If usedCount is true, the response will include the number of times the connector is in use by Models and Items. If false, no counts are returned. If omitted the default is false.
 ```
-> Use the REST API to determine if a Connector is compatible with a specific Power Port.
-```py
-def getLocations(self):
+GET api/v2/settings/connectors/{connectorId}
 ```
-> Returns a list or all Locations.
-```py
-def getLocation(self, id: int):
+|Parameter|Type|
+|---|---|
+|connectorId|number|
+|usedCount|boolean|
+
+## createConnector(payload)
+> Add a new Connector. Returns JSON entity containing Connector information that was passed in from the Request payload.
 ```
-> Get a single Location.
-```py
-def addLocation(self, data: dict, proceedOnWarning: bool = False):
+POST api/v2/settings/connectors payload
 ```
-> Add a Location.
-```py
-def modifyLocation(self, id: int, data: dict, proceedOnWarning: bool = False):
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## updateConnector(connectorId, payload)
+> Update an existing Connector. Returns JSON entity containing Connector information that was passed in from the Request payload.
 ```
-> Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify.
-```py
-def deleteLocation(self, id: int):
+PUT api/v2/settings/connectors/{connectorId} payload
 ```
-> Delete a Location.
-```py
-def searchLocations(self, data: dict, pageNumber: int, pageSize: int):
+|Parameter|Type|
+|---|---|
+|connectorId|number|
+|payload|object|
+
+## deleteConnector(payload)
+> Delete one or more Connector records.
 ```
-> Search for one or more Locations by user supplied search criteria.
-```py
-def getLocationFieldList(self):
+POST api/v2/settings/connectors/delete payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## searchConnectors(pageNumber, pageSize, usedCount, payload)
+> Retrieve a List of Connectors. Returns JSON entity containing Connector information that was passed in from the Request payload. Please note, Compatible Connectors are not returned by this API, but can be returned when querying a single Connector using the /api/v2/settings/connectors/{connectorId} API.
+```
+POST api/v2/settings/connectors/quicksearch payload
+```
+|Parameter|Type|
+|---|---|
+|pageNumber|number|
+|pageSize|number|
+|usedCount|boolean|
+|payload|object|
+
+## deleteConnectorImage(connectorId)
+> Delete a Connector Image using the Connector ID.
+```
+DELETE api/v2/settings/connectors/{connectorId}/images
 ```
-> Returns a list of all Location fields.
+|Parameter|Type|
+|---|---|
+|connectorId|number|
```

