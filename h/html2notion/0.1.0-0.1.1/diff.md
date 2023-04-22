# Comparing `tmp/html2notion-0.1.0.tar.gz` & `tmp/html2notion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.0.tar", last modified: Fri Apr 21 05:19:42 2023, max compression
+gzip compressed data, was "html2notion-0.1.1.tar", last modified: Sat Apr 22 07:03:10 2023, max compression
```

## Comparing `html2notion-0.1.0.tar` & `html2notion-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.917884 html2notion-0.1.0/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.0/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3842 2023-04-21 05:19:42.918120 html2notion-0.1.0/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3353 2023-03-20 01:38:35.000000 html2notion-0.1.0/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.892447 html2notion-0.1.0/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.0/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2953 2023-04-20 02:54:09.000000 html2notion-0.1.0/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.906694 html2notion-0.1.0/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.0/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3181 2023-04-20 03:04:33.000000 html2notion-0.1.0/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.0/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2481 2023-04-20 11:03:46.000000 html2notion-0.1.0/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     8549 2023-04-21 02:54:02.000000 html2notion-0.1.0/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.0/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     8804 2023-04-21 02:35:36.000000 html2notion-0.1.0/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7030 2023-04-12 04:47:53.000000 html2notion-0.1.0/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2387 2023-04-21 02:20:28.000000 html2notion-0.1.0/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.912511 html2notion-0.1.0/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.0/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.0/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.0/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.0/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.896818 html2notion-0.1.0/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3842 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      875 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-21 05:19:42.000000 html2notion-0.1.0/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.0/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-21 05:19:42.919111 html2notion-0.1.0/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.0/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-21 05:19:42.916702 html2notion-0.1.0/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.0/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.0/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.0/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    15597 2023-04-20 11:59:35.000000 html2notion-0.1.0/tests/test_yinxiang.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.165860 html2notion-0.1.1/
+-rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.1/LICENSE
+-rw-r--r--   0 feizhao    (501) staff       (20)     4520 2023-04-22 07:03:10.166375 html2notion-0.1.1/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)     4031 2023-04-22 06:54:35.000000 html2notion-0.1.1/README.md
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.136957 html2notion-0.1.1/html2notion/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.1/html2notion/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2953 2023-04-20 14:39:58.000000 html2notion-0.1.1/html2notion/main.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.152382 html2notion-0.1.1/html2notion/translate/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.1/html2notion/translate/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3181 2023-04-20 14:39:58.000000 html2notion-0.1.1/html2notion/translate/batch_import.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.1/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2481 2023-04-20 14:39:58.000000 html2notion-0.1.1/html2notion/translate/html2json.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7894 2023-04-21 14:23:32.000000 html2notion-0.1.1/html2notion/translate/html2json_base.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      430 2023-04-19 23:45:05.000000 html2notion-0.1.1/html2notion/translate/html2json_default.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     8804 2023-04-21 14:23:32.000000 html2notion-0.1.1/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7030 2023-04-19 15:11:43.000000 html2notion-0.1.1/html2notion/translate/notion_export.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2387 2023-04-20 23:03:16.000000 html2notion-0.1.1/html2notion/translate/notion_import.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.159481 html2notion-0.1.1/html2notion/utils/
+-rw-r--r--   0 feizhao    (501) staff       (20)      427 2023-03-25 00:02:40.000000 html2notion-0.1.1/html2notion/utils/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      828 2023-03-22 13:58:21.000000 html2notion-0.1.1/html2notion/utils/load_config.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.1/html2notion/utils/log.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.1/html2notion/utils/timeutil.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.141466 html2notion-0.1.1/html2notion.egg-info/
+-rw-r--r--   0 feizhao    (501) staff       (20)     4520 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)      875 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      170 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/requires.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-04-22 07:03:10.000000 html2notion-0.1.1/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.1/pyproject.toml
+-rw-r--r--   0 feizhao    (501) staff       (20)      852 2023-04-22 07:03:10.168348 html2notion-0.1.1/setup.cfg
+-rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.1/setup.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-22 07:03:10.165006 html2notion-0.1.1/tests/
+-rw-r--r--   0 feizhao    (501) staff       (20)     2892 2023-04-20 14:39:58.000000 html2notion-0.1.1/tests/test_batchimport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.1/tests/test_cosupload.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.1/tests/test_notionexport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)    15597 2023-04-20 14:39:58.000000 html2notion-0.1.1/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.0/LICENSE` & `html2notion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/PKG-INFO` & `html2notion-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,106 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.0
+Version: 0.1.1
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-html2notion is a very useful Python library that allows you to import content from HTML documents into Notion notes, making it easier for you to organize information on the Notion platform. In addition, because html2notion is compatible with Evernote, you can also use it to export notes from Evernote to Notion.
+[简体中文](./README_zh.md)
 
-The html2notion library is very powerful and supports converting HTML files to various elements in Notion, such as text blocks, headings, images, code blocks, and more. These elements can be arranged and edited freely in Notion, which is very convenient.
+html2notion is an incredibly useful tool written in Python, which allows you to import content from HTML documents into Notion notes, making it more convenient for you to organize information on the Notion platform. In addition, html2notion has been specifically optimized for the content of Evernote, and you can also use it to import notes from Evernote into Notion.
 
-If you are looking for a way to better manage your notes and information and want to use the Notion platform, then the html2notion library is a great choice. You just need to install it and you can start converting HTML documents to Notion notes.
+html2notion has powerful features and supports converting various tags in HTML files into corresponding Blocks in Notion, such as rich text blocks, headings, images, code blocks, quotes, links, etc. Below are examples of converting notes from Evernote into Notion pages.
 
-# Installation
+![yinxiang notion(simple demos)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion.png)
 
-1. First, you need to install the html2notion library in your Python environment. You can use the pip command to install it:
+![yinxiang notion2(rich text)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion2.png)
+
+# Prepare
+
+You only need 3 steps to use htmlnotion to import HTML into Notion.
+
+## Duplicate database
+
+Click the link [notion template](https://selfboot.notion.site/selfboot/130bb48c6cbd4abbbb713d4d8472481a?v=ddda20d3f46b4b44a055d06792c142f0). As shown in the image below, use the "Duplicate" button to copy a new database to your own Notion workspace.
+
+![notion template](https://github.com/selfboot/html2notion/blob/master/demos/notion_templage.png)
+
+## Install html2notion
+
+Requires python>=3.8, install the html2notion library. You can use the pip command to install it:
 
 ```
 pip install html2notion
-
 ```
 
-# Usage
+## Prepare Notion Configuration
 
-## Get Notion parameters
+We need to use the `Notion API key` and `Database ID` to authorize html2notion to access the Notion database. Please follow these steps:
 
-To get a Notion API key, follow these steps:
+1. Create an integration;
+2. Share a database with your integration;
+3. Export the database ID;
 
-1. Log in to [Notion](https://www.notion.so/). If you don't have a Notion account yet, please register one first.
-2. Go to the [Notion Developer](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration) page.
-3. Click "My integrations".
-4. Click "New integration".
-5. Enter a name and click "Submit".
-6. Click "Add a client secret".
-7. Copy the generated API key to your code.
+When sharing the database here, you need to choose the previously duplicated database because the import operation requires some preset [properties](https://developers.notion.com/reference/property-object) information in this database.
 
-To authorize a Notion API key to access a database, follow these steps:
+For specific methods, please refer to the Notion official documentation [create an integration](https://developers.notion.com/docs/create-a-notion-integration).
 
-1. Go to the database you want to share with the API key.
-2. Click the three dots next to the database name.
-3. Now your API key will be able to access this database.
+After the setup is complete, write your API Key and database ID into a configuration file config.json.
 
-Note that in order for an API key to access a database, you must first add it as an integration to Notion. To add an integration, go to the Notion Developer page and follow the instructions. For more information, see Notion's API documentation: [Notion API Docs](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration).
+```shell
+{
+    "notion": {
+        "database_id": "<***demo***>",
+        "api_key": "<***demo***>"
+    }
+}
+```
 
-To get the ID of a Notion database, follow these steps:
+# Usage
 
-1. Go to the Notion database you want to import HTML into.
-2. Click the three dots next to the database name.
-3. Select "Properties".
-4. Hover over the column where you want to import HTML and click the three dots next to the column name.
-5. Click "Property settings".
-6. Copy the database ID to your code.
+You can use `html2notion -h` to view detailed help documentation.
 
-## Tencent Cloud COS key
+```shell
+usage: html2notion [-h] --conf CONF [--log LOG] [--batch BATCH] (--file FILE | --dir DIR)
 
-## Evernote migration
+Html2notion: Save HTML to your Notion notes quickly and easily, while keeping the original format as much as possible
 
-If you want to import notes from Evernote into Notion, you can use Evernote's export function to export notes as HTML files and then use the above command to import them into Notion.
+options:
+  -h, --help     show this help message and exit
+  --conf CONF    conf file path
+  --log LOG      log direct path
+  --batch BATCH  batch save concurrent limit
+  --file FILE    Save single html file to notion
+  --dir DIR      Save all html files in the dir to notion
+```
 
-# Supported HTML elements
+For example, if you want to import all html files in the `./demos` directory into Notion, you can use the following command:
 
-The following is a list of HTML elements supported by html2notion:
+```shell
+html2notion --conf config.json --dir ./demos --log ~/logs --batch 10
+```
 
-- `p`
-- `h1`, `h2`, `h3`, `h4`, `h5`, `h6`
-- `ul`, `ol`
-- `li`
-- `a`
-- `img`
-- `code`
-- `blockquote`
-- `hr`
-- `br`
+The above command will import all html files in the `./demos` directory into Notion, while outputting logs to the `~/logs` directory, with up to 10 concurrent tasks.
 
 # More information
 
 You can find more information and examples in the html2notion library's Issue: [html2notion](https://github.com/selfboot/html2notion/issues)
 
 ## Contribution
 
-If you find any errors or have any improvement suggestions, please do not hesitate to submit a pull request or issue. We are happy to accept your contributions and feedback!
+If you find any errors or have any suggestions for improvement, please do not hesitate to submit a pull request or raise an issue, I am more than happy to accept your contributions and feedback!
+
+If you encounter import failures, you can submit the html file and log file together in the issue for easier problem identification.
+
+> If there are any private information in the files, please remove it first.
+
 
 ## License
 
-This project uses the MIT license. Please refer to the LICENSE file for details.
+This project uses the MIT license. Please refer to the [LICENSE](./LICENSE) for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `html2notion-0.1.0/README.md` & `html2notion-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,93 @@
-html2notion is a very useful Python library that allows you to import content from HTML documents into Notion notes, making it easier for you to organize information on the Notion platform. In addition, because html2notion is compatible with Evernote, you can also use it to export notes from Evernote to Notion.
+[简体中文](./README_zh.md)
 
-The html2notion library is very powerful and supports converting HTML files to various elements in Notion, such as text blocks, headings, images, code blocks, and more. These elements can be arranged and edited freely in Notion, which is very convenient.
+html2notion is an incredibly useful tool written in Python, which allows you to import content from HTML documents into Notion notes, making it more convenient for you to organize information on the Notion platform. In addition, html2notion has been specifically optimized for the content of Evernote, and you can also use it to import notes from Evernote into Notion.
 
-If you are looking for a way to better manage your notes and information and want to use the Notion platform, then the html2notion library is a great choice. You just need to install it and you can start converting HTML documents to Notion notes.
+html2notion has powerful features and supports converting various tags in HTML files into corresponding Blocks in Notion, such as rich text blocks, headings, images, code blocks, quotes, links, etc. Below are examples of converting notes from Evernote into Notion pages.
 
-# Installation
+![yinxiang notion(simple demos)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion.png)
 
-1. First, you need to install the html2notion library in your Python environment. You can use the pip command to install it:
+![yinxiang notion2(rich text)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion2.png)
+
+# Prepare
+
+You only need 3 steps to use htmlnotion to import HTML into Notion.
+
+## Duplicate database
+
+Click the link [notion template](https://selfboot.notion.site/selfboot/130bb48c6cbd4abbbb713d4d8472481a?v=ddda20d3f46b4b44a055d06792c142f0). As shown in the image below, use the "Duplicate" button to copy a new database to your own Notion workspace.
+
+![notion template](https://github.com/selfboot/html2notion/blob/master/demos/notion_templage.png)
+
+## Install html2notion
+
+Requires python>=3.8, install the html2notion library. You can use the pip command to install it:
 
 ```
 pip install html2notion
-
 ```
 
-# Usage
+## Prepare Notion Configuration
 
-## Get Notion parameters
+We need to use the `Notion API key` and `Database ID` to authorize html2notion to access the Notion database. Please follow these steps:
 
-To get a Notion API key, follow these steps:
+1. Create an integration;
+2. Share a database with your integration;
+3. Export the database ID;
 
-1. Log in to [Notion](https://www.notion.so/). If you don't have a Notion account yet, please register one first.
-2. Go to the [Notion Developer](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration) page.
-3. Click "My integrations".
-4. Click "New integration".
-5. Enter a name and click "Submit".
-6. Click "Add a client secret".
-7. Copy the generated API key to your code.
+When sharing the database here, you need to choose the previously duplicated database because the import operation requires some preset [properties](https://developers.notion.com/reference/property-object) information in this database.
 
-To authorize a Notion API key to access a database, follow these steps:
+For specific methods, please refer to the Notion official documentation [create an integration](https://developers.notion.com/docs/create-a-notion-integration).
 
-1. Go to the database you want to share with the API key.
-2. Click the three dots next to the database name.
-3. Now your API key will be able to access this database.
+After the setup is complete, write your API Key and database ID into a configuration file config.json.
 
-Note that in order for an API key to access a database, you must first add it as an integration to Notion. To add an integration, go to the Notion Developer page and follow the instructions. For more information, see Notion's API documentation: [Notion API Docs](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration).
+```shell
+{
+    "notion": {
+        "database_id": "<***demo***>",
+        "api_key": "<***demo***>"
+    }
+}
+```
 
-To get the ID of a Notion database, follow these steps:
+# Usage
 
-1. Go to the Notion database you want to import HTML into.
-2. Click the three dots next to the database name.
-3. Select "Properties".
-4. Hover over the column where you want to import HTML and click the three dots next to the column name.
-5. Click "Property settings".
-6. Copy the database ID to your code.
+You can use `html2notion -h` to view detailed help documentation.
 
-## Tencent Cloud COS key
+```shell
+usage: html2notion [-h] --conf CONF [--log LOG] [--batch BATCH] (--file FILE | --dir DIR)
 
-## Evernote migration
+Html2notion: Save HTML to your Notion notes quickly and easily, while keeping the original format as much as possible
 
-If you want to import notes from Evernote into Notion, you can use Evernote's export function to export notes as HTML files and then use the above command to import them into Notion.
+options:
+  -h, --help     show this help message and exit
+  --conf CONF    conf file path
+  --log LOG      log direct path
+  --batch BATCH  batch save concurrent limit
+  --file FILE    Save single html file to notion
+  --dir DIR      Save all html files in the dir to notion
+```
 
-# Supported HTML elements
+For example, if you want to import all html files in the `./demos` directory into Notion, you can use the following command:
 
-The following is a list of HTML elements supported by html2notion:
+```shell
+html2notion --conf config.json --dir ./demos --log ~/logs --batch 10
+```
 
-- `p`
-- `h1`, `h2`, `h3`, `h4`, `h5`, `h6`
-- `ul`, `ol`
-- `li`
-- `a`
-- `img`
-- `code`
-- `blockquote`
-- `hr`
-- `br`
+The above command will import all html files in the `./demos` directory into Notion, while outputting logs to the `~/logs` directory, with up to 10 concurrent tasks.
 
 # More information
 
 You can find more information and examples in the html2notion library's Issue: [html2notion](https://github.com/selfboot/html2notion/issues)
 
 ## Contribution
 
-If you find any errors or have any improvement suggestions, please do not hesitate to submit a pull request or issue. We are happy to accept your contributions and feedback!
+If you find any errors or have any suggestions for improvement, please do not hesitate to submit a pull request or raise an issue, I am more than happy to accept your contributions and feedback!
+
+If you encounter import failures, you can submit the html file and log file together in the issue for easier problem identification.
+
+> If there are any private information in the files, please remove it first.
+
 
 ## License
 
-This project uses the MIT license. Please refer to the LICENSE file for details.
+This project uses the MIT license. Please refer to the [LICENSE](./LICENSE) for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `html2notion-0.1.0/html2notion/main.py` & `html2notion-0.1.1/html2notion/main.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/batch_import.py` & `html2notion-0.1.1/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/cos_uploader.py` & `html2notion-0.1.1/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/html2json.py` & `html2notion-0.1.1/html2notion/translate/html2json.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/html2json_base.py` & `html2notion-0.1.1/html2notion/translate/html2json_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,85 +61,60 @@
             if value
         }
 
     @staticmethod
     def generate_link(**kwargs):
         if not kwargs.get("plain_text", ""):
             return
-        text_obj = {}
-        text_obj["href"] = kwargs.get("url", "")
-        text_obj["plain_text"] = kwargs.get("plain_text", "")
-        text_obj["text"] = {}
-        text_obj["text"]["link"] = {}
-        text_obj["text"]["link"]["url"] = kwargs.get("url", "")
-        text_obj["text"]["content"] = kwargs.get("plain_text", "")
-        text_obj["type"] = "text"
-        return text_obj
+        return {
+            "href": kwargs.get("url", ""),
+            "plain_text": kwargs.get("plain_text", ""),
+            "text": {
+                "link": {"url": kwargs.get("url", "")},
+                "content": kwargs.get("plain_text", "")
+            },
+            "type": "text"
+        }
 
     @staticmethod
     def generate_text(**kwargs):
-        if not kwargs.get("plain_text", ""):
+        plain_text = kwargs.get("plain_text", "")
+        if not plain_text:
             return
-        text_obj = {}
-        text_obj["plain_text"] = kwargs.get("plain_text", "")
-        text_obj["text"] = {}
-        text_obj["text"]["content"] = kwargs.get("plain_text", "")
-        text_obj["annotations"] = {}
-        for key, value in kwargs.items():
-            if key == "plain_text" or key not in Html2JsonBase._text_annotations:
-                continue
-            if not isinstance(value, Html2JsonBase._text_annotations[key]):
-                logger.warn(f"Invalid annotation: {key}={value}")
-            text_obj["annotations"][key] = value
-        if not text_obj["annotations"]:
-            del text_obj["annotations"]
-        text_obj["type"] = "text"
+        annotations = {
+            key: value
+            for key, value in kwargs.items()
+            if key in Html2JsonBase._text_annotations and isinstance(value, Html2JsonBase._text_annotations[key])
+        }
+        text_obj = {
+            "plain_text": plain_text,
+            "text": {"content": plain_text},
+            "type": "text"
+        }
+        if annotations:
+            text_obj["annotations"] = annotations
+
         return text_obj
 
-    # properties = {
-    # "Title": {
-    #     "title": [
-    #         {
-    #             "text": {
-    #                 "content": "Tuscan Kale"
-    #             }
-    #         }
-    #     ]
-    # }}
     @staticmethod
     def generate_properties(**kwargs):
-        properties_obj = {}
         title = kwargs.get("title", "")
-        properties_obj["Title"] = {
-            "title": [{"text": {"content": title}}]
-        }
-
         url = kwargs.get("url", "")
-        if url:
-            properties_obj["URL"] = {
-                "url": url,
-                "type": "url"
-            }
-
         tags = kwargs.get("tags", [])
-        if tags:
-            properties_obj["Tags"] = {
-                "type": "multi_select",
-                "multi_select": [
-                    {"name": tag} for tag in tags]
-            }
-
         created_time = kwargs.get("created_time", "")
-        if created_time:
-            properties_obj["Created"] = {
-                "date": {
-                    "start": created_time
-                },
-                "type": "date"
-            }
+
+        property_map = {
+            "Title": {"title": [{"text": {"content": title}}]} if title else None,
+            "URL": {"url": url, "type": "url"} if url else None,
+            "Tags": {"type": "multi_select", "multi_select": [{"name": tag} for tag in tags]} if tags else None,
+            "Created": {"date": {"start": created_time}, "type": "date"} if created_time else None,
+        }
+
+        properties_obj = {key: value for key, value in property_map.items() if value is not None}
+
         logger.debug(f"properties: {properties_obj}")
         return properties_obj
 
     @staticmethod
     def is_same_annotations_text(text_one: dict, text_another: dict):
         if text_one["type"] != "text" or text_another["type"] != "text":
             return False
```

### Comparing `html2notion-0.1.0/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.1/html2notion/translate/html2json_yinxiang.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/notion_export.py` & `html2notion-0.1.1/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/translate/notion_import.py` & `html2notion-0.1.1/html2notion/translate/notion_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/utils/load_config.py` & `html2notion-0.1.1/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion/utils/log.py` & `html2notion-0.1.1/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.1/html2notion.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,106 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.0
+Version: 0.1.1
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-html2notion is a very useful Python library that allows you to import content from HTML documents into Notion notes, making it easier for you to organize information on the Notion platform. In addition, because html2notion is compatible with Evernote, you can also use it to export notes from Evernote to Notion.
+[简体中文](./README_zh.md)
 
-The html2notion library is very powerful and supports converting HTML files to various elements in Notion, such as text blocks, headings, images, code blocks, and more. These elements can be arranged and edited freely in Notion, which is very convenient.
+html2notion is an incredibly useful tool written in Python, which allows you to import content from HTML documents into Notion notes, making it more convenient for you to organize information on the Notion platform. In addition, html2notion has been specifically optimized for the content of Evernote, and you can also use it to import notes from Evernote into Notion.
 
-If you are looking for a way to better manage your notes and information and want to use the Notion platform, then the html2notion library is a great choice. You just need to install it and you can start converting HTML documents to Notion notes.
+html2notion has powerful features and supports converting various tags in HTML files into corresponding Blocks in Notion, such as rich text blocks, headings, images, code blocks, quotes, links, etc. Below are examples of converting notes from Evernote into Notion pages.
 
-# Installation
+![yinxiang notion(simple demos)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion.png)
 
-1. First, you need to install the html2notion library in your Python environment. You can use the pip command to install it:
+![yinxiang notion2(rich text)](https://github.com/selfboot/html2notion/blob/master/demos/yinxiang_notion2.png)
+
+# Prepare
+
+You only need 3 steps to use htmlnotion to import HTML into Notion.
+
+## Duplicate database
+
+Click the link [notion template](https://selfboot.notion.site/selfboot/130bb48c6cbd4abbbb713d4d8472481a?v=ddda20d3f46b4b44a055d06792c142f0). As shown in the image below, use the "Duplicate" button to copy a new database to your own Notion workspace.
+
+![notion template](https://github.com/selfboot/html2notion/blob/master/demos/notion_templage.png)
+
+## Install html2notion
+
+Requires python>=3.8, install the html2notion library. You can use the pip command to install it:
 
 ```
 pip install html2notion
-
 ```
 
-# Usage
+## Prepare Notion Configuration
 
-## Get Notion parameters
+We need to use the `Notion API key` and `Database ID` to authorize html2notion to access the Notion database. Please follow these steps:
 
-To get a Notion API key, follow these steps:
+1. Create an integration;
+2. Share a database with your integration;
+3. Export the database ID;
 
-1. Log in to [Notion](https://www.notion.so/). If you don't have a Notion account yet, please register one first.
-2. Go to the [Notion Developer](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration) page.
-3. Click "My integrations".
-4. Click "New integration".
-5. Enter a name and click "Submit".
-6. Click "Add a client secret".
-7. Copy the generated API key to your code.
+When sharing the database here, you need to choose the previously duplicated database because the import operation requires some preset [properties](https://developers.notion.com/reference/property-object) information in this database.
 
-To authorize a Notion API key to access a database, follow these steps:
+For specific methods, please refer to the Notion official documentation [create an integration](https://developers.notion.com/docs/create-a-notion-integration).
 
-1. Go to the database you want to share with the API key.
-2. Click the three dots next to the database name.
-3. Now your API key will be able to access this database.
+After the setup is complete, write your API Key and database ID into a configuration file config.json.
 
-Note that in order for an API key to access a database, you must first add it as an integration to Notion. To add an integration, go to the Notion Developer page and follow the instructions. For more information, see Notion's API documentation: [Notion API Docs](https://developers.notion.com/docs/getting-started#step-2-share-a-database-with-your-integration).
+```shell
+{
+    "notion": {
+        "database_id": "<***demo***>",
+        "api_key": "<***demo***>"
+    }
+}
+```
 
-To get the ID of a Notion database, follow these steps:
+# Usage
 
-1. Go to the Notion database you want to import HTML into.
-2. Click the three dots next to the database name.
-3. Select "Properties".
-4. Hover over the column where you want to import HTML and click the three dots next to the column name.
-5. Click "Property settings".
-6. Copy the database ID to your code.
+You can use `html2notion -h` to view detailed help documentation.
 
-## Tencent Cloud COS key
+```shell
+usage: html2notion [-h] --conf CONF [--log LOG] [--batch BATCH] (--file FILE | --dir DIR)
 
-## Evernote migration
+Html2notion: Save HTML to your Notion notes quickly and easily, while keeping the original format as much as possible
 
-If you want to import notes from Evernote into Notion, you can use Evernote's export function to export notes as HTML files and then use the above command to import them into Notion.
+options:
+  -h, --help     show this help message and exit
+  --conf CONF    conf file path
+  --log LOG      log direct path
+  --batch BATCH  batch save concurrent limit
+  --file FILE    Save single html file to notion
+  --dir DIR      Save all html files in the dir to notion
+```
 
-# Supported HTML elements
+For example, if you want to import all html files in the `./demos` directory into Notion, you can use the following command:
 
-The following is a list of HTML elements supported by html2notion:
+```shell
+html2notion --conf config.json --dir ./demos --log ~/logs --batch 10
+```
 
-- `p`
-- `h1`, `h2`, `h3`, `h4`, `h5`, `h6`
-- `ul`, `ol`
-- `li`
-- `a`
-- `img`
-- `code`
-- `blockquote`
-- `hr`
-- `br`
+The above command will import all html files in the `./demos` directory into Notion, while outputting logs to the `~/logs` directory, with up to 10 concurrent tasks.
 
 # More information
 
 You can find more information and examples in the html2notion library's Issue: [html2notion](https://github.com/selfboot/html2notion/issues)
 
 ## Contribution
 
-If you find any errors or have any improvement suggestions, please do not hesitate to submit a pull request or issue. We are happy to accept your contributions and feedback!
+If you find any errors or have any suggestions for improvement, please do not hesitate to submit a pull request or raise an issue, I am more than happy to accept your contributions and feedback!
+
+If you encounter import failures, you can submit the html file and log file together in the issue for easier problem identification.
+
+> If there are any private information in the files, please remove it first.
+
 
 ## License
 
-This project uses the MIT license. Please refer to the LICENSE file for details.
+This project uses the MIT license. Please refer to the [LICENSE](./LICENSE) for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `html2notion-0.1.0/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.1/html2notion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/setup.cfg` & `html2notion-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.0
+version = 0.1.1
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.0/tests/test_batchimport.py` & `html2notion-0.1.1/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/tests/test_cosupload.py` & `html2notion-0.1.1/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/tests/test_notionexport.py` & `html2notion-0.1.1/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.0/tests/test_yinxiang.py` & `html2notion-0.1.1/tests/test_yinxiang.py`

 * *Files identical despite different names*

