# Comparing `tmp/blurry_cli-0.1.0.tar.gz` & `tmp/blurry_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.1.0.tar", max compression
+gzip compressed data, was "blurry_cli-0.2.0.tar", max compression
```

## Comparing `blurry_cli-0.1.0.tar` & `blurry_cli-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     4369 2023-04-09 16:34:17.582035 blurry_cli-0.1.0/README.md
--rw-r--r--   0        0        0     7503 2023-04-09 16:34:17.585369 blurry_cli-0.1.0/blurry/__init__.py
--rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/blurry/__main__.py
--rw-r--r--   0        0        0      527 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/blurry/async_typer.py
--rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/blurry/constants.py
--rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.1.0/blurry/images.py
--rw-r--r--   0        0        0     6811 2023-03-28 22:14:17.179004 blurry_cli-0.1.0/blurry/markdown/__init__.py
--rw-r--r--   0        0        0      642 2023-03-28 22:14:17.179004 blurry_cli-0.1.0/blurry/markdown/blur_blurry_name_plugin.py
--rw-r--r--   0        0        0     1022 2023-04-09 15:03:09.554313 blurry_cli-0.1.0/blurry/markdown/container.py
--rw-r--r--   0        0        0     1633 2023-04-09 15:02:59.097386 blurry_cli-0.1.0/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0      628 2023-03-28 22:14:17.179004 blurry_cli-0.1.0/blurry/markdown/punctuation_plugin.py
--rw-r--r--   0        0        0     1304 2023-03-28 22:14:17.179004 blurry_cli-0.1.0/blurry/markdown/python_code_plugin.py
--rw-r--r--   0        0        0     2261 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/blurry/open_graph.py
--rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.1.0/blurry/py.typed
--rw-r--r--   0        0        0     1967 2023-04-05 22:10:55.888871 blurry_cli-0.1.0/blurry/settings.py
--rw-r--r--   0        0        0     1538 2023-03-28 22:11:29.443893 blurry_cli-0.1.0/blurry/sitemap.py
--rw-r--r--   0        0        0      602 2023-04-06 01:16:20.756982 blurry_cli-0.1.0/blurry/types.py
--rw-r--r--   0        0        0     4535 2023-04-09 16:34:17.585369 blurry_cli-0.1.0/blurry/utils.py
--rw-r--r--   0        0        0     1475 2023-04-09 16:34:17.592036 blurry_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 blurry_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1784 2023-04-16 22:37:50.018954 blurry_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     8177 2023-04-16 23:06:33.073434 blurry_cli-0.2.0/blurry/__init__.py
+-rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/__main__.py
+-rw-r--r--   0        0        0      527 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/async_typer.py
+-rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/constants.py
+-rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.2.0/blurry/images.py
+-rw-r--r--   0        0        0     6514 2023-04-16 22:37:50.018954 blurry_cli-0.2.0/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1633 2023-04-15 17:13:08.997639 blurry_cli-0.2.0/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0     2261 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/open_graph.py
+-rw-r--r--   0        0        0      189 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      644 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1471 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/py.typed
+-rw-r--r--   0        0        0     2042 2023-04-09 23:10:30.264113 blurry_cli-0.2.0/blurry/settings.py
+-rw-r--r--   0        0        0     1538 2023-03-28 22:11:29.443893 blurry_cli-0.2.0/blurry/sitemap.py
+-rw-r--r--   0        0        0      636 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/types.py
+-rw-r--r--   0        0        0     4535 2023-04-22 14:16:05.282134 blurry_cli-0.2.0/blurry/utils.py
+-rw-r--r--   0        0        0     1988 2023-04-22 15:07:18.954697 blurry_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 blurry_cli-0.2.0/PKG-INFO
```

### Comparing `blurry_cli-0.1.0/LICENSE` & `blurry_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/__init__.py` & `blurry_cli-0.2.0/blurry/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,51 @@
 from datetime import datetime
 from mimetypes import guess_type
 from mimetypes import types_map
 from pathlib import Path
 from typing import Any
 from typing import Coroutine
 
-import htmlmin
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 from jinja2 import select_autoescape
 from livereload import Server
+from rich import print
 
 from blurry.async_typer import AsyncTyper
 from blurry.constants import ENV_VAR_PREFIX
 from blurry.images import generate_images_for_srcset
 from blurry.markdown import convert_markdown_file_to_html
 from blurry.open_graph import open_graph_meta_tags
+from blurry.plugins import discovered_html_plugins
+from blurry.plugins import discovered_markdown_plugins
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import get_templates_directory
 from blurry.settings import SETTINGS
 from blurry.sitemap import write_sitemap_file
 from blurry.types import DirectoryFileData
 from blurry.types import MarkdownFileData
+from blurry.types import TemplateContext
 from blurry.utils import content_path_to_url
 from blurry.utils import convert_content_path_to_directory_in_build
 from blurry.utils import format_schema_data
-from blurry.utils import minify_style_tags
 from blurry.utils import sort_directory_file_data_by_date
 from blurry.utils import write_index_file_creating_path
 
 
 def json_converter_with_dates(item: Any) -> None | str:
     if isinstance(item, datetime):
         return item.strftime("%Y-%M-%D")
 
 
+print("Markdown plugins:", [p.name for p in discovered_markdown_plugins])
+print("HTML plugins:", [p.name for p in discovered_html_plugins])
+
+
 CONTENT_DIR = get_content_directory()
 TEMPLATE_DIR = get_templates_directory()
 
 app = AsyncTyper()
 
 jinja_env = Environment(
     loader=FileSystemLoader(TEMPLATE_DIR), autoescape=select_autoescape(["html", "xml"])
@@ -68,15 +74,15 @@
 
 async def write_html_file(
     file_data: MarkdownFileData,
     file_data_list: list[MarkdownFileData],
     file_data_by_directory: dict[Path, list[MarkdownFileData]],
     release: bool,
 ):
-    extra_context = {}
+    extra_context: TemplateContext = {}
     # Gather data from other files in this directory if this is an index file
     if file_data.path.name == "index.md":
         sibling_pages = [
             {
                 "url": content_path_to_url(f.path),
                 **f.front_matter,
             }
@@ -84,55 +90,63 @@
             if f.path != file_data.path
         ]
         extra_context["sibling_pages"] = sibling_pages
     folder_in_build = convert_content_path_to_directory_in_build(file_data.path)
 
     schema_type = file_data.front_matter.get("@type")
     if not schema_type:
-        raise ValueError(f"Required @type value missing in file: {file_data.path}")
+        raise ValueError(
+            f"Required @type value missing in file or TOML front matter invalid: "
+            f"{file_data.path}"
+        )
     template = jinja_env.get_template(f"{schema_type}.html")
 
+    # Map custom template name to Schema.org type
+    if mapped_schema_type := SETTINGS["TEMPLATE_SCHEMA_TYPES"].get(schema_type):
+        file_data.front_matter["@type"] = mapped_schema_type
+
     # Include non-schema variables as top-level context values, removing them from
     # front_matter
     front_matter = file_data.front_matter
-    schema_variables = {}
-    template_context = {}
+    schema_variables: TemplateContext = {}
+    template_context: TemplateContext = {}
     non_schema_variable_prefix = SETTINGS["FRONTMATTER_NON_SCHEMA_VARIABLE_PREFIX"]
     for key, value in front_matter.items():
         if key.startswith(non_schema_variable_prefix):
             template_context[key.replace(non_schema_variable_prefix, "", 1)] = value
             continue
         schema_variables[key] = value
 
     schema_data = json.dumps(
         format_schema_data(schema_variables),
         default=json_converter_with_dates,
     )
     schema_type_tag = f'<script type="application/ld+json">{schema_data}</script>'
 
-    html = template.render(
-        dataclasses=dataclasses,
-        body=file_data.body,
-        schema_data=schema_data,
-        schema_type_tag=schema_type_tag,
-        open_graph_tags=open_graph_meta_tags(file_data.front_matter),
-        build_path=folder_in_build,
-        file_data_by_directory={
+    template_context = {
+        "body": file_data.body,
+        "schema_data": schema_data,
+        "schema_type_tag": schema_type_tag,
+        "open_graph_tags": open_graph_meta_tags(file_data.front_matter),
+        "build_path": folder_in_build,
+        "file_data_by_directory": {
             str(path): data for path, data in file_data_by_directory.items()
         },
-        settings=SETTINGS,
+        "settings": SETTINGS,
         **schema_variables,
         **extra_context,
         **template_context,
-    )
+    }
 
-    if release:
-        # Minify HTML and CSS
-        html = htmlmin.minify(html, remove_empty_space=True)
-        html = minify_style_tags(html)
+    html = template.render(dataclasses=dataclasses, **template_context)
+    for html_plugin in discovered_html_plugins:
+        try:
+            html = html_plugin.load()(html, template_context, release)
+        except Exception as err:
+            print(f"Error initializing plugin {html_plugin}: {err}")
 
     # Write file
     write_index_file_creating_path(folder_in_build, html)
 
 
 @app.async_command()
 async def build(release=True):
@@ -181,22 +195,22 @@
             markdown_tasks.append(
                 write_html_file(
                     file_data, file_data_list, file_data_by_directory, release
                 )
             )
 
     task_count = len(markdown_tasks) + len(non_markdown_tasks)
-    print(f"Gathered {task_count} tasks (sitemap and {task_count - 1} content files)")
+    print(f"Gathered {task_count} tasks")
 
     await asyncio.gather(*markdown_tasks)
     await asyncio.gather(*non_markdown_tasks)
     end = datetime.now()
 
     difference = end - start
-    print(f"Took {difference.total_seconds()} seconds")
+    print(f"Built site in {difference.total_seconds()} seconds")
 
 
 async def build_development():
     await build(release=False)
 
 
 @app.command()
```

### Comparing `blurry_cli-0.1.0/blurry/async_typer.py` & `blurry_cli-0.2.0/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/images.py` & `blurry_cli-0.2.0/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/markdown/__init__.py` & `blurry_cli-0.2.0/blurry/markdown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from pathlib import Path
 from typing import Any
 from typing import Type
 from typing import TypeGuard
 
 import mistune
-from mistune.directives import FencedDirective
-from mistune.plugins.task_lists import task_lists
-from mistune.plugins.formatting import strikethrough
+from mistune import BlockState
 from mistune.plugins.abbr import abbr
-from mistune.plugins.footnotes import footnotes
-from mistune.plugins.url import url
 from mistune.plugins.def_list import def_list
+from mistune.plugins.footnotes import footnotes
+from mistune.plugins.formatting import strikethrough
 from mistune.plugins.table import table
+from mistune.plugins.task_lists import task_lists
+from mistune.plugins.url import url
 from mistune.util import escape
-from mistune import BlockState
 from wand.image import Image
 
-from .blur_blurry_name_plugin import blur_blurry_name
-from .container import Container
 from .front_matter import parse_front_matter
-from .punctuation_plugin import punctuation
-from .python_code_plugin import python_code
-from .python_code_plugin import python_code_in_list
 from blurry.images import add_image_width_to_path
 from blurry.images import generate_sizes_string
 from blurry.images import generate_srcset_string
 from blurry.images import get_widths_for_image_width
 from blurry.images import THUMBNAIL_WIDTH
+from blurry.plugins import discovered_markdown_plugins
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import SETTINGS
 from blurry.utils import build_path_to_url
 from blurry.utils import content_path_to_url
 from blurry.utils import convert_relative_path_in_markdown_to_relative_build_path
 from blurry.utils import path_to_url_pathname
@@ -131,26 +126,22 @@
 
 
 renderer = BlurryRenderer(escape=False)
 markdown = mistune.Markdown(
     renderer,
     plugins=[
         abbr,
-        blur_blurry_name,
         def_list,
         footnotes,
-        punctuation,
-        python_code,
-        python_code_in_list,
         strikethrough,
         table,
         task_lists,
         url,
-        FencedDirective([Container()], ":"),
-    ],
+    ]
+    + [plugin.load() for plugin in discovered_markdown_plugins],
 )
 
 
 def convert_markdown_file_to_html(filepath: Path) -> tuple[str, dict[str, Any]]:
     if not markdown.renderer:
         raise Exception("Blurry markdown renderer not set on Mistune Markdown instance")
```

### Comparing `blurry_cli-0.1.0/blurry/markdown/container.py` & `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from mistune.directives import Admonition
+from mistune.directives import FencedDirective
 from mistune.directives.admonition import render_admonition_content
 
 
 class Container(Admonition):
     """Custom admonition directive using an <aside> HTML element"""
 
     SUPPORTED_NAMES = {
@@ -28,7 +29,10 @@
             md.renderer.register("admonition_content", render_admonition_content)
 
 
 def render_admonition(self, text, name, **attrs):
     _cls = attrs.get("class", "")
     class_attribute = f"{name} {_cls}".strip()
     return f'<aside role="note" class="{class_attribute}">{text}</aside>'
+
+
+container = FencedDirective([Container()], ":")
```

### Comparing `blurry_cli-0.1.0/blurry/markdown/front_matter.py` & `blurry_cli-0.2.0/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/markdown/punctuation_plugin.py` & `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from re import Match
 from mistune import InlineState, InlineParser, Markdown
 
 EM_DASH_PATTERN = r"---"
 EN_DASH_PATTERN = r"--"
 
 
-def parse_em_dash(_: InlineParser, m: Match, state: InlineState):
-    pos = m.end()
+def parse_em_dash(_: InlineParser, match: Match, state: InlineState):
+    pos = match.end()
     state.append_token({"type": "text", "raw": "—"})
     return pos
 
 
-def parse_en_dash(_: InlineParser, m: Match, state: InlineState):
-    pos = m.end()
+def parse_en_dash(_: InlineParser, match: Match, state: InlineState):
+    pos = match.end()
     state.append_token({"type": "text", "raw": "–"})
     return pos
 
 
 def punctuation(md: Markdown):
     md.inline.register("punctuation_em_dash", EM_DASH_PATTERN, parse_em_dash)
     md.inline.register("punctuation_en_dash", EN_DASH_PATTERN, parse_en_dash)
```

### Comparing `blurry_cli-0.1.0/blurry/markdown/python_code_plugin.py` & `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import inspect
 import re
-from operator import attrgetter
+import importlib
 
-from mistune import Markdown
-
-__all__ = ["python_code", "python_code_in_list"]
+from mistune import Markdown, BlockState, BlockParser
 
 PYTHON_CODE_PATTERN = r"[\s]*@(?P<language>[a-z]+)<(?P<path>.+)>"
 
 
-def parse_python_code(block, match: re.Match, state):
+def parse_python_code(_: BlockParser, match: re.Match, state: BlockState):
     language = match.group("language")
     path = match.group("path")
     state.append_token(
         {
             "type": "python_code",
             "attrs": {"language": language, "path": path},
         }
     )
     return match.end() + 1
 
 
 def render_python_code(_, language: str, path: str):
-    package_name, reference_path = path.split(".", 1)
-    package = __import__(package_name)
-    reference = attrgetter(reference_path)(package)
+    module, _, reference_name = path.rpartition(".")
+    module = importlib.import_module(module)
+    try:
+        # If path references a variable within a module
+        reference = getattr(module, reference_name)
+    except AttributeError:
+        # If path references a module
+        reference = importlib.import_module(path)
     reference_source = inspect.getsource(reference)
+
     return f'<pre><code class="language-{language}">{reference_source}</code></pre>'
 
 
 def python_code(md: Markdown):
     """A mistune plugin to insert Python code."""
     md.block.register(
         "python_code", PYTHON_CODE_PATTERN, parse_python_code, before="list"
```

### Comparing `blurry_cli-0.1.0/blurry/open_graph.py` & `blurry_cli-0.2.0/blurry/open_graph.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/settings.py` & `blurry_cli-0.2.0/blurry/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class Settings(TypedDict):
     AVIF_COMPRESSION_QUALITY: int
     BUILD_DIRECTORY_NAME: str
     CONTENT_DIRECTORY_NAME: str
     TEMPLATES_DIRECTORY_NAME: str
+    TEMPLATE_SCHEMA_TYPES: dict[str, str]
 
     DEV_HOST: str
     DEV_PORT: int
     DOMAIN: str
     IMAGE_WIDTHS: list[int]
     MAXIMUM_IMAGE_WIDTH: int
     THUMBNAIL_WIDTH: int
@@ -35,14 +36,15 @@
     # Sizes adapted from: https://link.medium.com/UqzDeLKwyeb
     "IMAGE_WIDTHS": [360, 640, 768, 1024, 1366, 1600, 1920],
     "MAXIMUM_IMAGE_WIDTH": 1920,
     "THUMBNAIL_WIDTH": 250,
     "USE_HTTP": False,
     "RUNSERVER": False,
     "FRONTMATTER_NON_SCHEMA_VARIABLE_PREFIX": "~",
+    "TEMPLATE_SCHEMA_TYPES": {},
 }
 
 try:
     blurry_config = toml.load(open("blurry.toml"))
     user_settings = blurry_config["blurry"]
     for setting, value in user_settings.items():
         SETTINGS[setting.upper()] = value
```

### Comparing `blurry_cli-0.1.0/blurry/sitemap.py` & `blurry_cli-0.2.0/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/blurry/types.py` & `blurry_cli-0.2.0/blurry/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,7 +21,9 @@
     LOCAL_BUSINESS = "LocalBusiness"
     NEWS_MEDIA_ORGANIZATION = "NewsMediaOrganization"
     ORGANIZATION = "Organization"
     PERSON = "Person"
 
 
 DirectoryFileData = dict[Path, list[MarkdownFileData]]
+
+TemplateContext = dict[str, Any]
```

### Comparing `blurry_cli-0.1.0/blurry/utils.py` & `blurry_cli-0.2.0/blurry/utils.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.1.0/pyproject.toml` & `blurry_cli-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
@@ -32,14 +32,15 @@
 Jinja2 = "^3.0.0"
 livereload = "^2.6.3"
 typer = "^0.6.1"
 Wand = "^0.6.6"
 toml = "^0.10.2"
 htmlmin = "^0.1.12"
 selectolax = "^0.3.6"
+rich = "^13.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 pytest-watch = "^4.2.0"
 pytest-cov = "^2.11.1"
 black = "^22.10.0"
 
@@ -53,8 +54,17 @@
 [tool.pyright]
 include = ["blurry/**"]
 exclude = [
     "**/node_modules",
     "**/__pycache__",
     "**/.*",
     "blurry/tests"
-]
+]
+
+[tool.poetry.plugins."blurry.html_plugins"]
+minify_html = 'blurry.plugins.html_plugins.minify_html_plugin:minify_html'
+
+[tool.poetry.plugins."blurry.markdown_plugins"]
+python_code = 'blurry.plugins.markdown_plugins.python_code_plugin:python_code'
+python_code_in_list = 'blurry.plugins.markdown_plugins.python_code_plugin:python_code_in_list'
+punctuation = 'blurry.plugins.markdown_plugins.punctuation_plugin:punctuation'
+container = 'blurry.plugins.markdown_plugins.container_plugin:container'
```

