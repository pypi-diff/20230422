# Comparing `tmp/baiduspiderCreatedByHanXu-0.0.1.tar.gz` & `tmp/baiduspiderCreatedByHanXu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baiduspiderCreatedByHanXu-0.0.1.tar", last modified: Fri Apr 21 15:37:35 2023, max compression
+gzip compressed data, was "baiduspiderCreatedByHanXu-0.0.2.tar", last modified: Sat Apr 22 06:40:25 2023, max compression
```

## Comparing `baiduspiderCreatedByHanXu-0.0.1.tar` & `baiduspiderCreatedByHanXu-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.631669 baiduspiderCreatedByHanXu-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.617668 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:42:30.000000 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/__init__.py
--rw-rw-rw-   0        0        0     3874 2023-04-21 15:33:25.000000 baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/spider.py
--rw-rw-rw-   0        0        0     1090 2023-04-20 14:42:03.000000 baiduspiderCreatedByHanXu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1005 2023-04-21 15:37:35.630682 baiduspiderCreatedByHanXu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-21 12:48:11.000000 baiduspiderCreatedByHanXu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 15:37:35.627669 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     1005 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 15:37:35.000000 baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 15:37:35.631669 baiduspiderCreatedByHanXu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3212 2023-04-21 15:37:29.000000 baiduspiderCreatedByHanXu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:40:25.976893 baiduspiderCreatedByHanXu-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-22 06:40:25.961893 baiduspiderCreatedByHanXu-0.0.2/BaiduImageSpider/
+-rw-rw-rw-   0        0        0        0 2023-04-21 12:42:30.000000 baiduspiderCreatedByHanXu-0.0.2/BaiduImageSpider/__init__.py
+-rw-rw-rw-   0        0        0     3874 2023-04-21 15:33:25.000000 baiduspiderCreatedByHanXu-0.0.2/BaiduImageSpider/spider.py
+-rw-rw-rw-   0        0        0     1090 2023-04-20 14:42:03.000000 baiduspiderCreatedByHanXu-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1162 2023-04-22 06:40:25.975892 baiduspiderCreatedByHanXu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-04-22 06:13:40.000000 baiduspiderCreatedByHanXu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 06:40:25.972893 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     1162 2023-04-22 06:40:25.000000 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-22 06:40:25.000000 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 06:40:25.000000 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 06:40:25.000000 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-22 06:40:25.000000 baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 06:40:25.976893 baiduspiderCreatedByHanXu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3277 2023-04-22 06:40:12.000000 baiduspiderCreatedByHanXu-0.0.2/setup.py
```

### Comparing `baiduspiderCreatedByHanXu-0.0.1/BaiduImageSpider/spider.py` & `baiduspiderCreatedByHanXu-0.0.2/BaiduImageSpider/spider.py`

 * *Files identical despite different names*

### Comparing `baiduspiderCreatedByHanXu-0.0.1/LICENSE` & `baiduspiderCreatedByHanXu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baiduspiderCreatedByHanXu-0.0.1/PKG-INFO` & `baiduspiderCreatedByHanXu-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baiduspiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a project used to get a large number of images in Baidu.
 Home-page: https://gitee.com/UnderTurrets/baidu_image_spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -14,10 +14,17 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This is a project used to get a large number of images in Baidu.
+- use the following code to use the package
+```python
+from BaiduImageSpider import spider
+if __name__ == '__main__':
+    spider = spider.Spider_baidu_image()
+    spider()
+```
```

### Comparing `baiduspiderCreatedByHanXu-0.0.1/baiduspiderCreatedByHanXu.egg-info/PKG-INFO` & `baiduspiderCreatedByHanXu-0.0.2/baiduspiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baiduspiderCreatedByHanXu
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a project used to get a large number of images in Baidu.
 Home-page: https://gitee.com/UnderTurrets/baidu_image_spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -14,10 +14,17 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This is a project used to get a large number of images in Baidu.
+- use the following code to use the package
+```python
+from BaiduImageSpider import spider
+if __name__ == '__main__':
+    spider = spider.Spider_baidu_image()
+    spider()
+```
```

### Comparing `baiduspiderCreatedByHanXu-0.0.1/setup.py` & `baiduspiderCreatedByHanXu-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,20 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="baiduspiderCreatedByHanXu",
-    version="0.0.1",
+    version="0.0.2",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="This is a project used to get a large number of images in Baidu.",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://gitee.com/UnderTurrets/baidu_image_spider",
     packages=find_packages(),
 
     # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     # data_files=[
     #     ("", ["conf/*.conf"]),
     #     ("/usr/lib/systemd/system/", ["bin/*.service"]),
@@ -56,15 +57,15 @@
 
     # 不打包某些文件
     # exclude_package_data={
     #     "bandwidth_reporter":["*.txt"]
     #            },
 
     # 表明当前模块依赖哪些包，若环境中没有，则会从pypi中下载安装
-    install_requires=["requests",],
+    install_requires=["requests","urllib","os"],
 
     # setup.py 本身要依赖的包，这通常是为一些setuptools的插件准备的配置
     # 这里列出的包，不会自动安装。
     # setup_requires=["",],
 
     # 仅在测试时需要使用的依赖，在正常发布的代码中是没有用的。
     # 在执行python setup.py test时，可以自动安装这三个库，确保测试的正常运行。
```

