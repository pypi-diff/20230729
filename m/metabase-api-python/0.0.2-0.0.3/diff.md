# Comparing `tmp/metabase-api-python-0.0.2.tar.gz` & `tmp/metabase_api_python-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-python-0.0.2.tar", last modified: Sat Jul 29 09:43:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

