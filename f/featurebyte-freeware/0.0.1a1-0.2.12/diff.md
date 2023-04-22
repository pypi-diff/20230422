# Comparing `tmp/featurebyte_freeware-0.0.1a1.tar.gz` & `tmp/featurebyte_freeware-0.2.12-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebyte_freeware-0.0.1a1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

