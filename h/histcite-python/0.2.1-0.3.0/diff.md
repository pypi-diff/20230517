# Comparing `tmp/histcite-python-0.2.1.tar.gz` & `tmp/histcite-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.2.1.tar", last modified: Sun May 14 15:19:05 2023, max compression
+gzip compressed data, was "histcite-python-0.3.0.tar", last modified: Wed May 17 06:50:42 2023, max compression
```

## Comparing `histcite-python-0.2.1.tar` & `histcite-python-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 15:18:51.000000 histcite-python-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-14 15:19:05.536476 histcite-python-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-14 15:18:51.000000 histcite-python-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.532476 histcite-python-0.2.1/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:19:05.536476 histcite-python-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-14 15:18:51.000000 histcite-python-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_parse_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:50:42.644319 histcite-python-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 06:50:31.000000 histcite-python-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-05-17 06:50:42.644319 histcite-python-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-17 06:50:31.000000 histcite-python-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:50:42.640319 histcite-python-0.3.0/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-17 06:50:31.000000 histcite-python-0.3.0/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:50:42.640319 histcite-python-0.3.0/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 06:50:42.000000 histcite-python-0.3.0/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:50:42.644319 histcite-python-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 06:50:31.000000 histcite-python-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:50:42.640319 histcite-python-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-17 06:50:31.000000 histcite-python-0.3.0/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-17 06:50:31.000000 histcite-python-0.3.0/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-17 06:50:31.000000 histcite-python-0.3.0/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.2.1/LICENSE` & `histcite-python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.1/PKG-INFO` & `histcite-python-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,16 @@
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
-- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
+- `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -47,24 +48,25 @@
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
-| `CSSCI` | 从CSSCI数据库正常导出即可 |
-> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。不勾选 `Truncate to optimize for Excel`|
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
-| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
@@ -128,19 +130,16 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
-1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
-`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
-
-2、如何去重？  
-`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
-`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
+|  | Web of Science | CSSCI | Scopus|
+| --- | --- | --- | --- |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；</br>否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [ ] 支持 `Scopus` 题录数据
+- [x] 支持 `Scopus` 题录数据
 - [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.2.1/README.md` & `histcite-python-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
-- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
+- `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -24,24 +25,25 @@
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
-| `CSSCI` | 从CSSCI数据库正常导出即可 |
-> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。不勾选 `Truncate to optimize for Excel`|
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
-| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
@@ -105,19 +107,16 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
-1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
-`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
-
-2、如何去重？  
-`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
-`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
+|  | Web of Science | CSSCI | Scopus|
+| --- | --- | --- | --- |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；</br>否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [ ] 支持 `Scopus` 题录数据
+- [x] 支持 `Scopus` 题录数据
 - [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.2.1/histcite/cli.py` & `histcite-python-0.3.0/histcite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from histcite.compute_metrics import ComputeMetrics
 from histcite.process_file import ProcessFile
 from histcite.network_graph import GraphViz
     
 def main():
     parser = argparse.ArgumentParser(description='A Python interface to histcite.')
     parser.add_argument('-f','--folder_path', type=str, required=True, help='folder path of the downloaded files')
-    parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci'], help='source type of the downloaded files')
+    parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci','scopus'], help='source type of the downloaded files')
     parser.add_argument('-n','--node_num', type=int, default=50, help='node number in the citation network graph')
     parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
     # 将结果存放在用户指定的folder_path下的result文件夹中
     output_path = os.path.join(args.folder_path,'result')
     if not os.path.exists(output_path):
```

### Comparing `histcite-python-0.2.1/histcite/compute_metrics.py` & `histcite-python-0.3.0/histcite/compute_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,24 +36,24 @@
         elif 'LCS' not in use_cols and 'TC' not in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count'}).rename(columns={col: 'Recs'})
         else:
             raise ValueError('Invalid columns list')
         return grouped_df.sort_values('Recs', ascending=False)
     
     def _generate_author_table(self):
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             use_cols = ['AU','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['AU','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'AU','; ')
     
     def _generate_keywords_table(self):
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             use_cols = ['DE','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['DE','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'DE','; ',True)
     
@@ -64,27 +64,27 @@
             use_cols = ['C3','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'C3','; ')
     
     def _generate_records_table(self):
         """生成文献简表"""
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             use_cols = ['AU','TI','SO','LCS','TC','LCR','NR']
         elif self.source_type == 'cssci':
-            use_cols = ['AU','TI','SO','LCS','LCR']
+            use_cols = ['AU','TI','SO','LCS','LCR','NR']
         else:
             raise ValueError('Invalid source type')
         records_table = self.docs_table[use_cols]
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             records_table = records_table.rename(columns={'TC':'GCS','NR':'GCR'})
         return records_table
     
     def _generate_journal_table(self):
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             use_cols = ['SO','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['SO','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'SO')
 
@@ -96,19 +96,19 @@
         use_cols = ['DT']
         return self.__generate_table(use_cols,'DT')
    
     def _generate_reference_table(self):
         """生成参考文献表，按照引用次数降序排列，同时标记是否为本地文献"""
         if self.source_type == 'wos':
             check_cols = ['PY','J9','VL','BP']
-        elif self.source_type == 'cssci':
+        elif self.source_type in ['cssci','scopus']:
             check_cols = ['first_AU','TI']
         else:
             raise ValueError('Invalid source type')
-        use_cols = self.reference_table.columns.tolist()[:-1]
+        use_cols = self.reference_table.columns.tolist()[:-1]  
         reference_table = self.reference_table.groupby(use_cols,as_index=False).size()
         reference_table = reference_table.sort_values(by='size',ascending=False)
         reference_table = reference_table.rename(columns={'size':'Recs'})
         common_table = reference_table.reset_index().merge(self.docs_table[check_cols],on=check_cols)
         reference_table['local'] = 0
         reference_table.loc[common_table['index'],'local'] = 1
         return reference_table
@@ -121,10 +121,12 @@
         with pd.ExcelWriter(save_path) as writer:
             self._generate_records_table().to_excel(writer,sheet_name='Records',index=False)
             self._generate_author_table().to_excel(writer,sheet_name='Authors')
             self._generate_journal_table().to_excel(writer,sheet_name='Journals')
             self._generate_reference_table().to_excel(writer,sheet_name='Cited References',index=False)
             self._generate_keywords_table().to_excel(writer,sheet_name='Keywords')
             self._generate_year_table().to_excel(writer,sheet_name='Years')
-            self._generate_institution_table().to_excel(writer,sheet_name='Institutions')
-            if self.source_type == 'wos':
+            
+            if self.source_type in ['wos','cssci']:
+                self._generate_institution_table().to_excel(writer,sheet_name='Institutions')
+            if self.source_type in ['wos','scopus']:
                 self._generate_document_type_table().to_excel(writer,sheet_name='Document Type')
```

### Comparing `histcite-python-0.2.1/histcite/network_graph.py` & `histcite-python-0.3.0/histcite/network_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,18 +85,22 @@
             
         for dot_edge in dot_edge_list:
             dot_text += dot_edge
         dot_text += '}'
         return dot_text
     
     def generate_graph_node_file(self)->pd.DataFrame:
+
+        # source_type会对节点信息产生影响
         if self.source_type == 'wos':
             use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
         elif self.source_type == 'cssci':
-            use_cols = ['doc_index','AU','PY','SO','LCS']
+            use_cols = ['doc_index','AU','TI','PY','SO','LCS']
+        elif self.source_type == 'scopus':
+            use_cols = ['doc_index','AU','TI','PY','SO','LCS','TC']
         else:
             raise ValueError('invalid source type')
         graph_node_table = self.docs_table.loc[self.node_list,use_cols]
         
         try:
             graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
         except KeyError:
```

### Comparing `histcite-python-0.2.1/histcite/parse_reference.py` & `histcite-python-0.3.0/histcite/parse_reference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import re
 
 class ParseReference:
     def __init__(self,doc_index,cr_cell:str,source_type:str):
         """Parse citation records from a cr cell
         doc_index: index of the record
         cr_cell: cr cell
-        source_type: wos|cssci
+        source_type: wos|cssci|scopus
         """
-        if source_type=='wos':
-            sep = '; '
-        elif source_type=='cssci':
-            sep = '\n'
-        else:
-            raise ValueError('Invalid source type')
-        
+        sep = '; '
         try:
             self.cr_list = cr_cell.split(sep)
             self.cr_count = len(self.cr_list)
         except AttributeError:
             self.cr_count = 0
-        self.doc_index = doc_index
-        self.source_type = source_type
+        else:
+            self.doc_index = doc_index
+            self.source_type = source_type
 
     @staticmethod
-    def _parse_wos_cr(cr):
-        """Parse a single citation record"""
+    def _parse_wos_cr(cr:str):
         AU,PY,J9,VL,BP,DI = None,None,None,None,None,None
         cr_data = {}
 
         try:
             AU,PY,J9,other = re.split(r', (?![^\[\]]*\])',cr,3)
         except ValueError:
             if len(fields := re.split(r', (?![^\[\]]*\])',cr,2))==3:
@@ -65,63 +59,82 @@
             cr_data['J9'] = J9
             cr_data['VL'] = VL 
             cr_data['BP'] = BP 
             cr_data['DI'] = DI 
             return cr_data
     
     @staticmethod
-    def _parse_cssci_cr(cr):
-
-        pattern = re.compile(r'(?<!\d)\.(?!\d)|(?<=\d)\.(?!\d)|(?<!\d)\.(?=\d)|(?<=\d{4})\.(?=\d{4})')
+    def _parse_cssci_cr(cr:str):
+        
+        au_pattern = re.compile(r'(?<!\d)\.(?!\d)|(?<=\d)\.(?!\d)|(?<!\d)\.(?=\d)|(?<=\d{4})\.(?=\d{4})')
         # 中文参考文献
         if re.search(r'[\u4e00-\u9fa5]',cr):
             try:
-                # _,AU,TI,_ = cr.split('.',3)
-                _,AU,TI,_ = pattern.split(cr,3)
+                _,AU,TI,_ = au_pattern.split(cr,3)
                 if ',' not in AU:
                     return {'first_AU':AU,'TI':TI}
             except ValueError:
                 return None
     
         # 英文参考文献
         else:
             if index_AU := re.search(r'^(\d+\.(.*?))\.[A-Za-z"“\d]{1}[a-zA-Z\s\d]+',cr):
                 AU = index_AU.group(2)
                 if AU !='':
-                    # other = cr.replace(f'{AU}.','')
                     other = cr.replace(index_AU.group(1),'')
                     try:
-                        # _,TI,_ = other.split('.',2)
-                        _,TI,_ = pattern.split(other,2)
+                        _,TI,_ = au_pattern.split(other,2)
                         return {'first_AU':AU,'TI':TI}
                     except ValueError:
                         return None
                         
                 else:
                     try:
-                        _,_,TI,_ = pattern.split(cr,3)
+                        _,_,TI,_ = au_pattern.split(cr,3)
                     except ValueError:
                         _,_,TI,_ = cr.split('.',3)
-                    finally:
-                        return {'first_AU':AU,'TI':TI} # type:ignore
-                     
+                    return {'first_AU':AU,'TI':TI}
+    
+    @staticmethod
+    def _parse_scopus_cr(cr:str,TI_pattern):
+        
+        if TI := TI_pattern.search(cr):
+            TI = TI[0]
+            if re.match('^[a-z]',TI):
+                # print('No TI:',cr)
+                return None
+            else:
+                left_cr = cr.replace(TI,'')
+                try:
+                    first_AU = left_cr.split(',',1)[0]
+                    if re.match('[A-Za-z]',first_AU):
+                        return {'first_AU':first_AU,'TI':TI.strip(',;?.').lower()}
+                    else:
+                        # print('No AU:',cr)
+                        return None
+                except IndexError:
+                    return None
+                
     def parse_cr_cell(self):
         if self.cr_count == 0:
             return None
         
         if self.source_type == "wos":
             parsed_cr_list = [self._parse_wos_cr(i) for i in self.cr_list]
             keys = ['first_AU','PY','J9','VL','BP','DI']
         elif self.source_type == "cssci":
             parsed_cr_list = [self._parse_cssci_cr(i) for i in self.cr_list]
             keys = ['first_AU','TI']
+        elif self.source_type == "scopus":
+            TI_pattern = re.compile(r'\b(?:[^\.,\s]+\s){4,}[^\.,\s]+(?:,|\?|\.|;|$)')
+            parsed_cr_list = [self._parse_scopus_cr(i,TI_pattern) for i in self.cr_list]
+            keys = ['first_AU','TI']
         else:
-            raise ValueError()
+            raise ValueError('Invalid source type')
         
         result = {key:[] for key in keys}
         for single in parsed_cr_list:
             if single is not None:
                 for key in keys:
                     result[key].append(single[key])
-        
         result['doc_index'] = self.doc_index
         return result
```

### Comparing `histcite-python-0.2.1/histcite/process_file.py` & `histcite-python-0.3.0/histcite/process_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 import os
 import re
 import pandas as pd
 from histcite.parse_reference import ParseReference
 from histcite.recognize_reference import RecognizeReference
 
+class ProcessWosFile:
+    @staticmethod
+    def extract_first_author(au_cell:str):
+        return au_cell.split(';',1)[0].replace(',','')
+
 class ProcessCssciFile:
     @staticmethod
-    def process_orgs(cell):
+    def process_org(cell):
         org_set = set(re.findall(r'](.*?)(?:/|$)',cell))
         org_list = [i.replace('.','') for i in org_set]
         return '; '.join(org_list)
 
-class ProcessWosFile:
+class ProcessScopusFile:
     @staticmethod
-    def extract_first_author(au_cell:str):
-        """提取一作"""
-        return au_cell.split(';',1)[0].replace(',','')
-
+    def extract_first_author(au_field:pd.Series):
+        return au_field.str.split(pat=';',n=1,expand=True)[0]
+    
+class ReadFile:
+    @staticmethod
+    def _read_csv(file_path:str,use_cols:list,sep:str=',')->pd.DataFrame:
+        try:
+            df = pd.read_csv(
+                file_path,
+                sep=sep,
+                header=0,
+                on_bad_lines='skip',
+                usecols=use_cols,
+                dtype_backend="pyarrow")
+            return df
+        except ValueError:
+            file_name = os.path.basename(file_path)
+            raise ValueError(f'File {file_name} is not a valid csv file')
+        
 class ProcessFile:
 
     def __init__(self,folder_path:str,source_type:str):
         """
         folder_path: 文件夹路径\n
         source_type: 数据来源 wos|cssci|scopus|pubmed
         """
         self.folder_path = folder_path
         self.source_type = source_type
         if source_type=='wos':
             self.file_name_list = [i for i in os.listdir(folder_path) if i[:9]=='savedrecs']
         elif source_type=='cssci':
             self.file_name_list = [i for i in os.listdir(folder_path) if i[:3]=='LY_']
+        elif source_type=='scopus':
+            self.file_name_list = [i for i in os.listdir(folder_path) if i[:6]=='scopus']
         else:
             raise ValueError('Invalid source type')
         
     def _read_wos_file(self,file_name:str)->pd.DataFrame:
         """读取wos表单"""
         use_cols = ['AU','TI','SO','DT','CR','DE','C3','NR','TC','Z9','J9','PY','VL','BP','DI','UT']
         file_path = os.path.join(self.folder_path,file_name)
-        try:
-            df = pd.read_csv(
-                file_path,sep='\t',
-                header=0,
-                on_bad_lines='skip',
-                usecols=use_cols,
-                dtype_backend="pyarrow") 
-        except ValueError:
-            raise ValueError(f'File {file_name} is not a tab delimited file of wos')
-        
-        else:
-            # 转换数据类型
-            df['BP'] = df['BP'].apply(pd.to_numeric,errors='coerce')
-            df['VL'] = df['VL'].apply(pd.to_numeric,errors='coerce')
-            df = df.astype({'BP':'int64[pyarrow]', 'VL':'int64[pyarrow]'})
-            
-            # 提取一作
-            first_au = df['AU'].apply(ProcessWosFile.extract_first_author)
-            df.insert(1,'first_AU',first_au)
-            return df
+        df = ReadFile._read_csv(file_path,use_cols,'\t')
         
+        # 转换数据类型
+        df['BP'] = df['BP'].apply(pd.to_numeric,errors='coerce')
+        df['VL'] = df['VL'].apply(pd.to_numeric,errors='coerce')
+        df = df.astype({'BP':'int64[pyarrow]', 'VL':'int64[pyarrow]'})
+        
+        # 提取一作
+        first_au = df['AU'].apply(ProcessWosFile.extract_first_author)
+        df.insert(1,'first_AU',first_au)
+        return df
+    
     def _read_cssci_file(self,file_name:str)->pd.DataFrame:
         """读取cssci文本文件"""
         file_path = os.path.join(self.folder_path,file_name)
         with open(file_path,'r') as f:
             text = f.read()
         
         if text[:16] != '南京大学中国社会科学研究评价中心':
@@ -78,63 +91,92 @@
                 contents[field] = re.findall(field_pattern,body_text,flags=re.S)
         
         df = pd.DataFrame.from_dict(contents)
         df.columns = ['TI','AU','FU','SO','first_org','C3','first_AU','PY&VL&BP&EP','DE','CR']
         df['AU'] = df['AU'].str.replace('/','; ')
         df['DE'] = df['DE'].str.replace('/','; ')
         df['PY'] = df['PY&VL&BP&EP'].str.extract(r'^(\d{4}),',expand=False)
-        df['C3'] = df['C3'].apply(ProcessCssciFile.process_orgs)
+        df['C3'] = df['C3'].apply(ProcessCssciFile.process_org)
+        df['CR'] = df['CR'].str.replace('\n','; ')
+        df['NR'] = df['CR'].str.count('; ')
+        return df
+    
+    def _read_scopus_file(self,file_name:str)->pd.DataFrame:
+        """读取scopus表单"""
+        use_cols = ['Authors','Title','Year','Source title','Volume','Issue','Cited by','DOI','Affiliations','Author Keywords','References','Document Type','EID']
+        file_path = os.path.join(self.folder_path,file_name)
+        df = ReadFile._read_csv(file_path,use_cols)
+        df.columns = ['AU','TI','PY','SO','VL','IS','TC','DI','C3','DE','CR','DT','EID']
+        df['NR'] = df['CR'].str.count('; ')
+        df['first_AU'] = ProcessScopusFile.extract_first_author(df['AU'])
         return df
     
     def concat_table(self):
         """合并多个dataframe"""
         if len(self.file_name_list)>1:
             if self.source_type=='wos':
                 docs_table = pd.concat([self._read_wos_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
             elif self.source_type=='cssci':
                 docs_table = pd.concat([self._read_cssci_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
+            elif self.source_type=='scopus':
+                docs_table = pd.concat([self._read_scopus_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
             else:
                 raise ValueError('Invalid source type')
         
         elif len(self.file_name_list)==1:
             if self.source_type=='wos':
                 docs_table = self._read_wos_file(self.file_name_list[0])
             elif self.source_type=='cssci':
                 docs_table = self._read_cssci_file(self.file_name_list[0])
+            elif self.source_type=='scopus':
+                docs_table = self._read_scopus_file(self.file_name_list[0])
             else:
                 raise ValueError('Invalid source type')
         
         else:
             raise FileNotFoundError('No valid file in the folder')
         
         original_num = docs_table.shape[0]
         # 删除重复数据
         if self.source_type=='wos':
             docs_table.drop_duplicates(subset=['UT'],ignore_index=True,inplace=True) # 根据入藏号删除重复数据
         elif self.source_type=='cssci':
             docs_table.drop_duplicates(subset=['TI','first_AU'],ignore_index=True,inplace=True) # 根据题名和一作删除重复数据
+        elif self.source_type=='scopus':
+            docs_table.drop_duplicates(subset=['EID'],ignore_index=True,inplace=True) # 根据eid删除重复数据
         current_num = docs_table.shape[0]
         print(f'共读取 {original_num} 条数据，去重后剩余 {current_num} 条')
         
         # 按照年份进行排序
         docs_table = docs_table.sort_values(by='PY',ignore_index=True)
         docs_table.insert(0,'doc_index',docs_table.index)
+
+        # scopus题名转小写
+        if self.source_type == 'scopus':
+            self.TI_COPY = docs_table['TI'].copy()
+            docs_table['TI'] = docs_table['TI'].str.lower()
+        
         self.docs_table = docs_table
         return docs_table
     
     def __generate_reference_table(self,cr_series:pd.Series):
         """生成参考文献表格"""
         if self.source_type=='wos':
             parsed_cr_cells = [ParseReference(doc_index,cell,'wos').parse_cr_cell() for doc_index,cell in cr_series.items()]
             reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
             reference_table = reference_table.astype({'PY':'int64[pyarrow]', 'VL':'int64[pyarrow]', 'BP':'int64[pyarrow]'})
         
         elif self.source_type=='cssci':
             parsed_cr_cells = [ParseReference(doc_index,cell,'cssci').parse_cr_cell() for doc_index,cell in cr_series.items()]
             reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
+         
+        elif self.source_type=='scopus':
+            parsed_cr_cells = [ParseReference(doc_index,cell,'scopus').parse_cr_cell() for doc_index,cell in cr_series.items()]
+            reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
+
         else:
             raise ValueError('Invalid source type')
         self.reference_table = reference_table
     
     @staticmethod
     def __reference2citation(reference_field:pd.Series)->pd.Series:
         """参考文献转换到引文"""
@@ -144,23 +186,27 @@
                 for ref_index in ref_list:
                     citation_field[ref_index].append(doc_index)
         return citation_field
     
     def process_citation(self):
         """处理引文"""
         self.__generate_reference_table(self.docs_table['CR'])
-        recognize_reference_instance = RecognizeReference(self.docs_table,self.reference_table)
         
         if self.source_type=='wos':
-            reference_field = self.docs_table.apply(lambda row:recognize_reference_instance.recognize_wos_reference(row.name),axis=1)
+            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_wos_reference(self.docs_table,self.reference_table,row.name),axis=1)
         elif self.source_type=='cssci':
-            reference_field = self.docs_table.apply(lambda row:recognize_reference_instance.recognize_cssci_reference(row.name,True),axis=1)
+            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_cssci_reference(self.docs_table,self.reference_table,row.name),axis=1)
+        elif self.source_type=='scopus':
+            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_scopus_reference(self.docs_table,self.reference_table,row.name),axis=1)
         else:
             raise ValueError('Invalid source type')
         
         citation_field = self.__reference2citation(reference_field)
         lcr_field = reference_field.apply(len)
         lcs_field = citation_field.apply(len)
         self.docs_table['reference'] = [';'.join([str(j) for j in i]) if i else None for i in reference_field]
         self.docs_table['citation'] = [';'.join([str(j) for j in i]) if i else None for i in citation_field]
         self.docs_table['LCR'] = lcr_field
-        self.docs_table['LCS'] = lcs_field
+        self.docs_table['LCS'] = lcs_field
+
+        if self.source_type == 'scopus':
+            self.docs_table['TI'] = self.TI_COPY
```

### Comparing `histcite-python-0.2.1/histcite/recognize_reference.py` & `histcite-python-0.3.0/histcite/recognize_reference.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,96 @@
 import pandas as pd
 
-class RecognizeReference:
-    """识别参考文献"""
-
-    def __init__(self,docs_table:pd.DataFrame, reference_table:pd.DataFrame) -> None:
+class RecognizeCommonReference:
+    def __init__(self,docs_table:pd.DataFrame, reference_table:pd.DataFrame):
         self.docs_table = docs_table
         self.reference_table = reference_table
 
-    def recognize_wos_reference(self,row_index,merge_method=False)->list:
+    def filter_tables(self,row_index,compare_cols:list)->tuple:
+        assert set(compare_cols+['PY','doc_index']).issubset(self.docs_table.columns)
+        assert set(compare_cols).issubset(self.reference_table.columns)
+
+        row_year = self.docs_table.loc[row_index,'PY']
+        child_reference_table = self.reference_table[self.reference_table['doc_index']==row_index].dropna(subset=compare_cols)
+        child_docs_table = self.docs_table[self.docs_table['PY']<=row_year].dropna(subset=compare_cols)
+        return child_docs_table,child_reference_table
+    
+    def recognize_ref(self,child_docs_table:pd.DataFrame,
+                            child_reference_table:pd.DataFrame,
+                            compare_cols:list,
+                            merge_method:bool)->list:
+        
+        local_ref_list = []
+        if merge_method:
+            common_table = child_docs_table[['doc_index']+compare_cols].merge(child_reference_table[compare_cols])
+            if common_table.shape[0]>0:
+                common_table = common_table.drop_duplicates(subset='doc_index',ignore_index=True)
+                local_ref_list.extend(common_table['doc_index'].tolist())
+        else:
+            for idx,row_data in child_docs_table.iterrows():
+                for _,child_reference in child_reference_table.iterrows():
+                    if all(row_data[col]==child_reference[col] for col in compare_cols):
+                        local_ref_list.append(idx)
+        return local_ref_list
+
+
+class RecognizeReference():
+    """识别参考文献"""
+
+    @staticmethod
+    def recognize_wos_reference(docs_table:pd.DataFrame,
+                                reference_table:pd.DataFrame,
+                                row_index:int)->list:
+        
         local_ref_list = []
-        child_reference_table = self.reference_table[self.reference_table['doc_index']==row_index]
-            
+        child_reference_table = reference_table[reference_table['doc_index']==row_index]
+        
         # 存在DOI
         child_reference_table_doi = child_reference_table[child_reference_table['DI'].notna()]['DI']
-        child_docs_table_doi = self.docs_table[self.docs_table['DI'].notna()]['DI']
+        child_docs_table_doi = docs_table[docs_table['DI'].notna()]['DI']
         local_ref_list.extend(child_docs_table_doi[child_docs_table_doi.isin(child_reference_table_doi)].index.tolist())
         
         # 不存在DOI
         compare_cols = ['first_AU','PY','J9','BP']
         child_reference_table_left = child_reference_table[child_reference_table['DI'].isna()].dropna(subset=compare_cols)
         child_reference_py = child_reference_table_left['PY']
         child_reference_bp = child_reference_table_left['BP']
 
         # 年份符合，页码符合，doi为空
-        child_docs_table_left = self.docs_table[(self.docs_table['PY'].isin(child_reference_py))&(self.docs_table['BP'].isin(child_reference_bp)&self.docs_table['DI'].isna())].dropna(subset=compare_cols)
-        
-        if merge_method:
-            common_table = child_docs_table_left[['doc_index']+compare_cols].merge(child_reference_table_left)
-            if common_table.shape[0]>0:
-                common_table = common_table.drop_duplicates(subset='doc_index',ignore_index=True)
-                local_ref_list.extend(common_table['doc_index'].tolist())
-          
-        else:
-            for idx,row_data in child_docs_table_left.iterrows():
-                for _,child_reference in child_reference_table_left.iterrows():
-                    if all(row_data[col]==child_reference[col] for col in compare_cols):
-                        local_ref_list.append(idx)
+        recognize_instance = RecognizeCommonReference(docs_table,reference_table)
+        child_docs_table_left = docs_table[(docs_table['PY'].isin(child_reference_py))&(docs_table['BP'].isin(child_reference_bp)&docs_table['DI'].isna())].dropna(subset=compare_cols)
+        local_ref_list.extend(recognize_instance.recognize_ref(child_docs_table_left,child_reference_table_left,compare_cols,merge_method=True))
         
+        try:
+            local_ref_list.remove(row_index)
+        except ValueError:
+            pass
         return local_ref_list
     
-    def recognize_cssci_reference(self,row_index,merge_method=False)->list:
-        local_ref_list = []
+    @staticmethod
+    def recognize_cssci_reference(docs_table:pd.DataFrame,
+                                  reference_table:pd.DataFrame,
+                                  row_index:int)->list:
+        
         compare_cols = ['first_AU','TI']
-        child_reference_table = self.reference_table[self.reference_table['doc_index']==row_index].dropna(subset=compare_cols)
-        row_year = self.docs_table.loc[row_index,'PY']
-        child_docs_table = self.docs_table[self.docs_table['PY']<=row_year].dropna(subset=compare_cols)
-
-        if merge_method:
-            common_table = child_docs_table[['doc_index']+compare_cols].merge(child_reference_table[compare_cols])
-            if common_table.shape[0]>0:
-                common_table = common_table.drop_duplicates(subset='doc_index',ignore_index=True)
-                local_ref_list.extend(common_table['doc_index'].tolist())
-        else:
-            for idx,row_data in child_docs_table.iterrows():
-                for _,child_reference in child_reference_table.iterrows():
-                    if all(row_data[col]==child_reference[col] for col in compare_cols):
-                        local_ref_list.append(idx)
-        return local_ref_list
+        recognize_instance = RecognizeCommonReference(docs_table,reference_table)
+        child_docs_table,child_reference_table = recognize_instance.filter_tables(row_index,compare_cols)
+        result = recognize_instance.recognize_ref(child_docs_table,child_reference_table,compare_cols,merge_method=True)
+        try:
+            result.remove(row_index)
+        except ValueError:
+            pass
+        return result
+    
+    @staticmethod
+    def recognize_scopus_reference(docs_table:pd.DataFrame,
+                                   reference_table:pd.DataFrame,
+                                   row_index:int)->list:
+        compare_cols = ['first_AU','TI']
+        recognize_instance = RecognizeCommonReference(docs_table,reference_table)
+        child_docs_table,child_reference_table = recognize_instance.filter_tables(row_index,compare_cols)
+        result = recognize_instance.recognize_ref(child_docs_table,child_reference_table,compare_cols,merge_method=True)
+        try:
+            result.remove(row_index)
+        except ValueError:
+            pass
+        return result
```

### Comparing `histcite-python-0.2.1/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.3.0/histcite_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,16 @@
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
-- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持，并对调用方式进行调整；
+- `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
+- `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -47,24 +48,25 @@
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | 核心合集，格式选择 Tab delimited file/制表符分隔文件，导出内容选择 Full Record and Cited References/全记录与引用的参考文献 或者是 Custome selection/自定义选择项，全选字段 |
-| `CSSCI` | 从CSSCI数据库正常导出即可 |
-> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹下。
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。不勾选 `Truncate to optimize for Excel`|
+> 注：文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
-| -t | --source_type | 题录数据来源，可选 `wos` 或 `cssci`，必须指定 |
+| -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
@@ -128,19 +130,16 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
-1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
-`CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
-
-2、如何去重？  
-`Web of Science:` 按照 `UT` 入藏号字段进行去重。  
-`CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
+|  | Web of Science | CSSCI | Scopus|
+| --- | --- | --- | --- |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；</br>否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [ ] 支持 `Scopus` 题录数据
+- [x] 支持 `Scopus` 题录数据
 - [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.2.1/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.3.0/histcite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.1/setup.py` & `histcite-python-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.2.1",
+    version="0.3.0",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.2.1/tests/test_network_graph.py` & `histcite-python-0.3.0/tests/test_network_graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+import pytest
 import pandas as pd
 from histcite.network_graph import GraphViz
 
+@pytest.mark.skip(reason='This is a function factory')
+def test_graph(file_path,source_type):
+    def new_func():
+        docs_table = pd.read_csv(file_path,dtype_backend='pyarrow')
+        doc_indices = docs_table.sort_values('LCS', ascending=False).index[:10]
+        G = GraphViz(docs_table,source_type)
+        graph_dot_file = G.generate_dot_file(doc_indices)
+        return graph_dot_file
+    return new_func
+
 def test_wos_graph():
     file_path = 'tests/wos_docs_table.csv'
-    docs_table = pd.read_csv(file_path,dtype_backend='pyarrow')
-    doc_indices = docs_table.sort_values('LCS', ascending=False).index[:50]
-    G = GraphViz(docs_table,'wos')
-    graph_dot_file = G.generate_dot_file(doc_indices)
+    graph_dot_file = test_graph(file_path,'wos')()
     assert graph_dot_file[:7] == 'digraph'
 
 def test_cssci_graph():
     file_path = 'tests/cssci_docs_table.csv'
-    docs_table = pd.read_csv(file_path,dtype_backend='pyarrow')
-    doc_indices = docs_table.sort_values('LCS', ascending=False).index[:50]
-    G = GraphViz(docs_table,'cssci')
-    graph_dot_file = G.generate_dot_file(doc_indices)
+    graph_dot_file = test_graph(file_path,'cssci')()
+    assert graph_dot_file[:7] == 'digraph'
+
+def test_scopus_graph():
+    file_path = 'tests/scopus_docs_table.csv'
+    graph_dot_file = test_graph(file_path,'scopus')()
     assert graph_dot_file[:7] == 'digraph'
```

