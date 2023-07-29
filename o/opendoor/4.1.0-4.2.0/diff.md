# Comparing `tmp/opendoor-4.1.0.tar.gz` & `tmp/opendoor-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendoor-4.1.0.tar", last modified: Thu Jul  6 23:02:54 2023, max compression
+gzip compressed data, was "opendoor-4.2.0.tar", last modified: Sat Jul 29 10:15:07 2023, max compression
```

## Comparing `opendoor-4.1.0.tar` & `opendoor-4.2.0.tar`

### file list

```diff
@@ -1,154 +1,157 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.492164 opendoor-4.1.0/
--rw-r--r--   0 admin      (501) staff       (20)    33726 2023-06-25 18:07:26.000000 opendoor-4.1.0/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       85 2023-06-22 22:00:04.000000 opendoor-4.1.0/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)    11582 2023-07-06 23:02:54.491486 opendoor-4.1.0/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)    10419 2023-07-06 22:59:19.000000 opendoor-4.1.0/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.382415 opendoor-4.1.0/data/
--rwxr-xr-x   0 admin      (501) staff       (20)  1031011 2023-07-06 22:58:58.000000 opendoor-4.1.0/data/directories.dat
--rw-r--r--   0 admin      (501) staff       (20)      211 2023-07-06 22:58:58.000000 opendoor-4.1.0/data/ignored.dat
--rwxr-xr-x   0 admin      (501) staff       (20)     5098 2023-06-22 22:00:04.000000 opendoor-4.1.0/data/proxies.dat
--rw-r--r--   0 admin      (501) staff       (20)  2960836 2023-07-06 22:58:58.000000 opendoor-4.1.0/data/subdomains.dat
--rwxr-xr-x   0 admin      (501) staff       (20)     7678 2023-06-22 22:00:04.000000 opendoor-4.1.0/data/useragents.dat
--rwxr-xr-x   0 admin      (501) staff       (20)     1361 2023-06-22 22:00:04.000000 opendoor-4.1.0/opendoor.conf
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.392743 opendoor-4.1.0/opendoor.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    11582 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     3511 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       70 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-26 06:12:20.000000 opendoor-4.1.0/opendoor.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)       76 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       10 2023-07-06 23:02:54.000000 opendoor-4.1.0/opendoor.egg-info/top_level.txt
--rwxr-xr-x   0 admin      (501) staff       (20)     1219 2023-06-22 22:34:55.000000 opendoor-4.1.0/opendoor.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 23:02:54.492396 opendoor-4.1.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     4677 2023-06-27 07:45:40.000000 opendoor-4.1.0/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.396676 opendoor-4.1.0/src/
--rw-r--r--   0 admin      (501) staff       (20)     1414 2023-06-22 22:14:43.000000 opendoor-4.1.0/src/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4958 2023-06-25 21:02:39.000000 opendoor-4.1.0/src/controller.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.398995 opendoor-4.1.0/src/core/
--rw-r--r--   0 admin      (501) staff       (20)     2064 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.401575 opendoor-4.1.0/src/core/color/
--rw-r--r--   0 admin      (501) staff       (20)      708 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/color/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2252 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/color/color.py
--rw-r--r--   0 admin      (501) staff       (20)     4667 2023-06-26 20:14:13.000000 opendoor-4.1.0/src/core/core.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.403865 opendoor-4.1.0/src/core/decorators/
--rw-r--r--   0 admin      (501) staff       (20)      717 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/decorators/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1523 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/decorators/timer.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.406386 opendoor-4.1.0/src/core/filesystem/
--rw-r--r--   0 admin      (501) staff       (20)      718 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/filesystem/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      948 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/filesystem/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     9990 2023-07-05 09:54:30.000000 opendoor-4.1.0/src/core/filesystem/filesystem.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.408214 opendoor-4.1.0/src/core/helper/
--rw-r--r--   0 admin      (501) staff       (20)      710 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/helper/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     5942 2023-07-05 09:52:28.000000 opendoor-4.1.0/src/core/helper/helper.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.414664 opendoor-4.1.0/src/core/http/
--rw-r--r--   0 admin      (501) staff       (20)      828 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2009 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     4423 2023-07-05 05:39:00.000000 opendoor-4.1.0/src/core/http/http.py
--rw-r--r--   0 admin      (501) staff       (20)     5113 2023-06-24 18:19:16.000000 opendoor-4.1.0/src/core/http/https.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.417391 opendoor-4.1.0/src/core/http/plugins/
--rw-r--r--   0 admin      (501) staff       (20)      772 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/plugins/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      953 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/plugins/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.423142 opendoor-4.1.0/src/core/http/plugins/response/
--rw-r--r--   0 admin      (501) staff       (20)     1102 2023-07-05 09:19:24.000000 opendoor-4.1.0/src/core/http/plugins/response/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3415 2023-07-02 21:53:40.000000 opendoor-4.1.0/src/core/http/plugins/response/collation.py
--rw-r--r--   0 admin      (501) staff       (20)     1689 2023-07-02 21:53:40.000000 opendoor-4.1.0/src/core/http/plugins/response/file.py
--rw-r--r--   0 admin      (501) staff       (20)     1701 2023-07-02 21:53:40.000000 opendoor-4.1.0/src/core/http/plugins/response/indexof.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.425532 opendoor-4.1.0/src/core/http/plugins/response/provider/
--rw-r--r--   0 admin      (501) staff       (20)      729 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/plugins/response/provider/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1612 2023-07-05 10:14:28.000000 opendoor-4.1.0/src/core/http/plugins/response/provider/provider.py
--rw-r--r--   0 admin      (501) staff       (20)     1763 2023-07-02 21:53:18.000000 opendoor-4.1.0/src/core/http/plugins/response/skipempty.py
--rw-r--r--   0 admin      (501) staff       (20)     2446 2023-07-06 13:43:16.000000 opendoor-4.1.0/src/core/http/plugins/response/skipsizes.py
--rw-r--r--   0 admin      (501) staff       (20)     1851 2023-07-05 09:59:28.000000 opendoor-4.1.0/src/core/http/plugins/response_plugin.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.432484 opendoor-4.1.0/src/core/http/providers/
--rw-r--r--   0 admin      (501) staff       (20)      865 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/providers/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1868 2023-07-05 04:34:58.000000 opendoor-4.1.0/src/core/http/providers/accept.py
--rw-r--r--   0 admin      (501) staff       (20)     1035 2023-07-04 23:39:25.000000 opendoor-4.1.0/src/core/http/providers/cache.py
--rw-r--r--   0 admin      (501) staff       (20)     1462 2023-07-05 05:34:27.000000 opendoor-4.1.0/src/core/http/providers/cookies.py
--rw-r--r--   0 admin      (501) staff       (20)     2416 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/providers/debug.py
--rw-r--r--   0 admin      (501) staff       (20)     2569 2023-07-04 23:42:07.000000 opendoor-4.1.0/src/core/http/providers/header.py
--rw-r--r--   0 admin      (501) staff       (20)     1847 2023-07-05 05:33:30.000000 opendoor-4.1.0/src/core/http/providers/request.py
--rw-r--r--   0 admin      (501) staff       (20)     5521 2023-07-03 19:25:27.000000 opendoor-4.1.0/src/core/http/providers/response.py
--rw-r--r--   0 admin      (501) staff       (20)     5229 2023-06-24 18:19:22.000000 opendoor-4.1.0/src/core/http/proxy.py
--rw-r--r--   0 admin      (501) staff       (20)     5194 2023-07-04 23:31:48.000000 opendoor-4.1.0/src/core/http/response.py
--rw-r--r--   0 admin      (501) staff       (20)     2149 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/http/socks.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.438778 opendoor-4.1.0/src/core/logger/
--rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4499 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/colorize.py
--rw-r--r--   0 admin      (501) staff       (20)     1832 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/config.py
--rw-r--r--   0 admin      (501) staff       (20)     1754 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/exception.py
--rw-r--r--   0 admin      (501) staff       (20)     2730 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/logger.py
--rw-r--r--   0 admin      (501) staff       (20)     4216 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/logger/rainbow.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.443584 opendoor-4.1.0/src/core/options/
--rw-r--r--   0 admin      (501) staff       (20)      712 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/options/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1651 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/options/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     3987 2023-06-22 22:39:58.000000 opendoor-4.1.0/src/core/options/filter.py
--rw-r--r--   0 admin      (501) staff       (20)    14279 2023-06-22 22:02:04.000000 opendoor-4.1.0/src/core/options/options.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.447545 opendoor-4.1.0/src/core/system/
--rw-r--r--   0 admin      (501) staff       (20)      736 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/system/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      945 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/system/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     2023 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/system/output.py
--rw-r--r--   0 admin      (501) staff       (20)     2887 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/system/process.py
--rw-r--r--   0 admin      (501) staff       (20)     3748 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/core/system/terminal.py
--rw-r--r--   0 admin      (501) staff       (20)      918 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.448213 opendoor-4.1.0/src/lib/
--rw-r--r--   0 admin      (501) staff       (20)     1227 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.455468 opendoor-4.1.0/src/lib/browser/
--rw-r--r--   0 admin      (501) staff       (20)      749 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/browser/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     9761 2023-06-26 09:16:52.000000 opendoor-4.1.0/src/lib/browser/browser.py
--rw-r--r--   0 admin      (501) staff       (20)    10269 2023-07-05 05:09:21.000000 opendoor-4.1.0/src/lib/browser/config.py
--rw-r--r--   0 admin      (501) staff       (20)     6888 2023-07-04 15:18:19.000000 opendoor-4.1.0/src/lib/browser/debug.py
--rw-r--r--   0 admin      (501) staff       (20)     1168 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/browser/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     1336 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/browser/filter.py
--rw-r--r--   0 admin      (501) staff       (20)     3866 2023-06-26 09:21:52.000000 opendoor-4.1.0/src/lib/browser/threadpool.py
--rw-r--r--   0 admin      (501) staff       (20)     2908 2023-06-26 09:15:42.000000 opendoor-4.1.0/src/lib/browser/worker.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.457312 opendoor-4.1.0/src/lib/events/
--rw-r--r--   0 admin      (501) staff       (20)      716 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/events/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      938 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/events/events.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.459751 opendoor-4.1.0/src/lib/io/
--rw-r--r--   0 admin      (501) staff       (20)      755 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/io/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1388 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/io/arguments.py
--rw-r--r--   0 admin      (501) staff       (20)     1174 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/io/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.462095 opendoor-4.1.0/src/lib/package/
--rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/package/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1166 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/package/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     9626 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/package/package.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.465089 opendoor-4.1.0/src/lib/reader/
--rw-r--r--   0 admin      (501) staff       (20)      747 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reader/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      768 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reader/config.py
--rw-r--r--   0 admin      (501) staff       (20)     1162 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reader/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     9530 2023-06-22 22:03:29.000000 opendoor-4.1.0/src/lib/reader/reader.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.467632 opendoor-4.1.0/src/lib/reporter/
--rw-r--r--   0 admin      (501) staff       (20)      753 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      935 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.471622 opendoor-4.1.0/src/lib/reporter/plugins/
--rw-r--r--   0 admin      (501) staff       (20)      963 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1980 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/html.py
--rw-r--r--   0 admin      (501) staff       (20)     1919 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/json.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.473141 opendoor-4.1.0/src/lib/reporter/plugins/provider/
--rw-r--r--   0 admin      (501) staff       (20)      721 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/provider/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2295 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/provider/provider.py
--rw-r--r--   0 admin      (501) staff       (20)     1403 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/std.py
--rw-r--r--   0 admin      (501) staff       (20)     1996 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/reporter/plugins/txt.py
--rw-r--r--   0 admin      (501) staff       (20)     2578 2023-06-26 09:23:46.000000 opendoor-4.1.0/src/lib/reporter/reporter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.476282 opendoor-4.1.0/src/lib/tpl/
--rw-r--r--   0 admin      (501) staff       (20)      737 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/tpl/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4062 2023-07-02 21:50:13.000000 opendoor-4.1.0/src/lib/tpl/config.py
--rw-r--r--   0 admin      (501) staff       (20)     1150 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/tpl/exceptions.py
--rw-r--r--   0 admin      (501) staff       (20)     6678 2023-06-22 22:00:04.000000 opendoor-4.1.0/src/lib/tpl/tpl.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 23:02:54.489940 opendoor-4.1.0/tests/
--rw-r--r--   0 admin      (501) staff       (20)      688 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2947 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_controller.py
--rw-r--r--   0 admin      (501) staff       (20)     1386 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_core_filter.py
--rw-r--r--   0 admin      (501) staff       (20)     3825 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_core_options.py
--rw-r--r--   0 admin      (501) staff       (20)     1228 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_core_terminal.py
--rw-r--r--   0 admin      (501) staff       (20)     8026 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser.py
--rw-r--r--   0 admin      (501) staff       (20)     4153 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser_config.py
--rw-r--r--   0 admin      (501) staff       (20)     3161 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser_debug.py
--rw-r--r--   0 admin      (501) staff       (20)     1877 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser_filter.py
--rw-r--r--   0 admin      (501) staff       (20)     2631 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser_threadpool.py
--rw-r--r--   0 admin      (501) staff       (20)     1463 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_browser_worker.py
--rw-r--r--   0 admin      (501) staff       (20)     1454 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_events.py
--rw-r--r--   0 admin      (501) staff       (20)     4205 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_package.py
--rw-r--r--   0 admin      (501) staff       (20)     9092 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_reader.py
--rw-r--r--   0 admin      (501) staff       (20)     5287 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_reporter.py
--rw-r--r--   0 admin      (501) staff       (20)     5521 2023-06-22 22:00:04.000000 opendoor-4.1.0/tests/test_lib_tpl.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.279091 opendoor-4.2.0/
+-rw-r--r--   0 admin      (501) staff       (20)    33726 2023-06-25 18:07:26.000000 opendoor-4.2.0/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       85 2023-06-22 22:00:04.000000 opendoor-4.2.0/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)    11455 2023-07-29 10:15:07.278386 opendoor-4.2.0/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)    10292 2023-07-29 10:08:33.000000 opendoor-4.2.0/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.172514 opendoor-4.2.0/data/
+-rwxr-xr-x   0 admin      (501) staff       (20)  1030745 2023-07-27 22:19:22.000000 opendoor-4.2.0/data/directories.back.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)  1030867 2023-07-28 22:00:57.000000 opendoor-4.2.0/data/directories.dat
+-rw-r--r--   0 admin      (501) staff       (20)      236 2023-07-25 00:17:07.000000 opendoor-4.2.0/data/ignored.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     5098 2023-06-22 22:00:04.000000 opendoor-4.2.0/data/proxies.dat
+-rw-r--r--   0 admin      (501) staff       (20)  2962131 2023-07-11 00:21:00.000000 opendoor-4.2.0/data/subdomains.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     7678 2023-06-22 22:00:04.000000 opendoor-4.2.0/data/useragents.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     1361 2023-06-22 22:00:04.000000 opendoor-4.2.0/opendoor.conf
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.176948 opendoor-4.2.0/opendoor.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    11455 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     3613 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       70 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-26 06:12:20.000000 opendoor-4.2.0/opendoor.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)       76 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       10 2023-07-29 10:15:07.000000 opendoor-4.2.0/opendoor.egg-info/top_level.txt
+-rwxr-xr-x   0 admin      (501) staff       (20)     1219 2023-06-22 22:34:55.000000 opendoor-4.2.0/opendoor.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-29 10:15:07.279284 opendoor-4.2.0/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     4677 2023-06-27 07:45:40.000000 opendoor-4.2.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.178996 opendoor-4.2.0/src/
+-rw-r--r--   0 admin      (501) staff       (20)     1414 2023-06-22 22:14:43.000000 opendoor-4.2.0/src/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4958 2023-06-25 21:02:39.000000 opendoor-4.2.0/src/controller.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.180524 opendoor-4.2.0/src/core/
+-rw-r--r--   0 admin      (501) staff       (20)     2064 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.181924 opendoor-4.2.0/src/core/color/
+-rw-r--r--   0 admin      (501) staff       (20)      708 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/color/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2252 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/color/color.py
+-rw-r--r--   0 admin      (501) staff       (20)     4721 2023-07-28 10:13:42.000000 opendoor-4.2.0/src/core/core.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.183344 opendoor-4.2.0/src/core/decorators/
+-rw-r--r--   0 admin      (501) staff       (20)      717 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/decorators/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1523 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/decorators/timer.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.185376 opendoor-4.2.0/src/core/filesystem/
+-rw-r--r--   0 admin      (501) staff       (20)      718 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/filesystem/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      948 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/filesystem/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)    10659 2023-07-19 13:38:38.000000 opendoor-4.2.0/src/core/filesystem/filesystem.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.187458 opendoor-4.2.0/src/core/helper/
+-rw-r--r--   0 admin      (501) staff       (20)      710 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/helper/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     5942 2023-07-05 09:52:28.000000 opendoor-4.2.0/src/core/helper/helper.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.193775 opendoor-4.2.0/src/core/http/
+-rw-r--r--   0 admin      (501) staff       (20)      828 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2009 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     4839 2023-07-27 22:33:55.000000 opendoor-4.2.0/src/core/http/http.py
+-rw-r--r--   0 admin      (501) staff       (20)     5501 2023-07-27 22:34:14.000000 opendoor-4.2.0/src/core/http/https.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.196410 opendoor-4.2.0/src/core/http/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)      772 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/plugins/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      953 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/plugins/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.202084 opendoor-4.2.0/src/core/http/plugins/response/
+-rw-r--r--   0 admin      (501) staff       (20)     1102 2023-07-05 09:19:24.000000 opendoor-4.2.0/src/core/http/plugins/response/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3415 2023-07-02 21:53:40.000000 opendoor-4.2.0/src/core/http/plugins/response/collation.py
+-rw-r--r--   0 admin      (501) staff       (20)     1689 2023-07-09 04:57:36.000000 opendoor-4.2.0/src/core/http/plugins/response/file.py
+-rw-r--r--   0 admin      (501) staff       (20)     1701 2023-07-02 21:53:40.000000 opendoor-4.2.0/src/core/http/plugins/response/indexof.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.204339 opendoor-4.2.0/src/core/http/plugins/response/provider/
+-rw-r--r--   0 admin      (501) staff       (20)      729 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/plugins/response/provider/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1612 2023-07-05 10:14:28.000000 opendoor-4.2.0/src/core/http/plugins/response/provider/provider.py
+-rw-r--r--   0 admin      (501) staff       (20)     1760 2023-07-10 11:11:46.000000 opendoor-4.2.0/src/core/http/plugins/response/skipempty.py
+-rw-r--r--   0 admin      (501) staff       (20)     2444 2023-07-10 20:44:15.000000 opendoor-4.2.0/src/core/http/plugins/response/skipsizes.py
+-rw-r--r--   0 admin      (501) staff       (20)     1851 2023-07-05 09:59:28.000000 opendoor-4.2.0/src/core/http/plugins/response_plugin.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.215275 opendoor-4.2.0/src/core/http/providers/
+-rw-r--r--   0 admin      (501) staff       (20)      962 2023-07-27 22:04:39.000000 opendoor-4.2.0/src/core/http/providers/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1703 2023-07-23 21:05:10.000000 opendoor-4.2.0/src/core/http/providers/accept.py
+-rw-r--r--   0 admin      (501) staff       (20)     1035 2023-07-23 18:43:04.000000 opendoor-4.2.0/src/core/http/providers/cache.py
+-rw-r--r--   0 admin      (501) staff       (20)     1077 2023-07-27 22:17:28.000000 opendoor-4.2.0/src/core/http/providers/connection.py
+-rw-r--r--   0 admin      (501) staff       (20)     1462 2023-07-05 05:34:27.000000 opendoor-4.2.0/src/core/http/providers/cookies.py
+-rw-r--r--   0 admin      (501) staff       (20)     2484 2023-07-27 22:30:01.000000 opendoor-4.2.0/src/core/http/providers/debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     2273 2023-07-27 23:54:13.000000 opendoor-4.2.0/src/core/http/providers/header.py
+-rw-r--r--   0 admin      (501) staff       (20)     2110 2023-07-27 22:07:36.000000 opendoor-4.2.0/src/core/http/providers/request.py
+-rw-r--r--   0 admin      (501) staff       (20)     5521 2023-07-09 04:57:55.000000 opendoor-4.2.0/src/core/http/providers/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     1456 2023-07-24 16:55:52.000000 opendoor-4.2.0/src/core/http/providers/user_agent.py
+-rw-r--r--   0 admin      (501) staff       (20)     5634 2023-07-27 22:44:04.000000 opendoor-4.2.0/src/core/http/proxy.py
+-rw-r--r--   0 admin      (501) staff       (20)     5268 2023-07-09 04:58:38.000000 opendoor-4.2.0/src/core/http/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     2149 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/http/socks.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.221629 opendoor-4.2.0/src/core/logger/
+-rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4499 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/colorize.py
+-rw-r--r--   0 admin      (501) staff       (20)     1832 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1754 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)     2730 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/logger.py
+-rw-r--r--   0 admin      (501) staff       (20)     4216 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/logger/rainbow.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.224791 opendoor-4.2.0/src/core/options/
+-rw-r--r--   0 admin      (501) staff       (20)      712 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/options/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1651 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/options/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     3987 2023-06-22 22:39:58.000000 opendoor-4.2.0/src/core/options/filter.py
+-rw-r--r--   0 admin      (501) staff       (20)    14570 2023-07-27 22:12:22.000000 opendoor-4.2.0/src/core/options/options.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.227731 opendoor-4.2.0/src/core/system/
+-rw-r--r--   0 admin      (501) staff       (20)      736 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/system/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      945 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/system/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     2023 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/system/output.py
+-rw-r--r--   0 admin      (501) staff       (20)     2887 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/system/process.py
+-rw-r--r--   0 admin      (501) staff       (20)     3748 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/core/system/terminal.py
+-rw-r--r--   0 admin      (501) staff       (20)      918 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.228297 opendoor-4.2.0/src/lib/
+-rw-r--r--   0 admin      (501) staff       (20)     1227 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.233489 opendoor-4.2.0/src/lib/browser/
+-rw-r--r--   0 admin      (501) staff       (20)      749 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/browser/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     9761 2023-06-26 09:16:52.000000 opendoor-4.2.0/src/lib/browser/browser.py
+-rw-r--r--   0 admin      (501) staff       (20)    10526 2023-07-27 22:15:29.000000 opendoor-4.2.0/src/lib/browser/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     7093 2023-07-27 22:35:00.000000 opendoor-4.2.0/src/lib/browser/debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     1168 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/browser/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     1336 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/browser/filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     3864 2023-07-27 00:01:07.000000 opendoor-4.2.0/src/lib/browser/threadpool.py
+-rw-r--r--   0 admin      (501) staff       (20)     2908 2023-06-26 09:15:42.000000 opendoor-4.2.0/src/lib/browser/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.235147 opendoor-4.2.0/src/lib/events/
+-rw-r--r--   0 admin      (501) staff       (20)      716 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/events/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      938 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/events/events.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.238202 opendoor-4.2.0/src/lib/io/
+-rw-r--r--   0 admin      (501) staff       (20)      755 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/io/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1388 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/io/arguments.py
+-rw-r--r--   0 admin      (501) staff       (20)     1174 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/io/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.240506 opendoor-4.2.0/src/lib/package/
+-rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/package/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1166 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/package/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     9622 2023-07-19 13:41:50.000000 opendoor-4.2.0/src/lib/package/package.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.243959 opendoor-4.2.0/src/lib/reader/
+-rw-r--r--   0 admin      (501) staff       (20)      747 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reader/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      768 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reader/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1162 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reader/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     9533 2023-07-26 20:57:28.000000 opendoor-4.2.0/src/lib/reader/reader.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.247338 opendoor-4.2.0/src/lib/reporter/
+-rw-r--r--   0 admin      (501) staff       (20)      753 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      935 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.256852 opendoor-4.2.0/src/lib/reporter/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)      963 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1980 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/html.py
+-rw-r--r--   0 admin      (501) staff       (20)     1919 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/json.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.258499 opendoor-4.2.0/src/lib/reporter/plugins/provider/
+-rw-r--r--   0 admin      (501) staff       (20)      721 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/provider/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2283 2023-07-09 06:52:10.000000 opendoor-4.2.0/src/lib/reporter/plugins/provider/provider.py
+-rw-r--r--   0 admin      (501) staff       (20)     1403 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/std.py
+-rw-r--r--   0 admin      (501) staff       (20)     1996 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/reporter/plugins/txt.py
+-rw-r--r--   0 admin      (501) staff       (20)     2578 2023-07-09 09:46:31.000000 opendoor-4.2.0/src/lib/reporter/reporter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.262270 opendoor-4.2.0/src/lib/tpl/
+-rw-r--r--   0 admin      (501) staff       (20)      737 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/tpl/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4049 2023-07-27 22:23:55.000000 opendoor-4.2.0/src/lib/tpl/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1150 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/tpl/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     6678 2023-06-22 22:00:04.000000 opendoor-4.2.0/src/lib/tpl/tpl.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-29 10:15:07.277241 opendoor-4.2.0/tests/
+-rw-r--r--   0 admin      (501) staff       (20)      688 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2947 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_controller.py
+-rw-r--r--   0 admin      (501) staff       (20)     1386 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_core_filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     3825 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_core_options.py
+-rw-r--r--   0 admin      (501) staff       (20)     1228 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_core_terminal.py
+-rw-r--r--   0 admin      (501) staff       (20)     8026 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_browser.py
+-rw-r--r--   0 admin      (501) staff       (20)     4153 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_browser_config.py
+-rw-r--r--   0 admin      (501) staff       (20)     3165 2023-07-28 10:14:15.000000 opendoor-4.2.0/tests/test_lib_browser_debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     1877 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_browser_filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     2631 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_browser_threadpool.py
+-rw-r--r--   0 admin      (501) staff       (20)     1463 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_browser_worker.py
+-rw-r--r--   0 admin      (501) staff       (20)     1454 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_events.py
+-rw-r--r--   0 admin      (501) staff       (20)     4205 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_package.py
+-rw-r--r--   0 admin      (501) staff       (20)     9092 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_reader.py
+-rw-r--r--   0 admin      (501) staff       (20)     5287 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_reporter.py
+-rw-r--r--   0 admin      (501) staff       (20)     5521 2023-06-22 22:00:04.000000 opendoor-4.2.0/tests/test_lib_tpl.py
```

### Comparing `opendoor-4.1.0/LICENSE` & `opendoor-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/PKG-INFO` & `opendoor-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendoor
-Version: 4.1.0
+Version: 4.2.0
 Summary: OWASP WEB Directory Scanner
 Home-page: https://github.com/stanislav-web/OpenDoor
 Author: Brain Storm Team
 Author-email: nomail@gmail.com
 Maintainer: Brain Storm Team
 Maintainer-email: nomail@gmail.com
 License: GPL
@@ -51,29 +51,28 @@
 [![Codacy Security Scan](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml)
 [![Codespaces Prebuilds](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds)
 [![Dependency Review](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml)
 [![CodeQL](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql)
 
 [Read The Docs](https://opendoor.readthedocs.io/)
 
-* *Current 4.1.0 (07.07.2023)*
-    - Directories: 83262
+* *Current 4.2.0 (29.07.2023)*
+    - Directories: 83012
     - Subdomains: 255260
   
 #### [Changelog](CHANGELOG.md) (last changes)
-v4.1.0 (07.07.2023) **Gain more power!**
-
--   Added `--sniff skipsizes=25:60:101:...`: allow skipping redirect to 200 OK pages which not found
--   Fix `--sniff skipempty`: increase condition value to detect empty content <= 1000 bytes detect as empty page instead of 100 bytes
--   Fix `ResponseError: Unknown response status : 525`: added to define incorrect SSL handshakes
--   Fix `Object of type HTTPHeaderDictItemView is not JSON serializable`: if `--debug` set `3`
--   Fix response encode failed`('Received response with content-encoding: gzip, but failed to decode it.', error('Error -3 while decompressing data: incorrect header check'))`
--   Added `+20` new directories to internal wordlist
--   Added `+74242` new subdomains to internal wordlist
--   Optimize internal wordlist directories.txt list (sort, removed trash lines)
+v4.2.0 (29.07.2023)
+---------------------------
+- Fixed: `--sniff skipempty,skipsizes=NUM:NUM...` moved pages to ignore in reports instead of just skipping
+- Fixed: invalid response statuses received because of invalid headers were passed
+- Fixed: --accept-cookie param. Now it is working correctly if the server provided Cookies for surfing
+- Optimized `directories_count` and `subdomains_count` operation to reduce RAM usage.
+- Removed: `-262` directories from internal wordlist because of trash
+- Edit Keep-Alive connection type moved to a separate parameter `--keep-alive`
+- Optimized internal wordlist directories.txt list (sort, removed trash lines)
 
 ***Testing of the software on the live commercial systems and organizations is prohibited!***
 
 ![Alt text](http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg "OpenDoor OWASP")
 
 - ✅ directories scanner
 - ✅ subdomains scanner
@@ -175,14 +174,15 @@
   -m METHOD, --method METHOD
                         Request method (use HEAD as default)
   -d DELAY, --delay DELAY
                         Delay between requests threading
   --timeout TIMEOUT     Request timeout (30 sec default)
   -r RETRIES, --retries RETRIES
                         Max retries to reconnect (default 3)
+  --keep-alive          Use keep-alive connection
   --accept-cookies      Accept and route cookies from responses
   --tor                 Using built-in proxylist
   --torlist TORLIST     Path to custom proxylist
   --proxy PROXY         Custom permanent proxy server
   --random-agent        Randomize user-agent per request
 
 Sniff tools:
```

### Comparing `opendoor-4.1.0/README.md` & `opendoor-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,29 +23,28 @@
 [![Codacy Security Scan](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml)
 [![Codespaces Prebuilds](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds)
 [![Dependency Review](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml)
 [![CodeQL](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql)
 
 [Read The Docs](https://opendoor.readthedocs.io/)
 
-* *Current 4.1.0 (07.07.2023)*
-    - Directories: 83262
+* *Current 4.2.0 (29.07.2023)*
+    - Directories: 83012
     - Subdomains: 255260
   
 #### [Changelog](CHANGELOG.md) (last changes)
-v4.1.0 (07.07.2023) **Gain more power!**
-
--   Added `--sniff skipsizes=25:60:101:...`: allow skipping redirect to 200 OK pages which not found
--   Fix `--sniff skipempty`: increase condition value to detect empty content <= 1000 bytes detect as empty page instead of 100 bytes
--   Fix `ResponseError: Unknown response status : 525`: added to define incorrect SSL handshakes
--   Fix `Object of type HTTPHeaderDictItemView is not JSON serializable`: if `--debug` set `3`
--   Fix response encode failed`('Received response with content-encoding: gzip, but failed to decode it.', error('Error -3 while decompressing data: incorrect header check'))`
--   Added `+20` new directories to internal wordlist
--   Added `+74242` new subdomains to internal wordlist
--   Optimize internal wordlist directories.txt list (sort, removed trash lines)
+v4.2.0 (29.07.2023)
+---------------------------
+- Fixed: `--sniff skipempty,skipsizes=NUM:NUM...` moved pages to ignore in reports instead of just skipping
+- Fixed: invalid response statuses received because of invalid headers were passed
+- Fixed: --accept-cookie param. Now it is working correctly if the server provided Cookies for surfing
+- Optimized `directories_count` and `subdomains_count` operation to reduce RAM usage.
+- Removed: `-262` directories from internal wordlist because of trash
+- Edit Keep-Alive connection type moved to a separate parameter `--keep-alive`
+- Optimized internal wordlist directories.txt list (sort, removed trash lines)
 
 ***Testing of the software on the live commercial systems and organizations is prohibited!***
 
 ![Alt text](http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg "OpenDoor OWASP")
 
 - ✅ directories scanner
 - ✅ subdomains scanner
@@ -147,14 +146,15 @@
   -m METHOD, --method METHOD
                         Request method (use HEAD as default)
   -d DELAY, --delay DELAY
                         Delay between requests threading
   --timeout TIMEOUT     Request timeout (30 sec default)
   -r RETRIES, --retries RETRIES
                         Max retries to reconnect (default 3)
+  --keep-alive          Use keep-alive connection
   --accept-cookies      Accept and route cookies from responses
   --tor                 Using built-in proxylist
   --torlist TORLIST     Path to custom proxylist
   --proxy PROXY         Custom permanent proxy server
   --random-agent        Randomize user-agent per request
 
 Sniff tools:
```

### Comparing `opendoor-4.1.0/data/directories.dat` & `opendoor-4.2.0/data/directories.back.dat`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 !images
 !mssql_setup.asp
 !mysql_setup.asp
 !res
 !setup.asp
 !textove_diskuse
 !ut
+%00.cfm
 %3f
 %3f.back
 %3f.bak
 %3f.bak_Edietplus
 %3f.save
 %3f.save1
 %3f.save2
 %3f.save3
 %3f~
 %3f~1~
 %3f~2~
 %3f~3~
 %20..
+%2500.cfm
 0-0-1
 0-12
 -7.php
 0-9.html
 0-a.html
 00-backup
 00-cache
@@ -735,14 +737,15 @@
 .gitCOMMIT_EDITMSG
 .gitconfig
 .gitdescription
 .gitFETCH_HEAD
 .gitHEAD
 .githead
 .github
+.github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/codacy.yml
 .github/workflowsblank.yml
 .github/workflowsci.yml
 .github/workflowsdependabot.yml
 .github/workflowsdocker.yml
 .github/workflowsmaster.yml
 .github/workflowsmaven.yml
@@ -1566,14 +1569,15 @@
 .travis.yml~
 .travisci.yml
 .travisconfig.yml
 .trellix
 .tugboat
 .tvsconfig
 .tx
+.tx/config
 .txconfig
 .txt
 .upload
 .user.ini
 .usermin
 .users
 .vacation.cache
@@ -1927,14 +1931,25 @@
 01.pdf
 1.php
 01.php
 001.php
 1.rar
 1.shtml
 1.sql
+1.sql.7z
+1.sql.bz2
+1.sql.gz
+1.sql.rar
+1.sql.tar
+1.sql.tar.bz2
+1.sql.tar.bzip2
+1.sql.tar.gz
+1.sql.tar.gzip
+1.sql.tgz
+1.sql.zip
 1.swf
 1.tar
 1.tar.bz2
 1.tar.gz
 1.txt
 1.xml
 1.zip
@@ -2711,14 +2726,15 @@
 404-error.html
 404-error.php
 404-error.shtml
 404-forward.aspx
 404-not-found.html
 404-page.aspx
 404-urlrewrite.asp
+404_106321.cfm
 404_error.htm
 404_error.html
 404_error.php
 404_master.phtml
 404_notfound.aspx
 404_page.html
 404_slave.phtml
@@ -6501,14 +6517,16 @@
 _micro
 _misc
 _mm
 _mm.php
 _mmdbscripts
 _mmserverscripts
 _mmServerScripts
+_mmServerScripts/MMHTTPDB.php
+_mmServerScripts/MMSERVERINFO.cfm
 _mmServerScriptsMMHTTPDB.asp
 _mmServerScriptsMMHTTPDB.php
 _mobile
 _mod_files
 _mods
 _modules
 _monopoly
@@ -7289,14 +7307,18 @@
 access.ini
 access.json
 access.log
 access.php
 access.phtml
 access.txt
 access.xml
+access/admin
+access/admin.php
+access/login
+access/login.php
 access_.log
 access_admin
 access_admin.asp
 access_admin.html
 access_admin.php
 access_db
 access_denied.html
@@ -7401,16 +7423,19 @@
 account.lasso
 Account.php
 account.php
 account.phtml
 account.shtml
 account.view
 account/login
+account/login.php
 account/logon
+account/logon.php
 account/signin
+account/signin.php
 account_
 account_bill.php
 account_change.php
 account_check.js.php
 account_checks.php
 account_create.php
 account_created.php
@@ -7473,25 +7498,28 @@
 accountmy
 accountmypro
 accountregistration
 accounts
 Accounts
 accounts.asp
 accounts.cgi
+accounts.dat
 accounts.htm
 accounts.html
 accounts.jsp
 accounts.pdf
 accounts.php
 accounts.pl
 accounts.py
+accounts.rar
 accounts.rb
 accounts.sql
 accounts.txt
 accounts.xml
+accounts.zip
 accounts/login
 accounts/logon
 accounts/signin
 accountsetting.aspx
 accountsettings
 accountsettings.asp
 accountsettings.php
@@ -7889,27 +7917,28 @@
 ad.cgi
 ad.confirm.email
 ad.error
 ad.forget.pass
 ad.htm
 ad.html
 ad.js
-ad.phdo
 ad.php
 ad.swf
 ad/editpage
 ad/html
 ad1
 ad2
 ad2_redirect.asp
 ad2_view.asp
 ad3
 ad1.html
 ad2.html
 ad3.html
+ad_
+ad_.php
 ad_admin.asp
 ad_admin.html
 ad_admin.php
 ad_banner.php
 ad_banner_click.php
 ad_banners
 ad_build.asp
@@ -7924,14 +7953,15 @@
 ad_js.php
 ad_js_display.php
 ad_login
 ad_login.php
 ad_manage
 ad_manage.php
 ad_manager
+ad_manager.php
 Ad_panel.php
 ad_panel.php
 ad_redirect.asp
 ad_server
 ad_tags
 ad_tracker.php
 ad_view.asp
@@ -8499,19 +8529,29 @@
 adm.py
 Adm.rb
 adm.rb
 Adm.shtml
 adm.shtml
 adm/admloginuser
 adm/cms
+adm/cms.php
+adm/cms/login
+adm/cms/login.php
 adm/cmsauth.php
 adm/cmslogin.php
 adm/index
+adm/index.asp
+adm/index.js
+adm/index.php
+adm/index.phtml
 adm/log
+adm/log.dat
+adm/log.log
 adm/login
+adm/login.php
 adm1n
 adm1n.php
 adm2
 adm3
 adm3.php
 adm_auth
 adm_auth.asp
@@ -8523,14 +8563,16 @@
 Adm_auth.php
 adm_auth.phtml
 adm_cp
 adm_login
 adm_manager
 adm_mgmt
 adm_panel
+adm_panel/login
+adm_panel/login.php
 adm_sec
 adm_stat
 admadmin
 admadmloginuser.asp
 admadmloginuser.cfm
 admadmloginuser.cgi
 admadmloginuser.html
@@ -8743,46 +8785,52 @@
 admin.trash.php
 Admin.txt
 admin.txt
 admin.webc
 admin.woa
 admin.zip
 admin/%3bindex
+admin/10_system_support_accounts/index.php
 admin/_logsaccess-log
 admin/_logsaccess.log
 admin/_logsaccess_log
 admin/_logserr.log
 admin/_logserror-log
 admin/_logserror.log
 admin/_logserror_log
 admin/_logslogin.txt
 Admin/Account
 Admin/account
 admin/account
 admin/admin
+admin/admin.php
+admin/admin.html
 admin/admin-login
 admin/admin/login
 admin/admin_login
 admin/adminlogin
 admin/adminLogin
 admin/adminlogin.php
 Admin/auth
+admin/auth
+admin/auth.php
 admin/autoedit
 admin/backup
 admin/backup.rar
 admin/backup.sql
 admin/backup.tar.gz
 admin/backup.txt
 admin/backup.zip
 admin/backups
 admin/cms
 admin/cmseditor
 admin/content/sitetree
 admin/controlpanel
 admin/cp
+admin/cp.php
 admin/css/imagespineapp.ico
 admin/CuteEditor
 admin/daili/webedit
 admin/dailiwebedit
 admin/data
 admin/data.rar
 admin/data.sql
@@ -8856,14 +8904,20 @@
 admin/home.php
 admin/html
 admin/include/htmleditor/admin
 admin/includesconfigure.php
 admin/includesconfigure.php~
 admin/includesconfigure.phtml
 admin/index
+admin/index.asp
+admin/index.cfm?fuseaction=cLogin.main
+admin/index.js
+admin/index.php
+admin/index.php/login/
+admin/index.phtml
 admin/ips.dat
 admin/ips.rar
 admin/ips.tar.gz
 admin/ips.txt
 admin/ips.zip
 admin/js/tiny_mce
 admin/js/tinymce
@@ -8873,18 +8927,23 @@
 Admin/knowledge/dsmgr/usersGroupManager.asp
 Admin/knowledge/dsmgr/usersGroupManager.php
 Admin/knowledge/dsmgr/usersUserManager.asp
 Admin/knowledge/dsmgr/usersUserManager.php
 admin/lavery_Edit
 admin/local
 admin/log
+admin/log.log
 admin/logerror.log
 Admin/login
 admin/login
+admin/login.php
 admin/logs
+admin/logs.php
+admin/logs/log.log
+admin/logs/log.txt
 admin/logsaccess-log
 admin/logsaccess.log
 admin/logsaccess_log
 admin/logserr.log
 admin/logserror-log
 admin/logserror.log
 admin/logserror_log
@@ -8918,28 +8977,31 @@
 admin/privatelogs.txt
 admin/privatelogs.xml
 admin/scripts/fckeditor
 admin/scriptsfckeditor
 admin/scriptsfckeditor.js
 admin/secureadmin.aspx
 admin/securelogon.jsp
+admin/service.php
+admin/settings.php
 admin/sign/in
 admin/signin
 admin/signin.php
 admin/sql.rar
 admin/sql.sql
 admin/sql.tar.gz
 admin/sql.zip
 admin/sqladmin
 admin/sxd
 admin/sysadmin
 admin/templatesedit_pic.html
 admin/tiny_mce/plugins/cyberim
 admin/up
 admin/views/ajax/autocomplete/usera
+admin/visit.php
 admin/web
 admin/webedit
 admin/webedit/editor/filemanager
 admin/WebEditor
 admin/webeditor
 admin/www.zip
 admin1
@@ -9183,14 +9245,20 @@
 admin_board.asp
 admin_board.html
 admin_board.php
 admin_board.xml
 admin_boardset.asp
 admin_boardset.html
 admin_boardset.php
+admin_bot
+admin_bot.php
+admin_bot/admins.php
+admin_bot/index.php
+admin_bot/login.php
+admin_bot/settings.php
 admin_bulkemails.php
 admin_bulkkats.php
 admin_c
 admin_c.php
 admin_cat.asp
 admin_cat.html
 admin_cat.php
@@ -9278,17 +9346,17 @@
 admin_enc_zend.php
 admin_events
 admin_events.php
 admin_expired.asp
 admin_expired.html
 admin_expired.php
 admin_file
-admin_files
 Admin_files
 admin_files.php
+admin_files/admin.html
 admin_folder
 admin_forums.asp
 admin_forums.html
 admin_forums.php
 admin_func.php
 admin_functions.php
 admin_gespro
@@ -9918,14 +9986,15 @@
 adminer-3.4.0.asp
 adminer-3.4.0.php
 adminer-4.0.3.php
 adminer-4.1.0.php
 adminer-4.2.0.php
 adminer-4.2.1.php
 adminer.php
+adminer/index.php
 adminer_coverage.ser
 admineradminer.php
 adminerindex.php
 adminerror.log
 adminerror.txt
 adminerror_log
 adminerrors.log
@@ -10141,32 +10210,43 @@
 administrator/auth
 administrator/backup.rar
 administrator/backup.sql
 administrator/backup.tar.gz
 administrator/backup.txt
 administrator/backup.zip
 administrator/cache
+administrator/components/com_k2/install.mysql.sql
+administrator/components/com_k2/uninstall.mysql.sql
 administrator/data.rar
 administrator/data.sql
 administrator/data.tar.gz
 administrator/data.txt
 administrator/data.zip
 administrator/db
 administrator/enter
 administrator/includes
 administrator/index
+administrator/index.asp
+administrator/index.js
+administrator/index.php
+administrator/index.phtml
 Administrator/login
 administrator/login
+administrator/login.asp
+administrator/login.js
+administrator/login.php
+administrator/login.phtml
 administrator/logs
 administrator/manifests/filesjoomla.xml
 administrator/phpMyAdmin
 administrator/phpmyadmin
 administrator/PMA
 administrator/pma
 administrator/sign
+administrator/sign.php
 administrator/signin
 administrator/web
 administrator2
 administrator2.php
 administrator_center
 administrator_cp
 administrator_login
@@ -12405,20 +12485,23 @@
 api/_swagger_
 api/action
 api/adm
 api/admin
 api/admistrator
 api/apidocsswagger.json
 api/caskgraphql
+api/config
+api/config.json
 api/configbulkedit
 api/configdiff
 api/configrunning_hash
 api/configsave
 api/debugschedlock
 api/devservices
+api/docs
 api/enter
 api/health
 api/healthcheck
 api/incidentsevents
 api/incidentsopen
 api/jsjishigou.js
 api/jsonwsinvoke
@@ -13922,25 +14005,35 @@
 auth.pl
 auth.py
 auth.rb
 auth.tar.gz
 auth.xml
 auth.zip
 auth/adm
+auth/adm.php
 auth/admin
+auth/admin.php
 auth/administrator
 auth/catalogue
 auth/enter
 auth/login
+auth/login.php
 auth/logon
+auth/logon.php
 auth/panel
+auth/panel.php
 auth/pass
+auth/pass.dat
+auth/pass.json
+auth/pass.php
+auth/pass.txt
 auth/password
 auth/shop
 auth/sign
+auth/sign.php
 auth/signin
 auth_ads.php
 auth_ldap.php
 auth_mnet.php
 auth_old.php
 auth_user.php
 auth_user_file.txt
@@ -14020,14 +14113,15 @@
 authorized_keys.txt
 authorizefailed
 authorizenet.log
 authorizenet.php
 authorlist
 authorpic
 authors
+AUTHORS
 authors.aspx
 authors.php
 authors.pwd
 authpanel.php
 authpass
 authpass.json
 authpass.php
@@ -14424,16 +14518,19 @@
 b1n4ry.inc
 b1n4ry.php
 b1n4ry.phtml
 b1n4ry.py
 b1ogindex
 b2
 b2b
+b2b/admin
+b2b/admin.php
 b2b_info_page.php
 b2badmin
+b2badmin.php
 b2c
 b2e
 b2evolution
 b2w
 b3
 b4
 B4ckup
@@ -14503,15 +14600,17 @@
 back-up.php
 back-up.phtml
 back.asp
 back.htm
 back.html
 back.js
 back.php
+back.rar
 back.sql
+back.zip
 back_links.php
 back_office
 back_office.php
 back_up
 backadmin
 backadmin.php
 backadmin/auth
@@ -14596,17 +14695,27 @@
 backup.php
 backup.php4
 backup.php5
 backup.pl
 backup.rar
 backup.sql
 Backup.Sql
+backup.sql.7z
 backup.sql.bz2
 backup.sql.gz
 backup.sql.old
+backup.sql.rar
+backup.sql.sql
+backup.sql.tar
+backup.sql.tar.bz2
+backup.sql.tar.bzip2
+backup.sql.tar.gz
+backup.sql.tar.gzip
+backup.sql.tgz
+backup.sql.zip
 backup.tar
 backup.tar.bz2
 backup.tar.gz
 backup.tgz
 Backup.Tpl
 backup.tpl
 backup.txt
@@ -14651,14 +14760,30 @@
 backups.tar
 backups.tar.bz2
 backups.tar.gz
 backups.tgz
 backups.tpl
 Backups.zip
 backups.zip
+backups/data.sql
+backups/data.tar.gz
+backups/data.txt
+backups/data.zip
+backups/site.rar
+backups/site.tar.gz
+backups/site.zip
+backups/sql.dat
+backups/sql.sql
+backups/sql.tar
+backups/sql.tar.gz
+backups/sql.txt
+backups/sql.zip
+backups/www.rar
+backups/www.tar.gz
+backups/www.zip
 backupsauth.php
 backupsback.dat
 backupsdb
 backupserver
 backupshome.rar
 backupshome.tar
 backupshome.tar.gz
@@ -14751,14 +14876,15 @@
 baker
 baks
 bakup
 balabit
 balance
 balance.html
 balance.php
+balancer-manager
 balances
 baldor
 balinese.html
 ball
 ballowntest.cfm
 baltimore
 bam
@@ -15851,14 +15977,19 @@
 binhostname
 bininstall.dat
 bininstall.js
 bininstall.php
 bininstall.sh
 bininstall.txt
 binky
+bin/cron.sh
+bin/cron.dat
+bin/cron.txt
+bin/install.txt
+bin/install.dat
 binlaunch.js
 binlaunch.php
 binlaunch.sh
 binlibs
 binlog.lib.php
 binreset-db-prod.sh
 binreset-db.sh
@@ -16090,14 +16221,16 @@
 blanky.htm
 blaright.php
 blast
 blasts
 blaxxun
 blaze
 blazeboard
+blazeds/messagebroker/http
+blazeds/messagebroker/httpsecure
 blazeds/messagebrokeramf
 blazeds/messagebrokerhttp
 blazeds/messagebrokerhttpsecure
 blazer
 blazix
 blb
 blc
@@ -16142,14 +16275,17 @@
 blockchain.json
 blockchain.php
 blockchain.rar
 blockchain.sql
 blockchain.tar.gz
 blockchain.txt
 blockchain.zip
+blockchain/admin
+blockchain/admin.js
+blockchain/admin.php
 blocked
 blocked.htm
 blocked.html
 blocked.php
 blockedusers.php
 blockemails.php
 blockform.php
@@ -16348,14 +16484,17 @@
 blue
 blue365.aspx
 bluebird
 bluecat
 bluechat
 bluecoat
 bluedome
+bluedragon.xml
+bluedragon.xml.bak.1
+bluedragon/admin.cfm
 blueface
 bluehouse
 blueprint
 blueprint.html
 blues
 blueshoes
 bluesky
@@ -17146,14 +17285,15 @@
 browsercrm
 browserepos.php
 browsererror.cfm
 browserinfo.asp
 browserinfo.php
 browserreqs.cfm
 browsers
+browserslist
 browserstop.htm
 browsersync
 browsesources.php
 browsetag.php
 browsethreads.aspx
 browsetrees-old.php
 browsetrees.php
@@ -18976,14 +19116,16 @@
 cdata.php
 cdb.php
 cdc
 cdcd
 cde
 c0de
 cdi
+cdkey.dat
+cdkey.txt
 cdm_ggao_tiezi.asp
 cdma
 cdn
 cdomain
 cdonts.asp
 cdontsmail.asp
 cdp
@@ -19165,45 +19307,68 @@
 cf_bulletin.cfc
 cf_calendar.cfm
 cf_nuke
 cfa
 cfa_text_include.js
 cfajax
 cfappman
+cfappman/index.cfm
 cfapps
 cfc
 cfcache
 cfcs
 cfd
 cfdg.php
 cfdocs
 Cfdocs
+cfdocs/cfcache.map
 cferror_request.cfm
 cfexec.cfm
+CFFileServlet/
 cffm
+cfform-internal
 cfform.js
+CFFormGateway/
 cfformprotect
 cffs
 cfg
 cfg.php
 cfg.txt
 cfg/cpp
 cfgectext.cfm
 cfhttp_test.cfm
 cfi
 cfi.html
 CFIDE
 Cfide
 cfide
+CFIDE/adminapi/
 CFIDE/administrator
 CFIDE/Administrator
+CFIDE/Administrator/
 cfide/administratorindex.cfm
 CFIDE/Administratorstartstop.html
+CFIDE/Application.cfm
+CFIDE/debug/
+CFIDE/install.cfm
+CFIDE/installers/
+CFIDE/scripts/
 CFIDE/scripts/ajax/FCKeditor
+CFIDE/scripts/ajax/FCKeditor/editor/dialog/fck_about.html
+CFIDE/scripts/ajax/FCKeditor/editor/dialog/fck_spellerpages/spellerpages/server-scripts/spellchecker.cfm
+CFIDE/scripts/ajax/FCKeditor/editor/filemanager/connectors/cfm/cf5_connector.cfm?command=GetFoldersAndFiles&type=Image&currentFolder=/
+CFIDE/scripts/ajax/FCKeditor/editor/filemanager/connectors/cfm/cf_connector.cfm?command=GetFoldersAndFiles&type=Image&currentFolder=/
+CFIDE/scripts/ajax/FCKeditor/editor/filemanager/upload/cfm/upload.cfm
+CFIDE/scripts/ajax/FCKeditor/fckeditor.cfm
 CFIDE/scripts/ajaxFCKeditor
+CFIDE/scripts/cfform.js
+CFIDE/scripts/css/
+CFIDE/scripts/xsl/
+CFIDE/wizards/
+CFIDE/wizards/common/utils.cfc
 CFIDEadministrator
 CFIDEinstall.cfm
 CFIDEmultiservermonitor-access-policy.xml
 cfincludes
 cfj
 cfkarchive
 cfm
@@ -19219,14 +19384,22 @@
 cfr
 cfs
 cfsearch.cgi
 cftags
 cftest
 cftp
 cfusion
+cfusion/cfapps/forums/data/forums.mdb
+cfusion/cfapps/forums/forums_.mdb
+cfusion/cfapps/security/data/realm.mdb
+cfusion/cfapps/security/realm_.mdb
+cfusion/database/cfexamples.mdb
+cfusion/database/cfsnippets.mdb
+cfusion/database/cypress.mdb
+cfusion/database/smpolicy.mdb
 cfwzjz.html
 cfx
 cg
 cg-bin
 cgame.php
 cgdv.php
 cgi
@@ -19329,14 +19502,15 @@
 cgi.html
 cgi.ini
 cgi.pan
 cgi.php
 cgi.pl
 cgi.pm
 cgi/account
+cgi/cfdocs/expeval/ExprCalc.cfm?
 cgi_bin
 cgi_src
 cgibin
 cgicentral
 cgicommon.cg
 cgicommon.cgi
 cgidir
@@ -19463,14 +19637,15 @@
 CHANGELOG.md
 changelog.md
 CHANGELOG.MD
 ChangeLog.md
 Changelog.md
 CHANGELOG.php
 changelog.php
+CHANGELOG.rst
 CHANGELOG.TXT
 CHANGELOG.txt
 changelog.txt
 ChangeLog.txt
 Changelog.txt
 Changelog.xml
 changelogin.html
@@ -20392,14 +20567,15 @@
 classes
 classes.html
 classes.php
 classes.txt
 classes.zip
 classes.zip,
 classes/gladiusREADME.TXT
+classes/SiteMap.php
 classes/uploadchanges.txt
 classes/uploaddocumentation.htm
 classes/uploadfoto_upload.php
 classes/uploadmultiple_upload_example.php
 classes/uploadupload_db_example.php
 classes/uploadupload_example.php
 classes_gen
@@ -20912,31 +21088,50 @@
 cms.csproj
 CMS.h
 cms.html
 cms.php
 cms.woolovers.com
 cms/_adminlogon.php
 cms/adm
+cms/adm.php
 cms/admin
+cms/admin.php
+cms/admin/__init__.py
+cms/admin/forms.py
+cms/admin/pageadmin.py
+cms/admin/permissionadmin.py
+cms/admin/placeholderadmin.py
+cms/admin/settingsadmin.py
+cms/admin/useradmin.py
 cms/adminindex.php
 cms/administrator
+cms/administrator.php
 cms/ajaxfilemanagerajax_login.php
+cms/api.py
+cms/api
 cms/auth
+cms/auth.php
 cms/componentslogin.ascx
 cms/config/sqlmysql.initial.sql
 cms/enter
 cms/kernel
 cms/kerneladmin.php
 cms/login
+cms/login.html
+cms/login.php
 cms/logs
 cms/logs/weblog
 cms/logsPerfOrgWebLog.log
 cms/logsweb.log
+cms/publisher
 cms/sign
 cms/signin
+cms/templates
+cms/templates/admin
+cms/tests
 cms/themes/cp_themes/default/imagesswfupload.swf
 cms/themes/cp_themes/default/imagesswfupload_f9.swf
 Cms/typo3
 cms1
 cms2
 cms3
 cms4
@@ -21093,31 +21288,31 @@
 cod.php
 cod.redirect
 cod.resultados
 cod.rss_cars
 cod.rss_homes
 cod.rss_jobs
 code
+code.txt
+code.php
 Code
 code-crafters
 code-of-practice
 code.7z
 code.asp
 code.aspx
 code.dat
 code.htm
 code.html
 code.json
-code.php
 code.php3
 code.rar
 code.tar.bz2
 code.tar.gz
 code.tgz
-code.txt
 code.zip
 code2
 code_tree
 code_view.php
 codeavalanche
 codebase
 codebase.php
@@ -21707,14 +21902,15 @@
 comparison.php
 comparison_list
 comparison_list.php
 comparisonpg.asp
 comparisons
 compass
 compass.rb
+compass/logon.jsp
 compasslogon.jsp
 compat
 compat.aspx
 compat.php
 compat.php41x.php
 compat.php42x.php
 compat.php50x.php
@@ -23420,17 +23616,21 @@
 cp.js
 Cp.php
 cp.php
 cp.phtml
 cp.topic.php
 cp.trackback.php
 cp/admin
+cp/admin.php
+cp/logon
 cp/auth
+cp/auth.php
 cp/authorization
 cp/login
+cp/login.php
 cp1.html
 cp_functions.php
 cp_header.php
 cp_view.asp
 cpa
 cpadmin
 cpadmin.aspx
@@ -23452,14 +23652,16 @@
 cpauthorization.php
 cpbackup-exclude.conf
 cpbt.php
 cpc
 cpcommerce
 cpd
 cpdemo
+demo/test.html
+demo/test.php
 cpg
 cpg-nuke
 cpg.aspx
 cpg.php
 cpg_config
 cpl
 cplay
@@ -24108,14 +24310,16 @@
 customer-support
 customer.
 customer.aspx
 customer.cfm
 customer.html
 customer.php
 customer/usersignup
+customer/usersignup.php
+customer/signup.php
 customer2.aspx
 customer404.aspx
 customer_addrma.asp
 customer_care
 customer_home.asp
 customer_images
 customer_info.php
@@ -24562,14 +24766,26 @@
 data.json
 data.jsp
 data.mdb
 data.php
 Data.php
 data.rar
 data.sql
+data.sql.7z
+data.sql.bz2
+data.sql.gz
+data.sql.rar
+data.sql.sql
+data.sql.tar
+data.sql.tar.bz2
+data.sql.tar.bzip2
+data.sql.tar.gz
+data.sql.tar.gzip
+data.sql.tgz
+data.sql.zip
 data.sqlite
 data.tar.bz2
 data.tar.gz
 data.tgz
 data.tsv
 data.txt
 data.xml
@@ -24968,14 +25184,15 @@
 databaseimages.php
 databasemiansha.asp
 databasemiansha.aspx
 databasemiansha.php
 databasems.asp
 databasems.aspx
 databasems.php
+databasenotes.html
 databaseok.asp
 databaseok.aspx
 databaseok.php
 databasep.asp
 databasep.aspx
 databasep.php
 databasephp1.asp
@@ -25301,36 +25518,53 @@
 db-admin.php
 db-admin.phtml
 db-central
 db-full.mysql
 db.
 db.7z
 db.asp
+db.bz2
 db.cgi
 db.class.php
 db.conf
 db.csv
 DB.dat
 db.dat
+db.gz
 db.html
 db.inc
 db.inc.php
 db.ini
 db.log
 db.mdb
 DB.php
 db.php
 Db.properties
 db.rar
 Db.script
 db.sql
+db.sql.7z
+db.sql.bz2
+db.sql.gz
+db.sql.rar
+db.sql.sql
+db.sql.tar
+db.sql.tar.bz2
+db.sql.tar.bzip2
+db.sql.tar.gz
+db.sql.tar.gzip
+db.sql.tgz
+db.sql.zip
 db.sqlite
 db.sqlite3
+db.tar
 db.tar.bz2
+db.tar.bzip2
 db.tar.gz
+db.tar.gzip
 db.tgz
 db.txt
 db.xml
 db.yaml
 db.zip
 db/db-admin
 db/dbadmin
@@ -25376,22 +25610,39 @@
 db1.sqlite
 db2.php
 db__.init.php
 db_access.php
 db_admin
 db_admin.php
 db_backup
+db_backup.7z
+db_backup.bz2
+db_backup.gz
 db_backup.php
 db_backup.rar
 db_backup.sql
+db_backup.sql.7z
 db_backup.sql.bz2
+db_backup.sql.gz
+db_backup.sql.rar
+db_backup.sql.sql
 db_backup.sql.tar
+db_backup.sql.tar.bz2
+db_backup.sql.tar.bzip2
+db_backup.sql.tar.gz
+db_backup.sql.tar.gzip
+db_backup.sql.tgz
+db_backup.sql.zip
 db_backup.tar
+db_backup.tar.bz2
 db_backup.tar.bzip2
 db_backup.tar.gz
+db_backup.tar.gzip
+db_backup.tgz
+db_backup.zip
 db_backups
 db_common.inc.php
 db_config.php
 db_conn
 db_conn.php
 db_connect
 db_connect.php
@@ -25437,24 +25688,71 @@
 dba
 dbaccess.class.php
 dbaccess.log
 dbaccountpage.php3
 dbadm
 dbadm.php
 dbadmin
+dbadmin.7z
+dbadmin.bz2
+dbadmin.gz
 dbadmin.php
 dbadmin.phtml
+dbadmin.rar
+dbadmin.sql
+dbadmin.sql.7z
+dbadmin.sql.bz2
+dbadmin.sql.gz
+dbadmin.sql.rar
+dbadmin.sql.sql
+dbadmin.sql.tar
+dbadmin.sql.tar.bz2
+dbadmin.sql.tar.bzip2
+dbadmin.sql.tar.gz
+dbadmin.sql.tar.gzip
+dbadmin.sql.tgz
+dbadmin.sql.zip
+dbadmin.tar
+dbadmin.tar.bz2
+dbadmin.tar.bzip2
+dbadmin.tar.gz
+dbadmin.tar.gzip
+dbadmin.tgz
+dbadmin.zip
 dbadminaccount.php
 dbadminindex.php
 dbadmins
 dbase
+dbase.7z
+dbase.bz2
+dbase.gz
 dbase.php
 dbase.phtml
+dbase.rar
 dbase.sql
+dbase.sql.7z
+dbase.sql.bz2
+dbase.sql.gz
+dbase.sql.rar
+dbase.sql.sql
+dbase.sql.tar
+dbase.sql.tar.bz2
+dbase.sql.tar.bzip2
+dbase.sql.tar.gz
+dbase.sql.tar.gzip
+dbase.sql.tgz
+dbase.sql.zip
+dbase.tar
+dbase.tar.bz2
+dbase.tar.bzip2
+dbase.tar.gz
+dbase.tar.gzip
+dbase.tgz
 dbase.xml
+dbase.zip
 dbauth
 dbauth.php
 dbback
 dbbackup
 dbbackup.php
 dbbackup.sql
 dbbak.php
@@ -25469,15 +25767,38 @@
 dbconnections.asp
 dbdata.sql
 dbdogaddsibling.php
 dbdoginsert.php
 dbdogupdate.php
 dbdomain.asp
 dbdump
+dbdump.7z
+dbdump.bz2
+dbdump.gz
+dbdump.rar
 dbdump.sql
+dbdump.sql.7z
+dbdump.sql.bz2
+dbdump.sql.gz
+dbdump.sql.rar
+dbdump.sql.sql
+dbdump.sql.tar
+dbdump.sql.tar.bz2
+dbdump.sql.tar.bzip2
+dbdump.sql.tar.gz
+dbdump.sql.tar.gzip
+dbdump.sql.tgz
+dbdump.sql.zip
+dbdump.tar
+dbdump.tar.bz2
+dbdump.tar.bzip2
+dbdump.tar.gz
+dbdump.tar.gzip
+dbdump.tgz
+dbdump.zip
 dbdumper.php
 dbdumps
 dbeditor
 dbef.php
 dbenter.php
 dberror.asp
 dberror.php
@@ -25668,14 +25989,15 @@
 debug.log
 debug.nsf
 debug.php
 debug.py
 debug.seam
 debug.txt
 debug.xml
+debug/default/view
 debug/pprof
 debug/pprofgoroutine?debug=1
 debug/pprofheap
 debug/pprofprofile
 debug/pproftrace
 debug/rusautorisation
 debug_error.jsp
@@ -27122,15 +27444,17 @@
 doc.aspx
 doc.htm
 doc.html
 doc.json
 doc.php
 doc.sh
 doc.txt
+doc/access.txt
 doc/api
+doc/cedentials.txt
 doc/enchanges.html
 doc/htmlindex.html
 doc1
 doc2
 doc3
 doc4
 doc5
@@ -27180,24 +27504,28 @@
 docs.aspx
 docs.dat
 docs.htm
 docs.json
 docs.php
 docs.txt
 docs/_build
+docs/access.txt
 docs/adm
 docs/admin
 docs/administrator
+docs/cedentials.txt
 docs/html/adminch01s04.html
 docs/html/adminch03s07.html
 docs/html/adminch01.html
 docs/html/adminindex.html
 docs/html/developerch03s15.html
 docs/html/developerch02.html
 docs/htmlindex.html
+docs/showtemp.cfm?
+docs/users.txt
 docs1
 docs01
 docs2
 docs02
 docs3
 docs03
 docs4
@@ -27711,14 +28039,15 @@
 dreamdiary
 dreamedit
 dreamedit.php
 dreamedit.sql
 dreamedit/includes/FCKEditor_/editor/filemanager/browser/mcpukbrowser.html
 dreamedit/includes/FCKEditor_/editor/filemanager/uploadtest.html
 dreamedit/login
+dreamedit/login.php
 dreameditlogin.php
 dreameditor
 dreameditor.php
 dreameesoft
 dreamer
 dreamforge
 dreamlevels
@@ -27895,31 +28224,44 @@
 dummy.htm
 dummy.html
 dummy.php
 dummy.txt
 dummypage.aspx
 dump
 dump.7z
+dump.bz2
+dump.gz
 dump.inc
 dump.inc.old
 dump.json
 dump.log
 dump.old
 Dump.php
 dump.php
 dump.rar
 dump.rdb
 dump.sh
 dump.sql
+dump.sql.7z
+dump.sql.bz2
+dump.sql.gz
 dump.sql.old
+dump.sql.tar
+dump.sql.tar.bz2
+dump.sql.tar.bzip2
+dump.sql.tar.gz
+dump.sql.tar.gzip
 dump.sql.tgz
+dump.sql.zip
 dump.sqlite
 dump.tar
 dump.tar.bz2
+dump.tar.bzip2
 dump.tar.gz
+dump.tar.gzip
 dump.tgz
 dump.txt
 dump.zip
 dump/admin
 dump/backup
 dumpadmin.php
 dumpenv
@@ -30984,14 +31326,17 @@
 export.jsp
 export.php
 export.txt
 export.xml
 export_db
 export_excel.php
 export_files
+export_import
+export_import.php
+export_import.phtml
 export_presets.cfg
 export_tags
 export_termin.php
 export_xml.php
 export_yatego.html
 exportcsv.php
 ExportedObj
@@ -31120,14 +31465,17 @@
 extranet.aspx
 extranet.html
 extras
 extras.aspx
 extras.htm
 extras.html
 extras.php
+extras/django_bash_completion
+extras/Makefile
+extras/README.TXT
 extrasdocumentation
 extrasforen
 extrastree.php
 extremail
 extreme
 extremoinfoppv
 extropia
@@ -31451,14 +31799,18 @@
 faqtest.htm
 far
 farben
 farcry
 farerules.aspx
 fares
 farm
+farmanager
+farmanager.asp
+farmanager.php
+farmanager.phtml
 farmer
 farmers_market.aspx
 farmpub
 farsi
 farsinews
 fas
 fashion
@@ -31649,14 +32001,16 @@
 FCKeditor/editor/filemanager/browser/mcpuk
 fckeditor/editor/filemanager/browser/upload/phpupload.php
 FCKeditor/editor/filemanager/connectors
 fckeditor/editor/filemanager/connectors/aspconnector.asp
 fckeditor/editor/filemanager/connectors/aspupload.asp
 fckeditor/editor/filemanager/connectors/aspxconnector.aspx
 fckeditor/editor/filemanager/connectors/aspxupload.aspx
+FCKeditor/editor/filemanager/connectors/cfm/cf5_connector.cfm?command=GetFoldersAndFiles&type=Image&currentFolder=/
+FCKeditor/editor/filemanager/connectors/cfm/cf_connector.cfm?command=GetFoldersAndFiles&type=Image&currentFolder=/
 fckeditor/editor/filemanager/connectors/phpconnector.php
 fckeditor/editor/filemanager/connectors/phpupload.php
 fckeditor/editor/filemanager/connectorstest.html
 FCKeditor/editor/filemanager/connectorsuploadtest.html
 fckeditor/editor/filemanager/upload/aspupload.asp
 fckeditor/editor/filemanager/upload/aspxupload.aspx
 fckeditor/editor/filemanager/upload/phpupload.php
@@ -32525,14 +32879,15 @@
 fitnesstext
 fitxategia
 fitxer
 fitxer1.php
 fitxers
 five
 five.html
+fivecms
 fivefingers.php
 fiveofthebest
 fivepop.cfm
 fivestar
 fiwin
 fix
 fix.html
@@ -32606,14 +32961,15 @@
 flash.htm
 flash.html
 flash.js
 flash.php
 flash.swf
 flash.txt
 flash.xml
+flash/java/javabean/FlashJavaBean.html
 flash2
 flash1.swf
 flash02.swf
 flash_1.swf
 flash_banners
 flash_container.php
 flash_detection.swf
@@ -32641,14 +32997,15 @@
 flashgames
 flashindex.html
 flashobject.js
 flashpeak
 flashplayer
 flashs
 flashservices
+flashservices/gateway
 flashsite
 flashstats
 Flashtest
 flashtest
 flashtesttext
 flashtext
 flashvideo
@@ -32666,14 +33023,20 @@
 fleet.html
 fletch
 fletcher
 flets
 flex
 flex-sign-in
 flex2gateway
+flex2gateway/
+flex2gateway/amf
+flex2gateway/amfpolling
+flex2gateway/cfamfpolling
+flex2gateway/http
+flex2gateway/httpsecure
 flex2gatewayamf
 flex2gatewayamfpolling
 flex2gatewaycfamfpoolling
 flex2gatewayhttp
 flex2gatewayhttpsecure
 flexarms.html
 flexbackup
@@ -33117,14 +33480,16 @@
 form2.asp
 form2.html
 form2.php
 form3.cfm
 form3.php
 form_1.asp
 form_2.asp
+form_auth
+form_auth.php
 form_back
 form_check.js.php
 form_compcert.cfm
 form_confirm.php
 form_contact.inc.php
 form_contact.php
 form_edit.inc.php
@@ -34172,14 +34537,15 @@
 functions_recent.php
 functions_search.php
 functions_users.php
 functions_zip.php
 fund
 fund.html
 funding
+FUNDING.yml
 fundraising
 fundraising_2007
 funds
 funduc
 funerals
 fungi
 fungible
@@ -34816,14 +35182,16 @@
 geologin.php
 geomap.php
 geometry
 geonetwork
 george
 georgia
 georgia.html
+geoserver
+geoserver/web
 geosign.php
 geosignin.php
 geotarget
 geotest.php
 geoTrack
 geovision
 ger
@@ -35808,14 +36176,17 @@
 gprocessnew.jsp
 gproftpd
 gprs
 gprs_search.aspx
 gps
 gps.php
 gpsdrive
+gptbot
+gptbot.js
+gptbot.php
 gpx.php
 gq
 gr
 gr-gb
 gr-qc
 gr.php
 gra
@@ -37275,14 +37646,27 @@
 home.nsf
 home.old
 home.php
 Home.php
 home.phtml
 home.rar
 home.shtml
+home.sql
+home.sql.7z
+home.sql.bz2
+home.sql.gz
+home.sql.rar
+home.sql.sql
+home.sql.tar
+home.sql.tar.bz2
+home.sql.tar.bzip2
+home.sql.tar.gz
+home.sql.tar.gzip
+home.sql.tgz
+home.sql.zip
 home.subscribe
 home.swf
 home.tar
 home.tar.bz2
 home.tar.gz
 home.unsubscribe
 home.xml
@@ -38944,14 +39328,17 @@
 in-portal
 in-the-news
 in.aspx
 in.cgi
 in.htm
 in.jsp
 in.php
+in/login
+in/login.php
+in/wp-login.php
 in2site
 in_dex.html
 in_process
 inactivatejob.asp
 inactive
 inactive.php
 inadmin
@@ -39363,17 +39750,22 @@
 index.wml
 index.xhtml
 index.xml
 index.xml.gz
 index.y
 index.zip
 index/_
+index/admin
+index/admin.js
+index/admin.php
 index/ajaxlang?callback=define&controllername=user
+index/files
 index/userindex.html
 index/userlogin.html
+index/userlogin.php
 index1
 index1a.html
 index1a.php
 index2
 index3
 index5kfreeroll.php
 index1.asp
@@ -41946,14 +42338,15 @@
 jr
 jre
 jref
 jrobot
 jrobottest
 jrobotwww
 jrun
+jrunscripts
 js
 js-global
 js-lib
 js.
 js.asp
 js.aspx
 js.axd
@@ -42013,14 +42406,16 @@
 js_includes/tiny_mce/plugins/ajaxfilemanagerajax_login.php
 js_menu
 js_menu.php
 js_new
 js_old
 js_peels
 js_scripts
+js_tests
+js_tests/tests.html
 jsajax.php
 jsajax_x.js
 jsapi
 jsapi.js
 jsarticle.php
 jsawstats_misc_tracker.js
 jsbase.js
@@ -42125,14 +42520,15 @@
 jssdcms.js
 jsso
 jsspecial.php
 jssresource
 jstester.htm
 jstiny_mce
 jstinymce
+jstl-war/index.html
 jstree
 jswizard.inc.php
 jsx
 jsyndication.aspx
 jsZeroClipboard.swf
 jsZeroClipboard10.swf
 jt
@@ -43305,14 +43701,15 @@
 largerphoto
 largescale
 larkin
 larramendi k.e.
 larry
 larry1
 lars
+larsik/login.php
 lart.php
 larymsecure.php
 las
 las-vegas
 las-vegas.html
 las12345
 lasalle
@@ -43469,24 +43866,31 @@
 lc/systemconsole
 lcaquote.html
 lcb
 lcc.html
 lcc404.html
 lccon6.nsf
 lcdproc
+lcds-samples/messagebroker/http
+lcds-samples/messagebroker/httpsecure
 lcds-samples/messagebrokerhttp
 lcds-samples/messagebrokerhttpsecure
+lcds/messagebroker/http
+lcds/messagebroker/httpsecure
 lcds/messagebrokerhttp
 lcds/messagebrokerhttpsecure
 ld
 ld.php
 ldap
 ldap.php
 ldap.prop
 ldap.prop.sample
+ldap/admin.php
+ldap/login.php
+ldapy
 ldc
 ldccheckmail.aspx
 ldcclaimmail.aspx
 ldi.php
 ldi_check.php
 ldi_table.php
 le
@@ -43964,16 +44368,17 @@
 license.html
 license.inc
 LICENSE.md
 license.md
 license.pdf
 license.php
 LICENSE.php
-license.txt
+LICENSE.python
 LICENSE.txt
+license.txt
 License.txt
 license.xml
 license_afl
 license_afl.txt
 license_ee.txt
 license_key.php
 licenses
@@ -46602,14 +47007,15 @@
 manage_index
 manage_index.php
 manage_login.asp
 manage_login.jsp
 manage_login.php
 manage_main
 manage_main.php
+manage_orders
 manage_page
 manage_web.asp
 manage_web.jsp
 manage_web.php
 manageaccount.asp
 manageaccount.aspx
 manageaddr.cfm
@@ -46662,14 +47068,15 @@
 manager/jmxproxy?invoke=BEANNAME&op=METHODNAME&ps=COMMASEPARATEDPARAMETERS
 manager/jmxproxy?invoke=Catalina%3Atype%3DService&op=findConnectors&ps=
 manager/jmxproxy?qry=STUFF
 manager/jmxproxy?set=BEANNAME&att=MYATTRIBUTE&val=NEWVALUE
 manager/login
 manager/sign
 manager/signin
+manager/status
 manager/statusall
 manager_admin
 manager_laywer.html
 manager_old.php
 manageradmin
 manageradmin.asp
 0manageradmin.asp
@@ -46702,14 +47109,15 @@
 mangas
 mango
 manic
 manica
 MANIFEST
 manifest
 MANIFEST.bak
+MANIFEST.in
 manifest.js
 manifest.json
 MANIFEST.MF
 manifest.mf
 manifest.php
 manifest.xml
 manifest.yml
@@ -47951,14 +48359,16 @@
 message_view.asp
 message_view.php
 messageboard
 messageboard.asp
 messageboard.cfm
 messageboards
 messagebox.php
+messagebroker/http
+messagebroker/httpsecure
 messagebrokeramf
 messagec.php
 messagecenter
 messagecenter.aspx
 messagecentre.ep
 MessageDrivenBeans/docs
 MessageDrivenBeans/docsservlet
@@ -48946,19 +49356,45 @@
 modules
 Modules
 modules.asp
 modules.html
 modules.order
 modules.php
 modules/admin
+modules/articles/admin.php
+modules/bnr/admin.php
+modules/catalog/admin.php
+modules/catsimple/admin.php
+modules/comments/admin.php
+modules/counters/admin.php
+modules/export_import/export_import.php
+modules/export_import/export_import_uni.php
+modules/export_import/import.php
+modules/export_import/ymarket.php
+modules/faq/admin.php
+modules/features/admin.php
+modules/goods/admin.php
+modules/goods/tags.php
+modules/letter/admin.php
+modules/letter/newsletter.php
+modules/letter/settings.php
+modules/makers/admin.php
 modules/mod_socialpinboard_menusaveimagefromupload.php
+modules/news/admin.php
+modules/orders/admin.php
+modules/otzivy/admin.php
+modules/pages/admin.php
+modules/sprav/social.php
+modules/sprav/sprav.php
 modules/TinyMCETinyMCEModuleInfo.asp
 modules/TinyMCETinyMCEModuleInfo.js
 modules/TinyMCETinyMCEModuleInfo.php
+modules/users/admin.php
 modules/vendor/phpunit/phpunitphpunit
+modules/voting/admin.php
 modules2
 modules_admin
 modules_admin.php
 modules_profile
 modulesadmin
 modulesadmin.php
 modulesBackupReplicationApp
@@ -49747,14 +50183,15 @@
 My_admin
 my_admin.php
 my_adminadmin.php
 my_adminauth.php
 my_adminenter.ph
 my_adminlogin.php
 my_ads.php
+my_aj.php
 my_auctions.php
 my_avatar.asp
 my_avatar_show.asp
 my_basket.asp
 my_bids.php
 my_cache
 my_cart.cfm
@@ -50094,33 +50531,43 @@
 mysql
 MYSQL
 MySQL
 mysql tuoku.php
 mysql-admin
 mysql-admin.php
 mysql-adminindex.php
+mysql.7z
 mysql.aspx
 mysql.bak
 mysql.bz2
 mysql.class.php
 mysql.dbi.lib.php
 mysql.err
 mysql.gz
 mysql.html
 mysql.log
 mysql.php
 mysql.rar
 mysql.sql
 mysql.sql.7z
 mysql.sql.bz2
+mysql.sql.gz
+mysql.sql.rar
 mysql.sql.tar
 mysql.sql.tar.bz2
+mysql.sql.tar.bzip2
+mysql.sql.tar.gz
+mysql.sql.tar.gzip
+mysql.sql.tgz
+mysql.sql.zip
 mysql.tar
 mysql.tar.bz2
+mysql.tar.bzip2
 mysql.tar.gz
+mysql.tar.gzip
 mysql.tgz
 mysql.user
 mysql.zip
 mysql/2.x
 mysql/3.x
 mysql/admin
 mysql/db
@@ -51511,14 +51958,15 @@
 nlnl-myoffice.html
 nlogclicks.cfm
 nlogin.php
 nlsubscribers.php
 nm
 nm.php
 nmanagerpro
+nmcms
 nmdeluxe
 nmh
 nmplay.php
 nms
 nmsitemap.jhtml
 Nmtokens.php
 nmvt.cfm
@@ -52046,27 +52494,27 @@
 nukeaddon
 nukebrowser
 nuked-klan
 nukedit
 nukescripts
 nukestyles
 nul
+nul.dbm
 null
+null.dbm
 null.html
 null.htw
 Null.php
 null.php
 null.printer
-nullbranded.tk
 nulllogic
 nullmailer
 nullsoft
 nulo
 num.php
-num9873
 number
 Number.php
 number9
 Numberformat.php
 numberFormat.php
 numbers
 numbers.php
@@ -52146,16 +52594,14 @@
 o.cgi
 o.dat
 o.html
 o.php
 O.php
 o.red
 o.sql
-o.t.a
-o.t.a.
 o.txt
 o.zip
 o2
 o2php
 o8
 o2.cgi
 o3.cgi
@@ -53519,14 +53965,15 @@
 osf
 osg
 osh
 osi.aspx
 osi.html
 osiris
 oskin
+osLes
 osmxperson
 osnov.php
 osp
 ospfd.conf
 osprey.php
 oss
 oss.html
@@ -53947,53 +54394,14 @@
 pag_reg_accesso.php
 pagamento
 pagamento.asp
 pagamento.aspx
 Page
 page
 page,shop.browse
-page,shop.cart
-page-1
-page-2
-page-1.htm
-page-1.html
-page-2.html
-page-3.html
-page-4.html
-page-5.html
-page-6.html
-page-7.html
-page-8.html
-page-9.html
-page-10.html
-page-11.html
-page-12.html
-page-13.html
-page-18.html
-page-21.htm
-page-21.html
-page-22.htm
-page-23.htm
-page-24.htm
-page-24.html
-page-25.htm
-page-26.htm
-page-27.htm
-page-28.htm
-page-29.htm
-page-30.htm
-page-31.htm
-page-32.htm
-page-33.htm
-page-34.htm
-page-35.htm
-page-36.htm
-page-37.htm
-page-38.htm
-page-39.htm
 page-about.html
 page-contact.html
 page-error.aspx
 page-faq.html
 page-info.html
 page-new.php
 page-not-found
@@ -56370,14 +56778,16 @@
 phpunit.php
 phpunit.xml
 phpunit.xml.dist
 phpunit/phpunit/src/Util/PHPeval-stdin.php
 phpunit/phpunit/Util/PHPeval-stdin.php
 phpunit/src/Util/PHPeval-stdin.php
 phpunit/Util/PHPeval-stdin.php
+phpunit_mysql.xml
+phpunit_pgsql.xml
 phpunity
 phpunsharpmask.php
 phpversion.php
 phpWahl
 phpwcms
 phpwcms.php
 phpweather
@@ -59210,839 +59620,14 @@
 progressreports.rss
 progs
 progshadyrestw.pdf
 proguard
 proj
 proj-base
 proj-cms
-proj354.rss
-proj358.rss
-proj360.rss
-proj362.rss
-proj364.rss
-proj372.rss
-proj415.rss
-proj441.rss
-proj485.rss
-proj493.rss
-proj554.rss
-proj565.rss
-proj586.rss
-proj593.rss
-proj607.rss
-proj615.rss
-proj624.rss
-proj628.rss
-proj640.rss
-proj651.rss
-proj655.rss
-proj659.rss
-proj662.rss
-proj663.rss
-proj667.rss
-proj674.rss
-proj683.rss
-proj684.rss
-proj699.rss
-proj714.rss
-proj736.rss
-proj739.rss
-proj757.rss
-proj787.rss
-proj791.rss
-proj803.rss
-proj835.rss
-proj836.rss
-proj876.rss
-proj877.rss
-proj879.rss
-proj880.rss
-proj881.rss
-proj898.rss
-proj921.rss
-proj939.rss
-proj949.rss
-proj951.rss
-proj957.rss
-proj958.rss
-proj980.rss
-proj987.rss
-proj1007.rss
-proj1015.rss
-proj1035.rss
-proj1038.rss
-proj1039.rss
-proj1040.rss
-proj1041.rss
-proj1044.rss
-proj1049.rss
-proj1050.rss
-proj1066.rss
-proj1073.rss
-proj1078.rss
-proj1099.rss
-proj1101.rss
-proj1102.rss
-proj1103.rss
-proj1112.rss
-proj1113.rss
-proj1116.rss
-proj1127.rss
-proj1128.rss
-proj1129.rss
-proj1131.rss
-proj1132.rss
-proj1141.rss
-proj1142.rss
-proj1143.rss
-proj1145.rss
-proj1147.rss
-proj1150.rss
-proj1151.rss
-proj1153.rss
-proj1154.rss
-proj1155.rss
-proj1156.rss
-proj1167.rss
-proj1168.rss
-proj1169.rss
-proj1173.rss
-proj1174.rss
-proj1175.rss
-proj1176.rss
-proj1179.rss
-proj1182.rss
-proj1200.rss
-proj1202.rss
-proj1203.rss
-proj1204.rss
-proj1206.rss
-proj1207.rss
-proj1211.rss
-proj1212.rss
-proj1221.rss
-proj1229.rss
-proj1232.rss
-proj1234.rss
-proj1236.rss
-proj1238.rss
-proj1245.rss
-proj1246.rss
-proj1252.rss
-proj1263.rss
-proj1264.rss
-proj1268.rss
-proj1271.rss
-proj1272.rss
-proj1278.rss
-proj1279.rss
-proj1280.rss
-proj1285.rss
-proj1286.rss
-proj1287.rss
-proj1288.rss
-proj1289.rss
-proj1290.rss
-proj1331.rss
-proj1349.rss
-proj1352.rss
-proj1357.rss
-proj1375.rss
-proj1380.rss
-proj1384.rss
-proj1394.rss
-proj1395.rss
-proj1404.rss
-proj1408.rss
-proj1410.rss
-proj1412.rss
-proj1413.rss
-proj1414.rss
-proj1427.rss
-proj1436.rss
-proj1464.rss
-proj1479.rss
-proj1485.rss
-proj1486.rss
-proj1487.rss
-proj1490.rss
-proj1492.rss
-proj1494.rss
-proj1495.rss
-proj1496.rss
-proj1497.rss
-proj1501.rss
-proj1503.rss
-proj1505.rss
-proj1508.rss
-proj1509.rss
-proj1510.rss
-proj1512.rss
-proj1513.rss
-proj1514.rss
-proj1515.rss
-proj1516.rss
-proj1517.rss
-proj1520.rss
-proj1524.rss
-proj1526.rss
-proj1532.rss
-proj1534.rss
-proj1538.rss
-proj1539.rss
-proj1540.rss
-proj1543.rss
-proj1544.rss
-proj1545.rss
-proj1546.rss
-proj1548.rss
-proj1555.rss
-proj1556.rss
-proj1558.rss
-proj1559.rss
-proj1560.rss
-proj1561.rss
-proj1562.rss
-proj1564.rss
-proj1566.rss
-proj1568.rss
-proj1575.rss
-proj1576.rss
-proj1578.rss
-proj1581.rss
-proj1583.rss
-proj1585.rss
-proj1586.rss
-proj1593.rss
-proj1594.rss
-proj1596.rss
-proj1599.rss
-proj1601.rss
-proj1604.rss
-proj1608.rss
-proj1609.rss
-proj1611.rss
-proj1612.rss
-proj1619.rss
-proj1621.rss
-proj1625.rss
-proj1627.rss
-proj1628.rss
-proj1629.rss
-proj1633.rss
-proj1634.rss
-proj1639.rss
-proj1643.rss
-proj1644.rss
-proj1645.rss
-proj1647.rss
-proj1648.rss
-proj1653.rss
-proj1655.rss
-proj1657.rss
-proj1658.rss
-proj1659.rss
-proj1660.rss
-proj1662.rss
-proj1666.rss
-proj1667.rss
-proj1669.rss
-proj1679.rss
-proj1683.rss
-proj1689.rss
-proj1690.rss
-proj1692.rss
-proj1693.rss
-proj1700.rss
-proj1702.rss
-proj1703.rss
-proj1709.rss
-proj1713.rss
-proj1715.rss
-proj1716.rss
-proj1720.rss
-proj1724.rss
-proj1725.rss
-proj1728.rss
-proj1729.rss
-proj1731.rss
-proj1732.rss
-proj1734.rss
-proj1735.rss
-proj1737.rss
-proj1741.rss
-proj1744.rss
-proj1745.rss
-proj1747.rss
-proj1748.rss
-proj1749.rss
-proj1750.rss
-proj1751.rss
-proj1752.rss
-proj1755.rss
-proj1756.rss
-proj1757.rss
-proj1758.rss
-proj1759.rss
-proj1760.rss
-proj1761.rss
-proj1762.rss
-proj1763.rss
-proj1765.rss
-proj1766.rss
-proj1768.rss
-proj1769.rss
-proj1770.rss
-proj1771.rss
-proj1772.rss
-proj1773.rss
-proj1776.rss
-proj1778.rss
-proj1779.rss
-proj1784.rss
-proj1787.rss
-proj1788.rss
-proj1789.rss
-proj1790.rss
-proj1791.rss
-proj1792.rss
-proj1794.rss
-proj1795.rss
-proj1796.rss
-proj1797.rss
-proj1798.rss
-proj1799.rss
-proj1802.rss
-proj1803.rss
-proj1804.rss
-proj1805.rss
-proj1806.rss
-proj1807.rss
-proj1810.rss
-proj1815.rss
-proj1818.rss
-proj1821.rss
-proj1826.rss
-proj1829.rss
-proj1830.rss
-proj1831.rss
-proj1832.rss
-proj1833.rss
-proj1834.rss
-proj1837.rss
-proj1840.rss
-proj1841.rss
-proj1842.rss
-proj1846.rss
-proj1847.rss
-proj1851.rss
-proj1853.rss
-proj1854.rss
-proj1855.rss
-proj1856.rss
-proj1858.rss
-proj1859.rss
-proj1860.rss
-proj1863.rss
-proj1866.rss
-proj1868.rss
-proj1869.rss
-proj1871.rss
-proj1873.rss
-proj1875.rss
-proj1876.rss
-proj1877.rss
-proj1881.rss
-proj1882.rss
-proj1883.rss
-proj1884.rss
-proj1885.rss
-proj1886.rss
-proj1887.rss
-proj1890.rss
-proj1891.rss
-proj1893.rss
-proj1894.rss
-proj1895.rss
-proj1896.rss
-proj1897.rss
-proj1898.rss
-proj1899.rss
-proj1900.rss
-proj1901.rss
-proj1903.rss
-proj1905.rss
-proj1908.rss
-proj1909.rss
-proj1910.rss
-proj1911.rss
-proj1912.rss
-proj1918.rss
-proj1919.rss
-proj1924.rss
-proj1925.rss
-proj1926.rss
-proj1931.rss
-proj1932.rss
-proj1933.rss
-proj1936.rss
-proj1938.rss
-proj1939.rss
-proj1943.rss
-proj1946.rss
-proj1949.rss
-proj1950.rss
-proj1953.rss
-proj1954.rss
-proj1956.rss
-proj1957.rss
-proj1958.rss
-proj1959.rss
-proj1960.rss
-proj1962.rss
-proj1963.rss
-proj1965.rss
-proj1969.rss
-proj1970.rss
-proj1973.rss
-proj1975.rss
-proj1976.rss
-proj1977.rss
-proj1978.rss
-proj1979.rss
-proj1982.rss
-proj1983.rss
-proj1984.rss
-proj1990.rss
-proj1994.rss
-proj1997.rss
-proj1999.rss
-proj2002.rss
-proj2003.rss
-proj2006.rss
-proj2007.rss
-proj2009.rss
-proj2010.rss
-proj2012.rss
-proj2015.rss
-proj2016.rss
-proj2017.rss
-proj2018.rss
-proj2021.rss
-proj2022.rss
-proj2023.rss
-proj2027.rss
-proj2028.rss
-proj2029.rss
-proj2030.rss
-proj2038.rss
-proj2039.rss
-proj2040.rss
-proj2041.rss
-proj2044.rss
-proj2045.rss
-proj2046.rss
-proj2047.rss
-proj2048.rss
-proj2051.rss
-proj2053.rss
-proj2055.rss
-proj2056.rss
-proj2059.rss
-proj2060.rss
-proj2062.rss
-proj2063.rss
-proj2066.rss
-proj2068.rss
-proj2071.rss
-proj2073.rss
-proj2078.rss
-proj2079.rss
-proj2080.rss
-proj2081.rss
-proj2083.rss
-proj2084.rss
-proj2085.rss
-proj2086.rss
-proj2089.rss
-proj2090.rss
-proj2091.rss
-proj2092.rss
-proj2093.rss
-proj2095.rss
-proj2096.rss
-proj2098.rss
-proj2099.rss
-proj2100.rss
-proj2101.rss
-proj2106.rss
-proj2108.rss
-proj2109.rss
-proj2112.rss
-proj2113.rss
-proj2132.rss
-proj2149.rss
-proj2150.rss
-proj2154.rss
-proj2156.rss
-proj2160.rss
-proj2161.rss
-proj2165.rss
-proj2179.rss
-proj2183.rss
-proj2193.rss
-proj2195.rss
-proj2202.rss
-proj2219.rss
-proj2229.rss
-proj2230.rss
-proj2240.rss
-proj2242.rss
-proj2247.rss
-proj2284.rss
-proj2291.rss
-proj2335.rss
-proj2360.rss
-proj2363.rss
-proj2364.rss
-proj2376.rss
-proj2382.rss
-proj2436.rss
-proj2443.rss
-proj2448.rss
-proj2450.rss
-proj2452.rss
-proj2464.rss
-proj2466.rss
-proj2467.rss
-proj2468.rss
-proj2484.rss
-proj2488.rss
-proj2492.rss
-proj2494.rss
-proj2498.rss
-proj2501.rss
-proj2503.rss
-proj2507.rss
-proj2508.rss
-proj2511.rss
-proj2513.rss
-proj2519.rss
-proj2520.rss
-proj2534.rss
-proj2540.rss
-proj2542.rss
-proj2544.rss
-proj2548.rss
-proj2554.rss
-proj2555.rss
-proj2566.rss
-proj2584.rss
-proj2594.rss
-proj2607.rss
-proj2608.rss
-proj2610.rss
-proj2615.rss
-proj2617.rss
-proj2620.rss
-proj2633.rss
-proj2650.rss
-proj2660.rss
-proj2680.rss
-proj2695.rss
-proj2696.rss
-proj2731.rss
-proj2734.rss
-proj2739.rss
-proj2740.rss
-proj2741.rss
-proj2751.rss
-proj2754.rss
-proj2756.rss
-proj2777.rss
-proj2813.rss
-proj2820.rss
-proj2828.rss
-proj2996.rss
-proj3013.rss
-proj3149.rss
-proj3180.rss
-proj3181.rss
-proj3182.rss
-proj3189.rss
-proj3396.rss
-proj3399.rss
-proj3408.rss
-proj3422.rss
-proj3431.rss
-proj3498.rss
-proj3507.rss
-proj3583.rss
-proj3595.rss
-proj3632.rss
-proj3644.rss
-proj3717.rss
-proj3807.rss
-proj3818.rss
-proj3839.rss
-proj3844.rss
-proj3864.rss
-proj3877.rss
-proj3898.rss
-proj3903.rss
-proj3904.rss
-proj3911.rss
-proj3934.rss
-proj3935.rss
-proj3947.rss
-proj3957.rss
-proj3969.rss
-proj3979.rss
-proj4010.rss
-proj4016.rss
-proj4020.rss
-proj4025.rss
-proj4092.rss
-proj4104.rss
-proj4168.rss
-proj4170.rss
-proj4223.rss
-proj4427.rss
-proj4503.rss
-proj4554.rss
-proj4559.rss
-proj4561.rss
-proj4562.rss
-proj4563.rss
-proj4567.rss
-proj4568.rss
-proj4571.rss
-proj4576.rss
-proj4583.rss
-proj4661.rss
-proj4676.rss
-proj4678.rss
-proj4681.rss
-proj4718.rss
-proj4741.rss
-proj4792.rss
-proj4847.rss
-proj4853.rss
-proj4878.rss
-proj4898.rss
-proj4900.rss
-proj4902.rss
-proj4918.rss
-proj5050.rss
-proj5053.rss
-proj5096.rss
-proj5134.rss
-proj5177.rss
-proj5195.rss
-proj5243.rss
-proj5253.rss
-proj5281.rss
-proj5350.rss
-proj5460.rss
-proj5469.rss
-proj5501.rss
-proj5532.rss
-proj5547.rss
-proj5548.rss
-proj5558.rss
-proj5559.rss
-proj5566.rss
-proj5582.rss
-proj5600.rss
-proj5670.rss
-proj5673.rss
-proj5679.rss
-proj5707.rss
-proj5708.rss
-proj5759.rss
-proj5810.rss
-proj5811.rss
-proj5828.rss
-proj5832.rss
-proj5842.rss
-proj5860.rss
-proj5861.rss
-proj5885.rss
-proj5886.rss
-proj5928.rss
-proj5931.rss
-proj5947.rss
-proj5962.rss
-proj5964.rss
-proj5967.rss
-proj5982.rss
-proj5992.rss
-proj6047.rss
-proj6051.rss
-proj6061.rss
-proj6107.rss
-proj6133.rss
-proj6150.rss
-proj6163.rss
-proj6188.rss
-proj6235.rss
-proj6303.rss
-proj6307.rss
-proj6312.rss
-proj6315.rss
-proj6372.rss
-proj6378.rss
-proj6411.rss
-proj6443.rss
-proj6525.rss
-proj6532.rss
-proj6535.rss
-proj6538.rss
-proj6546.rss
-proj6553.rss
-proj6563.rss
-proj6568.rss
-proj6569.rss
-proj6570.rss
-proj6589.rss
-proj6592.rss
-proj6595.rss
-proj6597.rss
-proj6600.rss
-proj6607.rss
-proj6625.rss
-proj6627.rss
-proj6629.rss
-proj6637.rss
-proj6638.rss
-proj6639.rss
-proj6640.rss
-proj6641.rss
-proj6643.rss
-proj6644.rss
-proj6650.rss
-proj6651.rss
-proj6652.rss
-proj6656.rss
-proj6659.rss
-proj6660.rss
-proj6661.rss
-proj6689.rss
-proj6724.rss
-proj6758.rss
-proj6783.rss
-proj6803.rss
-proj6822.rss
-proj6832.rss
-proj6854.rss
-proj6879.rss
-proj6889.rss
-proj6903.rss
-proj6922.rss
-proj6928.rss
-proj6994.rss
-proj7014.rss
-proj7067.rss
-proj7074.rss
-proj7100.rss
-proj7101.rss
-proj7112.rss
-proj7320.rss
-proj7325.rss
-proj7329.rss
-proj7478.rss
-proj7498.rss
-proj7512.rss
-proj7532.rss
-proj7549.rss
-proj7553.rss
-proj7554.rss
-proj7569.rss
-proj7583.rss
-proj7584.rss
-proj7614.rss
-proj7617.rss
-proj7626.rss
-proj7639.rss
-proj7649.rss
-proj7677.rss
-proj7684.rss
-proj7687.rss
-proj7694.rss
-proj7717.rss
-proj7723.rss
-proj7734.rss
-proj7739.rss
-proj7762.rss
-proj7779.rss
-proj7797.rss
-proj7863.rss
-proj7864.rss
-proj7954.rss
-proj7957.rss
-proj7975.rss
-proj7979.rss
-proj7983.rss
-proj7990.rss
-proj8007.rss
-proj8010.rss
-proj8016.rss
-proj8018.rss
-proj8039.rss
-proj8063.rss
-proj8074.rss
-proj8172.rss
-proj8174.rss
-proj8175.rss
-proj8195.rss
-proj8203.rss
-proj8204.rss
-proj8212.rss
-proj8220.rss
-proj8225.rss
-proj8226.rss
-proj8228.rss
-proj8274.rss
-proj8290.rss
-proj8312.rss
-proj8321.rss
-proj8324.rss
-proj8331.rss
-proj8334.rss
-proj8348.rss
-proj8351.rss
-proj8360.rss
-proj8373.rss
-proj8383.rss
-proj8390.rss
-proj8394.rss
-proj8396.rss
-proj8398.rss
-proj8399.rss
-proj8400.rss
-proj8409.rss
-proj8412.rss
-proj8413.rss
-proj8414.rss
-proj8415.rss
-proj8416.rss
-proj8430.rss
-proj8439.rss
-proj8444.rss
-proj8478.rss
-proj8481.rss
-proj8493.rss
-proj8497.rss
-proj8498.rss
-proj8508.rss
-proj8520.rss
-proj8536.rss
-proj8561.rss
-proj8580.rss
-proj8672.rss
 proj_cord.php
 proj_details.php
 proj_details_new.php
 project
 project-admins
 project-admins.php
 project.cfm
@@ -60504,14 +60089,15 @@
 Public/Scriptsnotexist_path.js
 Public/ScriptsScript.js
 public_admin
 public_bracket.asp
 public_echo.php
 public_ftp
 public_html
+public_html.sql
 public_htmladmin.php
 public_htmllogin.php
 public_htmlrobots.txt
 public_hts
 public_security
 publica
 publicacion
@@ -61247,14 +60833,20 @@
 raiden
 raidenhttpd
 raiders
 rail
 rail.html
 raileurope
 railo-context
+railo-context/admin/server.cfm
+railo-context/admin/web.cfm
+railo-context/templates/display/debugging-console-output.cfm?requestID=1
+railo-context/templates/display/debugging-console-output.cfm?requestID=1&_debug_action=store
+railo-context/templates/display/debugging-console.cfm
+railo-context/test.cfm
 rails
 rails.php
 rails/infoproperties
 railsactions
 railway
 rain
 rainbow
@@ -63494,14 +63086,15 @@
 revistas
 revitol.html
 revival
 revize
 revogames
 revolution
 revolver
+revshell.php
 revuepresse.asp
 reward
 rewards
 rewards-program
 rewrite
 rewrite.asp
 rewrite.php
@@ -64583,14 +64176,16 @@
 sampleposteddata.php
 samplereports
 samples
 samples.htm
 samples.html
 samples.php
 samples/activitysessions
+samples/messagebroker/http
+samples/messagebroker/httpsecure
 samples/messagebrokeramf
 samples/messagebrokerhttp
 samples/messagebrokerhttpsecure
 samplesactivitysessions
 samplesactivitysessions.php
 SamplesGallery
 samplesite
@@ -65119,14 +64714,16 @@
 script-solution.de
 script-www
 script.
 script.js
 script.php
 script.shtml
 script.txt
+script/databases/makered.mdb
+script/databases/makered97.mdb
 script/jqueryplugins/dataTables/extras/TableTools/media/swfZeroClipboard.swf
 script_index.html
 script_library
 scriptaculous
 scriptaculous.js
 scriptconf
 scriptcontent
@@ -65160,18 +64757,21 @@
 scripts/ckeditor/ckfinder/core/connector/aspxconnector.aspx
 scripts/ckeditor/ckfinder/core/connector/phpconnector.php
 scripts/fckeditor/editor/filemanager
 scripts/fckeditor/editor/filemanager/browser/defaultbrowser.html
 scripts/fckeditor/editorfckdialog.html
 scripts/iisadmin/ism.dll?httpdir
 scripts/iisadminism.dll
+scripts/install-npm-dependencies.sh
 scripts/js/fckeditor/editor/filemanager/connectorstest.html
 scripts/kcfinder
 scripts/kcfinder/upload
+scripts/manage_translations.py
 scripts/root.exe?c+dir
+scripts/rpm-install.sh
 scripts/samples
 scripts/samples/searchwebhits.exe
 scripts/tiny_mce
 scripts/tiny_mce/plugins/ajaxfilemanagerajax_login.php
 scripts/tiny_mce/plugins/ajaxfilemanagerajaxfilemanager.php
 scripts/tinymce
 scripts/toolsgetdrvs.exe
@@ -65368,15 +64968,14 @@
 search3.html
 search3.php
 search4.php
 search5.html
 search97cgi
 search123
 search2000
-search?fulltext=1&search_submit=Search
 search_
 search_a9.cgi
 search_ad.php
 search_add.php
 search_admin
 search_admin.php
 search_advanced.asp
@@ -65914,14 +65513,15 @@
 seite_15.php
 seiten
 Seitenframes
 sejour
 sejour-quick.htm
 sel
 seladdr.cfm
+seladmin
 seladresse.php
 selecciona.asp
 selecciona2.asp
 select
 select.asp
 select.aspx
 select.htm
@@ -66724,24 +66324,26 @@
 setup
 Setup
 setup-config.php
 setup.
 setup.asp
 setup.aspx
 setup.bat
+setup.cfg
 setup.data
 setup.exe
 setup.htm
 setup.html
 setup.inc
 setup.log
 setup.mvc
 setup.nsf
 Setup.php
 setup.php
+setup.py
 setup.sql
 setup.txt
 setup.xml
 setup/admin
 setup/build
 setup_info.php
 setup_info_class.php
@@ -67067,14 +66669,15 @@
 shop-bin
 shop-checkout.html
 shop-script
 shop.asp
 shop.aspx
 shop.axd
 shop.cards
+shop.cart
 shop.cgi
 shop.dll
 shop.htm
 shop.html
 shop.jsp
 shop.old
 shop.orders
@@ -67129,14 +66732,17 @@
 shop_image
 shop_info.php
 shop_inventory.php
 shop_iteminfo.php
 shop_msgclear.php
 shop_old
 shop_quickorder.asp
+shop_registration
+shop_registration.html
+shop_registration.php
 shop_renewal.asp
 shop_test
 shopa_upload.asp
 shopa_ups_track.asp
 shopaccess.php
 shopad
 shopaddtocart.asp
@@ -68024,14 +67630,25 @@
 site.js
 site.master
 site.master.cs
 site.old
 site.php
 site.rar
 site.sql
+site.sql.7z
+site.sql.bz2
+site.sql.gz
+site.sql.rar
+site.sql.tar
+site.sql.tar.bz2
+site.sql.tar.bzip2
+site.sql.tar.gz
+site.sql.tar.gzip
+site.sql.tgz
+site.sql.zip
 site.swf
 site.tar
 site.tar.bz2
 site.tar.gz
 site.txt
 site.xml
 site.zip
@@ -68629,14 +68246,15 @@
 slurpconfirm404
 sm
 sm.html
 sm.php
 sm5
 sm_cancelled.php
 sm_completed.php
+sm_ctmpl
 sma
 smail
 smail.php
 small
 small-business
 small_image
 smallbusiness
@@ -68662,14 +68280,15 @@
 smarterror.aspx
 smartertools
 smartfeed.php
 smartfeed_url.php
 smartforce
 smartftp
 smarthtml
+SmarTicketApp/index.html
 SmartImage.class.php
 smartimage.php
 SmartIRC.php
 smartisoft
 smartline
 smartlink.js
 smartlist
@@ -69395,14 +69014,15 @@
 spezial
 spgpartenaires
 sphera
 sphider
 sphider-1.3.4
 sphider-1.3.5
 sphinx
+sphinxapi.php
 sphiro
 sphome.php
 sphpblog
 spi
 spice
 spid
 spidean
@@ -69574,28 +69194,43 @@
 sql-admin
 sql-admin.php
 sql-ledger
 sql.7z
 sql.asp
 sql.aspx
 SQL.aspx
+sql.bz2
 sql.class.php
 sql.db
+sql.gz
 sql.htm
 sql.html
 sql.inc
 sql.log
 sql.php
 SQL.php
 sql.php3
 sql.rar
 sql.sql
+sql.sql.7z
+sql.sql.bz2
+sql.sql.gz
+sql.sql.rar
+sql.sql.tar
+sql.sql.tar.bz2
+sql.sql.tar.bzip2
+sql.sql.tar.gz
+sql.sql.tar.gzip
+sql.sql.tgz
+sql.sql.zip
 sql.tar
 sql.tar.bz2
+sql.tar.bzip2
 sql.tar.gz
+sql.tar.gzip
 sql.tgz
 sql.txt
 sql.zip
 sql/adm
 sql/admin
 sql/administrator
 sql/auth
@@ -71509,14 +71144,15 @@
 sx_recommander.asp
 sxcarto.asp
 sxd
 sxd/backup
 sxdpro
 sxema
 sy
+sy3
 syas
 sybari
 sybase
 sybergen
 sybex
 sybil
 syconos
@@ -72342,14 +71978,15 @@
 technicalStaff.php
 technicalStaffEN.php
 technico.txt
 techniek
 technik
 technique
 technique-print.htm
+techniques/servlets/index.html
 techno
 techno.htm
 technologies
 technologies.
 technologies.asp
 technology
 Technology
@@ -72583,14 +72220,25 @@
 temp.html
 TEMP.ini
 TEMP.json
 TEMP.php
 temp.php
 temp.rar
 temp.sql
+temp.sql.7z
+temp.sql.bz2
+temp.sql.gz
+temp.sql.rar
+temp.sql.tar
+temp.sql.tar.bz2
+temp.sql.tar.bzip2
+temp.sql.tar.gz
+temp.sql.tar.gzip
+temp.sql.tgz
+temp.sql.zip
 temp.tar
 temp.tar.bz2
 temp.tar.gz
 temp.tbz
 temp.tgz
 TEMP.txt
 TEMP.xml
@@ -72940,14 +72588,20 @@
 test.sql
 test.sqlite
 test.swf
 test.txt
 test.woa
 test.xml
 test.zip
+test/admin
+test/admin.html
+test/admin.php
+test/administrator
+test/administrator.html
+test/administrator.php
 test/tmp
 test/version_tmp
 test1
 test01
 test2
 test3
 test4
@@ -73193,14 +72847,19 @@
 tests
 TESTS
 Tests
 tests.html
 tests.jsf
 tests.php
 tests/unit
+tests/wsgi
+tests/wsgi/__init__.py
+tests/wsgi/tests.py
+tests/wsgi/urls.py
+tests/wsgi/wsgi.py
 testsearch
 testsearch.asp
 testsearch.htm
 testseite
 testseite.html
 testserver
 testsessions.php
@@ -74499,14 +74158,15 @@
 tovary.html
 tovers
 tower
 towerblog
 town
 town.php
 towns
+tox.ini
 toxic
 toxmlrpc.inc.php
 toxsoft
 toy-story
 toyota
 toys
 toys-cart.aspx
@@ -74655,14 +74315,17 @@
 trade-traffic
 trade.asp
 trade.cgi
 trade.htm
 trade.html
 trade.notify.php
 trade.php
+trade/admin
+trade/admin.aspx
+trade/admin.php
 trade2.html
 trade_offer.php
 tradedoubler
 tradedoubler.jsp
 tradefiles
 tradehistory.asp
 tradein-form.htm
@@ -74848,14 +74511,15 @@
 travel.php
 travel_plans
 travelagents
 traveler
 travelers
 Travelling.php
 travellinks.htm
+travelnet/home.jsp
 travelnow
 travelpod-roll.flv
 travels
 travelscape
 travelstart
 travers
 travian
@@ -75813,14 +75477,15 @@
 upcoming.php
 upd
 update
 update-core.php
 update-links.php
 update-profile.aspx
 update-rss.php
+update-v
 update.action
 update.asp
 update.aspx
 update.cgi
 update.dat
 update.htm
 update.html
@@ -75937,21 +75602,21 @@
 upgrade.htm
 upgrade.html
 UPGRADE.php
 upgrade.php
 upgrade.pl
 upgrade.readme
 UPGRADE.txt
+UPGRADE.md
 upgrade.txt
 upgrade.xml
 upgrade_config.php
 UPGRADE_README.txt
 upgradeapi.php
 upgradelog.xml
-UpgradeLog.XML
 upgradelog2.xml
 upgradeplan.php
 upgrades
 upgradestep1.asp
 upguard
 upimages
 upimages.php
@@ -75982,14 +75647,26 @@
 upload.inc
 upload.jsp
 upload.php
 Upload.php
 upload.php3
 upload.shtm
 upload.shtml
+upload.sql
+upload.sql.7z
+upload.sql.bz2
+upload.sql.gz
+upload.sql.rar
+upload.sql.tar
+upload.sql.tar.bz2
+upload.sql.tar.bzip2
+upload.sql.tar.gz
+upload.sql.tar.gzip
+upload.sql.tgz
+upload.sql.zip
 upload.txt
 upload/admin
 upload/administrator
 upload/files/upload/filescmd.asp
 upload/files/upload/filescmd.php
 upload/files1.asp
 upload/files1.aspx
@@ -76479,14 +76156,15 @@
 uploads.aspx
 uploads.cfm
 uploads.htm
 uploads.html
 uploads.php
 uploads.php3
 uploads.shtm
+uploads/Flash
 uploads2
 uploads_admin
 uploads_admin.php
 uploads_event
 uploads_forum
 uploads_group
 uploads_user
@@ -77323,35 +77001,56 @@
 userreview.php
 userrights
 userrss.php
 userrss2.php
 users
 Users
 users-m-auth.html
+users.7z
 users.asp
 users.aspx
+users.bz2
 users.cgi
 users.class.php
 users.csv
 users.dat
 users.db
+users.gz
 users.htm
 users.html
 users.inc
 users.ini
 users.json
 users.log
 users.mdb
 users.php
 users.pwd
+users.rar
 users.sql
+users.sql.7z
+users.sql.bz2
 users.sql.gz
+users.sql.rar
+users.sql.tar
+users.sql.tar.bz2
+users.sql.tar.bzip2
+users.sql.tar.gz
+users.sql.tar.gzip
+users.sql.tgz
+users.sql.zip
 users.sqlite
+users.tar
+users.tar.bz2
+users.tar.bzip2
+users.tar.gz
+users.tar.gzip
+users.tgz
 users.txt
 users.xls
+users.zip
 users/admin
 users/Editer
 users/login
 users_actions.php
 users_add.php
 users_birthdays.php
 users_files
@@ -77570,23 +77269,25 @@
 v.html
 v.php
 V.php
 v.sql
 v.zip
 v/admin
 v1
+v1/logger.json
 v1/publicyql
 v1/test/jsconsole.html
 v1/test/jsconsole_ajax.js
 v1api-doc
 v1api-docs
 v1scheduler
 v1swagger.json
 v2
 v2/keys?recursive=true
+v2/logger.json
 v2_basket.php
 v2_catalog
 v2_play_song.php
 v2_search.php
 v2api-doc
 v2api-docs
 v2b
@@ -78163,14 +77864,16 @@
 vestern
 vestiges.html
 vetrina.php
 veure
 vf
 vfend
 vfg
+vfm-admin
+vfm-admin.php
 vfolder.ghp
 vforum
 vfs
 vg
 vg1
 vg_image.php
 vgn
@@ -79112,14 +78815,16 @@
 wacha
 wachtwoord.html
 wackowiki
 wadbsearch
 wadmin
 wadmin.php
 waer.html
+waf.json
+waf.xml
 wagner
 wahm
 wai
 wais
 waistcoat.aspx
 wait.aspx
 wait.htm
@@ -79547,14 +79252,16 @@
 WEB-INF/spring-configpresentation-config.xml
 WEB-INF/spring-configservices-config.xml
 WEB-INF/spring-configservices-remote-config.xml
 WEB-INF/spring-configurationfilters.xml
 WEB-INF/springwebmvc-config.xml
 WEB-INF/src
 WEB-INF/strutsstruts-config.xml
+WEB-INF/web.xml
+WEB-INF/webapp.properties
 WEB-INFapplication-client.xml
 WEB-INFapplication_config.xml
 WEB-INFapplicationContext.xml
 WEB-INFbeans.xml
 WEB-INFcas-servlet.xml
 WEB-INFcas.properties
 WEB-INFclasses
@@ -79675,14 +79382,25 @@
 web.php
 web.rar
 web.Release.config
 web.root
 Web.sitemap
 web.sitemap
 web.sql
+web.sql.7z
+web.sql.bz2
+web.sql.gz
+web.sql.rar
+web.sql.tar
+web.sql.tar.bz2
+web.sql.tar.bzip2
+web.sql.tar.gz
+web.sql.tar.gzip
+web.sql.tgz
+web.sql.zip
 web.tar
 web.tar.bz2
 web.tar.gz
 web.tgz
 web.xml
 web.zip
 web/adminlogin
@@ -79757,29 +79475,30 @@
 webaccess
 webacoo.inc
 webacoo.php
 webacoo.phtml
 webacoo.py
 webad
 webadm
+webadm.php
 webadmin
+webadmin.php
 WebAdmin
 Webadmin
 webadmin.
 webadmin.asp
 webadmin.aspx
 webadmin.cfm
 webadmin.cgi
 webadmin.html
 Webadmin.html
 webadmin.inc
 webadmin.js
 webadmin.jsp
 webadmin.nsf
-webadmin.php
 WebAdmin.php
 Webadmin.php
 webadmin.phtml
 webadmin.py
 webadmin/admin
 WebAdmin/Editor
 webadmin/htmledit
@@ -80358,14 +80077,15 @@
 welcome.cfm
 welcome.cgi?p=logo
 welcome.htm
 welcome.html
 welcome.jsp
 welcome.msg
 welcome.php
+welcome.phtml
 welcome.shtml
 welcome1.php
 welcome2.php
 welcome_ads
 welcome_old.php
 welcomeback
 welcomeback.php
@@ -80981,14 +80701,16 @@
 world.kokuken
 world.php
 world2
 world_flags
 world_map.cgi
 worldcup
 worldgroup
+worldmusic/action/catalog
+worldmusic/action/cdlist
 worldpay
 worldpay.aspx
 worldpay.php
 worldpayreturn
 worldpayreturn.aspx
 worldvision
 worldwide
@@ -81854,14 +81576,16 @@
 wps
 wps/cmis_proxy/http/www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg247798.html?Logout&RedirectTo=http:/example.com
 wps/common_proxy/http/www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg247798.html?Logout&RedirectTo=http:/example.com
 wps/contenthandler/!ut/p/digest!8skKFbWr_TwcZcvoc9Dn3g/?uri=http://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg247798.html?Logout&RedirectTo=http:/example.com
 wps/myproxy/http/www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg247798.html?Logout&RedirectTo=http:/example.com
 wps/PA_WCM_Authoring_UI/proxy/httpexample.com
 wps/PA_WCM_Authoring_UI/proxy/httpsexample.com
+wps/portal/login
+wps/portal/login.php
 wps/proxy/http/www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/sg247798.html?Logout&RedirectTo=http:/example.com
 wpscripts
 wptest
 wpthumbnails
 wptouch.php
 wpwp-login.php
 wqsb
@@ -81920,14 +81644,15 @@
 writings
 wroclaw-hotele.php
 wrong_rules.php
 wrong_section.php
 wrt
 ws
 ws-client
+ws-client/loanCalculation.jsp
 ws.php
 ws.zip
 ws2
 ws2004/Public
 ws_admin
 WS_FTP
 ws_ftp
@@ -81979,14 +81704,15 @@
 wsoshell.inc
 wsoshell.php
 wsoshell.phtml
 wsoshell.py
 wsp
 wsr.aspx
 wsr.php
+WSRPProducer/
 wss
 WSsamples
 wsscxt.html
 wstat
 wstat7
 wstats
 wstats.php
@@ -82040,14 +81766,26 @@
 www.aral-design.de
 www.key
 www.kutxa.net-en
 www.log
 www.php
 www.rar
 www.sql
+www.sql.7z
+www.sql.bz2
+www.sql.gz
+www.sql.rar
+www.sql.sql
+www.sql.tar
+www.sql.tar.bz2
+www.sql.tar.bzip2
+www.sql.tar.gz
+www.sql.tar.gzip
+www.sql.tgz
+www.sql.zip
 www.st-patricks.com
 www.tar
 www.tar.bz2
 www.tar.gz
 www.tgz
 www.txuri-urdin.com
 www.web-teck.com
@@ -83250,13 +82988,13 @@
 萧萧asp大马超强版.asp
 虚拟机提权大马.asp
 说明.txt
 超强版 大.aspa
 超强版.asp
 转换字符的一句话a.asp
 过狗asp一句话.asp
-邪恶十进制 大.asa
+邪恶十进制 大.asp
 配置文档.txt
 项目配置文档.txt
 预编译出错shell.aspx
 风云专用.asp
 黑客动画吧 专用免杀版.asp
```

### Comparing `opendoor-4.1.0/data/proxies.dat` & `opendoor-4.2.0/data/proxies.dat`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/data/subdomains.dat` & `opendoor-4.2.0/data/subdomains.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 0
 00
 000
 0000
 00000
 000000
+*
 0-search
 0-www
 1
 01
 001
 0001
 00001
@@ -4677,15 +4678,111 @@
 11192521404255
 11285521401250
 11290521402560
 60427579112530
 6041506118703183
 574540296544344000
 574540296544344112
+_afpovertcp._tcp
+_aix._tcp
+_autodiscover._tcp
+_caldav._tcp
+_certificates._tcp
+_cisco-phone-http
+_cisco-phone-tftp
+_cisco-uds._tcp
+_ciscowtp._tcp
+_client._smtp
+_client._smtp._tcp
+_cmp._tcp
+_collab-edge._tls
+_crl._tcp
+_crls._tcp
+_cuplogin._tcp
 _domainkey
+_finger._tcp
+_ftp
+_ftp._tcp
+_gc._tcp
+_h323be._tcp
+_h323be._udp
+_h323cs._tcp
+_h323cs._udp
+_h323ls._tcp
+_h323ls._udp
+_h323rs._tcp
+_h323rs._udp
+_hkp._tcp
+_hkps._tcp
+_http._tcp
+_https._tcp
+_imap._tcp
+_imap.tcp
+_jabber
+_jabber-client._tcp
+_jabber-client._udp
+_jabber._tcp
+_jabber._udp
+_kerberos._tcp
+_kerberos._tcp.dc._msdcs
+_kerberos._udp
+_kerberos.tcp.dc._msdcs
+_kpasswd._tcp
+_kpasswd._udp
+_ldap._tcp
+_ldap._tcp.dc._msdcs
+_ldap._tcp.ForestDNSZones
+_ldap._tcp.gc._msdcs
+_ldap._tcp.pdc._msdcs
+_mysqlsrv._tcp
+_nfs
+_nntp._tcp
+_ntp
+_ntp._udp
+_ocsp._tcp
+_pgpkeys._tcp
+_pgprevokations._tcp
+_pkixrep._tcp
+_pop3s._tcp
+_pop3._tcp
+_pptp
+_rdp._tcp
+_sftp._tcp
+_sip
+_sip._tcp
+_sip._tcp.internal
+_sip._tls
+_sip._udp
+_sipfederationtls._tcp
+_sipinternal._tcp
+_sipinternaltls._tcp
+_sips._tcp
+_smtp._tcp
+_snmp
+_snmp
+_snmp._udp
+_sql._tcp
+_ssh._tcp
+_stun._tcp
+_stun._udp
+_svcp._tcp
+_tcp
+_telnet._tcp
+_test._tcp
+_tls
+_udp
+_vlmcs._tcp
+_vlmcs._udp
+_whois._tcp
+_wpad._tcp
+_xmpp-client._tcp
+_xmpp-client._udp
+_xmpp-server
+_xmpp-server._tcp
+_xmpp-server._udp
 a
 0a
 a0
 a00
 a-24
 a-b-c-flowers
 a-bipolar
@@ -80273,14 +80370,15 @@
 gbs
 gbs7071
 gbt
 gburg
 gburns
 gc
 gc-_msdcs
+gc._msdcs
 gc1
 gc2
 gc9ye
 gc552
 gc2006
 gca
 gcapps-jp
@@ -107607,14 +107705,15 @@
 ipumu
 ipv4
 ipv4add6
 ipv4with6
 ipv6
 ipv6-teredo
 ipv6test
+ipv6.teredo
 ipvax
 ipw
 ipx
 ipxgw
 ipxpress
 ipxrouter
 iq
```

### Comparing `opendoor-4.1.0/data/useragents.dat` & `opendoor-4.2.0/data/useragents.dat`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/opendoor.conf` & `opendoor-4.2.0/opendoor.conf`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/opendoor.egg-info/PKG-INFO` & `opendoor-4.2.0/opendoor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendoor
-Version: 4.1.0
+Version: 4.2.0
 Summary: OWASP WEB Directory Scanner
 Home-page: https://github.com/stanislav-web/OpenDoor
 Author: Brain Storm Team
 Author-email: nomail@gmail.com
 Maintainer: Brain Storm Team
 Maintainer-email: nomail@gmail.com
 License: GPL
@@ -51,29 +51,28 @@
 [![Codacy Security Scan](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codacy.yml)
 [![Codespaces Prebuilds](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/codespaces/create_codespaces_prebuilds)
 [![Dependency Review](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/dependency-review.yml)
 [![CodeQL](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/stanislav-web/OpenDoor/actions/workflows/github-code-scanning/codeql)
 
 [Read The Docs](https://opendoor.readthedocs.io/)
 
-* *Current 4.1.0 (07.07.2023)*
-    - Directories: 83262
+* *Current 4.2.0 (29.07.2023)*
+    - Directories: 83012
     - Subdomains: 255260
   
 #### [Changelog](CHANGELOG.md) (last changes)
-v4.1.0 (07.07.2023) **Gain more power!**
-
--   Added `--sniff skipsizes=25:60:101:...`: allow skipping redirect to 200 OK pages which not found
--   Fix `--sniff skipempty`: increase condition value to detect empty content <= 1000 bytes detect as empty page instead of 100 bytes
--   Fix `ResponseError: Unknown response status : 525`: added to define incorrect SSL handshakes
--   Fix `Object of type HTTPHeaderDictItemView is not JSON serializable`: if `--debug` set `3`
--   Fix response encode failed`('Received response with content-encoding: gzip, but failed to decode it.', error('Error -3 while decompressing data: incorrect header check'))`
--   Added `+20` new directories to internal wordlist
--   Added `+74242` new subdomains to internal wordlist
--   Optimize internal wordlist directories.txt list (sort, removed trash lines)
+v4.2.0 (29.07.2023)
+---------------------------
+- Fixed: `--sniff skipempty,skipsizes=NUM:NUM...` moved pages to ignore in reports instead of just skipping
+- Fixed: invalid response statuses received because of invalid headers were passed
+- Fixed: --accept-cookie param. Now it is working correctly if the server provided Cookies for surfing
+- Optimized `directories_count` and `subdomains_count` operation to reduce RAM usage.
+- Removed: `-262` directories from internal wordlist because of trash
+- Edit Keep-Alive connection type moved to a separate parameter `--keep-alive`
+- Optimized internal wordlist directories.txt list (sort, removed trash lines)
 
 ***Testing of the software on the live commercial systems and organizations is prohibited!***
 
 ![Alt text](http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg "OpenDoor OWASP")
 
 - ✅ directories scanner
 - ✅ subdomains scanner
@@ -175,14 +174,15 @@
   -m METHOD, --method METHOD
                         Request method (use HEAD as default)
   -d DELAY, --delay DELAY
                         Delay between requests threading
   --timeout TIMEOUT     Request timeout (30 sec default)
   -r RETRIES, --retries RETRIES
                         Max retries to reconnect (default 3)
+  --keep-alive          Use keep-alive connection
   --accept-cookies      Accept and route cookies from responses
   --tor                 Using built-in proxylist
   --torlist TORLIST     Path to custom proxylist
   --proxy PROXY         Custom permanent proxy server
   --random-agent        Randomize user-agent per request
 
 Sniff tools:
```

### Comparing `opendoor-4.1.0/opendoor.egg-info/SOURCES.txt` & `opendoor-4.2.0/opendoor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 opendoor.conf
 opendoor.py
 setup.py
+data/directories.back.dat
 data/directories.dat
 data/ignored.dat
 data/proxies.dat
 data/subdomains.dat
 data/useragents.dat
 opendoor.egg-info/PKG-INFO
 opendoor.egg-info/SOURCES.txt
@@ -47,19 +48,21 @@
 src/core/http/plugins/response/skipempty.py
 src/core/http/plugins/response/skipsizes.py
 src/core/http/plugins/response/provider/__init__.py
 src/core/http/plugins/response/provider/provider.py
 src/core/http/providers/__init__.py
 src/core/http/providers/accept.py
 src/core/http/providers/cache.py
+src/core/http/providers/connection.py
 src/core/http/providers/cookies.py
 src/core/http/providers/debug.py
 src/core/http/providers/header.py
 src/core/http/providers/request.py
 src/core/http/providers/response.py
+src/core/http/providers/user_agent.py
 src/core/logger/__init__.py
 src/core/logger/colorize.py
 src/core/logger/config.py
 src/core/logger/exception.py
 src/core/logger/logger.py
 src/core/logger/rainbow.py
 src/core/options/__init__.py
```

### Comparing `opendoor-4.1.0/opendoor.py` & `opendoor-4.2.0/opendoor.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/setup.py` & `opendoor-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/__init__.py` & `opendoor-4.2.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/controller.py` & `opendoor-4.2.0/src/controller.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/__init__.py` & `opendoor-4.2.0/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/color/__init__.py` & `opendoor-4.2.0/src/core/color/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/color/color.py` & `opendoor-4.2.0/src/core/color/color.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/core.py` & `opendoor-4.2.0/src/core/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,27 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
+fVersion = open('VERSION', 'r+').readline().rstrip()
 
 CoreConfig = {
     'info': {
         'name': 'Opendoor scanner',
         'repository': 'git@github.com:stanislav-web/OpenDoor.git',
         'remote_version': 'https://raw.githubusercontent.com/stanislav-web/OpenDoor/master/VERSION',
         'license': 'License: GNU General Public License',
-        'version': '4.0.6',
+        'version': fVersion,
         'documentation': 'https://opendoor.readthedocs.org',
         'required_versions': {
             'minor': '3.7',
-            'major': '3.10'
+            'major': '3.11'
         },
     },
     'data': {
         'directories': 'data/directories.dat',
         'ignored': 'data/ignored.dat',
         'proxies': 'data/proxies.dat',
         'subdomains': 'data/subdomains.dat',
```

### Comparing `opendoor-4.1.0/src/core/decorators/__init__.py` & `opendoor-4.2.0/src/core/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/decorators/timer.py` & `opendoor-4.2.0/src/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/filesystem/__init__.py` & `opendoor-4.2.0/src/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/filesystem/exceptions.py` & `opendoor-4.2.0/src/core/filesystem/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/filesystem/filesystem.py` & `opendoor-4.2.0/src/core/filesystem/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,19 +243,39 @@
         filepath = os.path.join(filename)
 
         if not os.path.isfile(filepath):
             raise FileSystemError("{0} is not a file ".format(filename))
         if not os.access(filepath, os.R_OK):
             raise FileSystemError("Configuration file {0} can not be read. Setup chmod 0644".format(filepath))
 
-        with open(filepath) as f_handler:
+        with open(filepath, 'r') as f_handler:
             data = f_handler.readlines()
         return data
 
     @staticmethod
+    def count_lines(filename):
+        """
+        Count lines in .txt file
+        :param str filename: input filename
+        :raise FileSystemError
+        :return: list
+        """
+
+        filepath = os.path.join(filename)
+
+        if not os.path.isfile(filepath):
+            raise FileSystemError("{0} is not a file ".format(filename))
+        if not os.access(filepath, os.R_OK):
+            raise FileSystemError("Configuration file {0} can not be read. Setup chmod 0644".format(filepath))
+        with open(filepath, 'r') as f_handler:
+            for count, line in enumerate(f_handler):
+                pass
+        return count + 1
+
+    @staticmethod
     def readcfg(filename):
         """
         Read .cfg file
         :param str filename: input filename
         :raise FileSystemError
         :return: configparser.RawConfigParser
         """
```

### Comparing `opendoor-4.1.0/src/core/helper/__init__.py` & `opendoor-4.2.0/src/core/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/helper/helper.py` & `opendoor-4.2.0/src/core/helper/helper.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/__init__.py` & `opendoor-4.2.0/src/core/http/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/exceptions.py` & `opendoor-4.2.0/src/core/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/http.py` & `opendoor-4.2.0/src/core/http/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,18 @@
         :param src.lib.browser.config.Config config: global configurations
         :param DebugProvider debug: debugger
         """
 
         try:
             self.__tpl = kwargs.get('tpl')
             RequestProvider.__init__(self, config, agent_list=kwargs.get('agent_list'))
-
+            self.__headers = self._headers
+            self.__connection_header = 'default'
+            if True is config.keep_alive:
+                self.__connection_header = self._keep_alive
         except (TypeError, ValueError) as error:
             raise HttpRequestError(error)
 
         self.__cfg = config
         self.__debug = debug
 
         if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
@@ -58,40 +61,43 @@
         try:
             pool = HTTPConnectionPool(self.__cfg.host,
                                       port=self.__cfg.port,
                                       maxsize=self.__cfg.threads,
                                       timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
                                       block=True)
             if self._HTTP_DBG_LEVEL <= self.__debug.level:
-                self.__debug.debug_connection_pool('http_pool_start', pool)
+                self.__debug.debug_connection_pool('http_pool_start', pool, self.__connection_header)
             return pool
         except Exception as error:
             raise HttpRequestError(str(error))
 
     def request(self, url):
         """
         Client request HTTP
         :param str url: request uri
         :return: urllib3.HTTPResponse
         """
 
+        self.__headers.update({'User-Agent': self._user_agent})
+        if 'default' is not self.__connection_header:
+            self.__headers.update({'Connection': self.__connection_header})
         if self._HTTP_DBG_LEVEL <= self.__debug.level:
-            self.__debug.debug_request(self._headers, url, self.__cfg.method)
+            self.__debug.debug_request(self.__headers, url, self.__cfg.method)
         try:
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
                 response = self.__pool.request(self.__cfg.method,
                                                helper.parse_url(url).path,
-                                               headers=self._headers,
+                                               headers=self.__headers,
                                                retries=self.__cfg.retries,
                                                assert_same_host=True,
                                                redirect=False)
                 self.cookies_middleware(is_accept=self.__cfg.accept_cookies, response=response)
             else:
                 response = PoolManager().request(self.__cfg.method, url,
-                                                 headers=self._headers,
+                                                 headers=self.__headers,
                                                  retries=self.__cfg.retries,
                                                  assert_same_host=False,
                                                  redirect=False,
                                                  timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout))
             return response
 
         except MaxRetryError:
```

### Comparing `opendoor-4.1.0/src/core/http/https.py` & `opendoor-4.2.0/src/core/http/https.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,22 @@
 
     def __init__(self, config, debug, **kwargs):
         """
         HttpsRequest instance
         :param src.lib.browser.config.Config config: global configurations
         :param DebugProvider debug: debugger
         """
-                
+
         try:
             self.__tpl = kwargs.get('tpl')
             RequestProvider.__init__(self, config, agent_list=kwargs.get('agent_list'))
-
+            self.__headers = self._headers
+            self.__connection_header = 'default'
+            if True is config.keep_alive:
+                self.__connection_header = self._keep_alive
         except (TypeError, ValueError) as error:
             raise HttpsRequestError(error)
 
         self.__cfg = config
         self.__debug = debug
         if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
             self.__pool = self.__https_pool()
@@ -71,48 +74,49 @@
         try:
             pool = HTTPSConnectionPool(
                     host=self.__cfg.host,
                     port=self.__cfg.port,
                     maxsize=self.__cfg.threads,
                     timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
                     cert_reqs='CERT_NONE',
-                    block=True)
+                    )
             if self._HTTP_DBG_LEVEL <= self.__debug.level:
-                self.__debug.debug_connection_pool('https_pool_start', pool)
+                self.__debug.debug_connection_pool('https_pool_start', pool, self.__connection_header)
 
             return pool
         except Exception as error:
             raise HttpsRequestError(str(error))
 
     def request(self, url):
         """
         Client request SSL
         :param str url: request uri
         :return: urllib3.HTTPResponse
         """
 
-        if self._HTTP_DBG_LEVEL <= self.__debug.level:
-            self.__debug.debug_request(self._headers, url, self.__cfg.method)
+        self.__headers.update({'User-Agent': self._user_agent})
+        if 'default' is not self.__connection_header:
+            self.__headers.update({'Connection': self.__connection_header})
 
+        if self._HTTP_DBG_LEVEL <= self.__debug.level:
+            self.__debug.debug_request(self.__headers, url, self.__cfg.method)
         try:
-
             disable_warnings(InsecureRequestWarning)
-
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:  # directories requests
                 response = self.__pool.request(self.__cfg.method,
                                                helper.parse_url(url).path,
-                                               headers=self._headers,
+                                               headers=self.__headers,
                                                retries=self.__cfg.retries,
                                                assert_same_host=False,
                                                redirect=False)
                 self.cookies_middleware(is_accept=self.__cfg.accept_cookies, response=response)
             else:  # subdomains
 
                 response = PoolManager().request(self.__cfg.method, url,
-                                                 headers=self._headers,
+                                                 headers=self.__headers,
                                                  retries=self.__cfg.retries,
                                                  assert_same_host=False,
                                                  redirect=False,
                                                  timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout))
             return response
 
         except MaxRetryError:
```

### Comparing `opendoor-4.1.0/src/core/http/plugins/__init__.py` & `opendoor-4.2.0/src/core/http/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/exceptions.py` & `opendoor-4.2.0/src/core/http/plugins/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/__init__.py` & `opendoor-4.2.0/src/core/http/plugins/response/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/collation.py` & `opendoor-4.2.0/src/core/http/plugins/response/collation.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/file.py` & `opendoor-4.2.0/src/core/http/plugins/response/file.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/indexof.py` & `opendoor-4.2.0/src/core/http/plugins/response/indexof.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/provider/__init__.py` & `opendoor-4.2.0/src/core/http/plugins/response/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/provider/provider.py` & `opendoor-4.2.0/src/core/http/plugins/response/provider/provider.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/skipempty.py` & `opendoor-4.2.0/src/core/http/plugins/response/skipempty.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from .provider import ResponsePluginProvider
 
 
 class SkipemptyResponsePlugin(ResponsePluginProvider):
     """ SkipemptyResponsePlugin class"""
 
     DESCRIPTION = 'SkipEmpty (skip empty success pages)'
-    RESPONSE_INDEX = 'failed'
+    RESPONSE_INDEX = 'skip'
     DEFAULT_STATUSES = [100, 101, 200, 201, 202, 203, 204, 205, 206, 207, 208]
-    DEFAULT_RECON_TO_SKIP_EMPTY_PAGE = 1000
+    DEFAULT_RECON_TO_SKIP_EMPTY_PAGE = 500
 
     def __init__(self, void):
         """
         ResponsePluginProvider constructor
         """
 
         ResponsePluginProvider.__init__(self)
```

### Comparing `opendoor-4.1.0/src/core/http/plugins/response/skipsizes.py` & `opendoor-4.2.0/src/core/http/plugins/response/skipsizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from src.core.helper import Helper
 
 
 class SkipSizesResponsePlugin(ResponsePluginProvider):
     """ SkipSizesResponsePlugin class"""
 
     DESCRIPTION = 'SkipSizesStatuses (skip target sizes of page: {} kbs for 200 OK redirects)'
-    RESPONSE_INDEX = 'failed'
+    RESPONSE_INDEX = 'skip'
     DEFAULT_STATUSES = [200]
     SIZE_VALUES = None
 
     def __init__(self, values):
         """
         ResponsePluginProvider constructor
         """
```

### Comparing `opendoor-4.1.0/src/core/http/plugins/response_plugin.py` & `opendoor-4.2.0/src/core/http/plugins/response_plugin.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/providers/__init__.py` & `opendoor-4.2.0/src/lib/reader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,13 +12,10 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-from .cookies import CookiesProvider
-from .debug import DebugProvider
-from .header import HeaderProvider
-from .request import RequestProvider
-from .response import ResponseProvider
+from .exceptions import ReaderError
+from .reader import Reader
```

### Comparing `opendoor-4.1.0/src/core/http/providers/accept.py` & `opendoor-4.2.0/src/core/http/providers/accept.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,18 +23,17 @@
     """ AcceptHeaderProvider class"""
 
     def __init__(self):
         """
         Init interface
         """
 
-        self.__accept = 'text/xml,application/xml,application/xhtml+xml,text/html;q=0.9,text/plain;q=0.8,image/png,' \
-                        'image/jpeg,*/*;q=0.5'
+        self.__accept = '*/*'
 
-        self.__accept_encoding = 'identity, deflate, compress, gzip, br'
+        self.__accept_encoding = 'identity'
 
         self.__accept_language = (
             'en-US,en;q=0.5,ru-RU,ru;q=0.8',
             'ru-RU,ru;q=0.8,en-US;q=0.6,en;q=0.4,uk;q=0.2,es;q=0.2,pl;q=0.2',
             'en,en-gb;q=0.8, en;q=0.7'
         )
```

### Comparing `opendoor-4.1.0/src/core/http/providers/cache.py` & `opendoor-4.2.0/src/core/http/providers/cache.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/providers/cookies.py` & `opendoor-4.2.0/src/core/http/providers/cookies.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/providers/debug.py` & `opendoor-4.2.0/src/core/http/providers/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,20 @@
         """
         Debug info for user agent
         :return: bool
         """
 
         pass
 
-    def debug_connection_pool(self, keymsg, pool):
+    def debug_connection_pool(self, keymsg, pool, connection_type):
         """
         Debug connection pool message
         :param str keymsg: tpl key
         :param object pool: pool object
+        :param object connection_type: type string
         :return: bool
         """
 
         pass
 
     def debug_proxy_pool(self):
         """
```

### Comparing `opendoor-4.1.0/src/core/http/providers/header.py` & `opendoor-4.2.0/src/core/http/providers/header.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,74 +12,60 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-import random
+from urllib3 import HTTPHeaderDict
 
 from .accept import AcceptHeaderProvider
 from .cache import CacheControlProvider
 
 
 class HeaderProvider(AcceptHeaderProvider, CacheControlProvider):
     """ HeaderProvider class"""
 
-    def __init__(self, config, agent_list=()):
+    def __init__(self, config):
         """
-        Init interface. Accept an external params
+        Init interface.
+        Accept external params
         :param src.lib.browser.config.Config config: browser configurations
-        :param dict agent_list: user agent list
         """
 
-        self.__headers = {}
+        self.__headers = HTTPHeaderDict()
+
         self.__cfg = config
-        self.__agent_list = agent_list
 
         AcceptHeaderProvider.__init__(self)
         CacheControlProvider.__init__(self)
 
-    @property
-    def __user_agent(self):
-        """
-        Get user agent
-        :return: str
-        """
-
-        if True is self.__cfg.is_random_user_agent:
-            index = random.randrange(0, len(self.__agent_list))
-            user_agent = self.__agent_list[index].strip()
-        else:
-            user_agent = self.__cfg.user_agent
-        return user_agent
-
     def add_header(self, key, value):
         """
         Add custom header
 
         :param str key: header name
         :param str value: header value
         :return: HeaderProvider
         """
 
-        self.__headers[key] = value
-
+        self.__headers.update({key.strip(): value.strip()})
         return self
 
     @property
     def _headers(self):
         """
         Get Headers
         :return: dict headers
         """
 
-        self.add_header('Accept', self._accept)\
-            .add_header('Accept-Encoding', self._accept_encoding)\
-            .add_header('Accept-Language', self._accept_language)\
-            .add_header('Referer', ''.join([self.__cfg.scheme, self.__cfg.host]))\
-            .add_header('User-Agent', self.__user_agent)\
-            .add_header('Cache-Control', self._cache_control)\
-            .add_header('Connection', 'keep-alive')\
+        origin = ''.join([self.__cfg.scheme, self.__cfg.host])
+        referer = ''.join([self.__cfg.scheme, self.__cfg.host]) + ':' + str(self.__cfg.port)
+        self.add_header('Accept', self._accept) \
+            .add_header('Accept-Encoding', self._accept_encoding) \
+            .add_header('Accept-Language', self._accept_language) \
+            .add_header('Origin', origin) \
+            .add_header('Referer', referer) \
+            .add_header('Cache-Control', self._cache_control) \
+            .add_header('Upgrade-Insecure-Requests', '1') \
             .add_header('Pragma', 'no-cache')
-
         return self.__headers
```

### Comparing `opendoor-4.1.0/src/core/http/providers/request.py` & `opendoor-4.2.0/src/core/http/providers/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,33 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
 from .cookies import CookiesProvider
 from .header import HeaderProvider
+from .user_agent import UserAgentHeaderProvider
+from .connection import ConnectionHeaderProvider
 
 
-class RequestProvider(CookiesProvider, HeaderProvider):
+class RequestProvider(CookiesProvider, HeaderProvider, UserAgentHeaderProvider, ConnectionHeaderProvider):
     """ RequestProvider class"""
 
     _HTTP_DBG_LEVEL = 2
 
     def __init__(self, config, agent_list):
         """
         Init interface
         :param src.lib.browser.config.Config config: configurations
         :param dict agent_list: list of user agents
         """
 
-        HeaderProvider.__init__(self, config, agent_list)
+        HeaderProvider.__init__(self, config)
+        ConnectionHeaderProvider.__init__(self, config)
+        UserAgentHeaderProvider.__init__(self, config, agent_list)
         CookiesProvider.__init__(self)
 
     def request(self, url):
         """
         Client request
         :param str url: request uri
         :return: None
@@ -44,15 +48,15 @@
 
         pass
 
     def cookies_middleware(self, is_accept, response):
         """
         Route fetched cookies from first response to the next requests
         :param is_accept: Is cookies was accepted
-        :param urllib3.response.HTTPResponse response: Http response
+        :param urllib3.response.BaseHTTPResponse response: Http response
         :return: None
         """
 
         if True is is_accept and hasattr(response, 'headers'):
             self._fetch_cookies(response.headers)
             if True is self._is_cookie_fetched:
                 self.add_header('Cookie', self._push_cookies())
```

### Comparing `opendoor-4.1.0/src/core/http/providers/response.py` & `opendoor-4.2.0/src/core/http/providers/response.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/http/proxy.py` & `opendoor-4.2.0/src/core/http/proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,39 +16,41 @@
     Development Team: Brain Storm Team
 """
 
 import importlib
 import random
 
 from urllib3 import ProxyManager, Timeout, disable_warnings
-from urllib3.exceptions import DependencyWarning, MaxRetryError, ProxySchemeUnknown,\
+from urllib3.exceptions import DependencyWarning, MaxRetryError, ProxySchemeUnknown, \
     ReadTimeoutError, InsecureRequestWarning
 
 from src.core import helper
 from .exceptions import ProxyRequestError
 from .providers import DebugProvider
 from .providers import RequestProvider
 
 
 class Proxy(RequestProvider, DebugProvider):
-
     """Proxy class"""
 
     def __init__(self, config, debug, **kwargs):
         """
         Proxy instance
         :param src.lib.browser.config.Config config: global configurations
         :param DebugProvider debug: debugger
         """
 
         try:
             self.__tpl = kwargs.get('tpl')
             self.__proxylist = kwargs.get('proxy_list')
             RequestProvider.__init__(self, config, agent_list=kwargs.get('agent_list'))
-
+            self.__headers = self._headers
+            self.__connection_header = 'default'
+            if True is config.keep_alive:
+                self.__connection_header = self._keep_alive
             self.__server = None
             self.__pm = None
             self.__cfg = config
             self.__debug = debug
             self.__debug.debug_proxy_pool()
 
             if False is config.is_standalone_proxy and 0 == len(self.__proxylist):
@@ -69,22 +71,21 @@
             self.__server = self.__cfg.proxy if True is self.__cfg.is_standalone_proxy else self.__get_random_proxy()
 
             if self.__get_proxy_type(self.__server) == 'socks':
 
                 disable_warnings(InsecureRequestWarning)
 
                 if not hasattr(self, '__pm'):
-
                     package_module = importlib.import_module('urllib3.contrib.socks')
                     self.__pm = getattr(package_module, 'SOCKSProxyManager')
 
                 pool = self.__pm(self.__server,
                                  num_pools=self.__cfg.threads,
                                  timeout=Timeout(self.__cfg.timeout,
-                                 read=self.__cfg.timeout),
+                                                 read=self.__cfg.timeout),
                                  block=True)
             else:
                 pool = ProxyManager(self.__server,
                                     num_pools=self.__cfg.threads,
                                     timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
                                     block=True)
             return pool
@@ -94,16 +95,20 @@
     def request(self, url):
         """
         Client request using Proxy
         :param str url: request uri
         :return: urllib3.HTTPResponse
         """
 
+        self.__headers.update({'User-Agent': self._user_agent})
+        if 'default' is not self.__connection_header:
+            self.__headers.update({'Connection': self.__connection_header})
+
         if self._HTTP_DBG_LEVEL <= self.__debug.level:
-            self.__debug.debug_request(self._headers, url, self.__cfg.method)
+            self.__debug.debug_request(self.__headers, url, self.__cfg.method)
 
         try:
             response = self.__pool_request(url)
             return response
 
         except MaxRetryError:
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
@@ -119,15 +124,15 @@
         """
         Shadow pool request
         :param string url: target url
         :return: urllib3.HTTPResponse
         """
 
         pool = self.__proxy_pool()
-        response = pool.request(self.__cfg.method, url, headers=self._headers, retries=self.__cfg.retries,
+        response = pool.request(self.__cfg.method, url, headers=self.__headers, retries=self.__cfg.retries,
                                 redirect=False)
 
         self.cookies_middleware(is_accept=self.__cfg.accept_cookies, response=response)
 
         return response
 
     def __get_random_proxy(self):
```

### Comparing `opendoor-4.1.0/src/core/http/response.py` & `opendoor-4.2.0/src/core/http/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         :param list ignore_list: ignore list
         :raise ResponseError
         :return: dict
         """
 
         if hasattr(response, 'status'):
             if self.HTTP_DBG_LEVEL <= self.__debug.level:
+                response.headers.update({'Status': str(response.status)})
                 if helper.is_jsonable(response.headers.items()):
                     self.__debug.debug_response(response.headers.items())
                 else:
                     self.__debug.debug_response(dict(response.headers))
 
             try:
                 status = super(Response, self).detect(request_url, response)
```

### Comparing `opendoor-4.1.0/src/core/http/socks.py` & `opendoor-4.2.0/src/core/http/socks.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/__init__.py` & `opendoor-4.2.0/src/core/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/colorize.py` & `opendoor-4.2.0/src/core/logger/colorize.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/config.py` & `opendoor-4.2.0/src/core/logger/config.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/exception.py` & `opendoor-4.2.0/src/core/logger/exception.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/logger.py` & `opendoor-4.2.0/src/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/logger/rainbow.py` & `opendoor-4.2.0/src/core/logger/rainbow.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/options/__init__.py` & `opendoor-4.2.0/src/core/options/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/options/exceptions.py` & `opendoor-4.2.0/src/core/options/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/options/filter.py` & `opendoor-4.2.0/src/core/options/filter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/options/options.py` & `opendoor-4.2.0/src/core/options/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,23 @@
                 "action": "store",
                 "help": "Max retries to reconnect (default 3)",
                 "type": int
             },
             {
                 "group": "request",
                 "args": None,
+                "argl": "--keep-alive",
+                "default": False,
+                "action": "store_true",
+                "help": "Use keep-alive connection",
+                "type": bool
+            },
+            {
+                "group": "request",
+                "args": None,
                 "argl": "--accept-cookies",
                 "default": False,
                 "action": "store_true",
                 "help": "Accept and route cookies from responses",
                 "type": bool
             },
             {
```

### Comparing `opendoor-4.1.0/src/core/system/__init__.py` & `opendoor-4.2.0/src/core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/system/exceptions.py` & `opendoor-4.2.0/src/core/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/system/output.py` & `opendoor-4.2.0/src/core/system/output.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/system/process.py` & `opendoor-4.2.0/src/core/system/process.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/core/system/terminal.py` & `opendoor-4.2.0/src/core/system/terminal.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/exceptions.py` & `opendoor-4.2.0/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/__init__.py` & `opendoor-4.2.0/src/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/browser/__init__.py` & `opendoor-4.2.0/src/lib/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/browser/browser.py` & `opendoor-4.2.0/src/lib/browser/browser.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/browser/config.py` & `opendoor-4.2.0/src/lib/browser/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,29 @@
     DEFAULT_REPORT = 'std'
     DEFAULT_SCAN = 'directories'
     SUBDOMAINS_SCAN = 'subdomains'
     DEFAULT_SCHEME = 'http://'
     DEFAULT_HTTP_PORT = 80
     DEFAULT_SSL_PORT = 443
     DEFAULT_HTTP_METHOD = 'HEAD'
-    DEFAULT_USER_AGENT = 'Opera/9.0 (Windows NT 5.1; U; en)'
+    DEFAULT_USER_AGENT = 'PostmanRuntime/7.29.0'
 
     def __init__(self, params):
         """
         Read filtered input params
         :param dict params: input cli arguments
         """
 
         self._scan = params.get('scan')
         self._scheme = self.DEFAULT_SCHEME if params.get('scheme') is None else params.get('scheme')
         self._ssl = params.get('ssl')
         self._host = params.get('host')
         self._proxy = '' if params.get('proxy') is None else params.get('proxy')
         self._accept_cookies = False if params.get('accept_cookies') is None else True
+        self._keep_alive = False if params.get('keep_alive') is None else True
         self._port = params.get('port')
         self._wordlist = params.get('wordlist')
         self._reports_dir = params.get('reports_dir')
         self._prefix = "" if params.get('prefix') is None else params.get('prefix')
         self._reports = params.get('reports')
         self._extensions = params.get('extensions')
         self._ignore_extensions = params.get('ignore_extensions')
@@ -167,17 +168,19 @@
         :return: float
         """
         return self._timeout
 
     @timeout.setter
     def timeout(self, value):
         """
-        timeout param setter
+        Timeout param setter
         :param int value:
         :return: None
+        @param value:
+        @return:
         """
 
         self._timeout = float(value)
         return self._timeout
 
     @property
     def retries(self):
@@ -244,15 +247,15 @@
             if 0 < len(self._sniff):
                 return True
         return False
 
     @property
     def sniffers(self):
         """
-        Get sniffers list
+        Get a sniffer
         :return: list
         """
 
         return self._sniff
 
     @property
     def is_random_list(self):
@@ -271,15 +274,15 @@
         """
 
         return self._is_extension_filter
 
     @property
     def is_ignore_extension_filter(self):
         """
-        If scan list filtered by ignore extensions
+        If a scan list filtered by ignore extensions
         :return: bool
         """
 
         return self._is_ignore_extension_filter
 
     @property
     def is_standalone_proxy(self):
@@ -432,7 +435,16 @@
     def accept_cookies(self):
         """
         Accept cookies property
         :return: bool
         """
 
         return self._accept_cookies
+
+    @property
+    def keep_alive(self):
+        """
+        If connection keep-alive
+        :return: bool
+        """
+
+        return self._keep_alive
```

### Comparing `opendoor-4.1.0/src/lib/browser/debug.py` & `opendoor-4.2.0/src/lib/browser/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
-
 from src.core import helper
 from src.core import sys
 from src.core.http.providers.debug import DebugProvider
 # noinspection PyPep8Naming
 from src.lib.tpl import Tpl as tpl
 
 
@@ -63,15 +62,15 @@
                 tpl.debug(key='browser', browser=self.__cfg.user_agent)
 
         return True
 
     def debug_list(self, total_lines):
         """
         Debug scan list
-        :param int total_lines: list lines
+        :param int total_lines:  lines
         :return: bool
         """
 
         if 0 < self.__level:
             if True is self.__cfg.is_random_list:
                 tpl.debug(key='randomizing')
             if self.__cfg.DEFAULT_SCAN is self.__cfg.scan:
@@ -83,25 +82,26 @@
                     tpl.debug(key='directories', total=total_lines)
             else:
                 tpl.debug(key='subdomains', total=total_lines)
             tpl.debug(key='create_queue', threads=self.__cfg.threads)
 
         return True
 
-    def debug_connection_pool(self, keymsg, pool):
+    def debug_connection_pool(self, keymsg, pool, connection_type):
         """
         Debug connection pool message
         :param str keymsg: tpl key
         :param object pool: pool object
+        :param object connection_type: type string
         :return: bool
         """
 
-        tpl.debug(key=keymsg)
+        tpl.debug(key=keymsg, type=connection_type)
         if pool:
-            tpl.debug(str(pool))
+            tpl.debug(str(pool), type=connection_type)
 
         return True
 
     def debug_proxy_pool(self):
         """
         Debug proxy pool message
         :return: bool
@@ -122,14 +122,16 @@
         """
         Debug request
         :param dict request_header: request header
         :param str url: request url
         :param str method: request method
         :return: bool
         """
+        if type(request_header) is not dict:
+            request_header = request_header.__dict__
 
         request_header.update({'Request URI': url})
         request_header.update({'Request Method': method})
 
         tpl.debug(key='request_header_dbg', dbg=helper.to_json(request_header))
 
         return True
```

### Comparing `opendoor-4.1.0/src/lib/browser/exceptions.py` & `opendoor-4.2.0/src/lib/browser/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/browser/filter.py` & `opendoor-4.2.0/src/lib/browser/filter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/browser/threadpool.py` & `opendoor-4.2.0/src/lib/browser/threadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.total_items_size = total_items
         self.is_started = True
 
         for _ in range(num_threads):
 
             worker = Worker(self.__queue, num_threads, timeout)
             if False is worker.is_alive():
-                worker.setDaemon(True)
+                worker.daemon = True
                 worker.start()
                 self.__workers.append(worker)
 
     @property
     def size(self):
         """
         Get pool size
```

### Comparing `opendoor-4.1.0/src/lib/browser/worker.py` & `opendoor-4.2.0/src/lib/browser/worker.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/events/__init__.py` & `opendoor-4.2.0/src/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/events/events.py` & `opendoor-4.2.0/src/lib/events/events.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/io/__init__.py` & `opendoor-4.2.0/src/lib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/io/arguments.py` & `opendoor-4.2.0/src/lib/io/arguments.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/io/exceptions.py` & `opendoor-4.2.0/src/lib/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/package/__init__.py` & `opendoor-4.2.0/src/lib/package/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/package/exceptions.py` & `opendoor-4.2.0/src/lib/package/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/package/package.py` & `opendoor-4.2.0/src/lib/package/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,49 +267,49 @@
         Get number of directories in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
             filename = CoreConfig.get('data').get('directories')
-            count = filesystem.read(filename).__len__()
+            count = filesystem.count_lines(filename)
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __subdomains_count():
         """
-        Get number of subdomains in basic wordlist
+        Get the number of subdomains in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
             filename = CoreConfig.get('data').get('subdomains')
-            count = filesystem.read(filename).__len__()
+            count = filesystem.count_lines(filename)
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __browsers_count():
         """
-        Get number of browsers in basic wordlist
+        Get the number of browsers in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
             filename = CoreConfig.get('data').get('useragents')
-            count = filesystem.read(filename).__len__()
+            count = filesystem.count_lines(filename)
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
@@ -318,13 +318,13 @@
         Get number of proxies in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
             filename = CoreConfig.get('data').get('proxies')
-            count = filesystem.read(filename).__len__()
+            count = filesystem.count_lines(filename)
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
```

### Comparing `opendoor-4.1.0/src/lib/reader/__init__.py` & `opendoor-4.2.0/src/lib/reporter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-from .exceptions import ReaderError
-from .reader import Reader
+from .exceptions import ReporterError
+from .reporter import Reporter
```

### Comparing `opendoor-4.1.0/src/lib/reader/config.py` & `opendoor-4.2.0/src/lib/reader/config.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reader/exceptions.py` & `opendoor-4.2.0/src/lib/reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reader/reader.py` & `opendoor-4.2.0/src/lib/reader/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             return self.__ignored
 
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
 
     def get_proxies(self):
         """
-        Get proxy list
+        Get a proxy list
         :raise ReaderError
         :return: list
         """
 
         try:
             if False is self.__browser_config.get('is_standalone_proxy'):
 
@@ -231,15 +231,15 @@
             self.__counter = len(newlist)
 
         except (CoreSystemError, FileSystemError) as error:
             raise ReaderError(error)
 
     def filter_by_ignore_extension(self, target, output, extensions):
         """
-        Specific filter for selected exuensions
+        Specific filter for selected extensions
 
         :param str target: target list
         :param str output: output list
         :param list extensions: filtered extensions
         :return: None
         """
 
@@ -253,15 +253,14 @@
             for ext in extensions:
                 pattern += '(?!\.{0})'.format(ext)
             pattern += '.)*$'
             newlist = filesystem.filter_file_lines(dirlist, pattern)
             filesystem.makefile(output_file)
             filesystem.writelist(output_file, newlist, '\n')
             self.__counter = len(newlist)
-
         except (CoreSystemError, FileSystemError) as error:
             raise ReaderError(error)
 
     def count_total_lines(self):
         """
         Count total lines inside wordlist
         :raise ReaderError
@@ -269,15 +268,15 @@
         """
         try:
             if 0 == self.__counter:
                 if True is self.__browser_config.get('is_external_wordlist'):
                     dirlist = self.__browser_config.get('wordlist')
                 else:
                     dirlist = self.__config.get(self.__browser_config.get('list'))
-                self.__counter = len(filesystem.read(dirlist))
+                self.__counter = filesystem.count_lines(dirlist)
 
             return self.__counter
 
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
 
     @property
```

### Comparing `opendoor-4.1.0/src/lib/reporter/__init__.py` & `opendoor-4.2.0/src/lib/tpl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,10 +12,9 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-from .exceptions import ReporterError
-from .reporter import Reporter
-
+from .tpl import Tpl
+from .exceptions import TplError
```

### Comparing `opendoor-4.1.0/src/lib/reporter/exceptions.py` & `opendoor-4.2.0/src/lib/reporter/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/__init__.py` & `opendoor-4.2.0/src/lib/reporter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/html.py` & `opendoor-4.2.0/src/lib/reporter/plugins/html.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/json.py` & `opendoor-4.2.0/src/lib/reporter/plugins/json.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/provider/__init__.py` & `opendoor-4.2.0/src/lib/reporter/plugins/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/provider/provider.py` & `opendoor-4.2.0/src/lib/reporter/plugins/provider/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._target = str(target)
         self._data = {}
         self.__set_data(data)
 
     def __set_data(self, data):
         """
         Set report data
-        :param dict data: report data
+        :param dict data:
         :return:
         """
 
         if False is isinstance(data, dict):
             raise TypeError("Report data has a wrong type")
         self._data = data
```

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/std.py` & `opendoor-4.2.0/src/lib/reporter/plugins/std.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/plugins/txt.py` & `opendoor-4.2.0/src/lib/reporter/plugins/txt.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/reporter/reporter.py` & `opendoor-4.2.0/src/lib/reporter/reporter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/tpl/__init__.py` & `opendoor-4.2.0/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-from .tpl import Tpl
-from .exceptions import TplError
+pass
```

### Comparing `opendoor-4.1.0/src/lib/tpl/config.py` & `opendoor-4.2.0/src/lib/tpl/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,29 @@
         'create_queue_progress': 'Create queue {bar}',
         'scanning': 'Scanning {host} ...',
         'debug': 'Starting debug level {level}. Using scan method: {method} ...',
         'randomizing': 'Randomizing scan list ...',
         'browser': 'Fetching user-agent: {browser}',
         'directories': 'Read {total} directories list by line',
         'ext_filter': 'Read {total} directories list required only: {ext}',
-        'ext_ignore_filter': 'Read {total} directories list exclude only: {ext}',
+        'ext_ignore_filter': 'Read {total} directories exclude only: {ext}',
         'create_queue': 'Creating queue with {threads} thread(s)...',
         'subdomains': 'Read {total} subdomains list by line...',
         'random_browser': 'Fetching random user-agent per request...',
         'total_time_lvl3': 'Total time running: {time}',
         'thread_limit': 'Threads has been reduced to {max} (max) instead of {threads}',
         'stop_threads': 'Stopping threads ({threads})...',
         'option_prompt': 'Press "[C]ontinue" to resume or "[E]xit" to abort session: ',
         'resume_threads': 'Resuming scan...',
         'get_item': '{percent} [{current}/{total}] - {size} - {item}',
         'ignored_item': 'skip [{current}/{total}] - Ignored {item}',
         'max_retry_error': 'skip. Max retries exceeded: {url}',
         'addtopool': 'Adding {total} lines to queue...',
-        'http_pool_start': 'Using HTTP keep-alive connection',
-        'https_pool_start': 'Using SSL keep-alive connection',
+        'http_pool_start': 'Using HTTP {type} connection',
+        'https_pool_start': 'Using SSL {type} connection',
         'proxy_pool_standalone': 'Using custom proxy server: {server}',
         'proxy_pool_internal_start': 'Fetching internal proxy list...',
         'proxy_pool_external_start': 'Fetching external proxy list...',
         'request_header_dbg': 'Request header:\n{dbg}',
         'response_header_dbg': 'Response header:\n{dbg}',
         'load_sniffer_plugin': 'Load sniffer: {description}',
         'ignored_path': 'Ignored. The path {path} in ignore list',
```

### Comparing `opendoor-4.1.0/src/lib/tpl/exceptions.py` & `opendoor-4.2.0/src/lib/tpl/exceptions.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/src/lib/tpl/tpl.py` & `opendoor-4.2.0/src/lib/tpl/tpl.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/__init__.py` & `opendoor-4.2.0/src/core/http/providers/connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,8 +12,29 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
     Development Team: Brain Storm Team
 """
 
-pass
+
+class ConnectionHeaderProvider(object):
+    """ ConnectionHeaderProvider class"""
+
+    KEEP_ALIVE = 'keep-alive'
+
+    def __init__(self, config):
+        """
+        Init interface
+        Parameters:
+        """
+
+        self.__cfg = config
+
+    @property
+    def _keep_alive(self):
+        """
+        Get 'Connection' Header
+        :return: str
+        """
+
+        return self.KEEP_ALIVE
```

### Comparing `opendoor-4.1.0/tests/test_controller.py` & `opendoor-4.2.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_core_filter.py` & `opendoor-4.2.0/tests/test_core_filter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_core_options.py` & `opendoor-4.2.0/tests/test_core_options.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_core_terminal.py` & `opendoor-4.2.0/tests/test_core_terminal.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_browser.py` & `opendoor-4.2.0/tests/test_lib_browser.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_browser_config.py` & `opendoor-4.2.0/tests/test_lib_browser_config.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_browser_debug.py` & `opendoor-4.2.0/tests/test_lib_browser_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         """ Debug.debug_list() test """
 
         self.assertTrue(self.debug.debug_list(1))
 
     def test_debug_connection_pool(self):
         """ Debug.debug_connection_pool() test """
 
-        self.assertTrue(self.debug.debug_connection_pool('http_pool_start', ''))
+        self.assertTrue(self.debug.debug_connection_pool('http_pool_start', '', ''))
 
     def test_debug_proxy_pool(self):
         """ Debug.debug_proxy_pool() test """
 
         self.assertTrue(self.debug.debug_proxy_pool())
 
     def test_debug_user_agents(self):
```

### Comparing `opendoor-4.1.0/tests/test_lib_browser_filter.py` & `opendoor-4.2.0/tests/test_lib_browser_filter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_browser_threadpool.py` & `opendoor-4.2.0/tests/test_lib_browser_threadpool.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_browser_worker.py` & `opendoor-4.2.0/tests/test_lib_browser_worker.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_events.py` & `opendoor-4.2.0/tests/test_lib_events.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_package.py` & `opendoor-4.2.0/tests/test_lib_package.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_reader.py` & `opendoor-4.2.0/tests/test_lib_reader.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_reporter.py` & `opendoor-4.2.0/tests/test_lib_reporter.py`

 * *Files identical despite different names*

### Comparing `opendoor-4.1.0/tests/test_lib_tpl.py` & `opendoor-4.2.0/tests/test_lib_tpl.py`

 * *Files identical despite different names*

