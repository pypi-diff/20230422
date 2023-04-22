# Comparing `tmp/espeak_phonemizer_windows-1.0.3.post0.tar.gz` & `tmp/espeak_phonemizer_windows-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espeak_phonemizer_windows-1.0.3.post0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

