# Comparing `tmp/d3graph-2.4.5.tar.gz` & `tmp/d3graph-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\d3graph-2.4.5.tar", last modified: Tue May 16 17:53:03 2023, max compression
+gzip compressed data, was "d3graph-2.4.6.tar", last modified: Wed May 17 20:44:31 2023, max compression
```

## Comparing `d3graph-2.4.5.tar` & `d3graph-2.4.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.120359 d3graph-2.4.5/
--rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.5/LICENSE
--rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6289 2023-05-16 17:53:03.120359 d3graph-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.099385 d3graph-2.4.5/d3graph/
--rw-rw-rw-   0        0        0     1652 2023-05-16 17:51:26.000000 d3graph-2.4.5/d3graph/__init__.py
--rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.5/d3graph/adjmat_vec.py
--rw-rw-rw-   0        0        0    56679 2023-05-16 17:11:42.000000 d3graph-2.4.5/d3graph/d3graph.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.117340 d3graph-2.4.5/d3graph/d3js/
--rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/__init__.py
--rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    11158 2023-05-16 10:08:09.000000 d3graph-2.4.5/d3graph/d3js/d3graphscript.js
--rw-rw-rw-   0        0        0     1253 2023-05-16 10:07:47.000000 d3graph-2.4.5/d3graph/d3js/index.html.j2
--rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/style.css
--rw-rw-rw-   0        0        0    18011 2023-05-16 13:01:27.000000 d3graph-2.4.5/d3graph/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.111354 d3graph-2.4.5/d3graph.egg-info/
--rw-rw-rw-   0        0        0     6289 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-05-16 17:53:03.124323 d3graph-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.119334 d3graph-2.4.5/tests/
--rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.5/tests/__init__.py
--rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.5/tests/conftest.py
--rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.5/tests/test_d3graph.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:44:31.162736 d3graph-2.4.6/
+-rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6248 2023-05-17 20:44:31.163734 d3graph-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 20:44:31.068270 d3graph-2.4.6/d3graph/
+-rw-rw-rw-   0        0        0     1652 2023-05-17 20:39:46.000000 d3graph-2.4.6/d3graph/__init__.py
+-rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.6/d3graph/adjmat_vec.py
+-rw-rw-rw-   0        0        0    57248 2023-05-17 20:37:18.000000 d3graph-2.4.6/d3graph/d3graph.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:44:31.136291 d3graph-2.4.6/d3graph/d3js/
+-rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.6/d3graph/d3js/__init__.py
+-rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.6/d3graph/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    11193 2023-05-16 21:50:16.000000 d3graph-2.4.6/d3graph/d3js/d3graphscript.js
+-rw-rw-rw-   0        0        0     1278 2023-05-17 20:33:43.000000 d3graph-2.4.6/d3graph/d3js/index.html.j2
+-rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.6/d3graph/d3js/style.css
+-rw-rw-rw-   0        0        0    18024 2023-05-17 20:42:53.000000 d3graph-2.4.6/d3graph/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:44:31.099695 d3graph-2.4.6/d3graph.egg-info/
+-rw-rw-rw-   0        0        0     6248 2023-05-17 20:44:30.000000 d3graph-2.4.6/d3graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-17 20:44:30.000000 d3graph-2.4.6/d3graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:44:30.000000 d3graph-2.4.6/d3graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-05-17 20:44:30.000000 d3graph-2.4.6/d3graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 20:44:30.000000 d3graph-2.4.6/d3graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-05-17 20:44:31.180461 d3graph-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:44:31.161758 d3graph-2.4.6/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.6/tests/conftest.py
+-rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.6/tests/test_d3graph.py
```

### Comparing `d3graph-2.4.5/LICENSE` & `d3graph-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/PKG-INFO` & `d3graph-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.5.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +115,7 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `d3graph-2.4.5/README.md` & `d3graph-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/d3graph/__init__.py` & `d3graph-2.4.6/d3graph/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     json_create,
     adjmat2dict,
     data_checks,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.4.5'
+__version__ = '2.4.6'
 
 
 # module level doc-string
 __doc__ = """
 d3graph
 =======================================================================================
```

### Comparing `d3graph-2.4.5/d3graph/adjmat_vec.py` & `d3graph-2.4.6/d3graph/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/d3graph/d3graph.py` & `d3graph-2.4.6/d3graph/d3graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,29 +73,30 @@
     * D3Graph: https://towardsdatascience.com/creating-beautiful-stand-alone-interactive-d3-charts-with-python-804117cb95a7
     * D3Blocks: https://towardsdatascience.com/d3blocks-the-python-library-to-create-interactive-and-standalone-d3js-charts-3dda98ce97d4
     * Github : https://github.com/erdogant/d3graph
     * Documentation: https://erdogant.github.io/d3graph/
 
     """
 
-    def __init__(self, collision: float = 0.5, charge: int = 450, slider: List[int] = None, verbose: int = 20) -> None:
+    def __init__(self, collision: float = 0.5, charge: int = 450, slider: List[int] = None, support='text', verbose: int = 20) -> None:
         """Initialize d3graph."""
         if slider is None:
             slider = [None, None]
         # Cleaning
         self._clean()
         # Some library compatibility checks
         library_compatibility_checks()
         # Set the logger
         set_logger(verbose=verbose)
         # Setup configurations
         self.config = {}
         self.config['collision'] = collision
         self.config['charge'] = -abs(charge)
         self.config['slider'] = slider
+        self.config['support'] = get_support(support)
         # Set paths
         self.config['curpath'] = os.path.dirname(os.path.abspath(__file__))
         self.config['d3_library'] = os.path.abspath(os.path.join(self.config['curpath'], 'd3js/d3.v3.js'))
         self.config['d3_script'] = os.path.abspath(os.path.join(self.config['curpath'], 'd3js/d3graphscript.js'))
         self.config['css'] = os.path.abspath(os.path.join(self.config['curpath'], 'd3js/style.css'))
 
     def _clean(self, clean_config: bool = True) -> None:
@@ -686,17 +687,17 @@
                    'CLICK_COMMENT': CLICK_COMMENT,
                    'CLICK_FILL': click_properties['fill'],
                    'CLICK_STROKE': click_properties['stroke'],
                    'CLICK_SIZE': click_properties['size'],
                    'CLICK_STROKEW': click_properties['stroke-width'],
                    'slider_comment_start': show_slider[0],
                    'slider_comment_stop': show_slider[1],
+                   'SUPPORT': self.config['support'],
                    }
 
-        # Issue14: https://github.com/erdogant/d3graph/issues/14
         try:
             jinja_env = Environment(loader=PackageLoader(package_name=__name__, package_path='d3js'))
         except:
             jinja_env = Environment(loader=PackageLoader(package_name='d3graph', package_path='d3js'))
         index_template = jinja_env.get_template('index.html.j2')
         html = index_template.render(content)
 
@@ -1355,7 +1356,19 @@
         else:
             fontcolor = np.array(['#000080'] * nodecount)
     else:
         assert 'fontcolor not possible'
     if len(fontcolor) != nodecount: raise ValueError("[fontcolor] must be of same length as the number of nodes")
     # return
     return fontcolor
+
+
+def get_support(support):
+    script=''
+    if isinstance(support, bool) and (not support): support = None
+    if isinstance(support, bool) and support: support = 'text'
+    if support is not None:
+        script="<script async src='https://media.ethicalads.io/media/client/ethicalads.min.js'></script>"
+        script = script + '\n' + "<div data-ea-publisher='erdogantgithubio' data-ea-type='{TYPE}' data-ea-style='stickybox'></div>".replace('{TYPE}', support)
+
+    # Return
+    return script
```

### Comparing `d3graph-2.4.5/d3graph/d3js/d3.v3.js` & `d3graph-2.4.6/d3graph/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/d3graph/d3js/d3graphscript.js` & `d3graph-2.4.6/d3graph/d3js/d3graphscript.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -146,15 +146,16 @@
             return d.node_name
         }) // NODE-TEXT
         .style("font-size", function(d) {
             return d.node_fontsize + "px";
         }) // set font size equal to node edge size
         .style("fill", function(d) {
             return d.node_fontcolor;
-        }); // set the text fill color to the same as node color
+        }) // set the text fill color to the same as node color
+        .style("font-family", "monospace");
     //  .style("stroke", "gray");
 
     let showInHover = ["node_tooltip"]; // Tooltip
     node.append("title")
         .text((d) => Object.keys(d)
             .filter((key) => showInHover.indexOf(key) !== -1)
             .map((key) => `${d[key]}`)
```

### Comparing `d3graph-2.4.5/d3graph/d3js/index.html.j2` & `d3graph-2.4.6/d3graph/d3js/index.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 <!DOCTYPE html>
 
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>{{ title }}</title>
+
+    {{ SUPPORT }}
+
     <style type="text/css">
         {% include "style.css" %}
     </style>
 </head>
 <body>
 
 
@@ -25,14 +28,15 @@
                 distance: {{ edge_distance }},
                 directed: {{ directed | lower }},
                 collision: {{ collision }}
             })
         });
     </script>
 
+
 <!-- SLIDER -->
 {{ slider_comment_start }}
 
     {% if max_slider > min_slider %}
 	<div style="max-width:{{ width }}px;">
         <form>
             <h3>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
+{{ SUPPORT }}
   {{ slider_comment_start }} {% if max_slider > min_slider %}
 **** Edge Threshold {{ min_slider }} [Unknown INPUT type] {{ max_slider }} ****
 {% endif %} {{ slider_comment_stop }}
```

### Comparing `d3graph-2.4.5/d3graph/examples.py` & `d3graph-2.4.6/d3graph/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from d3graph import d3graph, adjmat2vec
 
 # %% Edge distance
 
 # Import
 from d3graph import d3graph
 # intialize to load example dataset
-d3 = d3graph()
+d3 = d3graph(support=False)
 adjmat, _ = d3.import_example('bigbang')
 
 # Initialize with clustering colors
 d3.graph(adjmat, color='cluster')
 
 # Set all edge labels to "test"
 d3.set_edge_properties(directed=True, minmax_distance=None)
```

### Comparing `d3graph-2.4.5/d3graph.egg-info/PKG-INFO` & `d3graph-2.4.6/d3graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.5.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +115,7 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `d3graph-2.4.5/setup.py` & `d3graph-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/tests/conftest.py` & `d3graph-2.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.5/tests/test_d3graph.py` & `d3graph-2.4.6/tests/test_d3graph.py`

 * *Files identical despite different names*

