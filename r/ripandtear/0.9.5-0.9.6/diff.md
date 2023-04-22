# Comparing `tmp/ripandtear-0.9.5.tar.gz` & `tmp/ripandtear-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripandtear-0.9.5.tar", last modified: Sat Apr 22 16:58:50 2023, max compression
+gzip compressed data, was "ripandtear-0.9.6.tar", last modified: Sat Apr 22 18:42:07 2023, max compression
```

## Comparing `ripandtear-0.9.5.tar` & `ripandtear-0.9.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:58:50.725273 ripandtear-0.9.5/
--rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.5/LICENSE
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 16:58:50.729272 ripandtear-0.9.5/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 16:57:20.000000 ripandtear-0.9.5/README.md
--rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.5/pyproject.toml
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:58:50.721273 ripandtear-0.9.5/ripandtear/
--rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-22 16:57:20.000000 ripandtear-0.9.5/ripandtear/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-02-28 02:57:32.000000 ripandtear-0.9.5/ripandtear/__main__.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:58:50.725273 ripandtear-0.9.5/ripandtear/extractors/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.5/ripandtear/extractors/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/bunkr.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.5/ripandtear/extractors/common.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/coomer.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/cyberdrop.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/gfycat.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/gofile.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/imgur.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/jpg.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/reddit.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     9383 2023-04-22 15:55:11.000000 ripandtear-0.9.5/ripandtear/extractors/redgifs.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/extractors/tiktits.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:58:50.725273 ripandtear-0.9.5/ripandtear/utils/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.5/ripandtear/utils/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.5/ripandtear/utils/cli_arguments.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.5/ripandtear/utils/color.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/utils/conductor.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-03-02 23:14:20.000000 ripandtear-0.9.5/ripandtear/utils/content_finder.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.5/ripandtear/utils/custom_types.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/utils/downloader.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.5/ripandtear/utils/file_hasher.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/utils/file_sorter.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.5/ripandtear/utils/logger.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.5/ripandtear/utils/progress.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.5/ripandtear/utils/rat_info.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.5/ripandtear/utils/rat_interaction.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.5/ripandtear/utils/tracker.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 16:58:50.725273 ripandtear-0.9.5/ripandtear.egg-info/
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/SOURCES.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/dependency_links.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/entry_points.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/requires.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-22 16:58:50.000000 ripandtear-0.9.5/ripandtear.egg-info/top_level.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-22 16:58:50.729272 ripandtear-0.9.5/setup.cfg
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.639579 ripandtear-0.9.6/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.6/LICENSE
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 18:42:07.639579 ripandtear-0.9.6/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 18:41:05.000000 ripandtear-0.9.6/README.md
+-rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.6/pyproject.toml
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.631579 ripandtear-0.9.6/ripandtear/
+-rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/__main__.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.635579 ripandtear-0.9.6/ripandtear/extractors/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.6/ripandtear/extractors/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/bunkr.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.6/ripandtear/extractors/common.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/coomer.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/cyberdrop.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/gfycat.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/gofile.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/imgur.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/jpg.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/reddit.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     9382 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/extractors/redgifs.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/tiktits.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.639579 ripandtear-0.9.6/ripandtear/utils/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.6/ripandtear/utils/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.6/ripandtear/utils/cli_arguments.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/color.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/conductor.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/utils/content_finder.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/custom_types.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/downloader.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.6/ripandtear/utils/file_hasher.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/file_sorter.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/logger.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/progress.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.6/ripandtear/utils/rat_info.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/rat_interaction.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/tracker.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.635579 ripandtear-0.9.6/ripandtear.egg-info/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/SOURCES.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/dependency_links.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/entry_points.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/requires.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/top_level.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-22 18:42:07.639579 ripandtear-0.9.6/setup.cfg
```

### Comparing `ripandtear-0.9.5/LICENSE` & `ripandtear-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/PKG-INFO` & `ripandtear-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.5
+Version: 0.9.6
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -138,15 +138,15 @@
 ## Examples
 
 ### Download a link
 
 Ripandtear has extractors to download content from many different content providers (see ***Supported Sites***). The simplest use case is to download content from a supported url
 
 
-`ripandtear -d 'https://www.supportedsite.com/<content-id>,https://www.differentsite.io/<content-id>.jpg'`
+`ripandtear -d 'https://www.supportedsite.com/<content-id>|https://www.differentsite.io/<content-id>.jpg'`
 
 `ripandtear` - the name of the program
 
 `-d` - `-d` stands for download. If Ripandtear recognizes the url it will download all the content it can find into the current directory. You can download multiple links at once by seperating them with commas (,) or even adding multiple `-d` flags in the same command
 
 ### Creating a new user
 
@@ -196,15 +196,15 @@
 ### Adding another username
 
 You find out that the same content creator uses multiple different reddit names. 
 You want to add the new name you found.
 Doing that is extreamly easy. 
 All you have to do is run the following command:
 
-`ripandtear -r 'new_example_reddit_username,plus_another_username' -r 'even_another_name'`
+`ripandtear -r 'new_example_reddit_username|plus_another_username' -r 'even_another_name'`
 
 Ripandtear looks in the current directory for a .rat file. If a .rat doesn't exist is creates one (naming itself after the current directory) and adds the names. 
 If it finds a .rat it adds the new username(s) to the already existing .rat file. 
 You can even add multiple names at once by separting them with commas (,) and/or multiple identical flags. 
 Don't worry about accidentally adding the same name multiple times. 
 Ripandtear makes sure that each name stored in the .rat is unique and that there are no duplicates. 
 This approach applies for all username categories. See ***stored names*** to see which usernames you can store and the flags to use to set them.
```

### Comparing `ripandtear-0.9.5/README.md` & `ripandtear-0.9.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 ## Examples
 
 ### Download a link
 
 Ripandtear has extractors to download content from many different content providers (see ***Supported Sites***). The simplest use case is to download content from a supported url
 
 
-`ripandtear -d 'https://www.supportedsite.com/<content-id>,https://www.differentsite.io/<content-id>.jpg'`
+`ripandtear -d 'https://www.supportedsite.com/<content-id>|https://www.differentsite.io/<content-id>.jpg'`
 
 `ripandtear` - the name of the program
 
 `-d` - `-d` stands for download. If Ripandtear recognizes the url it will download all the content it can find into the current directory. You can download multiple links at once by seperating them with commas (,) or even adding multiple `-d` flags in the same command
 
 ### Creating a new user
 
@@ -184,15 +184,15 @@
 ### Adding another username
 
 You find out that the same content creator uses multiple different reddit names. 
 You want to add the new name you found.
 Doing that is extreamly easy. 
 All you have to do is run the following command:
 
-`ripandtear -r 'new_example_reddit_username,plus_another_username' -r 'even_another_name'`
+`ripandtear -r 'new_example_reddit_username|plus_another_username' -r 'even_another_name'`
 
 Ripandtear looks in the current directory for a .rat file. If a .rat doesn't exist is creates one (naming itself after the current directory) and adds the names. 
 If it finds a .rat it adds the new username(s) to the already existing .rat file. 
 You can even add multiple names at once by separting them with commas (,) and/or multiple identical flags. 
 Don't worry about accidentally adding the same name multiple times. 
 Ripandtear makes sure that each name stored in the .rat is unique and that there are no duplicates. 
 This approach applies for all username categories. See ***stored names*** to see which usernames you can store and the flags to use to set them.
```

### Comparing `ripandtear-0.9.5/ripandtear/__main__.py` & `ripandtear-0.9.6/ripandtear/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,105 +118,105 @@
             rat_info.print_rat('urls_to_download')
 
         if args.print_youtube:
             rat_info.print_rat('names', 'youtube')
 
         if args.reddit:
             for entry in args.reddit:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'reddit', name)
 
         if args.redgifs:
             for entry in args.redgifs:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'redgifs', name)
 
         if args.onlyfans:
             for entry in args.onlyfans:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'onlyfans', name)
 
         if args.fansly:
             for entry in args.fansly:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'fansly', name)
 
         if args.pornhub:
             for entry in args.pornhub:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'pornhub', name)
 
         if args.twitter:
             for entry in args.twitter:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'twitter', name)
 
         if args.tiktits:
             for entry in args.tiktits:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'tiktits', name)
 
         if args.instagram:
             for entry in args.instagram:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'instagram', name)
 
         if args.youtube:
             for entry in args.youtube:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'youtube', name)
 
         if args.tiktok:
             for entry in args.tiktok:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'tiktok', name)
 
         if args.twitch:
             for entry in args.twitch:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'twitch', name)
 
         if args.patreon:
             for entry in args.patreon:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'patreon', name)
 
         if args.tumblr:
             for entry in args.tumblr:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'tumblr', name)
 
         if args.myfreecams:
             for entry in args.myfreecams:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'myfreecams', name)
 
         if args.chaturbate:
             for entry in args.chaturbate:
-                for name in entry.split(','):
+                for name in entry.split('|'):
                     rat_info.update_rat('names', 'chaturbate', name)
 
         if args.simp:
             for entry in args.simp:
-                for url in entry.split(','):
+                for url in entry.split('|'):
                     rat_info.update_rat('links', 'simpcity', url)
 
         if args.coomer:
             for entry in args.coomer:
-                for url in entry.split(','):
+                for url in entry.split('|'):
                     rat_info.update_rat('links', 'coomer', url)
 
         if args.url_add:
             for entry in args.url_add:
-                for url in entry.split(','):
+                for url in entry.split('|'):
                     rat_info.update_rat('urls_to_download', None, url)
 
         if args.urls_downloaded:
             for entry in args.urls_downloaded:
-                for url in entry.split(','):
+                for url in entry.split('|'):
                     rat_info.update_rat('urls_downloaded', None, url)
 
         if args.erase_errors:
             rat_info.erase_error_dictionaries()
 
         if args.get_urls or \
                 args.download or \
```

### Comparing `ripandtear-0.9.5/ripandtear/extractors/bunkr.py` & `ripandtear-0.9.6/ripandtear/extractors/bunkr.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/common.py` & `ripandtear-0.9.6/ripandtear/extractors/common.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/coomer.py` & `ripandtear-0.9.6/ripandtear/extractors/coomer.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/cyberdrop.py` & `ripandtear-0.9.6/ripandtear/extractors/cyberdrop.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/gfycat.py` & `ripandtear-0.9.6/ripandtear/extractors/gfycat.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/gofile.py` & `ripandtear-0.9.6/ripandtear/extractors/gofile.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/imgur.py` & `ripandtear-0.9.6/ripandtear/extractors/imgur.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/jpg.py` & `ripandtear-0.9.6/ripandtear/extractors/jpg.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/reddit.py` & `ripandtear-0.9.6/ripandtear/extractors/reddit.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/extractors/redgifs.py` & `ripandtear-0.9.6/ripandtear/extractors/redgifs.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         elif re_tag_url.match(url_dictionary['url']):
 
             log.debug("Tags url found. Preparing download")
             await self.tag_download(url_dictionary.copy())
 
     async def tag_download(self, url_dictionary: UrlDictionary) -> None:
 
-        log.info(f"Found Tag. Preparing download")
+        log.info("Found Tag. Preparing download")
 
         async with async_playwright() as pw:
 
             try:
                 browser = await pw.chromium.launch()
                 page = await browser.new_page()
                 await page.goto(url_dictionary['url'])
```

### Comparing `ripandtear-0.9.5/ripandtear/extractors/tiktits.py` & `ripandtear-0.9.6/ripandtear/extractors/tiktits.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/cli_arguments.py` & `ripandtear-0.9.6/ripandtear/utils/cli_arguments.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/color.py` & `ripandtear-0.9.6/ripandtear/utils/color.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/conductor.py` & `ripandtear-0.9.6/ripandtear/utils/conductor.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/content_finder.py` & `ripandtear-0.9.6/ripandtear/utils/content_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     return url_dictionary
 
 
 async def download_urls(args, url_dictionary: UrlDictionary) -> None:
 
     tasks = []
     for entry in args.download:
-        for url in entry.split(','):
+        for url in entry.split('|'):
 
             url_dictionary: UrlDictionary = url_dictionary_constructor(
                 url.strip(), url_dictionary.copy(), download=True,)
 
             tasks.append(asyncio.create_task(
                 conductor.validate_url(url_dictionary.copy())))
 
@@ -114,15 +114,15 @@
 async def print_urls(args, url_dictionary: UrlDictionary) -> None:
 
     tracker = Tracker.getInstance()
 
     tasks = []
 
     for entry in args.get_urls:
-        for url in entry.split(','):
+        for url in entry.split('|'):
 
             new_url_dictionary: UrlDictionary = url_dictionary_constructor(
                 url.strip(), url_dictionary.copy(), download=False)
 
             tasks.append(asyncio.create_task(
                 conductor.validate_url(new_url_dictionary.copy())))
```

### Comparing `ripandtear-0.9.5/ripandtear/utils/custom_types.py` & `ripandtear-0.9.6/ripandtear/utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/downloader.py` & `ripandtear-0.9.6/ripandtear/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/file_hasher.py` & `ripandtear-0.9.6/ripandtear/utils/file_hasher.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/file_sorter.py` & `ripandtear-0.9.6/ripandtear/utils/file_sorter.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/progress.py` & `ripandtear-0.9.6/ripandtear/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/rat_info.py` & `ripandtear-0.9.6/ripandtear/utils/rat_info.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/rat_interaction.py` & `ripandtear-0.9.6/ripandtear/utils/rat_interaction.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear/utils/tracker.py` & `ripandtear-0.9.6/ripandtear/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/ripandtear.egg-info/PKG-INFO` & `ripandtear-0.9.6/ripandtear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.5
+Version: 0.9.6
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -138,15 +138,15 @@
 ## Examples
 
 ### Download a link
 
 Ripandtear has extractors to download content from many different content providers (see ***Supported Sites***). The simplest use case is to download content from a supported url
 
 
-`ripandtear -d 'https://www.supportedsite.com/<content-id>,https://www.differentsite.io/<content-id>.jpg'`
+`ripandtear -d 'https://www.supportedsite.com/<content-id>|https://www.differentsite.io/<content-id>.jpg'`
 
 `ripandtear` - the name of the program
 
 `-d` - `-d` stands for download. If Ripandtear recognizes the url it will download all the content it can find into the current directory. You can download multiple links at once by seperating them with commas (,) or even adding multiple `-d` flags in the same command
 
 ### Creating a new user
 
@@ -196,15 +196,15 @@
 ### Adding another username
 
 You find out that the same content creator uses multiple different reddit names. 
 You want to add the new name you found.
 Doing that is extreamly easy. 
 All you have to do is run the following command:
 
-`ripandtear -r 'new_example_reddit_username,plus_another_username' -r 'even_another_name'`
+`ripandtear -r 'new_example_reddit_username|plus_another_username' -r 'even_another_name'`
 
 Ripandtear looks in the current directory for a .rat file. If a .rat doesn't exist is creates one (naming itself after the current directory) and adds the names. 
 If it finds a .rat it adds the new username(s) to the already existing .rat file. 
 You can even add multiple names at once by separting them with commas (,) and/or multiple identical flags. 
 Don't worry about accidentally adding the same name multiple times. 
 Ripandtear makes sure that each name stored in the .rat is unique and that there are no duplicates. 
 This approach applies for all username categories. See ***stored names*** to see which usernames you can store and the flags to use to set them.
```

### Comparing `ripandtear-0.9.5/ripandtear.egg-info/SOURCES.txt` & `ripandtear-0.9.6/ripandtear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.5/setup.cfg` & `ripandtear-0.9.6/setup.cfg`

 * *Files identical despite different names*

