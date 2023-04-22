# Comparing `tmp/torrent-hound-2.0.1.tar.gz` & `tmp/torrent-hound-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrent-hound-2.0.1.tar", last modified: Sat Apr 22 01:33:21 2023, max compression
+gzip compressed data, was "torrent-hound-2.1.0.tar", last modified: Sat Apr 22 14:40:40 2023, max compression
```

## Comparing `torrent-hound-2.0.1.tar` & `torrent-hound-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:33:21.971453 torrent-hound-2.0.1/
--rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-2.0.1/MANIFEST.in
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:33:21.968036 torrent-hound-2.0.1/PKG-INFO
--rw-r--r--   0 yashovardhan   (501) staff       (20)     1974 2023-04-22 01:31:31.000000 torrent-hound-2.0.1/README.rst
--rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2023-04-22 01:33:21.974193 torrent-hound-2.0.1/setup.cfg
--rw-r--r--   0 yashovardhan   (501) staff       (20)      830 2023-04-22 01:24:27.000000 torrent-hound-2.0.1/setup.py
--rwxr--r--   0 yashovardhan   (501) staff       (20)    52365 2023-04-22 01:14:00.000000 torrent-hound-2.0.1/torrent-hound
-drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 01:33:21.966190 torrent-hound-2.0.1/torrent_hound.egg-info/
--rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/PKG-INFO
--rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/SOURCES.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/dependency_links.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/requires.txt
--rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 01:33:21.000000 torrent-hound-2.0.1/torrent_hound.egg-info/top_level.txt
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 14:40:40.993059 torrent-hound-2.1.0/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       18 2018-06-15 03:26:44.000000 torrent-hound-2.1.0/MANIFEST.in
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 14:40:40.992577 torrent-hound-2.1.0/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     1974 2023-04-22 01:31:31.000000 torrent-hound-2.1.0/README.rst
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       38 2023-04-22 14:40:40.993412 torrent-hound-2.1.0/setup.cfg
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      830 2023-04-22 14:39:22.000000 torrent-hound-2.1.0/setup.py
+-rwxr--r--   0 yashovardhan   (501) staff       (20)    58285 2023-04-22 14:40:11.000000 torrent-hound-2.1.0/torrent-hound
+drwxr-xr-x   0 yashovardhan   (501) staff       (20)        0 2023-04-22 14:40:40.991681 torrent-hound-2.1.0/torrent_hound.egg-info/
+-rw-r--r--   0 yashovardhan   (501) staff       (20)     2245 2023-04-22 14:40:40.000000 torrent-hound-2.1.0/torrent_hound.egg-info/PKG-INFO
+-rw-r--r--   0 yashovardhan   (501) staff       (20)      229 2023-04-22 14:40:40.000000 torrent-hound-2.1.0/torrent_hound.egg-info/SOURCES.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 14:40:40.000000 torrent-hound-2.1.0/torrent_hound.egg-info/dependency_links.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)       63 2023-04-22 14:40:40.000000 torrent-hound-2.1.0/torrent_hound.egg-info/requires.txt
+-rw-r--r--   0 yashovardhan   (501) staff       (20)        1 2023-04-22 14:40:40.000000 torrent-hound-2.1.0/torrent_hound.egg-info/top_level.txt
```

### Comparing `torrent-hound-2.0.1/PKG-INFO` & `torrent-hound-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrent-hound
-Version: 2.0.1
+Version: 2.1.0
 Summary: Search torrents from multiple websites via the CLI
 Home-page: https://github.com/baddymaster/torrent-hound
 Author: Yashovardhan Sharma
 Author-email: yash.s@tuta.io
 License: AGPL-3.0
 Requires-Python: >=3
```

### Comparing `torrent-hound-2.0.1/README.rst` & `torrent-hound-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `torrent-hound-2.0.1/setup.py` & `torrent-hound-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='torrent-hound',          # This is the name of your PyPI-package.
-    version='2.0.1',                 # Update the version number for new releases
+    version='2.1.0',                 # Update the version number for new releases
     scripts=['torrent-hound'],     # The name of your scipt, and also the command you'll be using for calling it
     description='Search torrents from multiple websites via the CLI',
     long_description=readme(),
     python_requires = '>=3',
     url='https://github.com/baddymaster/torrent-hound',
     install_requires=[
         'bs4',
```

### Comparing `torrent-hound-2.0.1/torrent-hound` & `torrent-hound-2.1.0/torrent-hound`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,21 @@
 import cfscrape as cfs
 import traceback
 
 defaultQuery, query = 'jason bourne', ''
 results_sky = None
 results_tpb_condensed = None
 results_tpb_api, num_results_tpb_api = None, 0
+results_1337x = None
 results, results_rarbg, exit, error_detected_rarbg, error_detected_tpb = None, None, None, None, None
-num_results, num_results_rarbg, num_results_sky, print_version = 0, 0, 0, 1
+num_results, num_results_rarbg, num_results_sky, num_results_1337x, print_version = 0, 0, 0, 0, 1
 auth_token = 'None'
 app_id = 'None'
 tpb_working_domain = 'tpb.tw'
-rarbg_url, skytorrents_url, tpb_url = '', '', ''
+rarbg_url, skytorrents_url, tpb_url, url_1337x = '', '', '', ''
 tpb_retries, max_tpb_retries = 0, 3
 
 def enum(**enums):
     """
     Lets define enums
     """
     return type('Enum', (), enums)
@@ -268,14 +269,107 @@
         return index - 1
     else:
         table_rarbg.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
         table_rarbg.align[colored.red('Torrent Name')] = 'l'
         print(table_rarbg)
         return 0
 
+def extract_magnet_link_1337x(url):
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
+    response = requests.get(url, headers=headers)
+    soup = BeautifulSoup(response.content, 'html.parser')
+    magnet_link = soup.find('a', href=lambda href: href and href.startswith("magnet:"))
+    if magnet_link:
+        return magnet_link['href']
+    else:
+        return None
+    
+def search1337x(search_string=defaultQuery, domain='1337x.to', quiet_mode=False, limit=10):
+    global results_1337x, url_1337x
+
+    query = removeAndReplaceSpaces(search_string)
+    page_no = 1
+    baseURL = f'https://{domain}'
+    url = f'{baseURL}/search/{query}/{page_no}/'
+    url_1337x = url
+    
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.0; WOW64; rv:24.0) Gecko/20100101 Firefox/24.0'}
+    response = requests.get(url, headers=headers)
+    soup = BeautifulSoup(response.text, 'html.parser')
+    results_1337x = []
+    
+    table = soup.find('table', {'class': 'table-list'})
+    rows = table.tbody.find_all('tr')
+    for row in rows[:limit]:
+        row_data = {}
+        name_col = row.find('td', {'class': 'coll-1 name'})
+        row_data['name'] = name_col.a.next_sibling.text
+        row_data['link'] = baseURL + name_col.a.next_sibling['href']
+        row_data['seeders'] = int(row.find('td', {'class': 'coll-2 seeds'}).text.strip())
+        row_data['leechers'] = int(row.find('td', {'class': 'coll-3 leeches'}).text.strip())
+        try:
+            row_data['ratio'] = format( (float(row_data['seeders'])/float(row_data['leechers'])), '.1f' )
+        except ZeroDivisionError:
+            row_data['ratio'] = 'inf'
+        row_data['time'] = row.find('td', {'class': 'coll-date'}).text.strip()
+        size_col = row.find('td', {'class': 'coll-4'})
+        if size_col:
+            row_data['size'] = size_col.contents[0].strip()
+        else:
+            row_data['size'] = ''
+        # uploader_col = row.find('td', {'class': 'coll-5'})
+        # if uploader_col:
+        #     row_data['uploader'] = uploader_col.contents[0].text.strip()
+        # else:
+        #     row_data['uploader'] = ''
+        row_data['magnet'] = extract_magnet_link_1337x(row_data['link'])
+        results_1337x.append(row_data)
+    return results_1337x
+
+def pretty_print_top_results_1337x(limit=10):
+    global results_1337x, num_results_tpb_api, num_results
+    table_1337x = VeryPrettyTable(left_padding_width=0, right_padding_width=0, padding_width=0)
+    no_str = str(colored.red('No'))
+    name_str = str(colored.red('Torrent Name'))
+    size_str = str(colored.red('Size'))
+    seed_str = str(colored.red('S'))
+    leech_str = str(colored.red('L'))
+    ratio_str = str(colored.red('S/L'))
+    table_1337x.field_names = [no_str, name_str, size_str, seed_str, leech_str, ratio_str]
+
+    #print '\n\t\t\t\t\t\t' + '+-----------+'
+    #print '\t\t\t\t\t\t| ' + colored.green('PirateBay') + ' |'
+    print('\n\t\t\t\t\t\t' + colored.green('1337x'))
+    # print results
+    if results_1337x != [{}] and results_1337x != [] and results_1337x != None:
+        #index = num_results_tpb_api + 1 # Index after TBP API
+        index = num_results + 1 # Index after TBP regular
+        for r in results_1337x[:limit]:
+            try :
+                table_1337x.add_row([index, r['name'][:57], r['size'], r['seeders'], r['leechers'], r['ratio']])
+                index = index + 1
+            except KeyError as e:
+                # Fix error where {} is included in results and screws up numbering #
+                if r != {}:
+                    print(r)
+                    print(e)
+        table_1337x.align[no_str] = 'l'
+        table_1337x.align[name_str] = 'l'
+        table_1337x.align[size_str] = 'r'
+        table_1337x.align[seed_str] = 'r'
+        table_1337x.align[leech_str] = 'r'
+        table_1337x.align[ratio_str] = 'r'
+        print(table_1337x)
+        return index - 1
+    else:
+        table_1337x.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
+        #table_piratebay.align[colored.red('Torrent Name')] = 'l'
+        print(table_1337x)
+        return num_results
+
 def searchSkyTorrents(search_string=defaultQuery, domain='skytorrents.lol', order_by=ORDER_BY_SKY.RELEVANCE, quiet_mode=False, limit=10):
     global results_sky, skytorrents_url
     search_string = removeAndReplaceSpaces(search_string)
     baseURL = 'https://' + domain
     url = baseURL + '/?query=' + search_string
     skytorrents_url = url
     #url = baseURL + '/search/all/' + order_by + '/1/?l=en-us&q=' + search_string
@@ -791,170 +885,182 @@
     else:
         table_piratebay.add_row(["Null", "Null", "Null", "Null", "Null", "Null"])
         #table_piratebay.align[colored.red('Torrent Name')] = 'l'
         print(table_piratebay)
         return num_results_rarbg
 
 def switch(arg, tpb_api=False):
-    global results, exit, defaultQuery, num_results, query, num_results_rarbg, results_rarbg, print_version, tpb_working_domain, results_tpb_api, num_results_tpb_api, rarbg_url, skytorrents_url, tpb_url
+    global results, exit, defaultQuery, num_results, query, num_results_rarbg, results_rarbg, print_version, tpb_working_domain, results_tpb_api, num_results_tpb_api, results_1337x, num_results_1337x, rarbg_url, skytorrents_url, tpb_url, url_1337x
     if ('c' in arg) and ('s' not in arg) and ('z' not in arg):
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results_tpb_api]['magnet']
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
                 print('Magnet link copied to clipboard!')
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif ('cs' in arg) and ('z' not in arg):
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results_tpb_api]['magnet']
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
                 webbrowser.open('https://www.seedr.cc', new=2)
                 print('Seedr.cc opened and Magnet link copied to clipboard!')
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif 'cz' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results_tpb_api]['magnet']
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results]['magnet']
                 pyperclip.copy(str(mLink))
                 webbrowser.open('https://zbigz.unihax.in/', new=2)
                 print('zbigz opened and Magnet link copied to clipboard!')
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif 'm' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results_tpb_api]['magnet']
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results]['magnet']
                 print("\nMagnet Link : \n" + mLink)
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif 'd' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         mLink = results_tpb_api[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results_tpb_api]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results_tpb_api]['magnet']
                 else:
                     if resNum <= num_results_rarbg :
                         mLink = results_rarbg[resNum-1]['magnet']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         mLink = results[(resNum-1)-num_results_rarbg]['magnet']
                     else:
-                        mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        #mLink = results_sky[(resNum-1)-num_results]['magnet']
+                        mLink = results_1337x[(resNum-1)-num_results]['magnet']
                 webbrowser.open(mLink, new=2)
                 print('Magnet link sent to default torrent client!')
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif 'o' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
             #print("resNum : %d" % resNum)
-            if resNum <= 0 or resNum > num_results_sky:
+            if resNum <= 0 or resNum > num_results_1337x:
                 print('Invalid command!\n')
             else:
                 if tpb_api == True:
                     if resNum <= num_results_rarbg :
                         tLink = results_rarbg[resNum-1]['link']
                         #print("resNum(%d) <= num_results_rarbg(%d)" % (resNum, results_rarbg))
                     elif resNum > num_results_rarbg and resNum <= num_results_tpb_api:
                         tLink = "https://" + tpb_working_domain + results_tpb_api[(resNum-1)-num_results_rarbg]['link']
                         #print("resNum(%d) > num_results_rarbg(%d) and resNum(%d) <= (num_results_rarbg(%d)+num_results(%d))" % (resNum, num_results_rarbg, resNum, num_results_rarbg, num_results))
                     else:
-                        tLink = results_sky[(resNum-1)-num_results_tpb_api]['link']
+                        #tLink = results_sky[(resNum-1)-num_results_tpb_api]['link']
                         #print("Reached SkyTorrents. Link : %s" % tLink)
+                        tLink = results_1337x[(resNum-1)-num_results_tpb_api]['link']
                 else:
                     if resNum <= num_results_rarbg :
                         tLink = results_rarbg[resNum-1]['link']
                     elif resNum > num_results_rarbg and resNum <= num_results:
                         #tLink = "https://" + tpb_working_domain + results[(resNum-1)-num_results_rarbg]['link']
                         tLink = results[(resNum-1)-num_results_rarbg]['link']
                     else:
-                        tLink = results_sky[(resNum-1)-num_results]['link']
+                        #tLink = results_sky[(resNum-1)-num_results]['link']
+                        tLink = results_1337x[(resNum-1)-num_results]['link']
                 #webbrowser.get('chrome').open(tLink, new=2)
                 webbrowser.open(tLink, new=2)
                 print('Torrent page opened in default browser!')
         except AttributeError:
             print('Enter a valid torrent number as well!')
     elif arg == 'u':
         print(colored.green('[RARBG] URL') + ' : ' + rarbg_url)
         print(colored.green('[PirateBay] URL') + ' : ' + tpb_url)
-        print(colored.green('[SkyTorrents] URL') + ' : ' + skytorrents_url)
+        print(colored.green('[SkyTorrents] URL') + ' : ' + url_1337x)
     elif arg == 'h':
         print_menu(0)
     elif arg == 'q':
         exit = True
     elif 'p' in arg:
         try:
             resNum = int(re.search(r'\d+', arg).group())
@@ -999,27 +1105,30 @@
         ------------------------''')
     elif arg == 1:
         print('''
         Enter 'q' to exit and 'h' to see all available commands.
         ''')
 
 def searchAllSites(query=defaultQuery, force_search=False, quiet_mode=False):
-    global results, results_rarbg, results_sky, results_tpb_api, tpb_retries, max_tpb_retries, tpb_working_domain, results_tpb_condensed
+    global results, results_rarbg, results_sky, results_tpb_api, tpb_retries, max_tpb_retries, tpb_working_domain, results_tpb_condensed, results_1337x
     #results = searchPirateBay(query, domain='pirateproxy.cam')
     #results = searchPirateBay(query)
 
     if force_search == True:
         results_rarbg = None
         results_tpb_api = None
         results_sky = None
+        results_1337x = None
         results = None
         results_tpb_condensed = None
 
+    print(colored.magenta("Searching RARBG..."), end='')
     if results_rarbg == None or results_rarbg == []:
         results_rarbg = searchRarbg(query, quiet_mode=quiet_mode)
+    print(colored.green("Done."))
     #     print 'R searching...'
     # else:
     #     print 'R not searching...'
     # print 'Results R : '
     # print results_rarbg
 
     # if results_tpb_api == None or results_tpb_api == []:
@@ -1038,45 +1147,53 @@
     # print results_tpb_api
     
     # if results == None or results == []:
     #     tpb_working_domain = 'thepiratebay.zone'
     #     results = searchPirateBay(query, quiet_mode=quiet_mode, domain=tpb_working_domain)
     # #     #print results
 
+    print(colored.magenta("Searching TBP..."), end='')
     if results_tpb_condensed == None or results_tpb_condensed == []:
         tpb_working_domain = 'thepiratebay.zone'
         results_tpb_condensed = searchPirateBayCondensed(search_string=query, domain=tpb_working_domain, quiet_mode=quiet_mode)
         results = results_tpb_condensed
+    print(colored.green("Done."))
     #     print('P searching...')
     # else:
     #     print('P not searching...')
     # print(f'Results P: {results_tpb_condensed}')
 
-    if results_sky == None or results_sky == []:
-        results_sky = searchSkyTorrents(query, quiet_mode=quiet_mode)
-    #     print 'S searching...'
+    # if results_sky == None or results_sky == []:
+    #     results_sky = searchSkyTorrents(query, quiet_mode=quiet_mode)
+    # #     print 'S searching...'
     # else:
     #     print 'S not searching...'
     # print 'Results S : '
     # print results_sky
 
+    print(colored.magenta("Searching 1337x..."), end='')
+    if results_1337x == None or results_1337x == []:
+        results_1337x = search1337x(query, quiet_mode=quiet_mode)
+    print(colored.green("Done."))
+
 def printCombinedTopResults():
     global num_results, num_results_rarbg
     num_results_rarbg = print_top_results_rarbg(10)
     num_results = print_top_results(10)
 
 def prettyPrintCombinedTopResults():
-    global num_results, num_results_rarbg, num_results_sky, num_results_tpb_api
+    global num_results, num_results_rarbg, num_results_sky, num_results_tpb_api, num_results_1337x
     num_results_rarbg = pretty_print_top_results_rarbg(10)
     num_results = pretty_print_top_results_piratebay(10)
     #num_results_tpb_api = pretty_print_top_results_piratebay_api(10)
     #num_results = num_results_tpb_api
 
-    num_results_sky = pretty_print_top_results_skytorrents(10)
-
+    #num_results_sky = pretty_print_top_results_skytorrents(10)
+    num_results_1337x = pretty_print_top_results_1337x(10)
+    
 def printTopResults(version=1):
     if version == 0:
         printCombinedTopResults()
     elif version == 1:
         prettyPrintCombinedTopResults()
 
 def convertListJSONToPureJSON(result_list): 
@@ -1096,25 +1213,27 @@
             rj_results[str(index)] = result_list[index]
             index += 1
         result_json['count'] = str(index) # Update total number of results
 
     return result_json
 
 def printResultsQuietly():
-    global results_rarbg, results_tpb_api, results_sky
+    global results_rarbg, results_tpb_api, results_sky, results_1337x
 
     results_json_rarbg = convertListJSONToPureJSON(results_rarbg)
     results_json_tpb = convertListJSONToPureJSON(results_tpb_api)
-    results_json_sky = convertListJSONToPureJSON(results_sky)
+    #results_json_sky = convertListJSONToPureJSON(results_sky)
+    results_json_1337x = convertListJSONToPureJSON(results_1337x)
     #print results_json_tpb
 
     combined_json_results = {}
     combined_json_results['rarbg'] = results_json_rarbg
     combined_json_results['tpb'] = results_json_tpb
-    combined_json_results['sky'] = results_json_sky
+    #combined_json_results['sky'] = results_json_sky
+    combined_json_results['1337x'] = results_json_1337x
 
     print(combined_json_results)
 
 def generateAppID(version=-1):
     if version == 0: # Product of 3 random numbers
         x, y, z = random.randint(1, 100), random.randint(1, 100), random.randint(1, 100)
         app_id = x * y * z
```

### Comparing `torrent-hound-2.0.1/torrent_hound.egg-info/PKG-INFO` & `torrent-hound-2.1.0/torrent_hound.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrent-hound
-Version: 2.0.1
+Version: 2.1.0
 Summary: Search torrents from multiple websites via the CLI
 Home-page: https://github.com/baddymaster/torrent-hound
 Author: Yashovardhan Sharma
 Author-email: yash.s@tuta.io
 License: AGPL-3.0
 Requires-Python: >=3
```

