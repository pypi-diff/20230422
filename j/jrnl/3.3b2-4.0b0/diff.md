# Comparing `tmp/jrnl-3.3b2.tar.gz` & `tmp/jrnl-4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrnl-3.3b2.tar", max compression
+gzip compressed data, was "jrnl-4.0b0.tar", max compression
```

## Comparing `jrnl-3.3b2.tar` & `jrnl-4.0b0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
--rw-r--r--   0        0        0    34916 2022-10-22 22:38:23.376022 jrnl-3.3b2/LICENSE.md
--rw-r--r--   0        0        0     3117 2022-10-22 22:38:23.376022 jrnl-3.3b2/README.md
--rw-r--r--   0        0        0     8994 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/DayOneJournal.py
--rw-r--r--   0        0        0     7548 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/EncryptedJournal.py
--rw-r--r--   0        0        0     7713 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/Entry.py
--rw-r--r--   0        0        0     4052 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/FolderJournal.py
--rw-r--r--   0        0        0    16605 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/Journal.py
--rw-r--r--   0        0        0      213 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/__init__.py
--rw-r--r--   0        0        0      182 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/__main__.py
--rw-r--r--   0        0        0       27 2022-10-22 22:38:31.792127 jrnl-3.3b2/jrnl/__version__.py
--rw-r--r--   0        0        0    11826 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/args.py
--rw-r--r--   0        0        0     2103 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/cli.py
--rw-r--r--   0        0        0     3078 2022-10-22 22:38:23.380022 jrnl-3.3b2/jrnl/color.py
--rw-r--r--   0        0        0     4929 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/commands.py
--rw-r--r--   0        0        0     7379 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/config.py
--rw-r--r--   0        0        0     2003 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/editor.py
--rw-r--r--   0        0        0      412 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/exception.py
--rw-r--r--   0        0        0     4933 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/install.py
--rw-r--r--   0        0        0    13456 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/jrnl.py
--rw-r--r--   0        0        0      351 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/messages/Message.py
--rw-r--r--   0        0        0     2259 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/messages/MsgStyle.py
--rw-r--r--   0        0        0     8380 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/messages/MsgText.py
--rw-r--r--   0        0        0      282 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/messages/__init__.py
--rw-r--r--   0        0        0      381 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/os_compat.py
--rw-r--r--   0        0        0     3314 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/output.py
--rw-r--r--   0        0        0     2373 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/override.py
--rw-r--r--   0        0        0      319 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/path.py
--rw-r--r--   0        0        0     1452 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/__init__.py
--rw-r--r--   0        0        0      880 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/dates_exporter.py
--rw-r--r--   0        0        0     3815 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/fancy_exporter.py
--rw-r--r--   0        0        0     1426 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/jrnl_importer.py
--rw-r--r--   0        0        0     2389 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/json_exporter.py
--rw-r--r--   0        0        0     3149 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/markdown_exporter.py
--rw-r--r--   0        0        0     1111 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/tag_exporter.py
--rw-r--r--   0        0        0     3578 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/text_exporter.py
--rw-r--r--   0        0        0      968 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/util.py
--rw-r--r--   0        0        0     2340 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/xml_exporter.py
--rw-r--r--   0        0        0     5075 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/plugins/yaml_exporter.py
--rw-r--r--   0        0        0     1745 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/prompt.py
--rw-r--r--   0        0        0      220 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/templates/sample.template
--rw-r--r--   0        0        0     3003 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/time.py
--rw-r--r--   0        0        0     5719 2022-10-22 22:38:23.384022 jrnl-3.3b2/jrnl/upgrade.py
--rw-r--r--   0        0        0     3914 2022-10-22 22:38:31.748127 jrnl-3.3b2/pyproject.toml
--rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 jrnl-3.3b2/setup.py
--rw-r--r--   0        0        0     4509 1970-01-01 00:00:00.000000 jrnl-3.3b2/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-03-25 23:04:12.940390 jrnl-4.0b0/LICENSE.md
+-rw-r--r--   0        0        0     3117 2023-03-25 23:04:12.940390 jrnl-4.0b0/README.md
+-rw-r--r--   0        0        0      213 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/__init__.py
+-rw-r--r--   0        0        0      183 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/__main__.py
+-rw-r--r--   0        0        0       26 2023-03-25 23:04:23.104532 jrnl-4.0b0/jrnl/__version__.py
+-rw-r--r--   0        0        0    13775 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/args.py
+-rw-r--r--   0        0        0     3227 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/color.py
+-rw-r--r--   0        0        0     4942 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/commands.py
+-rw-r--r--   0        0        0     8445 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/config.py
+-rw-r--r--   0        0        0    16420 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/controller.py
+-rw-r--r--   0        0        0     2031 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/editor.py
+-rw-r--r--   0        0        0     1480 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/BaseEncryption.py
+-rw-r--r--   0        0        0      192 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/BaseKeyEncryption.py
+-rw-r--r--   0        0        0     2447 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/BasePasswordEncryption.py
+-rw-r--r--   0        0        0     1657 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/Jrnlv1Encryption.py
+-rw-r--r--   0        0        0     1850 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/Jrnlv2Encryption.py
+-rw-r--r--   0        0        0      571 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/NoEncryption.py
+-rw-r--r--   0        0        0      954 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/encryption/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/exception.py
+-rw-r--r--   0        0        0     5856 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/install.py
+-rw-r--r--   0        0        0     8969 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/journals/DayOneJournal.py
+-rw-r--r--   0        0        0     8050 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/journals/Entry.py
+-rw-r--r--   0        0        0     4405 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/journals/FolderJournal.py
+-rw-r--r--   0        0        0    18385 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/journals/Journal.py
+-rw-r--r--   0        0        0      156 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/journals/__init__.py
+-rw-r--r--   0        0        0     1045 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/keyring.py
+-rw-r--r--   0        0        0     2263 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/main.py
+-rw-r--r--   0        0        0      409 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/messages/Message.py
+-rw-r--r--   0        0        0     2259 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/messages/MsgStyle.py
+-rw-r--r--   0        0        0     9438 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/messages/MsgText.py
+-rw-r--r--   0        0        0      282 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/messages/__init__.py
+-rw-r--r--   0        0        0      415 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/os_compat.py
+-rw-r--r--   0        0        0     3429 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/output.py
+-rw-r--r--   0        0        0     2463 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/override.py
+-rw-r--r--   0        0        0      350 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/path.py
+-rw-r--r--   0        0        0     1545 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/__init__.py
+-rw-r--r--   0        0        0     1033 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/dates_exporter.py
+-rw-r--r--   0        0        0     3997 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/fancy_exporter.py
+-rw-r--r--   0        0        0     1549 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/jrnl_importer.py
+-rw-r--r--   0        0        0     2566 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/json_exporter.py
+-rw-r--r--   0        0        0     3309 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/markdown_exporter.py
+-rw-r--r--   0        0        0     1272 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/tag_exporter.py
+-rw-r--r--   0        0        0     3844 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/text_exporter.py
+-rw-r--r--   0        0        0     1107 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/util.py
+-rw-r--r--   0        0        0     2605 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/xml_exporter.py
+-rw-r--r--   0        0        0     5230 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/plugins/yaml_exporter.py
+-rw-r--r--   0        0        0     2086 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/prompt.py
+-rw-r--r--   0        0        0      220 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/templates/sample.template
+-rw-r--r--   0        0        0     3117 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/time.py
+-rw-r--r--   0        0        0     6164 2023-03-25 23:04:12.944390 jrnl-4.0b0/jrnl/upgrade.py
+-rw-r--r--   0        0        0     4095 2023-03-25 23:04:23.056531 jrnl-4.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 jrnl-4.0b0/PKG-INFO
```

### Comparing `jrnl-3.3b2/LICENSE.md` & `jrnl-4.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jrnl-3.3b2/README.md` & `jrnl-4.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--
-Copyright © 2012-2022 jrnl contributors
+Copyright © 2012-2023 jrnl contributors
 License: https://www.gnu.org/licenses/gpl-3.0.html
 -->
 
 <p align="center">
 <a href="https://jrnl.sh">
 <img align="center" src="https://raw.githubusercontent.com/jrnl-org/jrnl/develop/docs_theme/assets/readme-header.png"/>
 </a>
```

### Comparing `jrnl-3.3b2/jrnl/DayOneJournal.py` & `jrnl-4.0b0/jrnl/journals/DayOneJournal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+import contextlib
 import datetime
 import fnmatch
 import os
 import platform
 import plistlib
 import re
 import socket
@@ -12,21 +13,22 @@
 import uuid
 import zoneinfo
 from pathlib import Path
 from xml.parsers.expat import ExpatError
 
 import tzlocal
 
-from jrnl import Entry
-from jrnl import Journal
 from jrnl import __title__
 from jrnl import __version__
 
+from .Entry import Entry
+from .Journal import Journal
 
-class DayOne(Journal.Journal):
+
+class DayOne(Journal):
     """A special Journal handling DayOne files"""
 
     # InvalidFileException was added to plistlib in Python3.4
     PLIST_EXCEPTIONS = (
         (ExpatError, plistlib.InvalidFileException)
         if hasattr(plistlib, "InvalidFileException")
         else ExpatError
@@ -34,15 +36,15 @@
 
     def __init__(self, **kwargs):
         self.entries = []
         self._deleted_entries = []
         self.can_be_encrypted = False
         super().__init__(**kwargs)
 
-    def open(self):
+    def open(self) -> "DayOne":
         filenames = []
         for root, dirnames, f in os.walk(self.config["journal"]):
             for filename in fnmatch.filter(f, "*.doentry"):
                 filenames.append(os.path.join(root, filename))
         self.entries = []
         for filename in filenames:
             with open(filename, "rb") as plist_entry:
@@ -58,66 +60,51 @@
                         timezone = zoneinfo.ZoneInfo(timezone_name)
                     date = dict_entry["Creation Date"]
                     # convert the date to UTC rather than keep messing with
                     # timezones
                     if timezone.key != "UTC":
                         date = date.replace(fold=1) + timezone.utcoffset(date)
 
-                    entry = Entry.Entry(
+                    entry = Entry(
                         self,
                         date,
                         text=dict_entry["Entry Text"],
                         starred=dict_entry["Starred"],
                     )
                     entry.uuid = dict_entry["UUID"]
                     entry._tags = [
                         self.config["tagsymbols"][0] + tag.lower()
                         for tag in dict_entry.get("Tags", [])
                     ]
+                    if entry._tags:
+                        entry._tags.sort()
 
                     """Extended DayOne attributes"""
-                    try:
+                    # just ignore it if the keys don't exist
+                    with contextlib.suppress(KeyError):
                         entry.creator_device_agent = dict_entry["Creator"][
                             "Device Agent"
                         ]
-                    except:  # noqa: E722
-                        pass
-                    try:
-                        entry.creator_generation_date = dict_entry["Creator"][
-                            "Generation Date"
-                        ]
-                    except:  # noqa: E722
-                        entry.creator_generation_date = date
-                    try:
                         entry.creator_host_name = dict_entry["Creator"]["Host Name"]
-                    except:  # noqa: E722
-                        pass
-                    try:
                         entry.creator_os_agent = dict_entry["Creator"]["OS Agent"]
-                    except:  # noqa: E722
-                        pass
-                    try:
                         entry.creator_software_agent = dict_entry["Creator"][
                             "Software Agent"
                         ]
-                    except:  # noqa: E722
-                        pass
-                    try:
                         entry.location = dict_entry["Location"]
-                    except:  # noqa: E722
-                        pass
-                    try:
                         entry.weather = dict_entry["Weather"]
-                    except:  # noqa: E722
-                        pass
+
+                    entry.creator_generation_date = dict_entry.get("Creator", {}).get(
+                        "Generation Date", date
+                    )
+
                     self.entries.append(entry)
         self.sort()
         return self
 
-    def write(self):
+    def write(self) -> None:
         """Writes only the entries that have been modified into plist files."""
         for entry in self.entries:
             if entry.modified:
                 utc_time = datetime.datetime.utcfromtimestamp(
                     time.mktime(entry.date.timetuple())
                 )
 
@@ -173,52 +160,60 @@
 
         for entry in self._deleted_entries:
             filename = os.path.join(
                 self.config["journal"], "entries", entry.uuid + ".doentry"
             )
             os.remove(filename)
 
-    def editable_str(self):
+    def editable_str(self) -> str:
         """Turns the journal into a string of entries that can be edited
         manually and later be parsed with eslf.parse_editable_str."""
         return "\n".join([f"{str(e)}\n# {e.uuid}\n" for e in self.entries])
 
-    def _update_old_entry(self, entry, new_entry):
-        for attr in ("title", "body", "date"):
+    def _update_old_entry(self, entry: Entry, new_entry: Entry) -> None:
+        for attr in ("title", "body", "date", "tags"):
             old_attr = getattr(entry, attr)
             new_attr = getattr(new_entry, attr)
             if old_attr != new_attr:
                 entry.modified = True
                 setattr(entry, attr, new_attr)
 
-    def _get_and_remove_uuid_from_entry(self, entry):
+    def _get_and_remove_uuid_from_entry(self, entry: Entry) -> Entry:
         uuid_regex = "^ *?# ([a-zA-Z0-9]+) *?$"
         m = re.search(uuid_regex, entry.body, re.MULTILINE)
         entry.uuid = m.group(1) if m else None
 
         # remove the uuid from the body
         entry.body = re.sub(uuid_regex, "", entry.body, flags=re.MULTILINE, count=1)
         entry.body = entry.body.rstrip()
 
         return entry
 
-    def parse_editable_str(self, edited):
+    def parse_editable_str(self, edited: str) -> None:
         """Parses the output of self.editable_str and updates its entries."""
         # Method: create a new list of entries from the edited text, then match
         # UUIDs of the new entries against self.entries, updating the entries
         # if the edited entries differ, and deleting entries from self.entries
         # if they don't show up in the edited entries anymore.
         entries_from_editor = self._parse(edited)
 
         for entry in entries_from_editor:
             entry = self._get_and_remove_uuid_from_entry(entry)
+            if entry._tags:
+                entry._tags.sort()
 
         # Remove deleted entries
         edited_uuids = [e.uuid for e in entries_from_editor]
         self._deleted_entries = [e for e in self.entries if e.uuid not in edited_uuids]
         self.entries[:] = [e for e in self.entries if e.uuid in edited_uuids]
 
         for entry in entries_from_editor:
             for old_entry in self.entries:
                 if entry.uuid == old_entry.uuid:
+                    if old_entry._tags:
+                        tags_not_in_body = [
+                            tag for tag in old_entry._tags if (tag not in entry._body)
+                        ]
+                        if tags_not_in_body:
+                            entry._tags.extend(tags_not_in_body.sort())
                     self._update_old_entry(old_entry, entry)
                     break
```

### Comparing `jrnl-3.3b2/jrnl/Entry.py` & `jrnl-4.0b0/jrnl/journals/Entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,92 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import datetime
 import logging
 import os
 import re
+from typing import TYPE_CHECKING
 
 import ansiwrap
 
-from .color import colorize
-from .color import highlight_tags_with_background_color
+from jrnl.color import colorize
+from jrnl.color import highlight_tags_with_background_color
+
+if TYPE_CHECKING:
+    from .Journal import Journal
 
 
 class Entry:
-    def __init__(self, journal, date=None, text="", starred=False):
+    def __init__(
+        self,
+        journal: "Journal",
+        date: datetime.datetime | None = None,
+        text: str = "",
+        starred: bool = False,
+    ):
         self.journal = journal  # Reference to journal mainly to access its config
         self.date = date or datetime.datetime.now()
         self.text = text
         self._title = None
         self._body = None
         self._tags = None
         self.starred = starred
         self.modified = False
 
     @property
-    def fulltext(self):
+    def fulltext(self) -> str:
         return self.title + " " + self.body
 
     def _parse_text(self):
         raw_text = self.text
         lines = raw_text.splitlines()
         if lines and lines[0].strip().endswith("*"):
             self.starred = True
             raw_text = lines[0].strip("\n *") + "\n" + "\n".join(lines[1:])
         self._title, self._body = split_title(raw_text)
         if self._tags is None:
             self._tags = list(self._parse_tags())
 
     @property
-    def title(self):
+    def title(self) -> str:
         if self._title is None:
             self._parse_text()
         return self._title
 
     @title.setter
-    def title(self, x):
+    def title(self, x: str):
         self._title = x
 
     @property
-    def body(self):
+    def body(self) -> str:
         if self._body is None:
             self._parse_text()
         return self._body
 
     @body.setter
-    def body(self, x):
+    def body(self, x: str):
         self._body = x
 
     @property
-    def tags(self):
+    def tags(self) -> list[str]:
         if self._tags is None:
             self._parse_text()
         return self._tags
 
     @tags.setter
-    def tags(self, x):
+    def tags(self, x: list[str]):
         self._tags = x
 
     @staticmethod
-    def tag_regex(tagsymbols):
+    def tag_regex(tagsymbols: str) -> re.Pattern:
         pattern = rf"(?<!\S)([{tagsymbols}][-+*#/\w]+)"
         return re.compile(pattern)
 
-    def _parse_tags(self):
+    def _parse_tags(self) -> set[str]:
         tagsymbols = self.journal.config["tagsymbols"]
         return {
             tag.lower() for tag in re.findall(Entry.tag_regex(tagsymbols), self.text)
         }
 
     def __str__(self):
         """Returns a string representation of the entry to be written into a journal file."""
@@ -86,15 +96,15 @@
             title += " *"
         return "{title}{sep}{body}\n".format(
             title=title,
             sep="\n" if self.body.rstrip("\n ") else "",
             body=self.body.rstrip("\n "),
         )
 
-    def pprint(self, short=False):
+    def pprint(self, short: bool = False) -> str:
         """Returns a pretty-printed version of the entry.
         If short is true, only print the title."""
         # Handle indentation
         if self.journal.config["indent_character"]:
             indent = self.journal.config["indent_character"].rstrip() + " "
         else:
             indent = ""
@@ -193,26 +203,26 @@
         return "<Entry '{}' on {}>".format(
             self.title.strip(), self.date.strftime("%Y-%m-%d %H:%M")
         )
 
     def __hash__(self):
         return hash(self.__repr__())
 
-    def __eq__(self, other):
+    def __eq__(self, other: "Entry"):
         if (
             not isinstance(other, Entry)
             or self.title.strip() != other.title.strip()
             or self.body.rstrip() != other.body.rstrip()
             or self.date != other.date
             or self.starred != other.starred
         ):
             return False
         return True
 
-    def __ne__(self, other):
+    def __ne__(self, other: "Entry"):
         return not self.__eq__(other)
 
 
 # Based on Segtok by Florian Leitner
 # https://github.com/fnl/segtok
 SENTENCE_SPLITTER = re.compile(
     r"""
@@ -226,15 +236,15 @@
     """,
     re.VERBOSE,
 )
 
 SENTENCE_SPLITTER_ONLY_NEWLINE = re.compile("\n")
 
 
-def split_title(text):
+def split_title(text: str) -> tuple[str, str]:
     """Splits the first sentence off from a text."""
     sep = SENTENCE_SPLITTER_ONLY_NEWLINE.search(text.lstrip())
     if not sep:
         sep = SENTENCE_SPLITTER.search(text)
         if not sep:
             return text, ""
     return text[: sep.end()].strip(), text[sep.end() :].strip()
```

### Comparing `jrnl-3.3b2/jrnl/FolderJournal.py` & `jrnl-4.0b0/jrnl/journals/FolderJournal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import codecs
 import fnmatch
 import os
+from typing import TYPE_CHECKING
 
-from jrnl import Journal
 from jrnl import time
 
+from .Journal import Journal
 
-def get_files(journal_config):
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+
+
+def get_files(journal_config: str) -> list[str]:
     """Searches through sub directories starting with journal_config and find all text files"""
     filenames = []
     for root, dirnames, f in os.walk(journal_config):
         for filename in fnmatch.filter(f, "*.txt"):
             filenames.append(os.path.join(root, filename))
     return filenames
 
 
-class Folder(Journal.Journal):
+class Folder(Journal):
     """A Journal handling multiple files in a folder"""
 
-    def __init__(self, name="default", **kwargs):
+    def __init__(self, name: str = "default", **kwargs):
         self.entries = []
         self._diff_entry_dates = []
         self.can_be_encrypted = False
         super().__init__(name, **kwargs)
 
-    def open(self):
+    def open(self) -> "Folder":
         filenames = []
         self.entries = []
         filenames = get_files(self.config["journal"])
         for filename in filenames:
             with codecs.open(filename, "r", "utf-8") as f:
                 journal = f.read()
                 self.entries.extend(self._parse(journal))
         self.sort()
         return self
 
-    def write(self):
+    def write(self) -> None:
         """Writes only the entries that have been modified into proper files."""
         # Create a list of dates of modified entries. Start with diff_entry_dates
         modified_dates = self._diff_entry_dates
         seen_dates = set(self._diff_entry_dates)
 
         for e in self.entries:
             if e.modified:
@@ -77,36 +82,40 @@
         # look for and delete empty files
         filenames = []
         filenames = get_files(self.config["journal"])
         for filename in filenames:
             if os.stat(filename).st_size <= 0:
                 os.remove(filename)
 
-    def delete_entries(self, entries_to_delete):
+    def delete_entries(self, entries_to_delete: list["Entry"]) -> None:
         """Deletes specific entries from a journal."""
         for entry in entries_to_delete:
             self.entries.remove(entry)
             self._diff_entry_dates.append(entry.date)
+            self.deleted_entry_count += 1
 
-    def change_date_entries(self, date):
+    def change_date_entries(self, date: str, entries_to_change: list["Entry"]) -> None:
         """Changes entry dates to given date."""
 
         date = time.parse(date)
 
         self._diff_entry_dates.append(date)
 
-        for entry in self.entries:
+        for entry in entries_to_change:
             self._diff_entry_dates.append(entry.date)
             entry.date = date
+            entry.modified = True
 
-    def parse_editable_str(self, edited):
+    def parse_editable_str(self, edited: str) -> None:
         """Parses the output of self.editable_str and updates its entries."""
         mod_entries = self._parse(edited)
         diff_entries = set(self.entries) - set(mod_entries)
         for e in diff_entries:
             self._diff_entry_dates.append(e.date)
         # Match those entries that can be found in self.entries and set
         # these to modified, so we can get a count of how many entries got
         # modified and how many got deleted later.
         for entry in mod_entries:
             entry.modified = not any(entry == old_entry for old_entry in self.entries)
+
+        self.increment_change_counts_by_edit(mod_entries)
         self.entries = mod_entries
```

### Comparing `jrnl-3.3b2/jrnl/Journal.py` & `jrnl-4.0b0/jrnl/journals/Journal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import datetime
 import logging
 import os
 import re
 
-from jrnl import Entry
 from jrnl import time
 from jrnl.config import validate_journal_name
+from jrnl.encryption import determine_encryption_method
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.path import expand_path
 from jrnl.prompt import yesno
 
+from .Entry import Entry
+
 
 class Tag:
     def __init__(self, name, count=0):
         self.name = name
         self.count = count
 
     def __str__(self):
@@ -43,46 +45,67 @@
             "indent_character": "|",
         }
         self.config.update(kwargs)
         # Set up date parser
         self.search_tags = None  # Store tags we're highlighting
         self.name = name
         self.entries = []
+        self.encryption_method = None
+
+        # Track changes to journal in session. Modified is tracked in Entry
+        self.added_entry_count = 0
+        self.deleted_entry_count = 0
 
     def __len__(self):
         """Returns the number of entries"""
         return len(self.entries)
 
     def __iter__(self):
         """Iterates over the journal's entries."""
         return (entry for entry in self.entries)
 
     @classmethod
-    def from_journal(cls, other):
+    def from_journal(cls, other: "Journal") -> "Journal":
         """Creates a new journal by copying configuration and entries from
         another journal object"""
         new_journal = cls(other.name, **other.config)
         new_journal.entries = other.entries
         logging.debug(
             "Imported %d entries from %s to %s",
             len(new_journal),
             other.__class__.__name__,
             cls.__name__,
         )
         return new_journal
 
-    def import_(self, other_journal_txt):
+    def import_(self, other_journal_txt: str) -> None:
         imported_entries = self._parse(other_journal_txt)
         for entry in imported_entries:
             entry.modified = True
 
         self.entries = list(frozenset(self.entries) | frozenset(imported_entries))
         self.sort()
 
-    def open(self, filename=None):
+    def _get_encryption_method(self) -> None:
+        encryption_method = determine_encryption_method(self.config["encrypt"])
+        self.encryption_method = encryption_method(self.name, self.config)
+
+    def _decrypt(self, text: bytes) -> str:
+        if self.encryption_method is None:
+            self._get_encryption_method()
+
+        return self.encryption_method.decrypt(text)
+
+    def _encrypt(self, text: str) -> bytes:
+        if self.encryption_method is None:
+            self._get_encryption_method()
+
+        return self.encryption_method.encrypt(text)
+
+    def open(self, filename: str | None = None) -> "Journal":
         """Opens the journal file defined in the config and parses it into a list of Entries.
         Entries have the form (date, title, body)."""
         filename = filename or self.config["journal"]
         dirname = os.path.dirname(filename)
         if not os.path.exists(filename):
             if not os.path.isdir(dirname):
                 os.makedirs(dirname)
@@ -100,51 +123,52 @@
                     MsgStyle.NORMAL,
                     {
                         "journal_name": self.name,
                         "filename": filename,
                     },
                 )
             )
+            self.write()
 
         text = self._load(filename)
+        text = self._decrypt(text)
         self.entries = self._parse(text)
         self.sort()
         logging.debug("opened %s with %d entries", self.__class__.__name__, len(self))
         return self
 
-    def write(self, filename=None):
+    def write(self, filename: str | None = None) -> None:
         """Dumps the journal into the config file, overwriting it"""
         filename = filename or self.config["journal"]
         text = self._to_text()
+        text = self._encrypt(text)
         self._store(filename, text)
 
-    def validate_parsing(self):
+    def validate_parsing(self) -> bool:
         """Confirms that the jrnl is still parsed correctly after being dumped to text."""
         new_entries = self._parse(self._to_text())
-        for i, entry in enumerate(self.entries):
-            if entry != new_entries[i]:
-                return False
-        return True
+        return all(entry == new_entries[i] for i, entry in enumerate(self.entries))
 
     @staticmethod
-    def create_file(filename):
+    def create_file(filename: str) -> None:
         with open(filename, "w"):
             pass
 
-    def _to_text(self):
+    def _to_text(self) -> str:
         return "\n".join([str(e) for e in self.entries])
 
-    def _load(self, filename):
-        raise NotImplementedError
+    def _load(self, filename: str) -> bytes:
+        with open(filename, "rb") as f:
+            return f.read()
 
-    @classmethod
-    def _store(filename, text):
-        raise NotImplementedError
+    def _store(self, filename: str, text: bytes) -> None:
+        with open(filename, "wb") as f:
+            f.write(text)
 
-    def _parse(self, journal_txt):
+    def _parse(self, journal_txt: str) -> list[Entry]:
         """Parses a journal that's stored in a string and returns a list of entries"""
 
         # Return empty array if the journal is blank
         if not journal_txt:
             return []
 
         # Initialise our current entry
@@ -162,48 +186,48 @@
                 # Passing in a date that had brackets around it
                 new_date = time.parse(date_blob, bracketed=True)
 
             if new_date:
                 if entries:
                     entries[-1].text = journal_txt[last_entry_pos : match.start()]
                 last_entry_pos = match.end()
-                entries.append(Entry.Entry(self, date=new_date))
+                entries.append(Entry(self, date=new_date))
 
         # If no entries were found, treat all the existing text as an entry made now
         if not entries:
-            entries.append(Entry.Entry(self, date=time.parse("now")))
+            entries.append(Entry(self, date=time.parse("now")))
 
         # Fill in the text of the last entry
         entries[-1].text = journal_txt[last_entry_pos:]
 
         for entry in entries:
             entry._parse_text()
         return entries
 
-    def pprint(self, short=False):
+    def pprint(self, short: bool = False) -> str:
         """Prettyprints the journal's entries"""
         return "\n".join([e.pprint(short=short) for e in self.entries])
 
     def __str__(self):
         return self.pprint()
 
     def __repr__(self):
         return f"<Journal with {len(self.entries)} entries>"
 
-    def sort(self):
+    def sort(self) -> None:
         """Sorts the Journal's entries by date"""
         self.entries = sorted(self.entries, key=lambda entry: entry.date)
 
-    def limit(self, n=None):
+    def limit(self, n: int | None = None) -> None:
         """Removes all but the last n entries"""
         if n:
             self.entries = self.entries[-n:]
 
     @property
-    def tags(self):
+    def tags(self) -> list[Tag]:
         """Returns a set of tuples (count, tag) for all tags present in the journal."""
         # Astute reader: should the following line leave you as puzzled as me the first time
         # I came across this construction, worry not and embrace the ensuing moment of enlightment.
         tags = [tag for entry in self.entries for tag in set(entry.tags)]
         # To be read: [for entry in journal.entries: for tag in set(entry.tags): tag]
         tag_counts = {(tags.count(tag), tag) for tag in tags}
         return [Tag(tag, count=count) for count, tag in sorted(tag_counts)]
@@ -213,14 +237,17 @@
         tags=[],
         month=None,
         day=None,
         year=None,
         start_date=None,
         end_date=None,
         starred=False,
+        tagged=False,
+        exclude_starred=False,
+        exclude_tagged=False,
         strict=False,
         contains=None,
         exclude=[],
     ):
         """Removes all entries from the journal that don't match the filter.
 
         tags is a list of tags, each being a string that starts with one of the
@@ -236,15 +263,17 @@
         entry is kept if any tag is present, unless they appear in exclude."""
         self.search_tags = {tag.lower() for tag in tags}
         excluded_tags = {tag.lower() for tag in exclude}
         end_date = time.parse(end_date, inclusive=True)
         start_date = time.parse(start_date)
 
         # If strict mode is on, all tags have to be present in entry
-        tagged = self.search_tags.issubset if strict else self.search_tags.intersection
+        has_tags = (
+            self.search_tags.issubset if strict else self.search_tags.intersection
+        )
 
         def excluded(tags):
             return 0 < len([tag for tag in tags if tag in excluded_tags])
 
         if contains:
             contains_lower = contains.casefold()
 
@@ -252,16 +281,17 @@
         # this approach allows various formats
         if month or day or year:
             compare_d = time.parse(f"{month or 1}.{day or 1}.{year or 1}")
 
         result = [
             entry
             for entry in self.entries
-            if (not tags or tagged(entry.tags))
-            and (not starred or entry.starred)
+            if (not tags or has_tags(entry.tags))
+            and (not (starred or exclude_starred) or entry.starred == starred)
+            and (not (tagged or exclude_tagged) or bool(entry.tags) == tagged)
             and (not month or entry.date.month == compare_d.month)
             and (not day or entry.date.day == compare_d.day)
             and (not year or entry.date.year == compare_d.year)
             and (not start_date or entry.date >= start_date)
             and (not end_date or entry.date <= end_date)
             and (not exclude or not excluded(entry.tags))
             and (
@@ -271,27 +301,31 @@
                     or contains_lower in entry.body.casefold()
                 )
             )
         ]
 
         self.entries = result
 
-    def delete_entries(self, entries_to_delete):
+    def delete_entries(self, entries_to_delete: list[Entry]) -> None:
         """Deletes specific entries from a journal."""
         for entry in entries_to_delete:
             self.entries.remove(entry)
+            self.deleted_entry_count += 1
 
-    def change_date_entries(self, date):
+    def change_date_entries(
+        self, date: datetime.datetime, entries_to_change: list[Entry]
+    ) -> None:
         """Changes entry dates to given date."""
         date = time.parse(date)
 
-        for entry in self.entries:
+        for entry in entries_to_change:
             entry.date = date
+            entry.modified = True
 
-    def prompt_action_entries(self, msg: MsgText):
+    def prompt_action_entries(self, msg: MsgText) -> list[Entry]:
         """Prompts for action for each entry in a journal, using given message.
         Returns the entries the user wishes to apply the action on."""
         to_act = []
 
         def ask_action(entry):
             return yesno(
                 Message(
@@ -303,17 +337,18 @@
 
         for entry in self.entries:
             if ask_action(entry):
                 to_act.append(entry)
 
         return to_act
 
-    def new_entry(self, raw, date=None, sort=True):
+    def new_entry(self, raw: str, date=None, sort: bool = True) -> Entry:
         """Constructs a new entry from some raw text input.
-        If a date is given, it will parse and use this, otherwise scan for a date in the input first."""
+        If a date is given, it will parse and use this, otherwise scan for a date in the input first.
+        """
 
         raw = raw.replace("\\n ", "\n").replace("\\n", "\n")
         # Split raw text into title and body
         sep = re.search(r"\n|[?!.]+ +\n?", raw)
         first_line = raw[: sep.end()].strip() if sep else raw
         starred = False
 
@@ -332,57 +367,59 @@
             starred
             or first_line.startswith("*")
             or first_line.endswith("*")
             or raw.startswith("*")
         )
         if not date:  # Still nothing? Meh, just live in the moment.
             date = time.parse("now")
-        entry = Entry.Entry(self, date, raw, starred=starred)
+        entry = Entry(self, date, raw, starred=starred)
         entry.modified = True
         self.entries.append(entry)
         if sort:
             self.sort()
         return entry
 
-    def editable_str(self):
+    def editable_str(self) -> str:
         """Turns the journal into a string of entries that can be edited
-        manually and later be parsed with eslf.parse_editable_str."""
+        manually and later be parsed with self.parse_editable_str."""
         return "\n".join([str(e) for e in self.entries])
 
-    def parse_editable_str(self, edited):
+    def parse_editable_str(self, edited: str) -> None:
         """Parses the output of self.editable_str and updates it's entries."""
         mod_entries = self._parse(edited)
         # Match those entries that can be found in self.entries and set
         # these to modified, so we can get a count of how many entries got
         # modified and how many got deleted later.
         for entry in mod_entries:
             entry.modified = not any(entry == old_entry for old_entry in self.entries)
-        self.entries = mod_entries
 
+        self.increment_change_counts_by_edit(mod_entries)
 
-class PlainJournal(Journal):
-    def _load(self, filename):
-        with open(filename, "r", encoding="utf-8") as f:
-            return f.read()
+        self.entries = mod_entries
 
-    def _store(self, filename, text):
-        with open(filename, "w", encoding="utf-8") as f:
-            f.write(text)
+    def increment_change_counts_by_edit(self, mod_entries: Entry) -> None:
+        if len(mod_entries) > len(self.entries):
+            self.added_entry_count += len(mod_entries) - len(self.entries)
+        else:
+            self.deleted_entry_count += len(self.entries) - len(mod_entries)
+
+    def get_change_counts(self) -> dict:
+        return {
+            "added": self.added_entry_count,
+            "deleted": self.deleted_entry_count,
+            "modified": len([e for e in self.entries if e.modified]),
+        }
 
 
 class LegacyJournal(Journal):
     """Legacy class to support opening journals formatted with the jrnl 1.x
     standard. Main difference here is that in 1.x, timestamps were not cuddled
     by square brackets. You'll not be able to save these journals anymore."""
 
-    def _load(self, filename):
-        with open(filename, "r", encoding="utf-8") as f:
-            return f.read()
-
-    def _parse(self, journal_txt):
+    def _parse(self, journal_txt: str) -> list[Entry]:
         """Parses a journal that's stored in a string and returns a list of entries"""
         # Entries start with a line that looks like 'date title' - let's figure out how
         # long the date will be by constructing one
         date_length = len(datetime.datetime.today().strftime(self.config["timeformat"]))
 
         # Initialise our current entry
         entries = []
@@ -402,15 +439,15 @@
 
                 if line.endswith("*"):
                     starred = True
                     line = line[:-1]
                 else:
                     starred = False
 
-                current_entry = Entry.Entry(
+                current_entry = Entry(
                     self, date=new_date, text=line[date_length + 1 :], starred=starred
                 )
             except ValueError:
                 # Happens when we can't parse the start of the line as an date.
                 # In this case, just append line to our body (after some
                 # escaping for the new format).
                 line = new_date_format_regex.sub(r" \1", line)
@@ -421,20 +458,21 @@
         if current_entry:
             entries.append(current_entry)
         for entry in entries:
             entry._parse_text()
         return entries
 
 
-def open_journal(journal_name, config, legacy=False):
+def open_journal(journal_name: str, config: dict, legacy: bool = False) -> Journal:
     """
     Creates a normal, encrypted or DayOne journal based on the passed config.
     If legacy is True, it will open Journals with legacy classes build for
     backwards compatibility with jrnl 1.x
     """
+    logging.debug(f"open_journal '{journal_name}'")
     validate_journal_name(journal_name, config)
     config = config.copy()
     config["journal"] = expand_path(config["journal"])
 
     if os.path.isdir(config["journal"]):
         if config["encrypt"]:
             print_msg(
@@ -446,29 +484,28 @@
                     },
                 )
             )
 
         if config["journal"].strip("/").endswith(".dayone") or "entries" in os.listdir(
             config["journal"]
         ):
-            from jrnl import DayOneJournal
+            from jrnl.journals import DayOne
 
-            return DayOneJournal.DayOne(**config).open()
+            return DayOne(**config).open()
         else:
-            from jrnl import FolderJournal
+            from jrnl.journals import Folder
 
-            return FolderJournal.Folder(journal_name, **config).open()
+            return Folder(journal_name, **config).open()
 
     if not config["encrypt"]:
         if legacy:
             return LegacyJournal(journal_name, **config).open()
         if config["journal"].endswith(os.sep):
-            from jrnl import FolderJournal
-
-            return FolderJournal.Folder(journal_name, **config).open()
-        return PlainJournal(journal_name, **config).open()
+            from jrnl.journals import Folder
 
-    from jrnl import EncryptedJournal
+            return Folder(journal_name, **config).open()
+        return Journal(journal_name, **config).open()
 
     if legacy:
-        return EncryptedJournal.LegacyEncryptedJournal(journal_name, **config).open()
-    return EncryptedJournal.EncryptedJournal(journal_name, **config).open()
+        config["encrypt"] = "jrnlv1"
+        return LegacyJournal(journal_name, **config).open()
+    return Journal(journal_name, **config).open()
```

### Comparing `jrnl-3.3b2/jrnl/args.py` & `jrnl-4.0b0/jrnl/args.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import argparse
 import re
 import textwrap
 
 from jrnl.commands import postconfig_decrypt
@@ -16,23 +16,60 @@
 from jrnl.plugins import IMPORT_FORMATS
 from jrnl.plugins import util
 
 
 class WrappingFormatter(argparse.RawTextHelpFormatter):
     """Used in help screen"""
 
-    def _split_lines(self, text, width):
+    def _split_lines(self, text: str, width: int) -> list[str]:
         text = text.split("\n\n")
         text = map(lambda t: self._whitespace_matcher.sub(" ", t).strip(), text)
         text = map(lambda t: textwrap.wrap(t, width=56), text)
         text = [item for sublist in text for item in sublist]
         return text
 
 
-def parse_args(args=[]):
+class IgnoreNoneAppendAction(argparse._AppendAction):
+    """
+    Pass -not without a following string and avoid appending
+    a None value to the excluded list
+    """
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        if values is not None:
+            super().__call__(parser, namespace, values, option_string)
+
+
+def parse_not_arg(
+    args: list[str], parsed_args: argparse.Namespace, parser: argparse.ArgumentParser
+) -> argparse.Namespace:
+    """
+    It's possible to use -not as a precursor to -starred and -tagged
+    to reverse their behaviour, however this requires some extra logic
+    to parse, and to ensure we still do not allow passing an empty -not
+    """
+
+    parsed_args.exclude_starred = False
+    parsed_args.exclude_tagged = False
+
+    if "-not-starred" in "".join(args):
+        parsed_args.starred = False
+        parsed_args.exclude_starred = True
+    if "-not-tagged" in "".join(args):
+        parsed_args.tagged = False
+        parsed_args.exclude_tagged = True
+    if "-not" in args and not any(
+        [parsed_args.exclude_starred, parsed_args.exclude_tagged, parsed_args.excluded]
+    ):
+        parser.error("argument -not: expected 1 argument")
+
+    return parsed_args
+
+
+def parse_args(args: list[str] = []) -> argparse.Namespace:
     """
     Argument parsing that is doable before the config is available.
     Everything else goes into "text" for later parsing.
     """
     parser = argparse.ArgumentParser(
         formatter_class=WrappingFormatter,
         add_help=False,
@@ -170,14 +207,19 @@
 
         jrnl "saturday at 2am: *Then I was like 'That log had a child!'" """
 
     composing = parser.add_argument_group(
         "Writing", textwrap.dedent(compose_msg).strip()
     )
     composing.add_argument("text", metavar="", nargs="*")
+    composing.add_argument(
+        "--template",
+        dest="template",
+        help="Path to template file. Can be a local path, absolute path, or a path relative to $XDG_DATA_HOME/jrnl/templates/",
+    )
 
     read_msg = (
         "To find entries from your journal, use any combination of the below filters."
     )
     reading = parser.add_argument_group("Searching", textwrap.dedent(read_msg))
     reading.add_argument(
         "-on", dest="on_date", metavar="DATE", help="Show entries on this date"
@@ -234,30 +276,40 @@
     reading.add_argument(
         "-starred",
         dest="starred",
         action="store_true",
         help="Show only starred entries (marked with *)",
     )
     reading.add_argument(
+        "-tagged",
+        dest="tagged",
+        action="store_true",
+        help="Show only entries that have at least one tag",
+    )
+    reading.add_argument(
         "-n",
         dest="limit",
         default=None,
         metavar="NUMBER",
         help="Show a maximum of NUMBER entries (note: '-n 3' and '-3' have the same effect)",
         nargs="?",
         type=int,
     )
     reading.add_argument(
         "-not",
         dest="excluded",
-        nargs=1,
+        nargs="?",
         default=[],
-        metavar="TAG",
-        action="extend",
-        help="Exclude entries with this tag",
+        metavar="TAG/FLAG",
+        action=IgnoreNoneAppendAction,
+        help=(
+            "If passed a string, will exclude entries with that tag. "
+            "Can be also used before -starred or -tagged flags, to exclude "
+            "starred or tagged entries respectively."
+        ),
     )
 
     search_options_msg = """    These help you do various tasks with the selected entries from your search.
     If used on their own (with no search), they will act on your entire journal"""
     exporting = parser.add_argument_group(
         "Searching Options", textwrap.dedent(search_options_msg)
     )
@@ -368,15 +420,15 @@
     alternate_config.add_argument(
         "--config-file",
         dest="config_file_path",
         type=str,
         default="",
         help="""
         Overrides default (created when first installed) config file for this command only.
-        
+
         Examples: \n
         \t - Use a work config file for this jrnl entry, call: \n
             \t jrnl --config-file /home/user1/work_config.yaml
         \t - Use a personal config file stored on a thumb drive: \n
             \t jrnl --config-file /media/user1/my-thumb-drive/personal_config.yaml
         """,
     )
@@ -384,9 +436,11 @@
     alternate_config.add_argument(
         "--cf", dest="config_file_path", type=str, default="", help=argparse.SUPPRESS
     )
 
     # Handle '-123' as a shortcut for '-n 123'
     num = re.compile(r"^-(\d+)$")
     args = [num.sub(r"-n \1", arg) for arg in args]
+    parsed_args = parser.parse_intermixed_args(args)
+    parsed_args = parse_not_arg(args, parsed_args, parser)
 
-    return parser.parse_intermixed_args(args)
+    return parsed_args
```

### Comparing `jrnl-3.3b2/jrnl/cli.py` & `jrnl-4.0b0/jrnl/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import logging
 import sys
 import traceback
 
+from rich.logging import RichHandler
+
+from jrnl import controller
 from jrnl.args import parse_args
 from jrnl.exception import JrnlException
-from jrnl.jrnl import run
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 
 
-def configure_logger(debug=False):
+def configure_logger(debug: bool = False) -> None:
     if not debug:
         logging.disable()
         return
 
     logging.basicConfig(
         level=logging.DEBUG,
-        format="%(levelname)-8s %(name)-12s %(message)s",
+        datefmt="[%X]",
+        format="%(message)s",
+        handlers=[RichHandler()],
     )
     logging.getLogger("parsedatetime").setLevel(logging.INFO)
     logging.getLogger("keyring.backend").setLevel(logging.ERROR)
+    logging.debug("Logging start")
 
 
-def cli(manual_args=None):
+def run(manual_args: list[str] | None = None) -> int:
     try:
         if manual_args is None:
             manual_args = sys.argv[1:]
 
         args = parse_args(manual_args)
         configure_logger(args.debug)
-        logging.debug("Parsed args: %s", args)
+        logging.debug("Parsed args:\n%s", args)
 
-        status_code = run(args)
+        status_code = controller.run(args)
 
     except JrnlException as e:
         status_code = 1
         e.print()
 
     except KeyboardInterrupt:
         status_code = 1
```

### Comparing `jrnl-3.3b2/jrnl/color.py` & `jrnl-4.0b0/jrnl/color.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import re
 from string import punctuation
 from string import whitespace
+from typing import TYPE_CHECKING
 
 import colorama
 
 from jrnl.os_compat import on_windows
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+
 if on_windows():
     colorama.init()
 
 
-def colorize(string, color, bold=False):
+def colorize(string: str, color: str, bold: bool = False) -> str:
     """Returns the string colored with colorama.Fore.color. If the color set by
     the user is "NONE" or the color doesn't exist in the colorama.Fore attributes,
     it returns the string without any modification."""
     color_escape = getattr(colorama.Fore, color.upper(), None)
     if not color_escape:
         return string
     elif not bold:
         return color_escape + string + colorama.Fore.RESET
     else:
         return colorama.Style.BRIGHT + color_escape + string + colorama.Style.RESET_ALL
 
 
-def highlight_tags_with_background_color(entry, text, color, is_title=False):
+def highlight_tags_with_background_color(
+    entry: "Entry", text: str, color: str, is_title: bool = False
+) -> str:
     """
     Takes a string and colorizes the tags in it based upon the config value for
     color.tags, while colorizing the rest of the text based on `color`.
     :param entry: Entry object, for access to journal config
     :param text: Text to be colorized
     :param color: Color for non-tag text, passed to colorize()
     :param is_title: Boolean flag indicating if the text is a title or not
@@ -41,17 +47,17 @@
         """Efficiently generate colorized tags / text from text fragments.
         Taken from @shobrook. Thanks, buddy :)
         :param fragments: List of strings representing parts of entry (tag or word).
         :rtype: List of tuples
         :returns [(colorized_str, original_str)]"""
         for part in fragments:
             if part and part[0] not in config["tagsymbols"]:
-                yield (colorize(part, color, bold=is_title), part)
+                yield colorize(part, color, bold=is_title), part
             elif part:
-                yield (colorize(part, config["colors"]["tags"], bold=True), part)
+                yield colorize(part, config["colors"]["tags"], bold=True), part
 
     config = entry.journal.config
     if config["highlight"]:  # highlight tags
         text_fragments = re.split(entry.tag_regex(config["tagsymbols"]), text)
 
         # Colorizing tags inside of other blocks of text
         final_text = ""
```

### Comparing `jrnl-3.3b2/jrnl/commands.py` & `jrnl-4.0b0/jrnl/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 """
 Functions in this file are standalone commands. All standalone commands are split into
 two categories depending on whether they require the config to be loaded to be able to
 run.
 
@@ -10,48 +10,49 @@
    config has been loaded.
 2. "postconfig" commands require to config to have already been loaded, parsed, and
    scoped before they can be run.
 
 Also, please note that all (non-builtin) imports should be scoped to each function to
 avoid any possible overhead for these standalone commands.
 """
+
 import argparse
+import logging
 import platform
 import sys
 
 from jrnl.config import cmd_requires_valid_journal_name
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
-from jrnl.prompt import create_password
 
 
-def preconfig_diagnostic(_):
+def preconfig_diagnostic(_) -> None:
     from jrnl import __title__
     from jrnl import __version__
 
     print(
         f"{__title__}: {__version__}\n"
         f"Python: {sys.version}\n"
         f"OS: {platform.system()} {platform.release()}"
     )
 
 
-def preconfig_version(_):
+def preconfig_version(_) -> None:
     import textwrap
 
     from jrnl import __title__
     from jrnl import __version__
 
     output = f"""
     {__title__} {__version__}
 
-    Copyright © 2012-2022 jrnl contributors
+    Copyright © 2012-2023 jrnl contributors
 
     This is free software, and you are welcome to redistribute it under certain
     conditions; for details, see: https://www.gnu.org/licenses/gpl-3.0.html
     """
 
     output = textwrap.dedent(output).strip()
 
@@ -64,15 +65,15 @@
     print(list_journals(config, args.export))
 
     return 0
 
 
 @cmd_requires_valid_journal_name
 def postconfig_import(args: argparse.Namespace, config: dict, **_) -> int:
-    from jrnl.Journal import open_journal
+    from jrnl.journals import open_journal
     from jrnl.plugins import get_importer
 
     # Requires opening the journal
     journal = open_journal(args.journal_name, config)
 
     format = args.export if args.export else "jrnl"
     get_importer(format).import_(journal, args.filename)
@@ -84,17 +85,16 @@
 def postconfig_encrypt(
     args: argparse.Namespace, config: dict, original_config: dict
 ) -> int:
     """
     Encrypt a journal in place, or optionally to a new file
     """
     from jrnl.config import update_config
-    from jrnl.EncryptedJournal import EncryptedJournal
     from jrnl.install import save_config
-    from jrnl.Journal import open_journal
+    from jrnl.journals import open_journal
 
     # Open the journal
     journal = open_journal(args.journal_name, config)
 
     if hasattr(journal, "can_be_encrypted") and not journal.can_be_encrypted:
         raise JrnlException(
             Message(
@@ -103,29 +103,32 @@
                 {
                     "journal_name": args.journal_name,
                     "journal_type": journal.__class__.__name__,
                 },
             )
         )
 
-    new_journal = EncryptedJournal.from_journal(journal)
-
     # If journal is encrypted, create new password
+    logging.debug("Clearing encryption method...")
+
     if journal.config["encrypt"] is True:
+        logging.debug("Journal already encrypted. Re-encrypting...")
         print(f"Journal {journal.name} is already encrypted. Create a new password.")
-        new_journal.password = create_password(new_journal.name)
+        journal.encryption_method.clear()
+    else:
+        journal.config["encrypt"] = True
+        journal.encryption_method = None
 
-    journal.config["encrypt"] = True
-    new_journal.write(args.filename)
+    journal.write(args.filename)
 
     print_msg(
         Message(
             MsgText.JournalEncryptedTo,
             MsgStyle.NORMAL,
-            {"path": args.filename or new_journal.config["journal"]},
+            {"path": args.filename or journal.config["journal"]},
         )
     )
 
     # Update the config, if we encrypted in place
     if not args.filename:
         update_config(
             original_config, {"encrypt": True}, args.journal_name, force_local=True
@@ -138,27 +141,28 @@
 @cmd_requires_valid_journal_name
 def postconfig_decrypt(
     args: argparse.Namespace, config: dict, original_config: dict
 ) -> int:
     """Decrypts into new file. If filename is not set, we encrypt the journal file itself."""
     from jrnl.config import update_config
     from jrnl.install import save_config
-    from jrnl.Journal import PlainJournal
-    from jrnl.Journal import open_journal
+    from jrnl.journals import open_journal
 
     journal = open_journal(args.journal_name, config)
+
+    logging.debug("Clearing encryption method...")
     journal.config["encrypt"] = False
+    journal.encryption_method = None
 
-    new_journal = PlainJournal.from_journal(journal)
-    new_journal.write(args.filename)
+    journal.write(args.filename)
     print_msg(
         Message(
             MsgText.JournalDecryptedTo,
             MsgStyle.NORMAL,
-            {"path": args.filename or new_journal.config["journal"]},
+            {"path": args.filename or journal.config["journal"]},
         )
     )
 
     # Update the config, if we decrypted in place
     if not args.filename:
         update_config(
             original_config, {"encrypt": False}, args.journal_name, force_local=True
```

### Comparing `jrnl-3.3b2/jrnl/config.py` & `jrnl-4.0b0/jrnl/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import argparse
 import logging
 import os
+from pathlib import Path
+from typing import Any
 from typing import Callable
 
 import colorama
 import xdg.BaseDirectory
+from rich.pretty import pretty_repr
 from ruamel.yaml import YAML
 from ruamel.yaml import constructor
 
 from jrnl import __version__
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
@@ -28,15 +31,14 @@
 DEFAULT_JOURNAL_KEY = "default"
 
 YAML_SEPARATOR = ": "
 YAML_FILE_ENCODING = "utf-8"
 
 
 def make_yaml_valid_dict(input: list) -> dict:
-
     """
 
     Convert a two-element list of configuration key-value pair into a flat dict.
 
     The dict is created through the yaml loader, with the assumption that
     "input[0]: input[1]" is valid yaml.
 
@@ -52,94 +54,121 @@
     yamlstr = YAML_SEPARATOR.join(input)
 
     runtime_modifications = YAML(typ="safe").load(yamlstr)
 
     return runtime_modifications
 
 
-def save_config(config, alt_config_path=None):
+def save_config(config: dict, alt_config_path: str | None = None) -> None:
     """Supply alt_config_path if using an alternate config through --config-file."""
     config["version"] = __version__
 
     yaml = YAML(typ="safe")
     yaml.default_flow_style = False  # prevents collapsing of tree structure
 
     with open(
         alt_config_path if alt_config_path else get_config_path(),
         "w",
         encoding=YAML_FILE_ENCODING,
     ) as f:
         yaml.dump(config, f)
 
 
-def get_config_path():
+def get_config_directory() -> str:
     try:
-        config_directory_path = xdg.BaseDirectory.save_config_path(XDG_RESOURCE)
+        return xdg.BaseDirectory.save_config_path(XDG_RESOURCE)
     except FileExistsError:
         raise JrnlException(
             Message(
                 MsgText.ConfigDirectoryIsFile,
                 MsgStyle.ERROR,
                 {
                     "config_directory_path": os.path.join(
                         xdg.BaseDirectory.xdg_config_home, XDG_RESOURCE
                     )
                 },
             ),
         )
 
-    return os.path.join(config_directory_path or home_dir(), DEFAULT_CONFIG_NAME)
+
+def get_config_path() -> Path:
+    try:
+        config_directory_path = get_config_directory()
+    except JrnlException:
+        return Path(home_dir(), DEFAULT_CONFIG_NAME)
+    return Path(config_directory_path, DEFAULT_CONFIG_NAME)
 
 
-def get_default_config():
+def get_default_config() -> dict[str, Any]:
     return {
         "version": __version__,
         "journals": {"default": {"journal": get_default_journal_path()}},
         "editor": os.getenv("VISUAL") or os.getenv("EDITOR") or "",
         "encrypt": False,
         "template": False,
         "default_hour": 9,
         "default_minute": 0,
         "timeformat": "%F %r",
         "tagsymbols": "#@",
         "highlight": True,
         "linewrap": 79,
         "indent_character": "|",
         "colors": {
-            "date": "none",
-            "title": "none",
             "body": "none",
+            "date": "none",
             "tags": "none",
+            "title": "none",
         },
     }
 
 
-def get_default_journal_path():
+def get_default_colors() -> dict[str, Any]:
+    return {
+        "body": "none",
+        "date": "black",
+        "tags": "yellow",
+        "title": "cyan",
+    }
+
+
+def get_default_journal_path() -> str:
     journal_data_path = xdg.BaseDirectory.save_data_path(XDG_RESOURCE) or home_dir()
     return os.path.join(journal_data_path, DEFAULT_JOURNAL_NAME)
 
 
-def scope_config(config, journal_name):
+def get_templates_path() -> Path:
+    # jrnl_xdg_resource_path is created by save_data_path if it does not exist
+    jrnl_xdg_resource_path = Path(xdg.BaseDirectory.save_data_path(XDG_RESOURCE))
+    jrnl_templates_path = jrnl_xdg_resource_path / "templates"
+    # Create the directory if needed.
+    jrnl_templates_path.mkdir(exist_ok=True)
+    return jrnl_templates_path
+
+
+def scope_config(config: dict, journal_name: str) -> dict:
     if journal_name not in config["journals"]:
         return config
     config = config.copy()
     journal_conf = config["journals"].get(journal_name)
     if type(journal_conf) is dict:
         # We can override the default config on a by-journal basis
         logging.debug(
-            "Updating configuration with specific journal overrides %s", journal_conf
+            "Updating configuration with specific journal overrides:\n%s",
+            pretty_repr(journal_conf),
         )
         config.update(journal_conf)
     else:
         # But also just give them a string to point to the journal file
         config["journal"] = journal_conf
+
+    logging.debug("Scoped config:\n%s", pretty_repr(config))
     return config
 
 
-def verify_config_colors(config):
+def verify_config_colors(config: dict) -> bool:
     """
     Ensures the keys set for colors are valid colorama.Fore attributes, or "None"
     :return: True if all keys are set correctly, False otherwise
     """
     all_valid_colors = True
     for key, color in config["colors"].items():
         upper_color = color.upper()
@@ -156,15 +185,15 @@
                     },
                 )
             )
             all_valid_colors = False
     return all_valid_colors
 
 
-def load_config(config_path):
+def load_config(config_path: str) -> dict:
     """Tries to load a config file from YAML."""
     try:
         with open(config_path, encoding=YAML_FILE_ENCODING) as f:
             yaml = YAML(typ="safe")
             yaml.allow_duplicate_keys = False
             return yaml.load(f)
     except constructor.DuplicateKeyError as e:
@@ -179,34 +208,36 @@
         )
         with open(config_path, encoding=YAML_FILE_ENCODING) as f:
             yaml = YAML(typ="safe")
             yaml.allow_duplicate_keys = True
             return yaml.load(f)
 
 
-def is_config_json(config_path):
+def is_config_json(config_path: str) -> bool:
     with open(config_path, "r", encoding="utf-8") as f:
         config_file = f.read()
     return config_file.strip().startswith("{")
 
 
-def update_config(config, new_config, scope, force_local=False):
+def update_config(
+    config: dict, new_config: dict, scope: str | None, force_local: bool = False
+) -> None:
     """Updates a config dict with new values - either global if scope is None
     or config['journals'][scope] is just a string pointing to a journal file,
     or within the scope"""
     if scope and type(config["journals"][scope]) is dict:  # Update to journal specific
         config["journals"][scope].update(new_config)
     elif scope and force_local:  # Convert to dict
         config["journals"][scope] = {"journal": config["journals"][scope]}
         config["journals"][scope].update(new_config)
     else:
         config.update(new_config)
 
 
-def get_journal_name(args, config):
+def get_journal_name(args: argparse.Namespace, config: dict) -> argparse.Namespace:
     args.journal_name = DEFAULT_JOURNAL_KEY
 
     # The first arg might be a journal name
     if args.text:
         potential_journal_name = args.text[0]
         if potential_journal_name[-1] == ":":
             potential_journal_name = potential_journal_name[0:-1]
```

### Comparing `jrnl-3.3b2/jrnl/editor.py` & `jrnl-4.0b0/jrnl/editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import logging
 import os
 import subprocess
 import sys
 import tempfile
@@ -13,15 +13,15 @@
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.os_compat import on_windows
 from jrnl.os_compat import split_args
 from jrnl.output import print_msg
 
 
-def get_text_from_editor(config, template=""):
+def get_text_from_editor(config: dict, template: str = "") -> str:
     suffix = ".jrnl"
     if config["template"]:
         template_filename = Path(config["template"]).name
         suffix = "-" + template_filename
     filehandle, tmpfile = tempfile.mkstemp(prefix="jrnl", text=True, suffix=suffix)
     os.close(filehandle)
 
@@ -46,15 +46,15 @@
 
     if not raw:
         raise JrnlException(Message(MsgText.NoTextReceived, MsgStyle.NORMAL))
 
     return raw
 
 
-def get_text_from_stdin():
+def get_text_from_stdin() -> str:
     print_msg(
         Message(
             MsgText.WritingEntryStart,
             MsgStyle.TITLE,
             {
                 "how_to_quit": MsgText.HowToQuitWindows
                 if on_windows()
@@ -62,14 +62,14 @@
             },
         )
     )
 
     try:
         raw = sys.stdin.read()
     except KeyboardInterrupt:
-        logging.error("Write mode: keyboard interrupt")
+        logging.error("Append mode: keyboard interrupt")
         raise JrnlException(
             Message(MsgText.KeyboardInterruptMsg, MsgStyle.ERROR_ON_NEW_LINE),
             Message(MsgText.JournalNotSaved, MsgStyle.WARNING),
         )
 
     return raw
```

### Comparing `jrnl-3.3b2/jrnl/install.py` & `jrnl-4.0b0/jrnl/install.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+import contextlib
 import glob
 import logging
 import os
 import sys
 
+from rich.pretty import pretty_repr
+
+from jrnl import __version__
 from jrnl.config import DEFAULT_JOURNAL_KEY
 from jrnl.config import get_config_path
+from jrnl.config import get_default_colors
 from jrnl.config import get_default_config
 from jrnl.config import get_default_journal_path
 from jrnl.config import load_config
 from jrnl.config import save_config
 from jrnl.config import verify_config_colors
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
@@ -21,54 +26,62 @@
 from jrnl.path import absolute_path
 from jrnl.path import expand_path
 from jrnl.path import home_dir
 from jrnl.prompt import yesno
 from jrnl.upgrade import is_old_version
 
 
-def upgrade_config(config_data, alt_config_path=None):
+def upgrade_config(config_data: dict, alt_config_path: str | None = None) -> None:
     """Checks if there are keys missing in a given config dict, and if so, updates the config file accordingly.
     This essentially automatically ports jrnl installations if new config parameters are introduced in later
     versions.
+    Also checks for existence of and difference in version number between config dict and current jrnl version,
+    and if so, update the config file accordingly.
     Supply alt_config_path if using an alternate config through --config-file."""
     default_config = get_default_config()
     missing_keys = set(default_config).difference(config_data)
     if missing_keys:
         for key in missing_keys:
             config_data[key] = default_config[key]
+
+    different_version = config_data["version"] != __version__
+    if different_version:
+        config_data["version"] = __version__
+
+    if missing_keys or different_version:
         save_config(config_data, alt_config_path)
         config_path = alt_config_path if alt_config_path else get_config_path()
         print_msg(
             Message(
                 MsgText.ConfigUpdated, MsgStyle.NORMAL, {"config_path": config_path}
             )
         )
 
 
-def find_default_config():
+def find_default_config() -> str:
     config_path = (
         get_config_path()
         if os.path.exists(get_config_path())
         else os.path.join(home_dir(), ".jrnl_config")
     )
     return config_path
 
 
-def find_alt_config(alt_config):
+def find_alt_config(alt_config: str) -> str:
     if not os.path.exists(alt_config):
         raise JrnlException(
             Message(
                 MsgText.AltConfigNotFound, MsgStyle.ERROR, {"config_file": alt_config}
             )
         )
 
     return alt_config
 
 
-def load_or_install_jrnl(alt_config_path):
+def load_or_install_jrnl(alt_config_path: str) -> dict:
     """
     If jrnl is already installed, loads and returns a default config object.
     If alternate config is specified via --config-file flag, it will be used.
     Else, perform various prompts to install jrnl.
     """
     config_path = (
         find_alt_config(alt_config_path) if alt_config_path else find_default_config()
@@ -97,19 +110,19 @@
         upgrade_config(config, alt_config_path)
         verify_config_colors(config)
 
     else:
         logging.debug("Configuration file not found, installing jrnl...")
         config = install()
 
-    logging.debug('Using configuration "%s"', config)
+    logging.debug('Using configuration:\n"%s"', pretty_repr(config))
     return config
 
 
-def install():
+def install() -> dict:
     _initialize_autocomplete()
 
     # Where to create the journal?
     default_journal_path = get_default_journal_path()
     user_given_path = print_msg(
         Message(
             MsgText.InstallJournalPathQuestion,
@@ -122,37 +135,49 @@
     )
     journal_path = absolute_path(user_given_path or default_journal_path)
     default_config = get_default_config()
     default_config["journals"][DEFAULT_JOURNAL_KEY]["journal"] = journal_path
 
     # If the folder doesn't exist, create it
     path = os.path.split(journal_path)[0]
-    try:
+    with contextlib.suppress(OSError):
         os.makedirs(path)
-    except OSError:
-        pass
 
     # Encrypt it?
     encrypt = yesno(Message(MsgText.EncryptJournalQuestion), default=False)
     if encrypt:
         default_config["encrypt"] = True
         print_msg(Message(MsgText.JournalEncrypted, MsgStyle.NORMAL))
 
+    # Use colors?
+    use_colors = yesno(Message(MsgText.UseColorsQuestion), default=True)
+    if use_colors:
+        default_config["colors"] = get_default_colors()
+
     save_config(default_config)
+
+    print_msg(
+        Message(
+            MsgText.InstallComplete,
+            MsgStyle.NORMAL,
+            params={"config_path": get_config_path()},
+        )
+    )
+
     return default_config
 
 
-def _initialize_autocomplete():
+def _initialize_autocomplete() -> None:
     # readline is not included in Windows Active Python and perhaps some other distributions
     if sys.modules.get("readline"):
         import readline
 
         readline.set_completer_delims(" \t\n;")
         readline.parse_and_bind("tab: complete")
         readline.set_completer(_autocomplete_path)
 
 
-def _autocomplete_path(text, state):
+def _autocomplete_path(text: str, state: int) -> list[str | None]:
     expansions = glob.glob(expand_path(text) + "*")
     expansions = [e + "/" if os.path.isdir(e) else e for e in expansions]
     expansions.append(None)
     return expansions[state]
```

### Comparing `jrnl-3.3b2/jrnl/jrnl.py` & `jrnl-4.0b0/jrnl/controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import logging
 import sys
+from typing import TYPE_CHECKING
 
 from jrnl import install
 from jrnl import plugins
 from jrnl import time
 from jrnl.config import DEFAULT_JOURNAL_KEY
 from jrnl.config import get_config_path
 from jrnl.config import get_journal_name
+from jrnl.config import get_templates_path
 from jrnl.config import scope_config
 from jrnl.editor import get_text_from_editor
 from jrnl.editor import get_text_from_stdin
 from jrnl.exception import JrnlException
-from jrnl.Journal import open_journal
+from jrnl.journals import open_journal
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.output import print_msgs
 from jrnl.override import apply_overrides
-from jrnl.path import expand_path
+from jrnl.path import absolute_path
 
+if TYPE_CHECKING:
+    from argparse import Namespace
 
-def run(args):
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
+
+def run(args: "Namespace"):
     """
     Flow:
     1. Run standalone command if it doesn't require config (help, version, etc), then exit
     2. Load config
     3. Run standalone command if it does require config (encrypt, decrypt, etc), then exit
     4. Load specified journal
-    5. Start write mode, or search mode
-    6. Profit
+    5. Start append mode, or search mode
+    6. Perform actions with results from search mode (if needed)
+    7. Profit
     """
 
     # Run command if possible before config is available
     if callable(args.preconfig_cmd):
         return args.preconfig_cmd(args)
 
     # Load the config, and extract journal name
@@ -60,222 +69,219 @@
     # Get the journal we're going to be working with
     journal = open_journal(args.journal_name, config)
 
     kwargs = {
         "args": args,
         "config": config,
         "journal": journal,
+        "old_entries": journal.entries,
     }
 
-    if _is_write_mode(**kwargs):
-        write_mode(**kwargs)
+    if _is_append_mode(**kwargs):
+        append_mode(**kwargs)
+        return
+
+    # If not append mode, then we're in search mode (only 2 modes exist)
+    search_mode(**kwargs)
+    entries_found_count = len(journal)
+    _print_entries_found_count(entries_found_count, args)
+
+    # Actions
+    _perform_actions_on_search_results(**kwargs)
+
+    if entries_found_count != 0 and _has_action_args(args):
+        _print_changed_counts(journal)
     else:
-        search_mode(**kwargs)
+        # display only occurs if no other action occurs
+        _display_search_results(**kwargs)
 
 
-def _is_write_mode(args, config, **kwargs):
-    """Determines if we are in write mode (as opposed to search mode)"""
-    write_mode = True
+def _perform_actions_on_search_results(**kwargs):
+    args = kwargs["args"]
+
+    # Perform actions (if needed)
+    if args.change_time:
+        _change_time_search_results(**kwargs)
 
+    if args.delete:
+        _delete_search_results(**kwargs)
+
+    # open results in editor (if `--edit` was used)
+    if args.edit:
+        _edit_search_results(**kwargs)
+
+
+def _is_append_mode(args: "Namespace", config: dict, **kwargs) -> bool:
+    """Determines if we are in append mode (as opposed to search mode)"""
     # Are any search filters present? If so, then search mode.
-    write_mode = not any(
-        (
-            args.contains,
-            args.delete,
-            args.edit,
-            args.change_time,
-            args.excluded,
-            args.export,
-            args.end_date,
-            args.today_in_history,
-            args.month,
-            args.day,
-            args.year,
-            args.limit,
-            args.on_date,
-            args.short,
-            args.starred,
-            args.start_date,
-            args.strict,
-            args.tags,
-        )
+    append_mode = (
+        not _has_search_args(args)
+        and not _has_action_args(args)
+        and not _has_display_args(args)
     )
 
     # Might be writing and want to move to editor part of the way through
     if args.edit and args.text:
-        write_mode = True
+        append_mode = True
 
     # If the text is entirely tags, then we are also searching (not writing)
-    if (
-        write_mode
-        and args.text
-        and all(word[0] in config["tagsymbols"] for word in " ".join(args.text).split())
-    ):
-        write_mode = False
+    if append_mode and args.text and _has_only_tags(config["tagsymbols"], args.text):
+        append_mode = False
+
+    return append_mode
+
+
+def _read_template_file(template_arg: str, template_path_from_config: str) -> str:
+    """
+    This function is called when either a template file is passed with --template, or config.template is set.
 
-    return write_mode
+    The processing logic is:
+        If --template was not used: Load the global template file.
+        If --template was used:
+            * Check $XDG_DATA_HOME/jrnl/templates/template_arg.
+            * Check template_arg as an absolute / relative path.
 
+        If a file is found, its contents are returned as a string.
+        If not, a JrnlException is raised.
+    """
+    logging.debug(
+        "Append mode: Either a template arg was passed, or the global config is set."
+    )
+
+    # If filename is unset, we are in this flow due to a global template being configured
+    if not template_arg:
+        logging.debug("Append mode: Global template configuration detected.")
+        global_template_path = absolute_path(template_path_from_config)
+        try:
+            with open(global_template_path, encoding="utf-8") as f:
+                template_data = f.read()
+                return template_data
+        except FileNotFoundError:
+            raise JrnlException(
+                Message(
+                    MsgText.CantReadTemplateGlobalConfig,
+                    MsgStyle.ERROR,
+                    {
+                        "global_template_path": global_template_path,
+                    },
+                )
+            )
+    else:  # A template CLI arg was passed.
+        logging.debug("Trying to load template from $XDG_DATA_HOME/jrnl/templates/")
+        jrnl_template_dir = get_templates_path()
+        logging.debug(f"Append mode: jrnl templates directory: {jrnl_template_dir}")
+        template_path = jrnl_template_dir / template_arg
+        try:
+            with open(template_path, encoding="utf-8") as f:
+                template_data = f.read()
+                return template_data
+        except FileNotFoundError:
+            logging.debug(
+                f"Couldn't open {template_path}. Treating --template argument like a local / abs path."
+            )
+            pass
+
+        normalized_template_arg_filepath = absolute_path(template_arg)
+        try:
+            with open(normalized_template_arg_filepath, encoding="utf-8") as f:
+                template_data = f.read()
+                return template_data
+        except FileNotFoundError:
+            raise JrnlException(
+                Message(
+                    MsgText.CantReadTemplateCLIArg,
+                    MsgStyle.ERROR,
+                    {
+                        "normalized_template_arg_filepath": normalized_template_arg_filepath,
+                        "jrnl_template_dir": template_path,
+                    },
+                )
+            )
 
-def write_mode(args, config, journal, **kwargs):
+
+def append_mode(args: "Namespace", config: dict, journal: "Journal", **kwargs) -> None:
     """
     Gets input from the user to write to the journal
+    0. Check for a template passed as an argument, or in the global config
     1. Check for input from cli
     2. Check input being piped in
     3. Open editor if configured (prepopulated with template if available)
     4. Use stdin.read as last resort
     6. Write any found text to journal, or exit
     """
-    logging.debug("Write mode: starting")
+    logging.debug("Append mode: starting")
 
-    if args.text:
-        logging.debug("Write mode: cli text detected: %s", args.text)
+    if args.template or config["template"]:
+        logging.debug(f"Append mode: template CLI arg detected: {args.template}")
+        # Read template file and pass as raw text into the composer
+        template_data = _read_template_file(args.template, config["template"])
+        raw = _write_in_editor(config, template_data)
+        if raw == template_data:
+            logging.error("Append mode: raw text was the same as the template")
+            raise JrnlException(Message(MsgText.NoChangesToTemplate, MsgStyle.NORMAL))
+    elif args.text:
+        logging.debug(f"Append mode: cli text detected: {args.text}")
         raw = " ".join(args.text).strip()
         if args.edit:
             raw = _write_in_editor(config, raw)
 
     elif not sys.stdin.isatty():
-        logging.debug("Write mode: receiving piped text")
+        logging.debug("Append mode: receiving piped text")
         raw = sys.stdin.read()
 
     else:
         raw = _write_in_editor(config)
 
     if not raw or raw.isspace():
-        logging.error("Write mode: couldn't get raw text or entry was empty")
+        logging.error("Append mode: couldn't get raw text or entry was empty")
         raise JrnlException(Message(MsgText.NoTextReceived, MsgStyle.NORMAL))
 
     logging.debug(
-        'Write mode: appending raw text to journal "%s": %s', args.journal_name, raw
+        f"Append mode: appending raw text to journal '{args.journal_name}': {raw}"
     )
     journal.new_entry(raw)
     if args.journal_name != DEFAULT_JOURNAL_KEY:
         print_msg(
             Message(
                 MsgText.JournalEntryAdded,
                 MsgStyle.NORMAL,
                 {"journal_name": args.journal_name},
             )
         )
     journal.write()
-    logging.debug("Write mode: completed journal.write()")
+    logging.debug("Append mode: completed journal.write()")
 
 
-def search_mode(args, journal, **kwargs):
+def search_mode(args: "Namespace", journal: "Journal", **kwargs) -> None:
     """
-    Search for entries in a journal, then either:
-    1. Send them to configured editor for user manipulation (and also
-       change their timestamps if requested)
-    2. Change their timestamps
-    2. Delete them (with confirmation for each entry)
-    3. Display them (with formatting options)
+    Search for entries in a journal, and return the
+    results. If no search args, then return all results
     """
-    kwargs = {
-        **kwargs,
-        "args": args,
-        "journal": journal,
-        "old_entries": journal.entries,
-    }
-
-    if _has_search_args(args):
-        _filter_journal_entries(**kwargs)
-        _print_entries_found_count(len(journal), args)
-
-    # Where do the search results go?
-    if args.edit:
-        # If we want to both edit and change time in one action
-        if args.change_time:
-            # Generate a new list instead of assigning so it won't be
-            # modified by _change_time_search_results
-            selected_entries = [e for e in journal.entries]
-
-            no_change_time_prompt = len(journal.entries) == 1
-            _change_time_search_results(no_prompt=no_change_time_prompt, **kwargs)
-
-            # Re-filter the journal enties (_change_time_search_results
-            # puts the filtered entries back); use selected_entries
-            # instead of running _search_journal again, because times
-            # have changed since the original search
-            kwargs["old_entries"] = journal.entries
-            journal.entries = selected_entries
-
-        _edit_search_results(**kwargs)
+    logging.debug("Search mode: starting")
 
-    elif not journal:
-        # Bail out if there are no entries and we're not editing
+    # If no search args, then return all results (don't filter anything)
+    if not _has_search_args(args) and not _has_display_args(args) and not args.text:
+        logging.debug("Search mode: has no search args")
         return
 
-    elif args.change_time:
-        _change_time_search_results(**kwargs)
-
-    elif args.delete:
-        _delete_search_results(**kwargs)
-
-    else:
-        _display_search_results(**kwargs)
+    logging.debug("Search mode: has search args")
+    _filter_journal_entries(args, journal)
 
 
-def _write_in_editor(config, template=None):
+def _write_in_editor(config: dict, prepopulated_text: str | None = None) -> str:
     if config["editor"]:
-        logging.debug("Write mode: opening editor")
-        if not template:
-            template = _get_editor_template(config)
-        raw = get_text_from_editor(config, template)
-
+        logging.debug("Append mode: opening editor")
+        raw = get_text_from_editor(config, prepopulated_text)
     else:
         raw = get_text_from_stdin()
 
     return raw
 
 
-def _get_editor_template(config, **kwargs):
-    logging.debug("Write mode: loading template for entry")
-
-    if not config["template"]:
-        logging.debug("Write mode: no template configured")
-        return ""
-
-    template_path = expand_path(config["template"])
-
-    try:
-        template = open(template_path).read()
-        logging.debug("Write mode: template loaded: %s", template)
-    except OSError:
-        logging.error("Write mode: template not loaded")
-        raise JrnlException(
-            Message(
-                MsgText.CantReadTemplate,
-                MsgStyle.ERROR,
-                {"template": template_path},
-            )
-        )
-
-    return template
-
-
-def _has_search_args(args):
-    return any(
-        (
-            args.on_date,
-            args.today_in_history,
-            args.text,
-            args.month,
-            args.day,
-            args.year,
-            args.start_date,
-            args.end_date,
-            args.strict,
-            args.starred,
-            args.excluded,
-            args.contains,
-            args.limit,
-        )
-    )
-
-
-def _filter_journal_entries(args, journal, **kwargs):
+def _filter_journal_entries(args: "Namespace", journal: "Journal", **kwargs) -> None:
     """Filter journal entries in-place based upon search args"""
     if args.on_date:
         args.start_date = args.end_date = args.on_date
 
     if args.today_in_history:
         now = time.parse("now")
         args.day = now.day
@@ -286,47 +292,53 @@
         month=args.month,
         day=args.day,
         year=args.year,
         start_date=args.start_date,
         end_date=args.end_date,
         strict=args.strict,
         starred=args.starred,
+        tagged=args.tagged,
         exclude=args.excluded,
+        exclude_starred=args.exclude_starred,
+        exclude_tagged=args.exclude_tagged,
         contains=args.contains,
     )
     journal.limit(args.limit)
 
 
-def _print_entries_found_count(count, args):
+def _print_entries_found_count(count: int, args: "Namespace") -> None:
+    logging.debug(f"count: {count}")
     if count == 0:
         if args.edit or args.change_time:
             print_msg(Message(MsgText.NothingToModify, MsgStyle.WARNING))
         elif args.delete:
             print_msg(Message(MsgText.NothingToDelete, MsgStyle.WARNING))
         else:
             print_msg(Message(MsgText.NoEntriesFound, MsgStyle.NORMAL))
-    elif args.limit:
+        return
+    elif args.limit and args.limit == count:
         # Don't show count if the user expects a limited number of results
+        logging.debug("args.limit is true-ish")
         return
-    elif args.edit or not (args.change_time or args.delete):
-        # Don't show count if we are ONLY changing the time or deleting entries
-        my_msg = (
-            MsgText.EntryFoundCountSingular
-            if count == 1
-            else MsgText.EntryFoundCountPlural
-        )
-        print_msg(Message(my_msg, MsgStyle.NORMAL, {"num": count}))
+
+    logging.debug("Printing general summary")
+    my_msg = (
+        MsgText.EntryFoundCountSingular if count == 1 else MsgText.EntryFoundCountPlural
+    )
+    print_msg(Message(my_msg, MsgStyle.NORMAL, {"num": count}))
 
 
-def _other_entries(journal, entries):
+def _other_entries(journal: "Journal", entries: list["Entry"]) -> list["Entry"]:
     """Find entries that are not in journal"""
     return [e for e in entries if e not in journal.entries]
 
 
-def _edit_search_results(config, journal, old_entries, **kwargs):
+def _edit_search_results(
+    config: dict, journal: "Journal", old_entries: list["Entry"], **kwargs
+) -> None:
     """
     1. Send the given journal entries to the user-configured editor
     2. Print out stats on any modifications to journal
     3. Write modifications to journal
     """
     if not config["editor"]:
         raise JrnlException(
@@ -336,37 +348,35 @@
                 {"config_file": get_config_path()},
             )
         )
 
     # separate entries we are not editing
     other_entries = _other_entries(journal, old_entries)
 
-    # Get stats now for summary later
-    old_stats = _get_predit_stats(journal)
-
     # Send user to the editor
-    edited = get_text_from_editor(config, journal.editable_str())
-    journal.parse_editable_str(edited)
+    try:
+        edited = get_text_from_editor(config, journal.editable_str())
+    except JrnlException as e:
+        if e.has_message_text(MsgText.NoTextReceived):
+            raise JrnlException(
+                Message(MsgText.NoEditsReceivedJournalNotDeleted, MsgStyle.WARNING)
+            )
+        else:
+            raise e
 
-    # Print summary if available
-    _print_edited_summary(journal, old_stats)
+    journal.parse_editable_str(edited)
 
     # Put back entries we separated earlier, sort, and write the journal
     journal.entries += other_entries
     journal.sort()
     journal.write()
 
 
-def _print_edited_summary(journal, old_stats, **kwargs):
-    stats = {
-        "added": len(journal) - old_stats["count"],
-        "deleted": old_stats["count"] - len(journal),
-        "modified": len([e for e in journal.entries if e.modified]),
-    }
-    stats["modified"] -= stats["added"]
+def _print_changed_counts(journal: "Journal", **kwargs) -> None:
+    stats = journal.get_change_counts()
     msgs = []
 
     if stats["added"] > 0:
         my_msg = (
             MsgText.JournalCountAddedSingular
             if stats["added"] == 1
             else MsgText.JournalCountAddedPlural
@@ -391,52 +401,54 @@
 
     if not msgs:
         msgs.append(Message(MsgText.NoEditsReceived, MsgStyle.NORMAL))
 
     print_msgs(msgs)
 
 
-def _get_predit_stats(journal):
+def _get_predit_stats(journal: "Journal") -> dict[str, int]:
     return {"count": len(journal)}
 
 
-def _delete_search_results(journal, old_entries, **kwargs):
+def _delete_search_results(
+    journal: "Journal", old_entries: list["Entry"], **kwargs
+) -> None:
     entries_to_delete = journal.prompt_action_entries(MsgText.DeleteEntryQuestion)
 
+    journal.entries = old_entries
+
     if entries_to_delete:
-        journal.entries = old_entries
         journal.delete_entries(entries_to_delete)
 
         journal.write()
 
 
-def _change_time_search_results(args, journal, old_entries, no_prompt=False, **kwargs):
+def _change_time_search_results(
+    args: "Namespace",
+    journal: "Journal",
+    old_entries: list["Entry"],
+    no_prompt: bool = False,
+    **kwargs,
+) -> None:
     # separate entries we are not editing
-    other_entries = _other_entries(journal, old_entries)
-
-    if no_prompt:
-        entries_to_change = journal.entries
-    else:
-        entries_to_change = journal.prompt_action_entries(
-            MsgText.ChangeTimeEntryQuestion
-        )
+    # @todo if there's only 1, don't prompt
+    entries_to_change = journal.prompt_action_entries(MsgText.ChangeTimeEntryQuestion)
 
     if entries_to_change:
-        other_entries += [e for e in journal.entries if e not in entries_to_change]
-        journal.entries = entries_to_change
-
         date = time.parse(args.change_time)
-        journal.change_date_entries(date)
+        journal.entries = old_entries
+        journal.change_date_entries(date, entries_to_change)
 
-        journal.entries += other_entries
-        journal.sort()
         journal.write()
 
 
-def _display_search_results(args, journal, **kwargs):
+def _display_search_results(args: "Namespace", journal: "Journal", **kwargs) -> None:
+    if len(journal) == 0:
+        return
+
     # Get export format from config file if not provided at the command line
     args.export = args.export or kwargs["config"].get("display_format")
 
     if args.tags:
         print(plugins.get_exporter("tags").export(journal))
 
     elif args.short or args.export == "short":
@@ -446,7 +458,54 @@
         print(journal.pprint())
 
     elif args.export:
         exporter = plugins.get_exporter(args.export)
         print(exporter.export(journal, args.filename))
     else:
         print(journal.pprint())
+
+
+def _has_search_args(args: "Namespace") -> bool:
+    """Looking for arguments that filter a journal"""
+    return any(
+        (
+            args.contains,
+            args.tagged,
+            args.excluded,
+            args.exclude_starred,
+            args.exclude_tagged,
+            args.end_date,
+            args.today_in_history,
+            args.month,
+            args.day,
+            args.year,
+            args.limit,
+            args.on_date,
+            args.starred,
+            args.start_date,
+            args.strict,  # -and
+        )
+    )
+
+
+def _has_action_args(args: "Namespace") -> bool:
+    return any(
+        (
+            args.change_time,
+            args.delete,
+            args.edit,
+        )
+    )
+
+
+def _has_display_args(args: "Namespace") -> bool:
+    return any(
+        (
+            args.tags,
+            args.short,
+            args.export,  # --format
+        )
+    )
+
+
+def _has_only_tags(tag_symbols: str, args_text: str) -> bool:
+    return all(word[0] in tag_symbols for word in " ".join(args_text).split())
```

### Comparing `jrnl-3.3b2/jrnl/messages/MsgStyle.py` & `jrnl-4.0b0/jrnl/messages/MsgStyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 from enum import Enum
 from typing import Callable
 from typing import NamedTuple
 
 from rich import box
```

### Comparing `jrnl-3.3b2/jrnl/messages/MsgText.py` & `jrnl-4.0b0/jrnl/messages/MsgText.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 from enum import Enum
 
 
 class MsgText(Enum):
     def __str__(self) -> str:
@@ -24,23 +24,31 @@
         Please note that jrnl 1.x is NOT forward compatible with this version of jrnl.
         If you choose to proceed, you will not be able to use your journals with
         older versions of jrnl anymore.
         """
 
     AllDoneUpgrade = "We're all done here and you can start enjoying jrnl 2"
 
+    InstallComplete = """
+        jrnl configuration created at {config_path}
+        For advanced features, read the docs at https://jrnl.sh
+    """
+
     # --- Prompts --- #
     InstallJournalPathQuestion = """
         Path to your journal file (leave blank for {default_journal_path}):
         """
     DeleteEntryQuestion = "Delete entry '{entry_title}'?"
     ChangeTimeEntryQuestion = "Change time for '{entry_title}'?"
     EncryptJournalQuestion = """
         Do you want to encrypt your journal? (You can always change this later)
         """
+    UseColorsQuestion = """
+        Do you want jrnl to use colors when displaying entries? (You can always change this later)
+        """
     YesOrNoPromptDefaultYes = "[Y/n]"
     YesOrNoPromptDefaultNo = "[y/N]"
     ContinueUpgrade = "Continue upgrading jrnl?"
 
     # these should be lowercase, if possible in language
     # "lowercase" means whatever `.lower()` returns
     OneCharacterYes = "y"
@@ -89,20 +97,28 @@
         """
 
     ConfigEncryptedForUnencryptableJournalType = """
         The config for journal "{journal_name}" has 'encrypt' set to true, but this type
         of journal can't be encrypted. Please fix your config file.
         """
 
+    DecryptionFailedGeneric = "The decryption of journal data failed."
+
     KeyboardInterruptMsg = "Aborted by user"
 
-    CantReadTemplate = """
-        Unreadable template
-        Could not read template file at:
-        {template}
+    CantReadTemplateGlobalConfig = """
+        Could not read template file defined in config:
+        {global_template_path}
+        """
+
+    CantReadTemplateCLIArg = """
+        Unable to find a template file based on the passed arg, and no global template was detected.
+        The following filepaths were checked:
+        jrnl XDG Template Directory : {jrnl_template_dir}
+        Local Filepath              : {normalized_template_arg_filepath}
         """
 
     NoNamedJournal = "No '{journal_name}' journal configured\n{journals}"
 
     DoesNotExist = "{name} does not exist"
 
     # --- Journal status ---#
@@ -145,20 +161,30 @@
         To use the --edit option, please specify an editor your config file:
             {config_file}
 
         For examples of how to configure an external editor, see:
             https://jrnl.sh/en/stable/external-editors/
         """
 
+    NoEditsReceivedJournalNotDeleted = """
+        No text received from editor. Were you trying to delete all the entries?
+
+        This seems a bit drastic, so the operation was cancelled.
+
+        To delete all entries, use the --delete option.
+        """
+
     NoEditsReceived = "No edits to save, because nothing was changed"
 
     NoTextReceived = """
         No entry to save, because no text was received
         """
-
+    NoChangesToTemplate = """
+        No entry to save, because the template was not changed
+    """
     # --- Upgrade --- #
     JournalFailedUpgrade = """
         The following journal{s} failed to upgrade:
         {failed_journals}
 
         Please tell us about this problem at the following URL:
         https://github.com/jrnl-org/jrnl/issues/new?title=JournalFailedUpgrade
```

### Comparing `jrnl-3.3b2/jrnl/output.py` & `jrnl-4.0b0/jrnl/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import textwrap
-from typing import Union
+from typing import Callable
 
 from rich.console import Console
 from rich.text import Text
 
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 
 
-def deprecated_cmd(old_cmd, new_cmd, callback=None, **kwargs):
+def deprecated_cmd(
+    old_cmd: str, new_cmd: str, callback: Callable | None = None, **kwargs
+) -> None:
     print_msg(
         Message(
             MsgText.DeprecatedCommand,
             MsgStyle.WARNING,
             {"old_cmd": old_cmd, "new_cmd": new_cmd},
         )
     )
 
     if callback is not None:
         callback(**kwargs)
 
 
-def journal_list_to_json(journal_list):
+def journal_list_to_json(journal_list: dict) -> str:
     import json
 
     return json.dumps(journal_list)
 
 
-def journal_list_to_yaml(journal_list):
+def journal_list_to_yaml(journal_list: dict) -> str:
     from io import StringIO
 
     from ruamel.yaml import YAML
 
     output = StringIO()
     YAML().dump(journal_list, output)
     return output.getvalue()
 
 
-def journal_list_to_stdout(journal_list):
+def journal_list_to_stdout(journal_list: dict) -> str:
     result = f"Journals defined in config ({journal_list['config_path']})\n"
     ml = min(max(len(k) for k in journal_list["journals"]), 20)
     for journal, cfg in journal_list["journals"].items():
         result += " * {:{}} -> {}\n".format(
             journal, ml, cfg["journal"] if isinstance(cfg, dict) else cfg
         )
     return result
 
 
-def list_journals(configuration, format=None):
+def list_journals(configuration: dict, format: str | None = None) -> str:
     from jrnl import config
 
     """List the journals specified in the configuration file"""
 
     journal_list = {
         "config_path": config.get_config_path(),
         "journals": configuration["journals"],
@@ -65,27 +67,27 @@
         return journal_list_to_json(journal_list)
     elif format == "yaml":
         return journal_list_to_yaml(journal_list)
     else:
         return journal_list_to_stdout(journal_list)
 
 
-def print_msg(msg: Message, **kwargs) -> Union[None, str]:
+def print_msg(msg: Message, **kwargs) -> str | None:
     """Helper function to print a single message"""
     kwargs["style"] = msg.style
     return print_msgs([msg], **kwargs)
 
 
 def print_msgs(
     msgs: list[Message],
     delimiter: str = "\n",
     style: MsgStyle = MsgStyle.NORMAL,
     get_input: bool = False,
     hide_input: bool = False,
-) -> Union[None, str]:
+) -> str | None:
     # Same as print_msg, but for a list
     text = Text("", end="")
     kwargs = style.decoration.args
 
     for i, msg in enumerate(msgs):
         kwargs = _add_extra_style_args_if_needed(kwargs, msg=msg)
 
@@ -109,15 +111,15 @@
     console.print(decorated_text, new_line_start=style.prepend_newline)
 
 
 def _get_console(stderr: bool = True) -> Console:
     return Console(stderr=stderr)
 
 
-def _add_extra_style_args_if_needed(args, msg):
+def _add_extra_style_args_if_needed(args: dict, msg: Message):
     args["border_style"] = msg.style.color
     args["title"] = msg.style.box_title
     return args
 
 
 def format_msg_text(msg: Message) -> Text:
     text = textwrap.dedent(msg.text.value)
```

### Comparing `jrnl-3.3b2/jrnl/override.py` & `jrnl-4.0b0/jrnl/override.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
-from argparse import Namespace
+from typing import TYPE_CHECKING
 
 from jrnl.config import make_yaml_valid_dict
 from jrnl.config import update_config
 
+if TYPE_CHECKING:
+    from argparse import Namespace
+
 
 # import logging
-def apply_overrides(args: Namespace, base_config: dict) -> dict:
+def apply_overrides(args: "Namespace", base_config: dict) -> dict:
     """Unpack CLI provided overrides into the configuration tree.
 
     :param overrides: List of configuration key-value pairs collected from the CLI
     :type overrides: list
     :param base_config: Configuration Loaded from the saved YAML
     :type base_config: dict
     :return: Configuration to be used during runtime with the overrides applied
@@ -20,32 +23,31 @@
     """
     overrides = vars(args).get("config_override", None)
     if not overrides:
         return base_config
 
     cfg_with_overrides = base_config.copy()
     for pairs in overrides:
-
         pairs = make_yaml_valid_dict(pairs)
         key_as_dots, override_value = _get_key_and_value_from_pair(pairs)
         keys = _convert_dots_to_list(key_as_dots)
         cfg_with_overrides = _recursively_apply(
             cfg_with_overrides, keys, override_value
         )
 
     update_config(base_config, cfg_with_overrides, None)
     return base_config
 
 
-def _get_key_and_value_from_pair(pairs):
+def _get_key_and_value_from_pair(pairs: dict) -> tuple:
     key_as_dots, override_value = list(pairs.items())[0]
     return key_as_dots, override_value
 
 
-def _convert_dots_to_list(key_as_dots):
+def _convert_dots_to_list(key_as_dots: str) -> list[str]:
     keys = key_as_dots.split(".")
     keys = [k for k in keys if k != ""]  # remove empty elements
     return keys
 
 
 def _recursively_apply(tree: dict, nodes: list, override_value) -> dict:
     """Recurse through configuration and apply overrides at the leaf of the config tree
```

### Comparing `jrnl-3.3b2/jrnl/plugins/__init__.py` & `jrnl-4.0b0/jrnl/plugins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+from typing import Type
+
 from jrnl.plugins.dates_exporter import DatesExporter
 from jrnl.plugins.fancy_exporter import FancyExporter
 from jrnl.plugins.jrnl_importer import JRNLImporter
 from jrnl.plugins.json_exporter import JSONExporter
 from jrnl.plugins.markdown_exporter import MarkdownExporter
 from jrnl.plugins.tag_exporter import TagExporter
 from jrnl.plugins.text_exporter import TextExporter
@@ -28,19 +30,19 @@
 __exporter_types["short"] = None
 __importer_types = {name: plugin for plugin in __importers for name in plugin.names}
 
 EXPORT_FORMATS = sorted(__exporter_types.keys())
 IMPORT_FORMATS = sorted(__importer_types.keys())
 
 
-def get_exporter(format):
+def get_exporter(format: str) -> Type[TextExporter] | None:
     for exporter in __exporters:
         if hasattr(exporter, "names") and format in exporter.names:
             return exporter
     return None
 
 
-def get_importer(format):
+def get_importer(format: str) -> Type[JRNLImporter] | None:
     for importer in __importers:
         if hasattr(importer, "names") and format in importer.names:
             return importer
     return None
```

### Comparing `jrnl-3.3b2/jrnl/plugins/dates_exporter.py` & `jrnl-4.0b0/jrnl/plugins/dates_exporter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 from collections import Counter
+from typing import TYPE_CHECKING
 
 from jrnl.plugins.text_exporter import TextExporter
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class DatesExporter(TextExporter):
     """This Exporter lists dates and their respective counts, for heatingmapping etc."""
 
     names = ["dates"]
     extension = "dates"
 
     @classmethod
-    def export_entry(cls, entry):
+    def export_entry(cls, entry: "Entry"):
         raise NotImplementedError
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns dates and their frequencies for an entire journal."""
         date_counts = Counter()
         for entry in journal.entries:
             # entry.date.date() gets date without time
             date = str(entry.date.date())
             date_counts[date] += 1
         result = "\n".join(f"{date}, {count}" for date, count in date_counts.items())
```

### Comparing `jrnl-3.3b2/jrnl/plugins/fancy_exporter.py` & `jrnl-4.0b0/jrnl/plugins/fancy_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import logging
 import os
 from textwrap import TextWrapper
+from typing import TYPE_CHECKING
 
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.plugins.text_exporter import TextExporter
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class FancyExporter(TextExporter):
     """This Exporter can convert entries and journals into text with unicode box drawing characters."""
 
     names = ["fancy", "boxed"]
     extension = "txt"
 
@@ -31,15 +36,15 @@
     border_i = "┠"
     border_j = "╌"
     border_k = "┤"
     border_l = "┖"
     border_m = "┘"
 
     @classmethod
-    def export_entry(cls, entry):
+    def export_entry(cls, entry: "Entry") -> str:
         """Returns a fancy unicode representation of a single entry."""
         date_str = entry.date.strftime(entry.journal.config["timeformat"])
 
         if entry.journal.config["linewrap"]:
             linewrap = entry.journal.config["linewrap"]
 
             if linewrap == "auto":
@@ -91,20 +96,22 @@
                 body_lines = w.wrap(line) or [cls.border_g]
                 for body_line in body_lines:
                     card.append(body_line.ljust(body_linewrap + 1) + cls.border_h)
         card.append(cls.border_l + cls.border_b * body_linewrap + cls.border_m)
         return "\n".join(card)
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal) -> str:
         """Returns a unicode representation of an entire journal."""
         return "\n".join(cls.export_entry(entry) for entry in journal)
 
 
-def check_provided_linewrap_viability(linewrap, card, journal):
+def check_provided_linewrap_viability(
+    linewrap: int, card: list[str], journal: "Journal"
+):
     if len(card[0]) > linewrap:
         width_violation = len(card[0]) - linewrap
         raise JrnlException(
             Message(
                 MsgText.LineWrapTooSmallForDateFormat,
                 MsgStyle.NORMAL,
                 {
```

### Comparing `jrnl-3.3b2/jrnl/plugins/jrnl_importer.py` & `jrnl-4.0b0/jrnl/plugins/jrnl_importer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import sys
+from typing import TYPE_CHECKING
 
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 
+if TYPE_CHECKING:
+    from jrnl.journals import Journal
+
 
 class JRNLImporter:
     """This plugin imports entries from other jrnl files."""
 
     names = ["jrnl"]
 
     @staticmethod
-    def import_(journal, input=None):
+    def import_(journal: "Journal", input: str | None = None) -> None:
         """Imports from an existing file if input is specified, and
         standard input otherwise."""
         old_cnt = len(journal.entries)
         if input:
             with open(input, "r", encoding="utf-8") as f:
                 other_journal_txt = f.read()
         else:
```

### Comparing `jrnl-3.3b2/jrnl/plugins/json_exporter.py` & `jrnl-4.0b0/jrnl/plugins/json_exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import json
+from typing import TYPE_CHECKING
 
 from jrnl.plugins.text_exporter import TextExporter
 from jrnl.plugins.util import get_tags_count
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class JSONExporter(TextExporter):
     """This Exporter can convert entries and journals into json."""
 
     names = ["json"]
     extension = "json"
 
     @classmethod
-    def entry_to_dict(cls, entry):
+    def entry_to_dict(cls, entry: "Entry") -> dict:
         entry_dict = {
             "title": entry.title,
             "body": entry.body,
             "date": entry.date.strftime("%Y-%m-%d"),
             "time": entry.date.strftime("%H:%M"),
             "tags": entry.tags,
             "starred": entry.starred,
@@ -45,20 +50,20 @@
                 entry_dict["creator"]["os_agent"] = entry.creator_os_agent
             if hasattr(entry, "creator_software_agent"):
                 entry_dict["creator"]["software_agent"] = entry.creator_software_agent
 
         return entry_dict
 
     @classmethod
-    def export_entry(cls, entry):
+    def export_entry(cls, entry: "Entry") -> str:
         """Returns a json representation of a single entry."""
         return json.dumps(cls.entry_to_dict(entry), indent=2) + "\n"
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns a json representation of an entire journal."""
         tags = get_tags_count(journal)
         result = {
             "tags": {tag: count for count, tag in tags},
             "entries": [cls.entry_to_dict(e) for e in journal.entries],
         }
         return json.dumps(result, indent=2)
```

### Comparing `jrnl-3.3b2/jrnl/plugins/markdown_exporter.py` & `jrnl-4.0b0/jrnl/plugins/markdown_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import os
 import re
+from typing import TYPE_CHECKING
 
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.plugins.text_exporter import TextExporter
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class MarkdownExporter(TextExporter):
     """This Exporter can convert entries and journals into Markdown."""
 
     names = ["md", "markdown"]
     extension = "md"
 
     @classmethod
-    def export_entry(cls, entry, to_multifile=True):
+    def export_entry(cls, entry: "Entry", to_multifile: bool = True) -> str:
         """Returns a markdown representation of a single entry."""
         date_str = entry.date.strftime(entry.journal.config["timeformat"])
         body_wrapper = "\n" if entry.body else ""
         body = body_wrapper + entry.body
 
         if to_multifile is True:
             heading = "#"
@@ -69,23 +74,23 @@
                     {"date": date_str, "title": entry.title},
                 )
             )
 
         return f"{heading} {date_str} {entry.title}\n{newbody} "
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns a Markdown representation of an entire journal."""
         out = []
         year, month = -1, -1
         for e in journal.entries:
-            if not e.date.year == year:
+            if e.date.year != year:
                 year = e.date.year
                 out.append("# " + str(year))
                 out.append("")
-            if not e.date.month == month:
+            if e.date.month != month:
                 month = e.date.month
                 out.append("## " + e.date.strftime("%B"))
                 out.append("")
             out.append(cls.export_entry(e, False))
         result = "\n".join(out)
         return result
```

### Comparing `jrnl-3.3b2/jrnl/plugins/tag_exporter.py` & `jrnl-4.0b0/jrnl/plugins/tag_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+from typing import TYPE_CHECKING
+
 from jrnl.plugins.text_exporter import TextExporter
 from jrnl.plugins.util import get_tags_count
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class TagExporter(TextExporter):
     """This Exporter can lists the tags for entries and journals, exported as a plain text file."""
 
     names = ["tags"]
     extension = "tags"
 
     @classmethod
-    def export_entry(cls, entry):
+    def export_entry(cls, entry: "Entry") -> str:
         """Returns a list of tags for a single entry."""
         return ", ".join(entry.tags)
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns a list of tags and their frequency for an entire journal."""
         tag_counts = get_tags_count(journal)
         result = ""
         if not tag_counts:
             return "[No tags found in journal.]"
         elif min(tag_counts)[0] == 0:
             tag_counts = filter(lambda x: x[0] > 1, tag_counts)
```

### Comparing `jrnl-3.3b2/jrnl/plugins/text_exporter.py` & `jrnl-4.0b0/jrnl/plugins/text_exporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import errno
 import os
 import re
 import unicodedata
+from typing import TYPE_CHECKING
 
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class TextExporter:
     """This Exporter can convert entries and journals into text files."""
 
     names = ["text", "txt"]
     extension = "txt"
 
     @classmethod
-    def export_entry(cls, entry):
+    def export_entry(cls, entry: "Entry") -> str:
         """Returns a string representation of a single entry."""
         return str(entry)
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns a string representation of an entire journal."""
         return "\n".join(cls.export_entry(entry) for entry in journal)
 
     @classmethod
-    def write_file(cls, journal, path):
+    def write_file(cls, journal: "Journal", path: str) -> str:
         """Exports a journal into a single file."""
         export_str = cls.export_journal(journal)
         with open(path, "w", encoding="utf-8") as f:
             f.write(export_str)
         print_msg(
             Message(
                 MsgText.JournalExportedTo,
@@ -42,21 +47,21 @@
                     "path": path,
                 },
             )
         )
         return ""
 
     @classmethod
-    def make_filename(cls, entry):
+    def make_filename(cls, entry: "Entry") -> str:
         return entry.date.strftime("%Y-%m-%d") + "_{}.{}".format(
             cls._slugify(str(entry.title)), cls.extension
         )
 
     @classmethod
-    def write_files(cls, journal, path):
+    def write_files(cls, journal: "Journal", path: str) -> str:
         """Exports a journal into individual files for each entry."""
         for entry in journal.entries:
             entry_is_written = False
             while not entry_is_written:
                 full_path = os.path.join(path, cls.make_filename(entry))
                 try:
                     with open(full_path, "w", encoding="utf-8") as f:
@@ -78,25 +83,25 @@
                 MsgText.JournalExportedTo,
                 MsgStyle.NORMAL,
                 {"path": path},
             )
         )
         return ""
 
-    def _slugify(string):
+    def _slugify(string: str) -> str:
         """Slugifies a string.
         Based on public domain code from https://github.com/zacharyvoase/slugify
         """
         normalized_string = str(unicodedata.normalize("NFKD", string))
         no_punctuation = re.sub(r"[^\w\s-]", "", normalized_string).strip().lower()
         slug = re.sub(r"[-\s]+", "-", no_punctuation)
         return slug
 
     @classmethod
-    def export(cls, journal, output=None):
+    def export(cls, journal: "Journal", output: str | None = None) -> str:
         """Exports to individual files if output is an existing path, or into
         a single file if output is a file name, or returns the exporter's
         representation as string if output is None."""
         if output and os.path.isdir(output):  # multiple files
             return cls.write_files(journal, output)
         elif output:  # single file
             return cls.write_file(journal, output)
```

### Comparing `jrnl-3.3b2/jrnl/plugins/util.py` & `jrnl-4.0b0/jrnl/plugins/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+from typing import TYPE_CHECKING
 
-def get_tags_count(journal):
+if TYPE_CHECKING:
+    from jrnl.journals import Journal
+
+
+def get_tags_count(journal: "Journal") -> set[tuple[int, str]]:
     """Returns a set of tuples (count, tag) for all tags present in the journal."""
     # Astute reader: should the following line leave you as puzzled as me the first time
     # I came across this construction, worry not and embrace the ensuing moment of enlightment.
     tags = [tag for entry in journal.entries for tag in set(entry.tags)]
     # To be read: [for entry in journal.entries: for tag in set(entry.tags): tag]
     tag_counts = {(tags.count(tag), tag) for tag in tags}
     return tag_counts
 
 
-def oxford_list(lst):
+def oxford_list(lst: list) -> str:
     """Return Human-readable list of things obeying the object comma)"""
     lst = sorted(lst)
     if not lst:
         return "(nothing)"
     elif len(lst) == 1:
         return lst[0]
     elif len(lst) == 2:
```

### Comparing `jrnl-3.3b2/jrnl/plugins/xml_exporter.py` & `jrnl-4.0b0/jrnl/plugins/xml_exporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+from typing import TYPE_CHECKING
 from xml.dom import minidom
 
 from jrnl.plugins.json_exporter import JSONExporter
 from jrnl.plugins.util import get_tags_count
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class XMLExporter(JSONExporter):
     """This Exporter can convert entries and journals into XML."""
 
     names = ["xml"]
     extension = "xml"
 
     @classmethod
-    def export_entry(cls, entry, doc=None):
+    def export_entry(
+        cls, entry: "Entry", doc: minidom.Document | None = None
+    ) -> minidom.Element | str:
         """Returns an XML representation of a single entry."""
         doc_el = doc or minidom.Document()
         entry_el = doc_el.createElement("entry")
         for key, value in cls.entry_to_dict(entry).items():
             elem = doc_el.createElement(key)
             elem.appendChild(doc_el.createTextNode(value))
             entry_el.appendChild(elem)
         if not doc:
             doc_el.appendChild(entry_el)
             return doc_el.toprettyxml()
         else:
             return entry_el
 
     @classmethod
-    def entry_to_xml(cls, entry, doc):
+    def entry_to_xml(cls, entry: "Entry", doc: minidom.Document) -> minidom.Element:
         entry_el = doc.createElement("entry")
         entry_el.setAttribute("date", entry.date.isoformat())
         if hasattr(entry, "uuid"):
             entry_el.setAttribute("uuid", entry.uuid)
         entry_el.setAttribute("starred", entry.starred)
         tags = entry.tags
         for tag in tags:
             tag_el = doc.createElement("tag")
             tag_el.setAttribute("name", tag)
             entry_el.appendChild(tag_el)
         entry_el.appendChild(doc.createTextNode(entry.fulltext))
         return entry_el
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal") -> str:
         """Returns an XML representation of an entire journal."""
         tags = get_tags_count(journal)
         doc = minidom.Document()
         xml = doc.createElement("journal")
         tags_el = doc.createElement("tags")
         entries_el = doc.createElement("entries")
         for count, tag in tags:
```

### Comparing `jrnl-3.3b2/jrnl/plugins/yaml_exporter.py` & `jrnl-4.0b0/jrnl/plugins/yaml_exporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import os
 import re
+from typing import TYPE_CHECKING
 
 from jrnl.exception import JrnlException
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.plugins.text_exporter import TextExporter
 
+if TYPE_CHECKING:
+    from jrnl.journals import Entry
+    from jrnl.journals import Journal
+
 
 class YAMLExporter(TextExporter):
     """This Exporter can convert entries and journals into Markdown formatted text with YAML front matter."""
 
     names = ["yaml"]
     extension = "md"
 
     @classmethod
-    def export_entry(cls, entry, to_multifile=True):
+    def export_entry(cls, entry: "Entry", to_multifile: bool = True) -> str:
         """Returns a markdown representation of a single entry, with YAML front matter."""
         if to_multifile is False:
             raise JrnlException(Message(MsgText.YamlMustBeDirectory, MsgStyle.ERROR))
 
         date_str = entry.date.strftime(entry.journal.config["timeformat"])
         body_wrapper = "\n" if entry.body else ""
         body = body_wrapper + entry.body
 
         tagsymbols = entry.journal.config["tagsymbols"]
-        # see also Entry.Entry.rag_regex
+        # see also Entry.rag_regex
         multi_tag_regex = re.compile(rf"(?u)^\s*([{tagsymbols}][-+*#/\w]+\s*)+$")
 
         """Increase heading levels in body text"""
         newbody = ""
         heading = "#"
         previous_line = ""
         warn_on_heading_level = False
@@ -120,10 +125,10 @@
             tags=", ".join([tag[1:] for tag in entry.tags]),
             dayone=dayone_attributes,
             body=spacebody,
             end="...",
         )
 
     @classmethod
-    def export_journal(cls, journal):
+    def export_journal(cls, journal: "Journal"):
         """Returns an error, as YAML export requires a directory as a target."""
         raise JrnlException(Message(MsgText.YamlMustBeDirectory, MsgStyle.ERROR))
```

### Comparing `jrnl-3.3b2/jrnl/prompt.py` & `jrnl-4.0b0/jrnl/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.output import print_msgs
@@ -31,22 +31,36 @@
             Message(MsgText.PasswordConfirmEntry, MsgStyle.PROMPT), **kwargs
         ):
             break
 
         print_msg(Message(MsgText.PasswordDidNotMatch, MsgStyle.ERROR))
 
     if yesno(Message(MsgText.PasswordStoreInKeychain), default=True):
-        from jrnl.EncryptedJournal import set_keychain
+        from jrnl.keyring import set_keyring_password
 
-        set_keychain(journal_name, pw)
+        set_keyring_password(pw, journal_name)
 
     return pw
 
 
-def yesno(prompt: Message, default: bool = True) -> bool:
+def prompt_password(first_try: bool = True) -> str:
+    if not first_try:
+        print_msg(Message(MsgText.WrongPasswordTryAgain, MsgStyle.WARNING))
+
+    return (
+        print_msg(
+            Message(MsgText.Password, MsgStyle.PROMPT),
+            get_input=True,
+            hide_input=True,
+        )
+        or ""
+    )
+
+
+def yesno(prompt: Message | str, default: bool = True) -> bool:
     response = print_msgs(
         [
             prompt,
             Message(
                 MsgText.YesOrNoPromptDefaultYes
                 if default
                 else MsgText.YesOrNoPromptDefaultNo
```

### Comparing `jrnl-3.3b2/jrnl/upgrade.py` & `jrnl-4.0b0/jrnl/upgrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Copyright © 2012-2022 jrnl contributors
+# Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
+import logging
 import os
 
-from jrnl import Journal
 from jrnl import __version__
 from jrnl.config import is_config_json
 from jrnl.config import load_config
 from jrnl.config import scope_config
-from jrnl.EncryptedJournal import EncryptedJournal
 from jrnl.exception import JrnlException
+from jrnl.journals import Journal
+from jrnl.journals import open_journal
 from jrnl.messages import Message
 from jrnl.messages import MsgStyle
 from jrnl.messages import MsgText
 from jrnl.output import print_msg
 from jrnl.output import print_msgs
 from jrnl.path import expand_path
 from jrnl.prompt import yesno
 
 
-def backup(filename, binary=False):
+def backup(filename: str, binary: bool = False):
     filename = expand_path(filename)
 
     try:
         with open(filename, "rb" if binary else "r") as original:
             contents = original.read()
 
         with open(filename + ".backup", "wb" if binary else "w") as backup:
@@ -38,22 +39,22 @@
     except FileNotFoundError:
         print_msg(Message(MsgText.DoesNotExist, MsgStyle.WARNING, {"name": filename}))
         cont = yesno(f"\nCreate {filename}?", default=False)
         if not cont:
             raise JrnlException(Message(MsgText.UpgradeAborted, MsgStyle.WARNING))
 
 
-def check_exists(path):
+def check_exists(path: str) -> bool:
     """
     Checks if a given path exists.
     """
     return os.path.exists(path)
 
 
-def upgrade_jrnl(config_path):
+def upgrade_jrnl(config_path: str) -> None:
     config = load_config(config_path)
 
     print_msg(Message(MsgText.WelcomeToJrnl, MsgStyle.NORMAL, {"version": __version__}))
 
     encrypted_journals = {}
     plain_journals = {}
     other_journals = {}
@@ -111,49 +112,59 @@
         journals=other_journals,
         header=Message(MsgText.JournalsToIgnore),
         **kwargs,
     )
 
     cont = yesno(Message(MsgText.ContinueUpgrade), default=False)
     if not cont:
-        raise JrnlException(Message(MsgText.UpgradeAborted), MsgStyle.WARNING)
+        raise JrnlException(Message(MsgText.UpgradeAborted, MsgStyle.WARNING))
 
     for journal_name, path in encrypted_journals.items():
         print_msg(
             Message(
                 MsgText.UpgradingJournal,
                 params={
                     "journal_name": journal_name,
                     "path": path,
                 },
             )
         )
 
         backup(path, binary=True)
-        old_journal = Journal.open_journal(
+        old_journal = open_journal(
             journal_name, scope_config(config, journal_name), legacy=True
         )
-        all_journals.append(EncryptedJournal.from_journal(old_journal))
+
+        logging.debug(f"Clearing encryption method for '{journal_name}' journal")
+
+        # Update the encryption method
+        new_journal = Journal.from_journal(old_journal)
+        new_journal.config["encrypt"] = "jrnlv2"
+        new_journal._get_encryption_method()
+        # Copy over password (jrnlv1 only supported password-based encryption)
+        new_journal.encryption_method.password = old_journal.encryption_method.password
+
+        all_journals.append(new_journal)
 
     for journal_name, path in plain_journals.items():
         print_msg(
             Message(
                 MsgText.UpgradingJournal,
                 params={
                     "journal_name": journal_name,
                     "path": path,
                 },
             )
         )
 
         backup(path)
-        old_journal = Journal.open_journal(
+        old_journal = open_journal(
             journal_name, scope_config(config, journal_name), legacy=True
         )
-        all_journals.append(Journal.PlainJournal.from_journal(old_journal))
+        all_journals.append(Journal.from_journal(old_journal))
 
     # loop through lists to validate
     failed_journals = [j for j in all_journals if not j.validate_parsing()]
 
     if len(failed_journals) > 0:
         raise JrnlException(
             Message(MsgText.AbortingUpgrade, MsgStyle.WARNING),
@@ -174,15 +185,15 @@
     print_msg(Message(MsgText.UpgradingConfig, MsgStyle.NORMAL))
 
     backup(config_path)
 
     print_msg(Message(MsgText.AllDoneUpgrade, MsgStyle.NORMAL))
 
 
-def is_old_version(config_path):
+def is_old_version(config_path: str) -> bool:
     return is_config_json(config_path)
 
 
 def _print_journal_summary(journals: dict, header: Message, pad: int) -> None:
     if not journals:
         return
```

### Comparing `jrnl-3.3b2/pyproject.toml` & `jrnl-4.0b0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jrnl"
-version = "v3.3-beta2"
+version = "v4.0-beta"
 description = "Collect your thoughts and notes without leaving the command line."
 authors = [
     "jrnl contributors <maintainers@jrnl.sh>",
     "Manuel Ebert <manuel@1450.me>",
     "Jonathan Wren <jonathan@nowandwren.com>",
     "Micah Ellison <micahellison@gmail.com>"
 ]
@@ -23,68 +23,54 @@
 
 [tool.poetry.urls]
 "Documentation" = "https://jrnl.sh"
 "Issue Tracker" = "https://github.com/jrnl-org/jrnl/issues"
 "Funding" = "https://opencollective.com/jrnl"
 
 [tool.poetry.dependencies]
-python = ">=3.9.0, <3.12"
+python = ">=3.10.0, <3.13"
 
 ansiwrap = "^0.8.4"
 colorama = ">=0.4"       # https://github.com/tartley/colorama/blob/master/CHANGELOG.rst
 cryptography = ">=3.0"   # https://cryptography.io/en/latest/api-stability.html
 keyring = ">=21.0"       # https://github.com/jaraco/keyring#integration
 parsedatetime = ">=2.6"
 python-dateutil = "^2.8" # https://github.com/dateutil/dateutil/blob/master/RELEASING
 pyxdg = ">=0.27.0"
 "ruamel.yaml" = "^0.17.21"
-rich = "^12.2.0"
+rich = ">=12.2.0, <14.0.0"
 
 # dayone-only deps
 tzlocal = ">=4.0"   # https://github.com/regebro/tzlocal/blob/master/CHANGES.txt
 
 [tool.poetry.dev-dependencies]
 black = { version = ">=21.5b2", allow-prereleases = true }
+flakeheaven = ">=3.0"
+flake8-black = ">=0.3.3"
+flake8-isort = ">=5.0.0"
+flake8-type-checking = ">=2.2.0"
+flake8-simplify = ">=0.19"
 ipdb = "*"
 isort = ">=5.10"
-mkdocs = ">=1.0,<1.3"
+mkdocs = ">=1.4"
+parse-type = ">=0.6.0"
 poethepoet = "*"
-pyproject-flake8 = "*"
 pytest = ">=6.2"
-pytest-bdd = ">=4.0.1,<6.0"
+pytest-bdd = ">=6.0"
 pytest-clarity = "*"
 pytest-xdist = ">=2.5.0"
 requests = "*"
 toml = ">=0.10"
 tox = "*"
 xmltodict = "*"
 
 [tool.poetry.scripts]
-jrnl = 'jrnl.cli:cli'
+jrnl = 'jrnl.main:run'
 
 [tool.poe.tasks]
-format-run = [
-  {cmd = "black ."},
-]
-format-check = [
-  {cmd = "black --version"},
-  {cmd = "black --check --diff ."},
-]
-style-check = [
-  {cmd = "pflake8 --version"},
-  {cmd = "pflake8 jrnl tests tasks.py"},
-]
-sort-run = [
-  {cmd = "isort ."},
-]
-sort-check = [
-  {cmd = "isort --version"},
-  {cmd = "isort --check ."},
-]
-
 docs-check.default_item_type = "script"
 docs-check.sequence = [
   "tasks:delete_files(['sitemap.xml', 'config.json'])",
   "tasks:generate_sitemap",
   "tasks:output_file('sitemap.xml')",
   "tasks:generate_pa11y_config_from_sitemap",
   "tasks:output_file('config.json')",
@@ -95,30 +81,31 @@
   {cmd = "mkdocs serve"},
 ]
 
 test-run = [
   {cmd = "tox -q -e py --"},
 ]
 
-installer-check = [
-  {cmd = "poetry --version"},
-  {cmd = "poetry check"},
+# Groups of tasks
+format.default_item_type = "cmd"
+format.sequence = [
+  "isort .",
+  "black .",
 ]
 
-# Groups of tasks
-format = [
-  "format-run",
-  "sort-run",
-]
-lint = [
-  "installer-check",
-  "style-check",
-  "sort-check",
-  "format-check",
+lint.env = { FLAKEHEAVEN_CACHE_TIMEOUT = "0" }
+lint.default_item_type = "cmd"
+lint.sequence = [
+  "poetry --version",
+  "poetry check",
+  "flakeheaven --version",
+  "flakeheaven plugins",
+  "flakeheaven lint",
 ]
+
 test = [
   "lint",
   "test-run",
 ]
 
 [tool.isort]
 profile = "black"
@@ -146,17 +133,37 @@
 filterwarnings = [
     "ignore::DeprecationWarning",
     "ignore:Flag style will be deprecated in.*",
     "ignore:[WinError 32].*",
     "ignore:[WinError 5].*"
 ]
 
-[tool.flake8]
-# ignore formatting warnings and errors because we use Black to autoformat
-extend-ignore = "E101,E111,E114,E115,E116,E117,E12,E13,E2,E3,E401,E5,E70,W1,W2,W3,W5"
+[tool.flakeheaven]
+max_line_length = 88
+exclude = [".git", ".tox", ".venv", "node_modules"]
+
+[tool.flakeheaven.plugins]
+"py*" = ["+*"]
+pycodestyle = [
+  "-E101",
+  "-E111", "-E114", "-E115", "-E116", "-E117",
+  "-E12*",
+  "-E13*",
+  "-E2*",
+  "-E3*",
+  "-E401",
+  "-E5*",
+  "-E70",
+  "-W1*", "-W2*", "-W3*", "-W5*",
+]
+"flake8-*" = ["+*"]
+flake8-black = ["-BLK901"]
+
+[tool.flakeheaven.exceptions."jrnl/journals/__init__.py"]
+pyflakes = ["-F401"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tox]
 # see: https://tox.wiki/en/latest/example/basic.html
@@ -164,14 +171,15 @@
 [tox]
 envlist = py
 isolated_build = True
 
 [testenv]
 deps =
   pytest >= 6.2
-  pytest-bdd >=4.0.1,<6.0
+  pytest-bdd >=6.0
   pytest-xdist >=2.5.0
+  parse-type >=0.6.0
   toml >=0.10
 
 commands = pytest {posargs}
 passenv = HOME
 """
```

### Comparing `jrnl-3.3b2/PKG-INFO` & `jrnl-4.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: jrnl
-Version: 3.3b2
+Version: 4.0b0
 Summary: Collect your thoughts and notes without leaving the command line.
 Home-page: https://jrnl.sh
 License: GPL-3.0-only
 Author: jrnl contributors
 Author-email: maintainers@jrnl.sh
 Maintainer: Jonathan Wren and Micah Ellison
 Maintainer-email: maintainers@jrnl.sh
-Requires-Python: >=3.9.0,<3.12
+Requires-Python: >=3.10.0,<3.13
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: News/Diary
 Requires-Dist: ansiwrap (>=0.8.4,<0.9.0)
 Requires-Dist: colorama (>=0.4)
 Requires-Dist: cryptography (>=3.0)
 Requires-Dist: keyring (>=21.0)
 Requires-Dist: parsedatetime (>=2.6)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: pyxdg (>=0.27.0)
-Requires-Dist: rich (>=12.2.0,<13.0.0)
+Requires-Dist: rich (>=12.2.0,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tzlocal (>=4.0)
 Project-URL: Documentation, https://jrnl.sh
 Project-URL: Funding, https://opencollective.com/jrnl
 Project-URL: Issue Tracker, https://github.com/jrnl-org/jrnl/issues
 Project-URL: Repository, https://github.com/jrnl-org/jrnl
 Description-Content-Type: text/markdown
 
 <!--
-Copyright © 2012-2022 jrnl contributors
+Copyright © 2012-2023 jrnl contributors
 License: https://www.gnu.org/licenses/gpl-3.0.html
 -->
 
 <p align="center">
 <a href="https://jrnl.sh">
 <img align="center" src="https://raw.githubusercontent.com/jrnl-org/jrnl/develop/docs_theme/assets/readme-header.png"/>
 </a>
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: jrnl Version: 3.3b2 Summary: Collect your thoughts
+Metadata-Version: 2.1 Name: jrnl Version: 4.0b0 Summary: Collect your thoughts
 and notes without leaving the command line. Home-page: https://jrnl.sh License:
 GPL-3.0-only Author: jrnl contributors Author-email: maintainers@jrnl.sh
 Maintainer: Jonathan Wren and Micah Ellison Maintainer-email:
-maintainers@jrnl.sh Requires-Python: >=3.9.0,<3.12 Classifier: Environment ::
+maintainers@jrnl.sh Requires-Python: >=3.10.0,<3.13 Classifier: Environment ::
 Console Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Office/Business :: News/Diary
-Requires-Dist: ansiwrap (>=0.8.4,<0.9.0) Requires-Dist: colorama (>=0.4)
-Requires-Dist: cryptography (>=3.0) Requires-Dist: keyring (>=21.0) Requires-
-Dist: parsedatetime (>=2.6) Requires-Dist: python-dateutil (>=2.8,<3.0)
-Requires-Dist: pyxdg (>=0.27.0) Requires-Dist: rich (>=12.2.0,<13.0.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: tzlocal (>=4.0)
-Project-URL: Documentation, https://jrnl.sh Project-URL: Funding, https://
-opencollective.com/jrnl Project-URL: Issue Tracker, https://github.com/jrnl-
-org/jrnl/issues Project-URL: Repository, https://github.com/jrnl-org/jrnl
-Description-Content-Type: text/markdown
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Office/
+Business :: News/Diary Requires-Dist: ansiwrap (>=0.8.4,<0.9.0) Requires-Dist:
+colorama (>=0.4) Requires-Dist: cryptography (>=3.0) Requires-Dist: keyring
+(>=21.0) Requires-Dist: parsedatetime (>=2.6) Requires-Dist: python-dateutil
+(>=2.8,<3.0) Requires-Dist: pyxdg (>=0.27.0) Requires-Dist: rich
+(>=12.2.0,<14.0.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-
+Dist: tzlocal (>=4.0) Project-URL: Documentation, https://jrnl.sh Project-URL:
+Funding, https://opencollective.com/jrnl Project-URL: Issue Tracker, https://
+github.com/jrnl-org/jrnl/issues Project-URL: Repository, https://github.com/
+jrnl-org/jrnl Description-Content-Type: text/markdown
   [https://raw.githubusercontent.com/jrnl-org/jrnl/develop/docs_theme/assets/
                               readme-header.png]
 jrnl [![Testing](https://github.com/jrnl-org/jrnl/workflows/Testing/badge.svg)]
 (https://github.com/jrnl-org/jrnl/actions?query=workflow%3ATesting) [!
 [Downloads](https://pepy.tech/badge/jrnl)](https://pepy.tech/project/jrnl) [!
 [Version](http://img.shields.io/pypi/v/jrnl.svg?style=flat)](https://
 pypi.python.org/pypi/jrnl/) [![Homebrew](https://img.shields.io/homebrew/v/
```

