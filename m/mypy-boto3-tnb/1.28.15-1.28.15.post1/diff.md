# Comparing `tmp/mypy-boto3-tnb-1.28.15.tar.gz` & `tmp/mypy_boto3_tnb-1.28.15.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-tnb-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

