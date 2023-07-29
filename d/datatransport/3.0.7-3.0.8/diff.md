# Comparing `tmp/datatransport-3.0.7.tar.gz` & `tmp/datatransport-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransport-3.0.7.tar", last modified: Thu Jul 27 22:31:25 2023, max compression
+gzip compressed data, was "datatransport-3.0.8.tar", last modified: Sat Jul 29 16:45:24 2023, max compression
```

## Comparing `datatransport-3.0.7.tar` & `datatransport-3.0.8.tar`

### file list

```diff
@@ -1,215 +1,224 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/
--rw-rw-r--   0 valentic   (500) valentic   (500)    50206 2023-07-27 21:23:37.000000 datatransport-3.0.7/CHANGES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.7/INSTALL
--rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.7/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.7/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.7/MIGRATION
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-27 22:31:25.000000 datatransport-3.0.7/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.7/README.rst
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/
--rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/.coverage
--rw-rw-r--   0 valentic   (500) valentic   (500)      121 2023-07-27 16:34:01.000000 datatransport-3.0.7/contrib/examples/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2333 2023-07-26 23:11:05.000000 datatransport-3.0.7/contrib/examples/archivegroups/archivegroups.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-26 21:56:24.000000 datatransport-3.0.7/contrib/examples/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/component/component.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1854 2023-07-27 04:14:34.000000 datatransport-3.0.7/contrib/examples/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/environ/environ.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1097 2023-07-26 20:31:33.000000 datatransport-3.0.7/contrib/examples/environ/environ.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.7/contrib/examples/examples.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/filewatch/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-26 21:29:22.000000 datatransport-3.0.7/contrib/examples/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/getbytes/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      874 2023-07-26 21:19:37.000000 datatransport-3.0.7/contrib/examples/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/hello/
--rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.7/contrib/examples/hello/hello.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      876 2023-07-26 20:27:09.000000 datatransport-3.0.7/contrib/examples/hello/helloworld.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/init/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1020 2023-07-26 20:28:47.000000 datatransport-3.0.7/contrib/examples/init/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/init/init.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/messagebox/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/messagebox.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/poll_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/poll_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/post_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/post_text.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/postpoll/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1090 2023-07-26 21:11:35.000000 datatransport-3.0.7/contrib/examples/postpoll/poll_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      918 2023-07-26 20:43:33.000000 datatransport-3.0.7/contrib/examples/postpoll/poll_text.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1162 2023-07-26 20:46:08.000000 datatransport-3.0.7/contrib/examples/postpoll/post_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1010 2023-07-26 20:34:43.000000 datatransport-3.0.7/contrib/examples/postpoll/post_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/postpoll/postpoll.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/rotatelogs/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      868 2023-07-26 21:20:22.000000 datatransport-3.0.7/contrib/examples/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/service/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1194 2023-07-27 16:36:41.000000 datatransport-3.0.7/contrib/examples/service/client.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/directory.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/echo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/service.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/spawn/spawn.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1304 2023-07-26 21:26:34.000000 datatransport-3.0.7/contrib/examples/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/watchdog/
--rwxr-xr-x   0 valentic   (500) valentic   (500)     1061 2023-07-26 21:27:53.000000 datatransport-3.0.7/contrib/examples/watchdog/crasher.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/watchdog/init_crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/archivegroups.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/component/component.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/config/config.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/config/config.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/diskmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/diskmonitor/diskmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/environ/environ.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/environ/environ.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/eventmonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/serverstate.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/plugin.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/postdata
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/
--rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/README
--rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/multipoll.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/reader.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/writer.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/plottool/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/plottool/datasource.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/plottool/plottool.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/checkdate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/postdatafiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/resourcemonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/
--rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/spawn/spawn.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/splitfiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/
--rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/poller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/source.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/syncpoller.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/test.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/wait/
--rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/wait/timer.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/wait/wait.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/
--rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/utils/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/createnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/getarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/postarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/rebuilddatabase
--rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/relaynewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/rmnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/watchtransport
--rw-rw-r--   0 valentic   (500) valentic   (500)     2611 2023-07-27 16:43:31.000000 datatransport-3.0.7/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-27 22:31:25.000000 datatransport-3.0.7/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/
--rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1539 2023-07-27 20:11:25.000000 datatransport-3.0.7/src/datatransport/accessmixin.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/commands/
--rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/cancelnewsgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/console.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/listnewsgroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transport_create_app.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportctl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportd.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportps.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.7/src/datatransport/commands/viewlog.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)     5325 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/DiskMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6212 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/EventMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4130 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/FilePost.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     9573 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/FileStore.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5308 2023-07-27 07:14:43.000000 datatransport-3.0.7/src/datatransport/components/GroupControl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/InstrumentStatus.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4975 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/NewsGateway.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7859 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/NewsgroupMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/PageKit.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/PlotTool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    12712 2023-07-27 07:14:43.000000 datatransport-3.0.7/src/datatransport/components/PostDataFiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/RealTimeFeed.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/ResourceMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6942 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/Scheduler.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/SyncPoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11743 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/WatchURL.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      645 2023-07-27 16:42:50.000000 datatransport-3.0.7/src/datatransport/components/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    52705 2023-07-26 23:57:41.000000 datatransport-3.0.7/src/datatransport/components/archivegroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2736 2023-07-27 16:48:23.000000 datatransport-3.0.7/src/datatransport/components/directoryservice.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5651 2023-07-26 21:50:04.000000 datatransport-3.0.7/src/datatransport/components/filewatch.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1304 2023-07-27 18:05:17.000000 datatransport-3.0.7/src/datatransport/configcomponent.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3065 2023-07-26 20:39:27.000000 datatransport-3.0.7/src/datatransport/directory.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-25 17:37:52.000000 datatransport-3.0.7/src/datatransport/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10799 2023-07-27 21:09:07.000000 datatransport-3.0.7/src/datatransport/newspoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8209 2023-07-27 21:58:14.000000 datatransport-3.0.7/src/datatransport/newsposter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    34275 2023-07-27 21:22:50.000000 datatransport-3.0.7/src/datatransport/newstool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    15543 2023-07-27 22:31:13.000000 datatransport-3.0.7/src/datatransport/processclient.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    13509 2023-07-20 22:01:05.000000 datatransport-3.0.7/src/datatransport/processgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/root.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/etc/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/templates/etc/transportd.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/groups/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4747 2023-07-27 05:02:15.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/watchdog.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.7/src/datatransport/transportconfig.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportlogger.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportmanager.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/utilities/
--rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4170 2023-07-27 03:27:27.000000 datatransport-3.0.7/src/datatransport/utilities/patterntemplate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/removefile.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/sizedesc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/xmlrpcdeferred.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4505 2023-07-27 16:47:53.000000 datatransport-3.0.7/src/datatransport/xmlrpcserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)     6376 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)     1330 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/entry_points.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/tests/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/tests/__pycache__/
--rw-rw-r--   0 valentic   (500) valentic   (500)     8651 2023-07-27 01:45:55.000000 datatransport-3.0.7/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2113 2023-07-27 01:45:50.000000 datatransport-3.0.7/tests/test_utilities_pattern.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_removefiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_sizedesc.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    50330 2023-07-28 01:50:10.000000 datatransport-3.0.8/CHANGES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.8/INSTALL
+-rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.8/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.8/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.8/MIGRATION
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 16:45:24.000000 datatransport-3.0.8/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.8/README.rst
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/.coverage
+-rw-rw-r--   0 valentic   (500) valentic   (500)      121 2023-07-27 16:34:01.000000 datatransport-3.0.8/contrib/examples/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2333 2023-07-26 23:11:05.000000 datatransport-3.0.8/contrib/examples/archivegroups/archivegroups.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-26 21:56:24.000000 datatransport-3.0.8/contrib/examples/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/component/component.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1854 2023-07-27 04:14:34.000000 datatransport-3.0.8/contrib/examples/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/diskmonitor/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-28 00:07:08.000000 datatransport-3.0.8/contrib/examples/diskmonitor/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      552 2023-07-28 01:46:30.000000 datatransport-3.0.8/contrib/examples/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/environ/environ.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1097 2023-07-26 20:31:33.000000 datatransport-3.0.8/contrib/examples/environ/environ.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.8/contrib/examples/examples.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/filepost/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:33:18.000000 datatransport-3.0.8/contrib/examples/filepost/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 03:19:27.000000 datatransport-3.0.8/contrib/examples/filepost/filepost.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-28 02:16:01.000000 datatransport-3.0.8/contrib/examples/filepost/watcher.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/filewatch/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-26 21:29:22.000000 datatransport-3.0.8/contrib/examples/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/getbytes/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      874 2023-07-26 21:19:37.000000 datatransport-3.0.8/contrib/examples/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/groupcontrol/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      636 2023-07-28 09:48:31.000000 datatransport-3.0.8/contrib/examples/groupcontrol/groupcontrol.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      996 2023-07-28 09:39:17.000000 datatransport-3.0.8/contrib/examples/groupcontrol/request.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/hello/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.8/contrib/examples/hello/hello.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      876 2023-07-26 20:27:09.000000 datatransport-3.0.8/contrib/examples/hello/helloworld.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/init/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1020 2023-07-26 20:28:47.000000 datatransport-3.0.8/contrib/examples/init/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/init/init.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/messagebox/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/messagebox.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/poll_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/poll_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/post_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/messagebox/post_text.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/postpoll/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1090 2023-07-26 21:11:35.000000 datatransport-3.0.8/contrib/examples/postpoll/poll_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      918 2023-07-26 20:43:33.000000 datatransport-3.0.8/contrib/examples/postpoll/poll_text.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1162 2023-07-26 20:46:08.000000 datatransport-3.0.8/contrib/examples/postpoll/post_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1010 2023-07-26 20:34:43.000000 datatransport-3.0.8/contrib/examples/postpoll/post_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/postpoll/postpoll.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/rotatelogs/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      868 2023-07-26 21:20:22.000000 datatransport-3.0.8/contrib/examples/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/service/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1194 2023-07-27 16:36:41.000000 datatransport-3.0.8/contrib/examples/service/client.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/directory.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/echo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/service/service.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/spawn/spawn.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1304 2023-07-26 21:26:34.000000 datatransport-3.0.8/contrib/examples/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples/watchdog/
+-rwxr-xr-x   0 valentic   (500) valentic   (500)     1061 2023-07-26 21:27:53.000000 datatransport-3.0.8/contrib/examples/watchdog/crasher.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/watchdog/init_crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/archivegroups.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/component/component.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/config/config.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/config/config.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/diskmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/environ/environ.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/environ/environ.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/eventmonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/eventmonitor/serverstate.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/plugin.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/instrumentstatus/postdata
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/README
+-rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/multipoll.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/reader.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/multipoll/writer.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/plottool/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/plottool/datasource.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/plottool/plottool.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/checkdate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/postdatafiles/postdatafiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/resourcemonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/spawn/spawn.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/splitfiles/splitfiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/poller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/source.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/syncpoller/syncpoller.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/test.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/wait/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/wait/timer.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/wait/wait.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/examples.v2/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/contrib/utils/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/createnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/getarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/postarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/rebuilddatabase
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/relaynewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/rmnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.8/contrib/utils/watchtransport
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2553 2023-07-28 05:11:21.000000 datatransport-3.0.8/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-29 16:45:24.000000 datatransport-3.0.8/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1539 2023-07-27 20:11:25.000000 datatransport-3.0.8/src/datatransport/accessmixin.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/commands/
+-rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/cancelnewsgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/console.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/listnewsgroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transport_create_app.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportctl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportd.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/commands/transportps.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.8/src/datatransport/commands/viewlog.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6359 2023-07-28 01:54:18.000000 datatransport-3.0.8/src/datatransport/components/EventMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/InstrumentStatus.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4978 2023-07-27 23:58:31.000000 datatransport-3.0.8/src/datatransport/components/NewsGateway.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8153 2023-07-29 16:44:12.000000 datatransport-3.0.8/src/datatransport/components/NewsgroupMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/PageKit.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-28 09:57:05.000000 datatransport-3.0.8/src/datatransport/components/PlotTool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    12712 2023-07-27 07:14:43.000000 datatransport-3.0.8/src/datatransport/components/PostDataFiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/RealTimeFeed.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/ResourceMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6942 2023-07-27 07:14:44.000000 datatransport-3.0.8/src/datatransport/components/Scheduler.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/components/SyncPoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11743 2023-07-27 07:14:44.000000 datatransport-3.0.8/src/datatransport/components/WatchURL.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      611 2023-07-28 05:11:11.000000 datatransport-3.0.8/src/datatransport/components/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    52705 2023-07-26 23:57:41.000000 datatransport-3.0.8/src/datatransport/components/archivegroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2736 2023-07-27 16:48:23.000000 datatransport-3.0.8/src/datatransport/components/directoryservice.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5993 2023-07-28 01:52:06.000000 datatransport-3.0.8/src/datatransport/components/diskmonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4945 2023-07-28 03:31:35.000000 datatransport-3.0.8/src/datatransport/components/filepost.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5651 2023-07-26 21:50:04.000000 datatransport-3.0.8/src/datatransport/components/filewatch.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5811 2023-07-28 09:53:16.000000 datatransport-3.0.8/src/datatransport/components/groupcontrol.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1304 2023-07-27 18:05:17.000000 datatransport-3.0.8/src/datatransport/configcomponent.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3065 2023-07-26 20:39:27.000000 datatransport-3.0.8/src/datatransport/directory.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-29 16:44:35.000000 datatransport-3.0.8/src/datatransport/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10799 2023-07-27 21:09:07.000000 datatransport-3.0.8/src/datatransport/newspoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8209 2023-07-27 21:58:14.000000 datatransport-3.0.8/src/datatransport/newsposter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    34276 2023-07-28 09:22:06.000000 datatransport-3.0.8/src/datatransport/newstool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    15585 2023-07-28 09:43:01.000000 datatransport-3.0.8/src/datatransport/processclient.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    13509 2023-07-20 22:01:05.000000 datatransport-3.0.8/src/datatransport/processgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/root.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/etc/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/templates/etc/transportd.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/groups/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4747 2023-07-27 05:02:15.000000 datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/watchdog.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.8/src/datatransport/transportconfig.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportlogger.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportmanager.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/transportserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport/utilities/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4170 2023-07-27 03:27:27.000000 datatransport-3.0.8/src/datatransport/utilities/patterntemplate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/removefile.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/sizedesc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.8/src/datatransport/utilities/xmlrpcdeferred.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4505 2023-07-27 16:47:53.000000 datatransport-3.0.8/src/datatransport/xmlrpcserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6623 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1278 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/entry_points.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-29 16:45:24.000000 datatransport-3.0.8/src/datatransport.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-29 16:45:24.000000 datatransport-3.0.8/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8651 2023-07-27 01:45:55.000000 datatransport-3.0.8/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2113 2023-07-27 01:45:50.000000 datatransport-3.0.8/tests/test_utilities_pattern.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_removefiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.8/tests/test_utilities_sizedesc.py
```

### Comparing `datatransport-3.0.7/CHANGES.txt` & `datatransport-3.0.8/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+2023-07-27  Todd Valentic
+    - DiskMonitor updated.
+
+    - Release 3.0.8
+
 2023-07-20  Todd Valentic
-    - Process group. Do not log error if no clients listed
-    - Process group. Change default shutdown timeout to be 30s
-    - Process group. Change shutdown timeout to be a timedelta
-    - Process client. Add stop() to request process to stop.
+    - ProcessGroup. Do not log error if no clients listed
+    - ProcessGroup. Change default shutdown timeout to be 30s
+    - ProcessGroup. Change shutdown timeout to be a timedelta
+    - ProcessClient. Add stop() to request process to stop.
     - NewsTool. Ensure enable is boolean
     - PatternTemplate. Missing pattern check. Update test.
     - NewsPoller. Code cleanup. Use AccessMixin
     - NewsPoster. Code cleanup. Use AccessMixin
     - NewsTool. Fix host/port setting
+    - ProcessClient. Make sure to logout in abort() 
 
     - Release 3.0.7
 
 2023-07-12  Todd Valentic
     - Make sure viewlog opens new files
     - Release 3.0.6
```

### Comparing `datatransport-3.0.7/INSTALL` & `datatransport-3.0.8/INSTALL`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/LICENSE` & `datatransport-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/MIGRATION` & `datatransport-3.0.8/MIGRATION`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/PKG-INFO` & `datatransport-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.7
+Version: 3.0.8
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.7/contrib/examples/.coverage` & `datatransport-3.0.8/contrib/examples/.coverage`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/archivegroups/archivegroups.conf` & `datatransport-3.0.8/contrib/examples/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/archivegroups/postdata.py` & `datatransport-3.0.8/contrib/examples/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/component/component.conf` & `datatransport-3.0.8/contrib/examples/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/component/demo.py` & `datatransport-3.0.8/contrib/examples/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/environ/environ.py` & `datatransport-3.0.8/contrib/examples/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/filewatch/createdata.py` & `datatransport-3.0.8/contrib/examples/filepost/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/getbytes/demo.py` & `datatransport-3.0.8/contrib/examples/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/getbytes/getbytes.conf` & `datatransport-3.0.8/contrib/examples/getbytes/getbytes.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/hello/helloworld.py` & `datatransport-3.0.8/contrib/examples/hello/helloworld.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/init/demo.py` & `datatransport-3.0.8/contrib/examples/init/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/messagebox/messagebox.conf` & `datatransport-3.0.8/contrib/examples/messagebox/messagebox.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/messagebox/poll_file.py` & `datatransport-3.0.8/contrib/examples/messagebox/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/messagebox/poll_text.py` & `datatransport-3.0.8/contrib/examples/messagebox/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/messagebox/post_file.py` & `datatransport-3.0.8/contrib/examples/messagebox/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/messagebox/post_text.py` & `datatransport-3.0.8/contrib/examples/messagebox/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/postpoll/poll_file.py` & `datatransport-3.0.8/contrib/examples/postpoll/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/postpoll/poll_text.py` & `datatransport-3.0.8/contrib/examples/postpoll/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/postpoll/post_file.py` & `datatransport-3.0.8/contrib/examples/postpoll/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/postpoll/post_text.py` & `datatransport-3.0.8/contrib/examples/postpoll/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/postpoll/postpoll.conf` & `datatransport-3.0.8/contrib/examples/postpoll/postpoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/rotatelogs/counter.py` & `datatransport-3.0.8/contrib/examples/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/service/client.py` & `datatransport-3.0.8/contrib/examples/service/client.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/service/echo.py` & `datatransport-3.0.8/contrib/examples/service/echo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/service/service.conf` & `datatransport-3.0.8/contrib/examples/service/service.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/spawn/spawner.py` & `datatransport-3.0.8/contrib/examples/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/watchdog/crasher.py` & `datatransport-3.0.8/contrib/examples/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples/watchdog/init_crasher.py` & `datatransport-3.0.8/contrib/examples/watchdog/init_crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/README` & `datatransport-3.0.8/contrib/examples.v2/README`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/archivegroups/archivegroups.conf` & `datatransport-3.0.8/contrib/examples.v2/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/archivegroups/postdata.py` & `datatransport-3.0.8/contrib/examples.v2/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/component/component.conf` & `datatransport-3.0.8/contrib/examples.v2/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/component/demo.py` & `datatransport-3.0.8/contrib/examples.v2/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/config/config.py` & `datatransport-3.0.8/contrib/examples.v2/config/config.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/environ/environ.py` & `datatransport-3.0.8/contrib/examples.v2/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/eventmonitor/eventmonitor.conf` & `datatransport-3.0.8/contrib/examples.v2/eventmonitor/eventmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/eventmonitor/serverstate.py` & `datatransport-3.0.8/contrib/examples.v2/eventmonitor/serverstate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/filewatch/createdata.py` & `datatransport-3.0.8/contrib/examples.v2/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/getbytes/demo.py` & `datatransport-3.0.8/contrib/examples.v2/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/instrumentstatus/instrumentstatus.conf` & `datatransport-3.0.8/contrib/examples.v2/instrumentstatus/instrumentstatus.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/instrumentstatus/postdata` & `datatransport-3.0.8/contrib/examples.v2/instrumentstatus/postdata`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/multipoll/multipoll.conf` & `datatransport-3.0.8/contrib/examples.v2/multipoll/multipoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/multipoll/writer.py` & `datatransport-3.0.8/contrib/examples.v2/multipoll/writer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf` & `datatransport-3.0.8/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/plottool/datasource.py` & `datatransport-3.0.8/contrib/examples.v2/plottool/datasource.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/plottool/plottool.conf` & `datatransport-3.0.8/contrib/examples.v2/plottool/plottool.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/postdatafiles/createfiles.py` & `datatransport-3.0.8/contrib/examples.v2/postdatafiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/postdatafiles/postdatafiles.conf` & `datatransport-3.0.8/contrib/examples.v2/postdatafiles/postdatafiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/rotatelogs/counter.py` & `datatransport-3.0.8/contrib/examples.v2/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/spawn/spawner.py` & `datatransport-3.0.8/contrib/examples.v2/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/splitfiles/createfiles.py` & `datatransport-3.0.8/contrib/examples.v2/splitfiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/splitfiles/splitfiles.conf` & `datatransport-3.0.8/contrib/examples.v2/splitfiles/splitfiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/syncpoller/source.py` & `datatransport-3.0.8/contrib/examples.v2/syncpoller/source.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/syncpoller/syncpoller.conf` & `datatransport-3.0.8/contrib/examples.v2/syncpoller/syncpoller.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/wait/timer.py` & `datatransport-3.0.8/contrib/examples.v2/wait/timer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/examples.v2/watchdog/crasher.py` & `datatransport-3.0.8/contrib/examples.v2/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/createnewsgroup` & `datatransport-3.0.8/contrib/utils/createnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/getarticle` & `datatransport-3.0.8/contrib/utils/getarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/postarticle` & `datatransport-3.0.8/contrib/utils/postarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/rebuilddatabase` & `datatransport-3.0.8/contrib/utils/rebuilddatabase`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/relaynewsgroup` & `datatransport-3.0.8/contrib/utils/relaynewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/rmnewsgroup` & `datatransport-3.0.8/contrib/utils/rmnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/contrib/utils/watchtransport` & `datatransport-3.0.8/contrib/utils/watchtransport`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/pyproject.toml` & `datatransport-3.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -41,19 +41,18 @@
 [project.urls]
 homepage="https://github.com/valentic/datatransport"
 repository="https://github.com/valentic/datatransport"
 
 [project.scripts]
     archivegroups = "datatransport.components.archivegroups:main"
     directoryservice = "datatransport.components.directoryservice:main"
-    diskmonitor = "datatransport.components.DiskMonitor:main"
-    filepost = "datatransport.components.FilePost:main"
-    filestore = "datatransport.components.FileStore:main"
+    diskmonitor = "datatransport.components.diskmonitor:main"
+    filepost = "datatransport.components.filepost:main"
     filewatch = "datatransport.components.filewatch:main"
-    groupcontrol = "datatransport.components.GroupControl:main"
+    groupcontrol = "datatransport.components.groupcontrol:main"
     instrumentstatus = "datatransport.components.InstrumentStatus:main"
     newsgateway = "datatransport.components.NewsGateway:main"
     newsgroupmonitor = "datatransport.components.NewsgroupMonitor:main"
     plottool = "datatransport.components.PlotTool:main"
     postdatafiles = "datatransport.components.PostDataFiles:main"
     realtimefeed = "datatransport.components.RealTimeFeed:main"
     resourcemonitor = "datatransport.components.ResourceMonitor:main"
```

### Comparing `datatransport-3.0.7/src/datatransport/__init__.py` & `datatransport-3.0.8/src/datatransport/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/accessmixin.py` & `datatransport-3.0.8/src/datatransport/accessmixin.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/cancelnewsgroup.py` & `datatransport-3.0.8/src/datatransport/commands/cancelnewsgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/console.py` & `datatransport-3.0.8/src/datatransport/commands/console.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/listnewsgroups.py` & `datatransport-3.0.8/src/datatransport/commands/listnewsgroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/transport_create_app.py` & `datatransport-3.0.8/src/datatransport/commands/transport_create_app.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/transportctl.py` & `datatransport-3.0.8/src/datatransport/commands/transportctl.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/transportd.py` & `datatransport-3.0.8/src/datatransport/commands/transportd.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/transportps.py` & `datatransport-3.0.8/src/datatransport/commands/transportps.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/commands/viewlog.py` & `datatransport-3.0.8/src/datatransport/commands/viewlog.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/DiskMonitor.py` & `datatransport-3.0.8/src/datatransport/components/diskmonitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,196 @@
+#!/usr/bin/env python3
+"""Disk Monitor Component"""
+
 ##########################################################################
 #
 #   DiskMonitor
 #
-#   Monitor disk space using results in ResourceMonitor
-#   snapshots. Produce trouble alerts when when running low.
+#   This process client monitors the system disk usage reported in the
+#   output messages from the ResourceMonitor client running in the
+#   ServerMonitor process group. A trouble message will be sent when
+#   disk space is running low.
 #
 #   2004-02-01	Todd Valentic
 #               Initial implementation.
 #
 #   2008-11-13  Todd Valentic
 #               Use SafeConfigParser
 #
 #   2016-12-23  Todd Valentic
 #               Use external texttable
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #               Python3 updates
-#                   ConfigParser -> sapphire.Parser 
+#                   ConfigParser -> sapphire.Parser
 #                   StringIO -> io.StringIO
 #                   sizeDesc -> size_desc
 #                   NewsPoster, NewsPoller
 #
+#   2023-07-27  Todd Valentic
+#               Updated for transport3 / python3
+#
 ##########################################################################
 
-import io
 import fnmatch
+import pathlib
 import sys
 
 import texttable
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport import NewsPoller
 from datatransport import newstool
-from datatransport import ConfigComponent
 from datatransport.utilities import size_desc
 
 import sapphire_config as sapphire
 
 
 class DiskMonitor(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
         self.news_poller = NewsPoller(self, callback=self.process)
         self.main = self.news_poller.main
 
+        self.cachefile = pathlib.Path("history")
         self.load_history()
 
-        self.includes = self.get_list("mounts.include", "*")
-        self.excludes = self.get_list("mounts.exclude", "")
-        self.maxusedpct = self.get_float("max.percent.used", 95)
+        sysmnts = "/dev* /run* /sys*"
+
+        self.includes = self.config.get_list("mounts.include", "*")
+        self.excludes = self.config.get_list("mounts.exclude", sysmnts)
+        self.max_used_pct = self.config.get_float("max.percent.used", 95)
 
     def load_history(self):
+        """Load history from cache"""
+
         self.history = sapphire.Parser()
-        self.history.read("history")
+        self.history.read(self.cachefile)
 
     def save_history(self):
-        self.history.write(open("history", "w"))
+        """Save history to cache"""
+
+        with self.cachefile.open("w", encoding="utf-8") as f:
+            self.history.write(f)
 
     def update_history(self, prefix, stats, mount):
+        """Update history"""
 
         if not self.history.has_section(mount):
             self.history.add_section(mount)
 
         for option in stats.options(mount):
             value = stats.get(mount, option)
             self.history.set(mount, f"{prefix}.{option}", value)
 
     def checkmount(self, stats, mount):
+        """Check mounted filesystem"""
 
         if self.history.has_section(mount):
-            prevalarm = self.history.get_int(mount, "last.alarm")
+            prevalarm = self.history.get_boolean(mount, "last.alarm")
         else:
-            prevalarm = 0
+            prevalarm = False
 
         usedpct = stats.get_float(mount, "usedpct")
-        curalarm = usedpct >= self.maxusedpct
+        curalarm = usedpct >= self.max_used_pct
 
         setalarm = not prevalarm and curalarm
         clearalarm = prevalarm and not curalarm
 
         if setalarm:
-            self.log.info("Warning: %s is %d%% full" % (mount, usedpct))
+            self.log.info("Warning: %s is %d%% full", mount, usedpct)
             notes = "Alarm set"
         elif clearalarm:
-            self.log.info("Cleared: %s is now only %d%% full" % (mount, usedpct))
+            self.log.info("Cleared: %s is now only %d%% full", mount, usedpct)
             notes = "Cleared alarm"
         elif curalarm and prevalarm:
             notes = "Low space alarm"
         else:
             notes = ""
 
         self.update_history("last", stats, mount)
         self.history.set(mount, "last.alarm", str(curalarm))
         self.history.set(mount, "last.notes", notes)
 
         return setalarm or clearalarm
 
     def check(self, stats):
+        """Check mounted filesystems"""
 
-        self.log.debug("Checking disk usage (limit is %d%%)" % self.maxusedpct)
+        self.log.debug("Checking disk usage (limit is %d%%)", self.max_used_pct)
 
         # Patchup for development debugging
         if not stats.has_section("System"):
             stats.add_section("System")
 
-        mounts = stats.get("System", "mounts").split()
+        mounts = stats.get_list("System", "mounts")
 
         for include in self.includes:
-            mounts = filter(lambda x: fnmatch.fnmatch(x, include), mounts)
+            mounts = [m for m in mounts if fnmatch.fnmatch(m, include)]
         for exclude in self.excludes:
-            mounts = filter(lambda x: not fnmatch.fnmatch(x, exclude), mounts)
+            mounts = [m for m in mounts if not fnmatch.fnmatch(m, exclude)]
 
         report = 0
 
         for mount in mounts:
             report += self.checkmount(stats, mount)
 
         if report:
             message = self.alert_message(mounts)
             try:
                 self.news_poster.post_text(message, date=self.timestamp)
-            except:
-                self.log.exception("Problem posting message")
+            except Exception as e: # pylint: disable=broad-exception-caught
+                self.log.exception("Problem posting message: %s", e)
 
     def alert_message(self, mounts):
+        """Return an alert message"""
 
         timestr = self.timestamp.strftime("%Y-%m-%d %H:%M")
 
         message = "\n"
-        message += "Disk Space Report - %s\n\n" % timestr
+        message += f"Disk Space Report - {timestr}\n\n"
 
         table = texttable.Texttable()
-        table.header(["Mount", "Total", "Avail", "Used", "% Full", "Notes"])
+        table.header(["Mount", "Total", "Used", "Avail", "% Full", "Notes"])
         table.set_cols_align(["l", "r", "r", "r", "r", "l"])
 
         for mount in mounts:
-
-            total = long(self.history.get(mount, "last.totalbytes"))
-            used = long(self.history.get(mount, "last.usedbytes"))
-            free = long(self.history.get(mount, "last.freebytes"))
+            total = self.history.get_float(mount, "last.totalbytes")
+            used = self.history.get_float(mount, "last.usedbytes")
+            free = self.history.get_float(mount, "last.freebytes")
             usedpct = self.history.get_float(mount, "last.usedpct")
 
             row = [mount]
             row.append(size_desc(total))
             row.append(size_desc(used))
             row.append(size_desc(free))
-            row.append("%d%%" % usedpct)
+            row.append(f"{usedpct:0.1f}%")
             row.append(self.history.get(mount, "last.notes"))
 
             table.add_row(row)
 
         message += table.draw()
         message += "\n"
 
         return message
 
     def process(self, message):
+        """Process handler"""
 
-        body = message.get_payload()
-        file = io.StringIO(body)
-        stats = sapphire.Parser()
-        stats.readfp(file)
+        stats = newstool.as_config(message)
 
         self.timestamp = newstool.message_date(message)
-        self.history.set("DEFAULT", "last.time", self.timestamp)
+        self.history.set("DEFAULT", "last.time", str(self.timestamp))
 
         self.check(stats)
         self.save_history()
 
 
 def main():
+    """Script entry point"""
     DiskMonitor(sys.argv).run()
```

### Comparing `datatransport-3.0.7/src/datatransport/components/EventMonitor.py` & `datatransport-3.0.8/src/datatransport/components/EventMonitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-############################################################
+#!/usr/bin/env python3
+"""Event Monitor Component"""
+
+##########################################################################
 #
 #   Event Monitor
 #
 #   2009-03-14  Todd Valentic
 #               Initial implementation.
 #
 #   2010-03-22  Todd Valentic
@@ -16,15 +19,18 @@
 #               Use datetime.timezone.utc
 #
 #   2022-10-19  Todd Valentic
 #               Python3 port
 #                   use get_ methods
 #                   use sapphire.Parser
 #
-############################################################
+#   2023-07-27  Todd Valentic
+#               Updated for transport3 / python3
+#
+##########################################################################
 
 import os
 import datetime
 
 from dateutil import parser
 
 from datatransport import ConfigComponent
@@ -104,15 +110,15 @@
     def add_states(self, *pos):
         for name in pos:
             self.states[name] = self.state_factory(name, self)
 
     def update(self, state, timestamp=None):
 
         if timestamp is None:
-            timestamp = datetime.datetime.now(utc)
+            timestamp = self.now()
 
         self.current.update(timestamp)
 
         if self.cur_state == state:
             self.changed = False
         else:
             self.history.append(self.current.history_entry())
```

### Comparing `datatransport-3.0.7/src/datatransport/components/FilePost.py` & `datatransport-3.0.8/src/datatransport/components/filepost.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env/python3
+"""File Post Component"""
+
 ##########################################################################
 #
 #   FilePost
 #
 #   This transport component watches for specified files to appear and
 #   posts them into a newsgroup. If the newsgroup does not exist, it
 #   will be created. Multiple files can be listed and they will be posted
@@ -34,95 +37,117 @@
 #
 #   2022-10-12  Todd Valentic
 #               Python3 port
 #                   Transport -> datatransport
 #                   removeFile -> remove_file
 #                   NewsPoster
 #
+#   2023-07-27  Todd Valentic
+#               Updated for transport3 / python3
+#
 ##########################################################################
 
-import os
 import sys
-import glob
-import time
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport import ConfigComponent
 from datatransport.utilities import remove_file
 
 
 class Watcher(ConfigComponent):
-    def __init__(self, name, parent):
-        ConfigComponent.__init__(self, "watch", name, parent)
-    
+    """Watch group component"""
+
+    def __init__(self, *p, **kw):
+        ConfigComponent.__init__(self, "watch", *p, **kw)
+
         self.news_poster = NewsPoster(self)
 
-        self.file_patterns = self.get_list("files")
-        self.remove_files = self.get_boolean("removefiles", True)
-        self.group_files = self.get_boolean("groupfiles", False)
-
-        self.log.info("Watch: %s" % name)
-        self.log.info("  Posting to %s" % self.get("post.newsgroup"))
-        self.log.info("  Watching for: %s" % self.file_patterns)
+        self.watchpath = self.config.get_path("path", ".")
+        self.filespecs = self.config.get_list("files")
+        self.remove_files = self.config.get_boolean("removefiles", True)
+        self.group_files = self.config.get_boolean("groupfiles", False)
+
+        if not self.filespecs:
+            self.abort("No watch files listed in the config file")
+
+        self.log.info("Posting to %s", self.config.get("post.newsgroup"))
+        self.log.info("Watching path: %s", self.watchpath)
+        self.log.info("Watching for: %s", self.filespecs)
 
     def find_files(self):
+        """Find matching files to post"""
 
         filenames = []
 
-        for pattern in self.file_patterns:
-            filenames.extend(glob.glob(pattern))
+        for filespec in self.filespecs:
+            filenames.extend(self.watchpath.glob(filespec))
 
-        filenames = [f for f in filenames if os.path.isfile(f)]
-        filenames.sort()
+        filenames = [f for f in filenames if f.is_file()]
 
-        if self.group_files and filenames:
-            filenames = [filenames]
-
-        return filenames
+        return sorted(filenames)
 
-    def check(self):
+    def process(self):
+        """Check for new files"""
 
-        files = self.find_files()
+        filenames = self.find_files()
 
-        if not files:
-            self.log.debug("No files present, sleeping")
+        if not filenames:
+            self.log.debug("No files present")
             return
 
-        for filegroup in files:
+        if self.group_files:
+            filenames = [filenames]
+
+        for filegroup in filenames:
+            starttime = self.now()
 
             try:
-                starttime = time.time()
                 self.news_poster.post(filegroup)
-                elapsed = time.time() - starttime
-                self.log.info("Files posted (%.2f s): %s" % (elapsed, filegroup))
-            except:
-                self.log.exception("Problem posting files")
+            except Exception as e:  # pylint: disable=broad-exception-caught
+                self.log.exception("Problem posting files: %s", e)
                 return
 
+            elapsed = (self.now() - starttime).total_seconds()
+            
+            if isinstance(filegroup, list):
+                names = [str(n) for n in filegroup]
+            else:
+                names = filegroup
+
+            self.log.info("Files posted (%0.2fs): %s", elapsed, names)
+
             if self.remove_files:
                 try:
                     remove_file(filegroup)
-                except:
-                    self.log.exception("Problem deleting file: %s" % filegroup)
+                except OSError as e:
+                    self.log.exception("Problem deleting file %s: %s", filegroup, e)
 
 
 class FilePost(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
-        self.rate = self.get_rate("rate")
-        self.watches = self.get_components("watches", Watcher)
+        self.rate = self.config.get_rate("pollrate")
+        self.watches = self.config.get_components("watches", factory=Watcher)
 
     def process(self):
+        """Process each file watch group"""
 
         for watch in self.watches.values():
-            watch.check()
+            watch.process()
+
+            if self.is_stopped():
+                break
 
     def main(self):
+        """Main application"""
 
         while self.wait(self.rate):
             self.process()
 
 
 def main():
+    """Script entry point"""
     FilePost(sys.argv).run()
```

### Comparing `datatransport-3.0.7/src/datatransport/components/GroupControl.py` & `datatransport-3.0.8/src/datatransport/templates/groups/ServerMonitor/watchdog.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,163 @@
-###########################################################################
-#
-#  GroupControl
-#
-#  This script polls a "control" newsgroup looking for messages to start
-#  and stop process groups.
-#
-#  History:
-#
-#   1.0.0   2000-01-19  TAV
-#           Initial implementation
-#
-#   1.0.1   2000-02-22  TAV
-#           Added the maillist reporting feature.
-#
-#   1.0.2   2000-02-26  TAV
-#           Improved wording and look of the mailing list message.
+#!/usr/bin/env python
+"""Watchdog"""
+
+############################################################################
 #
-#   1.0.3   2000-04-25  TAV
-#           Added connect() method to retry connecting to server incase it
-#               is busy during the initial contact.
+#   watchdog
 #
-#   1.0.4   2000-04-29  TAV
-#           Fixed bug in connect call.
+#   This script monitors the process group clients and reports any that
+#   were started but have seemed to stop running (they are registered but
+#   don't show up as an active process). In this case, the client is
+#   restarted. Messages are also sent to the watchdog list in this case.
 #
-#   1.0.5   2001-11-13  TAV
-#           Added prefix and postfix config options.
+#   History:
 #
-#   1.0.6   2001-12-26  TAV
-#           Changed tav -> sri
+#   2000-04-24  TAV
+#               Initial implementation
 #
-#   1.0.7   2002-01-25  Todd Valentic
-#           Updated to new NewsPollMixin interface.
+#   2002-01-20  Todd Valentic
+#               Improved wording of notification message.
 #
-#   1.0.8   2002-08-27  Todd Valentic
-#           Setup through configure script.
-#           sri.transport -> Transport
-#           use socket.getfqdn() versus sri.util.hostname()
+#   2002-01-24  Todd Valentic
+#               Added timestamp to message body.
 #
-#   1.0.9   2003-03-21  Todd Valentic
-#           Code cleanups. Use self.wait in connect()
-#           Use string methods instead of string module
-#           Split out baseclass from driver
+#   2002-01-25  Todd Valentic
+#               Added check for self.running
 #
-#   1.0.10  2003-05-09  Todd Valentic
-#           Moved the connection code up into __init__()
-#               we were sleeping 60 seconds on the first
-#               message process otherwise.
+#   2002-05-19  Todd Valentic
+#               Fixed call to restart client (now include arg string).
 #
-#   1.0.11  2003-06-30  Todd Valentic
-#           Updated to new NewsPoller interface.
+#   2002-08-28  Todd Valentic
+#               sri.transport -> Transport
+#               python -> python2
 #
-#   1.0.12  2004-08-08  Todd Valentic
-#           Use new XML-RPC interface to transport server.
+#   2003-04-15  Todd Valentic
+#               Changed config parameter pollrate -> rate
+#               Rate now specified in days/hours/mins/secs
 #
-#   1.0.13  2004-12-27  Todd Valentic
-#           Convert from mx.DateTime to datetime
+#   2004-02-08  Todd Valentic
+#               Use DeltaTime for rate
+#               Use string methods
 #
-#   1.0.14  2006-01-18  Todd Valentic
-#           Minor code cleanups
+#   2004-08-08  Todd Valentic
+#               Updated to new XML-RPC server interface
 #
-#   1.0.15  2006-10-26  Todd Valentic
-#           Use new CurrentTime method
+#   2004-08-25  Todd Valentic
+#               Converted to directly reading /proc instead of using ps
 #
-#   2022-10-07  Todd Valentic
-#               Reorder imports
-#               Python3 migration:
-#                   exception handling
-#                   NewsPoller, NewsPoster
+#   2004-12-30  Todd Valentic
+#               Convert from mx.DateTime to datetime
 #
-#   2023-07-28  Todd Valentic
-#               Updated for transport3 / python3
+#   2022-10-06  Todd Valentic
+#               Updated for transport3/python3
+#   
+#   2023-07-26  Todd Valentic
+#               Use config getters
 #
-###########################################################################
+############################################################################
 
-import os
-import socket
+import pathlib
 import sys
 
 from datatransport import ProcessClient
-from datatransport import NewsPoller
 from datatransport import NewsPoster
-from datatransport import newstool
 
 
-class GroupControl(ProcessClient):
+class Watchdog(ProcessClient):
+    """Watchdog Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
-        self.news_poster = NewsPoster(self)
-        self.news_poller = NewsPoller(self, callback=self.process)
-        self.main = self.news_poller.main
+    def init(self):
+        super().init()
 
-        self.prefix = self.config.get("prefix", "")
-        self.postfix = self.config.get("postfix", "")
-
-        self.connect()
+        self.news_poster = NewsPoster(self)
+        self.rate = self.config.get_rate("rate", "5m")
 
-    def connect(self):
+    def get_client_pids(self):
+        """Query server for expected client PIDs"""
 
-        self.log.info("Connecting to transport server")
+        pids = {}
 
-        while True:
+        for group in self.server.listgroups():
+            for client, info in self.server.listclients(group).items():
+                pid = info[1]
+                if pid:
+                    pids[pid] = (group, client)
 
-            try:
-                self.server.status()
-                return
-            except:
-                self.log.error("  - waiting 30 seconds to try again.")
+        return pids
 
-            if not self.wait(30):
-                break
+    def get_running_pids(self):
+        """Get list of running PIDs on system"""
 
-    def post_message(self, action, group):
+        proc = pathlib.Path("/proc")
+        return [int(x.name) for x in proc.iterdir() if x.name.isdigit()]
 
-        curtime = self.current_time()
-        hostname = socket.getfqdn()
+    def post_message(self, pid, group_name, client_name):
+        """Post a trouble message"""
 
         body = []
         body.append("")
-        body.append("  The following action has been performed:")
+        body.append(
+            "  The watchdog has detected the following client has stopped running:"
+        )
         body.append("")
-        body.append("      Command  : %s" % action)
-        body.append("      Group    : %s" % group)
-        body.append("      Time     : %s" % curtime)
-        body.append("      Server   : %s" % hostname)
+        body.append(f"      Client name: {client_name}")
+        body.append(f"       Group name: {group_name}")
+        body.append(f"       Process ID: {pid}")
+        body.append(f"       Time stamp: {self.now()}")
+        body.append("")
+        body.append("  The client has been restarted.")
         body.append("")
 
-        header = "%s %s" % (action, group)
+        header = f"Watchdog restart {client_name}"
 
         try:
             self.news_poster.set_subject(header)
             self.news_poster.post_text("\n".join(body))
-        except:
-            self.log.error("Error posting message to mailing list.")
+        except:  # pylint: disable=bare-except
+            self.log.error("Error posting notification message to the news server.")
 
-    def start_group(self, name):
-        self.log.info("Start request for %s" % name)
-        try:
-            self.server.startgroup(name)
-            self.post_message("start", name)
-        except NameError(msg):
-            self.log.info("  The process group does not exist")
+    def restart(self, pid, group, client):
+        """Restart the client process"""
 
-    def stop_group(self, name):
-        self.log.info("Stop request for %s" % name)
-        try:
-            self.server.stopgroup(name)
-            self.post_message("stop", name)
-        except NameError(msg):
-            self.log.info("  The process group does not exist")
+        self.log.info("Process '%s %s' (PID %s) is missing", group, client, pid)
+        self.log.info("  Attempting to restart")
+
+        self.post_message(pid, group, client)
 
-    def process(self, message):
+        try:
+            self.server.startclient(group, client)
+        except:  # pylint: disable=bare-except
+            self.log.info("  Error detected in client restart!")
 
-        filenames = newstool.save_files(message)
+    def checkup(self):
+        """Check to see if any clients have unexpectedly stopped"""
 
-        for filename in filenames:
+        self.log.info("Checking processes")
 
-            if self.is_stopped():
-                return
+        try:
+            self.server.status()
+        except:  # pylint: disable=bare-except
+            self.log.error("Cannot connect to the transport server!")
+            return
 
-            for line in open(filename):
+        client_pids = self.get_client_pids()
+        running_pids = self.get_running_pids()
 
-                try:
-                    command, name = line.split("=")
-                except:
-                    continue
+        for pid, entry in client_pids.items():
+            group, client = entry
 
-                command = command.strip().lower()
-                name = os.path.join(self.prefix, name.strip())
-                name = os.path.join(name, self.postfix)
+            if not pid in running_pids:
+                self.restart(pid, group, client)
 
-                if command == "start":
-                    self.start_group(name)
-                elif command == "stop":
-                    self.stop_group(name)
-                else:
-                    self.log.error("Unknown request: %s" % command)
+    def main(self):
+        """Main application"""
 
-            os.remove(filename)
+        while self.wait(self.rate):
+            self.checkup()
 
 
-def main():
-    GroupControl(sys.argv).run()
+if __name__ == "__main__":
+    Watchdog(sys.argv).run()
```

### Comparing `datatransport-3.0.7/src/datatransport/components/InstrumentStatus.py` & `datatransport-3.0.8/src/datatransport/components/InstrumentStatus.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/NewsGateway.py` & `datatransport-3.0.8/src/datatransport/components/NewsGateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         self.messages.clear()
         self.messages.sync()
 
     @synchronized(lock)
     def read(self, newsgroup):
         """Read entry from cache"""
      
-     return self.messages[newsgroup]
+        return self.messages[newsgroup]
 
     @synchronized(lock)
     def list(self):
         """List cache"""
       
       return self.messages.keys()
```

### Comparing `datatransport-3.0.7/src/datatransport/components/NewsgroupMonitor.py` & `datatransport-3.0.8/src/datatransport/components/NewsgroupMonitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+"""Newsgroup Monitor"""
+
 #####################################################################
 #
 #   Newsgroup Monitor
 #
 #   Monitors the news groups for messages
 #
 #   2009-05-04  Todd Valentic
@@ -18,51 +21,31 @@
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #               Python3 updates:
 #                   StringIO -> io.StringIO
 #               NewsPoller, NewsPoster
 #
+#   2023-07-29  Todd Valentic
+#               Updated for transport3 / python3
+#
 #####################################################################
 
 import io
 import sys
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport import NewsPoller
 from datatransport import ConfigComponent
 from datatransport.components import EventMonitor
 
-
-class FeedGroup(ConfigComponent):
-    def __init__(self, name, parent):
-        ConfigComponent.__init__(self, "feedgroup", name, parent)
-
-        self.log.info("  Feed group: %s" % name)
-
-        localvars = {"feedgroup": name, "section": "%(feedgroup)s:%(feed)s"}
-
-        for key, option in self.optionsdict().items():
-            value = self.get(option, raw=True)
-            localvars["feedgroup." + key] = value
-
-        feeds_dict = self.get_components("feeds", Feed, vars=localvars)
-        self.feeds = feeds_dict.values()
-
-    def check(self):
-
-        for feed in self.feeds:
-            try:
-                feed.check()
-            except:
-                self.log.exception("Problem checking %s" % feed.name)
-
-
 class Feed(EventMonitor.Member):
+    """Feed event monitor"""
+
     def __init__(self, *pos, **kw):
         EventMonitor.Member.__init__(self, "feed", *pos, **kw)
 
         self.news_poster = NewsPoster(self, quiet=True)
         self.news_poller = NewsPoller(self)
         self.main = news_poller.main
 
@@ -161,33 +144,61 @@
         message.append("")
 
         message = "\n".join(message)
 
         return subject, message
 
 
+class FeedGroup(ConfigComponent):
+    """Feed group component"""
+
+    def __init__(self, name, config, parent):
+        ConfigComponent.__init__(self, "feedgroup", name, config, parent)
+
+        self.log.info("  Feed group: %s", name)
+
+        localvars = {"feedgroup": name, "section": "%(feedgroup)s:%(feed)s"}
+
+        # TBD - Do we really need to forward there vars?
+
+        for key, option in self.optionsdict().items():
+            value = self.get(option, raw=True)
+            localvars["feedgroup." + key] = value
+
+        self.feeds = self.config.get_components("feeds", factory=Feed, vars=localvars)
+
+    def check(self):
+
+        for feed in self.feeds.values():
+            try:
+                feed.check()
+            except:
+                self.log.exception("Problem checking %s", feed.name)
+
 class NewsgroupMonitor(ProcessClient):
+    """Process client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.history_poster = NewsPoster(self, prefix="history", quiet=True)
         self.status_poster = NewsPoster(self, prefix="status", quiet=True)
         self.update_poster = NewsPoster(self, prefix="update", quiet=True)
 
         self.log.info("Loading feed groups")
 
-        self.feedgroups = self.get_components("feedgroups", FeedGroup).values()
+        self.feedgroups = self.config.get_components("feedgroups", factory=FeedGroup)
 
         if not self.feedgroups:
             self.feedgroups = [FeedGroup("", self)]
 
         self.feeds = {}
 
-        for feedgroup in self.feedgroups:
-            for feed in feedgroup.feeds:
+        for feedgroup in self.feedgroups.values():
+            for feed in feedgroup.feeds.values():
                 key = "%s:%s" % (feedgroup.name, feed.name)
                 self.feeds[key] = feed
 
         self.tracker = EventMonitor.EventMonitor(self.feeds)
         self.tracker.load("tracker")
 
         self.first_time = True
```

### Comparing `datatransport-3.0.7/src/datatransport/components/PageKit.py` & `datatransport-3.0.8/src/datatransport/components/PageKit.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/PlotTool.py` & `datatransport-3.0.8/src/datatransport/components/PlotTool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/PostDataFiles.py` & `datatransport-3.0.8/src/datatransport/components/PostDataFiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/RealTimeFeed.py` & `datatransport-3.0.8/src/datatransport/components/RealTimeFeed.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/ResourceMonitor.py` & `datatransport-3.0.8/src/datatransport/components/ResourceMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/Scheduler.py` & `datatransport-3.0.8/src/datatransport/components/Scheduler.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/SyncPoller.py` & `datatransport-3.0.8/src/datatransport/components/SyncPoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/WatchURL.py` & `datatransport-3.0.8/src/datatransport/components/WatchURL.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/__init__.py` & `datatransport-3.0.8/src/datatransport/components/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from .archivegroups	    import ArchiveGroups
+from .archivegroups     import ArchiveGroups
 from .directoryservice  import DirectoryService
-from .DiskMonitor	    import DiskMonitor
+from .diskmonitor       import DiskMonitor
 from .filewatch         import FileWatch
-from .FilePost          import FilePost
-from .FileStore         import FileStore
-from .GroupControl	    import GroupControl
+from .filepost          import FilePost
+from .groupcontrol      import GroupControl
 from .InstrumentStatus	import InstrumentStatus
 from .NewsgroupMonitor  import NewsgroupMonitor
 from .PlotTool          import PlotTool
-from .PostDataFiles	    import PostDataFiles
-from .RealTimeFeed	    import RealTimeFeed
+from .PostDataFiles     import PostDataFiles
+from .RealTimeFeed      import RealTimeFeed
 from .ResourceMonitor	import ResourceMonitor
 from .SyncPoller        import SyncPoller
-from .WatchURL		    import WatchURL
+from .WatchURL	        import WatchURL
```

### Comparing `datatransport-3.0.7/src/datatransport/components/archivegroups.py` & `datatransport-3.0.8/src/datatransport/components/archivegroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/directoryservice.py` & `datatransport-3.0.8/src/datatransport/components/directoryservice.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/components/filewatch.py` & `datatransport-3.0.8/src/datatransport/components/filewatch.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/configcomponent.py` & `datatransport-3.0.8/src/datatransport/configcomponent.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/directory.py` & `datatransport-3.0.8/src/datatransport/directory.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/newspoller.py` & `datatransport-3.0.8/src/datatransport/newspoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/newsposter.py` & `datatransport-3.0.8/src/datatransport/newsposter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/newstool.py` & `datatransport-3.0.8/src/datatransport/newstool.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
 
     if not message.is_multipart():
         if write:
             body = message.get_payload()
             filename = path / default
             make_path(filename)
             filename.write_text(body)
-        return [default]
+        return [filename]
 
     filenames = []
 
     counter = 1
     for part in message.walk():
         if part.get_content_maintype() == "multipart":
             continue
```

### Comparing `datatransport-3.0.7/src/datatransport/processclient.py` & `datatransport-3.0.8/src/datatransport/processclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,18 +469,18 @@
     def main(self):
         """Main application"""
 
     def run(self):
         """Run main application, capture any errors to log"""
         try:
             self.init()
-        except:  # pylint: disable=bare-except
+        except Exception:  # pylint: disable=broad-exception-caught
             self.log.exception("Problem detected in init")
             self.abort()
 
         try:
             self.main()
-        except:  # pylint: disable=bare-except
+        except Exception:  # pylint: disable=broad-exception-caught
             self.log.exception("Problem detected in main")
             return  # No clean exit so the watchdog will restart us
 
         self.exit()
```

### Comparing `datatransport-3.0.7/src/datatransport/processgroup.py` & `datatransport-3.0.8/src/datatransport/processgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/templates/etc/transportd.conf` & `datatransport-3.0.8/src/datatransport/templates/etc/transportd.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/watchdog.py` & `datatransport-3.0.8/src/datatransport/xmlrpcserver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,157 @@
-#!/usr/bin/env python
-"""Watchdog"""
+#!/usr/bin/env python3
+"""Transport XMLRPC Service"""
 
-############################################################################
+##########################################################################
 #
-#   watchdog
+#   Transport XLMRPC Service
 #
-#   This script monitors the process group clients and reports any that
-#   were started but have seemed to stop running (they are registered but
-#   don't show up as an active process). In this case, the client is
-#   restarted. Messages are also sent to the watchdog list in this case.
+#   This is the base class for the different XML-RPC based services
+#   used in the transport network. It interfaces with the directory
+#   service to bootstrap the local server.
 #
-#   History:
+#   2005-11-09  Todd Valentic
+#               Initial implementation.
 #
-#   2000-04-24  TAV
-#               Initial implementation
+#   2006-01-22  Todd Valentic
+#               Added intospection registration
 #
-#   2002-01-20  Todd Valentic
-#               Improved wording of notification message.
+#   2006-02-25  Todd Valentic
+#               Added idle function and timeout.
 #
-#   2002-01-24  Todd Valentic
-#               Added timestamp to message body.
+#   2006-06-14  Todd Valentic
+#               Use label in directory server for ident.
 #
-#   2002-01-25  Todd Valentic
-#               Added check for self.running
+#   2006-07-17  Todd Valentic
+#               Added try..except around request handle to catch
+#                   connection breaks.
 #
-#   2002-05-19  Todd Valentic
-#               Fixed call to restart client (now include arg string).
+#   2016-07-10  Todd Valentic
+#               Python 2.6+ has a more sophisticated serve_forver()
+#                   loop that ensures system calls complete and thus
+#                   results in the old implementation blocking forever.
+#                   Now we handle both the older and newer versions.
 #
-#   2002-08-28  Todd Valentic
-#               sri.transport -> Transport
-#               python -> python2
+#   2016-10-31  Todd Valentic
+#               Modify previous change to work on Python 2.4 as well.
 #
-#   2003-04-15  Todd Valentic
-#               Changed config parameter pollrate -> rate
-#               Rate now specified in days/hours/mins/secs
+#   2016-11-08  Todd Valentic
+#               Remove call to undefined shutdown() method.
+#               Fix type in assignment for server_forever for < python 2.6
 #
-#   2004-02-08  Todd Valentic
-#               Use DeltaTime for rate
-#               Use string methods
+#   2017-01-10	Todd Valentic
+# 		Restore call to shutdown() method - needed to exit,
+# 		    otherwise we deadlock. The function is inherited
+# 		    from SimpleXMLRPCServer
 #
-#   2004-08-08  Todd Valentic
-#               Updated to new XML-RPC server interface
+#   2017-06-08  Todd Valentic
+#               Rename ident() function to prevent conflict with
+#                   threading.Thread.ident when this class is mixed in with
+#                   Thread. This problem showed up in Python 2.6+
 #
-#   2004-08-25  Todd Valentic
-#               Converted to directly reading /proc instead of using ps
+#   2019-08-06  Todd Valentic
+#               Add timeout to RequestHandler
+#               Set allow_none
 #
-#   2004-12-30  Todd Valentic
-#               Convert from mx.DateTime to datetime
+#   2020-10-09  Todd Valentic
+#               Python3: xmlrpc.server
 #
-#   2022-10-06  Todd Valentic
-#               Updated for transport3/python3
-#   
-#   2023-07-26  Todd Valentic
-#               Use config getters
+#   2022-10-07  Todd Valentic
+#               Reorder imports
 #
-############################################################################
-
-import pathlib
-import sys
-
-from datatransport import ProcessClient
-from datatransport import NewsPoster
-
-
-class Watchdog(ProcessClient):
-    """Watchdog Process Client"""
+#   2023-07-04  Todd Valentic
+#               Convert from mixin class
+#
+##########################################################################
 
-    def __init__(self, argv):
-        ProcessClient.__init__(self, argv)
+import threading
+import xmlrpc.client
 
-    def init(self):
-        super().init()
+from xmlrpc.server import SimpleXMLRPCServer
+from xmlrpc.server import SimpleXMLRPCRequestHandler
 
-        self.news_poster = NewsPoster(self)
-        self.rate = self.config.get_rate("rate", "5m")
+from . import Directory
 
-    def get_client_pids(self):
-        """Query server for expected client PIDs"""
+SimpleXMLRPCRequestHandler.timeout = 5
 
-        pids = {}
 
-        for group in self.server.listgroups():
-            for client, info in self.server.listclients(group).items():
-                pid = info[1]
-                if pid:
-                    pids[pid] = (group, client)
+class XMLRPCServer(SimpleXMLRPCServer):
+    """Data Transport XMLRPC Server"""
 
-        return pids
+    # pylint: disable=too-many-arguments
 
-    def get_running_pids(self):
-        """Get list of running PIDs on system"""
+    def __init__(
+        self, parent, queue_size=20, port=None, label=None, callback=None, timeout=1
+    ):
+        self.parent = parent
+        self.callback = callback
+        self.timeout = timeout
 
-        proc = pathlib.Path("/proc")
-        return [int(x.name) for x in proc.iterdir() if x.name.isdigit()]
+        if port is None:
+            # This is a normal service client
 
-    def post_message(self, pid, group_name, client_name):
-        """Post a trouble message"""
+            self.directory = Directory(parent)
 
-        body = []
-        body.append("")
-        body.append(
-            "  The watchdog has detected the following client has stopped running:"
-        )
-        body.append("")
-        body.append(f"      Client name: {client_name}")
-        body.append(f"       Group name: {group_name}")
-        body.append(f"       Process ID: {pid}")
-        body.append(f"       Time stamp: {self.now()}")
-        body.append("")
-        body.append("  The client has been restarted.")
-        body.append("")
+            servicename = parent.config.get("service.name")
 
-        header = f"Watchdog restart {client_name}"
+            if not servicename:
+                parent.abort("No service.name found")
 
-        try:
-            self.news_poster.set_subject(header)
-            self.news_poster.post_text("\n".join(body))
-        except:  # pylint: disable=bare-except
-            self.log.error("Error posting notification message to the news server.")
+            port = self.directory.get(servicename, "port")
 
-    def restart(self, pid, group, client):
-        """Restart the client process"""
+            try:
+                label = self.directory.get(servicename, "label")
+            except xmlrpc.client.Fault:
+                label = None
 
-        self.log.info("Process '%s %s' (PID %s) is missing", group, client, pid)
-        self.log.info("  Attempting to restart")
+        self.allow_reuse_address = True
+        self.request_queue_size = queue_size
 
-        self.post_message(pid, group, client)
-
-        try:
-            self.server.startclient(group, client)
-        except:  # pylint: disable=bare-except
-            self.log.info("  Error detected in client restart!")
+        SimpleXMLRPCServer.__init__(
+            self, ("", port), allow_none=True, logRequests=False
+        )
 
-    def checkup(self):
-        """Check to see if any clients have unexpectedly stopped"""
+        self.register_introspection_functions()
+        self.register_function(self.my_ident, "ident")
+        self.register_function(self.status)
+
+        parent.log.info(f"Listening on port {port}")
+
+        if label:
+            self.servicelabel = label
+        else:
+            self.servicelabel = "No description available"
+
+    def my_ident(self):
+        """Service desciption"""
+        return self.servicelabel
+
+    def status(self):
+        """Indicate active"""
+        return 1
 
-        self.log.info("Checking processes")
+    def server_thread(self):
+        """Run server in separate thread"""
 
         try:
-            self.server.status()
+            self.serve_forever()
         except:  # pylint: disable=bare-except
-            self.log.error("Cannot connect to the transport server!")
-            return
+            pass
+        finally:
+            self.server_close()
 
-        client_pids = self.get_client_pids()
-        running_pids = self.get_running_pids()
-
-        for pid, entry in client_pids.items():
-            group, client = entry
+    def main(self):
+        """Run server"""
 
-            if not pid in running_pids:
-                self.restart(pid, group, client)
+        self.parent.log.info("Starting operations")
 
-    def main(self):
-        """Main application"""
+        thread = threading.Thread(None, self.server_thread)
+        thread.start()
 
-        while self.wait(self.rate):
-            self.checkup()
+        while self.parent.wait(self.timeout):
+            if self.callback:
+                self.callback()
 
+        self.shutdown()
+        thread.join()
 
-if __name__ == "__main__":
-    Watchdog(sys.argv).run()
+        self.parent.log.info("Finished")
```

### Comparing `datatransport-3.0.7/src/datatransport/transportconfig.py` & `datatransport-3.0.8/src/datatransport/transportconfig.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/transportlogger.py` & `datatransport-3.0.8/src/datatransport/transportlogger.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/transportmanager.py` & `datatransport-3.0.8/src/datatransport/transportmanager.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/transportserver.py` & `datatransport-3.0.8/src/datatransport/transportserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/datefunc.py` & `datatransport-3.0.8/src/datatransport/utilities/datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/makepath.py` & `datatransport-3.0.8/src/datatransport/utilities/makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/patterntemplate.py` & `datatransport-3.0.8/src/datatransport/utilities/patterntemplate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/removefile.py` & `datatransport-3.0.8/src/datatransport/utilities/removefile.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/sizedesc.py` & `datatransport-3.0.8/src/datatransport/utilities/sizedesc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport/utilities/xmlrpcdeferred.py` & `datatransport-3.0.8/src/datatransport/utilities/xmlrpcdeferred.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/src/datatransport.egg-info/PKG-INFO` & `datatransport-3.0.8/src/datatransport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.7
+Version: 3.0.8
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.7/src/datatransport.egg-info/SOURCES.txt` & `datatransport-3.0.8/src/datatransport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,27 @@
 contrib/examples.v2/wait/wait.conf
 contrib/examples.v2/watchdog/crasher.py
 contrib/examples.v2/watchdog/watchdog.conf
 contrib/examples/archivegroups/archivegroups.conf
 contrib/examples/archivegroups/postdata.py
 contrib/examples/component/component.conf
 contrib/examples/component/demo.py
+contrib/examples/diskmonitor/demo.py
+contrib/examples/diskmonitor/diskmonitor.conf
 contrib/examples/environ/environ.conf
 contrib/examples/environ/environ.py
+contrib/examples/filepost/createdata.py
+contrib/examples/filepost/filepost.conf
+contrib/examples/filepost/watcher.py
 contrib/examples/filewatch/createdata.py
 contrib/examples/filewatch/filewatch.conf
 contrib/examples/getbytes/demo.py
 contrib/examples/getbytes/getbytes.conf
+contrib/examples/groupcontrol/groupcontrol.conf
+contrib/examples/groupcontrol/request.py
 contrib/examples/hello/hello.conf
 contrib/examples/hello/helloworld.py
 contrib/examples/init/demo.py
 contrib/examples/init/init.conf
 contrib/examples/messagebox/messagebox.conf
 contrib/examples/messagebox/poll_file.py
 contrib/examples/messagebox/poll_text.py
@@ -121,34 +128,33 @@
 src/datatransport/commands/console.py
 src/datatransport/commands/listnewsgroups.py
 src/datatransport/commands/transport_create_app.py
 src/datatransport/commands/transportctl.py
 src/datatransport/commands/transportd.py
 src/datatransport/commands/transportps.py
 src/datatransport/commands/viewlog.py
-src/datatransport/components/DiskMonitor.py
 src/datatransport/components/EventMonitor.py
-src/datatransport/components/FilePost.py
-src/datatransport/components/FileStore.py
-src/datatransport/components/GroupControl.py
 src/datatransport/components/InstrumentStatus.py
 src/datatransport/components/NewsGateway.py
 src/datatransport/components/NewsgroupMonitor.py
 src/datatransport/components/PageKit.py
 src/datatransport/components/PlotTool.py
 src/datatransport/components/PostDataFiles.py
 src/datatransport/components/RealTimeFeed.py
 src/datatransport/components/ResourceMonitor.py
 src/datatransport/components/Scheduler.py
 src/datatransport/components/SyncPoller.py
 src/datatransport/components/WatchURL.py
 src/datatransport/components/__init__.py
 src/datatransport/components/archivegroups.py
 src/datatransport/components/directoryservice.py
+src/datatransport/components/diskmonitor.py
+src/datatransport/components/filepost.py
 src/datatransport/components/filewatch.py
+src/datatransport/components/groupcontrol.py
 src/datatransport/templates/etc/transportd.conf
 src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
 src/datatransport/templates/groups/ServerMonitor/watchdog.py
 src/datatransport/utilities/__init__.py
 src/datatransport/utilities/datefunc.py
 src/datatransport/utilities/makepath.py
 src/datatransport/utilities/patterntemplate.py
```

### Comparing `datatransport-3.0.7/src/datatransport.egg-info/entry_points.txt` & `datatransport-3.0.8/src/datatransport.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [console_scripts]
 archivegroups = datatransport.components.archivegroups:main
 cancelnewsgroup = datatransport.commands.cancelnewsgroup:main
 console = datatransport.commands.console:main
 directoryservice = datatransport.components.directoryservice:main
-diskmonitor = datatransport.components.DiskMonitor:main
-filepost = datatransport.components.FilePost:main
-filestore = datatransport.components.FileStore:main
+diskmonitor = datatransport.components.diskmonitor:main
+filepost = datatransport.components.filepost:main
 filewatch = datatransport.components.filewatch:main
-groupcontrol = datatransport.components.GroupControl:main
+groupcontrol = datatransport.components.groupcontrol:main
 instrumentstatus = datatransport.components.InstrumentStatus:main
 listnewsgroups = datatransport.commands.listnewsgroups:main
 newsgateway = datatransport.components.NewsGateway:main
 newsgroupmonitor = datatransport.components.NewsgroupMonitor:main
 plottool = datatransport.components.PlotTool:main
 postdatafiles = datatransport.components.PostDataFiles:main
 realtimefeed = datatransport.components.RealTimeFeed:main
```

### Comparing `datatransport-3.0.7/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc` & `datatransport-3.0.8/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/tests/test_utilities_datefunc.py` & `datatransport-3.0.8/tests/test_utilities_datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/tests/test_utilities_makepath.py` & `datatransport-3.0.8/tests/test_utilities_makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/tests/test_utilities_pattern.py` & `datatransport-3.0.8/tests/test_utilities_pattern.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/tests/test_utilities_removefiles.py` & `datatransport-3.0.8/tests/test_utilities_removefiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.7/tests/test_utilities_sizedesc.py` & `datatransport-3.0.8/tests/test_utilities_sizedesc.py`

 * *Files identical despite different names*

