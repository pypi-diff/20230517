# Comparing `tmp/pyXDSM-2.2.2-py3-none-any.whl.zip` & `tmp/pyXDSM-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14481 bytes, number of entries: 9
--rw-r--r--  2.0 unx    25189 b- defN 22-Aug-25 14:43 pyxdsm/XDSM.py
--rw-r--r--  2.0 unx       22 b- defN 22-Aug-25 14:43 pyxdsm/__init__.py
--rwxr-xr-x  2.0 unx     4164 b- defN 22-Aug-25 14:43 pyxdsm/diagram_styles.tex
--rw-r--r--  2.0 unx    20479 b- defN 22-Aug-25 14:43 pyxdsm/matrix_eqn.py
--rw-r--r--  2.0 unx      558 b- defN 22-Aug-25 14:43 pyXDSM-2.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2368 b- defN 22-Aug-25 14:43 pyXDSM-2.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-25 14:43 pyXDSM-2.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Aug-25 14:43 pyXDSM-2.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      688 b- defN 22-Aug-25 14:43 pyXDSM-2.2.2.dist-info/RECORD
-9 files, 53567 bytes uncompressed, 13305 bytes compressed:  75.2%
+Zip file size: 15329 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    28866 b- defN 23-May-17 17:31 pyxdsm/XDSM.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-17 17:31 pyxdsm/__init__.py
+-rwxr-xr-x  2.0 unx     4481 b- defN 23-May-17 17:31 pyxdsm/diagram_styles.tex
+-rw-r--r--  2.0 unx    20472 b- defN 23-May-17 17:31 pyxdsm/matrix_eqn.py
+-rw-r--r--  2.0 unx      527 b- defN 23-May-17 17:31 pyXDSM-2.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2309 b- defN 23-May-17 17:31 pyXDSM-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 17:31 pyXDSM-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-17 17:31 pyXDSM-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      688 b- defN 23-May-17 17:31 pyXDSM-2.3.0.dist-info/RECORD
+9 files, 57464 bytes uncompressed, 14153 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pyxdsm/diagram_styles.tex
 Comment: 
 
 Filename: pyxdsm/matrix_eqn.py
 Comment: 
 
-Filename: pyXDSM-2.2.2.dist-info/LICENSE.txt
+Filename: pyXDSM-2.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyXDSM-2.2.2.dist-info/METADATA
+Filename: pyXDSM-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: pyXDSM-2.2.2.dist-info/WHEEL
+Filename: pyXDSM-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyXDSM-2.2.2.dist-info/top_level.txt
+Filename: pyXDSM-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyXDSM-2.2.2.dist-info/RECORD
+Filename: pyXDSM-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxdsm/XDSM.py

```diff
@@ -109,58 +109,86 @@
         if var:
             spec.add(var)
 
 
 System = namedtuple("System", "node_name style label stack faded label_width spec_name")
 Input = namedtuple("Input", "node_name label label_width style stack faded")
 Output = namedtuple("Output", "node_name label label_width style stack faded side")
-Connection = namedtuple("Connection", "src target label label_width style stack faded")
+Connection = namedtuple("Connection", "src target label label_width style stack faded src_faded target_faded")
+Process = namedtuple("Process", "systems arrow faded")
 
 
-class XDSM(object):
-    def __init__(self, use_sfmath=True, optional_latex_packages=None):
+class XDSM:
+    def __init__(self, use_sfmath=True, optional_latex_packages=None, auto_fade=None):
         """Initialize XDSM object
 
         Parameters
         ----------
         use_sfmath : bool, optional
             Whether to use the sfmath latex package, by default True
         optional_latex_packages : string or list of strings, optional
             Additional latex packages to use when creating the pdf and tex versions of the diagram, by default None
+        auto_fade : dictionary, optional
+            Controls the automatic fading of inputs, outputs, connections and processes based on the fading of diagonal blocks. For each key "inputs", "outputs", "connections", and "processes", the value can be one of:
+            - "all" : fade all blocks
+            - "connected" : fade all components connected to faded blocks (both source and target must be faded for a conncection to be faded)
+            - "none" : do not auto-fade anything
+            For connections there are two additional options:
+            - "incoming" : Fade all connections that are incoming to faded blocks.
+            - "outgoing" : Fade all connections that are outgoing from faded blocks.
         """
         self.systems = []
         self.connections = []
         self.left_outs = {}
         self.right_outs = {}
         self.ins = {}
         self.processes = []
-        self.process_arrows = []
 
         self.use_sfmath = use_sfmath
         if optional_latex_packages is None:
             self.optional_packages = []
         else:
             if isinstance(optional_latex_packages, str):
                 self.optional_packages = [optional_latex_packages]
             elif isinstance(optional_latex_packages, list):
                 self.optional_packages = optional_latex_packages
             else:
                 raise ValueError("optional_latex_packages must be a string or a list of strings")
 
+        self.auto_fade = {"inputs": "none", "outputs": "none", "connections": "none", "processes": "none"}
+        fade_options = ["all", "connected", "none"]
+        if auto_fade is not None:
+            if any([key not in self.auto_fade for key in auto_fade.keys()]):
+                raise ValueError(
+                    "The supplied 'auto_fade' dictionary contains keys that are not recognized. "
+                    + "valid keys are 'inputs', 'outputs', 'connections', 'processes'."
+                )
+
+            self.auto_fade.update(auto_fade)
+        for key in self.auto_fade.keys():
+            option_is_valid = self.auto_fade[key] in fade_options or (
+                key == "connections" and self.auto_fade[key] in ["incoming", "outgoing"]
+            )
+            if not option_is_valid:
+                raise ValueError(
+                    f"The supplied 'auto_fade' dictionary contains an invalid value: '{key}'. "
+                    + "valid values are 'all', 'connected', 'none', 'incoming', 'outgoing'."
+                )
+
     def add_system(
         self,
         node_name,
         style,
         label,
         stack=False,
         faded=False,
         label_width=None,
         spec_name=None,
     ):
-        """
+        r"""
         Add a "system" block, which will be placed on the diagonal of the XDSM diagram.
 
         Parameters
         ----------
         node_name : str
             The unique name given to this component
 
@@ -194,15 +222,15 @@
         if spec_name is None:
             spec_name = node_name
 
         sys = System(node_name, style, label, stack, faded, label_width, spec_name)
         self.systems.append(sys)
 
     def add_input(self, name, label, label_width=None, style="DataIO", stack=False, faded=False):
-        """
+        r"""
         Add an input, which will appear in the top row of the diagram.
 
         Parameters
         ----------
         name : str
             The unique name given to this component
 
@@ -225,18 +253,25 @@
         stack : bool
             If true, the system will be displayed as several stacked rectangles,
             indicating the component is executed in parallel.
 
         faded : bool
             If true, the component will be faded, in order to highlight some other system.
         """
+        sys_faded = {}
+        for s in self.systems:
+            sys_faded[s.node_name] = s.faded
+        if (self.auto_fade["inputs"] == "all") or (
+            self.auto_fade["inputs"] == "connected" and name in sys_faded and sys_faded[name]
+        ):
+            faded = True
         self.ins[name] = Input("output_" + name, label, label_width, style, stack, faded)
 
     def add_output(self, name, label, label_width=None, style="DataIO", stack=False, faded=False, side="left"):
-        """
+        r"""
         Add an output, which will appear in the left or right-most column of the diagram.
 
         Parameters
         ----------
         name : str
             The unique name given to this component
 
@@ -263,14 +298,21 @@
         faded : bool
             If true, the component will be faded, in order to highlight some other system.
 
         side : str
             Must be one of ``['left', 'right']``. This parameter controls whether the output
             is placed on the left-most column or the right-most column of the diagram.
         """
+        sys_faded = {}
+        for s in self.systems:
+            sys_faded[s.node_name] = s.faded
+        if (self.auto_fade["outputs"] == "all") or (
+            self.auto_fade["outputs"] == "connected" and name in sys_faded and sys_faded[name]
+        ):
+            faded = True
         if side == "left":
             self.left_outs[name] = Output("left_output_" + name, label, label_width, style, stack, faded, side)
         elif side == "right":
             self.right_outs[name] = Output("right_output_" + name, label, label_width, style, stack, faded, side)
         else:
             raise ValueError("The option 'side' must be given as either 'left' or 'right'!")
 
@@ -280,15 +322,15 @@
         target,
         label,
         label_width=None,
         style="DataInter",
         stack=False,
         faded=False,
     ):
-        """
+        r"""
         Connects two components with a data line, and adds a label to indicate
         the data being transferred.
 
         Parameters
         ----------
         src : str
             The name of the source component.
@@ -321,32 +363,56 @@
         """
         if src == target:
             raise ValueError("Can not connect component to itself")
 
         if (not isinstance(label_width, int)) and (label_width is not None):
             raise ValueError("label_width argument must be an integer")
 
-        self.connections.append(Connection(src, target, label, label_width, style, stack, faded))
+        sys_faded = {}
+        for s in self.systems:
+            sys_faded[s.node_name] = s.faded
+
+        allFaded = self.auto_fade["connections"] == "all"
+        srcFaded = src in sys_faded and sys_faded[src]
+        targetFaded = target in sys_faded and sys_faded[target]
+        if (
+            allFaded
+            or (self.auto_fade["connections"] == "connected" and (srcFaded and targetFaded))
+            or (self.auto_fade["connections"] == "incoming" and targetFaded)
+            or (self.auto_fade["connections"] == "outgoing" and srcFaded)
+        ):
+            faded = True
+
+        self.connections.append(Connection(src, target, label, label_width, style, stack, faded, srcFaded, targetFaded))
 
-    def add_process(self, systems, arrow=True):
+    def add_process(self, systems, arrow=True, faded=False):
         """
         Add a process line between a list of systems, to indicate process flow.
 
         Parameters
         ----------
         systems : list
             The names of the components, in the order in which they should be connected.
             For a complete cycle, repeat the first component as the last component.
 
         arrow : bool
             If true, arrows will be added to the process lines to indicate the direction
             of the process flow.
         """
-        self.processes.append(systems)
-        self.process_arrows.append(arrow)
+        sys_faded = {}
+        for s in self.systems:
+            sys_faded[s.node_name] = s.faded
+        if (self.auto_fade["processes"] == "all") or (
+            self.auto_fade["processes"] == "connected"
+            and any(
+                [sys_faded[s] for s in systems if s in sys_faded.keys()]
+            )  # sometimes a process may contain off-diagonal blocks
+        ):
+            faded = True
+        self.processes.append(Process(systems, arrow, faded))
 
     def _build_node_grid(self):
         size = len(self.systems)
 
         comps_rows = np.arange(size)
         comps_cols = np.arange(size)
 
@@ -466,20 +532,24 @@
 
     def _build_edges(self):
         h_edges = []
         v_edges = []
 
         edge_format_string = "({start}) edge [{style}] ({end})"
         for conn in self.connections:
-            style = "DataLine"
-            if conn.faded:
-                style += ",faded"
+            h_edge_style = "DataLine"
+            v_edge_style = "DataLine"
+            if conn.src_faded or conn.faded:
+                h_edge_style += ",faded"
+            if conn.target_faded or conn.faded:
+                v_edge_style += ",faded"
             od_node_name = "{}-{}".format(conn.src, conn.target)
-            h_edges.append(edge_format_string.format(start=conn.src, end=od_node_name, style=style))
-            v_edges.append(edge_format_string.format(start=od_node_name, end=conn.target, style=style))
+
+            h_edges.append(edge_format_string.format(start=conn.src, end=od_node_name, style=h_edge_style))
+            v_edges.append(edge_format_string.format(start=od_node_name, end=conn.target, style=v_edge_style))
 
         for comp_name, out in self.left_outs.items():
             style = "DataLine"
             if out.faded:
                 style += ",faded"
             node_name = out.node_name
             h_edges.append(edge_format_string.format(start=comp_name, end=node_name, style=style))
@@ -494,14 +564,17 @@
         for comp_name, inp in self.ins.items():
             style = "DataLine"
             if inp.faded:
                 style += ",faded"
             node_name = inp.node_name
             v_edges.append(edge_format_string.format(start=comp_name, end=node_name, style=style))
 
+        h_edges = sorted(h_edges, key=lambda s: "faded" in s)
+        v_edges = sorted(v_edges, key=lambda s: "faded" in s)
+
         paths_str = "% Horizontal edges\n" + "\n".join(h_edges) + "\n"
         paths_str += "% Vertical edges\n" + "\n".join(v_edges) + ";"
 
         return paths_str
 
     def _build_process_chain(self):
         sys_names = [s.node_name for s in self.systems]
@@ -510,43 +583,45 @@
             + [data[0] for _, data in self.left_outs.items()]
             + [data[0] for _, data in self.right_outs.items()]
         )
         # comp_name, in_data in self.ins.items():
         #     node_name, style, label, stack = in_data
         chain_str = ""
 
-        for proc, arrow in zip(self.processes, self.process_arrows):
+        for proc in self.processes:
             chain_str += "{ [start chain=process]\n \\begin{pgfonlayer}{process} \n"
             start_tip = False
-            for i, sys in enumerate(proc):
+            for i, sys in enumerate(proc.systems):
                 if sys not in sys_names and sys not in output_names:
                     raise ValueError(
                         'process includes a system named "{}" but no system with that name exists.'.format(sys)
                     )
                 if sys in output_names and i == 0:
                     start_tip = True
                 if i == 0:
                     chain_str += "\\chainin ({});\n".format(sys)
                 else:
                     if sys in output_names or (i == 1 and start_tip):
-                        if arrow:
-                            chain_str += "\\chainin ({}) [join=by ProcessTipA];\n".format(sys)
+                        if proc.arrow:
+                            style = "ProcessTipA"
                         else:
-                            chain_str += "\\chainin ({}) [join=by ProcessTip];\n".format(sys)
+                            style = "ProcessTip"
                     else:
-                        if arrow:
-                            chain_str += "\\chainin ({}) [join=by ProcessHVA];\n".format(sys)
+                        if proc.arrow:
+                            style = "ProcessHVA"
                         else:
-                            chain_str += "\\chainin ({}) [join=by ProcessHV];\n".format(sys)
+                            style = "ProcessHV"
+                    if proc.faded:
+                        style = "Faded" + style
+                    chain_str += "\\chainin ({}) [join=by {}];\n".format(sys, style)
             chain_str += "\\end{pgfonlayer}\n}"
 
         return chain_str
 
     def _compose_optional_package_list(self):
-
         # Check for optional LaTeX packages
         optional_packages_list = self.optional_packages
         if self.use_sfmath:
             optional_packages_list.append("sfmath")
 
         # Join all packages into one string separated by comma
         optional_packages_str = ",".join(optional_packages_list)
```

## pyxdsm/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "2.2.2"
+__version__ = "2.3.0"
```

## pyxdsm/diagram_styles.tex

```diff
@@ -59,14 +59,18 @@
 
 % Edges
 \tikzstyle{DataLine} = [color=black!40,line width=5pt,line cap=rect]
 \tikzstyle{ProcessHV} = [-,line width=1pt,to path={-| (\tikztotarget)}]
 \tikzstyle{ProcessHVA} = [->,line width=1pt,to path={-| (\tikztotarget)}]
 \tikzstyle{ProcessTip} = [-,line width=1pt]
 \tikzstyle{ProcessTipA} = [->, line width=1pt]
+\tikzstyle{FadedProcessHV} = [-,line width=1pt,to path={-| (\tikztotarget)},color=black!30]
+\tikzstyle{FadedProcessHVA} = [->,line width=1pt,to path={-| (\tikztotarget)},color=black!30]
+\tikzstyle{FadedProcessTip} = [-,line width=1pt,color=black!30]
+\tikzstyle{FadedProcessTipA} = [->, line width=1pt,color=black!30]
 
 % Matrix options
 \tikzstyle{MatrixSetup} = [row sep=3mm, column sep=2mm]
 
 % Declare a background layer for showing node connections
 \pgfdeclarelayer{data}
 \pgfdeclarelayer{process}
```

## pyxdsm/matrix_eqn.py

```diff
@@ -275,15 +275,14 @@
         if isinstance(target, (list, tuple)):
             for t in target:
                 self._connections[src, t] = CellData(text=text, color=color, highlight="diag")
         else:
             self._connections[src, target] = CellData(text=text, color=color, highlight="diag")
 
     def _process_vars(self):
-
         if self._setup:
             return
 
         # deal with connections
         for (src, target), cell_data in self._connections.items():
             i_src = self._variables[src].idx
             j_target = self._variables[target].idx
@@ -393,15 +392,14 @@
         self._variables[name] = Variable(size=size, idx=self._n_vars, text=text, color=color)
         self._ij_variables[self._n_vars] = self._variables[name]
         self._n_vars += 1
 
         self._total_size += size
 
     def connect(self, src, target, text="", color=None, highlight=1):
-
         if isinstance(target, (list, tuple)):
             for t in target:
                 self._connections[src, t] = CellData(text=text, color=color, highlight=highlight)
         else:
             self._connections[src, target] = CellData(text=text, color=color, highlight=highlight)
 
     def text(self, src, target, text):
@@ -426,15 +424,14 @@
             j_target = self._variables[target].idx
 
             self._ij_text[i_src, j_target] = cell_data
 
         self._setup = True
 
     def jacobian(self, transpose=False):
-
         self._process_vars()
 
         tikz = []
 
         for i in range(self._n_vars):
             tikz.append(r"\blockrow{")
 
@@ -474,24 +471,22 @@
 
         lhs_tikz = "\n".join(tikz)
 
         self._terms.append(lhs_tikz)
         return lhs_tikz
 
     def vector(self, base_color="red", highlight=None):
-
         self._process_vars()
 
         tikz = []
 
         if highlight is None:
             highlight = np.ones(self._n_vars)
 
         for i, h_light in enumerate(highlight):
-
             color = _color(base_color, h_light)
 
             row_size = self._ij_variables[i].size
 
             tikz.append(r"\blockrow{\blockcol{")
             if h_light == "diag":
                 tikz.append(
@@ -505,15 +500,14 @@
 
         vec_tikz = "\n".join(tikz)
 
         self._terms.append(vec_tikz)
         return vec_tikz
 
     def operator(self, opperator="="):
-
         self._process_vars()
 
         tikz = []
 
         padding_size = (self._total_size - 1) / 2
 
         tikz.append(r"\blockrow{")
@@ -524,15 +518,14 @@
 
         op_tikz = "\n".join(tikz)
 
         self._terms.append(op_tikz)
         return op_tikz
 
     def spacer(self):
-
         self._process_vars()
 
         tikz = []
 
         for i in range(self._n_vars):
             row_size = self._ij_variables[i].size
```

## Comparing `pyXDSM-2.2.2.dist-info/LICENSE.txt` & `pyXDSM-2.3.0.dist-info/LICENSE.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-OpenMDAO Open Source License:
-
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this software except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
```

## Comparing `pyXDSM-2.2.2.dist-info/METADATA` & `pyXDSM-2.3.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXDSM
-Version: 2.2.2
+Version: 2.3.0
 Summary: Python script to generate PDF XDSM diagrams using TikZ and LaTeX
 Home-page: https://github.com/mdolab/pyXDSM
 Author: 
 Author-email: 
 License: Apache License Version 2.0
 Keywords: optimization multidisciplinary multi-disciplinary analysis n2 xdsm
 Platform: UNKNOWN
@@ -13,18 +13,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: numpy (>=1.16)
 
 # pyXDSM
-[![Build Status](https://dev.azure.com/mdolab/Public/_apis/build/status/mdolab.pyXDSM?repoName=mdolab%2FpyXDSM&branchName=main)](https://dev.azure.com/mdolab/Public/_build/latest?definitionId=33&repoName=mdolab%2FpyXDSM&branchName=main)
+[![Build Status](https://github.com/mdolab/pyXDSM/actions/workflows/test.yaml/badge.svg)](https://github.com/mdolab/pyXDSM/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.com/projects/mdolab-pyxdsm/badge/?version=latest)](https://mdolab-pyxdsm.readthedocs-hosted.com/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/pyxdsm)](https://pypi.org/project/pyXDSM/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyXDSM)
 
 A python library for generating publication quality PDF XDSM diagrams.
 This library is a thin wrapper that uses the TikZ library and LaTeX to build the PDFs.
```

## Comparing `pyXDSM-2.2.2.dist-info/RECORD` & `pyXDSM-2.3.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyxdsm/XDSM.py,sha256=HfyxZ0La6Ga2DhtX-_vMvpTmhxTG0zKegkXUW6jrBZs,25189
-pyxdsm/__init__.py,sha256=toAYzE_ok1SiBE0AqAVdW0O8YCXCwcx0w4JATYQuJOg,22
-pyxdsm/diagram_styles.tex,sha256=eH5HfyvW6dBjs0wSjesD0eE1ZsD20BNFrLLpoUr0s6Q,4164
-pyxdsm/matrix_eqn.py,sha256=GWUimUTyXNJZxWTOgWDI2XEh0fvpSdhl5MKO_2n7Juo,20479
-pyXDSM-2.2.2.dist-info/LICENSE.txt,sha256=LWjQpabMPeNN0FWFsTUJNGh8sSllfPl5amuEwVEP8es,558
-pyXDSM-2.2.2.dist-info/METADATA,sha256=w_vSiown2cYkYjPnzeqMWFfYCrXav3HlkW1iyZJjHNU,2368
-pyXDSM-2.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyXDSM-2.2.2.dist-info/top_level.txt,sha256=npcGjPKP63Oa98ZaKheVJDcSdxotLSxRHaCoCWCvCb4,7
-pyXDSM-2.2.2.dist-info/RECORD,,
+pyxdsm/XDSM.py,sha256=YyJlgA3Q5yhklDw_hPOERTPE0opVU9olSE9vimDnFNY,28866
+pyxdsm/__init__.py,sha256=CpK8IH_dCUAwg9tqv7zm9FxbBFkxCnED1JUiRe7cftU,22
+pyxdsm/diagram_styles.tex,sha256=5gr3bdHFWgf7Xf5on8ng3mQ4tHkQxaxqWcXkxIs3ViY,4481
+pyxdsm/matrix_eqn.py,sha256=4_gDqbJGtR8lrU5EQ0sNGRed_P4y0_MK-QDh8dzx-ec,20472
+pyXDSM-2.3.0.dist-info/LICENSE.txt,sha256=HVRWxdwgwMREFZkP3-3iL4dFs9Y55PAJD24YBuN5JL0,527
+pyXDSM-2.3.0.dist-info/METADATA,sha256=D6ph5Yi-Lo-OK2wPS9O09uxij57hMzSp5UyXQQeNgv8,2309
+pyXDSM-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyXDSM-2.3.0.dist-info/top_level.txt,sha256=npcGjPKP63Oa98ZaKheVJDcSdxotLSxRHaCoCWCvCb4,7
+pyXDSM-2.3.0.dist-info/RECORD,,
```

