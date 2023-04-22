# Comparing `tmp/pokepastes-scraper-0.2.0.tar.gz` & `tmp/pokepastes-scraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokepastes-scraper-0.2.0.tar", last modified: Tue Apr 18 07:32:23 2023, max compression
+gzip compressed data, was "pokepastes-scraper-0.2.1.tar", last modified: Sat Apr 22 01:29:16 2023, max compression
```

## Comparing `pokepastes-scraper-0.2.0.tar` & `pokepastes-scraper-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.872592 pokepastes-scraper-0.2.0/
--rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2951 2023-04-18 07:32:23.871107 pokepastes-scraper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2023-04-18 07:19:09.000000 pokepastes-scraper-0.2.0/README.md
--rw-rw-rw-   0        0        0      718 2023-04-18 07:30:59.000000 pokepastes-scraper-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 07:32:23.873090 pokepastes-scraper-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.820014 pokepastes-scraper-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.834900 pokepastes-scraper-0.2.0/src/pokepastes_scraper/
--rw-rw-rw-   0        0        0     7906 2023-04-18 07:11:43.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.864158 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/
--rw-rw-rw-   0        0        0     2951 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 07:32:23.000000 pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 07:32:23.868623 pokepastes-scraper-0.2.0/test/
--rw-rw-rw-   0        0        0      745 2023-04-18 07:13:19.000000 pokepastes-scraper-0.2.0/test/test_json_conversion.py
+drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.295613 pokepastes-scraper-0.2.1/
+-rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3003 2023-04-22 01:29:16.292603 pokepastes-scraper-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2023-04-19 01:33:09.000000 pokepastes-scraper-0.2.1/README.md
+-rw-rw-rw-   0        0        0      718 2023-04-22 01:28:04.000000 pokepastes-scraper-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 01:29:16.296593 pokepastes-scraper-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.221791 pokepastes-scraper-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.239764 pokepastes-scraper-0.2.1/src/pokepastes_scraper/
+-rw-rw-rw-   0        0        0     8070 2023-04-22 01:25:04.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.284629 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3003 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.287638 pokepastes-scraper-0.2.1/test/
+-rw-rw-rw-   0        0        0      745 2023-04-18 07:13:19.000000 pokepastes-scraper-0.2.1/test/test_json_conversion.py
```

### Comparing `pokepastes-scraper-0.2.0/LICENSE` & `pokepastes-scraper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokepastes-scraper-0.2.0/PKG-INFO` & `pokepastes-scraper-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,10 +63,10 @@
 Amoonguss with Sitrus Berry (Tera: Steel)
 Pelipper with Focus Sash (Tera: Flying)
 Palafin with Mystic Water (Tera: Water)
 Baxcalibur with Dragon Fang (Tera: Poison)
 Dragonite with Lum Berry (Tera: Flying)
 ```
 
-For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
+For a detailed example output of `team_from_url`, see `example/example.py` and its output `example/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.10+.
+Tested in python 3.11, but likely compatible with 3.10+. Feel free to contact me: myapaulogies@tuta.io
```

### Comparing `pokepastes-scraper-0.2.0/README.md` & `pokepastes-scraper-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 Amoonguss with Sitrus Berry (Tera: Steel)
 Pelipper with Focus Sash (Tera: Flying)
 Palafin with Mystic Water (Tera: Water)
 Baxcalibur with Dragon Fang (Tera: Poison)
 Dragonite with Lum Berry (Tera: Flying)
 ```
 
-For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
+For a detailed example output of `team_from_url`, see `example/example.py` and its output `example/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.10+.
+Tested in python 3.11, but likely compatible with 3.10+. Feel free to contact me: myapaulogies@tuta.io
```

### Comparing `pokepastes-scraper-0.2.0/pyproject.toml` & `pokepastes-scraper-0.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pokepastes-scraper"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="MyApaulogies", email="myapaulogies@tuta.io" },
 ]
 description = "Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pokepastes-scraper-0.2.0/src/pokepastes_scraper/__init__.py` & `pokepastes-scraper-0.2.1/src/pokepastes_scraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,30 +223,33 @@
             try:
                 setattr(res, k, v)
             except AttributeError:
                 print('WARN: skipping unknown field', k)
     
     return res
 
-def team_from_json(json_string: str | bytes | bytearray):
-    '''Returns a team given a JSON that was generated with `PokepastesTeam.to_json()`.'''
-    d: dict = json.loads(json_string)
+
+def team_from_dict(d: dict):
+    '''Returns a team given a `dict` representation of the JSON generated with `PokepastesTeam.to_json()`.'''
     res = PokepastesTeam()
     
     for k,v in d.items():
         if k == 'members':
             res.members = [_mon_from_dict(mon) for mon in v]
         else:
             try:
                 setattr(res, k, v)
             except AttributeError:
                 print('WARN: skipping unknown field', k)
     
     return res
 
+def team_from_json(json_string: str | bytes | bytearray):
+    '''Returns a team given a JSON that was generated with `PokepastesTeam.to_json()`.'''
+    return team_from_dict(json.loads(json_string))
 
 
 def team_from_url(url: str):
     page = requests.get(url)
     return team_from_html(page.text)
 
 def team_from_html(text: str):
@@ -254,15 +257,15 @@
     soup = BeautifulSoup(text, 'html.parser')
 
     sidebar: Tag = soup.find('aside')
     sidebar_iter = iter(sidebar.children)
 
     # get first six elements, and save three meaningful ones
     _, res.title, _, author_line, _, res.desc = \
-        [i.text.strip() for i in it.islice(sidebar_iter, 6)]
+        [i.text.strip() or None for i in it.islice(sidebar_iter, 6)]
 
     # get stuff right of first 'by' (there must be a better way)
     res.author = ''.join(author_line.split('by')[1:]).strip()
 
     html_mons = soup.find_all('pre')    
     res.members = [PokepastesMon._from_pre(mon) for mon in html_mons]
```

### Comparing `pokepastes-scraper-0.2.0/src/pokepastes_scraper.egg-info/PKG-INFO` & `pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,10 +63,10 @@
 Amoonguss with Sitrus Berry (Tera: Steel)
 Pelipper with Focus Sash (Tera: Flying)
 Palafin with Mystic Water (Tera: Water)
 Baxcalibur with Dragon Fang (Tera: Poison)
 Dragonite with Lum Berry (Tera: Flying)
 ```
 
-For a detailed example output of `team_from_url`, see `test/example.py` and its output `test/example_team.json`.
+For a detailed example output of `team_from_url`, see `example/example.py` and its output `example/example_team.json`.
 
-Tested in python 3.11, but likely compatible with 3.10+.
+Tested in python 3.11, but likely compatible with 3.10+. Feel free to contact me: myapaulogies@tuta.io
```

### Comparing `pokepastes-scraper-0.2.0/test/test_json_conversion.py` & `pokepastes-scraper-0.2.1/test/test_json_conversion.py`

 * *Files identical despite different names*

