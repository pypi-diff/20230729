# Comparing `tmp/SPCEj9bbotw-0.0.1.tar.gz` & `tmp/SPCEj9bbotw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.1.tar", last modified: Sat Jul 29 08:23:13 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.0.2.tar", last modified: Sat Jul 29 08:41:02 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.1.tar` & `SPCEj9bbotw-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:23:13.793681 SPCEj9bbotw-0.0.1/
--rw-rw-rw-   0        0        0       58 2023-07-29 08:23:13.793681 SPCEj9bbotw-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 08:23:13.791681 SPCEj9bbotw-0.0.1/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-07-29 08:23:13.000000 SPCEj9bbotw-0.0.1/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-07-29 08:23:13.000000 SPCEj9bbotw-0.0.1/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 08:23:13.000000 SPCEj9bbotw-0.0.1/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 08:23:13.000000 SPCEj9bbotw-0.0.1/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 08:23:13.793681 SPCEj9bbotw-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-07-29 08:23:05.000000 SPCEj9bbotw-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:41:02.877815 SPCEj9bbotw-0.0.2/
+-rw-rw-rw-   0        0        0       58 2023-07-29 08:41:02.877815 SPCEj9bbotw-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 08:41:02.863812 SPCEj9bbotw-0.0.2/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw/_.py
+-rw-rw-rw-   0        0        0       21 2023-07-29 08:40:09.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw/__init__.py
+-rw-rw-rw-   0        0        0     8306 2023-07-29 08:22:02.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw/kernels.py
+-rw-rw-rw-   0        0        0    14652 2023-07-29 08:40:11.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:41:02.875815 SPCEj9bbotw-0.0.2/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-07-29 08:41:02.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-29 08:41:02.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:41:02.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-29 08:41:02.000000 SPCEj9bbotw-0.0.2/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:41:02.877815 SPCEj9bbotw-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-07-29 08:40:12.000000 SPCEj9bbotw-0.0.2/setup.py
```

