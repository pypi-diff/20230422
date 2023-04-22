# Comparing `tmp/histcite-python-0.0.1.tar.gz` & `tmp/histcite-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.0.1.tar", last modified: Sat Apr 22 13:11:02 2023, max compression
+gzip compressed data, was "histcite-python-0.1.1.tar", last modified: Sat Apr 22 17:01:09 2023, max compression
```

## Comparing `histcite-python-0.0.1.tar` & `histcite-python-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:11:02.451618 histcite-python-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 13:10:47.000000 histcite-python-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-22 13:11:02.451618 histcite-python-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-04-22 13:10:47.000000 histcite-python-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:11:02.451618 histcite-python-0.0.1/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-22 13:10:47.000000 histcite-python-0.0.1/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:11:02.451618 histcite-python-0.0.1/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 13:11:02.000000 histcite-python-0.0.1/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 13:11:02.451618 histcite-python-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-22 13:10:47.000000 histcite-python-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:11:02.451618 histcite-python-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 13:10:47.000000 histcite-python-0.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-22 13:10:47.000000 histcite-python-0.0.1/test/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-22 13:10:47.000000 histcite-python-0.0.1/test/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-22 13:10:47.000000 histcite-python-0.0.1/test/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 17:00:55.000000 histcite-python-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-22 17:01:09.871692 histcite-python-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-22 17:00:55.000000 histcite-python-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.867692 histcite-python-0.1.1/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/parse_citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/process_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:01:09.871692 histcite-python-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-22 17:00:55.000000 histcite-python-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_parse_citation.py
```

### Comparing `histcite-python-0.0.1/LICENSE` & `histcite-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.0.1/PKG-INFO` & `histcite-python-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.0.1
+Version: 0.1.1
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [Python](https://www.python.org/) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -43,69 +43,72 @@
 
 ```console
 $ python3 -m pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-
 ```console
-$ 下载的wos文件夹路径为 ~/downloads/wos，引文网络图包含的节点数为 100
-$ histcite -f ~/downloads/wos -n 100
+$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
 ```
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文关系图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx` 和 `graph.dot` 两个文件，前者是引文统计表，后者为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。  
+> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
 
 生成的引文网络图如下所示：
 <img src="examples/graph.svg">  
 
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](https://github.com/doublessay/histcite-python/blob/main/demo.ipynb)
+2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
+import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
-folder_path = '~/downloads/wos' # 下载的题录数据存放的文件夹路径
+folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path) # 读取并处理题录数据
 concated_table = process.concat_table() # 合并多个文件
 
-# 提取所有文献的参考文献, 参考 test/reference_table.xlsx
+# 提取所有文献的参考文献
 reference_table = process.generate_reference_table(concated_table['CR']) 
 
-# 识别引文关系, 参考 test/citation_table.xlsx
+# 识别引文关系
 citation_table = process.process_citation(reference_table) 
 
 # 各分析单元的引文统计
 cm = ComputeMetrics(citation_table, reference_table)
-cm.write2excel('~/downloads/wos/statistics.xlsx')
+cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(primary_table)
-doc_indices = primary_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-dot_text = graph.generate_dot_text(doc_indices, allow_external_node=False) # 生成引文网络图的数据文件
-
-# 根据需要保存图文件
-with open('~/downloads/wos/result/graph.dot', 'w') as f:
+graph = Graphviz(citation_table)
+doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
+
+# 生成引文网络图节点文件
+graph_node_file = graph.generate_graph_node_file()
+graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 > `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | - | - | - |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
-| 是否提供前端界面 | 否 | 是 |
 | 是否开源 | 是 | 否 |
+| 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
 - [ ] 支持 `scopus` 题录数据
 - [ ] 构建GUI页面
```

### Comparing `histcite-python-0.0.1/README.md` & `histcite-python-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [Python](https://www.python.org/) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -20,69 +20,72 @@
 
 ```console
 $ python3 -m pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-
 ```console
-$ 下载的wos文件夹路径为 ~/downloads/wos，引文网络图包含的节点数为 100
-$ histcite -f ~/downloads/wos -n 100
+$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
 ```
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文关系图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx` 和 `graph.dot` 两个文件，前者是引文统计表，后者为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。  
+> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
 
 生成的引文网络图如下所示：
 <img src="examples/graph.svg">  
 
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](https://github.com/doublessay/histcite-python/blob/main/demo.ipynb)
+2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
+import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
-folder_path = '~/downloads/wos' # 下载的题录数据存放的文件夹路径
+folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path) # 读取并处理题录数据
 concated_table = process.concat_table() # 合并多个文件
 
-# 提取所有文献的参考文献, 参考 test/reference_table.xlsx
+# 提取所有文献的参考文献
 reference_table = process.generate_reference_table(concated_table['CR']) 
 
-# 识别引文关系, 参考 test/citation_table.xlsx
+# 识别引文关系
 citation_table = process.process_citation(reference_table) 
 
 # 各分析单元的引文统计
 cm = ComputeMetrics(citation_table, reference_table)
-cm.write2excel('~/downloads/wos/statistics.xlsx')
+cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(primary_table)
-doc_indices = primary_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-dot_text = graph.generate_dot_text(doc_indices, allow_external_node=False) # 生成引文网络图的数据文件
-
-# 根据需要保存图文件
-with open('~/downloads/wos/result/graph.dot', 'w') as f:
+graph = Graphviz(citation_table)
+doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
+
+# 生成引文网络图节点文件
+graph_node_file = graph.generate_graph_node_file()
+graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 > `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | - | - | - |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
-| 是否提供前端界面 | 否 | 是 |
 | 是否开源 | 是 | 否 |
+| 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
 - [ ] 支持 `scopus` 题录数据
 - [ ] 构建GUI页面
```

### Comparing `histcite-python-0.0.1/histcite/cli.py` & `histcite-python-0.1.1/histcite/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-import argparse
 import os
+import argparse
+import pandas as pd
 from histcite.compute_metrics import ComputeMetrics
 from histcite.process_table import ProcessTable
 from histcite.network_graph import GraphViz
-
-def generate_file_path(output_path:str, file_name:str):
-    if output_path:
-        return os.path.join(output_path,file_name)
-    else:
-        return file_name
     
 def main():
     parser = argparse.ArgumentParser(description='A Python interface to histcite.')
-    parser.add_argument('-f','--folder_path', type=str, help='下载的题录数据存放的文件夹路径')
-    # parser.add_argument('-o','--output_path', type=str, default=None, help='结果保存路径，默认为当前目录')
-    parser.add_argument('-g','--graph', type=str, default='false', help='是否仅生成图文件，默认为false')
-    parser.add_argument('-n','--node_num', type=int, default=50, help='生成图文件的节点数量，默认为50')
+    parser.add_argument('-f','--folder_path', type=str, help='folder path of the downloaded files')
+    parser.add_argument('-n','--node_num', type=int, default=50, help='node number in the citation network graph')
+    parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
     # 将结果存放在用户指定的 folder_path 下的result文件夹中
     output_path = os.path.join(args.folder_path,'result')
+    if not os.path.exists(output_path):
+        os.mkdir(output_path)
     process = ProcessTable(args.folder_path)
     concated_table = process.concat_table()
     reference_table = process.generate_reference_table(concated_table['CR'])
     citation_table = process.process_citation(reference_table)
 
-    if args.graph == 'false':
+    if not args.graph:
         cm = ComputeMetrics(citation_table, reference_table)
-        cm_output_path = generate_file_path(output_path,'statistics.xlsx')
+        cm_output_path = os.path.join(output_path,'statistics.xlsx')
         cm.write2excel(cm_output_path)
 
     doc_indices = citation_table.sort_values('LCS', ascending=False).index[:args.node_num]
-    graph = GraphViz(citation_table).generate_dot_text(doc_indices)
-    graph_output_path = generate_file_path(output_path,'graph.dot')
-    with open(graph_output_path,'w') as f:
-        f.write(graph)
+    graph = GraphViz(citation_table)
+    
+    # 生成图文件
+    graph_dot_file = graph.generate_dot_file(doc_indices)
+    graph_dot_path = os.path.join(output_path,'graph.dot')
+    with open(graph_dot_path,'w') as f:
+        f.write(graph_dot_file)
+
+    # 生成节点文件
+    graph_node_file = graph.generate_graph_node_file()
+    graph_node_file.to_excel(os.path.join(output_path,'graph.node.xlsx'),index=False)
```

### Comparing `histcite-python-0.0.1/histcite/compute_metrics.py` & `histcite-python-0.1.1/histcite/compute_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pandas as pd
 
 class ComputeMetrics:
     """生成统计结果"""
 
     def __init__(self,citation_table,reference_table):
         self.citation_table = citation_table
@@ -67,17 +68,20 @@
         reference_table = reference_table.sort_values(by='size',ascending=False)
         reference_table = reference_table.rename(columns={'size':'Recs'})
         common_table = reference_table.reset_index().merge(self.citation_table[check_cols],on=check_cols)
         reference_table['local'] = 0
         reference_table.loc[common_table['index'],'local'] = 1
         return reference_table
     
-    def write2excel(self,file_name):
+    def write2excel(self,save_path):
         """将统计结果写入excel"""
-        with pd.ExcelWriter(file_name) as writer:
+        save_folder_path = os.path.dirname(save_path)
+        if not os.path.exists(save_folder_path):
+            os.makedirs(save_folder_path)
+        with pd.ExcelWriter(save_path) as writer:
             self._generate_records_table().to_excel(writer,sheet_name='Records',index=False)
             self._generate_author_table().to_excel(writer,sheet_name='Authors')
             self._generate_journal_table().to_excel(writer,sheet_name='Journals')
             self._generate_reference_table().to_excel(writer,sheet_name='Cited References',index=False)
             self._generate_keywords_table().to_excel(writer,sheet_name='Keywords')
             self._generate_year_table().to_excel(writer,sheet_name='Years')
             self._generate_document_type_table().to_excel(writer,sheet_name='Document Type')
```

### Comparing `histcite-python-0.0.1/histcite/network_graph.py` & `histcite-python-0.1.1/histcite/network_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 class GraphViz:
 
-    def __init__(self,df):
-        self.citation_table = df
-        self.year_empty_index = set(df[df['PY'].isna()].index)
+    def __init__(self,citation_table):
+        self.citation_table = citation_table
+        self.year_empty_index = set(citation_table[citation_table['PY'].isna()].index)
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
 
         year_series = self.citation_table.loc[self.node_list,'PY']
         groups = year_series.groupby(year_series)
         year_list = [i[0] for i in groups]
@@ -51,15 +51,15 @@
 
         edge_list = {i:[] for i in sorted(source_node)}
         for edge in edge_set:
             edge_list[edge[0]].append(edge[1])
 
         return edge_list
         
-    def generate_dot_text(self,doc_indices,allow_external_node=False):
+    def generate_dot_file(self,doc_indices,allow_external_node=False):
         """生成dot文件
         doc_indices: 文献索引列表;
         allow_external_node: 是否允许出现doc_indices之外的节点，默认False
         """
         self.doc_indices = [i for i in doc_indices if i not in self.year_empty_index]
         self.allow_external_node = allow_external_node
 
@@ -84,8 +84,20 @@
         
         for dot_year_edge in dot_year_edge_list:
             dot_text += dot_year_edge
             
         for dot_edge in dot_edge_list:
             dot_text += dot_edge
         dot_text += '}'
-        return dot_text
+        return dot_text
+    
+    @staticmethod
+    def __extract_first_author(au_cell:str):
+        """提取一作"""
+        return au_cell.split(';',1)[0].replace(',','')
+    
+    def generate_graph_node_file(self)->pd.DataFrame:
+        use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
+        graph_node_table = self.citation_table.loc[self.node_list,use_cols]
+        graph_node_table['AU'] = graph_node_table['AU'].apply(self.__extract_first_author)
+        graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
+        return graph_node_table
```

### Comparing `histcite-python-0.0.1/histcite/parse_citation.py` & `histcite-python-0.1.1/histcite/parse_citation.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.0.1/histcite/process_table.py` & `histcite-python-0.1.1/histcite/process_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,22 @@
         self.file_name_list = [i for i in os.listdir(folder_path) if i[:4]=='save']
         
     def _read_table(self,file_name:str)->pd.DataFrame:
         """读取表单，返回dataframe"""
 
         use_cols = ['AU','TI','SO','DT','CR','DE','C3','NR','TC','Z9','J9','PY','VL','BP','DI','UT']
         file_path = os.path.join(self.folder_path,file_name)
-        single_df = pd.read_csv(
+        df = pd.read_csv(
             file_path,sep='\t',
             header=0,
             on_bad_lines='skip',
             usecols=use_cols,
             dtype_backend="pyarrow") # type: ignore
                               
-        return single_df
-    
-    @staticmethod
-    def __extract_first_author(au_field:str):
-        """提取一作"""
-        return au_field.split(';',1)[0].replace(',','')
+        return df
     
     def concat_table(self):
         """合并多个dataframe"""
 
         docs_table = pd.concat([self._read_table(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
         # 根据入藏号删除重复数据，一般不会有重复数据
         docs_table.drop_duplicates(subset='UT',ignore_index=True,inplace=True)
```

### Comparing `histcite-python-0.0.1/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.1.1/histcite_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.0.1
+Version: 0.1.1
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [Python](https://www.python.org/) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
@@ -43,69 +43,72 @@
 
 ```console
 $ python3 -m pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-
 ```console
-$ 下载的wos文件夹路径为 ~/downloads/wos，引文网络图包含的节点数为 100
-$ histcite -f ~/downloads/wos -n 100
+$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
 ```
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文关系图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx` 和 `graph.dot` 两个文件，前者是引文统计表，后者为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。  
+> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
 
 生成的引文网络图如下所示：
 <img src="examples/graph.svg">  
 
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](https://github.com/doublessay/histcite-python/blob/main/demo.ipynb)
+2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
+import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
-folder_path = '~/downloads/wos' # 下载的题录数据存放的文件夹路径
+folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path) # 读取并处理题录数据
 concated_table = process.concat_table() # 合并多个文件
 
-# 提取所有文献的参考文献, 参考 test/reference_table.xlsx
+# 提取所有文献的参考文献
 reference_table = process.generate_reference_table(concated_table['CR']) 
 
-# 识别引文关系, 参考 test/citation_table.xlsx
+# 识别引文关系
 citation_table = process.process_citation(reference_table) 
 
 # 各分析单元的引文统计
 cm = ComputeMetrics(citation_table, reference_table)
-cm.write2excel('~/downloads/wos/statistics.xlsx')
+cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(primary_table)
-doc_indices = primary_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-dot_text = graph.generate_dot_text(doc_indices, allow_external_node=False) # 生成引文网络图的数据文件
-
-# 根据需要保存图文件
-with open('~/downloads/wos/result/graph.dot', 'w') as f:
+graph = Graphviz(citation_table)
+doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
+
+# 生成引文网络图节点文件
+graph_node_file = graph.generate_graph_node_file()
+graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 > `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | - | - | - |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
-| 是否提供前端界面 | 否 | 是 |
 | 是否开源 | 是 | 否 |
+| 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
 - [ ] 支持 `scopus` 题录数据
 - [ ] 构建GUI页面
```

### Comparing `histcite-python-0.0.1/setup.py` & `histcite-python-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.0.1",
+    version="0.1.1",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=find_packages(),
```

### Comparing `histcite-python-0.0.1/test/test_parse_citation.py` & `histcite-python-0.1.1/test/test_parse_citation.py`

 * *Files identical despite different names*

