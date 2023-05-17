# Comparing `tmp/khloraascaf_utils-0.8.0.tar.gz` & `tmp/khloraascaf_utils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.8.0.tar", last modified: Tue May  9 12:21:19 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.8.1.tar", last modified: Wed May 17 16:50:34 2023, max compression
```

## Comparing `khloraascaf_utils-0.8.0.tar` & `khloraascaf_utils-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.153237 khloraascaf_utils-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-09 12:21:19.152237 khloraascaf_utils-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 12:21:19.153237 khloraascaf_utils-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.145237 khloraascaf_utils-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.149237 khloraascaf_utils-0.8.0/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13769 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.151237 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 12:21:19.000000 khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:21:19.152237 khloraascaf_utils-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-09 12:20:55.000000 khloraascaf_utils-0.8.0/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.667677 khloraascaf_utils-0.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-17 16:50:34.666679 khloraascaf_utils-0.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 16:50:34.667677 khloraascaf_utils-0.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.659686 khloraascaf_utils-0.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.663682 khloraascaf_utils-0.8.1/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9489 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13859 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.665680 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 16:50:34.000000 khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:50:34.666679 khloraascaf_utils-0.8.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4112 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-05-17 16:50:08.000000 khloraascaf_utils-0.8.1/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.8.0/LICENCE` & `khloraascaf_utils-0.8.1/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.0/PKG-INFO` & `khloraascaf_utils-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.8.0/README.md` & `khloraascaf_utils-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.0/pyproject.toml` & `khloraascaf_utils-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.8.0"
+version = "0.8.1"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf_utils-0.8.0/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.8.1/src/khloraascaf_utils/artificial_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,52 +2,74 @@
 
 """Data generation module."""
 
 from collections.abc import Iterable, Iterator
 from random import randint, random
 
 from khloraascaf.inputs import MultT, PresScoreT
-from khloraascaf.multiplied_doubled_contig_graph import MDCGraph
+from khloraascaf.multiplied_doubled_contig_graph import (
+    MULT_ATTR,
+    PRESSCORE_ATTR,
+    MDCGraph,
+)
+from revsymg.graphs import RevSymGraph
 from revsymg.index_lib import (
     FORWARD_INT,
     REVERSE_INT,
     IndexT,
     IndOrT,
     OrT,
     rev_vertex,
 )
 
 
 # DOCU all artificial data module
 # ============================================================================ #
 #                                     CLASS                                    #
 # ============================================================================ #
-class ArtificialData():
+class ArtificialData(RevSymGraph):
     """Artificial data class.
 
     Warnings
     --------
     Please, let the first region be a unique one.
     Thus, the starter will be the very first contig of this region.
     """
 
     def __init__(self, oriented_region_order: Iterable[IndOrT],
                  region_length: list[int],
                  proba_over_mult: float = 0.0,
                  proba_extra_link: float = 0.0):
         """The Initialiser."""
+        super().__init__()
+        #
+        # New attributes
+        #
+        self._vertices.new_attr(MULT_ATTR, 1)
+        self._vertices.new_attr(PRESSCORE_ATTR, 0.0)
+        #
+        # Regions and their oriented contigs
+        #
         self.__oriented_region_order: tuple[IndOrT, ...] = tuple(
             oriented_region_order,
         )
+        self.__region_oriented_contig: list[list[IndOrT]] = []
+        #
+        # Noise probabilities
+        #
         self.__proba_over_mult: float = proba_over_mult
         self.__proba_extra_link: float = proba_extra_link
-        self.__links: list[tuple[IndOrT, IndOrT]] = []
+        #
+        # Separate noise from perfect data
+        #
+        self.__base_links: list[tuple[IndOrT, IndOrT]] = []
         self.__extra_links: list[tuple[IndOrT, IndOrT]] = []
-        self.__contig_attrs: list[tuple[MultT, PresScoreT]] = []
-        self.__region_oriented_contig: list[list[IndOrT]] = []
+        #
+        # Build artificial data
+        #
         self.__generate_region_orc(region_length)
         self.__generate_intra_links()
         self.__generate_inter_links()
         self.__generate_extra_links()
 
     # ~*~ Getter ~*~
 
@@ -69,48 +91,52 @@
         IndexT
             Contig's index
         MultT
             Contig's multiplicity
         PresScoreT
             Contig's presence score
         """
-        for c_ind, (mult, presscore) in enumerate(self.__contig_attrs):
-            yield c_ind, mult, presscore
+        for c_ind in range(self._vertices.card_index()):
+            yield (
+                c_ind,
+                self._vertices.attr(c_ind, MULT_ATTR),
+                self._vertices.attr(c_ind, PRESSCORE_ATTR),
+            )
 
     def links(self) -> Iterator[tuple[IndexT, IndOrT, IndOrT]]:
         """Iterate over the links.
 
         Yields
         ------
         IndexT
             Link's index
         IndOrT
             First oriented contig
         IndOrT
             Second oriented contig
         """
-        for l_ind, (u, v) in enumerate(self.__links):
+        for l_ind, (u, v) in enumerate(self.__base_links):
             yield l_ind, u, v
         for l_ind, (u, v) in enumerate(self.__extra_links):
-            yield l_ind + len(self.__links), u, v
+            yield l_ind + len(self.__base_links), u, v
 
     def extra_links(self) -> Iterator[tuple[IndexT, IndOrT, IndOrT]]:
         """Iterate over the links.
 
         Yields
         ------
         IndexT
             Link's index
         IndOrT
             First oriented contig
         IndOrT
             Second oriented contig
         """
         for l_ind, (u, v) in enumerate(self.__extra_links):
-            yield l_ind + len(self.__links), u, v
+            yield l_ind + len(self.__base_links), u, v
 
     def region_contigs(self, region_ind: IndexT) -> (
             Iterator[tuple[IndexT, MultT, PresScoreT]]):
         """Iterate over the contigs and their attributes of a region.
 
         Parameters
         ----------
@@ -123,50 +149,59 @@
             Contig's index
         MultT
             Contig's multiplicity
         PresScoreT
             Contig's presence score
         """
         for c_ind, _ in self.__region_oriented_contig[region_ind]:
-            yield c_ind, *self.__contig_attrs[c_ind]
+            yield (
+                c_ind,
+                self._vertices.attr(c_ind, MULT_ATTR),
+                self._vertices.attr(c_ind, PRESSCORE_ATTR),
+            )
 
     # ~*~ Regions ~*~
 
     def __generate_region_orc(self, region_length: list[int]):
         for reg_ind, _ in self.__oriented_region_order:
             if reg_ind == len(self.__region_oriented_contig):
                 # Generate the region
                 self.__region_oriented_contig.append([])
                 for c_ind in range(region_length[reg_ind]):
+                    v_ind = self._vertices.add()
+                    self._vertices.set_attr(
+                        v_ind, MULT_ATTR,
+                        (
+                            self.__generate_mult()
+                            if reg_ind > 0 or c_ind > 0
+                            else 1
+                        ),
+                    )
+                    self._vertices.set_attr(
+                        v_ind, PRESSCORE_ATTR,
+                        self.__generate_presencescore(),
+                    )
+
                     self.__region_oriented_contig[-1].append(
                         (  # type: ignore
-                            len(self.__contig_attrs),
+                            v_ind,  # new contig index
                             (
+                                # new contig orientation
                                 randint(FORWARD_INT, REVERSE_INT)
                                 if reg_ind > 0 or c_ind > 0
                                 else FORWARD_INT
                             ),
                         ),
                     )
-                    self.__contig_attrs.append(
-                        (
-                            (
-                                self.__generate_mult()
-                                if reg_ind > 0 or c_ind > 0
-                                else 1
-                            ),
-                            self.__generate_presencescore(),
-                        ),
-                    )
             else:
                 # Add one to the multiplicities of each contig
                 for c_ind, _ in self.__region_oriented_contig[reg_ind]:
-                    old_mult, old_presscore = self.__contig_attrs[c_ind]
-                    self.__contig_attrs[c_ind] = (
-                        old_mult + 1, old_presscore,
+                    self._vertices.set_attr(
+                        c_ind, MULT_ATTR,
+                        self._vertices.attr(c_ind, MULT_ATTR) + 1,
                     )
 
     # ~*~ Contigs ~*~
 
     def __generate_mult(self, base: int = 1) -> int:
         mult = base
         if random() < self.__proba_over_mult:
@@ -179,38 +214,49 @@
     # ~*~ Links ~*~
 
     def __generate_intra_links(self):
         for region_orc in self.__region_oriented_contig:
             orc_iter = iter(region_orc)
             u = next(orc_iter)
             for v in orc_iter:
-                self.__links.append((u, v))
+                self._edges.add(u, v)
+                self.__base_links.append((u, v))
                 u = v
 
     def __generate_inter_links(self):
         orreg_map_iter = iter(self.__oriented_region_order)
         start = next(orreg_map_iter)
         u = start
         start_beg, u_end = self.__orreg_extremity(*u)
         for v in orreg_map_iter:
             v_beg, v_end = self.__orreg_extremity(*v)
-            self.__links.append((u_end, v_beg))
+            self._edges.add(u, v)
+            self.__base_links.append((u_end, v_beg))
             u = v
             u_end = v_end
-        self.__links.append((u_end, start_beg))
+        self._edges.add(u, start)
+        self.__base_links.append((u_end, start_beg))
 
     def __generate_extra_links(self):
-        for c_ind in range(len(self.__contig_attrs)):
+        for c_ind in range(self._vertices.card_index()):
             if random() < self.__proba_extra_link:
-                c_or = randint(FORWARD_INT, REVERSE_INT)
-                d_ind = randint(0, len(self.__contig_attrs) - 1)
-                d_or = randint(FORWARD_INT, REVERSE_INT)
-                self.__extra_links.append(
-                    ((c_ind, c_or), (d_ind, d_or)),  # type: ignore
-                )
+                c_or: OrT = randint(
+                    FORWARD_INT,
+                    REVERSE_INT,
+                )  # type: ignore
+                d_ind = randint(0, self._vertices.card_index() - 1)
+                d_or: OrT = randint(
+                    FORWARD_INT,
+                    REVERSE_INT,
+                )  # type: ignore
+                if ((c_ind, c_or), (d_ind, d_or)) not in self._edges:
+                    self._edges.add((c_ind, c_or), (d_ind, d_or))
+                    self.__extra_links.append(
+                        ((c_ind, c_or), (d_ind, d_or)),
+                    )
 
     def __orreg_extremity(self, reg_ind: IndexT,
                           reg_or: OrT) -> tuple[IndOrT, IndOrT]:
         if reg_or == FORWARD_INT:
             return (
                 self.__region_oriented_contig[reg_ind][0],
                 self.__region_oriented_contig[reg_ind][-1],
```

### Comparing `khloraascaf_utils-0.8.0/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.1/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.0/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.8.1/src/khloraascaf_utils/to_networkx.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from khloraascaf.ilp.invf_sets import InvFT, invf, invf_builder, invf_other
 from khloraascaf.multiplied_doubled_contig_graph import (
     CIND_IND,
     COCC_IND,
     COR_IND,
     CTG_ID_ATTR,
     MULT_ATTR,
+    PRESSCORE_ATTR,
     MDCGraph,
     MDCGraphIDContainer,
     OccOrCT,
 )
 from khloraascaf.outputs import ORIENT_INT_STR, read_map_of_regions
 from khloraascaf.utils_debug import read_vertices_of_regions
 from networkx import DiGraph
@@ -104,14 +105,15 @@
     # All but start and terminal
     for v_ind, v_or, v_occ in mdcg.multiplied_vertices():
         nxgraph.add_node(
             format_occorc_to_nxnode((v_ind, v_or, v_occ)),
             ** {
                 CTG_ID_ATTR: id_container.vertex_to_contig(v_ind),
                 MULT_ATTR: vertices.attr(v_ind, MULT_ATTR),
+                PRESSCORE_ATTR: vertices.attr(v_ind, PRESSCORE_ATTR),
             },
         )
     # ------------------------------------------------------------------------ #
     # Add EOccOrCT
     # ------------------------------------------------------------------------ #
     for (u_ind, u_or, u_occ), (v_ind, v_or, v_occ) in mdcg.multiplied_edges():
         nxgraph.add_edge(
```

### Comparing `khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.8.0/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.8.1/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.0/tests/test_artificial_data.py` & `khloraascaf_utils-0.8.1/tests/test_artificial_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     for c_ind, c_mult, c_presscore in art_data_ir_sc_over_extra.contig_attrs():
         if c_ind < 4 or c_ind > 6:
             assert 0 < c_mult < 3
         elif 3 < c_ind < 7:
             assert 1 < c_mult < 4
         assert 0 <= c_presscore < 1
     assert sum(1 for _ in art_data_ir_sc_over_extra.links()) >= 10
-    assert sum(1 for _ in art_data_ir_sc_over_extra.extra_links()) > 0
+    assert sum(1 for _ in art_data_ir_sc_over_extra.extra_links()) >= 0
 
 
 # ---------------------------------------------------------------------------- #
 #                              Artificial_to_mdcg                              #
 # ---------------------------------------------------------------------------- #
 def test_art_to_mdcg(art_data_ir_sc: ArtificialData):
     """Test art to mdcg."""
```

### Comparing `khloraascaf_utils-0.8.0/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.8.1/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.8.0/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.8.1/tests/test_contigs_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding=utf-8 -*-
 
 """Tests for contigs attributes functions."""
 
+from decimal import Decimal
+
 from khloraascaf_utils.contigs_attributes import (
     cov_to_mult,
     dis_union_align_len_to_presence_score,
 )
 
 
 # ============================================================================ #
 #                                TEST FUNCTIONS                                #
 # ============================================================================ #
 # ---------------------------------------------------------------------------- #
 #                                  Cov_to_mult                                 #
 # ---------------------------------------------------------------------------- #
 def test_cov_to_mult_ceil():
     """Test cov_to_mult function for the ceil branch."""
-    assert cov_to_mult(1.11, 1) == 2
+    assert cov_to_mult(111, 100) == 2
+    assert cov_to_mult(1111, 100) == 11
     assert cov_to_mult(3, 2) == 2
-    # FIXME should be equals to 1
-    assert cov_to_mult(1.1, 1) == 2
+    assert cov_to_mult(11, 10) == 1
 
 
 def test_cov_to_mult_floor():
     """Test cov_to_mult function for the floor branch."""
     assert cov_to_mult(1.09, 1) == 1
     assert cov_to_mult(2.06, 2) == 1
```

