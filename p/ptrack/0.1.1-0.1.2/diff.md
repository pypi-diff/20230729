# Comparing `tmp/ptrack-0.1.1.tar.gz` & `tmp/ptrack-0.1.2-1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrack-0.1.1.tar", last modified: Sat Jul 29 10:18:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

