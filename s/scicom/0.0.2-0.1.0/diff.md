# Comparing `tmp/scicom-0.0.2.tar.gz` & `tmp/scicom-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicom-0.0.2.tar", last modified: Tue Nov 15 10:52:06 2022, max compression
+gzip compressed data, was "scicom-0.1.0.tar", last modified: Wed May 17 13:12:39 2023, max compression
```

## Comparing `scicom-0.0.2.tar` & `scicom-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.355989 scicom-0.0.2/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      183 2022-11-11 14:57:57.000000 scicom-0.0.2/AUTHORS.rst
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1086 2022-11-11 14:57:57.000000 scicom-0.0.2/LICENSE.md
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     2013 2022-11-15 10:52:06.355989 scicom-0.0.2/PKG-INFO
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1235 2022-11-15 10:51:15.000000 scicom-0.0.2/README.md
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      104 2022-11-11 14:57:57.000000 scicom-0.0.2/pyproject.toml
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      952 2022-11-15 10:52:06.355989 scicom-0.0.2/setup.cfg
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.351989 scicom-0.0.2/src/
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.355989 scicom-0.0.2/src/scicom/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2022-11-11 14:57:57.000000 scicom-0.0.2/src/scicom/__init__.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.355989 scicom-0.0.2/src/scicom/letters/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2022-11-11 14:57:57.000000 scicom-0.0.2/src/scicom/letters/__init__.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.355989 scicom-0.0.2/src/scicom/letters/letters/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1194 2022-11-11 14:57:57.000000 scicom-0.0.2/src/scicom/letters/letters/SimpleContinuousModule.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2022-11-11 14:57:57.000000 scicom-0.0.2/src/scicom/letters/letters/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     2726 2022-11-15 09:38:50.000000 scicom-0.0.2/src/scicom/letters/letters/model.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4830 2022-11-15 09:38:43.000000 scicom-0.0.2/src/scicom/letters/letters/randomletter.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     3166 2022-11-15 09:38:41.000000 scicom-0.0.2/src/scicom/letters/letters/server.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)       51 2022-11-11 14:57:57.000000 scicom-0.0.2/src/scicom/letters/run.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2022-11-15 10:52:06.355989 scicom-0.0.2/src/scicom.egg-info/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     2013 2022-11-15 10:52:06.000000 scicom-0.0.2/src/scicom.egg-info/PKG-INFO
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      514 2022-11-15 10:52:06.000000 scicom-0.0.2/src/scicom.egg-info/SOURCES.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        1 2022-11-15 10:52:06.000000 scicom-0.0.2/src/scicom.egg-info/dependency_links.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)       83 2022-11-15 10:52:06.000000 scicom-0.0.2/src/scicom.egg-info/requires.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        7 2022-11-15 10:52:06.000000 scicom-0.0.2/src/scicom.egg-info/top_level.txt
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      232 2023-05-04 13:08:18.000000 scicom-0.1.0/AUTHORS.rst
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1086 2022-01-06 13:40:40.000000 scicom-0.1.0/LICENSE.md
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)       28 2023-05-08 08:24:28.000000 scicom-0.1.0/MANIFEST.in
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-05-17 13:12:39.769400 scicom-0.1.0/PKG-INFO
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1670 2023-01-16 10:15:23.000000 scicom-0.1.0/README.md
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      104 2021-09-30 09:13:37.000000 scicom-0.1.0/pyproject.toml
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1011 2023-05-17 13:12:39.769400 scicom-0.1.0/setup.cfg
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.765400 scicom-0.1.0/src/
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.765400 scicom-0.1.0/src/scicom/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.0/src/scicom/__init__.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/data/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    22954 2023-05-17 13:09:30.000000 scicom-0.1.0/src/scicom/data/agentsCoordinates.geojson
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)   327135 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     7225 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/relPop_plosOne.csv
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    73605 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/relativePopulation_1650.csv
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/historicalletters/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2023-05-04 12:33:04.000000 scicom-0.1.0/src/scicom/historicalletters/__init__.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     7915 2023-05-17 09:50:10.000000 scicom-0.1.0/src/scicom/historicalletters/agents.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4148 2023-05-15 09:22:32.000000 scicom-0.1.0/src/scicom/historicalletters/model.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2293 2023-05-15 09:25:08.000000 scicom-0.1.0/src/scicom/historicalletters/server.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2661 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/historicalletters/space.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1257 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/historicalletters/util.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/randomletters/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1206 2023-05-04 12:39:24.000000 scicom-0.1.0/src/scicom/randomletters/SimpleContinuousModule.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.0/src/scicom/randomletters/__init__.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4837 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/agents.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2723 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/model.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     3197 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/server.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      610 2023-05-04 12:51:27.000000 scicom-0.1.0/src/scicom/run.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom.egg-info/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/PKG-INFO
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      871 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/SOURCES.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        1 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/dependency_links.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      111 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/requires.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        7 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/top_level.txt
```

### Comparing `scicom-0.0.2/LICENSE.md` & `scicom-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scicom-0.0.2/setup.cfg` & `scicom-0.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scicom
-version = 0.0.2
+version = 0.1.0
 author = Bernardo S. Buarque, Malte Vogl
 author_email = bsbuarque@mpiwg-berlin.mpg.de, mvogl@mpiwg-berlin.mpg.de
 description = Simulating various aspects of scientific communication via Agent-based models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 project_urls = 
@@ -15,21 +15,24 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
+include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	mesa
+	mesa-geo
+	shapely >=2
 	pandas
 	networkx
 	numpy
-	cartopy
+	convert2geojson
 
 [options.extras_require]
 all = 
 	%(dev)s
 dev = 
 	twine
 	tox
```

### Comparing `scicom-0.0.2/src/scicom/letters/letters/SimpleContinuousModule.py` & `scicom-0.1.0/src/scicom/randomletters/SimpleContinuousModule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import mesa
 
 
 class SimpleCanvas(mesa.visualization.VisualizationElement):
-    local_includes = ["letters/simple_continuous_canvas.js"]
-    local_css_includes = ["letters/map.png"]
+    local_includes = ["randomletters/simple_continuous_canvas.js"]
+    local_css_includes = ["randomletters/map.png"]
     portrayal_method = None
     canvas_height = 720
     canvas_width = 1280
 
     def __init__(self, portrayal_method, canvas_height=720, canvas_width=1280):
         """
         Instantiate a new SimpleCanvas
```

### Comparing `scicom-0.0.2/src/scicom/letters/letters/model.py` & `scicom-0.1.0/src/scicom/randomletters/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import mesa
 import numpy as np
 import networkx as nx
 
-from .randomletter import LetterAgent, LetterNode
+from .agents import LetterAgent, LetterNode
 
 
 class LetterSpace(mesa.Model):
     """
     Letter sending model class. Handles agent creation, placement and scheduling.
 
     Each agent has a personal topic vector representing
@@ -57,15 +57,15 @@
             letter = LetterAgent(
                 i,
                 self,
                 pos,
                 topicVec,
                 **self.factors
             )
-            nx.set_node_attributes(self.G, {i:{'numLettersSend':0, 'numLettersReceived':0}})
+            nx.set_node_attributes(self.G, {i: {'numLettersSend': 0, 'numLettersReceived': 0}})
             letterNode = LetterNode(
                 i,
                 self,
                 topicVec,
             )
             self.space.place_agent(letter, pos)
             self.grid.place_agent(letterNode, node)
```

### Comparing `scicom-0.0.2/src/scicom/letters/letters/randomletter.py` & `scicom-0.1.0/src/scicom/randomletters/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import mesa
 import numpy as np
 
 
 class LetterAgent(mesa.Agent):
     """An agent with fixed initial start position.
-   
+  
     Each agent has a personal topic vector representing
     the shares the agent has of topics 1 to 10 with values
     between 0 and 1.
     Each agent has two different ranges, moveRange for deciding
     to move to another agents position, and letterRange to find
     potential correspondence partners. In addition a threshold
     value determines the necessary similarity between topic vectors
@@ -52,15 +52,15 @@
             for n in neighbors:
                 possible_steps.append(n.pos)
                 weights.append(n.lettersReceived)
             move = np.random.choice([0, 0, 0, 0, 0, 0, 0, 1])
             if move == 1:
                 new_position = self.random.choice(possible_steps)
                 self.model.space.move_agent(self, new_position)
-   
+  
     def sendLetter(self, neighbors):
         """Sending a letter based on an urn model."""
         possibleRec = []
         senders = self.lettersReceived
         receivers = self.lettersSend
         possibleRec.extend(senders)
         possibleRec.extend(receivers)
@@ -97,16 +97,16 @@
                 updateTopicVec = self.topicVec + self.updateTopic * np.random.uniform(0, 1) * (recipient.topicVec - self.topicVec)
                 self.model.letterLedger.append(
                     (self.unique_id, recipient.unique_id, self.pos, recipient.pos, updateTopicVec, self.model.schedule.steps)
                 )
                 self.topicLedger.append(
                     self.topicVec
                 )
-                self.topicVec = updateTopicVec      
-
+                self.topicVec = updateTopicVec
+               
     def step(self):
         neighborsMove = self.model.space.get_neighbors(self.pos, self.moveRange, False)
         neighborsSend = self.model.space.get_neighbors(self.pos, self.letterRange, False)
         self.sendLetter(neighborsSend)
         self.move(neighborsMove)
```

### Comparing `scicom-0.0.2/src/scicom/letters/letters/server.py` & `scicom-0.1.0/src/scicom/randomletters/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
         "Shape": "circle",
         "r": agent.numLettersReceived,
         "Filled": "true",
         "Color": color
     }
     return probDict
 
+
 def node_draw(G):
     nodes = []
     node_label_to_node_id = {}
     node_id = 0
-    edge_id = 0
+    # edge_id = 0
     for node_label, agents in G.nodes.data("agent"):
         node = G.nodes()[node_label]
         agent = agents[0]
         colortuple = set(agent.topicVec)
         nodes.append({
             "size": node["numLettersReceived"],
-            "color":  "#" + "".join(format(int(round(val * 255)), "02x") for val in colortuple),
+            "color": "#" + "".join(format(int(round(val * 255)), "02x") for val in colortuple),
             "tooltip": f"id: {agent.unique_id}<br>Topics: {agent.topicVec}",
         })
         node_label_to_node_id[node_label] = node_id
         node_id += 1
 
     portrayal = dict()
     portrayal["nodes"] = nodes
@@ -68,24 +69,28 @@
         "Strength of adoption",
         0.05,
         0.01,
         0.3,
         0.05,
         description="Choose how strongly letter sending changes ones topics.",
     ),
-    "updateHelp": mesa.visualization.StaticText("Higher value:<br/> A letter sender faster adopts to the topic of a receiver."),
+    "updateHelp": mesa.visualization.StaticText(
+        "Higher value:<br/> A letter sender faster adopts to the topic of a receiver."
+    ),
     "threshold": mesa.visualization.Slider(
         "Similarity threshold",
         0.5,
         0.0,
         1.0,
         0.1,
         description="Choose how similar two persons topics have to be, to send a letter.",
     ),
-    "thresholdHelp": mesa.visualization.StaticText("Higher value:<br/> Sending a letter is less likely."),
+    "thresholdHelp": mesa.visualization.StaticText(
+        "Higher value:<br/> Sending a letter is less likely."
+    ),
     "width": 360,
     "height": 180,
     "moveRange": mesa.visualization.Slider(
         "Range for moving position",
         20,
         0,
         100,
@@ -101,8 +106,8 @@
         description="Choose the visibility range for finding potential receipients.",
     ),
     "minSep": 3
 }
 
 server = mesa.visualization.ModularServer(
     LetterSpace, [letter_canvas, network_canvas], "Random Letters", model_params
-)
+)
```

