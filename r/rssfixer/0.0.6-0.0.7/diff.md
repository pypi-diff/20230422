# Comparing `tmp/rssfixer-0.0.6.tar.gz` & `tmp/rssfixer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.0.6.tar", last modified: Thu Apr 20 09:39:31 2023, max compression
+gzip compressed data, was "rssfixer-0.0.7.tar", last modified: Sat Apr 22 07:41:52 2023, max compression
```

## Comparing `rssfixer-0.0.6.tar` & `rssfixer-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081700 rssfixer-0.0.6/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-17 09:42:15.000000 rssfixer-0.0.6/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 09:39:31.081572 rssfixer-0.0.6/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     4084 2023-04-20 06:30:06.000000 rssfixer-0.0.6/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)      813 2023-04-20 09:37:42.000000 rssfixer-0.0.6/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-20 09:39:31.081744 rssfixer-0.0.6/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.079666 rssfixer-0.0.6/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.080521 rssfixer-0.0.6/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       61 2023-04-18 04:00:23.000000 rssfixer-0.0.6/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     8882 2023-04-20 09:37:26.000000 rssfixer-0.0.6/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081283 rssfixer-0.0.6/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     4627 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       65 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-20 09:39:31.000000 rssfixer-0.0.6/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-20 09:39:31.081411 rssfixer-0.0.6/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)     2341 2023-04-18 10:59:41.000000 rssfixer-0.0.6/src/tests/test_rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402802 rssfixer-0.0.7/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.0.7/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     5336 2023-04-22 07:41:52.402645 rssfixer-0.0.7/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     4533 2023-04-22 07:29:10.000000 rssfixer-0.0.7/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1110 2023-04-22 07:36:07.000000 rssfixer-0.0.7/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-22 07:41:52.402849 rssfixer-0.0.7/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.399063 rssfixer-0.0.7/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.400534 rssfixer-0.0.7/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.0.7/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     9165 2023-04-22 07:06:07.000000 rssfixer-0.0.7/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402034 rssfixer-0.0.7/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     5336 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      203 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402183 rssfixer-0.0.7/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)     4314 2023-04-22 07:25:23.000000 rssfixer-0.0.7/src/tests/test_rss.py
```

### Comparing `rssfixer-0.0.6/LICENSE` & `rssfixer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.6/PKG-INFO` & `rssfixer-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Information Technology
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: audit
+Provides-Extra: build
+Provides-Extra: lint
+Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
 [![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 ![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
 [![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
 python3 -m venv venv
@@ -29,15 +38,15 @@
 python3 -m pip install rssfixer
 ```
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
-### List
+### Simple list
 
 An example to generate a feed for [nccgroup][ncc] that have the links in a list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
@@ -60,23 +69,36 @@
 
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
+### General HTML
+
+An example for [tripwire.com][tri]:
+
+```bash
+rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
+
+```
+
+
 ### Usage
 
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES] [--html-url HTML_URL] [--html-title HTML_TITLE]
-                [--html-title-class HTML_TITLE_CLASS] [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS] [--json] [--json-entries JSON_ENTRIES]
-                [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE] [--html-title-class HTML_TITLE_CLASS]
+                [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS]
+                [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE]
+                [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
                 url
 
-Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list. Options are available to find links in other HTML elements or JSON strings.
+Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list.
+Options are available to find links in other HTML elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
@@ -106,13 +128,14 @@
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
   --list                Find entries in HTML <ul>-list (default)
 ```
 
 
   [bso]: https://www.crummy.com/software/BeautifulSoup/
-  [exa]: https://github.com/reuteras/rssfixer/blob/main/example/nccgroup.xml
-  [fge]: https://feedgen.kiesow.be/ 
+  [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
+  [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.0.6/README.md` & `rssfixer-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # rssfixer
 
 [![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 ![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
 [![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
 python3 -m venv venv
@@ -14,15 +15,15 @@
 python3 -m pip install rssfixer
 ```
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
-### List
+### Simple list
 
 An example to generate a feed for [nccgroup][ncc] that have the links in a list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
@@ -45,23 +46,36 @@
 
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
+### General HTML
+
+An example for [tripwire.com][tri]:
+
+```bash
+rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
+
+```
+
+
 ### Usage
 
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES] [--html-url HTML_URL] [--html-title HTML_TITLE]
-                [--html-title-class HTML_TITLE_CLASS] [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS] [--json] [--json-entries JSON_ENTRIES]
-                [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE] [--html-title-class HTML_TITLE_CLASS]
+                [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS]
+                [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE]
+                [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
                 url
 
-Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list. Options are available to find links in other HTML elements or JSON strings.
+Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list.
+Options are available to find links in other HTML elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
@@ -91,13 +105,14 @@
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
   --list                Find entries in HTML <ul>-list (default)
 ```
 
 
   [bso]: https://www.crummy.com/software/BeautifulSoup/
-  [exa]: https://github.com/reuteras/rssfixer/blob/main/example/nccgroup.xml
-  [fge]: https://feedgen.kiesow.be/ 
+  [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
+  [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

### Comparing `rssfixer-0.0.6/src/rssfixer/rss.py` & `rssfixer-0.0.7/src/rssfixer/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Generate rss feed for "blogs" without rss feed."""
 import argparse
+import importlib.metadata
 import json
 import re
 import sys
 
-import pkg_resources
 import requests
 from bs4 import BeautifulSoup
 from feedgen.feed import FeedGenerator
 
+try:
+    __version__ = importlib.metadata.version(__package__ or __name__)
+except importlib.metadata.PackageNotFoundError:  # pragma: no cover
+    __version__ = "0.0.0"
+
 
 def fetch_html(url):
     """Fetch HTML content from a URL."""
     try:
         response = requests.get(url, timeout=10)
-    except requests.exceptions.Timeout:
+    except requests.exceptions.Timeout:  # pragma: no cover
         print("ERROR: Request timed out")
         sys.exit(1)
     return response.text
 
 
 def find_entries(json_object, entries_key):
     """Find the entries in a JSON object with key "entries_key"."""
@@ -30,15 +35,15 @@
                 result = find_entries(value, entries_key)
                 if result is not None:
                     return result
     elif isinstance(json_object, list):
         for item in json_object:
             result = find_entries(item, entries_key)
             if result is not None:
-                return result
+                return result  # pragma: no cover
     return None
 
 
 def extract_links_ul(soup):
     """Extract links from an HTML page with links in <ul>-lists."""
     links = []
     unique_links = set()
@@ -55,15 +60,15 @@
                 # Exclude URLs containing "/category/" or "/author/"
                 if "/category/" not in url and "/author/" not in url:
                     # Check if the URL is unique
                     if url not in unique_links:
                         unique_links.add(url)
                         links.append((url, title, description))
 
-    if not links:
+    if not links:  # pragma: no cover
         print("ERROR: No links found")
         sys.exit(1)
     return links
 
 
 def extract_links_html(soup, arguments):
     """Extract links from an HTML page with links in selectable elements."""
@@ -73,29 +78,29 @@
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.html_entries):
         try:
             url = entry.findNext(arguments.html_url)["href"]
             title = entry.find(
                 arguments.html_title, re.compile(arguments.html_title_class)
             ).text.strip()
-        except (KeyError, AttributeError):
+        except (KeyError, AttributeError):  # pragma: no cover
             print("ERROR: Unable to find URL or title in HTML element")
             sys.exit(1)
         try:
             description = entry.find(
                 arguments.html_description, re.compile(arguments.html_description_class)
             ).text.strip()
-        except (KeyError, AttributeError):
+        except (KeyError, AttributeError):  # pragma: no cover
             # Ignore description if it's not found
             description = ""
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
 
-    if not links:
+    if not links:  # pragma: no cover
         print("ERROR: No links found")
         sys.exit(1)
     return links
 
 
 def extract_links_json(soup, arguments):
     """Extract links from JSON strings in an HTML page."""
@@ -110,27 +115,27 @@
             break
 
     # Extract the links from the JSON object
     for entry in entries:
         try:
             url = entry[arguments.json_url]
             title = entry[arguments.json_title]
-        except KeyError:
+        except KeyError:  # pragma: no cover
             print("ERROR: Unable to find URL or title in JSON object")
             sys.exit(1)
         try:
             description = entry[arguments.json_description]
         except KeyError:
             # Ignore description if it's not found
             description = ""
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
 
-    if links == []:
+    if links == []:  # pragma: no cover
         print("ERROR: No links found")
         sys.exit(1)
     return links
 
 
 def create_rss_feed(links, arguments):
     """Create an RSS feed from a list of links."""
@@ -155,25 +160,25 @@
 
     if vars(arguments).get("atom", False):
         return fg.atom_str(pretty=True).decode("utf-8")
     else:
         return fg.rss_str(pretty=True).decode("utf-8")
 
 
-def parse_arguments():
+def parse_arguments(arguments):
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description="""Generate RSS feed for blog that don't publish a feed.
         Default is to find links in a simple <ul>-list.
         Options are available to find links in other HTML elements or JSON strings."""
     )
     parser.add_argument(
         "--version",
         action="version",
-        version="%(prog)s " + pkg_resources.get_distribution("rssfixer").version,
+        version="%(prog)s " + __version__,
     )
     parser.add_argument("url", help="URL for the blog")
     parser.add_argument("--atom", action="store_true", help="Generate Atom feed")
     parser.add_argument("--base-url", help="Base URL for the blog")
     parser.add_argument("--html", action="store_true", help="Find entries in HTML")
     parser.add_argument(
         "--html-entries", default="article", help="HTML selector for entries"
@@ -225,15 +230,15 @@
         help='Title of the RSS feed (default: "My RSS Feed")',
     )
     parser.add_argument("-q", "--quiet", action="store_true", help="Suppress output")
     parser.add_argument(
         "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
     )
 
-    return parser
+    return parser.parse_args(arguments)
 
 
 def save_rss_feed(rss_feed, arguments):
     """Save the RSS feed to a file."""
     try:
         with open(arguments.output, "w", encoding="utf-8") as f:
             f.write(rss_feed)
@@ -246,19 +251,18 @@
             print(f"Atom feed created: {arguments.output}")
         else:
             print(f"RSS feed created: {arguments.output}")
 
 
 def main():
     """Main function."""
-    parsed_args = parse_arguments()
-    args = parsed_args.parse_args()
+    args = parse_arguments(sys.argv[1:])
 
     if vars(args).get("version"):
-        print(pkg_resources.require("rssfixer")[0].version)
+        print(__version__)
         sys.exit(0)
 
     # Get HTML content from URL
     html_content = fetch_html(args.url)
     soup = BeautifulSoup(html_content, "html.parser")
 
     # Select function to handle different types of blogs
@@ -273,8 +277,8 @@
 
     # Create RSS feed and save to file
     rss_feed = create_rss_feed(links, args)
     save_rss_feed(rss_feed, args)
 
 
 if __name__ == "__main__":
-    main()
+    main()  # pragma: no cover
```

### Comparing `rssfixer-0.0.6/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.0.7/src/rssfixer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Information Technology
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: audit
+Provides-Extra: build
+Provides-Extra: lint
+Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
 [![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 ![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
 [![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
+[![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
 python3 -m venv venv
@@ -29,15 +38,15 @@
 python3 -m pip install rssfixer
 ```
 
 ## Example
 
 Format for storing the links varies but I'll try and add more formats as I find them.
 
-### List
+### Simple list
 
 An example to generate a feed for [nccgroup][ncc] that have the links in a list:
 
 ```bash
 $ rssfixer --title nccgroup https://research.nccgroup.com/
 RSS feed created: rss_feed.xml
 ```
@@ -60,23 +69,36 @@
 
 An example for [truesec.com][tru]:
 
 ```bash
 rssfixer --json --quiet --output truesec.xml https://www.truesec.com/hub/blog
 ```
 
+### General HTML
+
+An example for [tripwire.com][tri]:
+
+```bash
+rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
+
+```
+
+
 ### Usage
 
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES] [--html-url HTML_URL] [--html-title HTML_TITLE]
-                [--html-title-class HTML_TITLE_CLASS] [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS] [--json] [--json-entries JSON_ENTRIES]
-                [--json-url JSON_URL] [--json-title JSON_TITLE] [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES]
+                [--html-url HTML_URL] [--html-title HTML_TITLE] [--html-title-class HTML_TITLE_CLASS]
+                [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS]
+                [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE]
+                [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
                 url
 
-Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list. Options are available to find links in other HTML elements or JSON strings.
+Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list.
+Options are available to find links in other HTML elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
@@ -106,13 +128,14 @@
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
   --list                Find entries in HTML <ul>-list (default)
 ```
 
 
   [bso]: https://www.crummy.com/software/BeautifulSoup/
-  [exa]: https://github.com/reuteras/rssfixer/blob/main/example/nccgroup.xml
-  [fge]: https://feedgen.kiesow.be/ 
+  [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
+  [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
+  [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
```

