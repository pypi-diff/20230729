# Comparing `tmp/mov_cli-1.4.8.tar.gz` & `tmp/mov_cli-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.8.tar", max compression
+gzip compressed data, was "mov_cli-1.4.9.tar", max compression
```

## Comparing `mov_cli-1.4.8.tar` & `mov_cli-1.4.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2023-07-29 02:30:28.709043 mov_cli-1.4.8/LICENSE
--rw-r--r--   0        0        0     6568 2023-07-29 02:30:28.709043 mov_cli-1.4.8/README.md
--rw-r--r--   0        0        0      657 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/__init__.py
--rw-r--r--   0        0        0      810 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      906 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0      341 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/tukipasti.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     3128 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     2772 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0      356 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ar.json
--rw-r--r--   0        0        0      356 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/de.json
--rw-r--r--   0        0        0      309 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/en.json
--rw-r--r--   0        0        0      348 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/fr.json
--rw-r--r--   0        0        0      338 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ko.json
--rw-r--r--   0        0        0      194 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/langs
--rw-r--r--   0        0        0      308 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/pl.json
--rw-r--r--   0        0        0      289 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/pt.json
--rw-r--r--   0        0        0      418 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ru.json
--rw-r--r--   0        0        0      660 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ta.json
--rw-r--r--   0        0        0     1258 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1570 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/player.py
--rw-r--r--   0        0        0     1505 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/props.py
--rw-r--r--   0        0        0     7437 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0     5071 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/select.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/anime/__init__.py
--rw-r--r--   0        0        0     3274 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/anime/gogoanime.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/viewasian.py
--rw-r--r--   0        0        0     3382 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/watchasian.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/cartoons/__init__.py
--rw-r--r--   0        0        0     3544 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/cartoons/kisscartoon.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/__init__.py
--rw-r--r--   0        0        0     7680 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/actvid.py
--rw-r--r--   0        0        0     3843 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/dopebox.py
--rw-r--r--   0        0        0     4242 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/remotestream.py
--rw-r--r--   0        0        0     3847 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/sflix.py
--rw-r--r--   0        0        0     1626 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/solar.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/__init__.py
--rw-r--r--   0        0        0     1943 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/einthusan.py
--rw-r--r--   0        0        0     2165 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/tamilyogi.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/international/__init__.py
--rw-r--r--   0        0        0     3950 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/international/wlext.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/livetv/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/livetv/eja.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/sports/__init__.py
--rw-r--r--   0        0        0     4474 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/sports/scdn.py
--rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/__init__.py
--rw-r--r--   0        0        0     2318 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/turkish123.py
--rw-r--r--   0        0        0     2909 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/yoturkish.py
--rw-r--r--   0        0        0      736 2023-07-29 02:30:28.713043 mov_cli-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 mov_cli-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-29 02:35:18.604855 mov_cli-1.4.9/LICENSE
+-rw-r--r--   0        0        0     6568 2023-07-29 02:35:18.604855 mov_cli-1.4.9/README.md
+-rw-r--r--   0        0        0      657 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0      341 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/extractors/tukipasti.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2772 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0      356 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/utils/lang/ar.json
+-rw-r--r--   0        0        0      356 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/utils/lang/de.json
+-rw-r--r--   0        0        0      309 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/en.json
+-rw-r--r--   0        0        0      348 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/fr.json
+-rw-r--r--   0        0        0      338 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/ko.json
+-rw-r--r--   0        0        0      194 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/langs
+-rw-r--r--   0        0        0      308 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/pl.json
+-rw-r--r--   0        0        0      289 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/pt.json
+-rw-r--r--   0        0        0      418 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/ru.json
+-rw-r--r--   0        0        0      660 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/lang/ta.json
+-rw-r--r--   0        0        0     1258 2023-07-29 02:35:18.604855 mov_cli-1.4.9/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1570 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1505 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/props.py
+-rw-r--r--   0        0        0     7437 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0     5071 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/utils/select.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/anime/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/anime/gogoanime.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/asian/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/asian/viewasian.py
+-rw-r--r--   0        0        0     3382 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/asian/watchasian.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/cartoons/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/cartoons/kisscartoon.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/__init__.py
+-rw-r--r--   0        0        0     7686 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/actvid.py
+-rw-r--r--   0        0        0     3843 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/dopebox.py
+-rw-r--r--   0        0        0     4242 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/remotestream.py
+-rw-r--r--   0        0        0     3847 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/sflix.py
+-rw-r--r--   0        0        0     1626 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/english/solar.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/indian/__init__.py
+-rw-r--r--   0        0        0     1943 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/indian/einthusan.py
+-rw-r--r--   0        0        0     2165 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/indian/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/indian/tamilyogi.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/international/__init__.py
+-rw-r--r--   0        0        0     3950 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/international/wlext.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/livetv/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/livetv/eja.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/sports/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/sports/scdn.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/turkish/__init__.py
+-rw-r--r--   0        0        0     2318 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/turkish/turkish123.py
+-rw-r--r--   0        0        0     2909 2023-07-29 02:35:18.608855 mov_cli-1.4.9/mov_cli/websites/turkish/yoturkish.py
+-rw-r--r--   0        0        0      736 2023-07-29 02:35:18.608855 mov_cli-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 mov_cli-1.4.9/PKG-INFO
```

### Comparing `mov_cli-1.4.8/LICENSE` & `mov_cli-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/README.md` & `mov_cli-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/__init__.py` & `mov_cli-1.4.9/mov_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/__main__.py` & `mov_cli-1.4.9/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.9/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.9/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/players/player.py` & `mov_cli-1.4.9/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/httpclient.py` & `mov_cli-1.4.9/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/lang/ta.json` & `mov_cli-1.4.9/mov_cli/utils/lang/ta.json`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/lang.py` & `mov_cli-1.4.9/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/player.py` & `mov_cli-1.4.9/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/props.py` & `mov_cli-1.4.9/mov_cli/utils/props.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/scraper.py` & `mov_cli-1.4.9/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/utils/select.py` & `mov_cli-1.4.9/mov_cli/utils/select.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/anime/gogoanime.py` & `mov_cli-1.4.9/mov_cli/websites/anime/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/asian/viewasian.py` & `mov_cli-1.4.9/mov_cli/websites/asian/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/asian/watchasian.py` & `mov_cli-1.4.9/mov_cli/websites/asian/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/cartoons/kisscartoon.py` & `mov_cli-1.4.9/mov_cli/websites/cartoons/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/english/actvid.py` & `mov_cli-1.4.9/mov_cli/websites/english/actvid.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         if missing_padding != 0:
             s += '=' * (4 - missing_padding)
         return s
 
     def gh_key(self):
         response_key = self.client.get('https://github.com/enimax-anime/key/blob/e6/key.txt').json()
         key = response_key["payload"]["blob"]["rawLines"][0]
-        key = eval(key)
+        key = json.loads(key)
         return key
 
     def md5(self, data):
         return hashlib.md5(data).digest()
 
     def get_key(self, salt, key):
         x = self.md5(key + salt)
```

### Comparing `mov_cli-1.4.8/mov_cli/websites/english/dopebox.py` & `mov_cli-1.4.9/mov_cli/websites/english/dopebox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/english/remotestream.py` & `mov_cli-1.4.9/mov_cli/websites/english/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/english/sflix.py` & `mov_cli-1.4.9/mov_cli/websites/english/sflix.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/english/solar.py` & `mov_cli-1.4.9/mov_cli/websites/english/solar.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/indian/einthusan.py` & `mov_cli-1.4.9/mov_cli/websites/indian/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/indian/streamblasters.py` & `mov_cli-1.4.9/mov_cli/websites/indian/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/indian/tamilyogi.py` & `mov_cli-1.4.9/mov_cli/websites/indian/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/international/wlext.py` & `mov_cli-1.4.9/mov_cli/websites/international/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/livetv/eja.py` & `mov_cli-1.4.9/mov_cli/websites/livetv/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/sports/scdn.py` & `mov_cli-1.4.9/mov_cli/websites/sports/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/turkish/turkish123.py` & `mov_cli-1.4.9/mov_cli/websites/turkish/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/mov_cli/websites/turkish/yoturkish.py` & `mov_cli-1.4.9/mov_cli/websites/turkish/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.8/pyproject.toml` & `mov_cli-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.8"
+version = "1.4.9"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@r3tr0ananas.lol>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.8/PKG-INFO` & `mov_cli-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.8
+Version: 1.4.9
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@r3tr0ananas.lol
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.8 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.9 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@r3tr0ananas.lol Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
```

