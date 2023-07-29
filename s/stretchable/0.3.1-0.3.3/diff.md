# Comparing `tmp/stretchable-0.3.1.tar.gz` & `tmp/stretchable-0.3.3-cp37-abi3-win_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

