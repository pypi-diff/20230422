# Comparing `tmp/discord-rich-help.py-0.1.0.tar.gz` & `tmp/discord-rich-help.py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-rich-help.py-0.1.0.tar", last modified: Sat Apr  1 07:19:51 2023, max compression
+gzip compressed data, was "discord-rich-help.py-0.1.1.tar", last modified: Sat Apr 22 09:26:47 2023, max compression
```

## Comparing `discord-rich-help.py-0.1.0.tar` & `discord-rich-help.py-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.825556 discord-rich-help.py-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.821556 discord-rich-help.py-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.821556 discord-rich-help.py-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-01 07:19:51.825556 discord-rich-help.py-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.821556 discord-rich-help.py-0.1.0/discord_rich_help/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/discord_rich_help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/discord_rich_help/help.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/discord_rich_help/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/discord_rich_help/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/discord_rich_help/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.821556 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-01 07:19:51.000000 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-01 07:19:51.000000 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 07:19:51.000000 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-01 07:19:51.000000 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-01 07:19:51.000000 discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 07:19:51.825556 discord-rich-help.py-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:51.821556 discord-rich-help.py-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 07:19:37.000000 discord-rich-help.py-0.1.0/tests/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.966437 discord-rich-help.py-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.966437 discord-rich-help.py-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/discord_rich_help/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/discord_rich_help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/discord_rich_help/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/discord_rich_help/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/discord_rich_help/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/discord_rich_help/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-22 09:26:47.000000 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-22 09:26:47.000000 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:26:47.000000 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-22 09:26:47.000000 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 09:26:47.000000 discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:47.970437 discord-rich-help.py-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:26:30.000000 discord-rich-help.py-0.1.1/tests/.gitkeep
```

### Comparing `discord-rich-help.py-0.1.0/.github/workflows/build.yaml` & `discord-rich-help.py-0.1.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/.github/workflows/release.yaml` & `discord-rich-help.py-0.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/.github/workflows/test.yaml` & `discord-rich-help.py-0.1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/.gitignore` & `discord-rich-help.py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/LICENSE` & `discord-rich-help.py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/PKG-INFO` & `discord-rich-help.py-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: discord-rich-help.py
-Version: 0.1.0
-Summary: The extension which make a rich-help command for discord.py
+Version: 0.1.1
+Summary: An extension which makes a rich-help command for discord.py
 Author-email: PescadoGames <official@pescadogames.com>
 Maintainer-email: Awayume <dev@awayume.jp>
 License: MIT License
 Project-URL: Repository, https://github.com/PescadoGames/discord-rich-help.py
 Project-URL: Documentation, https://github.com/PescadoGames/discord-rich-help.py/wiki
 Project-URL: Bug Tracker, https://github.com/PescadoGames/discord_rich_help.py/issues
 Keywords: discord,discord.py
@@ -36,15 +36,15 @@
 .. image:: https://img.shields.io/pypi/v/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI supported Python versions
 
-The extension which make a rich-help command for discord.py
+An extension which makes a rich-help command for discord.py
 
 Key Features
 -------------
 
 - Supports both message and slash commands.
 
 Installing
```

### Comparing `discord-rich-help.py-0.1.0/README.rst` & `discord-rich-help.py-0.1.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. image:: https://img.shields.io/pypi/v/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI supported Python versions
 
-The extension which make a rich-help command for discord.py
+An extension which makes a rich-help command for discord.py
 
 Key Features
 -------------
 
 - Supports both message and slash commands.
 
 Installing
```

### Comparing `discord-rich-help.py-0.1.0/discord_rich_help/__init__.py` & `discord-rich-help.py-0.1.1/discord_rich_help/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 # flake8: noqa
 
 __title__ = 'discord_rich_help'
 __author__ = 'PescadoGames'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2023 PescadoGames'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from typing import Literal, NamedTuple
 
 from .help import *
 
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaseLevel: Literal['alpha', 'beta', 'candidate', 'final']
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=0, minor=1, micro=0, releaseLevel='final', serial=0)
+version_info: VersionInfo = VersionInfo(major=0, minor=1, micro=1, releaseLevel='final', serial=0)
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `discord-rich-help.py-0.1.0/discord_rich_help/help.py` & `discord-rich-help.py-0.1.1/discord_rich_help/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,19 +254,19 @@
         view: HelpCommandView = HelpCommandView(page_length=len(self.pages), button_callback=self.switch_page)
 
         view.message = await self.get_destination().send(embed=bot_help, view=view)
 
     async def send_cog_help(self, cog: Cog) -> None:
         """|coro|
 
-        This will send "Command not found" error message.
+        This function is not implemented yet.
 
         .. versionadded:: 0.1
         """
-        await self.send_error_message(self.command_not_found(cog.qualified_name))
+        raise NotImplementedError('This function is not implemented yet.')
 
     async def send_group_help(self, group: Group[Any, Any, Any]) -> None:
         """|coro|
 
         Send a group help message.
 
         .. versionadded:: 0.1
```

### Comparing `discord-rich-help.py-0.1.0/discord_rich_help/text.py` & `discord-rich-help.py-0.1.1/discord_rich_help/text.py`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/discord_rich_help/ui.py` & `discord-rich-help.py-0.1.1/discord_rich_help/ui.py`

 * *Files identical despite different names*

### Comparing `discord-rich-help.py-0.1.0/discord_rich_help.py.egg-info/PKG-INFO` & `discord-rich-help.py-0.1.1/discord_rich_help.py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: discord-rich-help.py
-Version: 0.1.0
-Summary: The extension which make a rich-help command for discord.py
+Version: 0.1.1
+Summary: An extension which makes a rich-help command for discord.py
 Author-email: PescadoGames <official@pescadogames.com>
 Maintainer-email: Awayume <dev@awayume.jp>
 License: MIT License
 Project-URL: Repository, https://github.com/PescadoGames/discord-rich-help.py
 Project-URL: Documentation, https://github.com/PescadoGames/discord-rich-help.py/wiki
 Project-URL: Bug Tracker, https://github.com/PescadoGames/discord_rich_help.py/issues
 Keywords: discord,discord.py
@@ -36,15 +36,15 @@
 .. image:: https://img.shields.io/pypi/v/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/discord-rich-help.py.svg
    :target: https://pypi.python.org/pypi/discord-rich-help.py
    :alt: PyPI supported Python versions
 
-The extension which make a rich-help command for discord.py
+An extension which makes a rich-help command for discord.py
 
 Key Features
 -------------
 
 - Supports both message and slash commands.
 
 Installing
```

### Comparing `discord-rich-help.py-0.1.0/pyproject.toml` & `discord-rich-help.py-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "discord-rich-help.py"
 authors = [
     {name = "PescadoGames", email = "official@pescadogames.com"},
 ]
 maintainers = [
     {name = "Awayume", email = "dev@awayume.jp"},
 ]
-description = "The extension which make a rich-help command for discord.py"
+description = "An extension which makes a rich-help command for discord.py"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["discord", "discord.py"]
 license = {text = "MIT License"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
```

