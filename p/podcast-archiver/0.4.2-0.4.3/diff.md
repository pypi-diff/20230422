# Comparing `tmp/podcast_archiver-0.4.2.tar.gz` & `tmp/podcast_archiver-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-0.4.2.tar", max compression
+gzip compressed data, was "podcast_archiver-0.4.3.tar", max compression
```

## Comparing `podcast_archiver-0.4.2.tar` & `podcast_archiver-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1056 2023-04-21 15:02:10.848375 podcast_archiver-0.4.2/LICENSE
--rw-r--r--   0        0        0     4943 2023-04-22 14:50:21.743985 podcast_archiver-0.4.2/README.md
--rwxr-xr-x   0        0        0    15751 2023-04-21 20:38:07.066684 podcast_archiver-0.4.2/podcast_archiver.py
--rw-r--r--   0        0        0     1487 2023-04-22 15:16:17.321212 podcast_archiver-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5834 1970-01-01 00:00:00.000000 podcast_archiver-0.4.2/setup.py
--rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-22 15:52:07.926595 podcast_archiver-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4943 2023-04-22 15:52:07.926595 podcast_archiver-0.4.3/README.md
+-rwxr-xr-x   0        0        0    15774 2023-04-22 15:52:24.462695 podcast_archiver-0.4.3/podcast_archiver.py
+-rw-r--r--   0        0        0     1623 2023-04-22 15:52:24.462695 podcast_archiver-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 podcast_archiver-0.4.3/PKG-INFO
```

### Comparing `podcast_archiver-0.4.2/LICENSE` & `podcast_archiver-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.4.2/README.md` & `podcast_archiver-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `podcast_archiver-0.4.2/podcast_archiver.py` & `podcast_archiver-0.4.3/podcast_archiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from urllib.parse import urlparse
 from urllib.request import Request, urlopen
 
 import feedparser
 from dateutil.parser import parse as dateparse
 from feedparser import CharacterEncodingOverride
 
+__version__ = "0.4.3"
+
 
 class writeable_dir(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         prospective_dir = values
         if not path.isdir(prospective_dir):
             raise ArgumentTypeError(f"{prospective_dir} does not exist")
         if access(prospective_dir, W_OK):
```

### Comparing `podcast_archiver-0.4.2/pyproject.toml` & `podcast_archiver-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "0.4.2"
+version = "0.4.3"
 description = "Archive all episodes from your favorite podcasts"
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "podcast_archiver.py" }]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -15,14 +15,19 @@
     "Operating System :: POSIX :: Linux",
     "Topic :: Multimedia",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: System :: Archiving",
     "Topic :: Utilities",
 ]
 
+[tool.poetry-dynamic-versioning]
+enable = true
+vcs = "git"
+style = "semver"
+strict = true
 
 [tool.poetry.scripts]
 podcast-archiver = 'podcast_archiver:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dateutil = "^2.8.2"
@@ -62,9 +67,9 @@
 
 [tool.black]
 line-length = 120
 target-version = ['py39', 'py310', 'py311']
 
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `podcast_archiver-0.4.2/setup.py` & `podcast_archiver-0.4.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: podcast-archiver
+Version: 0.4.3
+Summary: Archive all episodes from your favorite podcasts
+License: MIT
+Author: Jan Willhaus
+Author-email: mail@janwillhaus.de
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Utilities
+Requires-Dist: feedparser (>=6.0.10,<7.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Description-Content-Type: text/markdown
 
-modules = \
-['podcast_archiver']
-install_requires = \
-['feedparser>=6.0.10,<7.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'tqdm>=4.65.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['podcast-archiver = podcast_archiver:main']}
-
-setup_kwargs = {
-    'name': 'podcast-archiver',
-    'version': '0.4.2',
-    'description': 'Archive all episodes from your favorite podcasts',
-    'long_description': '# Podcast Archiver\n\n<!-- markdownlint-disable MD033 MD013 -->\n<div align="center">\n\n![Podcast Archiver Logo](assets/icon.png)\n\n[![PyPI](https://img.shields.io/pypi/v/podcast-archiver.svg)](https://pypi.org/project/podcast-archiver/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/podcast-archiver.svg)](https://pypi.org/project/podcast-archiver/)\n\n[![Code Quality](https://app.codacy.com/project/badge/Grade/d0c31899a9964ccc82fa4080717d45a6)](https://app.codacy.com/gh/janw/podcast-archiver/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)\n\n[![Linter: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Dependency management: poetry](https://img.shields.io/badge/deps-poetry-blueviolet.svg)](https://poetry.eustace.io/docs/)\n\n</div>\n\nArchive all episodes from your favorite podcasts.\n\nThe archiver takes the feed URLs of your favorite podcasts and downloads all available episodes for you. Even those files "hidden" in a paged feed will be tapped, so you\'ll have an entire backup of the series. The archiver also supports updating an existing archive, so that it lends itself to be set up as a cronjob.\n\n## Outline\n\nIn my experience, very few full-fledged podcast clients are able to access a paged feed (following IETF RFC5005), so only the last few episodes of a podcast will be available to download. When you discover a podcast that has been around for quite a while, you\'ll have a hard time to follow the "gentle listener\'s duty" and listen to the whole archive. The script in this repository is supposed to help you acquiring every last episode of your new listening pleasure.\n\nBefore downloading any episode the function first fetches all available pages of the feed and prepares a list. That way, you will never miss any episode.\n\n## Setup\n\n### Python package\n\n`podcast-archiver` is Python 3.9+ compatible.\n\n```bash\n# Latest tagged/published version on PyPI:\npip install podcast-archiver\n\n# Latest master from GitHub:\npip install git+https://github.com/janw/podcast-archiver.git\n```\n\n### Docker image\n\nAlternatively `podcast-archiver` is available as a docker image as well:\n\n```bash\n# Latest tagged/published version, same as on PyPI:\ndocker run --rm ghcr.io/janw/podcast-archiver:latest\n\n# Latest master from GitHub:\ndocker run --rm ghcr.io/janw/podcast-archiver:edge\n```\n\n## Usage\n\nRun `podcast-archiver --help` for details on how to use it.\n\n### Full-fledged example\n\n```bash\npodcast-archiver -d ~/Music/Podcasts \\\n    --subdirs \\\n    --date-prefix \\\n    --progress \\\n    --verbose \\\n    -f http://logbuch-netzpolitik.de/feed/m4a \\\n    -f http://raumzeit-podcast.de/feed/m4a/ \\\n    -f https://feeds.lagedernation.org/feeds/ldn-mp3.xml\n```\n\n### Process the feed list from a file\n\nIf you have a larger list of podcasts and/or want to update the archive on a cronjob basis, the `-f` argument can be outsourced into a text file. The text file may contain one feed URL per line, looking like this:\n\n```bash\npodcast-archiver -d ~/Music/Podcasts -s -u -f feedlist.txt\n```\n\nwhere `feedlist.txt` contains the URLs as if entered into the command line:\n\n```text\n    http://logbuch-netzpolitik.de/feed/m4a\n    http://raumzeit-podcast.de/feed/m4a/\n    https://feeds.lagedernation.org/feeds/ldn-mp3.xml\n```\n\nThis way, you can easily add and remove feeds to the list and let the archiver fetch the newest episodes for example by adding it to your crontab.\n\n## Excursion: Unicode Normalization in Slugify\n\nThe `--slugify` option removes all ambiguous characters from folders and filenames used in the archiving process. The removal includes unicode normalization according to [Compatibility Decomposition](http://unicode.org/reports/tr15/tr15-18.html#Decomposition). What? Yeah, me too. I figured this is best seen in an example, so here\'s a fictitious episode name, and how it would be translated to an target filename using the Archiver:\n\n```text\nSPR001_Umlaute sind ausschließlich in schönen Sprachen/Dialekten zu finden.mp3\n```\n\nwill be turned into\n\n```text\nSPR001_Umlaute-sind-ausschlielich-in-schonen-SprachenDialekten-zu-finden.mp3\n```\n\nNote that "decorated" characters like `ö` are replaced with their basic counterparts (`o`), while somewhat ligatur-ish ones like `ß` (amongst most unessential punctuation) are removed entirely.\n\n## Todo\n\n* Add ability to define a preferred format on feeds that contain links for multiple audio codecs.\n* Add ability to define a range of episodes or time to download only episode from that point on or from there to the beginning or or or …\n* Add ability to choose a prefix episodes with the episode number (rarely necessary, since most podcasts feature some kind of episode numbering in the filename)\n* Add unittests\n',
-    'author': 'Jan Willhaus',
-    'author_email': 'mail@janwillhaus.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+# Podcast Archiver
 
+<!-- markdownlint-disable MD033 MD013 -->
+<div align="center">
+
+![Podcast Archiver Logo](assets/icon.png)
+
+[![PyPI](https://img.shields.io/pypi/v/podcast-archiver.svg)](https://pypi.org/project/podcast-archiver/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/podcast-archiver.svg)](https://pypi.org/project/podcast-archiver/)
+
+[![Code Quality](https://app.codacy.com/project/badge/Grade/d0c31899a9964ccc82fa4080717d45a6)](https://app.codacy.com/gh/janw/podcast-archiver/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+
+[![Linter: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Dependency management: poetry](https://img.shields.io/badge/deps-poetry-blueviolet.svg)](https://poetry.eustace.io/docs/)
+
+</div>
+
+Archive all episodes from your favorite podcasts.
+
+The archiver takes the feed URLs of your favorite podcasts and downloads all available episodes for you. Even those files "hidden" in a paged feed will be tapped, so you'll have an entire backup of the series. The archiver also supports updating an existing archive, so that it lends itself to be set up as a cronjob.
+
+## Outline
+
+In my experience, very few full-fledged podcast clients are able to access a paged feed (following IETF RFC5005), so only the last few episodes of a podcast will be available to download. When you discover a podcast that has been around for quite a while, you'll have a hard time to follow the "gentle listener's duty" and listen to the whole archive. The script in this repository is supposed to help you acquiring every last episode of your new listening pleasure.
+
+Before downloading any episode the function first fetches all available pages of the feed and prepares a list. That way, you will never miss any episode.
+
+## Setup
+
+### Python package
+
+`podcast-archiver` is Python 3.9+ compatible.
+
+```bash
+# Latest tagged/published version on PyPI:
+pip install podcast-archiver
+
+# Latest master from GitHub:
+pip install git+https://github.com/janw/podcast-archiver.git
+```
+
+### Docker image
+
+Alternatively `podcast-archiver` is available as a docker image as well:
+
+```bash
+# Latest tagged/published version, same as on PyPI:
+docker run --rm ghcr.io/janw/podcast-archiver:latest
+
+# Latest master from GitHub:
+docker run --rm ghcr.io/janw/podcast-archiver:edge
+```
+
+## Usage
+
+Run `podcast-archiver --help` for details on how to use it.
+
+### Full-fledged example
+
+```bash
+podcast-archiver -d ~/Music/Podcasts \
+    --subdirs \
+    --date-prefix \
+    --progress \
+    --verbose \
+    -f http://logbuch-netzpolitik.de/feed/m4a \
+    -f http://raumzeit-podcast.de/feed/m4a/ \
+    -f https://feeds.lagedernation.org/feeds/ldn-mp3.xml
+```
+
+### Process the feed list from a file
+
+If you have a larger list of podcasts and/or want to update the archive on a cronjob basis, the `-f` argument can be outsourced into a text file. The text file may contain one feed URL per line, looking like this:
+
+```bash
+podcast-archiver -d ~/Music/Podcasts -s -u -f feedlist.txt
+```
+
+where `feedlist.txt` contains the URLs as if entered into the command line:
+
+```text
+    http://logbuch-netzpolitik.de/feed/m4a
+    http://raumzeit-podcast.de/feed/m4a/
+    https://feeds.lagedernation.org/feeds/ldn-mp3.xml
+```
+
+This way, you can easily add and remove feeds to the list and let the archiver fetch the newest episodes for example by adding it to your crontab.
+
+## Excursion: Unicode Normalization in Slugify
+
+The `--slugify` option removes all ambiguous characters from folders and filenames used in the archiving process. The removal includes unicode normalization according to [Compatibility Decomposition](http://unicode.org/reports/tr15/tr15-18.html#Decomposition). What? Yeah, me too. I figured this is best seen in an example, so here's a fictitious episode name, and how it would be translated to an target filename using the Archiver:
+
+```text
+SPR001_Umlaute sind ausschließlich in schönen Sprachen/Dialekten zu finden.mp3
+```
+
+will be turned into
+
+```text
+SPR001_Umlaute-sind-ausschlielich-in-schonen-SprachenDialekten-zu-finden.mp3
+```
+
+Note that "decorated" characters like `ö` are replaced with their basic counterparts (`o`), while somewhat ligatur-ish ones like `ß` (amongst most unessential punctuation) are removed entirely.
+
+## Todo
+
+* Add ability to define a preferred format on feeds that contain links for multiple audio codecs.
+* Add ability to define a range of episodes or time to download only episode from that point on or from there to the beginning or or or …
+* Add ability to choose a prefix episodes with the episode number (rarely necessary, since most podcasts feature some kind of episode numbering in the filename)
+* Add unittests
 
-setup(**setup_kwargs)
```

