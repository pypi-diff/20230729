# Comparing `tmp/hmsysteme-1.2.tar.gz` & `tmp/hmsysteme-1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmsysteme-1.2.tar", last modified: Sat Jul 29 15:56:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

