# Comparing `tmp/orgee-0.0.4.tar.gz` & `tmp/orgee-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orgee-0.0.4.tar", last modified: Sun Dec 25 09:12:17 2022, max compression
+gzip compressed data, was "orgee-0.0.5.tar", last modified: Sat Apr 22 04:03:58 2023, max compression
```

## Comparing `orgee-0.0.4.tar` & `orgee-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 09:12:17.793853 orgee-0.0.4/
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)      385 2022-12-25 09:12:17.793853 orgee-0.0.4/PKG-INFO
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)       97 2022-12-25 09:11:38.000000 orgee-0.0.4/README.md
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)      121 2022-12-25 09:11:38.000000 orgee-0.0.4/pyproject.toml
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)      548 2022-12-25 09:12:17.793853 orgee-0.0.4/setup.cfg
-drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 09:12:17.793853 orgee-0.0.4/src/
-drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 09:12:17.793853 orgee-0.0.4/src/orgee/
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)       61 2022-12-25 05:46:06.000000 orgee-0.0.4/src/orgee/__init__.py
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)     9758 2022-12-25 03:25:33.000000 orgee-0.0.4/src/orgee/orgnode.py
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)     6572 2022-12-10 01:34:18.000000 orgee-0.0.4/src/orgee/parse_org.py
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 03:38:40.000000 orgee-0.0.4/src/orgee/py.typed
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)     3770 2022-12-25 04:55:04.000000 orgee-0.0.4/src/orgee/util.py
-drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 09:12:17.793853 orgee-0.0.4/src/orgee.egg-info/
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)      385 2022-12-25 09:12:17.000000 orgee-0.0.4/src/orgee.egg-info/PKG-INFO
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)      297 2022-12-25 09:12:17.000000 orgee-0.0.4/src/orgee.egg-info/SOURCES.txt
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)        1 2022-12-25 09:12:17.000000 orgee-0.0.4/src/orgee.egg-info/dependency_links.txt
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)        6 2022-12-25 09:12:17.000000 orgee-0.0.4/src/orgee.egg-info/top_level.txt
--rw-r--r--   0 chunglak  (1000) chunglak  (1000)        1 2022-12-25 09:02:52.000000 orgee-0.0.4/src/orgee.egg-info/zip-safe
+drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2023-04-22 04:03:58.647761 orgee-0.0.5/
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      386 2023-04-22 04:03:58.647761 orgee-0.0.5/PKG-INFO
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)       98 2023-04-22 04:03:49.000000 orgee-0.0.5/README.md
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      121 2023-04-22 04:03:49.000000 orgee-0.0.5/pyproject.toml
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      568 2023-04-22 04:03:58.651095 orgee-0.0.5/setup.cfg
+drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2023-04-22 04:03:58.644428 orgee-0.0.5/src/
+drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2023-04-22 04:03:58.647761 orgee-0.0.5/src/orgee/
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      150 2023-01-01 14:14:16.000000 orgee-0.0.5/src/orgee/__init__.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      740 2023-01-01 08:30:52.000000 orgee-0.0.5/src/orgee/link.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      730 2023-01-01 08:11:32.000000 orgee-0.0.5/src/orgee/markup.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)     8957 2023-01-01 14:14:54.000000 orgee-0.0.5/src/orgee/orgnode.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)     6631 2023-01-01 14:14:25.000000 orgee-0.0.5/src/orgee/parse_org.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)     4989 2023-01-21 13:11:03.000000 orgee-0.0.5/src/orgee/properties.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)        0 2022-12-25 03:38:40.000000 orgee-0.0.5/src/orgee/py.typed
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      285 2023-01-29 10:45:19.000000 orgee-0.0.5/src/orgee/tag.py
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)     3770 2023-01-29 10:44:55.000000 orgee-0.0.5/src/orgee/util.py
+drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2023-04-22 04:03:58.647761 orgee-0.0.5/src/orgee.egg-info/
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      386 2023-04-22 04:03:58.000000 orgee-0.0.5/src/orgee.egg-info/PKG-INFO
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      405 2023-04-22 04:03:58.000000 orgee-0.0.5/src/orgee.egg-info/SOURCES.txt
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)        1 2023-04-22 04:03:58.000000 orgee-0.0.5/src/orgee.egg-info/dependency_links.txt
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)        6 2023-04-22 04:03:58.000000 orgee-0.0.5/src/orgee.egg-info/top_level.txt
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)        1 2022-12-25 09:02:52.000000 orgee-0.0.5/src/orgee.egg-info/zip-safe
+drwxr-xr-x   0 chunglak  (1000) chunglak  (1000)        0 2023-04-22 04:03:58.647761 orgee-0.0.5/tests/
+-rw-r--r--   0 chunglak  (1000) chunglak  (1000)      716 2022-12-25 04:55:44.000000 orgee-0.0.5/tests/test_parse_property.py
```

### Comparing `orgee-0.0.4/setup.cfg` & `orgee-0.0.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = orgee
-version = 0.0.4
+version = 0.0.5
 url = https://github.com/chunglak/orgee
 author = Alfred Leung
 author_email = chunglak@gmail.com
 description = A tool to manipulate org-mode documents
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL-3.0-or-later
@@ -12,14 +12,15 @@
 [options]
 python_requires = >=3.10
 package_dir = 
 	=src
 packages = find:
 zip_safe = True
 include_package_data = True
+install_requires = 
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [options.package_data]
```

### Comparing `orgee-0.0.4/src/orgee/orgnode.py` & `orgee-0.0.5/src/orgee/orgnode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 from __future__ import annotations  # PEP 585
 
 import hashlib
+from enum import Enum
 from dataclasses import dataclass, field
 from typing import Any, Iterator  # pylint:disable=unused-import
 
-from .util import (
-    prop_by_key,
-    first_prop_by_key,
-    replace_prop,
-    clean_text,
-    extract_url,
-)
+from .properties import OrgProperties
+from .markup import remove_org_markup
+from .link import extract_url
 
 NOT_FOUND = -1
+DEFAULT_TODOS = (["TODO"], ["DONE"])
+
+
+class TodoType(Enum):
+    DONE = 0
+    TODO = 1
+    INVALID = 2
 
 
 @dataclass
 class RootMeta:
     # List of custom todos for the file
-    ptodos: tuple[list[str], list[str]] | None = None
+    # First list are the TODO keywords, second the DONE keywords
+    _todos: tuple[list[str], list[str]] | None = None
     # These are the files-wide properties (#+PROPERTY:)
     # Not the ones inside the properties drawer
-    properties: list[str] = field(default_factory=list)
+    file_properties: list[str] = field(default_factory=list)
     # Other #+-type of file-wide settings
     other_meta: list[tuple[str, str]] = field(default_factory=list)
 
     @property
     def todos(self) -> tuple[list[str], list[str]]:
-        return self.ptodos if self.ptodos else (["TODO"], ["DONE"])
+        return self._todos if self._todos else DEFAULT_TODOS
+
+    @todos.setter
+    def todos(self, todos: tuple[list[str], list[str]]):
+        self._todos = todos
 
-    def todo_type(self, kw: str) -> int:
+    def todo_type(self, kw: str) -> TodoType:
         todos, dones = self.todos
         if kw in todos:
-            return 1
+            return TodoType.TODO
         elif kw in dones:
-            return -1
+            return TodoType.DONE
         else:
-            return 0
-
-    def other_meta_by_key(
-        self, key: str, parse=True, case_insensitive=True
-    ) -> list:
-        return prop_by_key(
-            key=key,
-            props=self.other_meta,
-            parse=parse,
-            case_insensitive=case_insensitive,
-        )
-
-    def first_other_meta_by_key(
-        self, key: str, parse=True, case_insensitive=True
-    ) -> str | None:
-        return first_prop_by_key(
-            key=key,
-            props=self.other_meta,
-            parse=parse,
-            case_insensitive=case_insensitive,
-        )
+            return TodoType.INVALID
 
 
 class OrgNode:
     """
     If a node is a root nod (file node) then
     it has no parent, but it has a root_meta
     """
@@ -78,58 +67,46 @@
         self.root_meta: RootMeta | None = RootMeta() if is_root else None
         self.parent: OrgNode | None = parent
         # A node cannot both be a root node and have a parent
         assert not (self.root_meta and self.parent)
         # This lineno only works at import time
         # When the nodes are changed it's not valid anymore
         self.lineno: int = 1
-        self.properties: list[tuple[str, str]] = []
+        self.properties: OrgProperties = OrgProperties()
         self.children: list[OrgNode] = []
         self.todo: str | None = todo
         self.level: int | None = None
         self.title: str = title if title else ""
         self.body: list[str] = body if body else []
         self.tags: set[str] = tags if tags else set()
         self.counter_cookie: tuple[int, int] | None = counter_cookie
         self.find_child_by_title_index: int = NOT_FOUND
 
+    @staticmethod
+    def from_file(fn: str) -> OrgNode:
+        # pylint: disable=import-outside-toplevel
+        from .parse_org import parse_org_file
+
+        return parse_org_file(fn)
+
+    def __str__(self):
+        return self.title
+
     def all_tags(self) -> set[str]:
         """
         Return both the node's own tags and all the tags inherited from parent(s)
         """
         if self.parent:
             return self.tags | self.parent.all_tags()
         else:
             return self.tags
 
     def node_hash(self) -> str:
         return hashlib.sha256(self.dumps().encode("utf8")).hexdigest()
 
-    def prop_by_key(self, key: str, parse=True, case_insensitive=True) -> list:
-        return prop_by_key(
-            key=key,
-            props=self.properties,
-            parse=parse,
-            case_insensitive=case_insensitive,
-        )
-
-    def first_prop_by_key(
-        self, key: str, parse=True, case_insensitive=True
-    ) -> str | None:
-        ps = self.prop_by_key(
-            key=key, parse=parse, case_insensitive=case_insensitive
-        )
-        return ps[0] if ps else None
-
-    def replace_prop(self, key, value=None) -> list:
-        ps, self.properties = replace_prop(
-            key=key, props=self.properties, value=value
-        )
-        return ps
-
     def recurse_nodes(self) -> list[OrgNode]:
         """
         Depth-first traversal
         """
         nodes = [self]
         for c in self.children:
             nodes.extend(c.recurse_nodes())
@@ -154,41 +131,34 @@
     def dump(self, fn: str):
         with open(fn, "w", encoding="utf-8") as fh:
             fh.write(self.dumps())
 
     def dumps(self) -> str:
         ls: list[str] = []
         if rm := self.root_meta:
-            if self.properties:
-                ls.append(":PROPERTIES:")
-                for k, v in self.properties:
-                    ls.append(f":{k}: {v}")
-                ls.append(":END:")
+            if self.properties.has_properties():
+                ls.append(self.properties.dumps(create_drawer=True))
             if self.title:
                 ls.append(f"#+TITLE: {self.title}")
             if tags := sorted(self.tags):
                 ls.append(f"#+FILETAGS: {' '.join(tags)}")
-            if ptodos := rm.ptodos:
+            if (todos := rm.todos) != DEFAULT_TODOS:
                 ls.append(
-                    "#+TODO: %s | %s"
-                    % (" ".join(ptodos[0]), " ".join(ptodos[1]))
+                    "#+TODO: %s | %s" % (" ".join(todos[0]), " ".join(todos[1]))
                 )
-            if ps := rm.properties:
+            if ps := rm.file_properties:
                 for p in ps:
                     ls.append(f"#+PROPERTY: {p}")
             if ms := rm.other_meta:
                 for k, v in ms:
                     ls.append(f"#+{k.upper()}: {v}")
         else:
             ls.append(self.dump_heading())
-            if self.properties:
-                ls.append(":PROPERTIES:")
-                for k, v in self.properties:
-                    ls.append(f":{k}: {v}")
-                ls.append(":END:")
+            if self.properties.has_properties():
+                ls.append(self.properties.dumps(create_drawer=True))
         if body := self.body:
             ls.append("\n".join(body))
         for c in self.children:
             ls.append(c.dumps())
         return "\n".join(ls)
         # return ("\n".join(ls)).strip()
 
@@ -266,27 +236,27 @@
         title: str | None = None,
         url: str | None = None,
         tags: list[str] | None = None,
         startswith=False,
     ) -> OrgNode | None:
         def matching(s: str) -> bool:
             if title:
-                cs = clean_text(s)
+                cs = remove_org_markup(s)
                 if startswith:
                     # print(f"cs={cs}\ntitle={title}")
                     if not cs.startswith(title):
                         return False
                 elif cs != title:
                     return False
             if url and extract_url(s) != url:
                 return False
             return True
 
         if title:
-            title = clean_text(title)
+            title = remove_org_markup(title)
         for i, child in enumerate(self.children):
             # if clean_text(child.title) == title:
             if matching(child.title):
                 if tags and not (set(tags) <= set(child.tags)):
                     continue
                 self.find_child_by_title_index = i
                 return child
@@ -306,8 +276,8 @@
             if n:
                 return n.find_olp(olp[1:])
             else:
                 print(f"Failed at {olp[0]}")
                 return None
 
     def clean_title(self) -> str:
-        return clean_text(self.title)
+        return remove_org_markup(self.title)
```

### Comparing `orgee-0.0.4/src/orgee/parse_org.py` & `orgee-0.0.5/src/orgee/parse_org.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations  # PEP 585
 
 import logging
 import re
 
-from .orgnode import OrgNode, RootMeta
+from .orgnode import OrgNode, RootMeta, TodoType
+from .properties import OrgProperty
 
 
 def parse_org_file(fn: str) -> OrgNode:
     with open(fn, "r", encoding="utf8") as fh:
         return parse_org_document(fh.read())
 
 
@@ -79,16 +80,15 @@
                 in_props = False
             else:
                 m = re.match(r":([\w:\-\+]+):\s*(.*)\s*", line.lstrip())
                 if not m:
                     print(line)
                     raise Exception("Bad property")
                 k, v = m.groups()
-                node.properties.append((k, v))
-                # node.properties.append((k, process_property(v)))
+                node.properties.add_property(OrgProperty.from_raw((k, v)))
         elif is_root and lsl.startswith("#+"):
             assert node.root_meta
             rm = node.root_meta
             m = re.match(r"#\+([\w\-\+]+):\s*(.*)\s*", line.lstrip())
             if not m:
                 if lsl.startswith("#+begin_") or lsl.startswith("#+end"):
                     bodyl.append(line)
@@ -100,25 +100,25 @@
             kl = k.lower()
             if kl == "title":
                 node.title = v
             elif kl == "filetags":
                 # rm.filetags.update([t for t in v.split(" ") if t])
                 node.tags.update([t for t in v.split(" ") if t])
             elif kl == "property":
-                rm.properties.append(v)
+                rm.file_properties.append(v)
             elif kl == "todo":
                 if "|" in v:
                     stodos, sdones = v.split("|", maxsplit=1)
                     todos = [t.strip() for t in stodos.split(" ")]
                     dones = [t.strip() for t in sdones.split(" ")]
                 else:
                     ts = [t.strip() for t in v.split(" ")]
                     todos = ts[:-1]
                     dones = [ts[-1]]
-                rm.ptodos = ([t for t in todos if t], [t for t in dones if t])
+                rm.todos = ([t for t in todos if t], [t for t in dones if t])
             else:
                 node.root_meta.other_meta.append((k, v))
         else:
             bodyl.append(line)
 
         i += 1
     node.body = bodyl
@@ -139,15 +139,18 @@
         logging.error(stars)
         raise Exception("Heading doesn't start with stars!")
     dic["level"] = len(stars)
     # Parse todo
     if not root_meta:
         root_meta = RootMeta()
     todosplit = rest.split(" ", maxsplit=1)
-    if len(todosplit) > 1 and root_meta.todo_type(todosplit[0]):
+    if (
+        len(todosplit) > 1
+        and root_meta.todo_type(todosplit[0]) is not TodoType.INVALID
+    ):
         dic["todo"] = todosplit[0]
         rest = todosplit[1]
 
     m = re.match(r"(.*?)\s*:([\w@:]+):\s*$", rest)
     if m:
         title, tags = m.groups()
         dic["tags"] = tags.split(":")
```

### Comparing `orgee-0.0.4/src/orgee/util.py` & `orgee-0.0.5/src/orgee/util.py`

 * *Files identical despite different names*

