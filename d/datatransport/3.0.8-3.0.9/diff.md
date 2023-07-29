# Comparing `tmp/datatransport-3.0.8.tar.gz` & `tmp/datatransport-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransport-3.0.8.tar", last modified: Sat Jul 29 16:45:24 2023, max compression
+gzip compressed data, was "datatransport-3.0.9.tar", last modified: Sat Jul 29 17:10:23 2023, max compression
```

## Comparing `datatransport-3.0.8.tar` & `datatransport-3.0.9.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/
--rw-rw-r--   0 valentic   (500) valentic   (500)    50330 2023-07-28 01:50:10.000000 datatransport-3.0.8/CHANGES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.8/INSTALL
--rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.8/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.8/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.8/MIGRATION
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 16:45:24.000000 datatransport-3.0.8/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.8/README.rst
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/
--rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/.coverage
--rw-rw-r--   0 valentic   (500) valentic   (500)      121 2023-07-27 16:34:01.000000 datatransport-3.0.8/contrib/examples/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2333 2023-07-26 23:11:05.000000 datatransport-3.0.8/contrib/examples/archivegroups/archivegroups.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-26 21:56:24.000000 datatransport-3.0.8/contrib/examples/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/component/component.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1854 2023-07-27 04:14:34.000000 datatransport-3.0.8/contrib/examples/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/diskmonitor/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-28 00:07:08.000000 datatransport-3.0.8/contrib/examples/diskmonitor/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      552 2023-07-28 01:46:30.000000 datatransport-3.0.8/contrib/examples/diskmonitor/diskmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/environ/environ.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1097 2023-07-26 20:31:33.000000 datatransport-3.0.8/contrib/examples/environ/environ.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.8/contrib/examples/examples.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/filepost/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:33:18.000000 datatransport-3.0.8/contrib/examples/filepost/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 03:19:27.000000 datatransport-3.0.8/contrib/examples/filepost/filepost.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:16:01.000000 datatransport-3.0.8/contrib/examples/filepost/watcher.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/filewatch/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-26 21:29:22.000000 datatransport-3.0.8/contrib/examples/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/getbytes/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      874 2023-07-26 21:19:37.000000 datatransport-3.0.8/contrib/examples/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/groupcontrol/
--rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 09:48:31.000000 datatransport-3.0.8/contrib/examples/groupcontrol/groupcontrol.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      996 2023-07-28 09:39:17.000000 datatransport-3.0.8/contrib/examples/groupcontrol/request.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/hello/
--rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.8/contrib/examples/hello/hello.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      876 2023-07-26 20:27:09.000000 datatransport-3.0.8/contrib/examples/hello/helloworld.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/init/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1020 2023-07-26 20:28:47.000000 datatransport-3.0.8/contrib/examples/init/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/init/init.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/messagebox/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/messagebox.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/poll_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/poll_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/post_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/post_text.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/postpoll/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1090 2023-07-26 21:11:35.000000 datatransport-3.0.8/contrib/examples/postpoll/poll_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      918 2023-07-26 20:43:33.000000 datatransport-3.0.8/contrib/examples/postpoll/poll_text.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1162 2023-07-26 20:46:08.000000 datatransport-3.0.8/contrib/examples/postpoll/post_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1010 2023-07-26 20:34:43.000000 datatransport-3.0.8/contrib/examples/postpoll/post_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/postpoll/postpoll.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/rotatelogs/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      868 2023-07-26 21:20:22.000000 datatransport-3.0.8/contrib/examples/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/service/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1194 2023-07-27 16:36:41.000000 datatransport-3.0.8/contrib/examples/service/client.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/directory.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/echo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/service.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/spawn/spawn.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1304 2023-07-26 21:26:34.000000 datatransport-3.0.8/contrib/examples/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/watchdog/
--rwxr-xr-x   0 valentic   (500) valentic   (500)     1061 2023-07-26 21:27:53.000000 datatransport-3.0.8/contrib/examples/watchdog/crasher.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/watchdog/init_crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/archivegroups.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/component/component.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/config/config.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/config/config.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/diskmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/diskmonitor/diskmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/environ/environ.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/environ/environ.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/eventmonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/serverstate.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/plugin.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/postdata
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/
--rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/README
--rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/multipoll.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/reader.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/writer.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/plottool/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/plottool/datasource.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/plottool/plottool.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/checkdate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/postdatafiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/resourcemonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/
--rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/spawn/spawn.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/splitfiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/
--rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/poller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/source.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/syncpoller.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/test.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/wait/
--rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/wait/timer.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/wait/wait.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/
--rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/utils/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/createnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/getarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/postarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/rebuilddatabase
--rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/relaynewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/rmnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/watchtransport
--rw-rw-r--   0 valentic   (500) valentic   (500)     2553 2023-07-28 05:11:21.000000 datatransport-3.0.8/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-29 16:45:24.000000 datatransport-3.0.8/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/
--rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1539 2023-07-27 20:11:25.000000 datatransport-3.0.8/src/datatransport/accessmixin.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/commands/
--rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/cancelnewsgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/console.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/listnewsgroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transport_create_app.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportctl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportd.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportps.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.8/src/datatransport/commands/viewlog.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)     6359 2023-07-28 01:54:18.000000 datatransport-3.0.8/src/datatransport/components/EventMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/InstrumentStatus.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4978 2023-07-27 23:58:31.000000 datatransport-3.0.8/src/datatransport/components/NewsGateway.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8153 2023-07-29 16:44:12.000000 datatransport-3.0.8/src/datatransport/components/NewsgroupMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/PageKit.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-28 09:57:05.000000 datatransport-3.0.8/src/datatransport/components/PlotTool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    12712 2023-07-27 07:14:43.000000 datatransport-3.0.8/src/datatransport/components/PostDataFiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/RealTimeFeed.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/ResourceMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6942 2023-07-27 07:14:44.000000 datatransport-3.0.8/src/datatransport/components/Scheduler.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/SyncPoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11743 2023-07-27 07:14:44.000000 datatransport-3.0.8/src/datatransport/components/WatchURL.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      611 2023-07-28 05:11:11.000000 datatransport-3.0.8/src/datatransport/components/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    52705 2023-07-26 23:57:41.000000 datatransport-3.0.8/src/datatransport/components/archivegroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2736 2023-07-27 16:48:23.000000 datatransport-3.0.8/src/datatransport/components/directoryservice.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5993 2023-07-28 01:52:06.000000 datatransport-3.0.8/src/datatransport/components/diskmonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4945 2023-07-28 03:31:35.000000 datatransport-3.0.8/src/datatransport/components/filepost.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5651 2023-07-26 21:50:04.000000 datatransport-3.0.8/src/datatransport/components/filewatch.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5811 2023-07-28 09:53:16.000000 datatransport-3.0.8/src/datatransport/components/groupcontrol.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1304 2023-07-27 18:05:17.000000 datatransport-3.0.8/src/datatransport/configcomponent.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3065 2023-07-26 20:39:27.000000 datatransport-3.0.8/src/datatransport/directory.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-29 16:44:35.000000 datatransport-3.0.8/src/datatransport/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10799 2023-07-27 21:09:07.000000 datatransport-3.0.8/src/datatransport/newspoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8209 2023-07-27 21:58:14.000000 datatransport-3.0.8/src/datatransport/newsposter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    34276 2023-07-28 09:22:06.000000 datatransport-3.0.8/src/datatransport/newstool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    15585 2023-07-28 09:43:01.000000 datatransport-3.0.8/src/datatransport/processclient.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    13509 2023-07-20 22:01:05.000000 datatransport-3.0.8/src/datatransport/processgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/root.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/etc/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/templates/etc/transportd.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/groups/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4747 2023-07-27 05:02:15.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/watchdog.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.8/src/datatransport/transportconfig.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportlogger.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportmanager.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/utilities/
--rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4170 2023-07-27 03:27:27.000000 datatransport-3.0.8/src/datatransport/utilities/patterntemplate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/removefile.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/sizedesc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/xmlrpcdeferred.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4505 2023-07-27 16:47:53.000000 datatransport-3.0.8/src/datatransport/xmlrpcserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)     6623 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)     1278 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/entry_points.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/tests/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/tests/__pycache__/
--rw-rw-r--   0 valentic   (500) valentic   (500)     8651 2023-07-27 01:45:55.000000 datatransport-3.0.8/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2113 2023-07-27 01:45:50.000000 datatransport-3.0.8/tests/test_utilities_pattern.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_removefiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_sizedesc.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    50517 2023-07-29 17:10:07.000000 datatransport-3.0.9/CHANGES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.9/INSTALL
+-rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.9/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.9/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.9/MIGRATION
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 17:10:23.000000 datatransport-3.0.9/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.9/README.rst
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/.coverage
+-rw-rw-r--   0 valentic   (500) valentic   (500)      121 2023-07-27 16:34:01.000000 datatransport-3.0.9/contrib/examples/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2333 2023-07-26 23:11:05.000000 datatransport-3.0.9/contrib/examples/archivegroups/archivegroups.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-26 21:56:24.000000 datatransport-3.0.9/contrib/examples/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/component/component.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1854 2023-07-27 04:14:34.000000 datatransport-3.0.9/contrib/examples/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/diskmonitor/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-28 00:07:08.000000 datatransport-3.0.9/contrib/examples/diskmonitor/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      552 2023-07-28 01:46:30.000000 datatransport-3.0.9/contrib/examples/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/environ/environ.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1097 2023-07-26 20:31:33.000000 datatransport-3.0.9/contrib/examples/environ/environ.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.9/contrib/examples/examples.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/filepost/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:33:18.000000 datatransport-3.0.9/contrib/examples/filepost/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 03:19:27.000000 datatransport-3.0.9/contrib/examples/filepost/filepost.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:16:01.000000 datatransport-3.0.9/contrib/examples/filepost/watcher.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/filewatch/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-26 21:29:22.000000 datatransport-3.0.9/contrib/examples/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/getbytes/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      874 2023-07-26 21:19:37.000000 datatransport-3.0.9/contrib/examples/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/groupcontrol/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 09:48:31.000000 datatransport-3.0.9/contrib/examples/groupcontrol/groupcontrol.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      996 2023-07-28 09:39:17.000000 datatransport-3.0.9/contrib/examples/groupcontrol/request.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/hello/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.9/contrib/examples/hello/hello.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      876 2023-07-26 20:27:09.000000 datatransport-3.0.9/contrib/examples/hello/helloworld.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/init/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1020 2023-07-26 20:28:47.000000 datatransport-3.0.9/contrib/examples/init/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/init/init.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/messagebox/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/messagebox/messagebox.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/messagebox/poll_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/messagebox/poll_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/messagebox/post_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/messagebox/post_text.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/postpoll/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1090 2023-07-26 21:11:35.000000 datatransport-3.0.9/contrib/examples/postpoll/poll_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      918 2023-07-26 20:43:33.000000 datatransport-3.0.9/contrib/examples/postpoll/poll_text.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1162 2023-07-26 20:46:08.000000 datatransport-3.0.9/contrib/examples/postpoll/post_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1010 2023-07-26 20:34:43.000000 datatransport-3.0.9/contrib/examples/postpoll/post_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/postpoll/postpoll.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/rotatelogs/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      868 2023-07-26 21:20:22.000000 datatransport-3.0.9/contrib/examples/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/service/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1194 2023-07-27 16:36:41.000000 datatransport-3.0.9/contrib/examples/service/client.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/service/directory.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/service/echo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/service/service.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/spawn/spawn.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1304 2023-07-26 21:26:34.000000 datatransport-3.0.9/contrib/examples/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples/watchdog/
+-rwxr-xr-x   0 valentic   (500) valentic   (500)     1061 2023-07-26 21:27:53.000000 datatransport-3.0.9/contrib/examples/watchdog/crasher.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/watchdog/init_crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/archivegroups/archivegroups.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/component/component.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/config/config.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/config/config.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/diskmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/environ/environ.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/environ/environ.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/eventmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/eventmonitor/eventmonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/eventmonitor/serverstate.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/filewatch/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/getbytes/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/instrumentstatus/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/instrumentstatus/plugin.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/instrumentstatus/postdata
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/multipoll/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/multipoll/README
+-rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/multipoll/multipoll.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/multipoll/reader.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/multipoll/writer.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/newsgroupmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/plottool/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/plottool/datasource.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/plottool/plottool.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/postdatafiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/postdatafiles/checkdate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/postdatafiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/postdatafiles/postdatafiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/resourcemonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/rotatelogs/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/spawn/spawn.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/splitfiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/splitfiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/splitfiles/splitfiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/syncpoller/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/syncpoller/poller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/syncpoller/source.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/syncpoller/syncpoller.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/test.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/wait/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/wait/timer.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/wait/wait.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/examples.v2/watchdog/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/watchdog/crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/examples.v2/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/contrib/utils/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/createnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/getarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/postarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/rebuilddatabase
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/relaynewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/rmnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.9/contrib/utils/watchtransport
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2553 2023-07-28 05:11:21.000000 datatransport-3.0.9/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-29 17:10:23.000000 datatransport-3.0.9/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1539 2023-07-27 20:11:25.000000 datatransport-3.0.9/src/datatransport/accessmixin.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/commands/
+-rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/cancelnewsgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/console.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/listnewsgroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/transport_create_app.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/transportctl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/transportd.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/commands/transportps.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.9/src/datatransport/commands/viewlog.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6359 2023-07-28 01:54:18.000000 datatransport-3.0.9/src/datatransport/components/EventMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/components/InstrumentStatus.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4955 2023-07-29 17:08:08.000000 datatransport-3.0.9/src/datatransport/components/NewsGateway.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8153 2023-07-29 16:44:12.000000 datatransport-3.0.9/src/datatransport/components/NewsgroupMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/components/PageKit.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-28 09:57:05.000000 datatransport-3.0.9/src/datatransport/components/PlotTool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    12712 2023-07-27 07:14:43.000000 datatransport-3.0.9/src/datatransport/components/PostDataFiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/components/RealTimeFeed.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/components/ResourceMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6942 2023-07-27 07:14:44.000000 datatransport-3.0.9/src/datatransport/components/Scheduler.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/components/SyncPoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11743 2023-07-27 07:14:44.000000 datatransport-3.0.9/src/datatransport/components/WatchURL.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      611 2023-07-28 05:11:11.000000 datatransport-3.0.9/src/datatransport/components/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    52705 2023-07-26 23:57:41.000000 datatransport-3.0.9/src/datatransport/components/archivegroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2736 2023-07-27 16:48:23.000000 datatransport-3.0.9/src/datatransport/components/directoryservice.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5993 2023-07-28 01:52:06.000000 datatransport-3.0.9/src/datatransport/components/diskmonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4945 2023-07-28 03:31:35.000000 datatransport-3.0.9/src/datatransport/components/filepost.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5651 2023-07-26 21:50:04.000000 datatransport-3.0.9/src/datatransport/components/filewatch.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5811 2023-07-28 09:53:16.000000 datatransport-3.0.9/src/datatransport/components/groupcontrol.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1304 2023-07-27 18:05:17.000000 datatransport-3.0.9/src/datatransport/configcomponent.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3065 2023-07-26 20:39:27.000000 datatransport-3.0.9/src/datatransport/directory.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-29 17:10:13.000000 datatransport-3.0.9/src/datatransport/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10799 2023-07-27 21:09:07.000000 datatransport-3.0.9/src/datatransport/newspoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8209 2023-07-27 21:58:14.000000 datatransport-3.0.9/src/datatransport/newsposter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    34276 2023-07-28 09:22:06.000000 datatransport-3.0.9/src/datatransport/newstool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    15585 2023-07-28 09:43:01.000000 datatransport-3.0.9/src/datatransport/processclient.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    13509 2023-07-20 22:01:05.000000 datatransport-3.0.9/src/datatransport/processgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/root.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/templates/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/templates/etc/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/templates/etc/transportd.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/templates/groups/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/templates/groups/ServerMonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4747 2023-07-27 05:02:15.000000 datatransport-3.0.9/src/datatransport/templates/groups/ServerMonitor/watchdog.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.9/src/datatransport/transportconfig.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/transportlogger.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/transportmanager.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/transportserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport/utilities/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4170 2023-07-27 03:27:27.000000 datatransport-3.0.9/src/datatransport/utilities/patterntemplate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/removefile.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/sizedesc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.9/src/datatransport/utilities/xmlrpcdeferred.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4505 2023-07-27 16:47:53.000000 datatransport-3.0.9/src/datatransport/xmlrpcserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6623 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1278 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/entry_points.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-29 17:10:23.000000 datatransport-3.0.9/src/datatransport.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 17:10:23.000000 datatransport-3.0.9/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8651 2023-07-27 01:45:55.000000 datatransport-3.0.9/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.9/tests/test_utilities_datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.9/tests/test_utilities_makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2113 2023-07-27 01:45:50.000000 datatransport-3.0.9/tests/test_utilities_pattern.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.9/tests/test_utilities_removefiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.9/tests/test_utilities_sizedesc.py
```

### Comparing `datatransport-3.0.8/CHANGES.txt` & `datatransport-3.0.9/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
+2023-07-29  Todd Valentic
+    - NewsGateway. Fix formatting issue.
+    - Release 3.0.9
+
 2023-07-27  Todd Valentic
-    - DiskMonitor updated.
+    - DiskMonitor updated
+    - GroupControl updated
+    - FilePost updated
+    - DiskMonitor updated
+    - FileWatch updated
 
     - Release 3.0.8
 
 2023-07-20  Todd Valentic
     - ProcessGroup. Do not log error if no clients listed
     - ProcessGroup. Change default shutdown timeout to be 30s
     - ProcessGroup. Change shutdown timeout to be a timedelta
```

### Comparing `datatransport-3.0.8/INSTALL` & `datatransport-3.0.9/INSTALL`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/LICENSE` & `datatransport-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/MIGRATION` & `datatransport-3.0.9/MIGRATION`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/PKG-INFO` & `datatransport-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.8
+Version: 3.0.9
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.8/contrib/examples/.coverage` & `datatransport-3.0.9/contrib/examples/.coverage`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/archivegroups/archivegroups.conf` & `datatransport-3.0.9/contrib/examples/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/archivegroups/postdata.py` & `datatransport-3.0.9/contrib/examples/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/component/component.conf` & `datatransport-3.0.9/contrib/examples/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/component/demo.py` & `datatransport-3.0.9/contrib/examples/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/diskmonitor/demo.py` & `datatransport-3.0.9/contrib/examples/diskmonitor/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/diskmonitor/diskmonitor.conf` & `datatransport-3.0.9/contrib/examples/diskmonitor/diskmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/environ/environ.py` & `datatransport-3.0.9/contrib/examples/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/filepost/createdata.py` & `datatransport-3.0.9/contrib/examples/filepost/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/filepost/filepost.conf` & `datatransport-3.0.9/contrib/examples/filepost/filepost.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/filepost/watcher.py` & `datatransport-3.0.9/contrib/examples/filepost/watcher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/filewatch/createdata.py` & `datatransport-3.0.9/contrib/examples/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/getbytes/demo.py` & `datatransport-3.0.9/contrib/examples/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/getbytes/getbytes.conf` & `datatransport-3.0.9/contrib/examples/getbytes/getbytes.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/groupcontrol/groupcontrol.conf` & `datatransport-3.0.9/contrib/examples/groupcontrol/groupcontrol.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/groupcontrol/request.py` & `datatransport-3.0.9/contrib/examples/groupcontrol/request.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/hello/helloworld.py` & `datatransport-3.0.9/contrib/examples/hello/helloworld.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/init/demo.py` & `datatransport-3.0.9/contrib/examples/init/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/messagebox/messagebox.conf` & `datatransport-3.0.9/contrib/examples/messagebox/messagebox.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/messagebox/poll_file.py` & `datatransport-3.0.9/contrib/examples/messagebox/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/messagebox/poll_text.py` & `datatransport-3.0.9/contrib/examples/messagebox/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/messagebox/post_file.py` & `datatransport-3.0.9/contrib/examples/messagebox/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/messagebox/post_text.py` & `datatransport-3.0.9/contrib/examples/messagebox/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/postpoll/poll_file.py` & `datatransport-3.0.9/contrib/examples/postpoll/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/postpoll/poll_text.py` & `datatransport-3.0.9/contrib/examples/postpoll/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/postpoll/post_file.py` & `datatransport-3.0.9/contrib/examples/postpoll/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/postpoll/post_text.py` & `datatransport-3.0.9/contrib/examples/postpoll/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/postpoll/postpoll.conf` & `datatransport-3.0.9/contrib/examples/postpoll/postpoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/rotatelogs/counter.py` & `datatransport-3.0.9/contrib/examples/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/service/client.py` & `datatransport-3.0.9/contrib/examples/service/client.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/service/echo.py` & `datatransport-3.0.9/contrib/examples/service/echo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/service/service.conf` & `datatransport-3.0.9/contrib/examples/service/service.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/spawn/spawner.py` & `datatransport-3.0.9/contrib/examples/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/watchdog/crasher.py` & `datatransport-3.0.9/contrib/examples/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples/watchdog/init_crasher.py` & `datatransport-3.0.9/contrib/examples/watchdog/init_crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/README` & `datatransport-3.0.9/contrib/examples.v2/README`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/archivegroups/archivegroups.conf` & `datatransport-3.0.9/contrib/examples.v2/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/archivegroups/postdata.py` & `datatransport-3.0.9/contrib/examples.v2/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/component/component.conf` & `datatransport-3.0.9/contrib/examples.v2/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/component/demo.py` & `datatransport-3.0.9/contrib/examples.v2/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/config/config.py` & `datatransport-3.0.9/contrib/examples.v2/config/config.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/environ/environ.py` & `datatransport-3.0.9/contrib/examples.v2/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/eventmonitor/eventmonitor.conf` & `datatransport-3.0.9/contrib/examples.v2/eventmonitor/eventmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/eventmonitor/serverstate.py` & `datatransport-3.0.9/contrib/examples.v2/eventmonitor/serverstate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/filewatch/createdata.py` & `datatransport-3.0.9/contrib/examples.v2/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/getbytes/demo.py` & `datatransport-3.0.9/contrib/examples.v2/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/instrumentstatus/instrumentstatus.conf` & `datatransport-3.0.9/contrib/examples.v2/instrumentstatus/instrumentstatus.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/instrumentstatus/postdata` & `datatransport-3.0.9/contrib/examples.v2/instrumentstatus/postdata`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/multipoll/multipoll.conf` & `datatransport-3.0.9/contrib/examples.v2/multipoll/multipoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/multipoll/writer.py` & `datatransport-3.0.9/contrib/examples.v2/multipoll/writer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf` & `datatransport-3.0.9/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/plottool/datasource.py` & `datatransport-3.0.9/contrib/examples.v2/plottool/datasource.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/plottool/plottool.conf` & `datatransport-3.0.9/contrib/examples.v2/plottool/plottool.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/postdatafiles/createfiles.py` & `datatransport-3.0.9/contrib/examples.v2/postdatafiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/postdatafiles/postdatafiles.conf` & `datatransport-3.0.9/contrib/examples.v2/postdatafiles/postdatafiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/rotatelogs/counter.py` & `datatransport-3.0.9/contrib/examples.v2/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/spawn/spawner.py` & `datatransport-3.0.9/contrib/examples.v2/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/splitfiles/createfiles.py` & `datatransport-3.0.9/contrib/examples.v2/splitfiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/splitfiles/splitfiles.conf` & `datatransport-3.0.9/contrib/examples.v2/splitfiles/splitfiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/syncpoller/source.py` & `datatransport-3.0.9/contrib/examples.v2/syncpoller/source.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/syncpoller/syncpoller.conf` & `datatransport-3.0.9/contrib/examples.v2/syncpoller/syncpoller.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/wait/timer.py` & `datatransport-3.0.9/contrib/examples.v2/wait/timer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/examples.v2/watchdog/crasher.py` & `datatransport-3.0.9/contrib/examples.v2/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/createnewsgroup` & `datatransport-3.0.9/contrib/utils/createnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/getarticle` & `datatransport-3.0.9/contrib/utils/getarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/postarticle` & `datatransport-3.0.9/contrib/utils/postarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/rebuilddatabase` & `datatransport-3.0.9/contrib/utils/rebuilddatabase`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/relaynewsgroup` & `datatransport-3.0.9/contrib/utils/relaynewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/rmnewsgroup` & `datatransport-3.0.9/contrib/utils/rmnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/contrib/utils/watchtransport` & `datatransport-3.0.9/contrib/utils/watchtransport`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/pyproject.toml` & `datatransport-3.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/__init__.py` & `datatransport-3.0.9/src/datatransport/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/accessmixin.py` & `datatransport-3.0.9/src/datatransport/accessmixin.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/cancelnewsgroup.py` & `datatransport-3.0.9/src/datatransport/commands/cancelnewsgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/console.py` & `datatransport-3.0.9/src/datatransport/commands/console.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/listnewsgroups.py` & `datatransport-3.0.9/src/datatransport/commands/listnewsgroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/transport_create_app.py` & `datatransport-3.0.9/src/datatransport/commands/transport_create_app.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/transportctl.py` & `datatransport-3.0.9/src/datatransport/commands/transportctl.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/transportd.py` & `datatransport-3.0.9/src/datatransport/commands/transportd.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/transportps.py` & `datatransport-3.0.9/src/datatransport/commands/transportps.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/commands/viewlog.py` & `datatransport-3.0.9/src/datatransport/commands/viewlog.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/EventMonitor.py` & `datatransport-3.0.9/src/datatransport/components/EventMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/InstrumentStatus.py` & `datatransport-3.0.9/src/datatransport/components/InstrumentStatus.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/NewsGateway.py` & `datatransport-3.0.9/src/datatransport/components/NewsGateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,33 +84,33 @@
 
         self.messages.clear()
         self.messages.sync()
 
     @synchronized(lock)
     def read(self, newsgroup):
         """Read entry from cache"""
-     
+
         return self.messages[newsgroup]
 
     @synchronized(lock)
     def list(self):
         """List cache"""
-      
-      return self.messages.keys()
+
+        return self.messages.keys()
 
     @synchronized(lock)
     def get_string(self, newsgroup):
         """Reture message as string"""
-       
-       return self.messages[newsgroup].as_string()
+
+        return self.messages[newsgroup].as_string()
 
     @synchronized(lock)
     def unpickle(self, newsgroup):
         """Unpickle message"""
-        
+
         return pickle.loads(self.messages[newsgroup].get_payload())
 
 
 class Server(Thread, AccessMixin):
     """XMLRPC Server Interface"""
 
     def __init__(self, parent, data):
```

### Comparing `datatransport-3.0.8/src/datatransport/components/NewsgroupMonitor.py` & `datatransport-3.0.9/src/datatransport/components/NewsgroupMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/PageKit.py` & `datatransport-3.0.9/src/datatransport/components/PageKit.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/PlotTool.py` & `datatransport-3.0.9/src/datatransport/components/PlotTool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/PostDataFiles.py` & `datatransport-3.0.9/src/datatransport/components/PostDataFiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/RealTimeFeed.py` & `datatransport-3.0.9/src/datatransport/components/RealTimeFeed.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/ResourceMonitor.py` & `datatransport-3.0.9/src/datatransport/components/ResourceMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/Scheduler.py` & `datatransport-3.0.9/src/datatransport/components/Scheduler.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/SyncPoller.py` & `datatransport-3.0.9/src/datatransport/components/SyncPoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/WatchURL.py` & `datatransport-3.0.9/src/datatransport/components/WatchURL.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/__init__.py` & `datatransport-3.0.9/src/datatransport/components/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/archivegroups.py` & `datatransport-3.0.9/src/datatransport/components/archivegroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/directoryservice.py` & `datatransport-3.0.9/src/datatransport/components/directoryservice.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/diskmonitor.py` & `datatransport-3.0.9/src/datatransport/components/diskmonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/filepost.py` & `datatransport-3.0.9/src/datatransport/components/filepost.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/filewatch.py` & `datatransport-3.0.9/src/datatransport/components/filewatch.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/components/groupcontrol.py` & `datatransport-3.0.9/src/datatransport/components/groupcontrol.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/configcomponent.py` & `datatransport-3.0.9/src/datatransport/configcomponent.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/directory.py` & `datatransport-3.0.9/src/datatransport/directory.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/newspoller.py` & `datatransport-3.0.9/src/datatransport/newspoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/newsposter.py` & `datatransport-3.0.9/src/datatransport/newsposter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/newstool.py` & `datatransport-3.0.9/src/datatransport/newstool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/processclient.py` & `datatransport-3.0.9/src/datatransport/processclient.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/processgroup.py` & `datatransport-3.0.9/src/datatransport/processgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/templates/etc/transportd.conf` & `datatransport-3.0.9/src/datatransport/templates/etc/transportd.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/watchdog.py` & `datatransport-3.0.9/src/datatransport/templates/groups/ServerMonitor/watchdog.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/transportconfig.py` & `datatransport-3.0.9/src/datatransport/transportconfig.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/transportlogger.py` & `datatransport-3.0.9/src/datatransport/transportlogger.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/transportmanager.py` & `datatransport-3.0.9/src/datatransport/transportmanager.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/transportserver.py` & `datatransport-3.0.9/src/datatransport/transportserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/datefunc.py` & `datatransport-3.0.9/src/datatransport/utilities/datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/makepath.py` & `datatransport-3.0.9/src/datatransport/utilities/makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/patterntemplate.py` & `datatransport-3.0.9/src/datatransport/utilities/patterntemplate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/removefile.py` & `datatransport-3.0.9/src/datatransport/utilities/removefile.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/sizedesc.py` & `datatransport-3.0.9/src/datatransport/utilities/sizedesc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/utilities/xmlrpcdeferred.py` & `datatransport-3.0.9/src/datatransport/utilities/xmlrpcdeferred.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport/xmlrpcserver.py` & `datatransport-3.0.9/src/datatransport/xmlrpcserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport.egg-info/PKG-INFO` & `datatransport-3.0.9/src/datatransport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.8
+Version: 3.0.9
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.8/src/datatransport.egg-info/SOURCES.txt` & `datatransport-3.0.9/src/datatransport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/src/datatransport.egg-info/entry_points.txt` & `datatransport-3.0.9/src/datatransport.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc` & `datatransport-3.0.9/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/test_utilities_datefunc.py` & `datatransport-3.0.9/tests/test_utilities_datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/test_utilities_makepath.py` & `datatransport-3.0.9/tests/test_utilities_makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/test_utilities_pattern.py` & `datatransport-3.0.9/tests/test_utilities_pattern.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/test_utilities_removefiles.py` & `datatransport-3.0.9/tests/test_utilities_removefiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.8/tests/test_utilities_sizedesc.py` & `datatransport-3.0.9/tests/test_utilities_sizedesc.py`

 * *Files identical despite different names*

