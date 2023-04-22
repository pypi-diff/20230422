# Comparing `tmp/pyspoa-0.0.8a0.tar.gz` & `tmp/pyspoa-0.0.9-cp39-cp39-manylinux_2_24_x86_64.manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspoa-0.0.8a0.tar", last modified: Sat Apr  3 14:24:15 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

