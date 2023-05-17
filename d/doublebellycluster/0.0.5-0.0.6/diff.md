# Comparing `tmp/doublebellycluster-0.0.5.tar.gz` & `tmp/doublebellycluster-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doublebellycluster-0.0.5.tar", last modified: Sat Apr  1 20:45:34 2023, max compression
+gzip compressed data, was "doublebellycluster-0.0.6.tar", last modified: Wed May 17 07:54:41 2023, max compression
```

## Comparing `doublebellycluster-0.0.5.tar` & `doublebellycluster-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 20:45:34.672945 doublebellycluster-0.0.5/
--rw-rw-rw-   0        0        0    35821 2023-03-25 19:50:31.000000 doublebellycluster-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2457 2023-04-01 20:45:34.672945 doublebellycluster-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-04-01 20:45:27.000000 doublebellycluster-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-01 20:45:34.661948 doublebellycluster-0.0.5/doublebellycluster/
--rw-rw-rw-   0        0        0      113 2023-04-01 20:43:34.000000 doublebellycluster-0.0.5/doublebellycluster/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-03-25 20:03:34.000000 doublebellycluster-0.0.5/doublebellycluster/clustering-pavlov.py
--rw-rw-rw-   0        0        0      869 2023-03-25 19:50:31.000000 doublebellycluster-0.0.5/doublebellycluster/clustering_some.py
--rw-rw-rw-   0        0        0     2402 2023-04-01 11:24:37.000000 doublebellycluster-0.0.5/doublebellycluster/data_proportion.py
--rw-rw-rw-   0        0        0    10098 2023-04-01 20:36:44.000000 doublebellycluster-0.0.5/doublebellycluster/doublebellycluster.py
--rw-rw-rw-   0        0        0     1105 2023-04-01 20:27:31.000000 doublebellycluster-0.0.5/doublebellycluster/inter_dist.py
--rw-rw-rw-   0        0        0     1375 2023-04-01 19:22:20.000000 doublebellycluster-0.0.5/doublebellycluster/plots.py
--rw-rw-rw-   0        0        0      971 2023-04-01 12:59:12.000000 doublebellycluster-0.0.5/doublebellycluster/seq_match.py
-drwxrwxrwx   0        0        0        0 2023-04-01 20:45:34.668960 doublebellycluster-0.0.5/doublebellycluster.egg-info/
--rw-rw-rw-   0        0        0     2457 2023-04-01 20:45:34.000000 doublebellycluster-0.0.5/doublebellycluster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-04-01 20:45:34.000000 doublebellycluster-0.0.5/doublebellycluster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 20:45:34.000000 doublebellycluster-0.0.5/doublebellycluster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-01 20:45:34.000000 doublebellycluster-0.0.5/doublebellycluster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-01 20:45:34.000000 doublebellycluster-0.0.5/doublebellycluster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 20:45:34.672945 doublebellycluster-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-04-01 20:36:40.000000 doublebellycluster-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 20:45:34.670946 doublebellycluster-0.0.5/tests/
--rw-rw-rw-   0        0        0       74 2023-03-20 12:13:28.000000 doublebellycluster-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     8523 2023-03-20 12:13:28.000000 doublebellycluster-0.0.5/tests/yadisk_test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:54:41.958291 doublebellycluster-0.0.6/
+-rw-rw-rw-   0        0        0    35821 2023-03-25 19:50:31.000000 doublebellycluster-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2662 2023-05-17 07:54:41.957292 doublebellycluster-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1631 2023-05-16 12:40:24.000000 doublebellycluster-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 07:54:41.948294 doublebellycluster-0.0.6/doublebellycluster/
+-rw-rw-rw-   0        0        0        0 2023-05-16 18:44:07.000000 doublebellycluster-0.0.6/doublebellycluster/0_tes.py
+-rw-rw-rw-   0        0        0      153 2023-04-22 20:33:16.000000 doublebellycluster-0.0.6/doublebellycluster/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-03-25 20:03:34.000000 doublebellycluster-0.0.6/doublebellycluster/clustering-pavlov.py
+-rw-rw-rw-   0        0        0      869 2023-03-25 19:50:31.000000 doublebellycluster-0.0.6/doublebellycluster/clustering_some.py
+-rw-rw-rw-   0        0        0     2556 2023-05-15 21:34:54.000000 doublebellycluster-0.0.6/doublebellycluster/data_proportion.py
+-rw-rw-rw-   0        0        0    11548 2023-05-17 07:54:34.000000 doublebellycluster-0.0.6/doublebellycluster/doublebellycluster.py
+-rw-rw-rw-   0        0        0     1112 2023-05-14 21:34:48.000000 doublebellycluster-0.0.6/doublebellycluster/inter_dist.py
+-rw-rw-rw-   0        0        0     1253 2023-05-15 21:13:01.000000 doublebellycluster-0.0.6/doublebellycluster/plots.py
+-rw-rw-rw-   0        0        0      971 2023-04-01 12:59:12.000000 doublebellycluster-0.0.6/doublebellycluster/seq_match.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:54:41.954293 doublebellycluster-0.0.6/doublebellycluster.egg-info/
+-rw-rw-rw-   0        0        0     2662 2023-05-17 07:54:41.000000 doublebellycluster-0.0.6/doublebellycluster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-17 07:54:41.000000 doublebellycluster-0.0.6/doublebellycluster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:54:41.000000 doublebellycluster-0.0.6/doublebellycluster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-17 07:54:41.000000 doublebellycluster-0.0.6/doublebellycluster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 07:54:41.000000 doublebellycluster-0.0.6/doublebellycluster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:54:41.959292 doublebellycluster-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-15 13:36:51.000000 doublebellycluster-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:54:41.956294 doublebellycluster-0.0.6/tests/
+-rw-rw-rw-   0        0        0       74 2023-03-20 12:13:28.000000 doublebellycluster-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     8523 2023-03-20 12:13:28.000000 doublebellycluster-0.0.6/tests/yadisk_test.py
```

### Comparing `doublebellycluster-0.0.5/LICENSE` & `doublebellycluster-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doublebellycluster-0.0.5/PKG-INFO` & `doublebellycluster-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: doublebellycluster
-Version: 0.0.5
+Version: 0.0.6
 Summary: Библиотека кластеризации на анализе плотности
 Home-page: UNKNOWN
 Author: George Pavlov
 Author-email: pavlovgeorgem@yandex.ru
 License: LGPLv3
-Keywords: clustering intra_distance clustering-share-devide
+Keywords: clustering intra_distance clustering-share-devide sequence-matching
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -43,30 +43,35 @@
 Примеры
 *******
 
 .. code:: python
 
     import doublebellycluster
 
-    # J lkkkkkkk класс
+    # Главный класс
     doubleclustering = doublebellycluster.Doubleclustering()
     # запустить кластеризацию на данных xy
     # данные должны быть непрерывными
-    doubleclustering.do_continious( xy, show_plots = True,
-                          calc_aggregate_all= False,
-                          percentile_cut = 10)
 
+    xy['col'] = doubleclustering.do_continis( xy[['xx', 'yy']],
+                        calc_aggregate_all= True,
+                        percentile_cut = 10)
+    doubleclustering.d3_color_map(folder='C:/Users/User/Desktop',show_save = False)
+
+    doubleclustering.show_fi_plot_(folder='C:/Users/User/Desktop',show_save = False)
     
+
     # Есть еще функции
 
     # Сравнивает две последовательности
     doublebellycluster.seq_match(a, b)
 
     # найти расстояние между кластерами
-    doubleclustering.get_inter_dist(df,col)
+    doublebellycluster.get_inter_dist(df,col)
+
 
 
 
 
 История изменений
 *****************
 
@@ -76,7 +81,9 @@
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Если гео данные - то их нужно подготавливать :code:`import pyproj` 
   * Исправлено :code:`AttributeError` при вызове :code:`ResourceLinkObject.public_listdir()`
 
 
+
+
```

### Comparing `doublebellycluster-0.0.5/README.rst` & `doublebellycluster-0.0.6/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 Примеры
 *******
 
 .. code:: python
 
     import doublebellycluster
 
-    # J lkkkkkkk класс
+    # Главный класс
     doubleclustering = doublebellycluster.Doubleclustering()
     # запустить кластеризацию на данных xy
     # данные должны быть непрерывными
-    doubleclustering.do_continious( xy, show_plots = True,
-                          calc_aggregate_all= False,
-                          percentile_cut = 10)
 
+    xy['col'] = doubleclustering.do_continis( xy[['xx', 'yy']],
+                        calc_aggregate_all= True,
+                        percentile_cut = 10)
+    doubleclustering.d3_color_map(folder='C:/Users/User/Desktop',show_save = False)
+
+    doubleclustering.show_fi_plot_(folder='C:/Users/User/Desktop',show_save = False)
     
+
     # Есть еще функции
 
     # Сравнивает две последовательности
     doublebellycluster.seq_match(a, b)
 
     # найти расстояние между кластерами
-    doubleclustering.get_inter_dist(df,col)
+    doublebellycluster.get_inter_dist(df,col)
+
 
 
 
 
 История изменений
 *****************
 
@@ -52,7 +57,9 @@
 
   * Пока работает только на непрерывных данных
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Если гео данные - то их нужно подготавливать :code:`import pyproj` 
   * Исправлено :code:`AttributeError` при вызове :code:`ResourceLinkObject.public_listdir()`
+
+
```

### Comparing `doublebellycluster-0.0.5/doublebellycluster/clustering-pavlov.py` & `doublebellycluster-0.0.6/doublebellycluster/clustering-pavlov.py`

 * *Files identical despite different names*

### Comparing `doublebellycluster-0.0.5/doublebellycluster/clustering_some.py` & `doublebellycluster-0.0.6/doublebellycluster/clustering_some.py`

 * *Files identical despite different names*

### Comparing `doublebellycluster-0.0.5/doublebellycluster/doublebellycluster.py` & `doublebellycluster-0.0.6/doublebellycluster/doublebellycluster.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,322 +1,367 @@
 
 import copy
-from functools import reduce
-
-
 import numpy as np
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 import scipy.stats as st
 from sklearn.cluster import DBSCAN
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.metrics.pairwise import pairwise_distances
-
+ 
 import itertools
 
 from .inter_dist import get_inter_dist
 from .plots import plot_color_map, d3_color_map
 
+import os
+import warnings
 
+warnings.filterwarnings("ignore")
 
 
 class Doubleclustering:
 
-    def __init__(self):
+    def __init__(self, showing_all = False):
         self.working = True
+        self.eps = 0.015
+        self.showing_all = showing_all
+        dir = os.getcwd()
+        print(dir)
+        if 'pic' not in os.listdir(dir):
+            os.makedirs(os.path.join(dir,'pic'))
 
+        self.dir = os.path.join(dir,'pic')
 
-    def d3plot(self, xy, n, show_save = True):
 
+    def d3plot(self, xy):
 
-        xy['x'] = xy['xx'].to_list()
-        xy['y'] = xy['yy'].to_list()
 
-        xy[['x','y']] -= xy[['x','y']].min()
-        xy[['x','y']] /= xy[['x','y']].max()
+        D = xy.shape[1]
 
-        # getting xy
-        self.xy = xy
+        self.D = D
 
-        xx, yy = np.mgrid[0:1:n*100j, 0:1:n*100j]
-        positions = np.vstack([xx.ravel(), yy.ravel()])
-        values = np.vstack([xy.x, xy.y])
-        kernel = st.gaussian_kde(values)
-        f = np.reshape(kernel(positions).T, xx.shape)
-        f = f / f.max() * 100
+        if D==3:
+            self.eps = 0.05
+    
+        xy.columns=list(range(D))
 
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection="3d")
-        ax.plot_surface(xx, yy, f, cmap="Blues", lw=0.5, rstride=1, cstride=1)
-        ax.view_init(elev=80., azim=-90)
-        ax.contour(xx, yy, f, 10, colors="k", linestyles="solid")
+        for i in xy.columns:
+            xy[i] = xy[i].to_list()
         
-        if show_save:
-            plt.show()
-        else:
-            fig.savefig('C:/Users/User/Desktop/3d_plot.png')
+        xy -= xy.min()
+        xy /= xy.max()
 
-        self.f = f
+        # getting xy
+        self.xy = xy
 
+        n100 = min(10**(5/D),100)
+        
+        n_bins =  n100*np.ones(D)
+        bounds = np.repeat([(0,1)], D, axis = 0)
 
-    def do_fs_beer(self):
+        result = np.mgrid[[slice(row[0], row[1], n*1j) for row, n in zip(bounds, n_bins)]]
 
-        xy = self.xy
+        positions = np.vstack([i.ravel() for i in result])
+        values = np.vstack([xy[i] for i in xy.columns])
+        kernel = st.gaussian_kde(values)
+        print(result[0].shape)
+        f = kernel(positions).T
         
-        fs = [[[k, v, j] for v, j in enumerate(i)]
-            for k, i in enumerate(self.f)]
-        fs = [i for i in fs if len(i) > 0]
-        fs = reduce(lambda x, y: x + y, fs)
-        fs = pd.DataFrame(fs, columns=['x', 'y','f'])
+        def make_profii(k):
+            a=[]
+            num_dan = np.arange(0,D)[::-1]
+            for j in num_dan:
+                a += [k//(n100**j)]
+                k =k%(n100**j)
+            return a
+
+        fs = [make_profii(k)+[i] for k, i in enumerate(f)]
+        fs = pd.DataFrame(fs, columns=list(range(D))+['f'])
         fs = fs.sort_values('f',ascending=False)
-        fs['l']=-1
-        fs['l1']=-1
-        fs[['x', 'y']]/=100
 
-        Knn = KNeighborsClassifier(n_neighbors=1)
-        Knn.fit(xy[['x','y']], xy.index)
-        fs[['xx','yy']] = np.array(xy.loc[Knn.predict(fs[['x','y']]),['xx','yy']])
-        fs.index = range(fs.shape[0])
-
-        Knn = KNeighborsClassifier(n_neighbors=1)
-        Knn.fit(fs[['x','y']], fs.index)
-        lobl = Knn.predict(xy[['x','y']])
+        fs[list(range(D))] /=n100
+        
+        Knn = KNeighborsClassifier(n_neighbors=10)
+        Knn.fit(fs[range(D)], fs.index)
+        lobl = Knn.predict(xy)
         unique, counts = np.unique(lobl, return_counts=True)
 
         fs['len'] = fs.index.map(dict(zip(unique, counts)))
 
+        fs = fs.dropna()
+
+        fs.f -= fs.f.min()
+        fs.f /= fs.f.max()
+        fs.f *= 100
+
+        self.fs = fs
+
+        
+    def do_fs_beer(self):
+
+        fs = self.fs
 
-        d_mat = pd.DataFrame(pairwise_distances(fs[['xx','yy']]))
-        for i in range(d_mat.shape[0]):
-            d_mat.iloc[i, i] = np.nan
+        d_mat =pairwise_distances(fs[list(range(self.D))])
+
+        eps = fs[range(self.D)].std(0).diff().min()*2
+        print(eps)
 
         c = 100
         height = 5
-        dbs = DBSCAN(eps= 0.015, min_samples=1)
-
+        dbs = DBSCAN(eps= self.eps, min_samples=1)
+        fs['l']=-1
+        fs['l1']=-1
         while c > 5:
 
             fs1 = fs.loc[fs.f > c - height]
-            dbs = dbs.fit(fs1[['x', 'y']])
+            dbs = dbs.fit(fs1[range(self.D)])
             fs.loc[fs1.index,'l'] = dbs.labels_
 
             a_get0 = fs.loc[fs1.index].groupby('l')['l1'].unique().reset_index()
             a_get0['l1'] = a_get0['l1'].map(lambda x: list(x))
             a_get0['1']=a_get0['l1'].map(lambda x: len([i for i in x if i!=-1 ]))
             a_get0 = list(itertools.chain(*a_get0.loc[a_get0['1'] >= 2, 'l1'].to_list()))
             a_get0 = [i for i in a_get0 if i != -1]
             a_get1 = fs.loc[fs1.index].groupby('l1')['l'].count()
             a_get1 = fs.loc[fs1.index].groupby('l1').apply(lambda x: pd.Series({
-                'len': x['len'].sum(),
-                'mind '+str(c): d_mat.loc[x.index, x.index].min().max() + 2 * d_mat.loc[x.index, x.index].min().std()
+                'len': x['len'].sum()
+                # ,'mind '+str(c): d_mat.loc[x.index, x.index].min().max() + 2 * d_mat.loc[x.index, x.index].min().std()
             }))
 
             a_get1 = a_get1.loc[a_get1['len']>50]
             a_get1 = a_get1.drop('len', axis=1)
             a_get1 = a_get1.loc[a_get1.index.isin(a_get0)]
 
             if len(a_get1) > 0:
                 fs = fs.merge(a_get1, on = ['l1'], how = 'left')
                 fs['col '+ str(c)] = np.nan
                 fs.loc[fs['l1'].isin(a_get1.index),  'col ' + str(c)] = fs.loc[fs['l1'].isin(a_get1.index),'l1']
 
             fs['l1'] = copy.deepcopy(fs['l'])
             c -= height
 
+        fs = fs.drop(['l','l1'],axis=1)
+
         self.fs = fs
 
 
 
+
     def fs_regress_allneed(self):
 
         fs = self.fs
 
-        d_framedata = fs.iloc[:,7:]
+        d_framedata = fs.iloc[:,self.D + 2:]
         col = d_framedata.columns
         d_framedata = d_framedata[[i for i in col if 'col' in i]]
         for i in range(0,d_framedata.shape[1]-1):
             re = list(d_framedata.iloc[:,i].dropna().index)
 
             for jj in range(i+1,d_framedata.shape[1]):
 
                 a_var_step1 = list(d_framedata.iloc[re,jj].unique())
                 promejutoc_var = d_framedata.iloc[:, jj]
                 promejutoc_var[promejutoc_var.isin(a_var_step1)]=np.nan
                 d_framedata.iloc[:, jj] = promejutoc_var
 
-
         col = d_framedata.columns
         def get_h_done(x):
             x_k = np.where(x >= 0)[0]
             if len(x_k)>0:
                 k = min(list(x_k))
                 res = [int(col[k].split(' ')[1]), x[k]]
             else:
                 res = [np.nan]*2
             return res
+        
 
-        det_matrix = pd.DataFrame( np.array( d_framedata.apply(lambda x: get_h_done(x), axis =1).to_list()))
+        det_matrix = pd.DataFrame( np.array( d_framedata.apply(lambda x: get_h_done(x), axis =1).to_list()),
+                                  columns = ['level','cl'])
+        
         fs = fs.join(det_matrix)
         fs['fin_join'] = det_matrix.astype(str).apply(lambda x: '-'.join(x), axis =1)
-        fs = fs.sort_values([0,1])
-
+        fs = fs.sort_values(['level','cl'])
         fs_to_plot = fs.loc[fs['fin_join']!='nan-nan']
 
         self.fs = fs
         self.fs_to_plot = fs_to_plot
 
         
 
     def do_color_cluster(self):
 
         fs_to_plot = self.fs_to_plot
 
-        dist_mat_lil = get_inter_dist(fs_to_plot,'fin_join')
-        fs_resullt = fs_to_plot.groupby([0,'fin_join'])['len'].sum().reset_index()
-
-        print(dist_mat_lil)
-        print(fs_resullt)
+        dist_mat_lil = get_inter_dist(fs_to_plot[list(range(self.D))+['fin_join']],'fin_join')
+        fs_resullt = fs_to_plot.groupby(['level','fin_join'])['len'].sum().reset_index()
 
-        num_dic={i:k for k,i in enumerate(fs_to_plot[0].unique())}
+        num_dic={i:k for k,i in enumerate(fs_to_plot['level'].unique())}
 
         dd= {}
         for i in range(len(fs_resullt)):
 
             dd_dicccy=list(dd.keys()) + list(dd.values())
             read_file = fs_resullt.loc[i,]
             idx = pd.IndexSlice
             d_ma = dist_mat_lil.loc[idx[:, read_file['fin_join']],:].dropna(1)
             d_ma = d_ma.sort_values(d_ma.index[0], axis =1).iloc[:,:4]
-            print(d_ma)
             from_ = [i[1] for i in d_ma.columns if i[0]==read_file[0]]
             d_ma = d_ma.loc[:, idx[:,from_]]
-            print(d_ma)
             
             if d_ma.shape[1]:
                 ind = d_ma.columns[0][1]
-                print(True)
             else:
                 ind = read_file['fin_join'] 
 
             if read_file['fin_join'] not in dd_dicccy:
                 dd[read_file['fin_join']] = ind
 
         
         for i in dd_dicccy:
             if i not in dd.keys():
                 dd[i] = i
 
-        print(dd)
-
 
         fs_to_plot['fin_join'] = fs_to_plot['fin_join'].map(dd)   ##
-        
         self.fs_to_plot = fs_to_plot
 
 
-    def do_model_clusterspare(self):
 
-        fs_to_plot = self.fs_to_plot
+    def do_model_clusterspare(self, percentile_cut):
 
+        fs_to_plot = self.fs_to_plot
         fs = self.fs
-        
-        fs = fs.drop(['fin_join'],axis=1).merge(fs_to_plot[['x','y','fin_join']], on = ['x','y'], how = 'left')
-        llist = list(fs.loc[fs['fin_join'].isna()==False,0].unique()[::-1]) +[0.]
-        fs[0] = fs['f'].map(lambda x: max([i for i in llist if i<= int(x)]))
+
+        fs = fs.drop(['fin_join'],axis=1).merge(fs_to_plot[list(range(self.D))+['fin_join']], on = list(range(self.D)), how = 'left')
+        llist = list(fs.loc[fs['fin_join'].isna()==False,'level'].unique()[::-1]) +[0.]
+        fs['level'] = fs['f'].map(lambda x: max([i for i in llist if i<= int(x)]))
         for i in llist:
-            x = fs.loc[(fs[0]>=i)&(fs['fin_join'].isna()==False)]
+            x = fs.loc[(fs['level']>=i)&(fs['fin_join'].isna()==False)]
             Knn = KNeighborsClassifier(n_neighbors=2)
-            Knn.fit(x[['xx','yy']], x['fin_join'])
+            Knn.fit(x[list(range(self.D))], x['fin_join'])
             print(i)
-            if len(fs.loc[(fs[0]>=i)&(fs['fin_join'].isna()), 'fin_join']):
-                fs.loc[(fs[0]>=i)&(fs['fin_join'].isna()), 'fin_join'] = Knn.predict(fs.loc[(fs[0]>=i)&(fs['fin_join'].isna()), ['xx','yy']])
+            if len(fs.loc[(fs['level']>=i)&(fs['fin_join'].isna()), 'fin_join']):
+                fs.loc[(fs['level']>=i)&(fs['fin_join'].isna()), 'fin_join'] = Knn.predict(fs.loc[(fs['level']>=i)&(fs['fin_join'].isna()), list(range(self.D))])
+
+        fs['col'] = fs['fin_join'].map({i:k+1 for k,i in enumerate(fs['fin_join'].unique())})
 
         self.fs = fs
+        self.fs_to_plot = fs.loc[fs['level']>=percentile_cut]
 
 
     def end(self):
 
         fs_to_plot = self.fs_to_plot
-
         xy = self.xy
            
         Knn = KNeighborsClassifier(n_neighbors=10)
-        Knn.fit(fs_to_plot[['xx','yy']], fs_to_plot['fin_join'])
-        xy[ 'fin_join'] = Knn.predict(xy[['xx','yy']])
+        Knn.fit(fs_to_plot[list(range(self.D))], fs_to_plot['fin_join'])
+        xy[ 'fin_join'] = Knn.predict(xy[list(range(self.D))])
+        xy['col'] = xy['fin_join'].map({i:k+1 for k,i in enumerate(xy['fin_join'].unique())})
 
         self.xy = xy
 
 
-    def do_continious(self, xy, show_plots = True,
+    def do_continis(self, xy,
                       calc_aggregate_all= False,
                       percentile_cut = 10):
 
-        if xy.shape[1] == 2:
+        if xy.isna().sum().sum()==0:
             pass
         else:
-            raise ValueError('A very specific bad thing happened.')
+            raise ValueError('Nan is presutstvoble')
+
+        if xy.shape[1]>1 and xy.shape[1]<4 :
+            pass
+        else:
+            raise ValueError('Non number of variables')
+        
+        if xy.dtypes.astype(str).map(lambda x: 'int' in x or 'float' in x).all():
+            pass
+        else:
+            raise ValueError('Non doooable types.')
 
         if percentile_cut >= 0 and percentile_cut <= 100:
             pass
         else:
-            raise ValueError('A very specific bad thing happened.')
+            raise ValueError('Bad percentile cut')
 
-        self.d3plot(xy, 1, show_save = False)
+        self.d3plot(xy)
         self.do_fs_beer()
         self.fs_regress_allneed()
-        plot_color_map(self.fs_to_plot[['x','y','fin_join']],
-                       'first_exampl', show_save = False)
+
+        if self.showing_all: plot_color_map(self.fs_to_plot[[0,1,'fin_join']],
+                       self.dir + '/first_exampl', show_save = False)
 
         if calc_aggregate_all:
             self.do_color_cluster()
             # aggregate clusters all
-            plot_color_map(self.fs_to_plot[['x','y','fin_join']],
-                       'second_exampl', show_save = False)
+            if self.showing_all: plot_color_map(self.fs_to_plot[[0, 1 ,'fin_join']],
+                       self.dir + '/second_exampl', show_save = False)
 
                 
-        self.do_model_clusterspare()
+        self.do_model_clusterspare(percentile_cut)
 
-        fs = self.fs
-        fs_to_plot = fs.loc[fs[0]>=percentile_cut]
-        self.fs_to_plot = fs_to_plot
-
-        plot_color_map(fs_to_plot[['x','y','fin_join']], 
-                       'third_exampl', show_save = False)
+        if self.showing_all: plot_color_map(self.fs_to_plot[[0, 1 ,'fin_join']], 
+                       self.dir + '/third_exampl', show_save = False)
 
         self.end()
-        
-        plot_color_map(self.xy[['xx','yy','fin_join']], 
-                       'data_exampl', show_save = False)
+
+        return self.xy[ 'col']
         
 
-        d3_color_map(fs, 'd3_color', show_save = True)
+    def d3_color_map(self, folder='', show_save = False):
+        if self.showing_all:
+            folder = self.dir
+        if hasattr(self, 'fs'):
+            return d3_color_map(self.fs, folder + '/d3_color', show_save)
+        else:
+            raise ValueError('Not ccounted yet')
+
+    def show_fi_plot_(self, folder='', show_save = False):
+        if self.showing_all:
+            folder = self.dir
+        if 'fin_join' in self.xy.columns:
+            return plot_color_map(self.xy[[0, 1 ,'fin_join']], 
+                       self.dir + '/data_exampl', show_save)
+        else:
+            raise ValueError('Not ccounted yet')
 
         
 
 if __name__ == '__main__':
     
 
+    showing_all = True
+
     import pyproj
     proj_wgs84 = pyproj.Proj(init="epsg:4326")
     proj_gk4 = pyproj.Proj(init="epsg:20015")
 
 
-    xy = pd.read_csv('C:/Users/User/Desktop/yyy.csv')[['lat','lon']]
-
-    print(xy)
+    xy = pd.read_csv('C:/Users/User/Desktop/accidents.csv').iloc[:1000000]
 
     xy['xx'], xy['yy'] = pyproj.transform(proj_wgs84, proj_gk4, xy['lon'].values,
                                                         xy['lat'].values)
 
+    xy['xy'] = np.sin(xy['xx'])
+
+    xy = xy.loc[xy['Local_Authority_(District)']==12]
+
+    doubleclustering = Doubleclustering(showing_all)
 
-    xy = xy[['xx', 'yy']]
+    doubleclustering.eps = 0.015
 
-    doubleclustering = Doubleclustering()
 
-    doubleclustering.do_continious( xy, show_plots = True,
+    xy['col'] = doubleclustering.do_continis( xy[['xx', 'yy']],
                         calc_aggregate_all= True,
                         percentile_cut = 10)
 
+    doubleclustering.d3_color_map(folder='C:/Users/User/Desktop',show_save = False)
+
+    doubleclustering.show_fi_plot_(folder='C:/Users/User/Desktop',show_save = False)
+
+    print(xy)
+
 
-    doubleclustering.xy[['xx','yy','fin_join']].to_csv('C:/Users/User/Desktop/yyknn_dus.csv')
```

### Comparing `doublebellycluster-0.0.5/doublebellycluster/inter_dist.py` & `doublebellycluster-0.0.6/doublebellycluster/inter_dist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from sklearn.metrics.pairwise import pairwise_distances
 from itertools import permutations
 
 
 def get_inter_dist(df,col):
-    distm = pd.DataFrame(pairwise_distances(df[['xx','yy']]),
+    distm = pd.DataFrame(pairwise_distances(df.drop(col, axis = 1)),
                          index = df.index,
                          columns = df.index)
 
     colu = df[col].unique()
     colu = [list(items) for items in permutations(colu, r=2)]
 
     dist_mat_lil=[]
```

### Comparing `doublebellycluster-0.0.5/doublebellycluster/seq_match.py` & `doublebellycluster-0.0.6/doublebellycluster/seq_match.py`

 * *Files identical despite different names*

### Comparing `doublebellycluster-0.0.5/doublebellycluster.egg-info/PKG-INFO` & `doublebellycluster-0.0.6/doublebellycluster.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: doublebellycluster
-Version: 0.0.5
+Version: 0.0.6
 Summary: Библиотека кластеризации на анализе плотности
 Home-page: UNKNOWN
 Author: George Pavlov
 Author-email: pavlovgeorgem@yandex.ru
 License: LGPLv3
-Keywords: clustering intra_distance clustering-share-devide
+Keywords: clustering intra_distance clustering-share-devide sequence-matching
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -43,30 +43,35 @@
 Примеры
 *******
 
 .. code:: python
 
     import doublebellycluster
 
-    # J lkkkkkkk класс
+    # Главный класс
     doubleclustering = doublebellycluster.Doubleclustering()
     # запустить кластеризацию на данных xy
     # данные должны быть непрерывными
-    doubleclustering.do_continious( xy, show_plots = True,
-                          calc_aggregate_all= False,
-                          percentile_cut = 10)
 
+    xy['col'] = doubleclustering.do_continis( xy[['xx', 'yy']],
+                        calc_aggregate_all= True,
+                        percentile_cut = 10)
+    doubleclustering.d3_color_map(folder='C:/Users/User/Desktop',show_save = False)
+
+    doubleclustering.show_fi_plot_(folder='C:/Users/User/Desktop',show_save = False)
     
+
     # Есть еще функции
 
     # Сравнивает две последовательности
     doublebellycluster.seq_match(a, b)
 
     # найти расстояние между кластерами
-    doubleclustering.get_inter_dist(df,col)
+    doublebellycluster.get_inter_dist(df,col)
+
 
 
 
 
 История изменений
 *****************
 
@@ -76,7 +81,9 @@
 
 * **Release 1.3.1 (2023-02-28)**
 
   * Если гео данные - то их нужно подготавливать :code:`import pyproj` 
   * Исправлено :code:`AttributeError` при вызове :code:`ResourceLinkObject.public_listdir()`
 
 
+
+
```

### Comparing `doublebellycluster-0.0.5/doublebellycluster.egg-info/SOURCES.txt` & `doublebellycluster-0.0.6/doublebellycluster.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.rst
 setup.py
+doublebellycluster/0_tes.py
 doublebellycluster/__init__.py
 doublebellycluster/clustering-pavlov.py
 doublebellycluster/clustering_some.py
 doublebellycluster/data_proportion.py
 doublebellycluster/doublebellycluster.py
 doublebellycluster/inter_dist.py
 doublebellycluster/plots.py
```

### Comparing `doublebellycluster-0.0.5/setup.py` & `doublebellycluster-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,22 @@
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules"]
 
 setup(
     name = "doublebellycluster",
-    version = "0.0.5",
+    version = "0.0.6",
     author = "George Pavlov",
     author_email = "pavlovgeorgem@yandex.ru",
     url = "",
     description='Библиотека кластеризации на анализе плотности',
     long_description=long_description, 
     license="LGPLv3",
     classifiers=classifiers,
-    keywords='clustering intra_distance clustering-share-devide', 
+    keywords='clustering intra_distance clustering-share-devide sequence-matching', 
     packages=find_packages(),
     install_requires=['pandas', 'numpy', 'matplotlib', 'scipy',
     'scikit-learn'],
     
     python_requires='>=3.5'
 )
```

### Comparing `doublebellycluster-0.0.5/tests/yadisk_test.py` & `doublebellycluster-0.0.6/tests/yadisk_test.py`

 * *Files identical despite different names*

