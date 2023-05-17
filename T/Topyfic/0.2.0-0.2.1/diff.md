# Comparing `tmp/Topyfic-0.2.0.tar.gz` & `tmp/Topyfic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.2.0.tar", last modified: Wed Mar 29 18:26:48 2023, max compression
+gzip compressed data, was "Topyfic-0.2.1.tar", last modified: Wed May 17 21:52:29 2023, max compression
```

## Comparing `Topyfic-0.2.0.tar` & `Topyfic-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-03-29 18:26:48.443656 Topyfic-0.2.0/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.2.0/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-03-29 18:26:48.443740 Topyfic-0.2.0/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     2720 2023-02-16 21:19:00.000000 Topyfic-0.2.0/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-03-29 18:26:48.442384 Topyfic-0.2.0/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.2.0/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    38524 2023-02-16 00:05:32.000000 Topyfic-0.2.0/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.2.0/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10863 2023-01-20 10:16:01.000000 Topyfic-0.2.0/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     9008 2023-02-16 20:42:14.000000 Topyfic-0.2.0/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.2.0/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    27547 2023-02-14 00:28:54.000000 Topyfic-0.2.0/Topyfic/utils.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-03-29 18:26:48.443527 Topyfic-0.2.0/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-03-29 18:26:48.000000 Topyfic-0.2.0/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-03-29 18:26:48.000000 Topyfic-0.2.0/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-03-29 18:26:48.000000 Topyfic-0.2.0/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-03-29 18:26:48.000000 Topyfic-0.2.0/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-03-29 18:26:48.000000 Topyfic-0.2.0/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-03-29 18:26:48.444037 Topyfic-0.2.0/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1931 2023-03-29 18:19:12.000000 Topyfic-0.2.0/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.055492 Topyfic-0.2.1/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.2.1/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-05-17 21:52:29.055581 Topyfic-0.2.1/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.2.1/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.054180 Topyfic-0.2.1/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.2.1/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.2.1/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.2.1/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10863 2023-01-20 10:16:01.000000 Topyfic-0.2.1/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    11278 2023-05-01 21:58:44.000000 Topyfic-0.2.1/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.2.1/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    27641 2023-05-17 21:39:51.000000 Topyfic-0.2.1/Topyfic/utils.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.055268 Topyfic-0.2.1/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-17 21:52:29.000000 Topyfic-0.2.1/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-17 21:52:29.055908 Topyfic-0.2.1/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1931 2023-05-17 21:51:55.000000 Topyfic-0.2.1/setup.py
```

### Comparing `Topyfic-0.2.0/LICENSE.txt` & `Topyfic-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.0/PKG-INFO` & `Topyfic-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.0.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.2.0/README.md` & `Topyfic-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 
 ## Tutorials
 
 In general, you need to make three objects (Train, TopModel and Analysis). 
 
 The Train object can be initialized either from (a) single cell RNA-seq dataset or (b) single cell ATAC-seq or (c) bulk RNA-seq.
 
+Training part can be time-consuming depending on how big your data is, however you can learn each train model per random state in different jobs and then combine all together. Look at [this tutorial](tutorials/make_train_object.ipynb) for mor information.
+
 For guidance on using Topyfic to analyze your data look at our more depth-in tutorials:
 
-- [Analysing single cell C2C12 data only using regulatory elements](tutorials/C2C12__TFs_mirhgs_chromreg/C2C12.ipynb): Analysing single cell and single nucleus using C2C12 ENCODE datasets using regulatory elements instead of all genes.
+- [Analysing single cell C2C12 data only using regulatory elements](tutorials/C2C12_TFs_mirhgs_chromreg/C2C12.ipynb): Analysing single cell and single nucleus using C2C12 ENCODE datasets using regulatory elements instead of all genes.
 - [Analysing single cell microglia data](tutorials/microglia_all_genes/microglia.ipynb): Analysing single cell microglia data from [Model-AD portal](https://www.model-ad.org/).
 
+If you are using other methods to learn your topics but you are still interested in doing downstream analysis, you can embeded your results in the format describe [here](tutorials/topic_modeling_model.md). Once you have all your files read you can embed them in suitable format using [this notebook]().
+
 ## Cite
 
 comming soon ...
```

### Comparing `Topyfic-0.2.0/Topyfic/analysis.py` & `Topyfic-0.2.1/Topyfic/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         """
         if self.cell_participation is not None:
             print("cell participation is not empty!")
             print("new cell participation will be replaced!")
 
         lda_output = self.top_model.rLDA.transform(data.X)
         cell_participation = pd.DataFrame(lda_output,
-                                          columns=[f"Topic_{i + 1}" for i in range(self.top_model.N)],#list(self.top_model.topics.keys())
+                                          columns=[f"Topic_{i + 1}" for i in range(self.top_model.N)],
+                                          # list(self.top_model.topics.keys())
                                           index=data.obs.index)
         self.cell_participation = anndata.AnnData(cell_participation, obs=data.obs)
 
     def pie_structure_Chart(self,
                             level,
                             category=None,
                             ascending=None,
@@ -592,14 +593,15 @@
             figsize = (df.shape[0] / 1.5, 5)
 
         fig = plt.figure(figsize=figsize, facecolor='white')
 
         plt.bar(df['index'], df[0], color=color, width=0.5)
 
         plt.xlabel(self.top_model.name)
+        plt.title(f"Distribution of Cell-Topic participation of {self.top_model.name}")
         plt.ylabel("Average cell participation")
 
         if save:
             fig.savefig(f"{file_name}.{file_format}", bbox_inches='tight')
         if show:
             plt.show()
         else:
@@ -684,14 +686,80 @@
         if save:
             fig.savefig(f"{file_name}.{file_format}", bbox_inches='tight')
         if show:
             plt.show()
         else:
             plt.close()
 
+    def cell_participation_distribution(self,
+                                        plot_type="violin",
+                                        threshold=0.05,
+                                        max_topic=True,
+                                        label=None,
+                                        color="blue",
+                                        save=True,
+                                        show=True,
+                                        figsize=None,
+                                        file_format="pdf",
+                                        file_name="dist_cell_participation"):
+        """
+        plot showing distribution of max/all topics in cell participation for each topic
+
+        :param plot_type: type of the plot which can be "violin" or "bax"
+        :type plot_type: str
+        :param threshold: indicate the threshold to filter out cells with low participation in each topics (default: 0.05)
+        :type threshold: float
+        :param max_topic: indicate if you want to consider all topics for each cells (False) or only the topic with highest pariticipation (max topic) for each cells (True)
+        :type max_topic: bool
+        :param label: fill with dictionary contain mapping new name for each topics to name you want to show if you want to change default topic name
+        :type label: dict
+        :param color: color of bar plot (default: blue)
+        :type color: str
+        :param save: indicate if you want to save the plot or not (default: True)
+        :type save: bool
+        :param show: indicate if you want to show the plot or not (default: True)
+        :type show: bool
+        :param figsize: indicate the size of plot (default: (10 * (len(category) + 1), 10))
+        :type figsize: tuple of int
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: piechart_topicAvgCell)
+        :type file_name: str
+        """
+
+        if plot_type != "violin" and plot_type != "box":
+            sys.exit(f"plot_type is not correct! It should be violin or box")
+
+        df = self.cell_participation.to_df().copy(deep=True)
+        if max_topic:
+            max_topic_index = df.values.argmax(1)
+            for i in range(df.shape[1]):
+                index = np.where(max_topic_index == i)[0].tolist()
+                df[df.columns[i]][~df.index.isin(df.index[index])] = np.nan
+        df[df <= threshold] = np.nan
+        if label is not None:
+            df.rename(columns=label, inplace=True)
+        if figsize is None:
+            figsize = (df.shape[1] / 1.5, 5)
+        fig, ax = plt.subplots(figsize=figsize, facecolor='white')
+        if plot_type == "violin":
+            sns.violinplot(data=df, color=color, ax=ax)
+        else:
+            sns.boxplot(data=df, color=color, ax=ax)
+
+        plt.ylabel("cell participation")
+        plt.title(f"Distribution of Cell-Topic participation of {self.top_model.name}")
+
+        if save:
+            plt.savefig(f"{file_name}.{file_format}", bbox_inches='tight')
+        if show:
+            plt.show()
+        else:
+            plt.close()
+
     def plot_topic_composition(self,
                                category,
                                level="topic",
                                biotype="biotype",
                                label=False,
                                save=True,
                                show=True,
@@ -808,14 +876,76 @@
         if save:
             fig.savefig(f"{file_name}.{file_format}")
         if show:
             plt.show()
         else:
             plt.close()
 
+    def max_topic_cell_participation(self,
+                                     cutoff=10,
+                                     color="blue",
+                                     title="Maximum cell topic participation for each cells",
+                                     save=True,
+                                     show=True,
+                                     figsize=None,
+                                     file_format="pdf",
+                                     file_name="max_topic_cell_participation"):
+        """
+        step plot showing maximum cell participation
+
+        :param cutoff: indicate if you want to eliminate any cells with maximum participation less than this
+        :type cutoff: float
+        :param color: color of bar plot (default: blue)
+        :type color: str
+        :param title: indicate if you want to all title into plot (default: Maximum cell topic participation for each cells)
+        :type title: str
+        :param save: indicate if you want to save the plot or not (default: True)
+        :type save: bool
+        :param show: indicate if you want to show the plot or not (default: True)
+        :type show: bool
+        :param figsize: indicate the size of plot (default: (10 * (len(category) + 1), 10))
+        :type figsize: tuple of int
+        :param file_format: indicate the format of plot (default: pdf)
+        :type file_format: str
+        :param file_name: name and path of the plot use for save (default: piechart_topicAvgCell)
+        :type file_name: str
+        """
+        df = self.cell_participation.to_df().copy(deep=True)
+        df = df.apply(np.sort, axis=1)
+
+        max_topic = pd.DataFrame(index=df.index, columns=['Max_topic'])
+        for i in range(max_topic.shape[0]):
+            max_topic.iloc[i, 0] = df[i][-1] * 100
+        max_topic.sort_values(['Max_topic'], ascending=False, inplace=True)
+        max_topic['step'] = 100 * np.divide(range(1, max_topic.shape[0] + 1), max_topic.shape[0])
+        max_topic['Max_topic'] = max_topic['Max_topic'] * -1
+
+        if figsize is None:
+            figsize = (5, 5)
+
+        fig, ax = plt.figure(figsize=figsize, facecolor='white')
+
+        ax.step(max_topic['Max_topic'], max_topic['step'], color=color)
+
+        ax.set_xticks(range(-100, -cutoff + 1, 10))
+        ax.set_xticklabels(range(100, cutoff - 1, -10))
+        ax.set_ylim(0, 110)
+        ax.set_xlim(-100, -cutoff)
+
+        plt.title(title)
+        plt.xlabel('Maximum cell topic participation')
+        plt.ylabel("percentage of cells")
+
+        if save:
+            fig.savefig(f"{file_name}.{file_format}", bbox_inches='tight')
+        if show:
+            plt.show()
+        else:
+            plt.close()
+
     def save_analysis(self, name=None, save_path=""):
         """
         save Analysis class as a pickle file
 
         :param name: name of the pickle file (default: analysis_Analysis.top_model.name)
         :type name: str
         :param save_path: directory you want to use to save pickle file (default is saving near script)
```

### Comparing `Topyfic-0.2.0/Topyfic/main.py` & `Topyfic-0.2.1/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.0/Topyfic/topModel.py` & `Topyfic-0.2.1/Topyfic/topModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.0/Topyfic/topic.py` & `Topyfic-0.2.1/Topyfic/topic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sys
 import warnings
 import joblib
 import pandas as pd
 import numpy as np
+import yaml
+from yaml.loader import SafeLoader
 
 import gseapy as gp
 from gseapy.plot import dotplot
 from gseapy import gseaplot
 from reactome2py import analysis
 
 import matplotlib.pyplot as plt
@@ -196,7 +198,64 @@
                 name = term.split("(GO:")[1][:-1]
                 gseaplot(rank_metric=pre_res.ranking,
                          term=term,
                          **pre_res.results[term],
                          ofname=f"{file_name}_GO_{name}.{file_format}")
 
         return pre_res.res2d
+
+    def gene_weight_variance(self, save=True):
+        """
+        calculate the gene weight variance
+
+        :param save: added as an information to the Topic (default: True)
+        :type save: bool
+
+        :return: Gene weight variance for given topic
+        :rtype: float
+        """
+        variance = self.gene_weights.var().tolist()[0]
+
+        if save:
+            self.topic_information['variance'] = self.gene_weights.var().tolist()[0]
+
+        return print(f"Gene weight variance for given topic is {variance}")
+
+    def write_topic_yaml(self, topic_id=None, model_yaml_path="model.yaml", topic_yaml_path="topic.yaml", save=True):
+        """
+        write topic in YAML format
+
+        :param topic_id: unique topic ID (default is topic ID)
+        :type topic_id: str
+        :param model_yaml_path: model yaml path that has information about the dataset you use
+        :type model_yaml_path: str
+        :param topic_yaml_path: path that you use to save topic
+        :type topic_yaml_path: str
+        :param save: indicate if you want to save yaml file (True) or just show them (Fasle) (default: True)
+        :type save: bool
+        """
+
+        # check require columns
+        cols = self.gene_information.reset_index().columns
+        if not {'gene_name', 'gene_id'}.issubset(cols):
+            sys.exit(f"Gene information doesn't contain gene_name and gene_id columns!")
+
+        # Open the file and load the file
+        with open(model_yaml_path) as f:
+            model_yaml = yaml.load(f, Loader=SafeLoader)
+
+        if topic_id not in model_yaml['Topic IDs']:
+            sys.exit("Topic_id is not in model YAML file!")
+
+        topic_yaml = {'Topic ID': topic_id,
+                      'Gene weights': self.gene_weights.to_dict()[self.id],
+                      'Gene information': self.gene_information.to_dict(),
+                      'Topic information': self.topic_information.T.to_dict()[self.id]}
+
+        if save:
+            file = open(topic_yaml_path, "w")
+            yaml.dump(topic_yaml, file, default_flow_style=False)
+            file.close()
+        else:
+            yaml_string = yaml.dump(topic_yaml)
+            print("The Topic YAML is:")
+            print(yaml_string)
```

### Comparing `Topyfic-0.2.0/Topyfic/train.py` & `Topyfic-0.2.1/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.0/Topyfic/utils.py` & `Topyfic-0.2.1/Topyfic/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         name = '_'.join(name)
 
         top_model = TopModel(name=name,
                              N=n_rtopics,
                              gene_weights=gene_weights,
                              rlda=rlda)
 
-    return top_model, clustering
+    return top_model, clustering, adata
 
 
 def plot_cluster_contribution(clustering,
                               feature,
                               show_all=False,
                               portion=True,
                               save=True,
@@ -651,28 +651,33 @@
             nodePos = nx.spring_layout(g_connected_component)
 
             edge_labels = nx.get_edge_attributes(g_connected_component, "weight")
 
             node_color = nx.get_node_attributes(g_connected_component, "color").values()
             weights = nx.get_edge_attributes(g_connected_component, 'weight').values()
 
+            if len(connected_components) == 1:
+                ax = axs
+            else:
+                ax = axs[int(i / ncols), i % ncols]
+
             nx.draw_networkx(g_connected_component,
                              pos=nodePos,
                              width=list(weights),
                              with_labels=True,
                              node_color=list(node_color),
                              font_size=8,
                              node_size=500,
-                             ax=axs[int(i / ncols), i % ncols])
+                             ax=ax)
 
             nx.draw_networkx_edge_labels(g_connected_component,
                                          nodePos,
                                          edge_labels=edge_labels,
                                          font_size=7,
-                                         ax=axs[int(i / ncols), i % ncols])
+                                         ax=ax)
 
             i += 1
 
         [axi.axis('off') for axi in axs.ravel()]
         plt.tight_layout()
         if save:
             plt.savefig(f"{file_name}.{plot_format}")
```

### Comparing `Topyfic-0.2.0/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.2.1/Topyfic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.0.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.2.0/setup.py` & `Topyfic-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.2.0',  # version number
+    version='v0.2.1',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.0.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
```

