# Comparing `tmp/spotdl-4.1.6.tar.gz` & `tmp/spotdl-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl-4.1.6.tar", max compression
+gzip compressed data, was "spotdl-4.1.7.tar", max compression
```

## Comparing `spotdl-4.1.6.tar` & `spotdl-4.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1074 2023-04-17 19:57:40.066612 spotdl-4.1.6/LICENSE
--rw-r--r--   0        0        0     5921 2023-04-17 19:57:40.066612 spotdl-4.1.6/README.md
--rw-r--r--   0        0        0     2745 2023-04-17 19:57:40.070612 spotdl-4.1.6/pyproject.toml
--rw-r--r--   0        0        0     4668 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/__init__.py
--rw-r--r--   0        0        0      209 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/__main__.py
--rw-r--r--   0        0        0       58 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/_version.py
--rw-r--r--   0        0        0      186 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/__init__.py
--rw-r--r--   0        0        0      598 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/download.py
--rw-r--r--   0        0        0     3869 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/entry_point.py
--rw-r--r--   0        0        0     5995 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/meta.py
--rw-r--r--   0        0        0     2759 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/save.py
--rw-r--r--   0        0        0     4896 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/sync.py
--rw-r--r--   0        0        0     1702 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/url.py
--rw-r--r--   0        0        0     3041 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/console/web.py
--rw-r--r--   0        0        0       80 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/download/__init__.py
--rw-r--r--   0        0        0    26854 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/download/downloader.py
--rw-r--r--   0        0        0    13137 2023-04-17 19:57:40.070612 spotdl-4.1.6/spotdl/download/progress_handler.py
--rw-r--r--   0        0        0       54 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/__init__.py
--rw-r--r--   0        0        0      465 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/audio/__init__.py
--rw-r--r--   0        0        0    10831 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/audio/base.py
--rw-r--r--   0        0        0     2665 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     1840 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/audio/youtube.py
--rw-r--r--   0        0        0     2789 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3304 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3529 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/base.py
--rw-r--r--   0        0        0     3091 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/genius.py
--rw-r--r--   0        0        0     2765 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     1689 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/album.py
--rw-r--r--   0        0        0     3101 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/artist.py
--rw-r--r--   0        0        0     3615 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/options.py
--rw-r--r--   0        0        0     4199 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/playlist.py
--rw-r--r--   0        0        0     2186 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/result.py
--rw-r--r--   0        0        0     3230 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/saved.py
--rw-r--r--   0        0        0     9758 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/types/song.py
--rw-r--r--   0        0        0      103 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/__init__.py
--rw-r--r--   0        0        0     1001 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/archive.py
--rw-r--r--   0        0        0    18452 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/arguments.py
--rw-r--r--   0        0        0     6650 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/config.py
--rw-r--r--   0        0        0     3109 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/console.py
--rw-r--r--   0        0        0      571 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/downloader.py
--rw-r--r--   0        0        0    11688 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/ffmpeg.py
--rw-r--r--   0        0        0    14159 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/formatter.py
--rw-r--r--   0        0        0     7018 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/github.py
--rw-r--r--   0        0        0     5364 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/logging.py
--rw-r--r--   0        0        0      940 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/lrc.py
--rw-r--r--   0        0        0     4144 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/m3u.py
--rw-r--r--   0        0        0    23312 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/matching.py
--rw-r--r--   0        0        0    15525 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/metadata.py
--rw-r--r--   0        0        0    15207 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/search.py
--rw-r--r--   0        0        0     5660 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/spotify.py
--rw-r--r--   0        0        0    28221 2023-04-17 19:57:40.074612 spotdl-4.1.6/spotdl/utils/static.py
--rw-r--r--   0        0        0    15281 2023-04-17 19:57:40.078612 spotdl-4.1.6/spotdl/utils/web.py
--rw-r--r--   0        0        0     8150 1970-01-01 00:00:00.000000 spotdl-4.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-22 18:24:04.582924 spotdl-4.1.7/LICENSE
+-rw-r--r--   0        0        0     5977 2023-04-22 18:24:04.582924 spotdl-4.1.7/README.md
+-rw-r--r--   0        0        0     2746 2023-04-22 18:24:04.586924 spotdl-4.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4668 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/__main__.py
+-rw-r--r--   0        0        0       58 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/_version.py
+-rw-r--r--   0        0        0      186 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/download.py
+-rw-r--r--   0        0        0     4120 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/entry_point.py
+-rw-r--r--   0        0        0     5995 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/meta.py
+-rw-r--r--   0        0        0     2759 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/save.py
+-rw-r--r--   0        0        0     5067 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/sync.py
+-rw-r--r--   0        0        0     1702 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/url.py
+-rw-r--r--   0        0        0     3041 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/web.py
+-rw-r--r--   0        0        0       80 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/__init__.py
+-rw-r--r--   0        0        0    27039 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/downloader.py
+-rw-r--r--   0        0        0    13137 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/__init__.py
+-rw-r--r--   0        0        0    11137 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/base.py
+-rw-r--r--   0        0        0     2665 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     1840 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2789 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      382 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3304 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3529 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3091 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     2765 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     1689 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/album.py
+-rw-r--r--   0        0        0     3101 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/artist.py
+-rw-r--r--   0        0        0     3871 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/options.py
+-rw-r--r--   0        0        0     4199 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/playlist.py
+-rw-r--r--   0        0        0     2186 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/result.py
+-rw-r--r--   0        0        0     3230 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/saved.py
+-rw-r--r--   0        0        0     9758 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/song.py
+-rw-r--r--   0        0        0      103 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/archive.py
+-rw-r--r--   0        0        0    19690 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/arguments.py
+-rw-r--r--   0        0        0     6994 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/config.py
+-rw-r--r--   0        0        0     3109 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/console.py
+-rw-r--r--   0        0        0      571 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/downloader.py
+-rw-r--r--   0        0        0    11688 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/ffmpeg.py
+-rw-r--r--   0        0        0    14355 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/formatter.py
+-rw-r--r--   0        0        0     7018 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/github.py
+-rw-r--r--   0        0        0     5364 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/logging.py
+-rw-r--r--   0        0        0      940 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/lrc.py
+-rw-r--r--   0        0        0     4144 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/m3u.py
+-rw-r--r--   0        0        0    23312 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/matching.py
+-rw-r--r--   0        0        0    15525 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/metadata.py
+-rw-r--r--   0        0        0    15152 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/search.py
+-rw-r--r--   0        0        0     6870 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/static.py
+-rw-r--r--   0        0        0    15281 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/web.py
+-rw-r--r--   0        0        0     8199 1970-01-01 00:00:00.000000 spotdl-4.1.7/PKG-INFO
```

### Comparing `spotdl-4.1.6/LICENSE` & `spotdl-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/README.md` & `spotdl-4.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 ## Contributing
 
 Interested in contributing? Check out our [CONTRIBUTING.md](docs/CONTRIBUTING.md) to find
 resources around contributing along with a guide on how to set up a development environment.
 
 ## Donate
 
-### xnetcat
+help support the development and maintenance of the software ❤️
 
 [![paypal](https://img.shields.io/badge/paypal-%2300457C.svg?&style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/kko7)
 [![kofi](https://img.shields.io/badge/kofi-%23F16061.svg?&style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/xnetcat)
 
 ## License
 
 This project is Licensed under the [MIT](/LICENSE) License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spotdl-4.1.6/pyproject.toml` & `spotdl-4.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl"
-version = "4.1.6"
+version = "4.1.7"
 description = "Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/spotDL/spotify-downloader.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
@@ -24,64 +24,64 @@
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<3.12"
 
-spotipy = "^2.22.1"
+spotipy = "^2.23.0"
 ytmusicapi = [
     {version = "^0.22.0", python = "<3.8"},
     {version = "^0.24.0", python = ">=3.8"},
 ]
 pytube = "^12.1.3"
 yt-dlp = "^2023.3.4"
 mutagen = "^1.46.0"
-rich = "^13.3.3"
-beautifulsoup4 = "^4.12.1"
+rich = "^13.3.4"
+beautifulsoup4 = "^4.12.2"
 requests = "^2.28.2"
-rapidfuzz = "^2.15.0"
+rapidfuzz = "==2.15.1"
 python-slugify = {extras = ["unidecode"], version = "^8.0.1"}
-uvicorn = "^0.20.0"
+uvicorn = "^0.21.1"
 pydantic = "^1.10.7"
-fastapi = "^0.89.1"
-platformdirs = "^2.6.2"
+fastapi = "^0.95.1"
+platformdirs = "^3.2.0"
 pykakasi = "^2.2.1"
 syncedlyrics = "0.4.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-vcr = "^1.0.2"
-pyfakefs = "^5.2.0"
+pyfakefs = "^5.2.2"
 pytest-cov = "^4.0.0"
 pytest-subprocess = "^1.5.0"
-pytest-asyncio = "^0.20.3"
-mypy = "^0.991"
+pytest-asyncio = "^0.21.0"
+mypy = "^1.2.0"
 pylint = "^2.17.2"
-black = "^22.12.0"
+black = "^23.3.0"
 mdformat-gfm = "^0.3.5"
 types-orjson = "^3.6.2"
-types-python-slugify = "^7.0.0.1"
+types-python-slugify = "^8.0.0.2"
 types-requests = "^2.28.11.17"
-types-setuptools = "^65.7.0.4"
+types-setuptools = "^67.6.0.8"
 types-toml = "^0.10.8.6"
-types-ujson = "^5.7.0.1"
-pyinstaller = "^5.9.0"
+types-ujson = "^5.7.0.3"
+pyinstaller = "^5.10.1"
 mkdocs = "^1.4.2"
 isort = [
     {version = "^5.11.4", python = "<3.8"},
     {version = "^5.12.0", python = ">=3.8"},
 ]
 dill = "^0.3.6"
-mkdocs-material = "^9.1.5"
-mkdocstrings = "^0.19.1"
-mkdocstrings-python = "^0.8.3"
-pymdown-extensions = "^9.10"
+mkdocs-material = "^9.1.7"
+mkdocstrings = "^0.21.2"
+mkdocstrings-python = "^0.9.0"
+pymdown-extensions = "^9.11"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 
 [tool.poetry.scripts]
 spotdl = "spotdl:console_entry_point"
```

### Comparing `spotdl-4.1.6/spotdl/__init__.py` & `spotdl-4.1.7/spotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/console/download.py` & `spotdl-4.1.7/spotdl/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/console/entry_point.py` & `spotdl-4.1.7/spotdl/console/entry_point.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from spotdl.console.web import web
 from spotdl.download.downloader import Downloader, DownloaderError
 from spotdl.utils.arguments import parse_arguments
 from spotdl.utils.config import create_settings
 from spotdl.utils.console import ACTIONS, generate_initial_config, is_executable
 from spotdl.utils.ffmpeg import FFmpegError, download_ffmpeg, is_ffmpeg_installed
 from spotdl.utils.logging import init_logging
-from spotdl.utils.spotify import SpotifyClient, SpotifyError
+from spotdl.utils.spotify import SpotifyClient, SpotifyError, save_spotify_cache
 
 __all__ = ["console_entry_point", "OPERATIONS"]
 
 OPERATIONS = {
     "download": download,
     "sync": sync,
     "save": save,
@@ -73,14 +73,15 @@
         raise FFmpegError(
             "FFmpeg is not installed. Please run `spotdl --download-ffmpeg` to install it, "
             "or `spotdl --ffmpeg /path/to/ffmpeg` to specify the path to ffmpeg."
         )
 
     # Initialize spotify client
     SpotifyClient.init(**spotify_settings)
+    spotify_client = SpotifyClient()
 
     # If the application is frozen start web ui
     # or if the operation is `web`
     if is_executable() or arguments.operation == "web":
         # Start web ui
         web(web_settings, downloader_settings)
 
@@ -104,14 +105,17 @@
         )
 
     # Initialize the downloader
     # for download, load and preload operations
     downloader = Downloader(downloader_settings)
 
     def graceful_exit(_signal, _frame):
+        if spotify_settings["use_cache_file"]:
+            save_spotify_cache(spotify_client.cache)
+
         downloader.progress_handler.close()
         sys.exit(0)
 
     signal.signal(signal.SIGINT, graceful_exit)
     signal.signal(signal.SIGTERM, graceful_exit)
 
     try:
@@ -124,10 +128,13 @@
     except Exception:
         downloader.progress_handler.close()
 
         logger.exception("An error occurred")
 
         sys.exit(1)
 
+    if spotify_settings["use_cache_file"]:
+        save_spotify_cache(spotify_client.cache)
+
     downloader.progress_handler.close()
 
     return None
```

### Comparing `spotdl-4.1.6/spotdl/console/meta.py` & `spotdl-4.1.7/spotdl/console/meta.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/console/save.py` & `spotdl-4.1.7/spotdl/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/console/sync.py` & `spotdl-4.1.7/spotdl/console/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,30 +103,33 @@
                 downloader.settings["restrict"],
             )
             old_files.append((file_name, entry["url"]))
 
         new_urls = [song.url for song in songs_playlist]
 
         # Delete all song files whose URL is no longer part of the latest playlist
-        to_delete = [path for (path, url) in old_files if url not in new_urls]
+        if not downloader.settings["sync_without_deleting"]:
+            to_delete = [path for (path, url) in old_files if url not in new_urls]
 
-        for file in to_delete:
-            if file.exists():
-                logger.info("Deleting %s", file)
-                try:
-                    file.unlink()
-                except (PermissionError, OSError) as exc:
-                    logger.debug("Could not remove temp file: %s, error: %s", file, exc)
-            else:
-                logger.debug("%s does not exist.", file)
+            for file in to_delete:
+                if file.exists():
+                    logger.info("Deleting %s", file)
+                    try:
+                        file.unlink()
+                    except (PermissionError, OSError) as exc:
+                        logger.debug(
+                            "Could not remove temp file: %s, error: %s", file, exc
+                        )
+                else:
+                    logger.debug("%s does not exist.", file)
 
-        if len(to_delete) == 0:
-            logger.info("Nothing to delete...")
-        else:
-            logger.info("%s old songs were deleted.", len(to_delete))
+            if len(to_delete) == 0:
+                logger.info("Nothing to delete...")
+            else:
+                logger.info("%s old songs were deleted.", len(to_delete))
 
         if m3u_file:
             gen_m3u_files(
                 songs_playlist,
                 m3u_file,
                 downloader.settings["output"],
                 downloader.settings["format"],
```

### Comparing `spotdl-4.1.6/spotdl/console/url.py` & `spotdl-4.1.7/spotdl/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/console/web.py` & `spotdl-4.1.7/spotdl/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/download/downloader.py` & `spotdl-4.1.7/spotdl/download/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         - song: The song to search for.
 
         ### Returns
         - tuple with download url and audio provider if successful.
         """
 
         for audio_provider in self.audio_providers:
-            url = audio_provider.search(song)
+            url = audio_provider.search(song, self.settings["only_verified_results"])
             if url:
                 return url
 
             logger.debug("%s failed to find %s", audio_provider.name, song.display_name)
 
         raise LookupError(f"No results found for song: {song.display_name}")
 
@@ -375,46 +375,48 @@
 
         ### Notes
         - This function is synchronous.
         """
 
         # Check if song has name/artist and url/song_id
         if not (song.name and (song.artists or song.artist)) and not (
-            song.url and song.song_id
+            song.url or song.song_id
         ):
             logger.error("Song is missing required fields: %s", song.display_name)
             self.errors.append(f"Song is missing required fields: {song.display_name}")
 
             return song, None
 
-        # Initalize the progress tracker
-        display_progress_tracker = self.progress_handler.get_new_tracker(song)
-
+        reinitialized = False
         try:
-            reinitialized = False
-            try:
-                # Create the output file path
-                output_file = create_file_name(
-                    song,
-                    self.settings["output"],
-                    self.settings["format"],
-                    self.settings["restrict"],
-                )
-            except Exception:
-                song = reinit_song(song)
+            # Create the output file path
+            output_file = create_file_name(
+                song=song,
+                template=self.settings["output"],
+                file_extension=self.settings["format"],
+                restrict=self.settings["restrict"],
+                file_name_length=self.settings["max_filename_length"],
+            )
+        except Exception:
+            song = reinit_song(song)
 
-                output_file = create_file_name(
-                    song,
-                    self.settings["output"],
-                    self.settings["format"],
-                    self.settings["restrict"],
-                )
+            output_file = create_file_name(
+                song=song,
+                template=self.settings["output"],
+                file_extension=self.settings["format"],
+                restrict=self.settings["restrict"],
+                file_name_length=self.settings["max_filename_length"],
+            )
 
-                reinitialized = True
+            reinitialized = True
 
+        # Initalize the progress tracker
+        display_progress_tracker = self.progress_handler.get_new_tracker(song)
+
+        try:
             # Create the temp folder path
             temp_folder = get_temp_path()
 
             # Check if there is an already existing song file, with the same spotify URL in its
             # metadata, but saved under a different name. If so, save its path.
             dup_song_paths: List[Path] = self.known_songs.get(song.url, [])
```

### Comparing `spotdl-4.1.6/spotdl/download/progress_handler.py` & `spotdl-4.1.7/spotdl/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/audio/base.py` & `spotdl-4.1.7/spotdl/providers/audio/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         - The number of views.
         """
 
         data = self.get_download_metadata(url)
 
         return data["view_count"]
 
-    def search(self, song: Song) -> Optional[str]:
+    def search(self, song: Song, only_verified: bool = False) -> Optional[str]:
         """
         Search for a song and return best match.
 
         ### Arguments
         - song: The song to search for.
 
         ### Returns
@@ -160,14 +160,17 @@
 
         # search for song using isrc if it's available
         if song.isrc and self.SUPPORTS_ISRC and not self.search_query:
             isrc_results = self.get_results(
                 song.isrc, filter="songs", ignore_spelling=True
             )
 
+            if only_verified:
+                isrc_results = [result for result in isrc_results if result.verified]
+
             isrc_urls = [result.url for result in isrc_results]
             sorted_isrc_results = order_results(isrc_results, song, self.search_query)
             logger.debug(
                 "[%s] Found %s results for ISRC %s",
                 song.song_id,
                 len(isrc_results),
                 song.isrc,
@@ -197,14 +200,20 @@
                         return best_isrc[0].url
 
         results: Dict[Result, float] = {}
         for options in self.GET_RESULTS_OPTS:
             # Query YTM by songs only first, this way if we get correct result on the first try
             # we don't have to make another request
             search_results = self.get_results(search_query, **options)
+
+            if only_verified:
+                search_results = [
+                    result for result in search_results if result.verified
+                ]
+
             logger.debug(
                 "[%s] Found %s results for search query %s with options %s",
                 song.song_id,
                 len(search_results),
                 search_query,
                 options,
             )
```

### Comparing `spotdl-4.1.6/spotdl/providers/audio/sliderkz.py` & `spotdl-4.1.7/spotdl/providers/audio/sliderkz.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/audio/youtube.py` & `spotdl-4.1.7/spotdl/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/audio/ytmusic.py` & `spotdl-4.1.7/spotdl/providers/audio/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/lyrics/azlyrics.py` & `spotdl-4.1.7/spotdl/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/lyrics/base.py` & `spotdl-4.1.7/spotdl/providers/lyrics/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/lyrics/genius.py` & `spotdl-4.1.7/spotdl/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/lyrics/musixmatch.py` & `spotdl-4.1.7/spotdl/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/providers/lyrics/synced.py` & `spotdl-4.1.7/spotdl/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/album.py` & `spotdl-4.1.7/spotdl/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/artist.py` & `spotdl-4.1.7/spotdl/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/options.py` & `spotdl-4.1.7/spotdl/types/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     client_secret: str
     auth_token: Optional[str]
     user_auth: bool
     headless: bool
     cache_path: str
     no_cache: bool
     max_retries: int
+    use_cache_file: bool
 
 
 class DownloaderOptions(TypedDict):
     """
     Options used for initializing the Downloader.
     """
 
@@ -66,14 +67,17 @@
     simple_tui: bool
     fetch_albums: bool
     id3_separator: str
     ytm_data: bool
     add_unavailable: bool
     generate_lrc: bool
     force_update_metadata: bool
+    only_verified_results: bool
+    sync_without_deleting: bool
+    max_filename_length: Optional[int]
 
 
 class WebOptions(TypedDict):
     """
     Options used for initializing the Web server.
     """
 
@@ -100,14 +104,15 @@
     client_secret: str
     auth_token: Optional[str]
     user_auth: bool
     headless: bool
     cache_path: str
     no_cache: bool
     max_retries: int
+    use_cache_file: bool
 
 
 class DownloaderOptionalOptions(TypedDict, total=False):
     """
     Options used for initializing the Downloader.
     """
 
@@ -137,14 +142,17 @@
     simple_tui: bool
     fetch_albums: bool
     id3_separator: str
     ytm_data: bool
     add_unavailable: bool
     generate_lrc: bool
     force_update_metadata: bool
+    only_verified_results: bool
+    sync_without_deleting: bool
+    max_filename_length: Optional[int]
 
 
 class WebOptionalOptions(TypedDict, total=False):
     """
     Options used for initializing the Web server.
     """
```

### Comparing `spotdl-4.1.6/spotdl/types/playlist.py` & `spotdl-4.1.7/spotdl/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/result.py` & `spotdl-4.1.7/spotdl/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/saved.py` & `spotdl-4.1.7/spotdl/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/types/song.py` & `spotdl-4.1.7/spotdl/types/song.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/archive.py` & `spotdl-4.1.7/spotdl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/arguments.py` & `spotdl-4.1.7/spotdl/utils/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,22 @@
         "--dont-filter-results",
         dest="filter_results",
         action="store_const",
         const=False,
         help="Disable filtering results.",
     )
 
+    # Add use only verified results argument
+    parser.add_argument(
+        "--only-verified-results",
+        action="store_const",
+        const=True,
+        help="Use only verified results. (Not all providers support this)",
+    )
+
 
 def parse_spotify_options(parser: _ArgumentGroup):
     """
     Parse spotify options from the command line.
 
     ### Arguments
     - parser: The argument parser to add the options to.
@@ -213,14 +221,29 @@
     parser.add_argument(
         "--headless",
         action="store_const",
         const=True,
         help="Run in headless mode.",
     )
 
+    # Add use cache file argument
+    parser.add_argument(
+        "--use-cache-file",
+        action="store_const",
+        const=True,
+        help=(
+            "Use the cache file to get metadata. "
+            "It's located under C:\\Users\\user\\.spotdl\\.spotify_cache "
+            "or ~/.spotdl/.spotify_cache under linux. "
+            "It only caches tracks and "
+            "gets updated whenever spotDL gets metadata from Spotify. "
+            "(It may provide outdated metadata use with caution)"
+        ),
+    )
+
 
 def parse_ffmpeg_options(parser: _ArgumentGroup):
     """
     Parse ffmpeg options from the command line.
 
     ### Arguments
     - parser: The argument parser to add the options to.
@@ -464,14 +487,32 @@
     parser.add_argument(
         "--force-update-metadata",
         action="store_const",
         const=True,
         help="Force update metadata for songs that already have metadata.",
     )
 
+    # Sync without deleting
+    parser.add_argument(
+        "--sync-without-deleting",
+        action="store_const",
+        const=True,
+        help="Sync without deleting songs that are not in the query.",
+    )
+
+    # Max file name length
+    parser.add_argument(
+        "--max-filename-length",
+        type=int,
+        help=(
+            "Max file name length. "
+            "(This won't override the max file name length enforced by the OS)"
+        ),
+    )
+
 
 def parse_web_options(parser: _ArgumentGroup):
     """
     Parse web options from the command line.
 
     ### Arguments
     - parser: The argument parser to add the options to.
```

### Comparing `spotdl-4.1.6/spotdl/utils/config.py` & `spotdl-4.1.7/spotdl/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,25 @@
     ### Returns
     - The path to the spotipy cache file.
     """
 
     return get_spotdl_path() / ".spotipy"
 
 
+def get_spotify_cache_path() -> Path:
+    """
+    Get the path to the spotify cache folder.
+
+    ### Returns
+    - The path to the spotipy cache file.
+    """
+
+    return get_spotdl_path() / ".spotify_cache"
+
+
 def get_temp_path() -> Path:
     """
     Get the path to the temp folder.
 
     ### Returns
     - The path to the temp folder.
     """
@@ -224,14 +235,15 @@
     "client_secret": "212476d9b0f3472eaa762d90b19b0ba8",
     "auth_token": None,
     "user_auth": False,
     "headless": False,
     "cache_path": str(get_cache_path()),
     "no_cache": False,
     "max_retries": 3,
+    "use_cache_file": False,
 }
 
 DOWNLOADER_OPTIONS: DownloaderOptions = {
     "audio_providers": ["youtube-music"],
     "lyrics_providers": ["genius", "azlyrics", "musixmatch"],
     "playlist_numbering": False,
     "scan_for_songs": False,
@@ -257,14 +269,17 @@
     "simple_tui": False,
     "fetch_albums": False,
     "id3_separator": "/",
     "ytm_data": False,
     "add_unavailable": False,
     "generate_lrc": False,
     "force_update_metadata": False,
+    "only_verified_results": False,
+    "sync_without_deleting": False,
+    "max_filename_length": None,
 }
 
 WEB_OPTIONS: WebOptions = {
     "web_use_output_dir": False,
     "port": 8800,
     "host": "localhost",
     "keep_alive": False,
```

### Comparing `spotdl-4.1.6/spotdl/utils/console.py` & `spotdl-4.1.7/spotdl/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/downloader.py` & `spotdl-4.1.7/spotdl/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/ffmpeg.py` & `spotdl-4.1.7/spotdl/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/formatter.py` & `spotdl-4.1.7/spotdl/utils/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,24 +282,26 @@
 
 def create_file_name(
     song: Song,
     template: str,
     file_extension: str,
     restrict: bool = False,
     short: bool = False,
+    file_name_length: Optional[int] = None,
 ) -> Path:
     """
     Create the file name for the song, by replacing template variables with the actual values.
 
     ### Arguments
     - song: the song object
     - template: the template string
     - file_extension: the file extension to use
     - restrict: whether to sanitize the filename
     - short: whether to use the short version of the template
+    - file_name_length: the maximum length of the file name
 
     ### Returns
     - the formatted string as a Path object
     """
 
     # If template does not contain any of the keys,
     # append {artists} - {title}.{output-ext} to it
@@ -336,39 +338,41 @@
             santitized_parts.append(match.group(0))
         else:
             santitized_parts.append(part)
 
     # Join the parts of the path
     file = Path(*santitized_parts)
 
-    # Check if the file name length is greater than 255
-    if len(file.name) < 255:
+    length_limit = file_name_length or 255
+
+    # Check if the file name length is greater than the limit
+    if len(file.name) < length_limit:
         # Restrict the filename if needed
         if restrict:
             return restrict_filename(file)
 
         return file
 
-    # If the file name length is greater than 255,
+    # If the file name length is greater than ,
     # and we are already using the short version of the template,
     # fallback to default template
     if short is True:
         # Path template is already short, but we still can't create a file
         # so we reduce it even further
         if template == "{artist} - {title}.{output-ext}":
-            if len(song.name) > 240:
+            if len(song.name) > (length_limit * 0.80):
                 logger.warning(
                     "%s: File name is too long. Using only part of the song title.",
                     song.display_name,
                 )
 
                 name_parts = song.name.split(" ")
                 new_name = ""
                 for part in name_parts:
-                    if len(new_name) + len(part) < 240:
+                    if len(new_name) + len(part) < (length_limit * 0.80):
                         new_name += part + " "
                     else:
                         break
 
                 song.name = new_name.strip()
             else:
                 logger.warning(
```

### Comparing `spotdl-4.1.6/spotdl/utils/github.py` & `spotdl-4.1.7/spotdl/utils/github.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/logging.py` & `spotdl-4.1.7/spotdl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/lrc.py` & `spotdl-4.1.7/spotdl/utils/lrc.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/m3u.py` & `spotdl-4.1.7/spotdl/utils/m3u.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/matching.py` & `spotdl-4.1.7/spotdl/utils/matching.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/metadata.py` & `spotdl-4.1.7/spotdl/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/search.py` & `spotdl-4.1.7/spotdl/utils/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,15 +274,14 @@
 def reinit_song(song: Song) -> Song:
     """
     Update song object with new data
     from Spotify
 
     ### Arguments
     - song: Song object
-    - playlist_numbering: bool, default value is False
 
     ### Returns
     - Updated song object
     """
 
     data = song.json
     if data.get("url"):
```

### Comparing `spotdl-4.1.6/spotdl/utils/spotify.py` & `spotdl-4.1.7/spotdl/utils/spotify.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 
 ```python
 import spotdl.utils.spotify
 spotify.Spotify.init(client_id, client_secret)
 ```
 """
 
-from json import dumps
+import json
+import logging
 from typing import Dict, Optional
 
 import requests
 from spotipy import Spotify
 from spotipy.cache_handler import CacheFileHandler, MemoryCacheHandler
 from spotipy.oauth2 import SpotifyClientCredentials, SpotifyOAuth
 
-from spotdl.utils.config import get_cache_path
+from spotdl.utils.config import get_cache_path, get_spotify_cache_path
 
 __all__ = [
     "SpotifyError",
     "SpotifyClient",
+    "save_spotify_cache",
 ]
 
+logger = logging.getLogger(__name__)
+
 
 class SpotifyError(Exception):
     """
     Base class for all exceptions related to SpotifyClient.
     """
 
 
@@ -58,14 +62,15 @@
         self,
         client_id: str,
         client_secret: str,
         user_auth: bool = False,
         no_cache: bool = False,
         headless: bool = False,
         max_retries: int = 3,
+        use_cache_file: bool = False,
         auth_token: Optional[str] = None,
         cache_path: Optional[str] = None,
     ) -> "Singleton":
         """
         Initializes the SpotifyClient.
 
         ### Arguments
@@ -111,14 +116,15 @@
             )
         if auth_token is not None:
             credential_manager = None
 
         self.user_auth = user_auth
         self.no_cache = no_cache
         self.max_retries = max_retries
+        self.use_cache_file = use_cache_file
 
         # Create instance
         self._instance = super().__call__(
             auth=auth_token,
             auth_manager=credential_manager,
             status_forcelist=(429, 500, 502, 503, 504, 404),
         )
@@ -145,14 +151,24 @@
         - auth: The access token to use.
         - auth_manager: The auth manager to use.
         """
 
         super().__init__(*args, **kwargs)
         self._initialized = True
 
+        use_cache_file: bool = self.use_cache_file  # type: ignore # pylint: disable=E1101
+        cache_file_loc = get_spotify_cache_path()
+
+        if use_cache_file and cache_file_loc.exists():
+            with open(cache_file_loc, "r", encoding="utf-8") as cache_file:
+                self.cache = json.load(cache_file)
+        elif use_cache_file:
+            with open(cache_file_loc, "w", encoding="utf-8") as cache_file:
+                json.dump(self.cache, cache_file)
+
     def _get(self, url, args=None, payload=None, **kwargs):
         """
         Overrides the get method of the SpotifyClient.
         Allows us to cache requests
         """
 
         use_cache = not self.no_cache  # type: ignore # pylint: disable=E1101
@@ -160,16 +176,16 @@
         if args:
             kwargs.update(args)
 
         cache_key = None
         if use_cache:
             key_obj = dict(kwargs)
             key_obj["url"] = url
-            key_obj["data"] = dumps(payload)
-            cache_key = dumps(key_obj)
+            key_obj["data"] = json.dumps(payload)
+            cache_key = json.dumps(key_obj)
             if self.cache.get(cache_key) is not None:
                 return self.cache[cache_key]
 
         # Wrap in a try-except and retry up to `retries` times.
         response = None
         retries = self.max_retries  # type: ignore # pylint: disable=E1101
         while response is None:
@@ -180,7 +196,30 @@
                 if retries <= 0:
                     raise exc
 
         if use_cache and cache_key is not None:
             self.cache[cache_key] = response
 
         return response
+
+
+def save_spotify_cache(cache: Dict[str, Optional[Dict]]):
+    """
+    Saves the Spotify cache to a file.
+
+    ### Arguments
+    - cache: The cache to save.
+    """
+
+    cache_file_loc = get_spotify_cache_path()
+
+    logger.debug("Saving Spotify cache to %s", cache_file_loc)
+
+    # Only cache tracks
+    cache = {
+        key: value
+        for key, value in cache.items()
+        if value is not None and '"url": "tracks/' in key
+    }
+
+    with open(cache_file_loc, "w", encoding="utf-8") as cache_file:
+        json.dump(cache, cache_file)
```

### Comparing `spotdl-4.1.6/spotdl/utils/static.py` & `spotdl-4.1.7/spotdl/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/spotdl/utils/web.py` & `spotdl-4.1.7/spotdl/utils/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.6/PKG-INFO` & `spotdl-4.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl
-Version: 4.1.6
+Version: 4.1.7
 Summary: Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
@@ -23,29 +23,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Utilities
-Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
-Requires-Dist: fastapi (>=0.89.1,<0.90.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
-Requires-Dist: platformdirs (>=2.6.2,<3.0.0)
+Requires-Dist: platformdirs (>=3.2.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pykakasi (>=2.2.1,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
-Requires-Dist: rapidfuzz (>=2.15.0,<3.0.0)
+Requires-Dist: rapidfuzz (==2.15.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.3.3,<14.0.0)
-Requires-Dist: spotipy (>=2.22.1,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: spotipy (>=2.23.0,<3.0.0)
 Requires-Dist: syncedlyrics (==0.4.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Requires-Dist: ytmusicapi (>=0.22.0,<0.23.0) ; python_version < "3.8"
 Requires-Dist: ytmusicapi (>=0.24.0,<0.25.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://spotdl.rtfd.io/en/latest/
 Project-URL: Repository, https://github.com/spotDL/spotify-downloader.git
 Description-Content-Type: text/markdown
 
@@ -196,15 +196,15 @@
 ## Contributing
 
 Interested in contributing? Check out our [CONTRIBUTING.md](docs/CONTRIBUTING.md) to find
 resources around contributing along with a guide on how to set up a development environment.
 
 ## Donate
 
-### xnetcat
+help support the development and maintenance of the software ❤️
 
 [![paypal](https://img.shields.io/badge/paypal-%2300457C.svg?&style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/kko7)
 [![kofi](https://img.shields.io/badge/kofi-%23F16061.svg?&style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/xnetcat)
 
 ## License
 
 This project is Licensed under the [MIT](/LICENSE) License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

