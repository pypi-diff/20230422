# Comparing `tmp/yq-3.2.1.tar.gz` & `tmp/yq-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yq-3.2.1.tar", last modified: Wed Apr  5 01:36:45 2023, max compression
+gzip compressed data, was "yq-3.2.2.tar", last modified: Sat Apr 22 21:42:29 2023, max compression
```

## Comparing `yq-3.2.1.tar` & `yq-3.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.064396 yq-3.2.1/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.060121 yq-3.2.1/.github/
--rw-r--r--   0 kislyuk    (501) staff       (20)       18 2022-07-03 19:16:59.000000 yq-3.2.1/.github/FUNDING.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.060323 yq-3.2.1/.github/workflows/
--rw-r--r--   0 kislyuk    (501) staff       (20)      837 2023-04-05 01:34:39.000000 yq-3.2.1/.github/workflows/ci.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      477 2022-07-03 19:16:59.000000 yq-3.2.1/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)     7471 2023-04-05 01:36:26.000000 yq-3.2.1/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    10273 2017-01-14 17:06:39.000000 yq-3.2.1/LICENSE
--rw-r--r--   0 kislyuk    (501) staff       (20)       41 2019-10-14 14:51:41.000000 yq-3.2.1/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      432 2023-04-05 01:34:39.000000 yq-3.2.1/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     8009 2023-04-05 01:36:45.064249 yq-3.2.1/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     7079 2023-04-05 01:34:39.000000 yq-3.2.1/README.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)      696 2023-04-05 01:34:39.000000 yq-3.2.1/SECURITY.md
--rw-r--r--   0 kislyuk    (501) staff       (20)     2395 2023-04-05 01:34:39.000000 yq-3.2.1/common.mk
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.061169 yq-3.2.1/docs/
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-03 19:16:59.000000 yq-3.2.1/docs/changelog.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)     3430 2023-04-05 01:36:26.000000 yq-3.2.1/docs/cli-doc.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      950 2022-07-03 19:16:59.000000 yq-3.2.1/docs/conf.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      148 2022-08-21 12:28:41.000000 yq-3.2.1/docs/index.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)      263 2023-04-05 01:34:39.000000 yq-3.2.1/pyproject.toml
--rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-04-05 01:36:45.064434 yq-3.2.1/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1676 2023-04-05 01:36:13.000000 yq-3.2.1/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.061989 yq-3.2.1/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)     3468 2022-07-03 19:16:59.000000 yq-3.2.1/test/cfn.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      306 2022-07-03 19:16:59.000000 yq-3.2.1/test/doc.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2022-07-03 19:16:59.000000 yq-3.2.1/test/filter.jq
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    14963 2023-02-22 05:16:29.000000 yq-3.2.1/test/test.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.063274 yq-3.2.1/yq/
--rw-r--r--   0 kislyuk    (501) staff       (20)    13056 2023-04-05 01:34:39.000000 yq-3.2.1/yq/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2023-02-22 05:14:38.000000 yq-3.2.1/yq/__main__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3531 2023-02-22 05:14:38.000000 yq-3.2.1/yq/dumper.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8172 2023-02-22 05:14:38.000000 yq-3.2.1/yq/loader.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5711 2023-02-22 05:14:38.000000 yq-3.2.1/yq/parser.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-04-05 01:36:45.000000 yq-3.2.1/yq/version.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-05 01:36:45.064041 yq-3.2.1/yq.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8009 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)      512 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       63 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/entry_points.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      107 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        3 2023-04-05 01:36:45.000000 yq-3.2.1/yq.egg-info/top_level.txt
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.521258 yq-3.2.2/
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.516099 yq-3.2.2/.github/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       18 2022-07-03 19:16:59.000000 yq-3.2.2/.github/FUNDING.yml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.516335 yq-3.2.2/.github/workflows/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      837 2023-04-05 01:34:39.000000 yq-3.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      477 2022-07-03 19:16:59.000000 yq-3.2.2/.gitignore
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7598 2023-04-22 21:42:12.000000 yq-3.2.2/Changes.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10273 2017-01-14 17:06:39.000000 yq-3.2.2/LICENSE
+-rw-r--r--   0 kislyuk    (501) staff       (20)       41 2019-10-14 14:51:41.000000 yq-3.2.2/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)      432 2023-04-05 01:34:39.000000 yq-3.2.2/Makefile
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8281 2023-04-22 21:42:29.521048 yq-3.2.2/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7351 2023-04-22 21:40:20.000000 yq-3.2.2/README.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)      696 2023-04-05 01:34:39.000000 yq-3.2.2/SECURITY.md
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2395 2023-04-05 01:34:39.000000 yq-3.2.2/common.mk
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.517025 yq-3.2.2/docs/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-03 19:16:59.000000 yq-3.2.2/docs/changelog.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3430 2023-04-22 21:42:12.000000 yq-3.2.2/docs/cli-doc.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      950 2022-07-03 19:16:59.000000 yq-3.2.2/docs/conf.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      148 2022-08-21 12:28:41.000000 yq-3.2.2/docs/index.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)      263 2023-04-05 01:34:39.000000 yq-3.2.2/pyproject.toml
+-rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-04-22 21:42:29.521293 yq-3.2.2/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1676 2023-04-22 21:41:39.000000 yq-3.2.2/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.517676 yq-3.2.2/test/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3468 2022-07-03 19:16:59.000000 yq-3.2.2/test/cfn.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      306 2022-07-03 19:16:59.000000 yq-3.2.2/test/doc.yml
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2022-07-03 19:16:59.000000 yq-3.2.2/test/filter.jq
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    14963 2023-04-22 21:18:23.000000 yq-3.2.2/test/test.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.520285 yq-3.2.2/yq/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    13755 2023-04-22 21:33:06.000000 yq-3.2.2/yq/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)       56 2023-02-22 05:14:38.000000 yq-3.2.2/yq/__main__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3531 2023-02-22 05:14:38.000000 yq-3.2.2/yq/dumper.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8172 2023-02-22 05:14:38.000000 yq-3.2.2/yq/loader.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5911 2023-04-22 21:07:10.000000 yq-3.2.2/yq/parser.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-04-22 21:42:29.000000 yq-3.2.2/yq/version.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 21:42:29.520867 yq-3.2.2/yq.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8281 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)      512 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       63 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/entry_points.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      107 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        3 2023-04-22 21:42:29.000000 yq-3.2.2/yq.egg-info/top_level.txt
```

### Comparing `yq-3.2.1/.github/workflows/ci.yml` & `yq-3.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/Changes.rst` & `yq-3.2.2/Changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Changes for v3.2.2 (2023-04-22)
+===============================
+
+-  Allow XML documents to be streamed with –xml-item-depth
+
 Changes for v3.2.1 (2023-04-04)
 ===============================
 
 -  Relax tomlkit dependency version range to preserve Python 3.6
    compatibility (#165)
 
 Changes for v3.2.0 (2023-04-03)
```

### Comparing `yq-3.2.1/LICENSE` & `yq-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/PKG-INFO` & `yq-3.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.2.1
+Version: 3.2.2
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -128,15 +128,18 @@
 
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
-``xq a.xml b.xml``. Entity expansion and DTD resolution is disabled to avoid XML parsing vulnerabilities.
+``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
+the full doc into memory (for example, stream a `Wikipedia database dump <https://dumps.wikimedia.org>`_ with
+``cat enwiki-*.xml.bz2 | bunzip2 | xq . --xml-item-depth=2``). Entity expansion and DTD resolution is disabled to avoid
+XML parsing vulnerabilities.
 
 TOML support
 ------------
 ``yq`` supports `TOML <https://toml.io/>`_ as well. The ``yq`` package installs an executable, ``tomlq``, which uses the
 `tomlkit library <https://github.com/sdispater/tomlkit>`_ to transcode TOML to JSON, then pipes it to ``jq``. Roundtrip
 transcoding is available with the ``tomlq --toml-output``/``tomlq -t`` option.
```

### Comparing `yq-3.2.1/README.rst` & `yq-3.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,18 @@
 
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
-``xq a.xml b.xml``. Entity expansion and DTD resolution is disabled to avoid XML parsing vulnerabilities.
+``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
+the full doc into memory (for example, stream a `Wikipedia database dump <https://dumps.wikimedia.org>`_ with
+``cat enwiki-*.xml.bz2 | bunzip2 | xq . --xml-item-depth=2``). Entity expansion and DTD resolution is disabled to avoid
+XML parsing vulnerabilities.
 
 TOML support
 ------------
 ``yq`` supports `TOML <https://toml.io/>`_ as well. The ``yq`` package installs an executable, ``tomlq``, which uses the
 `tomlkit library <https://github.com/sdispater/tomlkit>`_ to transcode TOML to JSON, then pipes it to ``jq``. Roundtrip
 transcoding is available with the ``tomlq --toml-output``/``tomlq -t`` option.
```

### Comparing `yq-3.2.1/SECURITY.md` & `yq-3.2.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/common.mk` & `yq-3.2.2/common.mk`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/docs/cli-doc.txt` & `yq-3.2.2/docs/cli-doc.txt`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/docs/conf.py` & `yq-3.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/setup.py` & `yq-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="yq",
-    version="3.2.1",
+    version="3.2.2",
     url="https://github.com/kislyuk/yq",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Command-line YAML/XML processor - jq wrapper for YAML/XML documents",
     long_description=open("README.rst").read(),
     python_requires=">=3.6",
```

### Comparing `yq-3.2.1/test/cfn.yml` & `yq-3.2.2/test/cfn.yml`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/test/test.py` & `yq-3.2.2/test/test.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/yq/__init__.py` & `yq-3.2.2/yq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     output_stream=None,
     input_format="yaml",
     output_format="json",
     program_name="yq",
     width=None,
     indentless_lists=False,
     xml_root=None,
+    xml_item_depth=0,
     xml_dtd=False,
     xml_force_list=frozenset(),
     explicit_start=False,
     explicit_end=False,
     expand_merge_keys=True,
     expand_aliases=True,
     max_expansion_factor=1024,
@@ -238,15 +239,22 @@
                         max_expansion_factor=max_expansion_factor,
                         exit_func=exit_func,
                         prog=program_name,
                     )
                 elif input_format == "xml":
                     import xmltodict
 
-                    doc = xmltodict.parse(input_stream.read(), disable_entities=True, force_list=xml_force_list)
+                    if xml_item_depth != 0:
+                        raise Exception("xml_item_depth is not supported with xq -x")
+
+                    doc = xmltodict.parse(
+                        input_stream.buffer if isinstance(input_stream, io.TextIOWrapper) else input_stream.read(),
+                        disable_entities=True,
+                        force_list=xml_force_list,
+                    )
                     json.dump(doc, json_buffer, cls=JSONDateTimeEncoder)
                     json_buffer.write("\n")
                 elif input_format == "toml":
                     import tomlkit
 
                     doc = tomlkit.load(input_stream)  # type: ignore
                     json.dump(doc, json_buffer, cls=JSONDateTimeEncoder)
@@ -316,20 +324,29 @@
                         max_expansion_factor=max_expansion_factor,
                         exit_func=exit_func,
                         prog=program_name,
                     )
             elif input_format == "xml":
                 import xmltodict
 
+                def emit_entry(path, entry):
+                    json.dump(entry, jq.stdin)  # type: ignore
+                    jq.stdin.write("\n")  # type: ignore
+                    return True
+
                 for input_stream in input_streams:
-                    json.dump(
-                        xmltodict.parse(input_stream.read(), disable_entities=True, force_list=xml_force_list),
-                        jq.stdin,  # type: ignore
+                    doc = xmltodict.parse(
+                        input_stream.buffer if isinstance(input_stream, io.TextIOWrapper) else input_stream.read(),
+                        disable_entities=True,
+                        force_list=xml_force_list,
+                        item_depth=xml_item_depth,
+                        item_callback=emit_entry,
                     )
-                    jq.stdin.write("\n")  # type: ignore
+                    if doc:
+                        emit_entry(None, doc)
             elif input_format == "toml":
                 import tomlkit
 
                 for input_stream in input_streams:
                     json.dump(tomlkit.load(input_stream), jq.stdin, cls=JSONDateTimeEncoder)  # type: ignore
                     jq.stdin.write("\n")  # type: ignore
             else:
```

### Comparing `yq-3.2.1/yq/dumper.py` & `yq-3.2.2/yq/dumper.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/yq/loader.py` & `yq-3.2.2/yq/loader.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.1/yq/parser.py` & `yq-3.2.2/yq/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,41 +34,40 @@
         except Exception:
             pass
 
 
 def get_parser(program_name, description):
     # By default suppress these help strings and only enable them in the specific programs.
     yaml_output_help, yaml_roundtrip_help, width_help, indentless_help, grammar_help = [argparse.SUPPRESS] * 5
-    xml_output_help, xml_dtd_help, xml_root_help, xml_force_list_help = [argparse.SUPPRESS] * 4
+    xml_output_help, xml_item_depth_help, xml_dtd_help, xml_root_help, xml_force_list_help = [argparse.SUPPRESS] * 5
     toml_output_help = argparse.SUPPRESS
 
     if program_name == "yq":
         current_language = "YAML"
         yaml_output_help = "Transcode jq JSON output back into YAML and emit it"
         yaml_roundtrip_help = (
             "Transcode jq JSON output back into YAML and emit it. "
             "Preserve YAML tags and styles by representing them as extra items "
             "in their enclosing mappings and sequences while in JSON. This option "
             "is incompatible with jq filters that do not expect these extra items."
         )
         width_help = "When using --yaml-output, specify string wrap width"
-        indentless_help = "When using --yaml-output, indent block style lists (sequences) " "with 0 spaces instead of 2"
+        indentless_help = "When using --yaml-output, indent block style lists (sequences) with 0 spaces instead of 2"
         grammar_help = (
             "When using --yaml-output, specify output grammar (the default is 1.1 and will be changed "
             "to 1.2 in a future version). Setting this to 1.2 will cause strings like 'on' and 'no' to be "
             "emitted unquoted."
         )
     elif program_name == "xq":
         current_language = "XML"
         xml_output_help = "Transcode jq JSON output back into XML and emit it"
+        xml_item_depth_help = "Specify depth of items to emit (default 0; use a positive integer to stream large docs)"
         xml_dtd_help = "Preserve XML Document Type Definition (disables streaming of multiple docs)"
         xml_root_help = "When transcoding back to XML, envelope the output in an element with this name"
-        xml_force_list_help = (
-            "Tag name to pass to force_list parameter of xmltodict.parse(). " "Can be used multiple times."
-        )
+        xml_force_list_help = "Emit a list for elements with this name even if they occur only once (option can repeat)"
     elif program_name == "tomlq":
         current_language = "TOML"
         toml_output_help = "Transcode jq JSON output back into TOML and emit it"
     else:
         raise Exception("Unknown program name")
 
     description = description.replace("yq", program_name).replace("YAML", current_language)
@@ -103,14 +102,15 @@
     parser.add_argument("--explicit-start", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--explicit-end", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--no-expand-aliases", action="store_false", dest="expand_aliases", help=argparse.SUPPRESS)
     parser.add_argument("--max-expansion-factor", type=int, default=1024, help=argparse.SUPPRESS)
     parser.add_argument(
         "--xml-output", "-x", dest="output_format", action="store_const", const="xml", help=xml_output_help
     )
+    parser.add_argument("--xml-item-depth", type=int, default=0, help=xml_item_depth_help)
     parser.add_argument("--xml-dtd", action="store_true", help=xml_dtd_help)
     parser.add_argument("--xml-root", help=xml_root_help)
     parser.add_argument("--xml-force-list", action="append", help=xml_force_list_help)
     parser.add_argument(
         "--toml-output", "-t", dest="output_format", action="store_const", const="toml", help=toml_output_help
     )
     parser.add_argument("--in-place", "-i", action="store_true", help="Edit files in place (no backup - use caution)")
```

### Comparing `yq-3.2.1/yq.egg-info/PKG-INFO` & `yq-3.2.2/yq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.2.1
+Version: 3.2.2
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -128,15 +128,18 @@
 
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
-``xq a.xml b.xml``. Entity expansion and DTD resolution is disabled to avoid XML parsing vulnerabilities.
+``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
+the full doc into memory (for example, stream a `Wikipedia database dump <https://dumps.wikimedia.org>`_ with
+``cat enwiki-*.xml.bz2 | bunzip2 | xq . --xml-item-depth=2``). Entity expansion and DTD resolution is disabled to avoid
+XML parsing vulnerabilities.
 
 TOML support
 ------------
 ``yq`` supports `TOML <https://toml.io/>`_ as well. The ``yq`` package installs an executable, ``tomlq``, which uses the
 `tomlkit library <https://github.com/sdispater/tomlkit>`_ to transcode TOML to JSON, then pipes it to ``jq``. Roundtrip
 transcoding is available with the ``tomlq --toml-output``/``tomlq -t`` option.
```

### Comparing `yq-3.2.1/yq.egg-info/SOURCES.txt` & `yq-3.2.2/yq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

