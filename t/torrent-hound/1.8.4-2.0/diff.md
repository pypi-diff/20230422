# Comparing `tmp/torrent-hound-1.8.4.tar.gz` & `tmp/torrent-hound-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torrent-hound-1.8.4.tar", last modified: Mon Jul  5 02:52:01 2021, max compression
+gzip compressed data, was "torrent-hound-2.0.tar", last modified: Sat Apr 22 01:15:39 2023, max compression
```

## Comparing `torrent-hound-1.8.4.tar` & `torrent-hound-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2862 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/PKG-INFO
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2862 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/PKG-INFO
--rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/SOURCES.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/requires.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/top_level.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/torrent_hound.egg-info/dependency_links.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-1.8.4/MANIFEST.in
--rw-r--r--   0 yashovardhan   (501) staff       (20)      807 2021-07-05 02:47:14.000000 torrent-hound-1.8.4/setup.py
--rwxr--r--   0 yashovardhan   (501) staff       (20)    48912 2021-07-05 02:45:42.000000 torrent-hound-1.8.4/torrent-hound
--rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2021-07-05 02:52:01.000000 torrent-hound-1.8.4/setup.cfg
--rw-r--r--   0 yashovardhan   (501) staff       (20)     1976 2018-12-11 21:30:12.000000 torrent-hound-1.8.4/README.rst
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:15:39.585668 torrent-hound-2.0/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-2.0/MANIFEST.in
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:15:39.584923 torrent-hound-2.0/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     1976 2018-12-11 21:30:12.000000 torrent-hound-2.0/README.rst
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2023-04-22 01:15:39.585858 torrent-hound-2.0/setup.cfg
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      828 2023-04-22 01:13:10.000000 torrent-hound-2.0/setup.py
+-rwxr--r--   0 yashovardhan   (501) staff       (20)    52365 2023-04-22 01:14:00.000000 torrent-hound-2.0/torrent-hound
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:15:39.501730 torrent-hound-2.0/torrent_hound.egg-info/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:15:37.000000 torrent-hound-2.0/torrent_hound.egg-info/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2023-04-22 01:15:39.000000 torrent-hound-2.0/torrent_hound.egg-info/SOURCES.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:15:37.000000 torrent-hound-2.0/torrent_hound.egg-info/dependency_links.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2023-04-22 01:15:38.000000 torrent-hound-2.0/torrent_hound.egg-info/requires.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:15:38.000000 torrent-hound-2.0/torrent_hound.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `torrent-hound-1.8.4/PKG-INFO` & `torrent-hound-2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,76 @@
-Metadata-Version: 1.0
-Name: torrent-hound
-Version: 1.8.4
-Summary: Search torrents from multiple websites via the CLI
-Home-page: https://github.com/baddymaster/torrent-hound
-Author: Yashovardhan Sharma
-Author-email: yashovardhan@tuta.io
-License: AGPL-3.0
-Description: Torrent Hound
-        =============
-        
-        Search torrents from multiple websites via the CLI
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        -  Python 2.7
-        -  bs4
-        -  clint
-        -  pyperclip
-        -  humanize
-        -  VeryPrettyTable
-        -  cfscrape
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        Install package and dependencies directly via pip using
-        ``pip install torrent-hound``
-        
-        Or run ``pip install -r requirements.txt`` in the shell to install all
-        dependencies
-        
-        Update existing Intallation
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To upgrade ``torrent-hound`` via pip, run
-        ``pip install torrent-hound -U``
-        
-        If installed via ``git``, then simply run ``git pull`` in the shell
-        after navigating to the ``torrent-hound`` directory
-        
-        Otherwise download the latest binary from the ``releases`` section of
-        this repository
-        
-        Usage
-        ~~~~~
-        
-        If installed via pip, ``torrent-hound`` would have been added to
-        ``$PATH``. Simply run ``torrent-hound`` or
-        ``torrent-hound [search-query]`` to begin.
-        
-        Download the ``torrent-hound`` binary from the ``bin/`` directory.
-        
-        ``torrent-hound [search-query]`` or simply ``torrent-hound``
-        
-        Menu
-        ~~~~
-        
-        Available Commands :
-        
-        1. ``m<result number>`` - Print magnet link of selected torrent
-        2. ``c<result number>`` - Copy magnet link of selected torrent to
-           clipboard
-        3. ``d<result number>`` - Download torrent using default torrent client
-        4. ``o<result number>`` - Open the torrent page of the selected torrent
-           in the default browser
-        5. ``cs<result number>`` - Copy magnet link and open Seedr.cc
-        6. ``p<optional choice>`` - Print top 10 results from each website for
-           the given query
-        
-           ``<choice>`` : [{default : 1}, {0 : Print formatted result}, {1 :
-           Pretty print results}]
-        7. ``s`` - Enter a new query to search for over all avilable torrent
-           websites
-        8. ``r`` - Repeat last search (with same query)
-        
-        Help
-        ~~~~
-        
-        In case of an ``SSL Error``, consult `these answers on Stackoverflow`_
-        for potential fixes.
-        
-        .. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
-Platform: UNKNOWN
+Torrent Hound
+=============
+
+Search torrents from multiple websites via the CLI
+
+Requirements
+~~~~~~~~~~~~
+
+-  Python 2.7
+-  bs4
+-  clint
+-  pyperclip
+-  humanize
+-  VeryPrettyTable
+-  cfscrape
+
+Installation
+~~~~~~~~~~~~
+
+Install package and dependencies directly via pip using
+``pip install torrent-hound``
+
+Or run ``pip install -r requirements.txt`` in the shell to install all
+dependencies
+
+Update existing Intallation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To upgrade ``torrent-hound`` via pip, run
+``pip install torrent-hound -U``
+
+If installed via ``git``, then simply run ``git pull`` in the shell
+after navigating to the ``torrent-hound`` directory
+
+Otherwise download the latest binary from the ``releases`` section of
+this repository
+
+Usage
+~~~~~
+
+If installed via pip, ``torrent-hound`` would have been added to
+``$PATH``. Simply run ``torrent-hound`` or
+``torrent-hound [search-query]`` to begin.
+
+Download the ``torrent-hound`` binary from the ``bin/`` directory.
+
+``torrent-hound [search-query]`` or simply ``torrent-hound``
+
+Menu
+~~~~
+
+Available Commands :
+
+1. ``m<result number>`` - Print magnet link of selected torrent
+2. ``c<result number>`` - Copy magnet link of selected torrent to
+   clipboard
+3. ``d<result number>`` - Download torrent using default torrent client
+4. ``o<result number>`` - Open the torrent page of the selected torrent
+   in the default browser
+5. ``cs<result number>`` - Copy magnet link and open Seedr.cc
+6. ``p<optional choice>`` - Print top 10 results from each website for
+   the given query
+
+   ``<choice>`` : [{default : 1}, {0 : Print formatted result}, {1 :
+   Pretty print results}]
+7. ``s`` - Enter a new query to search for over all avilable torrent
+   websites
+8. ``r`` - Repeat last search (with same query)
+
+Help
+~~~~
+
+In case of an ``SSL Error``, consult `these answers on Stackoverflow`_
+for potential fixes.
+
+.. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
```

### Comparing `torrent-hound-1.8.4/torrent_hound.egg-info/PKG-INFO` & `torrent-hound-2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,86 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: torrent-hound
-Version: 1.8.4
+Version: 2.0
 Summary: Search torrents from multiple websites via the CLI
 Home-page: https://github.com/baddymaster/torrent-hound
 Author: Yashovardhan Sharma
-Author-email: yashovardhan@tuta.io
+Author-email: yash.s@tuta.io
 License: AGPL-3.0
-Description: Torrent Hound
-        =============
-        
-        Search torrents from multiple websites via the CLI
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        -  Python 2.7
-        -  bs4
-        -  clint
-        -  pyperclip
-        -  humanize
-        -  VeryPrettyTable
-        -  cfscrape
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        Install package and dependencies directly via pip using
-        ``pip install torrent-hound``
-        
-        Or run ``pip install -r requirements.txt`` in the shell to install all
-        dependencies
-        
-        Update existing Intallation
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To upgrade ``torrent-hound`` via pip, run
-        ``pip install torrent-hound -U``
-        
-        If installed via ``git``, then simply run ``git pull`` in the shell
-        after navigating to the ``torrent-hound`` directory
-        
-        Otherwise download the latest binary from the ``releases`` section of
-        this repository
-        
-        Usage
-        ~~~~~
-        
-        If installed via pip, ``torrent-hound`` would have been added to
-        ``$PATH``. Simply run ``torrent-hound`` or
-        ``torrent-hound [search-query]`` to begin.
-        
-        Download the ``torrent-hound`` binary from the ``bin/`` directory.
-        
-        ``torrent-hound [search-query]`` or simply ``torrent-hound``
-        
-        Menu
-        ~~~~
-        
-        Available Commands :
-        
-        1. ``m<result number>`` - Print magnet link of selected torrent
-        2. ``c<result number>`` - Copy magnet link of selected torrent to
-           clipboard
-        3. ``d<result number>`` - Download torrent using default torrent client
-        4. ``o<result number>`` - Open the torrent page of the selected torrent
-           in the default browser
-        5. ``cs<result number>`` - Copy magnet link and open Seedr.cc
-        6. ``p<optional choice>`` - Print top 10 results from each website for
-           the given query
-        
-           ``<choice>`` : [{default : 1}, {0 : Print formatted result}, {1 :
-           Pretty print results}]
-        7. ``s`` - Enter a new query to search for over all avilable torrent
-           websites
-        8. ``r`` - Repeat last search (with same query)
-        
-        Help
-        ~~~~
-        
-        In case of an ``SSL Error``, consult `these answers on Stackoverflow`_
-        for potential fixes.
-        
-        .. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
-Platform: UNKNOWN
+Requires-Python: >=3
+
+Torrent Hound
+=============
+
+Search torrents from multiple websites via the CLI
+
+Requirements
+~~~~~~~~~~~~
+
+-  Python 2.7
+-  bs4
+-  clint
+-  pyperclip
+-  humanize
+-  VeryPrettyTable
+-  cfscrape
+
+Installation
+~~~~~~~~~~~~
+
+Install package and dependencies directly via pip using
+``pip install torrent-hound``
+
+Or run ``pip install -r requirements.txt`` in the shell to install all
+dependencies
+
+Update existing Intallation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To upgrade ``torrent-hound`` via pip, run
+``pip install torrent-hound -U``
+
+If installed via ``git``, then simply run ``git pull`` in the shell
+after navigating to the ``torrent-hound`` directory
+
+Otherwise download the latest binary from the ``releases`` section of
+this repository
+
+Usage
+~~~~~
+
+If installed via pip, ``torrent-hound`` would have been added to
+``$PATH``. Simply run ``torrent-hound`` or
+``torrent-hound [search-query]`` to begin.
+
+Download the ``torrent-hound`` binary from the ``bin/`` directory.
+
+``torrent-hound [search-query]`` or simply ``torrent-hound``
+
+Menu
+~~~~
+
+Available Commands :
+
+1. ``m<result number>`` - Print magnet link of selected torrent
+2. ``c<result number>`` - Copy magnet link of selected torrent to
+   clipboard
+3. ``d<result number>`` - Download torrent using default torrent client
+4. ``o<result number>`` - Open the torrent page of the selected torrent
+   in the default browser
+5. ``cs<result number>`` - Copy magnet link and open Seedr.cc
+6. ``p<optional choice>`` - Print top 10 results from each website for
+   the given query
+
+   ``<choice>`` : [{default : 1}, {0 : Print formatted result}, {1 :
+   Pretty print results}]
+7. ``s`` - Enter a new query to search for over all avilable torrent
+   websites
+8. ``r`` - Repeat last search (with same query)
+
+Help
+~~~~
+
+In case of an ``SSL Error``, consult `these answers on Stackoverflow`_
+for potential fixes.
+
+.. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
```

### Comparing `torrent-hound-1.8.4/setup.py` & `torrent-hound-2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='torrent-hound',          # This is the name of your PyPI-package.
-    version='1.8.4',                 # Update the version number for new releases
+    version='2.0',                 # Update the version number for new releases
     scripts=['torrent-hound'],     # The name of your scipt, and also the command you'll be using for calling it
     description='Search torrents from multiple websites via the CLI',
     long_description=readme(),
+    python_requires = '>=3',
     url='https://github.com/baddymaster/torrent-hound',
     install_requires=[
         'bs4',
         'requests',
         'clint',
         'pyperclip',
         'humanize',
         'VeryPrettyTable',
         'cfscrape'
     ],
     author='Yashovardhan Sharma',
-    author_email='yashovardhan@tuta.io',
+    author_email='yash.s@tuta.io',
     license='AGPL-3.0',
 )
```

### Comparing `torrent-hound-1.8.4/torrent-hound` & `torrent-hound-2.0/torrent-hound`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # @author : Yashovardhan Sharma
 # @github : github.com/baddymaster
 
 #   <Torrent Hound - Search torrents from multiple websites via the CLI.>
-#    Copyright (C) <2017>  <Yashovardhan Sharma>
+#    Copyright (C) <2023>  <Yashovardhan Sharma>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as published
 #     by the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 #
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import print_function
+from builtins import input
+from builtins import str
 from bs4 import BeautifulSoup
 from datetime import datetime, timedelta
 from clint.textui import colored
 from veryprettytable import VeryPrettyTable
 import requests
 import re
 import sys
@@ -30,17 +33,19 @@
 import json
 import humanize
 import traceback
 import random
 import time
 import argparse
 import cfscrape as cfs
+import traceback
 
 defaultQuery, query = 'jason bourne', ''
 results_sky = None
+results_tpb_condensed = None
 results_tpb_api, num_results_tpb_api = None, 0
 results, results_rarbg, exit, error_detected_rarbg, error_detected_tpb = None, None, None, None, None
 num_results, num_results_rarbg, num_results_sky, print_version = 0, 0, 0, 1
 auth_token = 'None'
 app_id = 'None'
 tpb_working_domain = 'tpb.tw'
 rarbg_url, skytorrents_url, tpb_url = '', '', ''
@@ -83,74 +88,88 @@
                     SIZE_DESC = 'sd',
                     SIZE_ASC = 'sa',
                     NEWEST = 'ad',
                     OLDEST = 'aa')
 
 def generateNewTorrentAPIToken(error=False, quiet_mode=False):
     global auth_token, error_detected_rarbg, app_id
+    
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
+    headers_safari = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Safari/605.1.15'}
     refresh_url = 'https://torrentapi.org/pubapi_v2.php?get_token=get_token&app_id=' + str(app_id)
+    
+    #print(f"App ID: {app_id}")
+    #print(f"Token Refresh URL: {refresh_url}")
     try:
-        r = requests.get(refresh_url, headers=headers)
+        r = requests.get(refresh_url, headers=headers_safari)
         if(str(r).split()[1][1:4] != '200'):
             if quiet_mode == False:
-                print colored.red("HTTP Response Error : %s" % str(r))
+                print(colored.red("HTTP Response Error : %s" % str(r)))
             error_detected_rarbg = True
             return error_detected_rarbg
 
-        auth_token = json.loads(r.text)['token'].encode('utf-8')
-        #print auth_token
+        auth_token = json.loads(r.text)['token']
+        #print(f"Auth Token: {auth_token}")
+
         if error != False:
             success_string = '[RARBG] Success : Generated new token! '
             if quiet_mode == False:
-                print colored.blue(success_string)
-    except requests.exceptions.ConnectionError, e:
+                print(colored.blue(success_string))
+    except requests.exceptions.ConnectionError as e:
         err_string = str(e).split(',')[0]
         if 'Connection aborted' in err_string:
             if quiet_mode == False:
-                print colored.red("Server cannot be reached. Check Internet connectivity!")
+                print(colored.red("Server cannot be reached. Check Internet connectivity!"))
             #sys.exit(1)
     
     #except SysCallError, e:
     #    print colored.red("SysCallError for RARBG search. Fix?")
 
 def searchRarbg(search_string=defaultQuery, quiet_mode=False):
     global auth_token, results_rarbg, error_detected_rarbg, app_id, rarbg_url
     # API Documentaion : https://torrentapi.org/apidocs_v2.txt
     # https://torrentapi.org/pubapi_v2.php?mode=search&search_string=Suits%20S06E10&format=json_extended&ranked=0&token=7dib9orxpa&app_id=0
     # echo 'torrent-hound' | shasum -a 512
     generateNewTorrentAPIToken(quiet_mode=quiet_mode)
-    #print auth_token
+    #print(f"Auth Token: {auth_token}")
     if error_detected_rarbg == True:
         #print "Error detected!\n"
         return results_rarbg
 
+    #print(f"Auth token: {auth_token.decode('utf-8')}\n")
     search_string = search_string.replace(" ", "%20")
-    base_url = 'http://torrentapi.org/pubapi_v2.php?'
+    base_url = 'https://torrentapi.org/pubapi_v2.php?'
     new_token = 'get_token=get_token&app_id=' + str(app_id)
     search_criteria = 'mode=search&search_string=' + search_string + "&"
-    options = 'format=json_extended&ranked=0&token=' + auth_token + '&app_id=' + str(app_id)
+    options = 'format=json_extended&ranked=0&token=' + str(auth_token) + '&app_id=' + str(app_id)
     url = base_url + search_criteria + options
     rarbg_url = url
-    #print url
+    #print(f"RARBG Search URL: {url}")
+
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X x.y; rv:42.0) Gecko/20100101 Firefox/42.0'}
-    
+    # User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Safari/605.1.15
+    headers_safari = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Safari/605.1.15'}
+
     try:
-        response = requests.get(url, headers=headers)
-        #print response
+        response = requests.get(url, headers=headers_safari)
+        #print(f"Response: {response}")
         rt = response.text
-        #print rt
+        #print(f"Response Text: {rt}\n")
         response_json = json.loads(rt)
         #print response_json
-    except ValueError, e:
+    except Exception as e:
         if quiet_mode == False:
-            print colored.red('[RARBG] Error : ' + str(e))
             status_code = str(response).split()[1].strip('<[]>')
             if status_code == '429': # Too Many Requests
-                print colored.yellow('<HTTP 429> : Too Many Requests. Please try again after a while!')
+                print(colored.yellow('<HTTP 429> : Too Many Requests. Please try again after a while!'))
+                print(colored.red('[RARBG] Error : ' + str(e)))
+            else:
+                print(colored.red('[RARBG] Error : ' + str(e)))
+            #traceback.print_exc()
+            
         return []
     results_rarbg = []
 
     error_detected_rarbg = checkResponseForErrors(response_json, quiet_mode=quiet_mode)
     if(error_detected_rarbg == False):
         results_rarbg = parse_results_rarbg(response_json, quiet_mode=quiet_mode)
     return results_rarbg
@@ -159,15 +178,15 @@
     global results_rarbg, error_detected_rarbg, query, auth_token
     search_string = query.replace(" ", "%20")
 
     if 'error_code' in response_json:
         #print 'In function'
         error_string = '[RARBG] Error : ' + response_json['error']
         if quiet_mode == False:
-            print colored.magenta(error_string)
+            print(colored.magenta(error_string))
         
         if response_json['error_code'] == 4:
             generateNewTorrentAPIToken(error=True)
             results_rarbg = searchRarbg(search_string)
         # elif response_json['error_code'] == 20:
         #     print "No results found. Try different keywords!\n"
         return True #Some error detected
@@ -198,63 +217,63 @@
                 res['ratio'] = format( (float(res['seeders'])/float(res['leechers'])), '.1f' )
             except ZeroDivisionError:
                 res['ratio'] = 'inf'
             res['magnet'] = post['download']
             results_rarbg.append(res)
     else:
         if quiet_mode == False:
-            print "----------- " + colored.green('RARBG') + " -----------"
-            print "             [No results found]                "
+            print("----------- " + colored.green('RARBG') + " -----------")
+            print("             [No results found]                ")
         return []
     return results_rarbg
 
 def print_top_results_rarbg(limit=10):
     global results_rarbg
     if results_rarbg != [] and results_rarbg != None:
-        print '\n---------------------------------------------- ' + colored.green('RARBG') + ' ----------------------------------------------'
-        print '{0} {1} {2} {3} {4} {5}'.format(colored.red('No.').ljust(3), colored.red('Torrent Name').ljust(60), colored.red('File Size').rjust(10), colored.red('Seeders').rjust(7), colored.red('Leechers').rjust(6), colored.red('Ratio').rjust(6))
+        print('\n---------------------------------------------- ' + colored.green('RARBG') + ' ----------------------------------------------')
+        print('{0} {1} {2} {3} {4} {5}'.format(colored.red('No.').ljust(3), colored.red('Torrent Name').ljust(60), colored.red('File Size').rjust(10), colored.red('Seeders').rjust(7), colored.red('Leechers').rjust(6), colored.red('Ratio').rjust(6)))
         index = 1
         for r in results_rarbg[:limit]:
-            print '{0} {1} {2} {3} {4} {5}'.format(str(index).ljust(3), r['name'][:60].ljust(60), r['size'].rjust(10), str(r['seeders']).rjust(6), str(r['leechers']).rjust(6), str(r['ratio']).rjust(8))
+            print('{0} {1} {2} {3} {4} {5}'.format(str(index).ljust(3), r['name'][:60].ljust(60), r['size'].rjust(10), str(r['seeders']).rjust(6), str(r['leechers']).rjust(6), str(r['ratio']).rjust(8)))
             index = index + 1
-        print "---------------------------------------------------------------------------------------------------"
+        print("---------------------------------------------------------------------------------------------------")
         return index - 1
 
 def pretty_print_top_results_rarbg(limit=10):
     global results_rarbg
     table_rarbg = VeryPrettyTable(left_padding_width=0, right_padding_width=0, padding_width=0)
     no_str = str(colored.red('No'))
     name_str = str(colored.red('Torrent Name'))
     size_str = str(colored.red('Size'))
     seed_str = str(colored.red('S'))
     leech_str = str(colored.red('L'))
     ratio_str = str(colored.red('S/L'))
     table_rarbg.field_names = [no_str, name_str, size_str, seed_str, leech_str, ratio_str]
 
-    print '\n\t\t\t\t\t\t' + colored.green('RARBG')
+    print('\n\t\t\t\t\t\t' + colored.green('RARBG'))
     if (results_rarbg != []) and (results_rarbg != None):
         #print 'Empty table'
         #print '{0} {1} {2} {3} {4} {5}'.format(colored.red('No.').ljust(3), colored.red('Torrent Name').ljust(60), colored.red('File Size').rjust(10), colored.red('Seeders').rjust(7), colored.red('Leechers').rjust(6), colored.red('Ratio').rjust(6))
         index = 1
         for r in results_rarbg[:limit]:
             table_rarbg.add_row([index, r['name'][:57], r['size'], r['seeders'], r['leechers'], r['ratio']])
             #print '{0} {1} {2} {3} {4} {5}'.format(str(index).ljust(3), r['name'][:60].ljust(60), r['size'].rjust(10), str(r['seeders']).rjust(6), str(r['leechers']).rjust(6), str(r['ratio']).rjust(8))
             index = index + 1
         table_rarbg.align[no_str] = 'l'
         table_rarbg.align[name_str] = 'l'
         table_rarbg.align[size_str] = 'r'
         table_rarbg.align[seed_str] = 'r'
         table_rarbg.align[leech_str] = 'r'
         table_rarbg.align[ratio_str] = 'r'
-        print table_rarbg
+        print(table_rarbg)
         return index - 1
     else:
         table_rarbg.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
         table_rarbg.align[colored.red('Torrent Name')] = 'l'
-        print table_rarbg
+        print(table_rarbg)
         return 0
 
 def searchSkyTorrents(search_string=defaultQuery, domain='skytorrents.lol', order_by=ORDER_BY_SKY.RELEVANCE, quiet_mode=False, limit=10):
     global results_sky, skytorrents_url
     search_string = removeAndReplaceSpaces(search_string)
     baseURL = 'https://' + domain
     url = baseURL + '/?query=' + search_string
@@ -273,16 +292,16 @@
 
         trows = tbody.findAll("tr")
         #print len(trows)
         for trow in trows[:limit]:
             res = {}
             tds = trow.findAll("td")
             #tds[0] -> Name, Magnet, Link
-            res['name'] = tds[0].findAll("a")[0].contents[0].encode('utf-8')
-            res['link'] = baseURL + '/' + tds[0].findAll("a")[0].attrs['href'].encode('utf-8')
+            res['name'] = tds[0].findAll("a")[0].contents[0]
+            res['link'] = baseURL + '/' + tds[0].findAll("a")[0].attrs['href']
 
             if tds[0].findAll("img")[0].attrs['src'] == '/files/thumb_upm.png' and tds[0].findAll("img")[1].attrs['src'] == '/files/thumb_downm.png':
                 # Both upvotes and downvotes found
                 res['up'] = '{:+}'.format(int(tds[0].contents[2]))
                 res['down'] = '{:+}'.format(int(tds[0].contents[4]))
             elif tds[0].findAll("img")[0].attrs['src'] == '/files/thumb_upm.png':
                 # Only upvotes, no downvotes found
@@ -293,38 +312,39 @@
                 res['up'] = '0'
                 res['down'] = '{:+}'.format(int(tds[0].contents[2]))
             else:
                 # No upvotes or downvotes found
                 res['up'] = '0'
                 res['down'] = '0'
             
-            res['magnet'] = tds[0].findAll("a")[2].attrs['href'].encode('utf-8')
+            res['magnet'] = tds[0].findAll("a")[2].attrs['href']
             #tds[1] -> Size
             res['size'] = tds[1].contents[0].encode('utf-8')
             #tds[2] -> No. of files
             # res['num_files'] = tds[0].contents[0].encode('utf-8')
             #tds[3] -> Date added
             # res['date'] = tds[3].contents[0].encode('utf-8')
             #tds[4] -> Seeders
-            res['seeders'] = tds[4].contents[0].encode('utf-8').replace(',', '')
+            res['seeders'] = tds[4].contents[0].replace(',', '')
             #tds[5] -> Leechers
-            res['leechers'] = tds[5].contents[0].encode('utf-8').replace(',', '')
+            res['leechers'] = tds[5].contents[0].replace(',', '')
             try:
                 res['ratio'] = format( (float(res['seeders'])/float(res['leechers'])), '.1f' )
             except ZeroDivisionError:
                 res['ratio'] = 'inf'
             results_sky.append(res)
 
-    except Exception, e:
+    except Exception as e:
         if quiet_mode == False:
             if tbody == None:
-                print colored.magenta("[SkyTorrents] Error : No results found")    
+                print(colored.magenta("[SkyTorrents] Error : No results found"))    
             else:
-                print colored.red("[SkyTorrents] Error : Unkown problem while searching")
-                print colored.yellow('ERR_MSG : ' + str(e))
+                print(colored.red("[SkyTorrents] Error : Unkown problem while searching"))
+                print(colored.yellow('ERR_MSG : ' + str(e)))
+                #traceback.print_exc()
 
     return results_sky
 
 def removeAndReplaceSpaces(string):
     if string[0] == " ":
         string = string[1:]
     return string.replace(" ", "+")
@@ -339,43 +359,88 @@
     leech_str = str(colored.red('L'))
     ratio_str = str(colored.red('S/L'))
     votes_str = str(colored.red('Votes'))
     table_skytorrents.field_names = [no_str, name_str, size_str, seed_str, leech_str, ratio_str, votes_str]
 
     #print '\n\t\t\t\t\t\t' + '+-----------+'
     #print '\t\t\t\t\t\t| ' + colored.green('PirateBay') + ' |'
-    print '\n\t\t\t\t\t\t' + colored.green('Sky Torrents')
+    print('\n\t\t\t\t\t\t' + colored.green('Sky Torrents'))
     # print results
     if results_sky != [{}] and results_sky != [] and results_sky != None:
         #index = num_results_tpb_api + 1
         index = num_results + 1
         for r in results_sky[:limit]:
             try :
-                table_skytorrents.add_row([index, r['name'][:57], r['size'], r['seeders'], r['leechers'], r['ratio'], (r['up'] + '/' + r['down'])])
+                table_skytorrents.add_row([index, r['name'][:57], r['size'].decode('utf-8'), r['seeders'], r['leechers'], r['ratio'], (r['up'] + '/' + r['down'])])
                 index = index + 1
-            except KeyError, e:
+            except KeyError as e:
                 # Fix error where {} is included in results and screws up numbering #
                 if r != {}:
-                    print r
-                    print e
+                    print(r)
+                    print(e)
         table_skytorrents.align[no_str] = 'l'
         table_skytorrents.align[name_str] = 'l'
         table_skytorrents.align[size_str] = 'r'
         table_skytorrents.align[seed_str] = 'r'
         table_skytorrents.align[leech_str] = 'r'
         table_skytorrents.align[ratio_str] = 'r'
         table_skytorrents.align[votes_str] = 'c'
-        print table_skytorrents
+        print(table_skytorrents)
         return index - 1
     else:
         table_skytorrents.add_row(["Null", "Null", "Null", "Null", "Null", "Null", "Null"])
         #table_piratebay.align[colored.red('Torrent Name')] = 'l'
-        print table_skytorrents
+        print(table_skytorrents)
         return num_results
 
+def searchPirateBayCondensed(search_string=defaultQuery, page=0, order_by=ORDER_BY.SEEDERS, domain='thepiratebay.org', quiet_mode=False, limit=10):
+    global tpb_working_domain, tpb_url, results_tpb_condensed
+    url = f'https://{tpb_working_domain}/s/?q={removeAndReplaceSpaces(search_string)}&page=0&orderby=99'
+    tpb_url = url
+    #print url
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
+    table = None
+
+    try:
+        r = requests.get(url, headers=headers)
+        soup = BeautifulSoup(r.content, "html.parser")
+        table = soup.find("table", {"id": "searchResult"})
+        trs = table.findAll("tr")
+        del trs[:1]
+
+        results_tpb_condensed = []
+        #for tr in trs:
+        for tr in trs[:limit]:
+            tds = tr.findAll("td")
+
+            res = {}
+            link_name = tds[1].find("a", {"class": "detLink"})
+            res['name'] = link_name.contents[0].strip()
+            res['link'] = link_name["href"]
+            res['seeders'] = int(tds[2].contents[0])
+            res['leechers'] = int(tds[3].contents[0])
+            try:
+                res['ratio'] = format( (float(res['seeders'])/float(res['leechers'])), '.1f' )
+            except ZeroDivisionError:
+                res['ratio'] = 'inf'
+            res['magnet'] = tds[1].find("img", {"alt": "Magnet link"}).parent['href']
+            res['size'] = str(tds[1].find("font").contents[0].split(',')[1].split(' ')[2].replace('\xa0', ' '))
+
+            results_tpb_condensed.append(res)
+    except Exception as e:
+        if quiet_mode == False:
+            if table == None:
+                print(colored.magenta("[PirateBay] Error : No results found"))
+            else:
+                print(colored.red("[PirateBay] Error : Unkown problem while searching"))
+                print(colored.yellow('ERR_MSG : ' + str(e)))
+                #table = None
+    #print(f"Search results TBP: {results_tpb_condensed}")
+    return results_tpb_condensed
+
 def searchPirateBay(search_string = defaultQuery, page = 0, order_by = ORDER_BY.UPLOADER, domain = 'thepiratebay.org', quiet_mode=False):
     """
     Searches for the given string in The Pirate Bay.
     Returns a list of dictionaries with the information of each torrent.
     """
     global tpb_working_domain, tpb_url
     baseURL = 'https://' + domain + '/s/?q='
@@ -385,79 +450,79 @@
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
     try:
         r = requests.get(url, headers=headers)
         soup = BeautifulSoup(r.content, "html.parser")
         table = soup.find("table", {"id": "searchResult"})
         # print "TBP Response : \n"
         # print r.content
-    except requests.exceptions.ConnectionError, e:
+    except requests.exceptions.ConnectionError as e:
         #print e
         err_string = str(e).split(',')[2]
         #print err_string
         if 'Operation timed out' in err_string:
             if domain == 'thepiratebay.org':
                 tpb_working_domain = alternate_domain ='piratebay.red'
                 error_str = colored.yellow("[PirateBay] Error : Connection to ") + colored.magenta(domain) + colored.yellow(" timed out.\n")
                 error_str += colored.yellow("Trying to connect via ") + colored.magenta(alternate_domain) + colored.yellow("...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 return searchPirateBay(search_string=search_string, domain='piratebay.red')
             elif domain == 'piratebay.red':
                 error_str = colored.yellow("[PirateBay] Error : Connection to ") + colored.magenta(domain) + colored.yellow(" timed out.\n")
                 error_str += colored.red("Exiting. Try connecting via a proxy...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 table = None
                 #sys.exit(1)
         elif 'Connection refused' in err_string:
             if domain == 'thepiratebay.org':
                 tpb_working_domain = alternate_domain = 'piratebay.red'
                 error_str = colored.red("[PirateBay] Error : Connection to ") + (domain) + colored.red(" refused.\n")
                 error_str += colored.red("Trying to connect via ") + (alternate_domain) + colored.red("...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 return searchPirateBay(search_string=search_string, domain='piratebay.red')
             elif domain == 'piratebay.red':
                 error_str = colored.red("[PirateBay] Error : Connection to ") + (domain) + colored.red(" refused.\n")
                 error_str += colored.red("Exiting. Try connecting via a proxy...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 table = None
                 #sys.exit(1)
         elif 'failed to respond' in err_string:
             if domain == 'thepiratebay.org':
                 tpb_working_domain = alternate_domain = 'piratebay.red'
                 error_str = colored.red("[PirateBay] Error : Connection to ") + (domain) + colored.red(" is probably blocked.\n")
                 error_str += colored.red("Trying to connect via ") + (alternate_domain) + colored.red("...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 return searchPirateBay(search_string=search_string, domain='piratebay.red')
             elif domain == 'piratebay.red':
                 error_str = colored.red("[PirateBay] Error : Connection to ") + (domain) + colored.red(" refused.\n")
                 error_str += colored.red("Exiting. Try connecting via a proxy...")
                 if quiet_mode == False:
-                    print error_str
+                    print(error_str)
                 table = None
                 #sys.exit(1)
         else:
             error_str = colored.red("[PirateBay] Unhandled Error : ") + colored.red(str(e)) + colored.red("\nExiting...")
             if quiet_mode == False:
-                print error_str
+                print(error_str)
             table = None
             #sys.exit(1)
-    except TypeError, e:
+    except TypeError as e:
         #print("Something's wrong...")
         table = None
 
     # print table
     if table == None:
         if domain == 'piratebay.red':
             error_string = str(colored.yellow('[PirateBay] Error : No results found. ')) + str(colored.magenta(domain)) + str(colored.yellow(' might be unreachable!'))
             if quiet_mode == False:
-                print error_string
+                print(error_string)
             return _parse_search_result_table(table, quiet_mode)
         else:
             tpb_working_domain = alternate_domain = 'piratebay.red'
             # print "!!!!"
             error_string = str(colored.yellow('[PirateBay] Error  : No results found. ')) + str(colored.magenta(domain)) + str(colored.yellow(' might be unreachable!'))
             error_string += str(colored.yellow('\nTrying ')) + str(colored.magenta(alternate_domain)) + str(colored.yellow('...'))
             if quiet_mode == False:
@@ -482,15 +547,15 @@
         #print tr
         index += 1
         if(error_detected_tpb == False):
             results.append(_parse_search_result_table_row(tr))
         else:
             error_string = '[PirateBay] Error  : No results found'
             if quiet_mode == False:
-                print colored.yellow(error_string)
+                print(colored.yellow(error_string))
             break
     return results
 
 def _parse_search_result_table_row(tr):
     global error_detected_tpb, tpb_working_domain
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
     
@@ -511,28 +576,28 @@
         m = re.search(r"^Uploaded (Today|Y-day|\d\d-\d\d)\xc2\xa0(\d{4}|\d\d:\d\d), " + r"Size (\d+(?:.\d*)?\xc2\xa0(?:[KMG]iB))", desc_string)
         try :
             temp_size = str(m.group(3)).replace('\xc2\xa0', ' ')
             s1 = temp_size.split('.')
             #print s1
             try:
                 s2 = s1[1].split(' ')
-            except IndexError, e: # Special case where size is an integer (eg. s1 = 2 GiB), i.e, no decimal place
+            except IndexError as e: # Special case where size is an integer (eg. s1 = 2 GiB), i.e, no decimal place
                 #print 'Reached here'
                 s1 = s1[0].split(' ')
                 #print s1
                 s2 = ['0']
                 s2.append(s1[1])
                 temp_size = s1[0] + '.0 ' + s1[1]
             if(len(s1[0]) == 4):
                 res['size'] = s1[0] + s2[1]
             elif(len(s1[0]) == 3):
                 res['size'] = s1[0] + '.' + s2[0][0] + " " + s2[1]
             else:
                 res['size'] = temp_size
-        except AttributeError, e:
+        except AttributeError as e:
             #print 'Reached here next'
             error_detected_tpb = True
             #print e
             #print "\nRegex misbehaving. Try running the script again!\n"
             return {}
         now = datetime.today()
         if re.match(r"\d{4}", m.group(2)) == None:
@@ -565,17 +630,17 @@
             magnet_link_page = 'https://' + tpb_working_domain + res['link']
             #print magnet_link_page
             try:
                 magnet_req = requests.get(magnet_link_page, headers=headers)
                 soup2 = BeautifulSoup(magnet_req.content, "html.parser")
                 content = soup2.find_all(class_='download')
                 res['magnet'] = content[0].contents[1].attrs['href'].encode('utf-8')
-            except Exception, e:
-                print colored.red("[PirateBay] Error : Unkown problem while searching for magnet link")
-                print colored.yellow('ERR_MSG : ' + str(e))
+            except Exception as e:
+                print(colored.red("[PirateBay] Error : Unkown problem while searching for magnet link"))
+                print(colored.yellow('ERR_MSG : ' + str(e)))
         #print res
         return res
 
 def searchPirateBayWithAPI(search_string = defaultQuery, sort_by = SORT_BY_TBP.SEEDS_DESC, domain = 'tpbc.herokuapp.com', quiet_mode=False):
     global results_tpb_api, tpb_url
     base_url = 'https://' + domain
     url = base_url + '/search/' + removeAndReplaceSpaces(search_string) + '/?sort=' + sort_by
@@ -583,18 +648,18 @@
 
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
     
     try:
         response = requests.get(url, headers=headers)
         response_json = json.loads(response.text)
         results_tpb_api = parse_results_tpb_api(response_json, quiet_mode=quiet_mode)
-    except Exception, e:
+    except Exception as e:
         if quiet_mode == False :
-            print colored.red("[PirateBay] : Error while searching")
-            print colored.yellow('ERR_MSG : ' + str(e))
+            print(colored.red("[PirateBay] : Error while searching"))
+            print(colored.yellow('ERR_MSG : ' + str(e)))
         #traceback.print_exc()
     
     # try:
     #     results_tpb_api = parse_results_tpb_api(response_json)
     # except Exception, e:
     #     print colored.red("[PirateBay] : Error while parsing search results.")
     #     print colored.yellow('ERR_MSG : ' + str(e))
@@ -603,15 +668,15 @@
 
 def parse_results_tpb_api(response_json, quiet_mode=False):
     #global results_tpb_api
     results_list = []
     if response_json == []:
         if quiet_mode == False:
             error_string = '[PirateBay] Error : No results found'
-            print colored.magenta(error_string)
+            print(colored.magenta(error_string))
         return []
     else:
         for post in response_json:
             res = {}
             res['name'] = post['title'].encode('utf-8')
             #res['link'] = ''
 
@@ -631,115 +696,115 @@
             res['magnet'] = post['magnet'].encode('utf-8')
             results_list.append(res)
     
     return results_list
 
 def getQuery():
     global query
-    query = raw_input('Enter search query : ')
+    query = input('Enter search query : ')
     return query
 
 def print_top_results(limit=10):
     global results
     if results != [{}]:
-        print '-------------------------------------------- ' + colored.green('PirateBay') + ' --------------------------------------------'
-        print '{0} {1} {2} {3} {4} {5}'.format(colored.red('No.').ljust(3), colored.red('Torrent Name').ljust(60), colored.red('File Size').rjust(10), colored.red('Seeders').rjust(7), colored.red('Leechers').rjust(6), colored.red('Ratio').rjust(6))
+        print('-------------------------------------------- ' + colored.green('PirateBay') + ' --------------------------------------------')
+        print('{0} {1} {2} {3} {4} {5}'.format(colored.red('No.').ljust(3), colored.red('Torrent Name').ljust(60), colored.red('File Size').rjust(10), colored.red('Seeders').rjust(7), colored.red('Leechers').rjust(6), colored.red('Ratio').rjust(6)))
         index = num_results_rarbg + 1
         for r in results[:limit]:
-            print '{0} {1} {2} {3} {4} {5}'.format(str(index).ljust(3), r['name'][:60].ljust(60), r['size'].rjust(11), str(r['seeders']).rjust(6), str(r['leechers']).rjust(6), str(r['ratio']).rjust(8))
+            print('{0} {1} {2} {3} {4} {5}'.format(str(index).ljust(3), r['name'][:60].ljust(60), r['size'].rjust(11), str(r['seeders']).rjust(6), str(r['leechers']).rjust(6), str(r['ratio']).rjust(8)))
             index = index + 1
-        print "---------------------------------------------------------------------------------------------------"
+        print("---------------------------------------------------------------------------------------------------")
         return index - 1
 
 def pretty_print_top_results_piratebay(limit=10):
     global results, num_results_rarbg
     table_piratebay = VeryPrettyTable(left_padding_width=0, right_padding_width=0, padding_width=0)
     no_str = str(colored.red('No'))
     name_str = str(colored.red('Torrent Name'))
     size_str = str(colored.red('Size'))
     seed_str = str(colored.red('S'))
     leech_str = str(colored.red('L'))
     ratio_str = str(colored.red('S/L'))
     table_piratebay.field_names = [no_str, name_str, size_str, seed_str, leech_str, ratio_str]
 
-    print '\n\t\t\t\t\t\t' + colored.green('PirateBay')
+    print('\n\t\t\t\t\t\t' + colored.green('PirateBay'))
     # print results
     if results != [{}] and results != [] and results != None:
         index = num_results_rarbg + 1
         #print index
         #print len(results)
         for r in results[:limit]:
             try :
                 #print index
                 #print r
                 table_piratebay.add_row([index, r['name'][:57], r['size'], r['seeders'], r['leechers'], r['ratio']])
                 index = index + 1
-            except KeyError, e:
+            except KeyError as e:
                 # Fix error where {} is included in results and screws up numbering #
                 if r != {}:
-                    print r
-                    print e
+                    print(r)
+                    print(e)
         table_piratebay.align[no_str] = 'l'
         table_piratebay.align[name_str] = 'l'
         table_piratebay.align[size_str] = 'r'
         table_piratebay.align[seed_str] = 'r'
         table_piratebay.align[leech_str] = 'r'
         table_piratebay.align[ratio_str] = 'r'
-        print table_piratebay
+        print(table_piratebay)
         return index - 1
     else:
         table_piratebay.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
         #table_piratebay.align[colored.red('Torrent Name')] = 'l'
-        print table_piratebay
+        print(table_piratebay)
         return num_results_rarbg
 
 def pretty_print_top_results_piratebay_api(limit=10):
     global results_tpb_api, num_results_rarbg
     table_piratebay = VeryPrettyTable(left_padding_width=0, right_padding_width=0, padding_width=0)
     no_str = str(colored.red('No'))
     name_str = str(colored.red('Torrent Name'))
     size_str = str(colored.red('Size'))
     seed_str = str(colored.red('S'))
     leech_str = str(colored.red('L'))
     ratio_str = str(colored.red('S/L'))
     table_piratebay.field_names = [no_str, name_str, size_str, seed_str, leech_str, ratio_str]
 
-    print '\n\t\t\t\t\t\t' + colored.green('PirateBay')
+    print('\n\t\t\t\t\t\t' + colored.green('PirateBay'))
     if results_tpb_api != [] and results_tpb_api != None:
         index = num_results_rarbg + 1
         for r in results_tpb_api[:limit]:
             try :
                 table_piratebay.add_row([index, r['name'][:57], r['size'], r['seeders'], r['leechers'], r['ratio']])
                 index = index + 1
-            except KeyError, e:
+            except KeyError as e:
                 # Fix error where {} is included in results and screws up numbering #
                 if r != {}:
-                    print r
-                    print e
+                    print(r)
+                    print(e)
         table_piratebay.align[no_str] = 'l'
         table_piratebay.align[name_str] = 'l'
         table_piratebay.align[size_str] = 'r'
         table_piratebay.align[seed_str] = 'r'
         table_piratebay.align[leech_str] = 'r'
         table_piratebay.align[ratio_str] = 'r'
-        print table_piratebay
+        print(table_piratebay)
         return index - 1
     else:
         table_piratebay.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
         #table_piratebay.align[colored.red('Torrent Name')] = 'l'
-        print table_piratebay
+        print(table_piratebay)
         return num_results_rarbg
 
 def switch(arg, tpb_api=False):
     global results, exit, defaultQuery, num_results, query, num_results_rarbg, results_rarbg, print_version, tpb_working_domain, results_tpb_api, num_results_tpb_api, rarbg_url, skytorrents_url, tpb_url
     if ('c' in arg) and ('s' not in arg) and ('z' not in arg):
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command!\n'
+                print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
@@ -748,22 +813,22 @@
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
                         mLink = results_sky[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
-                print 'Magnet link copied to clipboard!'
+                print('Magnet link copied to clipboard!')
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif ('cs' in arg) and ('z' not in arg):
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command!\n'
+                print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
@@ -773,22 +838,22 @@
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
                         mLink = results_sky[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
                 webbrowser.open('https://www.seedr.cc', new=2)
-                print 'Seedr.cc opened and Magnet link copied to clipboard!'
+                print('Seedr.cc opened and Magnet link copied to clipboard!')
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif 'cz' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command!\n'
+                print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
@@ -798,22 +863,22 @@
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
                         mLink = results_sky[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
                 webbrowser.open('https://zbigz.unihax.in/', new=2)
-                print 'zbigz opened and Magnet link copied to clipboard!'
+                print('zbigz opened and Magnet link copied to clipboard!')
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif 'm' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command\n'
+                print('Invalid command\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
@@ -821,22 +886,22 @@
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
                         mLink = results_sky[(resNum-1)-num_results]['magnet']
-                print "\nMagnet Link : \n" + mLink
+                print("\nMagnet Link : \n" + mLink)
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif 'd' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command!\n'
+                print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
@@ -845,24 +910,23 @@
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
                         mLink = results_sky[(resNum-1)-num_results]['magnet']
                 webbrowser.open(mLink, new=2)
-                print 'Magnet link sent to default torrent client!'
+                print('Magnet link sent to default torrent client!')
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif 'o' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            #re.search('r\d+', 'r1').group()
             #print("resNum : %d" % resNum)
             if resNum <= 0 or resNum > num_results_sky:
-                print 'Invalid command!\n'
+                print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         tLink = results_rarbg[resNum-1]['link']
                         #print("resNum(%d) <= num_results_rarbg(%d)" % (resNum, results_rarbg))
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         tLink = "https://" + tpb_working_domain + results_tpb_api[(resNum-1)-num_results_rarbg]['link']
@@ -872,87 +936,87 @@
                         #print("Reached SkyTorrents. Link : %s" % tLink)
                 else:
                     if resNum <= num_results_rarbg :
                         tLink = results_rarbg[resNum-1]['link']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         #tLink = "https://" + tpb_working_domain + results[(resNum-1)-num_results_rarbg]['link']
                         tLink = results[(resNum-1)-num_results_rarbg]['link']
-                        #print(tLink)
                     else:
                         tLink = results_sky[(resNum-1)-num_results]['link']
                 #webbrowser.get('chrome').open(tLink, new=2)
                 webbrowser.open(tLink, new=2)
-                print 'Torrent page opened in default browser!'
+                print('Torrent page opened in default browser!')
         except AttributeError:
-            print 'Enter a valid torrent number as well!'
+            print('Enter a valid torrent number as well!')
     elif arg == 'u':
-        print colored.green('[RARBG] URL') + ' : ' + rarbg_url
-        print colored.green('[PirateBay] URL') + ' : ' + tpb_url
-        print colored.green('[SkyTorrents] URL') + ' : ' + skytorrents_url
+        print(colored.green('[RARBG] URL') + ' : ' + rarbg_url)
+        print(colored.green('[PirateBay] URL') + ' : ' + tpb_url)
+        print(colored.green('[SkyTorrents] URL') + ' : ' + skytorrents_url)
     elif arg == 'h':
         print_menu(0)
     elif arg == 'q':
         exit = True
     elif 'p' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
             if resNum == 0:
                 printTopResults(resNum)
             elif resNum == 1:
                 printTopResults(resNum)
             else:
-                print "Not a valid option!"
+                print("Not a valid option!")
         except AttributeError:
             if arg == 'p':
                 printTopResults(print_version)
             else:
-                print "Not a valid command!"
+                print("Not a valid command!")
     elif arg == 's':
-        query = raw_input("Enter query : ")
+        query = input("Enter query : ")
         if query == '':
             query = defaultQuery
         searchAllSites(query, force_search=True)
         printTopResults(print_version)
     elif arg == 'r':
         searchAllSites(query)
         printTopResults(print_version)
     else:
-        print 'Invalid command!\n'
+        print('Invalid command!\n')
 
 def print_menu(arg=0):
     if arg == 0:
-        print '''
+        print('''
         ------ Help Menu -------
         Available Commands :
         1. m<result number> - Print magnet link of selected torrent
         2. c<result number> - Copy magnet link of selected torrent to clipboard
         3. d<result number> - Download torrent using default torrent client
         4. o<result number> - Open the torrent page of the selected torrent in the default browser
         5. cs<result number> - Copy magnet link and open seedr.cc
         6. cz<result number> - Copy magnet link and open zbigz
         7. p[optional:<choice>] - Print top 10 results from each website for the given query
             <choice> : [{default : 1}, {0 : Print formatted result}, {1 : Pretty print results}]
         8. s - Enter a new query to search for over all avilable torrent websites
         9. r - Repeat last search (with same query)
-        ------------------------'''
+        ------------------------''')
     elif arg == 1:
-        print '''
+        print('''
         Enter 'q' to exit and 'h' to see all available commands.
-        '''
+        ''')
 
 def searchAllSites(query=defaultQuery, force_search=False, quiet_mode=False):
-    global results, results_rarbg, results_sky, results_tpb_api, tpb_retries, max_tpb_retries, tpb_working_domain
+    global results, results_rarbg, results_sky, results_tpb_api, tpb_retries, max_tpb_retries, tpb_working_domain, results_tpb_condensed
     #results = searchPirateBay(query, domain='pirateproxy.cam')
     #results = searchPirateBay(query)
 
     if force_search == True:
         results_rarbg = None
         results_tpb_api = None
         results_sky = None
         results = None
+        results_tpb_condensed = None
 
     if results_rarbg == None or results_rarbg == []:
         results_rarbg = searchRarbg(query, quiet_mode=quiet_mode)
     #     print 'R searching...'
     # else:
     #     print 'R not searching...'
     # print 'Results R : '
@@ -969,18 +1033,27 @@
 
     #     print 'P searching...'
     # else:
     #     print 'P not searching...'
     # print 'Results P : '
     # print results_tpb_api
     
-    if results == None or results == []:
+    # if results == None or results == []:
+    #     tpb_working_domain = 'thepiratebay.zone'
+    #     results = searchPirateBay(query, quiet_mode=quiet_mode, domain=tpb_working_domain)
+    # #     #print results
+
+    if results_tpb_condensed == None or results_tpb_condensed == []:
         tpb_working_domain = 'thepiratebay.zone'
-        results = searchPirateBay(query, quiet_mode=quiet_mode, domain=tpb_working_domain)
-        #print results
+        results_tpb_condensed = searchPirateBayCondensed(search_string=query, domain=tpb_working_domain, quiet_mode=quiet_mode)
+        results = results_tpb_condensed
+    #     print('P searching...')
+    # else:
+    #     print('P not searching...')
+    # print(f'Results P: {results_tpb_condensed}')
 
     if results_sky == None or results_sky == []:
         results_sky = searchSkyTorrents(query, quiet_mode=quiet_mode)
     #     print 'S searching...'
     # else:
     #     print 'S not searching...'
     # print 'Results S : '
@@ -1035,15 +1108,15 @@
     #print results_json_tpb
 
     combined_json_results = {}
     combined_json_results['rarbg'] = results_json_rarbg
     combined_json_results['tpb'] = results_json_tpb
     combined_json_results['sky'] = results_json_sky
 
-    print combined_json_results
+    print(combined_json_results)
 
 def generateAppID(version=-1):
     if version == 0: # Product of 3 random numbers
         x, y, z = random.randint(1, 100), random.randint(1, 100), random.randint(1, 100)
         app_id = x * y * z
     else : # Hash current epoch time
         epoch_time = time.time()
@@ -1077,9 +1150,9 @@
     else: # Continue in interactive mode
         searchAllSites(query) # quiet_mode is off by default
         printTopResults(print_version)
         
         exit = False
         while(exit != True):
             print_menu(1)
-            choice = raw_input("Enter command : ")
+            choice = input("Enter command : ")
             switch(choice, tpb_api=False)
```

### Comparing `torrent-hound-1.8.4/README.rst` & `torrent-hound-2.0/torrent_hound.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: torrent-hound
+Version: 2.0
+Summary: Search torrents from multiple websites via the CLI
+Home-page: https://github.com/baddymaster/torrent-hound
+Author: Yashovardhan Sharma
+Author-email: yash.s@tuta.io
+License: AGPL-3.0
+Requires-Python: >=3
+
 Torrent Hound
 =============
 
 Search torrents from multiple websites via the CLI
 
 Requirements
 ~~~~~~~~~~~~
@@ -69,8 +79,8 @@
 
 Help
 ~~~~
 
 In case of an ``SSL Error``, consult `these answers on Stackoverflow`_
 for potential fixes.
 
-.. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
+.. _these answers on Stackoverflow: https://stackoverflow.com/questions/31649390/python-requests-ssl-handshake-failure
```

