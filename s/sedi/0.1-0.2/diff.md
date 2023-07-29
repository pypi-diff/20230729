# Comparing `tmp/sedi-0.1.tar.gz` & `tmp/sedi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedi-0.1.tar", last modified: Sat Jul 29 11:13:04 2023, max compression
+gzip compressed data, was "sedi-0.2.tar", last modified: Sat Jul 29 11:22:03 2023, max compression
```

## Comparing `sedi-0.1.tar` & `sedi-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:13:04.169593 sedi-0.1/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:13:04.169593 sedi-0.1/PKG-INFO
--rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2440 2023-07-29 11:12:47.000000 sedi-0.1/sed.py
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:13:04.169593 sedi-0.1/sedi.egg-info/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:13:04.000000 sedi-0.1/sedi.egg-info/PKG-INFO
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      158 2023-07-29 11:13:04.000000 sedi-0.1/sedi.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 11:13:04.000000 sedi-0.1/sedi.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       53 2023-07-29 11:13:04.000000 sedi-0.1/sedi.egg-info/entry_points.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        4 2023-07-29 11:13:04.000000 sedi-0.1/sedi.egg-info/top_level.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 11:13:04.169593 sedi-0.1/setup.cfg
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      329 2023-07-29 11:10:03.000000 sedi-0.1/setup.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:22:03.931608 sedi-0.2/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:22:03.931608 sedi-0.2/PKG-INFO
+-rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2478 2023-07-29 11:20:23.000000 sedi-0.2/sed.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:22:03.931608 sedi-0.2/sedi.egg-info/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      158 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       53 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/entry_points.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        4 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/top_level.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 11:22:03.931608 sedi-0.2/setup.cfg
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      329 2023-07-29 11:21:23.000000 sedi-0.2/setup.py
```

### Comparing `sedi-0.1/sed.py` & `sedi-0.2/sed.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,18 @@
 
     # Overwrite the original file with the munged temporary file in a
     # manner preserving file attributes (e.g., permissions).
     shutil.copystat(filename, tmp_file.name)
     shutil.move(tmp_file.name, new_filename)
 
 def main():
+    print("hello world!!!")
     # Do it for Johnny.
-    try: 
-        proc = subprocess.run(["mkdir -p tmp"], shell=True, check=True, capture_output=True)
-        sed_to_file('./etc/regfile.tmp', './tmp/regfile', 'AWS_ACCOUNT', '1234')
-    except Exception as ex:
-        print("error: " + str(ex))
+    # try: 
+    #     proc = subprocess.run(["mkdir -p tmp"], shell=True, check=True, capture_output=True)
+    #     sed_to_file('./etc/regfile.tmp', './tmp/regfile', 'AWS_ACCOUNT', '1234')
+    # except Exception as ex:
+    #     print("error: " + str(ex))
 
 
 if __name__ == "__main__":
     main()
```

