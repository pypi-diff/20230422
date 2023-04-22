# Comparing `tmp/spotify-to-musi-1.0.2.tar.gz` & `tmp/spotify_to_musi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-to-musi-1.0.2.tar", max compression
+gzip compressed data, was "spotify_to_musi-2.0.0.tar", max compression
```

## Comparing `spotify-to-musi-1.0.2.tar` & `spotify_to_musi-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0     1082 2022-04-30 04:14:50.831047 spotify-to-musi-1.0.2/LICENSE
--rw-r--r--   0        0        0     1418 2022-07-17 20:43:48.264390 spotify-to-musi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1674 2022-05-15 01:35:43.376818 spotify-to-musi-1.0.2/README.md
--rw-r--r--   0        0        0     1056 2022-07-16 02:44:19.027147 spotify-to-musi-1.0.2/spotify_to_musi/__init__.py
--rw-r--r--   0        0        0     3730 2022-07-17 20:41:43.426669 spotify-to-musi-1.0.2/spotify_to_musi/__main__.py
--rw-r--r--   0        0        0     2887 2022-07-16 03:44:45.913206 spotify-to-musi-1.0.2/spotify_to_musi/cache.py
--rw-r--r--   0        0        0     1897 2022-07-17 20:00:30.529188 spotify-to-musi-1.0.2/spotify_to_musi/commons.py
--rw-r--r--   0        0        0    14625 2022-07-17 20:16:15.730316 spotify-to-musi-1.0.2/spotify_to_musi/main.py
--rw-r--r--   0        0        0     1087 2022-05-12 20:01:34.542338 spotify-to-musi-1.0.2/spotify_to_musi/paths.py
--rw-r--r--   0        0        0        0 2022-05-12 20:01:34.542338 spotify-to-musi-1.0.2/spotify_to_musi/py.typed
--rw-r--r--   0        0        0     2863 2022-07-16 19:27:20.892373 spotify-to-musi-1.0.2/spotify_to_musi/typings/core.py
--rw-r--r--   0        0        0      846 2022-05-12 20:01:34.543335 spotify-to-musi-1.0.2/spotify_to_musi/typings/musi.py
--rw-r--r--   0        0        0     2744 2022-05-12 20:01:34.544332 spotify-to-musi-1.0.2/spotify_to_musi/typings/spotify.py
--rw-r--r--   0        0        0      768 2022-07-16 19:30:09.868528 spotify-to-musi-1.0.2/spotify_to_musi/typings/youtube.py
--rw-r--r--   0        0        0     2644 2022-07-17 20:46:58.648748 spotify-to-musi-1.0.2/setup.py
--rw-r--r--   0        0        0     3159 2022-07-17 20:46:58.648748 spotify-to-musi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-04-30 04:14:50.831047 spotify_to_musi-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2412 2023-04-22 00:53:35.525411 spotify_to_musi-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1708 2023-04-22 00:53:50.158969 spotify_to_musi-2.0.0/README.md
+-rw-r--r--   0        0        0      749 2023-04-19 20:59:57.112853 spotify_to_musi-2.0.0/spotify_to_musi/__init__.py
+-rw-r--r--   0        0        0     4137 2023-04-22 00:47:11.473199 spotify_to_musi-2.0.0/spotify_to_musi/__main__.py
+-rw-r--r--   0        0        0     3531 2023-04-19 20:53:14.471015 spotify_to_musi-2.0.0/spotify_to_musi/commons.py
+-rw-r--r--   0        0        0     1088 2023-04-16 23:05:44.315588 spotify_to_musi-2.0.0/spotify_to_musi/exceptions.py
+-rw-r--r--   0        0        0      982 2023-04-22 00:01:10.469619 spotify_to_musi-2.0.0/spotify_to_musi/main.py
+-rw-r--r--   0        0        0     5631 2023-04-22 00:14:25.119714 spotify_to_musi-2.0.0/spotify_to_musi/musi.py
+-rw-r--r--   0        0        0     5538 2023-04-22 00:01:10.485440 spotify_to_musi-2.0.0/spotify_to_musi/oauth.py
+-rw-r--r--   0        0        0     1024 2023-04-22 00:24:41.849747 spotify_to_musi-2.0.0/spotify_to_musi/paths.py
+-rw-r--r--   0        0        0        0 2022-05-12 20:01:34.542338 spotify_to_musi-2.0.0/spotify_to_musi/py.typed
+-rw-r--r--   0        0        0    12619 2023-04-22 00:01:10.500456 spotify_to_musi-2.0.0/spotify_to_musi/spotify.py
+-rw-r--r--   0        0        0     3688 2023-04-22 00:01:10.504904 spotify_to_musi-2.0.0/spotify_to_musi/tracks_cache.py
+-rw-r--r--   0        0        0       35 2023-04-16 22:55:23.576124 spotify_to_musi-2.0.0/spotify_to_musi/typings/__init__.py
+-rw-r--r--   0        0        0     2469 2023-04-22 00:22:56.472209 spotify_to_musi-2.0.0/spotify_to_musi/typings/core.py
+-rw-r--r--   0        0        0     4108 2023-04-22 00:25:10.891189 spotify_to_musi-2.0.0/spotify_to_musi/typings/musi.py
+-rw-r--r--   0        0        0     4215 2023-04-19 21:00:48.910481 spotify_to_musi-2.0.0/spotify_to_musi/typings/spotify.py
+-rw-r--r--   0        0        0     1611 2023-04-22 00:01:10.537402 spotify_to_musi-2.0.0/spotify_to_musi/typings/youtube.py
+-rw-r--r--   0        0        0    10001 2023-04-21 23:58:33.475408 spotify_to_musi-2.0.0/spotify_to_musi/youtube.py
+-rw-r--r--   0        0        0    12837 2023-04-22 00:16:02.227785 spotify_to_musi-2.0.0/spotify_to_musi/ytmusic.py
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 spotify_to_musi-2.0.0/PKG-INFO
```

### Comparing `spotify-to-musi-1.0.2/LICENSE` & `spotify_to_musi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify-to-musi-1.0.2/pyproject.toml` & `spotify_to_musi-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,79 @@
 [tool.poetry]
 name = "spotify-to-musi"
 description = "Transfer Spotify playlists to Musi."
-version = "1.0.2"
+version = "2.0.0"
 readme = "README.md"
 license = "MIT"
 authors = ["Hexiro <mail@hexiro.me>"]
 repository = "https://github.com/hexiro/spotify-to-musi"
 keywords = ["spotify", "music", "musi", "transfer", "cli"]
 classifiers = [
     "Natural Language :: English",
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries ",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-ytmusicapi = "^0.22.0"
-rich = "^12.5.1"
-rich-click = "^1.5.1"
-requests = "^2.28.1"
-requests-toolbelt = "^0.9.1"
-spotipy = "^2.20.0"
+python = "^3.9"
+rich = "^13.3.4"
+rich-click = "^1.6.1"
+aiofiles = "^23.1.0"
+httpx = "^0.24.0"
+pydantic = "^1.10.7"
+pyfy = "^2.2.0"
+sanic = "^23.3.0"
+async-cache = "^1.1.1"
+typing-extensions = {version = "^4.5.0", python = "<3.11"}
+uvloop = {version = "^0.17.0", platform = "linux"}
 
 [tool.poetry.scripts]
 spotify-to-musi = "spotify_to_musi.__main__:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/hexiro/spotify-to-musi/issues"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+pytest-asyncio = "^0.21.0"
+mypy = "^1.2.0"
+ruff = "^0.0.261"
+black = "^23.3.0"
+isort = "^5.12.0"
+types-aiofiles = "^23.1.0.1"
+pre-commit = "^3.2.2"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 119
+target-version = ["py38"]
+
+[tool.ruff]
+select = ["ANN", "TCH", "N", "S", "B", "A", "C4", "EM", "INP", "PIE", "SIM", "ERA", "TRY", "TID", "RUF", "F"]
+ignore = [
+    "E501",    # let black handle line length
+    "ANN401",  # if everything is going to be typed, some things have to be any
+    "A003",    # attributes with the same name as builtins is okay
+    "EM101",   # I personally think it's okay to use a string literal in this case.
+]  
+
+[tool.ruff.per-file-ignores]
+"tests/*.py" = ["S101"]   # allow using assert in tests
+
+[tool.mypy]
+ignore_missing_imports = true
+disable_error_code = "call-arg"
+
+[tool.isort]
+profile = "black"
```

### Comparing `spotify-to-musi-1.0.2/README.md` & `spotify_to_musi-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 
 # Why Musi?
 
 Musi allows you to listen to any song (video) from YouTube without being interrupted with ads like with Spotify.
 As someone who doesn't have a music streaming subscription I prefer to use Spotify on Desktop and Musi on mobile,
 so I created this app to transfer songs between the two.
 
-# Spotify API
+# Spotify Credentials Setup
 
-1. Go to https://developer.spotify.com/dashboard/ \
+1. Navigate to https://developer.spotify.com/dashboard \
    ![Dashboard](./.github/assets/dashboard.png)
-2. Choose an app name and accept the terms and conditions. \
-   ![CREATE AN APP](./.github/assets/create-an-app.png)
-3. Set callback to https://example.com/callback/ \
-   ![Set Callback](./.github/assets/set-callback.png)
-4. View Client ID and Client Secret \
-   ![SHOW CLIENT SECRET](./.github/assets/show-client-secret.png)
-5. Rename .env.example to .env and set secrets \
-   ![.env file](./.github/assets/dotenv-file.png)
-6. Upon running the script for the first time, you will be prompted with something that looks like this: \
-   ![first time setup](./.github/assets/first-time-setup.png)
-7. Click the URL, Sign In if you need to and proceed until you see a page that looks like this: \
-   ![img.png](.github/assets/example.com.png)
-8. Copy the URL of the page you were redirected to and paste it into the console of the program and enter
+2. Create an app with the name & description of your choice.
+   Make sure the callback URL is set to http://localhost:5000/callback/spotify \
+   ![Create App](./.github/assets/create-an-app.png)
+3. Open Settings \
+    ![Open Settings](./.github/assets/open-settings.png)
+4. View Client ID and Client Secret and store them in a safe place. \
+   ![View Client Credentials](./.github/assets/view-client-credentials.png)
+5. Initialize setup script with `spotify-to-musi setup` & enter Client ID and Client Secret \
+   ![Setup](./.github/assets/setup.png)
+6. Open the link (http://localhost:5000/callback/spotify) in your browser and authorize with Spotify \
+   ![Authorize](./.github/assets/authorize.png)
+7. Return to your terminal, and you should be successfully authorized! :3 \
+    ![Successfully Authorized](./.github/assets/successfully-authorized.png)
+
+
 
 # PyCharm Usage
 
 If you're running pycharm, make sure `emulate terminal in output console` is enabled<br>
 
 references:
```

### Comparing `spotify-to-musi-1.0.2/spotify_to_musi/__main__.py` & `spotify_to_musi-2.0.0/spotify_to_musi/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,137 @@
 """Entrypoint and CLI handler."""
 from __future__ import annotations
 
-import logging
-import os
+import asyncio
+import functools
+import sys
+import typing as t
 
-from typing import TYPE_CHECKING
+import pyfy.excs
 import rich
-
 import rich_click as click
-import spotipy
-import spotipy.oauth2
-import spotipy.exceptions
+from rich.prompt import Prompt
+
+from spotify_to_musi import main, oauth, spotify
+from spotify_to_musi.commons import spotify_client_credentials
+from spotify_to_musi.paths import SPOTIFY_CREDENTIALS_PATH
+
 
-from .commons import SPOTIFY_ID_REGEX
-from .cache import has_unpatched_spotify_secrets, patch_spotify_secrets, store_spotify_secrets
-from .main import get_spotify, transfer_spotify_to_musi
-from .paths import spotify_cache_path, spotify_data_path
+def async_cmd(func: t.Callable) -> t.Callable:
+    """
+    Hack to make click support async commands.
 
+    Reference:
+        https://stackoverflow.com/q/67558717/10830115
+    """
 
-if TYPE_CHECKING:
-    from .typings.spotify import SpotifyLikedSong, SpotifyPlaylist
+    @functools.wraps(func)
+    def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        if sys.platform == "win32":
+            # Set the policy to prevent "Event loop is closed" error on Windows - https://github.com/encode/httpx/issues/914
+            asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+        elif sys.platform == "linux":
+            import uvloop  # type: ignore
 
+            uvloop.install()
 
-click.rich_click.STYLE_OPTION = "bold magenta"
-click.rich_click.STYLE_SWITCH = "bold blue"
-click.rich_click.STYLE_METAVAR = "bold red"
-click.rich_click.MAX_WIDTH = 75
+        return asyncio.run(func(*args, **kwargs))
 
-console = rich.get_console()
-logger = logging.getLogger(__name__)
+    return wrapper
 
 
 @click.group()
-def cli():
+@async_cmd
+async def cli() -> None:
     pass
 
 
 @cli.command()
+@async_cmd
 @click.option(
     "-u",
     "--user",
     is_flag=True,
     help="Transfer liked songs and playlists of authorized user.",
     default=False,
     show_default=True,
 )
-@click.option("-pl", "--playlist", help="Transfer Spotify playlist(s) by URL.", multiple=True, type=str)
-def transfer(user: bool, playlist: list[str]):
-    """Transfer songs from Spotify to Musi."""
-    if has_unpatched_spotify_secrets():
-        patch_spotify_secrets()
+@click.option(
+    "-pl",
+    "--playlist",
+    help="Transfer Spotify playlist(s) by URL.",
+    multiple=True,
+    type=str,
+)
+async def transfer(user: bool, playlist: list[str]) -> None:
+    """
+    Transfer songs from Spotify to Musi.
+    """
+
+    await spotify.init()
 
     try:
-        get_spotify()
-    except spotipy.oauth2.SpotifyOauthError:
-        console.print("[red]Spotify not authorized. Please run `setup` first.[/red]")
+        await spotify.spotify.me()
+    except pyfy.excs.SpotifyError:
+        rich.print("[bold red]Spotify not authorized. Please run `[white]setup[/white]` first.[/bold red]")
         return
 
     if not user and not playlist:
-        console.print("[red]Not uploading user's playlists and no playlist(s) were specified.[/red]")
+        rich.print("[bold red]Failed to transfer. No playlist(s) nor the user's library were specified.[/bold red]")
         return
 
-    transfer_spotify_to_musi(user, playlist)
+    await main.transfer_spotify_to_musi(transfer_user_library=user, extra_playlist_urls=playlist)
 
 
 @cli.command()
-def setup():
-    """Configure Spotify API and other options."""
-    grey = "#808080"
-    spotify_to_musi_text = f"[bold][green]spotify[/green][reset]-to-[/reset][dark_orange3]musi[/dark_orange3][/bold]"
-    welcome_text = f"Welcome to {spotify_to_musi_text} first time setup! [i](Ctrl + C to exit)[/i]"
-
-    if has_unpatched_spotify_secrets():
-        patch_spotify_secrets()
-        welcome_text += (
-            "\n* Your secrets are already set! Only run this script again if you need to authorize with Spotify again."
-        )
-
-    console.print(welcome_text, highlight=True, markup=True)
-
-    def prompt(for_: str, default: str | None = None) -> str:
-        default_text: str = ""
-        if default:
-            if len(default) > 5:
-                mid_point = len(default) // 2
-                default_fragment = f"{default[:mid_point]}..."
-            else:
-                default_fragment = default
-            default_text = f" [{grey}][[i]{default_fragment}[/i]][/{grey}]"
-        text = f"[magenta]{for_}{default_text}[/magenta]: "
-
-        res = console.input(text) or default
-        while not res:
-            console.print("[red]Please enter a value.[/red]")
-            res = console.input(text)
-        return res
-
-    spotify_client_id = prompt("Spotify Client ID", default=os.getenv("SPOTIPY_CLIENT_ID"))
-    spotify_client_secret = prompt("Spotify Client Secret", default=os.getenv("SPOTIPY_CLIENT_SECRET"))
-    store_spotify_secrets(spotify_client_id, spotify_client_secret)
-    patch_spotify_secrets()
-    try:
-        get_spotify()
-    except spotipy.oauth2.SpotifyOauthError:
-        spotify_cache_path.unlink()
+@async_cmd
+async def setup() -> None:
+    """
+    Configure Spotify w/ OAuth.
+    """
+    spotify_to_musi_text = "[bold][green]Spotify[/green][white]-to-[/white][dark_orange3]Musi[/dark_orange3][/bold]"
+    welcome_text = f"{spotify_to_musi_text} first time setup! [i grey53](Ctrl + C to exit)[/i grey53]\n"
+
+    stored_client_id: str | None = None
+    stored_client_secret: str | None = None
+
+    spotify_client_creds = await spotify_client_credentials()
+    if spotify_client_creds:
+        stored_client_id, stored_client_secret = spotify_client_creds
+
+    if stored_client_id and stored_client_secret:
+        welcome_text += "[grey53]* Your secrets are already set! Only run this script if you need to authorize with Spotify again.[/grey53]\n"
+
+    rich.print(welcome_text)
+
+    def style_prompt(prompt: str) -> str:
+        return f"[bold white]{prompt}[/bold white][grey53]"
+
+    spotify_client_id: str | None = None
+    spotify_client_secret: str | None = None
+
+    while not spotify_client_id:
+        spotify_client_id = Prompt.ask(style_prompt("Spotify Client ID"), default=stored_client_id)
+    while not spotify_client_secret:
+        spotify_client_secret = Prompt.ask(style_prompt("Spotify Client Secret"), default=stored_client_secret)
+
+    rich.print(
+        f"\nPlease open your browser and navigate to [blue underline]{oauth.URL}[/blue underline]\nAuthorize with Spotify and return once done.\n"
+    )
+
+    await oauth.run(
+        spotify_client_id=spotify_client_id,
+        spotify_client_secret=spotify_client_secret,
+    )
+
     try:
-        get_spotify()
-    except spotipy.oauth2.SpotifyOauthError:
-        console.print("[red]Uh Oh? Spotify isn't authorized. Please check your credentials.[/red]")
-        return
-    console.print("[green]Spotify authorized![/green]")
+        await spotify.init()
+        await spotify.spotify.me()
+    except pyfy.excs.SpotifyError:
+        SPOTIFY_CREDENTIALS_PATH.unlink()
+        rich.print("[red]Uh Oh? Spotify isn't authorized. Please check your credentials.[/red]")
+
+    rich.print("[bold green]Spotify Authorized![/bold green]")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `spotify-to-musi-1.0.2/PKG-INFO` & `spotify_to_musi-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 Metadata-Version: 2.1
 Name: spotify-to-musi
-Version: 1.0.2
+Version: 2.0.0
 Summary: Transfer Spotify playlists to Musi.
 Home-page: https://github.com/hexiro/spotify-to-musi
 License: MIT
 Keywords: spotify,music,musi,transfer,cli
 Author: Hexiro
 Author-email: mail@hexiro.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries 
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
-Requires-Dist: rich-click (>=1.5.1,<2.0.0)
-Requires-Dist: spotipy (>=2.20.0,<3.0.0)
-Requires-Dist: ytmusicapi (>=0.22.0,<0.23.0)
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: async-cache (>=1.1.1,<2.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyfy (>=2.2.0,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Requires-Dist: sanic (>=23.3.0,<24.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
+Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; sys_platform == "linux"
 Project-URL: Bug Tracker, https://github.com/hexiro/spotify-to-musi/issues
 Project-URL: Repository, https://github.com/hexiro/spotify-to-musi
 Description-Content-Type: text/markdown
 
 # spotify-to-musi
 
 > Transfer your [Spotify](https://spotify.com) playlists to [Musi](https://feelthemusi.com).
@@ -41,31 +47,33 @@
 
 # Why Musi?
 
 Musi allows you to listen to any song (video) from YouTube without being interrupted with ads like with Spotify.
 As someone who doesn't have a music streaming subscription I prefer to use Spotify on Desktop and Musi on mobile,
 so I created this app to transfer songs between the two.
 
-# Spotify API
+# Spotify Credentials Setup
 
-1. Go to https://developer.spotify.com/dashboard/ \
+1. Navigate to https://developer.spotify.com/dashboard \
    ![Dashboard](./.github/assets/dashboard.png)
-2. Choose an app name and accept the terms and conditions. \
-   ![CREATE AN APP](./.github/assets/create-an-app.png)
-3. Set callback to https://example.com/callback/ \
-   ![Set Callback](./.github/assets/set-callback.png)
-4. View Client ID and Client Secret \
-   ![SHOW CLIENT SECRET](./.github/assets/show-client-secret.png)
-5. Rename .env.example to .env and set secrets \
-   ![.env file](./.github/assets/dotenv-file.png)
-6. Upon running the script for the first time, you will be prompted with something that looks like this: \
-   ![first time setup](./.github/assets/first-time-setup.png)
-7. Click the URL, Sign In if you need to and proceed until you see a page that looks like this: \
-   ![img.png](.github/assets/example.com.png)
-8. Copy the URL of the page you were redirected to and paste it into the console of the program and enter
+2. Create an app with the name & description of your choice.
+   Make sure the callback URL is set to http://localhost:5000/callback/spotify \
+   ![Create App](./.github/assets/create-an-app.png)
+3. Open Settings \
+    ![Open Settings](./.github/assets/open-settings.png)
+4. View Client ID and Client Secret and store them in a safe place. \
+   ![View Client Credentials](./.github/assets/view-client-credentials.png)
+5. Initialize setup script with `spotify-to-musi setup` & enter Client ID and Client Secret \
+   ![Setup](./.github/assets/setup.png)
+6. Open the link (http://localhost:5000/callback/spotify) in your browser and authorize with Spotify \
+   ![Authorize](./.github/assets/authorize.png)
+7. Return to your terminal, and you should be successfully authorized! :3 \
+    ![Successfully Authorized](./.github/assets/successfully-authorized.png)
+
+
 
 # PyCharm Usage
 
 If you're running pycharm, make sure `emulate terminal in output console` is enabled<br>
 
 references:
```

