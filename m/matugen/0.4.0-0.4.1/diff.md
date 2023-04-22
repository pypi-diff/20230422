# Comparing `tmp/matugen-0.4.0.tar.gz` & `tmp/matugen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matugen-0.4.0.tar", max compression
+gzip compressed data, was "matugen-0.4.1.tar", max compression
```

## Comparing `matugen-0.4.0.tar` & `matugen-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1615 2023-04-17 19:24:00.227213 matugen-0.4.0/README.md
--rw-r--r--   0        0        0      388 2023-04-18 19:23:03.501766 matugen-0.4.0/matugen/__main__.py
--rw-r--r--   0        0        0     9157 2023-04-21 18:30:09.147119 matugen-0.4.0/matugen/util.py
--rw-r--r--   0        0        0      433 2023-04-21 18:31:38.638471 matugen-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 matugen-0.4.0/setup.py
--rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 matugen-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2332 2023-04-22 15:44:30.340763 matugen-0.4.1/README.md
+-rw-r--r--   0        0        0      389 2023-04-22 14:05:25.047553 matugen-0.4.1/matugen/__main__.py
+-rw-r--r--   0        0        0    10801 2023-04-22 15:42:12.316265 matugen-0.4.1/matugen/util.py
+-rw-r--r--   0        0        0      473 2023-04-22 13:51:37.507846 matugen-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 matugen-0.4.1/setup.py
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 matugen-0.4.1/PKG-INFO
```

### Comparing `matugen-0.4.0/README.md` & `matugen-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,27 @@
     <a href="#installation">Installation</a>
     ·
     <a href="#usage">Usage</a>
     ·
     <a href="https://github.com/InioX/matugen/wiki">Wiki</a>
 </div>
 
+<div align="center">
+     <br>
+     <a href="https://pypi.org/project/matugen/">
+          <img alt="PyPI" src="https://img.shields.io/pypi/v/matugen?color=white&logo=pypi&logoColor=white&style=for-the-badge">
+     </a>
+     <a href="https://github.com/InioX/Matugen/actions/workflows/python-app.yml">
+          <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/InioX/matugen/python-app.yml?color=white&style=for-the-badge">
+     </a>
+     <a href="https://github.com/InioX/matugen/tags/">
+          <img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/InioX/matugen?color=white&logo=github&logoColor=white&style=for-the-badge">
+     </a>
+</div>
+
 ## Description
 [Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.
 
 ## Installation
 ### From Pypi
 >**Note** Assuming you have python with pip installed
 ```shell
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
  [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                           4fe9-9ee5-a1a1395d70dc.png]
                              ****** Matugen ******
                 A material you color generation tool for linux
                          Installation Â· Usage Â· Wiki
+
+         [PyPI] [GitHub_Workflow_Status] [GitHub_tag_(latest_by_date)]
 ## Description [Material Design 3](https://m3.material.io/) offers a new color
 system that allows for more flexible and dynamic use of color. The new system
 includes a wider range of colors, as well as a range of tints and shades that
 can be used to create subtle variations in color. ## Installation ### From Pypi
 >**Note** Assuming you have python with pip installed ```shell pip install
 matugen ``` ### Usage ```shell # Dark theme matugen /path/to/wallpaper/ # Light
 theme matugen /path/to/wallpaper/ -l ``` Example: ```shell matugen ~/wall/
```

### Comparing `matugen-0.4.0/matugen/util.py` & `matugen-0.4.1/matugen/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,47 @@
+import importlib.metadata
+import logging
 import os
 import re
-import logging
-import pathlib
 import subprocess
-import importlib.metadata
-from material_color_utilities_python import Image, themeFromImage
-from rich.logging import RichHandler
+from argparse import ArgumentParser, Namespace
 from configparser import ConfigParser
-from argparse import Namespace, ArgumentParser
 from pathlib import Path
 
+from material_color_utilities_python import Image, themeFromImage
+from rich import traceback
+from rich.logging import RichHandler
+
+traceback.install(extra_lines=3)
 
 logging.basicConfig(
     level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
 )
 
 log = logging.getLogger("rich")
 
 
+class InvalidFileExtension(Exception):
+    """
+    Exception raised when provided extension doesnt match with the expected one
+
+    @param extension -- The extension of the file
+    @param message -- The expected extension of the file
+    """
+
+    def __init__(self, expected_extension, extension):
+        self.extension = extension
+        self.expected_extension = expected_extension
+
+        self.message = (
+            f"Invalid file extension. Expected {expected_extension}, got '{extension}'"
+        )
+        super().__init__(self.message)
+
+
 def get_version() -> str:
     """
     Get matugen version. This is a wrapper around importlib.metadata.version().
 
 
     @return matugen version as a string
     """
@@ -63,14 +83,38 @@
         "-c",
         "--config",
         help="the config for generating templates",
         default="~/.config/matugen/config.ini",
         type=str,
     )
     args: Namespace = parser.parse_args()
+
+    # Check if the args provided are valid
+    VALID_WALLPAPER_EXTENSIONS = [".png", ".jpg"]
+    VALID_CONFIG_EXTENSIONS = [".ini"]
+    WALLPAPER_PATH = Path(args.wallpaper).expanduser()
+    CONFIG_PATH = Path(args.config).expanduser()
+
+    WALLPAPER_EXTENSION = Path(args.wallpaper).suffix
+    CONFIG_EXTENSION = Path(args.config).suffix
+
+    if WALLPAPER_EXTENSION == "":
+        raise FileNotFoundError("Invalid wallpaper file path.")
+    elif Path(args.wallpaper).suffix not in VALID_WALLPAPER_EXTENSIONS:
+        raise InvalidFileExtension(VALID_WALLPAPER_EXTENSIONS, WALLPAPER_EXTENSION)
+    elif not os.path.isfile(WALLPAPER_PATH):
+        raise FileNotFoundError("The wallpaper file doesnt exist.")
+
+    if CONFIG_EXTENSION == "":
+        raise FileNotFoundError("Invalid config file path.")
+    elif Path(args.config).suffix not in VALID_CONFIG_EXTENSIONS:
+        raise InvalidFileExtension(VALID_CONFIG_EXTENSIONS, CONFIG_EXTENSION)
+    elif not Path.is_file(CONFIG_PATH):
+        raise FileNotFoundError("The config file doesnt exist.")
+
     return args
 
 
 def reload_apps():
     """
     Reload apps to change the colors.
     """
@@ -108,15 +152,15 @@
     """
     Set wallpaper to given path.
 
     @param path - The path to the wallpaper to set.
     """
     session = get_session()
 
-    # setting the wallpaper on wayland with swaybg.
+    # Setting the wallpaper on wayland with swaybg.
     if session == "wayland":
         log.info("Wayland detected, setting wallpaper with swaybg")
         os.system("pkill swaybg > /dev/null 2>&1")
         os.system(f"swaybg -i {path} > /dev/null 2>&1 &")
     else:
         # TODO Use something else for x11
         return
@@ -167,74 +211,73 @@
         Read and parse config file. This is a wrapper around ConfigParser.read() that handles logging and error handling
 
         @param filename - Path to config file.
 
         @return Config object with parsed sections and template names from config file or None if there was an error reading the config.
         """
         config = ConfigParser()
-        config_path = Path(file).expanduser()
+        CONFIG_PATH = Path(file).expanduser()
         try:
-            config.read(config_path)
+            config.read(CONFIG_PATH)
         except OSError as err:
             logging.exception(f"Could not open {err.file}")
         else:
             logging.info(
-                f"Loaded {len(config.sections())} templates from {config_path}"
+                f"Loaded {len(config.sections())} templates from {CONFIG_PATH}"
             )
             return config
 
     @staticmethod
     def generate(scheme: dict, config: ConfigParser, wallpaper: str) -> dict:
         templates = [
             {
                 "name": config[item].name,
                 "template_path": Path(config[item]["template_path"]).expanduser(),
                 "output_path": Path(config[item]["output_path"]).expanduser(),
             }
             for item in config.sections()
         ]
 
-        for i, template in enumerate(templates):
+        HEX_VALUES = {key: value[1:] for key, value in scheme.items()}
+        RGB_VALUES = {
+            key: f"rgb{Color.hex_to_rgb(value[1:])}" for key, value in scheme.items()
+        }
+
+        # TODO: Use pathlib.Path instead of os.path
+        WALLPAPER_PATH = os.path.abspath(wallpaper)
 
+        for template in templates:
             try:
-                with open(template["template_path"], "r") as input:  # Template file
-                    input_data = input.read()
+                with open(template["template_path"], "r") as input_file:
+                    input_data = input_file.read()
             except OSError as err:
-                logging.error(f"Could not open {err.filename}")
-                i += 1
-                return
+                logging.exception(f"Could not open {err.filename}")
+                continue
 
             output_data = input_data
-            # print(f"i: {i}")
-            for h, (key, value) in enumerate(scheme.items()):
-                # print(f"H: {h}")
-                pattern = re.compile(f"@{{{key}}}")
-                pattern_hex = re.compile(f"@{{{key}.hex}}")
-                pattern_rgb = re.compile(f"@{{{key}.rgb}}")
-                pattern_wallpaper = re.compile("@{wallpaper}")
-
-                hex_stripped = value[1:]
-                rgb_value = f"rgb{Color.hex_to_rgb(hex_stripped)}"
-                wallpaper_value = os.path.abspath(wallpaper)
-
-                output_data = pattern.sub(hex_stripped, output_data)
-                output_data = pattern_hex.sub(value, output_data)
-                output_data = pattern_rgb.sub(rgb_value, output_data)
-                output_data = pattern_wallpaper.sub(wallpaper_value, output_data)
-                i += 1
+            for key in scheme:
+                PATTERN = re.compile(f"@{{{key}}}")
+                PATTERN_HEX = re.compile(f"@{{{key}.hex}}")
+                PATTERN_RGB = re.compile(f"@{{{key}.rgb}}")
+                PATTERN_WALLPAPER = re.compile("@{wallpaper}")
+
+                output_data = PATTERN.sub(HEX_VALUES[key], output_data)
+                output_data = PATTERN_HEX.sub(scheme[key], output_data)
+                output_data = PATTERN_RGB.sub(RGB_VALUES[key], output_data)
+                output_data = PATTERN_WALLPAPER.sub(WALLPAPER_PATH, output_data)
 
             try:
-                with open(template["output_path"], "w") as output:
-                    output.write(output_data)
+                with open(template["output_path"], "w") as output_file:
+                    output_file.write(output_data)
             except OSError as err:
                 logging.exception(
                     f'Could not write {template["name"]} template to {err.filename}'
                 )
             else:
-                log.info(
+                logging.info(
                     f'Exported {template["name"]} template to {template["output_path"]}'
                 )
 
 
 class Theme:
     @staticmethod
     def get(image: str):
@@ -243,18 +286,18 @@
 
         @param image - Path to the image to use.
 
         @return The theme as a dict containing multiple colorchemes.
         """
         log.info(f"Using image {image}")
         img = Image.open(image)
-        basewidth = 64
-        wpercent = basewidth / float(img.size[0])
+        BASEWIDTH = 64
+        wpercent = BASEWIDTH / float(img.size[0])
         hsize = int((float(img.size[1]) * float(wpercent)))
-        img = img.resize((basewidth, hsize), Image.Resampling.LANCZOS)
+        img = img.resize((BASEWIDTH, hsize), Image.Resampling.LANCZOS)
 
         return themeFromImage(img)
 
 
 class Scheme:
     def __init__(self, theme: str, lightmode: bool):
         """
```

### Comparing `matugen-0.4.0/setup.py` & `matugen-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['material-color-utilities-python==0.1.5', 'rich>=12.5.1,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['matugen = matugen.__main__:main']}
 
 setup_kwargs = {
     'name': 'matugen',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': '',
-    'long_description': '<div align="center">\n     <img src="https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-4fe9-9ee5-a1a1395d70dc.png" width=140>\n      <h1>Matugen</h1>\n </div>\n    \n<div align="center">\n  <b>A material you color generation tool for linux</b>\n</div>\n\n<div align="center">\n    <a href="#installation">Installation</a>\n    ·\n    <a href="#usage">Usage</a>\n    ·\n    <a href="https://github.com/InioX/matugen/wiki">Wiki</a>\n</div>\n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.\n\n## Installation\n### From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\nmatugen ~/wall/snow.png -l\n```\n\n### From repo with poetry\n>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd matugen\npoetry install\n```\n\n#### Usage\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n',
+    'long_description': '<div align="center">\n     <img src="https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-4fe9-9ee5-a1a1395d70dc.png" width=140>\n      <h1>Matugen</h1>\n </div>\n    \n<div align="center">\n  <b>A material you color generation tool for linux</b>\n</div>\n\n<div align="center">\n    <a href="#installation">Installation</a>\n    ·\n    <a href="#usage">Usage</a>\n    ·\n    <a href="https://github.com/InioX/matugen/wiki">Wiki</a>\n</div>\n\n<div align="center">\n     <br>\n     <a href="https://pypi.org/project/matugen/">\n          <img alt="PyPI" src="https://img.shields.io/pypi/v/matugen?color=white&logo=pypi&logoColor=white&style=for-the-badge">\n     </a>\n     <a href="https://github.com/InioX/Matugen/actions/workflows/python-app.yml">\n          <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/InioX/matugen/python-app.yml?color=white&style=for-the-badge">\n     </a>\n     <a href="https://github.com/InioX/matugen/tags/">\n          <img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/InioX/matugen?color=white&logo=github&logoColor=white&style=for-the-badge">\n     </a>\n</div>\n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.\n\n## Installation\n### From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\nmatugen ~/wall/snow.png -l\n```\n\n### From repo with poetry\n>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd matugen\npoetry install\n```\n\n#### Usage\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n',
     'author': 'InioX',
     'author_email': 'justimnix@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['matugen']
 package_data = \ {'': ['*']} install_requires = \ ['material-color-utilities-
 python==0.1.5', 'rich>=12.5.1,<13.0.0'] entry_points = \ {'console_scripts':
 ['matugen = matugen.__main__:main']} setup_kwargs = { 'name': 'matugen',
-'version': '0.4.0', 'description': '', 'long_description': '
+'version': '0.4.1', 'description': '', 'long_description': '
 \n [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                          4fe9-9ee5-a1a1395d70dc.png]\n
                              ****** Matugen ******
                                       \n
 \n \n
               \n A material you color generation tool for linux\n
 \n\n
                   \n Installation\n Â·\n Usage\n Â·\n Wiki\n
+\n\n
+                                      \n
+  \n \n_[PyPI]\n\n \n_[GitHub_Workflow_Status]\n\n \n_[GitHub_tag_(latest_by
+                                  date)]\n\n
 \n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new
 color system that allows for more flexible and dynamic use of color. The new
 system includes a wider range of colors, as well as a range of tints and shades
 that can be used to create subtle variations in color.\n\n## Installation\n###
 From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip
 install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/
 wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:
```

### Comparing `matugen-0.4.0/PKG-INFO` & `matugen-0.4.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matugen
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: InioX
 Author-email: justimnix@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,14 +25,27 @@
     <a href="#installation">Installation</a>
     ·
     <a href="#usage">Usage</a>
     ·
     <a href="https://github.com/InioX/matugen/wiki">Wiki</a>
 </div>
 
+<div align="center">
+     <br>
+     <a href="https://pypi.org/project/matugen/">
+          <img alt="PyPI" src="https://img.shields.io/pypi/v/matugen?color=white&logo=pypi&logoColor=white&style=for-the-badge">
+     </a>
+     <a href="https://github.com/InioX/Matugen/actions/workflows/python-app.yml">
+          <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/InioX/matugen/python-app.yml?color=white&style=for-the-badge">
+     </a>
+     <a href="https://github.com/InioX/matugen/tags/">
+          <img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/InioX/matugen?color=white&logo=github&logoColor=white&style=for-the-badge">
+     </a>
+</div>
+
 ## Description
 [Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.
 
 ## Installation
 ### From Pypi
 >**Note** Assuming you have python with pip installed
 ```shell
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: matugen Version: 0.4.0 Summary: Author: InioX
+Metadata-Version: 2.1 Name: matugen Version: 0.4.1 Summary: Author: InioX
 Author-email: justimnix@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 material-color-utilities-python (==0.1.5) Requires-Dist: rich
 (>=12.5.1,<13.0.0) Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                           4fe9-9ee5-a1a1395d70dc.png]
                              ****** Matugen ******
                 A material you color generation tool for linux
                          Installation Â· Usage Â· Wiki
+
+         [PyPI] [GitHub_Workflow_Status] [GitHub_tag_(latest_by_date)]
 ## Description [Material Design 3](https://m3.material.io/) offers a new color
 system that allows for more flexible and dynamic use of color. The new system
 includes a wider range of colors, as well as a range of tints and shades that
 can be used to create subtle variations in color. ## Installation ### From Pypi
 >**Note** Assuming you have python with pip installed ```shell pip install
 matugen ``` ### Usage ```shell # Dark theme matugen /path/to/wallpaper/ # Light
 theme matugen /path/to/wallpaper/ -l ``` Example: ```shell matugen ~/wall/
```

