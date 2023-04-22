# Comparing `tmp/analysisbykwok-0.0.19.tar.gz` & `tmp/analysisbykwok-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.19.tar", last modified: Fri Apr 14 05:21:27 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.20.tar", last modified: Sat Apr 22 12:18:06 2023, max compression
```

## Comparing `analysisbykwok-0.0.19.tar` & `analysisbykwok-0.0.20.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/
--rw-rw-rw-   0        0        0       62 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.121441 analysisbykwok-0.0.19/analysisbykwok/
--rw-rw-rw-   0        0        0    16655 2023-04-14 05:21:04.000000 analysisbykwok-0.0.19/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-14 05:20:39.000000 analysisbykwok-0.0.19/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.124433 analysisbykwok-0.0.19/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-14 05:20:46.000000 analysisbykwok-0.0.19/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.914706 analysisbykwok-0.0.20/
+-rw-rw-rw-   0        0        0       62 2023-04-22 12:18:06.914706 analysisbykwok-0.0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.895002 analysisbykwok-0.0.20/analysisbykwok/
+-rw-rw-rw-   0        0        0    17204 2023-04-22 12:08:05.000000 analysisbykwok-0.0.20/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-22 12:05:02.000000 analysisbykwok-0.0.20/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-22 12:18:06.913710 analysisbykwok-0.0.20/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-22 12:18:06.000000 analysisbykwok-0.0.20/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2023-04-22 12:11:58.000000 analysisbykwok-0.0.20/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 12:18:06.915704 analysisbykwok-0.0.20/setup.cfg
```

### Comparing `analysisbykwok-0.0.19/analysisbykwok/__init__.py` & `analysisbykwok-0.0.20/analysisbykwok/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import pandas as pd
-import qstock as qs
 import requests
 import random
 import email
-import time
 import imaplib
-import os
+import re
 from email.header import decode_header
-import datetime
 import execjs
 import json
 import mimetypes
 import smtplib   # 发送邮件模块
 from email import encoders
 from email.mime.multipart import MIMEMultipart    # 使用MIMEMultipart来标示这个邮件是多个部分组成的
 from email.mime.base import MIMEBase
@@ -293,48 +290,57 @@
             # print("title:", title)
             get_att(msg, dir)
     def ProgressBar(i, sum, printvalue):
         sys.stdout.write('\r')
         sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100 + 1), ((int(i / sum * 100))) * '■',
                                               (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
         sys.stdout.flush()
-    def GetPlateSon(PlatNames):
-        input(
-            '调用说明：\n注意，调用之前需要下载qstock的库，并且在函数qs.ths_index_member中修改源代码，将page的值传进去\n确认无误回车即可执行')
-        num = 1
-        codes = []
-        names = []
-        while num != 0:
-            data = qs.ths_index_member(num, PlatNames)
-            if len(data['代码']) != 1:
-                codes = codes + data['代码'].T.values.tolist()
-                names = names + data['名称'].T.values.tolist()
-                num = num + 1
-            else:
-                num = 0
-        PlatInfo = {}
-        PlatInfo['代码'] = codes
-        PlatInfo['名称'] = names
-        return PlatInfo
-    def GetPlateInfo(PlateInfoName, url):
-        ApiCode=input('输入tushare的秘钥')
-        pro = ts.pro_api(ApiCode)
 
+    def GetPlateSon(num):
+        if num == '':
+            res = requests.get(r'https://hq.stock.sohu.com/pl/pl-1631.html?uid=1681655630543283qgz&548285357286').text
+            res = json.loads(
+                res.split('PEAK_ODIA(')[1].split(')</script>')[0].replace('\'pllist\',', '').replace('\'', '"'))
+            info = ''
+            for son in res:
+                info = info + son[1] + ':' + son[0] + '、'
+            print('请将所需板块的编号作为参数传入进来，具体信息如下：\n', info)
+            input('')
+        else:
+            res = requests.get(r'https://q.stock.sohu.com/cn/bk_' + num + '.shtml').text
+            res = res.split('</tbody>')[0].split('<tbody>')[1]
+            res1 = res
+            name = re.compile(r'>\d{6}<').findall(res1)
+            res = re.compile(r'>[\u4e00-\u9fa5]+<').findall(res)
+            '''>[\u4e00-\u9fa5]+<'''  # 匹配名称
+            result1 = []
+            for son in res:
+                result1.append(son.replace('\'', '').replace('>', '').replace('<', ''))
+            result2 = []
+            for son1 in name:
+                result2.append(son1.replace('\'', '').replace('>', '').replace('<', ''))
+            result = {}
+            result['代码'] = result2
+            result['名称'] = result1
+            return result
+    def GetPlateInfo(PlateInfoName, url):
         def FindCode(codes):
             result = []
             pro = ts.pro_api(ApiCode)
             data = pro.daily(ts_code='')
             data = data.sort_values(by='ts_code')
             data = data['ts_code'].T.values.tolist()
             for i in range(0, len(data)):
                 if data[i][:6] == codes:
                     result.append(data[i])
             return result
 
         a =function.GetPlateSon(PlateInfoName)
+        ApiCode=input('输入tushare的秘钥：')
+        pro = ts.pro_api(ApiCode)
         print('正在下载' + str(PlateInfoName) + '板块的股票信息')
         for i in range(0, len(a['代码'])):
             code = FindCode(a['代码'][i])
             for son in code:
                 data = pro.daily(ts_code=son)
                 data.to_csv(r'{}\{}-{}.csv'.format(url, a['名称'][i], a['代码'][i]))
                 function.ProgressBar(i, len(a['代码']), a['名称'][i])
```

