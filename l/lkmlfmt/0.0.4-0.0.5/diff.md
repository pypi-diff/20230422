# Comparing `tmp/lkmlfmt-0.0.4.tar.gz` & `tmp/lkmlfmt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.4.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.5.tar", max compression
```

## Comparing `lkmlfmt-0.0.4.tar` & `lkmlfmt-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2647 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/README.md
--rw-r--r--   0        0        0       53 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2391 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/exception.py
--rw-r--r--   0        0        0    10847 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      757 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/parser.py
--rw-r--r--   0        0        0     4802 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/template.py
--rw-r--r--   0        0        0      552 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2647 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/README.md
+-rw-r--r--   0        0        0       53 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2546 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    11101 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/parser.py
+-rw-r--r--   0        0        0     4806 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/template.py
+-rw-r--r--   0        0        0      552 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.5/PKG-INFO
```

### Comparing `lkmlfmt-0.0.4/README.md` & `lkmlfmt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.4/lkmlfmt/command.py` & `lkmlfmt-0.0.5/lkmlfmt/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,39 +12,44 @@
 
 @click.command()
 @click.argument("file", type=click.Path(exists=True, path_type=Path), nargs=-1)
 @click.option(
     "--check",
     is_flag=True,
     help="\
-Don't update files.\
+Don't update files. \
 Instead, exit with status code 1 if any file should be modefied.",
 )
 @click.option(
+    "--clickhouse",
+    is_flag=True,
+    help="Specify `--dialect clickhouse` option when using sqlfmt.",
+)
+@click.option(
     "--log-level",
     type=click.Choice(
         ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
     ),
     default="WARNING",
 )
-def run(file: list[Path], check: bool, log_level: str) -> None:
+def run(file: list[Path], check: bool, clickhouse: bool, log_level: str) -> None:
     """Format LookML file(s).
 
     FILE is the LookML file(s) to format (directory is also OK).
     Files which does not end with `.lkml` will be ignored.
     """
     level = getattr(logging, log_level)
     logging.basicConfig(level=level)
 
     modified: list[bool] = []
 
     for f in filter_lkml(file):
         logger.debug(f"formatting {f}")
         before = f.read_text()
-        after = fmt(before)
+        after = fmt(before, clickhouse)
 
         if before == after:
             click.echo(f"{f} is skipped")
             modified.append(False)
             continue
 
         click.echo(f"{f} is modified")
```

### Comparing `lkmlfmt-0.0.4/lkmlfmt/formatter.py` & `lkmlfmt-0.0.5/lkmlfmt/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 COMMENT_MARKER = "#LKMLFMT_MARKER#"
 COMMENT = re.compile(rf"{COMMENT_MARKER}")
 BLANK_LINE = re.compile(r"^\s*$")
 ESCAPED_STRING_SINGLE = re.compile(r'"(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"')
 ESCAPED_STRING_TRIPLE = re.compile(r'"""(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"""')
 NOT_AND_OR = re.compile(r"(?<!\w)(not|and|or)(?!\w)")
 INDENT_WIDTH = 2
-MODE = api.Mode()
 
 
 class LkmlFormatter:
-    def __init__(self, lkml: str) -> None:
+    def __init__(self, lkml: str, clickhouse: bool) -> None:
         self.lkml = lkml
         self.curr_indent = 0
 
         tree, comments = parser.parse(lkml, set_position=True)
         self.tree = tree
         self.comments = comments
+        self.mode = api.Mode(dialect_name="clickhouse" if clickhouse else "polyglot")
 
     # NOTE
     # parents take care of self.curr_indent, but children call fmt_indent()
     # parents take care of separator of the children
     def fmt(
         self,
         tree: ParseTree | Token | list[ParseTree | Token] | None = None,
@@ -105,17 +105,17 @@
         # sql_xxx: ... ;; or expression_xxx: ... ;;
         with self.indent():
             # https://docs.python.org/3/library/functions.html#property
             Line.prefix = property(  # type: ignore
                 lambda s: " " * INDENT_WIDTH * (s.depth[0] + self.curr_indent)
             )
             if key.startswith("sql"):
-                value = _fmt_sql(value)
+                value = self._fmt_sql(value)
             else:
-                value = _fmt_expr(value)
+                value = self._fmt_expr(value)
 
         if "\n" not in value:
             return f"{lcomments}{self.fmt_indent()}{key}: {value.lstrip()} ;;"
 
         if not value.startswith(" "):  # fallback if sqlfmt does not support
             value = " " * ((self.curr_indent + 1) * INDENT_WIDTH) + value
 
@@ -274,59 +274,57 @@
                 joined += "\n"
 
             joined += "\n"
             joined += self.fmt(t)
 
         return joined
 
+    def _fmt_sql(self, liquid: str) -> str:
+        jinja, templates, dummies = template.to_jinja(liquid, "sqlfmt")
+        jinja = api.format_string(jinja, mode=self.mode).rstrip()
+        liquid = template.to_liquid_sqlfmt(jinja, templates, dummies)
+        return liquid
+
+    # NOTE let's rely on sqlfmt for not only sql but also looker expression!
+    def _fmt_expr(self, liquid: str) -> str:
+        # convert looker expr into sql
+        temp = liquid
+        temp = temp.replace("case", "lkmlfmt_case")
+        temp = temp.replace("when", "lkmlfmt_when")
+        temp = ESCAPED_STRING_SINGLE.sub(r'"""\g<inner>"""', temp)  # " -> """
+
+        temp = self._fmt_sql(temp)
+
+        # convert sql into looker expression
+        temp = ESCAPED_STRING_TRIPLE.sub(r'"\g<inner>"', temp)
+        temp = temp.replace("lkmlfmt_when", "when")
+        temp = temp.replace("lkmlfmt_case", "case")
+
+        splited = ESCAPED_STRING_SINGLE.split(temp)
+        expr = ""
+        for i, s in enumerate(splited):
+            match divmod(i, 4)[1]:  # mod
+                case 0:
+                    uppered = NOT_AND_OR.sub(lambda x: x.group(0).upper(), s)
+                    expr += uppered
+                case 1:
+                    expr += f'"{s}"'
+
+        return expr
+
 
 def _token(token: Token | ParseTree) -> Token:
     if isinstance(token, Token):
         return token
     raise LkmlfmtException()
 
 
 def _fmt_html(liquid: str) -> str:
     jinja, templates, dummies = template.to_jinja(liquid, "djhtml")
     jinja = DjHTML(jinja).indent(2)
     liquid = template.to_liquid_djhtml(jinja, templates, dummies)
     return liquid
 
 
-def _fmt_sql(liquid: str) -> str:
-    jinja, templates, dummies = template.to_jinja(liquid, "sqlfmt")
-    jinja = api.format_string(jinja, mode=MODE).rstrip()
-    liquid = template.to_liquid_sqlfmt(jinja, templates, dummies)
-    return liquid
-
-
-# NOTE let's rely on sqlfmt for not only sql but also looker expression!
-def _fmt_expr(liquid: str) -> str:
-    # convert looker expr into sql
-    temp = liquid
-    temp = temp.replace("case", "lkmlfmt_case")
-    temp = temp.replace("when", "lkmlfmt_when")
-    temp = ESCAPED_STRING_SINGLE.sub(r'"""\g<inner>"""', temp)  # " -> """
-
-    temp = _fmt_sql(temp)
-
-    # convert sql into looker expression
-    temp = ESCAPED_STRING_TRIPLE.sub(r'"\g<inner>"', temp)
-    temp = temp.replace("lkmlfmt_when", "when")
-    temp = temp.replace("lkmlfmt_case", "case")
-
-    splited = ESCAPED_STRING_SINGLE.split(temp)
-    expr = ""
-    for i, s in enumerate(splited):
-        match divmod(i, 4)[1]:  # mod
-            case 0:
-                uppered = NOT_AND_OR.sub(lambda x: x.group(0).upper(), s)
-                expr += uppered
-            case 1:
-                expr += f'"{s}"'
-
-    return expr
-
-
-def fmt(lkml: str) -> str:
-    formatter = LkmlFormatter(lkml)
+def fmt(lkml: str, clickhouse: bool) -> str:
+    formatter = LkmlFormatter(lkml, clickhouse)
     return formatter.fmt()
```

### Comparing `lkmlfmt-0.0.4/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.5/lkmlfmt/lkml.lark`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.4/lkmlfmt/parser.py` & `lkmlfmt-0.0.5/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.4/lkmlfmt/template.py` & `lkmlfmt-0.0.5/lkmlfmt/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Literal
 
 LIQUID_MARKER = "{{% set LKMLFMT_MARKER = {} %}}"
 TEMPLATE = re.compile(
     r"""(?P<tag>\{%-?\s*(?P<type>#|([a-z]*))([^"'}]*|'[^']*?'|"[^"]*?")*?-?%\})"""
     + r"""|(?P<obj>\{\{([^"'}]*|'[^']*?'|"[^"]*?")*?\}\})"""
-    + r"""|(?P<looker>\$\{[^}]*?\})""",
+    + r"""|(?P<looker>(\$|@)\{[^}]*?\})""",
 )
 DUMMY = re.compile(r"^(?P<lead_n> *?\n)?(?P<indent> *)")
 
 MODE = Literal["sqlfmt", "djhtml"]
 
 
 def to_jinja(liquid: str, mode: MODE = "sqlfmt") -> tuple[str, list[str], list[str]]:
```

### Comparing `lkmlfmt-0.0.4/pyproject.toml` & `lkmlfmt-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
```

### Comparing `lkmlfmt-0.0.4/PKG-INFO` & `lkmlfmt-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkmlfmt
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: dr666m1
 Author-email: skndr666m1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

