# Comparing `tmp/wizcli-0.1.0.tar.gz` & `tmp/wizcli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizcli-0.1.0.tar", max compression
+gzip compressed data, was "wizcli-0.1.1.tar", max compression
```

## Comparing `wizcli-0.1.0.tar` & `wizcli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.0/README.md
--rw-r--r--   0        0        0      327 2023-04-22 04:07:46.774152 wizcli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1481 2023-04-22 05:18:58.007580 wizcli-0.1.0/wizcli/cli.py
--rw-r--r--   0        0        0     2187 2023-04-22 04:37:46.764498 wizcli-0.1.0/wizcli/wiz.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.1/README.md
+-rw-r--r--   0        0        0      327 2023-04-22 05:31:39.892022 wizcli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1497 2023-04-22 05:31:26.200692 wizcli-0.1.1/wizcli/cli.py
+-rw-r--r--   0        0        0     2187 2023-04-22 04:37:46.764498 wizcli-0.1.1/wizcli/wiz.py
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.1/PKG-INFO
```

### Comparing `wizcli-0.1.0/wizcli/cli.py` & `wizcli-0.1.1/wizcli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 def common(
     ctx: typer.Context,
     host: str = typer.Option(None, "--host", "-h", envvar="WIZ_HOST"),
     port: int = 38899,
     verbose: bool = typer.Option(False, "--verbose", "-v"),
 ):
     if not host:
-        raise typer.Abort("Missing host.")
+        print("Missing host.")
+        raise typer.Abort()
 
     if verbose:
         typer.echo(f"WiZ {host=} {port=}")
 
     ctx.obj = State(
         wiz=Wiz(host, port),
         verbose=verbose
```

### Comparing `wizcli-0.1.0/wizcli/wiz.py` & `wizcli-0.1.1/wizcli/wiz.py`

 * *Files identical despite different names*

### Comparing `wizcli-0.1.0/PKG-INFO` & `wizcli-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizcli
-Version: 0.1.0
+Version: 0.1.1
 Summary: wiz cli
 Author: Agustin B
 Author-email: redraw@sdf.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

