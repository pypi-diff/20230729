# Comparing `tmp/cgl-py-0.0.8.tar.gz` & `tmp/cgl-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgl-py-0.0.8.tar", last modified: Wed Apr 19 15:39:58 2023, max compression
+gzip compressed data, was "cgl-py-0.0.9.tar", last modified: Wed Apr 19 16:29:19 2023, max compression
```

## Comparing `cgl-py-0.0.8.tar` & `cgl-py-0.0.9.tar`

### file list

```diff
@@ -1,385 +1,386 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.101219 cgl-py-0.0.8/
--rw-rw-rw-   0        0        0     1099 2023-04-18 09:35:58.000000 cgl-py-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      166 2023-04-18 09:44:34.000000 cgl-py-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1126 2023-04-19 15:39:58.100246 cgl-py-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11649 2023-04-18 09:35:50.000000 cgl-py-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.712730 cgl-py-0.0.8/cgl_py.egg-info/
--rw-rw-rw-   0        0        0     1126 2023-04-19 15:39:57.000000 cgl-py-0.0.8/cgl_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13032 2023-04-19 15:39:57.000000 cgl-py-0.0.8/cgl_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:39:57.000000 cgl-py-0.0.8/cgl_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-19 15:39:57.000000 cgl-py-0.0.8/cgl_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-19 15:39:57.000000 cgl-py-0.0.8/cgl_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0  3210527 2023-04-19 14:19:39.000000 cgl-py-0.0.8/cgl_wrapper.c
--rw-rw-rw-   0        0        0   107119 2023-04-19 14:19:35.000000 cgl-py-0.0.8/cgl_wrapper.pyx
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.713701 cgl-py-0.0.8/include/
--rw-rw-rw-   0        0        0   594421 2023-04-19 13:51:13.000000 cgl-py-0.0.8/include/cgl.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.685440 cgl-py-0.0.8/include/freetype/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.683494 cgl-py-0.0.8/include/freetype/builds/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.683494 cgl-py-0.0.8/include/freetype/builds/amiga/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.683494 cgl-py-0.0.8/include/freetype/builds/amiga/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.719541 cgl-py-0.0.8/include/freetype/builds/amiga/include/config/
--rw-rw-rw-   0        0        0     2252 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/builds/amiga/include/config/ftconfig.h
--rw-rw-rw-   0        0        0     4557 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/builds/amiga/include/config/ftmodule.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.720513 cgl-py-0.0.8/include/freetype/builds/atari/
--rw-rw-rw-   0        0        0      432 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/builds/atari/ATARI.H
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.721488 cgl-py-0.0.8/include/freetype/builds/vms/
--rw-rw-rw-   0        0        0     1760 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/builds/vms/ftconfig.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.722461 cgl-py-0.0.8/include/freetype/devel/
--rw-rw-rw-   0        0        0     1218 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/devel/ft2build.h
--rw-rw-rw-   0        0        0    41953 2023-02-08 20:09:03.000000 cgl-py-0.0.8/include/freetype/devel/ftoption.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.724407 cgl-py-0.0.8/include/freetype/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.727328 cgl-py-0.0.8/include/freetype/include/dlg/
--rw-rw-rw-   0        0        0    11104 2023-02-09 06:33:10.000000 cgl-py-0.0.8/include/freetype/include/dlg/dlg.h
--rw-rw-rw-   0        0        0     7401 2023-02-09 06:33:10.000000 cgl-py-0.0.8/include/freetype/include/dlg/output.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.782810 cgl-py-0.0.8/include/freetype/include/freetype/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.789623 cgl-py-0.0.8/include/freetype/include/freetype/config/
--rw-rw-rw-   0        0        0     1665 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/ftconfig.h
--rw-rw-rw-   0        0        0    24755 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/ftheader.h
--rw-rw-rw-   0        0        0     1476 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/ftmodule.h
--rw-rw-rw-   0        0        0    42004 2023-02-08 20:09:03.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/ftoption.h
--rw-rw-rw-   0        0        0     4753 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/ftstdlib.h
--rw-rw-rw-   0        0        0     7322 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/integer-types.h
--rw-rw-rw-   0        0        0     1646 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/mac-support.h
--rw-rw-rw-   0        0        0     4345 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/config/public-macros.h
--rw-rw-rw-   0        0        0   178033 2023-02-09 06:03:46.000000 cgl-py-0.0.8/include/freetype/include/freetype/freetype.h
--rw-rw-rw-   0        0        0     5658 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftadvanc.h
--rw-rw-rw-   0        0        0     2739 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftbbox.h
--rw-rw-rw-   0        0        0     5534 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftbdf.h
--rw-rw-rw-   0        0        0     9380 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftbitmap.h
--rw-rw-rw-   0        0        0     2888 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftbzip2.h
--rw-rw-rw-   0        0        0    34947 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftcache.h
--rw-rw-rw-   0        0        0     2735 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftchapters.h
--rw-rw-rw-   0        0        0     4189 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftcid.h
--rw-rw-rw-   0        0        0    51866 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftcolor.h
--rw-rw-rw-   0        0        0    49041 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftdriver.h
--rw-rw-rw-   0        0        0    12842 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/fterrdef.h
--rw-rw-rw-   0        0        0     9597 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/fterrors.h
--rw-rw-rw-   0        0        0     2306 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftfntfmt.h
--rw-rw-rw-   0        0        0     4281 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftgasp.h
--rw-rw-rw-   0        0        0    21662 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftglyph.h
--rw-rw-rw-   0        0        0    10979 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftgxval.h
--rw-rw-rw-   0        0        0     4362 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftgzip.h
--rw-rw-rw-   0        0        0    42856 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftimage.h
--rw-rw-rw-   0        0        0    11044 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftincrem.h
--rw-rw-rw-   0        0        0    12067 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftlcdfil.h
--rw-rw-rw-   0        0        0     7396 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftlist.h
--rw-rw-rw-   0        0        0     4313 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftlogging.h
--rw-rw-rw-   0        0        0     2868 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftlzw.h
--rw-rw-rw-   0        0        0     8060 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftmac.h
--rw-rw-rw-   0        0        0    23095 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftmm.h
--rw-rw-rw-   0        0        0    23351 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftmodapi.h
--rw-rw-rw-   0        0        0     6879 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftmoderr.h
--rw-rw-rw-   0        0        0     5552 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftotval.h
--rw-rw-rw-   0        0        0    17990 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftoutln.h
--rw-rw-rw-   0        0        0     6259 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftparams.h
--rw-rw-rw-   0        0        0     5087 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftpfr.h
--rw-rw-rw-   0        0        0     6869 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftrender.h
--rw-rw-rw-   0        0        0     4447 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftsizes.h
--rw-rw-rw-   0        0        0     8002 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftsnames.h
--rw-rw-rw-   0        0        0    22546 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftstroke.h
--rw-rw-rw-   0        0        0     3932 2023-02-09 05:51:54.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftsynth.h
--rw-rw-rw-   0        0        0     9181 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftsystem.h
--rw-rw-rw-   0        0        0     7761 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/fttrigon.h
--rw-rw-rw-   0        0        0    15352 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/fttypes.h
--rw-rw-rw-   0        0        0     8241 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ftwinfnt.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.814962 cgl-py-0.0.8/include/freetype/include/freetype/internal/
--rw-rw-rw-   0        0        0     7732 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/autohint.h
--rw-rw-rw-   0        0        0     2461 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/cffotypes.h
--rw-rw-rw-   0        0        0    12282 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/cfftypes.h
--rw-rw-rw-   0        0        0    11678 2023-02-08 20:24:39.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/compiler-macros.h
--rw-rw-rw-   0        0        0    16187 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftcalc.h
--rw-rw-rw-   0        0        0    13774 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftdebug.h
--rw-rw-rw-   0        0        0     9497 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftdrv.h
--rw-rw-rw-   0        0        0     4651 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftgloadr.h
--rw-rw-rw-   0        0        0     3377 2022-09-01 09:52:14.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/fthash.h
--rw-rw-rw-   0        0        0    16359 2023-02-08 20:09:03.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftmemory.h
--rw-rw-rw-   0        0        0     2549 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftmmtypes.h
--rw-rw-rw-   0        0        0    43719 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftobjs.h
--rw-rw-rw-   0        0        0     1177 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftpsprop.h
--rw-rw-rw-   0        0        0     7896 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftrfork.h
--rw-rw-rw-   0        0        0    24548 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftserv.h
--rw-rw-rw-   0        0        0    23800 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftstream.h
--rw-rw-rw-   0        0        0     6090 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/fttrace.h
--rw-rw-rw-   0        0        0     5922 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/ftvalid.h
--rw-rw-rw-   0        0        0    44675 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/psaux.h
--rw-rw-rw-   0        0        0    21551 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/pshints.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.829562 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/
--rw-rw-rw-   0        0        0     1797 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svbdf.h
--rw-rw-rw-   0        0        0     2922 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svcfftl.h
--rw-rw-rw-   0        0        0     2193 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svcid.h
--rw-rw-rw-   0        0        0     1403 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svfntfmt.h
--rw-rw-rw-   0        0        0     1937 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svgldict.h
--rw-rw-rw-   0        0        0     1802 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svgxval.h
--rw-rw-rw-   0        0        0     1131 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svkern.h
--rw-rw-rw-   0        0        0     3880 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svmetric.h
--rw-rw-rw-   0        0        0     8197 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svmm.h
--rw-rw-rw-   0        0        0     1308 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svotval.h
--rw-rw-rw-   0        0        0     1635 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpfr.h
--rw-rw-rw-   0        0        0     1636 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpostnm.h
--rw-rw-rw-   0        0        0     1743 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svprop.h
--rw-rw-rw-   0        0        0     4419 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpscmap.h
--rw-rw-rw-   0        0        0     2555 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpsinfo.h
--rw-rw-rw-   0        0        0     2167 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svsfnt.h
--rw-rw-rw-   0        0        0     2487 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svttcmap.h
--rw-rw-rw-   0        0        0     1060 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svtteng.h
--rw-rw-rw-   0        0        0     1307 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svttglyf.h
--rw-rw-rw-   0        0        0     1067 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svwinfnt.h
--rw-rw-rw-   0        0        0    33536 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/sfnt.h
--rw-rw-rw-   0        0        0     1087 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/svginterface.h
--rw-rw-rw-   0        0        0     8484 2023-02-05 06:51:42.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/t1types.h
--rw-rw-rw-   0        0        0    54710 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/tttypes.h
--rw-rw-rw-   0        0        0     8322 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/internal/wofftypes.h
--rw-rw-rw-   0        0        0    10793 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/otsvg.h
--rw-rw-rw-   0        0        0    23981 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/t1tables.h
--rw-rw-rw-   0        0        0    60004 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/ttnameid.h
--rw-rw-rw-   0        0        0    26082 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/tttables.h
--rw-rw-rw-   0        0        0     5269 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/freetype/tttags.h
--rw-rw-rw-   0        0        0     1032 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/include/ft2build.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.691312 cgl-py-0.0.8/include/freetype/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.847082 cgl-py-0.0.8/include/freetype/src/autofit/
--rw-rw-rw-   0        0        0    17366 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afblue.h
--rw-rw-rw-   0        0        0     4332 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afcjk.h
--rw-rw-rw-   0        0        0     3264 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afcover.h
--rw-rw-rw-   0        0        0      917 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afdummy.h
--rw-rw-rw-   0        0        0     1026 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/aferrors.h
--rw-rw-rw-   0        0        0     5292 2023-02-08 20:09:32.000000 cgl-py-0.0.8/include/freetype/src/autofit/afglobal.h
--rw-rw-rw-   0        0        0    16415 2023-02-08 20:09:03.000000 cgl-py-0.0.8/include/freetype/src/autofit/afhints.h
--rw-rw-rw-   0        0        0      881 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afindic.h
--rw-rw-rw-   0        0        0     6978 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/aflatin.h
--rw-rw-rw-   0        0        0     2360 2023-02-08 20:09:32.000000 cgl-py-0.0.8/include/freetype/src/autofit/afloader.h
--rw-rw-rw-   0        0        0     1236 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afmodule.h
--rw-rw-rw-   0        0        0     1130 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afranges.h
--rw-rw-rw-   0        0        0    11872 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afscript.h
--rw-rw-rw-   0        0        0     1726 2023-02-08 20:37:13.000000 cgl-py-0.0.8/include/freetype/src/autofit/afshaper.h
--rw-rw-rw-   0        0        0    15602 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afstyles.h
--rw-rw-rw-   0        0        0    19135 2023-02-08 20:09:03.000000 cgl-py-0.0.8/include/freetype/src/autofit/aftypes.h
--rw-rw-rw-   0        0        0      905 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afws-decl.h
--rw-rw-rw-   0        0        0      997 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/autofit/afws-iter.h
--rw-rw-rw-   0        0        0     1511 2023-02-08 20:47:06.000000 cgl-py-0.0.8/include/freetype/src/autofit/ft-hb.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.848055 cgl-py-0.0.8/include/freetype/src/base/
--rw-rw-rw-   0        0        0     2733 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/base/ftbase.h
--rw-rw-rw-   0        0        0     1455 2020-07-23 07:10:04.000000 cgl-py-0.0.8/include/freetype/src/base/md5.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.850975 cgl-py-0.0.8/include/freetype/src/bdf/
--rw-rw-rw-   0        0        0     8490 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/bdf/bdf.h
--rw-rw-rw-   0        0        0     1844 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/bdf/bdfdrivr.h
--rw-rw-rw-   0        0        0     1629 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/bdf/bdferror.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.859735 cgl-py-0.0.8/include/freetype/src/cache/
--rw-rw-rw-   0        0        0    15577 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftccache.h
--rw-rw-rw-   0        0        0     2313 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftccback.h
--rw-rw-rw-   0        0        0     1041 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcerror.h
--rw-rw-rw-   0        0        0    11886 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcglyph.h
--rw-rw-rw-   0        0        0     2781 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcimage.h
--rw-rw-rw-   0        0        0     5909 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcmanag.h
--rw-rw-rw-   0        0        0     8773 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcmru.h
--rw-rw-rw-   0        0        0     2513 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cache/ftcsbits.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.865575 cgl-py-0.0.8/include/freetype/src/cff/
--rw-rw-rw-   0        0        0     2248 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffcmap.h
--rw-rw-rw-   0        0        0      787 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffdrivr.h
--rw-rw-rw-   0        0        0     1001 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cfferrs.h
--rw-rw-rw-   0        0        0     1585 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffgload.h
--rw-rw-rw-   0        0        0     3423 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffload.h
--rw-rw-rw-   0        0        0     2024 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffobjs.h
--rw-rw-rw-   0        0        0     3671 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cffparse.h
--rw-rw-rw-   0        0        0     6922 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cff/cfftoken.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.872389 cgl-py-0.0.8/include/freetype/src/cid/
--rw-rw-rw-   0        0        0      999 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/ciderrs.h
--rw-rw-rw-   0        0        0     1226 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidgload.h
--rw-rw-rw-   0        0        0     1167 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidload.h
--rw-rw-rw-   0        0        0     3566 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidobjs.h
--rw-rw-rw-   0        0        0     3648 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidparse.h
--rw-rw-rw-   0        0        0      808 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidriver.h
--rw-rw-rw-   0        0        0     4502 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/cid/cidtoken.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.879203 cgl-py-0.0.8/include/freetype/src/gxvalid/
--rw-rw-rw-   0        0        0     2976 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvalid.h
--rw-rw-rw-   0        0        0    23564 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvcommn.h
--rw-rw-rw-   0        0        0     1384 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxverror.h
--rw-rw-rw-   0        0        0     6227 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvfeat.h
--rw-rw-rw-   0        0        0     1139 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmod.h
--rw-rw-rw-   0        0        0     3070 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmort.h
--rw-rw-rw-   0        0        0     2149 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmorx.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.890883 cgl-py-0.0.8/include/freetype/src/gzip/
--rw-rw-rw-   0        0        0   601195 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/gzip/crc32.h
--rw-rw-rw-   0        0        0    17172 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gzip/ftzconf.h
--rw-rw-rw-   0        0        0     7062 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/gzip/gzguts.h
--rw-rw-rw-   0        0        0      445 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gzip/inffast.h
--rw-rw-rw-   0        0        0     6426 2022-12-14 09:30:46.000000 cgl-py-0.0.8/include/freetype/src/gzip/inffixed.h
--rw-rw-rw-   0        0        0     6876 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/gzip/inflate.h
--rw-rw-rw-   0        0        0     3067 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gzip/inftrees.h
--rw-rw-rw-   0        0        0    99975 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gzip/zlib.h
--rw-rw-rw-   0        0        0     7679 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/gzip/zutil.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.891886 cgl-py-0.0.8/include/freetype/src/lzw/
--rw-rw-rw-   0        0        0     5273 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/lzw/ftzopen.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.895781 cgl-py-0.0.8/include/freetype/src/otvalid/
--rw-rw-rw-   0        0        0     2204 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/otvalid/otvalid.h
--rw-rw-rw-   0        0        0    19811 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/otvalid/otvcommn.h
--rw-rw-rw-   0        0        0     1059 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/otvalid/otverror.h
--rw-rw-rw-   0        0        0      822 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/otvalid/otvgpos.h
--rw-rw-rw-   0        0        0      816 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/otvalid/otvmod.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.899674 cgl-py-0.0.8/include/freetype/src/pcf/
--rw-rw-rw-   0        0        0     6624 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/pcf/pcf.h
--rw-rw-rw-   0        0        0     1402 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/pcf/pcfdrivr.h
--rw-rw-rw-   0        0        0     1000 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/pcf/pcferror.h
--rw-rw-rw-   0        0        0     1405 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/pcf/pcfread.h
--rw-rw-rw-   0        0        0     1704 2022-09-01 09:52:15.000000 cgl-py-0.0.8/include/freetype/src/pcf/pcfutil.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.906488 cgl-py-0.0.8/include/freetype/src/pfr/
--rw-rw-rw-   0        0        0      965 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrcmap.h
--rw-rw-rw-   0        0        0      809 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrdrivr.h
--rw-rw-rw-   0        0        0     1003 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrerror.h
--rw-rw-rw-   0        0        0     1108 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrgload.h
--rw-rw-rw-   0        0        0     3548 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrload.h
--rw-rw-rw-   0        0        0     2231 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrobjs.h
--rw-rw-rw-   0        0        0      915 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrsbit.h
--rw-rw-rw-   0        0        0     8421 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pfr/pfrtypes.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.924008 cgl-py-0.0.8/include/freetype/src/psaux/
--rw-rw-rw-   0        0        0     1913 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/afmparse.h
--rw-rw-rw-   0        0        0     1888 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/cffdecode.h
--rw-rw-rw-   0        0        0     3575 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psarrst.h
--rw-rw-rw-   0        0        0     1045 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/psauxerr.h
--rw-rw-rw-   0        0        0     1307 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/psauxmod.h
--rw-rw-rw-   0        0        0     6180 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psblues.h
--rw-rw-rw-   0        0        0     1770 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/psconv.h
--rw-rw-rw-   0        0        0     4144 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/pserror.h
--rw-rw-rw-   0        0        0     3837 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psfixed.h
--rw-rw-rw-   0        0        0     5536 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psfont.h
--rw-rw-rw-   0        0        0     5561 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psft.h
--rw-rw-rw-   0        0        0     4645 2023-01-17 18:03:58.000000 cgl-py-0.0.8/include/freetype/src/psaux/psglue.h
--rw-rw-rw-   0        0        0    10157 2023-01-17 18:03:59.000000 cgl-py-0.0.8/include/freetype/src/psaux/pshints.h
--rw-rw-rw-   0        0        0     3157 2023-01-17 18:03:59.000000 cgl-py-0.0.8/include/freetype/src/psaux/psintrp.h
--rw-rw-rw-   0        0        0    10595 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/psobjs.h
--rw-rw-rw-   0        0        0     2367 2023-01-17 18:03:59.000000 cgl-py-0.0.8/include/freetype/src/psaux/psread.h
--rw-rw-rw-   0        0        0     3817 2023-01-17 18:03:59.000000 cgl-py-0.0.8/include/freetype/src/psaux/psstack.h
--rw-rw-rw-   0        0        0     2751 2023-01-17 18:03:59.000000 cgl-py-0.0.8/include/freetype/src/psaux/pstypes.h
--rw-rw-rw-   0        0        0     3386 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/t1cmap.h
--rw-rw-rw-   0        0        0     2097 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psaux/t1decode.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.927901 cgl-py-0.0.8/include/freetype/src/pshinter/
--rw-rw-rw-   0        0        0     6849 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pshinter/pshalgo.h
--rw-rw-rw-   0        0        0     5056 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pshinter/pshglob.h
--rw-rw-rw-   0        0        0      779 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pshinter/pshmod.h
--rw-rw-rw-   0        0        0     1019 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pshinter/pshnterr.h
--rw-rw-rw-   0        0        0     4274 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/pshinter/pshrec.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.930821 cgl-py-0.0.8/include/freetype/src/psnames/
--rw-rw-rw-   0        0        0      785 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psnames/psmodule.h
--rw-rw-rw-   0        0        0     1041 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psnames/psnamerr.h
--rw-rw-rw-   0        0        0   272382 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/psnames/pstables.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.936661 cgl-py-0.0.8/include/freetype/src/raster/
--rw-rw-rw-   0        0        0     3108 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/raster/ftmisc.h
--rw-rw-rw-   0        0        0     1139 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/raster/ftraster.h
--rw-rw-rw-   0        0        0      792 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/raster/ftrend1.h
--rw-rw-rw-   0        0        0     1047 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/raster/rasterrs.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.940554 cgl-py-0.0.8/include/freetype/src/sdf/
--rw-rw-rw-   0        0        0     3011 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sdf/ftsdf.h
--rw-rw-rw-   0        0        0     4148 2023-02-08 04:27:48.000000 cgl-py-0.0.8/include/freetype/src/sdf/ftsdfcommon.h
--rw-rw-rw-   0        0        0      885 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sdf/ftsdferrs.h
--rw-rw-rw-   0        0        0     3504 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sdf/ftsdfrend.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.955154 cgl-py-0.0.8/include/freetype/src/sfnt/
--rw-rw-rw-   0        0        0     1234 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/pngshim.h
--rw-rw-rw-   0        0        0      775 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/sfdriver.h
--rw-rw-rw-   0        0        0     1007 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/sferrors.h
--rw-rw-rw-   0        0        0     1475 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/sfobjs.h
--rw-rw-rw-   0        0        0      908 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/sfwoff.h
--rw-rw-rw-   0        0        0     2202 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/sfwoff2.h
--rw-rw-rw-   0        0        0     1078 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttbdf.h
--rw-rw-rw-   0        0        0     3853 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttcmap.h
--rw-rw-rw-   0        0        0     1283 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttcmapc.h
--rw-rw-rw-   0        0        0     2609 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttcolr.h
--rw-rw-rw-   0        0        0     1084 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttcpal.h
--rw-rw-rw-   0        0        0     1250 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttkern.h
--rw-rw-rw-   0        0        0     2618 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttload.h
--rw-rw-rw-   0        0        0     1343 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttmtx.h
--rw-rw-rw-   0        0        0     1048 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttpost.h
--rw-rw-rw-   0        0        0     1734 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttsbit.h
--rw-rw-rw-   0        0        0     1057 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/ttsvg.h
--rw-rw-rw-   0        0        0      908 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/sfnt/woff2tags.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.957101 cgl-py-0.0.8/include/freetype/src/smooth/
--rw-rw-rw-   0        0        0     1317 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/smooth/ftgrays.h
--rw-rw-rw-   0        0        0     1039 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/smooth/ftsmerrs.h
--rw-rw-rw-   0        0        0      788 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/smooth/ftsmooth.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.959048 cgl-py-0.0.8/include/freetype/src/svg/
--rw-rw-rw-   0        0        0      845 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/svg/ftsvg.h
--rw-rw-rw-   0        0        0     1237 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/svg/svgtypes.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.966834 cgl-py-0.0.8/include/freetype/src/truetype/
--rw-rw-rw-   0        0        0      783 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttdriver.h
--rw-rw-rw-   0        0        0     1023 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/tterrors.h
--rw-rw-rw-   0        0        0     1419 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttgload.h
--rw-rw-rw-   0        0        0    13878 2023-02-08 16:14:41.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttgxvar.h
--rw-rw-rw-   0        0        0    22350 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttinterp.h
--rw-rw-rw-   0        0        0    12476 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttobjs.h
--rw-rw-rw-   0        0        0     1732 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttpload.h
--rw-rw-rw-   0        0        0     3958 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/truetype/ttsubpix.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.973648 cgl-py-0.0.8/include/freetype/src/type1/
--rw-rw-rw-   0        0        0     1338 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1afm.h
--rw-rw-rw-   0        0        0      804 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1driver.h
--rw-rw-rw-   0        0        0     1010 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1errors.h
--rw-rw-rw-   0        0        0     1245 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1gload.h
--rw-rw-rw-   0        0        0     3411 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1load.h
--rw-rw-rw-   0        0        0     3612 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1objs.h
--rw-rw-rw-   0        0        0     3872 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1parse.h
--rw-rw-rw-   0        0        0     5226 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type1/t1tokens.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.977543 cgl-py-0.0.8/include/freetype/src/type42/
--rw-rw-rw-   0        0        0      775 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type42/t42drivr.h
--rw-rw-rw-   0        0        0     1014 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type42/t42error.h
--rw-rw-rw-   0        0        0     2575 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type42/t42objs.h
--rw-rw-rw-   0        0        0     2120 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type42/t42parse.h
--rw-rw-rw-   0        0        0     1237 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/type42/t42types.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.979490 cgl-py-0.0.8/include/freetype/src/winfonts/
--rw-rw-rw-   0        0        0     1030 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/winfonts/fnterrs.h
--rw-rw-rw-   0        0        0     3268 2023-02-04 14:00:05.000000 cgl-py-0.0.8/include/freetype/src/winfonts/winfnt.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.691312 cgl-py-0.0.8/include/glad/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.691312 cgl-py-0.0.8/include/glad/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.979490 cgl-py-0.0.8/include/glad/include/KHR/
--rw-rw-rw-   0        0        0    11131 2022-11-02 08:36:46.000000 cgl-py-0.0.8/include/glad/include/KHR/khrplatform.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.981437 cgl-py-0.0.8/include/glad/include/glad/
--rw-rw-rw-   0        0        0  1115714 2022-11-02 08:36:46.000000 cgl-py-0.0.8/include/glad/include/glad/glad.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.692287 cgl-py-0.0.8/include/glfw/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.995094 cgl-py-0.0.8/include/glfw/deps/
--rw-rw-rw-   0        0        0     2193 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/getopt.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.999960 cgl-py-0.0.8/include/glfw/deps/glad/
--rw-rw-rw-   0        0        0   332433 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/glad/gl.h
--rw-rw-rw-   0        0        0    82918 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/glad/gles2.h
--rw-rw-rw-   0        0        0   342527 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/glad/vulkan.h
--rw-rw-rw-   0        0        0    14729 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/linmath.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.003854 cgl-py-0.0.8/include/glfw/deps/mingw/
--rw-rw-rw-   0        0        0     3228 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/mingw/_mingw_dxhelper.h
--rw-rw-rw-   0        0        0   115027 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/mingw/dinput.h
--rw-rw-rw-   0        0        0     8189 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/mingw/xinput.h
--rw-rw-rw-   0        0        0  1016476 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/nuklear.h
--rw-rw-rw-   0        0        0    14462 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/nuklear_glfw_gl2.h
--rw-rw-rw-   0        0        0    72945 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/stb_image_write.h
--rw-rw-rw-   0        0        0    16103 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/tinycthread.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.004827 cgl-py-0.0.8/include/glfw/deps/vs2008/
--rw-rw-rw-   0        0        0     7975 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/deps/vs2008/stdint.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:57.692287 cgl-py-0.0.8/include/glfw/include/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.007751 cgl-py-0.0.8/include/glfw/include/GLFW/
--rw-rw-rw-   0        0        0   242360 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/include/GLFW/glfw3.h
--rw-rw-rw-   0        0        0    20689 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/include/GLFW/glfw3native.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.025267 cgl-py-0.0.8/include/glfw/src/
--rw-rw-rw-   0        0        0     1935 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/cocoa_joystick.h
--rw-rw-rw-   0        0        0    13208 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/cocoa_platform.h
--rw-rw-rw-   0        0        0     1413 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/cocoa_time.h
--rw-rw-rw-   0        0        0    37247 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/internal.h
--rw-rw-rw-   0        0        0     2379 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/linux_joystick.h
--rw-rw-rw-   0        0        0   258038 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/mappings.h
--rw-rw-rw-   0        0        0     1456 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/null_joystick.h
--rw-rw-rw-   0        0        0     7154 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/null_platform.h
--rw-rw-rw-   0        0        0     5183 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/platform.h
--rw-rw-rw-   0        0        0     1474 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/posix_poll.h
--rw-rw-rw-   0        0        0     1723 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/posix_thread.h
--rw-rw-rw-   0        0        0     1530 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/posix_time.h
--rw-rw-rw-   0        0        0     1958 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/win32_joystick.h
--rw-rw-rw-   0        0        0    25565 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/win32_platform.h
--rw-rw-rw-   0        0        0     1760 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/win32_thread.h
--rw-rw-rw-   0        0        0     1497 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/win32_time.h
--rw-rw-rw-   0        0        0    26218 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/wl_platform.h
--rw-rw-rw-   0        0        0    45741 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/x11_platform.h
--rw-rw-rw-   0        0        0     1318 2022-08-18 08:28:59.000000 cgl-py-0.0.8/include/glfw/src/xkb_unicode.h
-drwxrwxrwx   0        0        0        0 2023-04-19 15:39:58.095379 cgl-py-0.0.8/lib/
--rw-rw-rw-   0        0        0   657284 2023-04-19 11:36:50.000000 cgl-py-0.0.8/lib/cgl.lib
--rw-rw-rw-   0        0        0  1862890 2023-04-18 07:47:30.000000 cgl-py-0.0.8/lib/freetype.lib
--rw-rw-rw-   0        0        0  1764004 2023-04-18 07:47:32.000000 cgl-py-0.0.8/lib/glad.lib
--rw-rw-rw-   0        0        0   699066 2023-04-18 07:47:35.000000 cgl-py-0.0.8/lib/glfw3.lib
--rw-rw-rw-   0        0        0  1097268 2023-04-19 11:39:31.000000 cgl-py-0.0.8/lib/libcgl.a
--rw-rw-rw-   0        0        0  6517496 2023-04-18 12:01:42.000000 cgl-py-0.0.8/lib/libfreetype.a
--rw-rw-rw-   0        0        0  2245782 2023-04-18 12:31:41.000000 cgl-py-0.0.8/lib/libglad.a
--rw-rw-rw-   0        0        0  2808432 2023-04-18 12:01:45.000000 cgl-py-0.0.8/lib/libglfw3.a
--rw-rw-rw-   0        0        0       42 2023-04-19 15:39:58.101219 cgl-py-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2725 2023-04-19 15:39:49.000000 cgl-py-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.720085 cgl-py-0.0.9/
+-rw-rw-rw-   0        0        0     1099 2023-04-18 09:35:58.000000 cgl-py-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      166 2023-04-18 09:44:34.000000 cgl-py-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1126 2023-04-19 16:29:19.720085 cgl-py-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11649 2023-04-18 09:35:50.000000 cgl-py-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.505883 cgl-py-0.0.9/cgl_py.egg-info/
+-rw-rw-rw-   0        0        0     1126 2023-04-19 16:29:19.000000 cgl-py-0.0.9/cgl_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13047 2023-04-19 16:29:19.000000 cgl-py-0.0.9/cgl_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:29:19.000000 cgl-py-0.0.9/cgl_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 16:29:19.000000 cgl-py-0.0.9/cgl_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 16:29:19.000000 cgl-py-0.0.9/cgl_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  3210527 2023-04-19 14:19:39.000000 cgl-py-0.0.9/cgl_wrapper.c
+-rw-rw-rw-   0        0        0   107119 2023-04-19 14:19:35.000000 cgl-py-0.0.9/cgl_wrapper.pyx
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.506859 cgl-py-0.0.9/include/
+-rw-rw-rw-   0        0        0   594421 2023-04-19 13:51:13.000000 cgl-py-0.0.9/include/cgl.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.477559 cgl-py-0.0.9/include/freetype/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.476586 cgl-py-0.0.9/include/freetype/builds/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.475606 cgl-py-0.0.9/include/freetype/builds/amiga/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.475606 cgl-py-0.0.9/include/freetype/builds/amiga/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.508806 cgl-py-0.0.9/include/freetype/builds/amiga/include/config/
+-rw-rw-rw-   0        0        0     2252 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/builds/amiga/include/config/ftconfig.h
+-rw-rw-rw-   0        0        0     4557 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/builds/amiga/include/config/ftmodule.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.508806 cgl-py-0.0.9/include/freetype/builds/atari/
+-rw-rw-rw-   0        0        0      432 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/builds/atari/ATARI.H
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.509780 cgl-py-0.0.9/include/freetype/builds/vms/
+-rw-rw-rw-   0        0        0     1760 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/builds/vms/ftconfig.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.510753 cgl-py-0.0.9/include/freetype/devel/
+-rw-rw-rw-   0        0        0     1218 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/devel/ft2build.h
+-rw-rw-rw-   0        0        0    41953 2023-02-08 20:09:03.000000 cgl-py-0.0.9/include/freetype/devel/ftoption.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.511726 cgl-py-0.0.9/include/freetype/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.512699 cgl-py-0.0.9/include/freetype/include/dlg/
+-rw-rw-rw-   0        0        0    11104 2023-02-09 06:33:10.000000 cgl-py-0.0.9/include/freetype/include/dlg/dlg.h
+-rw-rw-rw-   0        0        0     7401 2023-02-09 06:33:10.000000 cgl-py-0.0.9/include/freetype/include/dlg/output.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.540926 cgl-py-0.0.9/include/freetype/include/freetype/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.545793 cgl-py-0.0.9/include/freetype/include/freetype/config/
+-rw-rw-rw-   0        0        0     1665 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/ftconfig.h
+-rw-rw-rw-   0        0        0    24755 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/ftheader.h
+-rw-rw-rw-   0        0        0     1476 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/ftmodule.h
+-rw-rw-rw-   0        0        0    42004 2023-02-08 20:09:03.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/ftoption.h
+-rw-rw-rw-   0        0        0     4753 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/ftstdlib.h
+-rw-rw-rw-   0        0        0     7322 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/integer-types.h
+-rw-rw-rw-   0        0        0     1646 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/mac-support.h
+-rw-rw-rw-   0        0        0     4345 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/config/public-macros.h
+-rw-rw-rw-   0        0        0   178033 2023-02-09 06:03:46.000000 cgl-py-0.0.9/include/freetype/include/freetype/freetype.h
+-rw-rw-rw-   0        0        0     5658 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftadvanc.h
+-rw-rw-rw-   0        0        0     2739 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftbbox.h
+-rw-rw-rw-   0        0        0     5534 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftbdf.h
+-rw-rw-rw-   0        0        0     9380 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftbitmap.h
+-rw-rw-rw-   0        0        0     2888 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftbzip2.h
+-rw-rw-rw-   0        0        0    34947 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftcache.h
+-rw-rw-rw-   0        0        0     2735 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftchapters.h
+-rw-rw-rw-   0        0        0     4189 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftcid.h
+-rw-rw-rw-   0        0        0    51866 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftcolor.h
+-rw-rw-rw-   0        0        0    49041 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftdriver.h
+-rw-rw-rw-   0        0        0    12842 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/fterrdef.h
+-rw-rw-rw-   0        0        0     9597 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/fterrors.h
+-rw-rw-rw-   0        0        0     2306 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftfntfmt.h
+-rw-rw-rw-   0        0        0     4281 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftgasp.h
+-rw-rw-rw-   0        0        0    21662 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftglyph.h
+-rw-rw-rw-   0        0        0    10979 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftgxval.h
+-rw-rw-rw-   0        0        0     4362 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftgzip.h
+-rw-rw-rw-   0        0        0    42856 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftimage.h
+-rw-rw-rw-   0        0        0    11044 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftincrem.h
+-rw-rw-rw-   0        0        0    12067 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftlcdfil.h
+-rw-rw-rw-   0        0        0     7396 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftlist.h
+-rw-rw-rw-   0        0        0     4313 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftlogging.h
+-rw-rw-rw-   0        0        0     2868 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftlzw.h
+-rw-rw-rw-   0        0        0     8060 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftmac.h
+-rw-rw-rw-   0        0        0    23095 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftmm.h
+-rw-rw-rw-   0        0        0    23351 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftmodapi.h
+-rw-rw-rw-   0        0        0     6879 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftmoderr.h
+-rw-rw-rw-   0        0        0     5552 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftotval.h
+-rw-rw-rw-   0        0        0    17990 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftoutln.h
+-rw-rw-rw-   0        0        0     6259 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftparams.h
+-rw-rw-rw-   0        0        0     5087 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftpfr.h
+-rw-rw-rw-   0        0        0     6869 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftrender.h
+-rw-rw-rw-   0        0        0     4447 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftsizes.h
+-rw-rw-rw-   0        0        0     8002 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftsnames.h
+-rw-rw-rw-   0        0        0    22546 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftstroke.h
+-rw-rw-rw-   0        0        0     3932 2023-02-09 05:51:54.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftsynth.h
+-rw-rw-rw-   0        0        0     9181 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftsystem.h
+-rw-rw-rw-   0        0        0     7761 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/fttrigon.h
+-rw-rw-rw-   0        0        0    15352 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/fttypes.h
+-rw-rw-rw-   0        0        0     8241 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ftwinfnt.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.562340 cgl-py-0.0.9/include/freetype/include/freetype/internal/
+-rw-rw-rw-   0        0        0     7732 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/autohint.h
+-rw-rw-rw-   0        0        0     2461 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/cffotypes.h
+-rw-rw-rw-   0        0        0    12282 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/cfftypes.h
+-rw-rw-rw-   0        0        0    11678 2023-02-08 20:24:39.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/compiler-macros.h
+-rw-rw-rw-   0        0        0    16187 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftcalc.h
+-rw-rw-rw-   0        0        0    13774 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftdebug.h
+-rw-rw-rw-   0        0        0     9497 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftdrv.h
+-rw-rw-rw-   0        0        0     4651 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftgloadr.h
+-rw-rw-rw-   0        0        0     3377 2022-09-01 09:52:14.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/fthash.h
+-rw-rw-rw-   0        0        0    16359 2023-02-08 20:09:03.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftmemory.h
+-rw-rw-rw-   0        0        0     2549 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftmmtypes.h
+-rw-rw-rw-   0        0        0    43719 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftobjs.h
+-rw-rw-rw-   0        0        0     1177 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftpsprop.h
+-rw-rw-rw-   0        0        0     7896 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftrfork.h
+-rw-rw-rw-   0        0        0    24548 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftserv.h
+-rw-rw-rw-   0        0        0    23800 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftstream.h
+-rw-rw-rw-   0        0        0     6090 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/fttrace.h
+-rw-rw-rw-   0        0        0     5922 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/ftvalid.h
+-rw-rw-rw-   0        0        0    44675 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/psaux.h
+-rw-rw-rw-   0        0        0    21551 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/pshints.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.574020 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/
+-rw-rw-rw-   0        0        0     1797 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svbdf.h
+-rw-rw-rw-   0        0        0     2922 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svcfftl.h
+-rw-rw-rw-   0        0        0     2193 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svcid.h
+-rw-rw-rw-   0        0        0     1403 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svfntfmt.h
+-rw-rw-rw-   0        0        0     1937 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svgldict.h
+-rw-rw-rw-   0        0        0     1802 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svgxval.h
+-rw-rw-rw-   0        0        0     1131 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svkern.h
+-rw-rw-rw-   0        0        0     3880 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svmetric.h
+-rw-rw-rw-   0        0        0     8197 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svmm.h
+-rw-rw-rw-   0        0        0     1308 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svotval.h
+-rw-rw-rw-   0        0        0     1635 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpfr.h
+-rw-rw-rw-   0        0        0     1636 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpostnm.h
+-rw-rw-rw-   0        0        0     1743 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svprop.h
+-rw-rw-rw-   0        0        0     4419 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpscmap.h
+-rw-rw-rw-   0        0        0     2555 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpsinfo.h
+-rw-rw-rw-   0        0        0     2167 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svsfnt.h
+-rw-rw-rw-   0        0        0     2487 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svttcmap.h
+-rw-rw-rw-   0        0        0     1060 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svtteng.h
+-rw-rw-rw-   0        0        0     1307 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svttglyf.h
+-rw-rw-rw-   0        0        0     1067 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svwinfnt.h
+-rw-rw-rw-   0        0        0    33536 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/sfnt.h
+-rw-rw-rw-   0        0        0     1087 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/svginterface.h
+-rw-rw-rw-   0        0        0     8484 2023-02-05 06:51:42.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/t1types.h
+-rw-rw-rw-   0        0        0    54710 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/tttypes.h
+-rw-rw-rw-   0        0        0     8322 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/internal/wofftypes.h
+-rw-rw-rw-   0        0        0    10793 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/otsvg.h
+-rw-rw-rw-   0        0        0    23981 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/t1tables.h
+-rw-rw-rw-   0        0        0    60004 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/ttnameid.h
+-rw-rw-rw-   0        0        0    26082 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/tttables.h
+-rw-rw-rw-   0        0        0     5269 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/freetype/tttags.h
+-rw-rw-rw-   0        0        0     1032 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/include/ft2build.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.482426 cgl-py-0.0.9/include/freetype/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.584729 cgl-py-0.0.9/include/freetype/src/autofit/
+-rw-rw-rw-   0        0        0    17366 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afblue.h
+-rw-rw-rw-   0        0        0     4332 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afcjk.h
+-rw-rw-rw-   0        0        0     3264 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afcover.h
+-rw-rw-rw-   0        0        0      917 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afdummy.h
+-rw-rw-rw-   0        0        0     1026 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/aferrors.h
+-rw-rw-rw-   0        0        0     5292 2023-02-08 20:09:32.000000 cgl-py-0.0.9/include/freetype/src/autofit/afglobal.h
+-rw-rw-rw-   0        0        0    16415 2023-02-08 20:09:03.000000 cgl-py-0.0.9/include/freetype/src/autofit/afhints.h
+-rw-rw-rw-   0        0        0      881 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afindic.h
+-rw-rw-rw-   0        0        0     6978 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/aflatin.h
+-rw-rw-rw-   0        0        0     2360 2023-02-08 20:09:32.000000 cgl-py-0.0.9/include/freetype/src/autofit/afloader.h
+-rw-rw-rw-   0        0        0     1236 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afmodule.h
+-rw-rw-rw-   0        0        0     1130 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afranges.h
+-rw-rw-rw-   0        0        0    11872 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afscript.h
+-rw-rw-rw-   0        0        0     1726 2023-02-08 20:37:13.000000 cgl-py-0.0.9/include/freetype/src/autofit/afshaper.h
+-rw-rw-rw-   0        0        0    15602 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afstyles.h
+-rw-rw-rw-   0        0        0    19135 2023-02-08 20:09:03.000000 cgl-py-0.0.9/include/freetype/src/autofit/aftypes.h
+-rw-rw-rw-   0        0        0      905 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afws-decl.h
+-rw-rw-rw-   0        0        0      997 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/autofit/afws-iter.h
+-rw-rw-rw-   0        0        0     1511 2023-02-08 20:47:06.000000 cgl-py-0.0.9/include/freetype/src/autofit/ft-hb.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.585701 cgl-py-0.0.9/include/freetype/src/base/
+-rw-rw-rw-   0        0        0     2733 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/base/ftbase.h
+-rw-rw-rw-   0        0        0     1455 2020-07-23 07:10:04.000000 cgl-py-0.0.9/include/freetype/src/base/md5.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.587648 cgl-py-0.0.9/include/freetype/src/bdf/
+-rw-rw-rw-   0        0        0     8490 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/bdf/bdf.h
+-rw-rw-rw-   0        0        0     1844 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/bdf/bdfdrivr.h
+-rw-rw-rw-   0        0        0     1629 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/bdf/bdferror.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.592514 cgl-py-0.0.9/include/freetype/src/cache/
+-rw-rw-rw-   0        0        0    15577 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftccache.h
+-rw-rw-rw-   0        0        0     2313 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftccback.h
+-rw-rw-rw-   0        0        0     1041 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcerror.h
+-rw-rw-rw-   0        0        0    11886 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcglyph.h
+-rw-rw-rw-   0        0        0     2781 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcimage.h
+-rw-rw-rw-   0        0        0     5909 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcmanag.h
+-rw-rw-rw-   0        0        0     8773 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcmru.h
+-rw-rw-rw-   0        0        0     2513 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cache/ftcsbits.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.597410 cgl-py-0.0.9/include/freetype/src/cff/
+-rw-rw-rw-   0        0        0     2248 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffcmap.h
+-rw-rw-rw-   0        0        0      787 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffdrivr.h
+-rw-rw-rw-   0        0        0     1001 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cfferrs.h
+-rw-rw-rw-   0        0        0     1585 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffgload.h
+-rw-rw-rw-   0        0        0     3423 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffload.h
+-rw-rw-rw-   0        0        0     2024 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffobjs.h
+-rw-rw-rw-   0        0        0     3671 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cffparse.h
+-rw-rw-rw-   0        0        0     6922 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cff/cfftoken.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.601306 cgl-py-0.0.9/include/freetype/src/cid/
+-rw-rw-rw-   0        0        0      999 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/ciderrs.h
+-rw-rw-rw-   0        0        0     1226 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidgload.h
+-rw-rw-rw-   0        0        0     1167 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidload.h
+-rw-rw-rw-   0        0        0     3566 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidobjs.h
+-rw-rw-rw-   0        0        0     3648 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidparse.h
+-rw-rw-rw-   0        0        0      808 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidriver.h
+-rw-rw-rw-   0        0        0     4502 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/cid/cidtoken.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.606172 cgl-py-0.0.9/include/freetype/src/gxvalid/
+-rw-rw-rw-   0        0        0     2976 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvalid.h
+-rw-rw-rw-   0        0        0    23564 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvcommn.h
+-rw-rw-rw-   0        0        0     1384 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxverror.h
+-rw-rw-rw-   0        0        0     6227 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvfeat.h
+-rw-rw-rw-   0        0        0     1139 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmod.h
+-rw-rw-rw-   0        0        0     3070 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmort.h
+-rw-rw-rw-   0        0        0     2149 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmorx.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.612986 cgl-py-0.0.9/include/freetype/src/gzip/
+-rw-rw-rw-   0        0        0   601195 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/gzip/crc32.h
+-rw-rw-rw-   0        0        0    17172 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gzip/ftzconf.h
+-rw-rw-rw-   0        0        0     7062 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/gzip/gzguts.h
+-rw-rw-rw-   0        0        0      445 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gzip/inffast.h
+-rw-rw-rw-   0        0        0     6426 2022-12-14 09:30:46.000000 cgl-py-0.0.9/include/freetype/src/gzip/inffixed.h
+-rw-rw-rw-   0        0        0     6876 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/gzip/inflate.h
+-rw-rw-rw-   0        0        0     3067 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gzip/inftrees.h
+-rw-rw-rw-   0        0        0    99975 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gzip/zlib.h
+-rw-rw-rw-   0        0        0     7679 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/gzip/zutil.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.612986 cgl-py-0.0.9/include/freetype/src/lzw/
+-rw-rw-rw-   0        0        0     5273 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/lzw/ftzopen.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.615906 cgl-py-0.0.9/include/freetype/src/otvalid/
+-rw-rw-rw-   0        0        0     2204 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/otvalid/otvalid.h
+-rw-rw-rw-   0        0        0    19811 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/otvalid/otvcommn.h
+-rw-rw-rw-   0        0        0     1059 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/otvalid/otverror.h
+-rw-rw-rw-   0        0        0      822 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/otvalid/otvgpos.h
+-rw-rw-rw-   0        0        0      816 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/otvalid/otvmod.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.619799 cgl-py-0.0.9/include/freetype/src/pcf/
+-rw-rw-rw-   0        0        0     6624 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/pcf/pcf.h
+-rw-rw-rw-   0        0        0     1402 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/pcf/pcfdrivr.h
+-rw-rw-rw-   0        0        0     1000 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/pcf/pcferror.h
+-rw-rw-rw-   0        0        0     1405 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/pcf/pcfread.h
+-rw-rw-rw-   0        0        0     1704 2022-09-01 09:52:15.000000 cgl-py-0.0.9/include/freetype/src/pcf/pcfutil.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.623692 cgl-py-0.0.9/include/freetype/src/pfr/
+-rw-rw-rw-   0        0        0      965 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrcmap.h
+-rw-rw-rw-   0        0        0      809 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrdrivr.h
+-rw-rw-rw-   0        0        0     1003 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrerror.h
+-rw-rw-rw-   0        0        0     1108 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrgload.h
+-rw-rw-rw-   0        0        0     3548 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrload.h
+-rw-rw-rw-   0        0        0     2231 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrobjs.h
+-rw-rw-rw-   0        0        0      915 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrsbit.h
+-rw-rw-rw-   0        0        0     8421 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pfr/pfrtypes.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.636345 cgl-py-0.0.9/include/freetype/src/psaux/
+-rw-rw-rw-   0        0        0     1913 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/afmparse.h
+-rw-rw-rw-   0        0        0     1888 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/cffdecode.h
+-rw-rw-rw-   0        0        0     3575 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psarrst.h
+-rw-rw-rw-   0        0        0     1045 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/psauxerr.h
+-rw-rw-rw-   0        0        0     1307 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/psauxmod.h
+-rw-rw-rw-   0        0        0     6180 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psblues.h
+-rw-rw-rw-   0        0        0     1770 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/psconv.h
+-rw-rw-rw-   0        0        0     4144 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/pserror.h
+-rw-rw-rw-   0        0        0     3837 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psfixed.h
+-rw-rw-rw-   0        0        0     5536 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psfont.h
+-rw-rw-rw-   0        0        0     5561 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psft.h
+-rw-rw-rw-   0        0        0     4645 2023-01-17 18:03:58.000000 cgl-py-0.0.9/include/freetype/src/psaux/psglue.h
+-rw-rw-rw-   0        0        0    10157 2023-01-17 18:03:59.000000 cgl-py-0.0.9/include/freetype/src/psaux/pshints.h
+-rw-rw-rw-   0        0        0     3157 2023-01-17 18:03:59.000000 cgl-py-0.0.9/include/freetype/src/psaux/psintrp.h
+-rw-rw-rw-   0        0        0    10595 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/psobjs.h
+-rw-rw-rw-   0        0        0     2367 2023-01-17 18:03:59.000000 cgl-py-0.0.9/include/freetype/src/psaux/psread.h
+-rw-rw-rw-   0        0        0     3817 2023-01-17 18:03:59.000000 cgl-py-0.0.9/include/freetype/src/psaux/psstack.h
+-rw-rw-rw-   0        0        0     2751 2023-01-17 18:03:59.000000 cgl-py-0.0.9/include/freetype/src/psaux/pstypes.h
+-rw-rw-rw-   0        0        0     3386 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/t1cmap.h
+-rw-rw-rw-   0        0        0     2097 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psaux/t1decode.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.638292 cgl-py-0.0.9/include/freetype/src/pshinter/
+-rw-rw-rw-   0        0        0     6849 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pshinter/pshalgo.h
+-rw-rw-rw-   0        0        0     5056 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pshinter/pshglob.h
+-rw-rw-rw-   0        0        0      779 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pshinter/pshmod.h
+-rw-rw-rw-   0        0        0     1019 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pshinter/pshnterr.h
+-rw-rw-rw-   0        0        0     4274 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/pshinter/pshrec.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.640238 cgl-py-0.0.9/include/freetype/src/psnames/
+-rw-rw-rw-   0        0        0      785 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psnames/psmodule.h
+-rw-rw-rw-   0        0        0     1041 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psnames/psnamerr.h
+-rw-rw-rw-   0        0        0   272382 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/psnames/pstables.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.643159 cgl-py-0.0.9/include/freetype/src/raster/
+-rw-rw-rw-   0        0        0     3108 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/raster/ftmisc.h
+-rw-rw-rw-   0        0        0     1139 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/raster/ftraster.h
+-rw-rw-rw-   0        0        0      792 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/raster/ftrend1.h
+-rw-rw-rw-   0        0        0     1047 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/raster/rasterrs.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.645105 cgl-py-0.0.9/include/freetype/src/sdf/
+-rw-rw-rw-   0        0        0     3011 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sdf/ftsdf.h
+-rw-rw-rw-   0        0        0     4148 2023-02-08 04:27:48.000000 cgl-py-0.0.9/include/freetype/src/sdf/ftsdfcommon.h
+-rw-rw-rw-   0        0        0      885 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sdf/ftsdferrs.h
+-rw-rw-rw-   0        0        0     3504 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sdf/ftsdfrend.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.657759 cgl-py-0.0.9/include/freetype/src/sfnt/
+-rw-rw-rw-   0        0        0     1234 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/pngshim.h
+-rw-rw-rw-   0        0        0      775 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/sfdriver.h
+-rw-rw-rw-   0        0        0     1007 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/sferrors.h
+-rw-rw-rw-   0        0        0     1475 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/sfobjs.h
+-rw-rw-rw-   0        0        0      908 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/sfwoff.h
+-rw-rw-rw-   0        0        0     2202 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/sfwoff2.h
+-rw-rw-rw-   0        0        0     1078 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttbdf.h
+-rw-rw-rw-   0        0        0     3853 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttcmap.h
+-rw-rw-rw-   0        0        0     1283 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttcmapc.h
+-rw-rw-rw-   0        0        0     2609 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttcolr.h
+-rw-rw-rw-   0        0        0     1084 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttcpal.h
+-rw-rw-rw-   0        0        0     1250 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttkern.h
+-rw-rw-rw-   0        0        0     2618 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttload.h
+-rw-rw-rw-   0        0        0     1343 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttmtx.h
+-rw-rw-rw-   0        0        0     1048 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttpost.h
+-rw-rw-rw-   0        0        0     1734 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttsbit.h
+-rw-rw-rw-   0        0        0     1057 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/ttsvg.h
+-rw-rw-rw-   0        0        0      908 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/sfnt/woff2tags.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.658732 cgl-py-0.0.9/include/freetype/src/smooth/
+-rw-rw-rw-   0        0        0     1317 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/smooth/ftgrays.h
+-rw-rw-rw-   0        0        0     1039 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/smooth/ftsmerrs.h
+-rw-rw-rw-   0        0        0      788 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/smooth/ftsmooth.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.660678 cgl-py-0.0.9/include/freetype/src/svg/
+-rw-rw-rw-   0        0        0      845 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/svg/ftsvg.h
+-rw-rw-rw-   0        0        0     1237 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/svg/svgtypes.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.665545 cgl-py-0.0.9/include/freetype/src/truetype/
+-rw-rw-rw-   0        0        0      783 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttdriver.h
+-rw-rw-rw-   0        0        0     1023 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/tterrors.h
+-rw-rw-rw-   0        0        0     1419 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttgload.h
+-rw-rw-rw-   0        0        0    13878 2023-02-08 16:14:41.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttgxvar.h
+-rw-rw-rw-   0        0        0    22350 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttinterp.h
+-rw-rw-rw-   0        0        0    12476 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttobjs.h
+-rw-rw-rw-   0        0        0     1732 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttpload.h
+-rw-rw-rw-   0        0        0     3958 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/truetype/ttsubpix.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.671385 cgl-py-0.0.9/include/freetype/src/type1/
+-rw-rw-rw-   0        0        0     1338 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1afm.h
+-rw-rw-rw-   0        0        0      804 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1driver.h
+-rw-rw-rw-   0        0        0     1010 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1errors.h
+-rw-rw-rw-   0        0        0     1245 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1gload.h
+-rw-rw-rw-   0        0        0     3411 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1load.h
+-rw-rw-rw-   0        0        0     3612 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1objs.h
+-rw-rw-rw-   0        0        0     3872 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1parse.h
+-rw-rw-rw-   0        0        0     5226 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type1/t1tokens.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.674305 cgl-py-0.0.9/include/freetype/src/type42/
+-rw-rw-rw-   0        0        0      775 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type42/t42drivr.h
+-rw-rw-rw-   0        0        0     1014 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type42/t42error.h
+-rw-rw-rw-   0        0        0     2575 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type42/t42objs.h
+-rw-rw-rw-   0        0        0     2120 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type42/t42parse.h
+-rw-rw-rw-   0        0        0     1237 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/type42/t42types.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.675280 cgl-py-0.0.9/include/freetype/src/winfonts/
+-rw-rw-rw-   0        0        0     1030 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/winfonts/fnterrs.h
+-rw-rw-rw-   0        0        0     3268 2023-02-04 14:00:05.000000 cgl-py-0.0.9/include/freetype/src/winfonts/winfnt.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.483402 cgl-py-0.0.9/include/glad/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.483402 cgl-py-0.0.9/include/glad/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.675280 cgl-py-0.0.9/include/glad/include/KHR/
+-rw-rw-rw-   0        0        0    11131 2022-11-02 08:36:46.000000 cgl-py-0.0.9/include/glad/include/KHR/khrplatform.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.676252 cgl-py-0.0.9/include/glad/include/glad/
+-rw-rw-rw-   0        0        0  1115714 2022-11-02 08:36:46.000000 cgl-py-0.0.9/include/glad/include/glad/glad.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.485348 cgl-py-0.0.9/include/glfw/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.682092 cgl-py-0.0.9/include/glfw/deps/
+-rw-rw-rw-   0        0        0     2193 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/getopt.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.684042 cgl-py-0.0.9/include/glfw/deps/glad/
+-rw-rw-rw-   0        0        0   332433 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/glad/gl.h
+-rw-rw-rw-   0        0        0    82918 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/glad/gles2.h
+-rw-rw-rw-   0        0        0   342527 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/glad/vulkan.h
+-rw-rw-rw-   0        0        0    14729 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/linmath.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.686962 cgl-py-0.0.9/include/glfw/deps/mingw/
+-rw-rw-rw-   0        0        0     3228 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/mingw/_mingw_dxhelper.h
+-rw-rw-rw-   0        0        0   115027 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/mingw/dinput.h
+-rw-rw-rw-   0        0        0     8189 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/mingw/xinput.h
+-rw-rw-rw-   0        0        0  1016476 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/nuklear.h
+-rw-rw-rw-   0        0        0    14462 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/nuklear_glfw_gl2.h
+-rw-rw-rw-   0        0        0    72945 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/stb_image_write.h
+-rw-rw-rw-   0        0        0    16103 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/tinycthread.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.686962 cgl-py-0.0.9/include/glfw/deps/vs2008/
+-rw-rw-rw-   0        0        0     7975 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/deps/vs2008/stdint.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.485348 cgl-py-0.0.9/include/glfw/include/
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.688908 cgl-py-0.0.9/include/glfw/include/GLFW/
+-rw-rw-rw-   0        0        0   242360 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/include/GLFW/glfw3.h
+-rw-rw-rw-   0        0        0    20689 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/include/GLFW/glfw3native.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.698672 cgl-py-0.0.9/include/glfw/src/
+-rw-rw-rw-   0        0        0     1935 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/cocoa_joystick.h
+-rw-rw-rw-   0        0        0    13208 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/cocoa_platform.h
+-rw-rw-rw-   0        0        0     1413 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/cocoa_time.h
+-rw-rw-rw-   0        0        0    37247 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/internal.h
+-rw-rw-rw-   0        0        0     2379 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/linux_joystick.h
+-rw-rw-rw-   0        0        0   258038 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/mappings.h
+-rw-rw-rw-   0        0        0     1456 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/null_joystick.h
+-rw-rw-rw-   0        0        0     7154 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/null_platform.h
+-rw-rw-rw-   0        0        0     5183 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/platform.h
+-rw-rw-rw-   0        0        0     1474 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/posix_poll.h
+-rw-rw-rw-   0        0        0     1723 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/posix_thread.h
+-rw-rw-rw-   0        0        0     1530 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/posix_time.h
+-rw-rw-rw-   0        0        0     1958 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/win32_joystick.h
+-rw-rw-rw-   0        0        0    25565 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/win32_platform.h
+-rw-rw-rw-   0        0        0     1760 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/win32_thread.h
+-rw-rw-rw-   0        0        0     1497 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/win32_time.h
+-rw-rw-rw-   0        0        0    26218 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/wl_platform.h
+-rw-rw-rw-   0        0        0    45741 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/x11_platform.h
+-rw-rw-rw-   0        0        0     1318 2022-08-18 08:28:59.000000 cgl-py-0.0.9/include/glfw/src/xkb_unicode.h
+drwxrwxrwx   0        0        0        0 2023-04-19 16:29:19.716192 cgl-py-0.0.9/lib/
+-rw-rw-rw-   0        0        0   657284 2023-04-19 11:36:50.000000 cgl-py-0.0.9/lib/cgl.lib
+-rw-rw-rw-   0        0        0  1862890 2023-04-18 07:47:30.000000 cgl-py-0.0.9/lib/freetype.lib
+-rw-rw-rw-   0        0        0  1764004 2023-04-18 07:47:32.000000 cgl-py-0.0.9/lib/glad.lib
+-rw-rw-rw-   0        0        0   699066 2023-04-18 07:47:35.000000 cgl-py-0.0.9/lib/glfw3.lib
+-rw-rw-rw-   0        0        0  1097268 2023-04-19 11:39:31.000000 cgl-py-0.0.9/lib/libcgl.a
+-rw-rw-rw-   0        0        0  6517496 2023-04-18 12:01:42.000000 cgl-py-0.0.9/lib/libfreetype.a
+-rw-rw-rw-   0        0        0  2245782 2023-04-18 12:31:41.000000 cgl-py-0.0.9/lib/libglad.a
+-rw-rw-rw-   0        0        0  2808432 2023-04-18 12:01:45.000000 cgl-py-0.0.9/lib/libglfw3.a
+-rw-rw-rw-   0        0        0      150 2023-04-19 16:28:52.000000 cgl-py-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:29:19.720085 cgl-py-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2725 2023-04-19 16:29:03.000000 cgl-py-0.0.9/setup.py
```

### Comparing `cgl-py-0.0.8/LICENSE` & `cgl-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/PKG-INFO` & `cgl-py-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgl-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python Wrapper for CGL
 Home-page: https://github.com/Jaysmito101/cgl
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://www.libcgl.tech/
 Project-URL: Issue tracker, https://github.com/Jaysmito101/cgl/issues
```

### Comparing `cgl-py-0.0.8/README.md` & `cgl-py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/cgl_py.egg-info/PKG-INFO` & `cgl-py-0.0.9/cgl_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgl-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python Wrapper for CGL
 Home-page: https://github.com/Jaysmito101/cgl
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://www.libcgl.tech/
 Project-URL: Issue tracker, https://github.com/Jaysmito101/cgl/issues
```

### Comparing `cgl-py-0.0.8/cgl_py.egg-info/SOURCES.txt` & `cgl-py-0.0.9/cgl_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 cgl_wrapper.c
 cgl_wrapper.pyx
+pyproject.toml
 setup.py
 ./cgl_wrapper.pyx
 cgl_py.egg-info/PKG-INFO
 cgl_py.egg-info/SOURCES.txt
 cgl_py.egg-info/dependency_links.txt
 cgl_py.egg-info/requires.txt
 cgl_py.egg-info/top_level.txt
```

### Comparing `cgl-py-0.0.8/cgl_wrapper.c` & `cgl-py-0.0.9/cgl_wrapper.c`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/cgl_wrapper.pyx` & `cgl-py-0.0.9/cgl_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/cgl.h` & `cgl-py-0.0.9/include/cgl.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/builds/amiga/include/config/ftconfig.h` & `cgl-py-0.0.9/include/freetype/builds/amiga/include/config/ftconfig.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/builds/amiga/include/config/ftmodule.h` & `cgl-py-0.0.9/include/freetype/builds/amiga/include/config/ftmodule.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/builds/vms/ftconfig.h` & `cgl-py-0.0.9/include/freetype/builds/vms/ftconfig.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/devel/ft2build.h` & `cgl-py-0.0.9/include/freetype/devel/ft2build.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/devel/ftoption.h` & `cgl-py-0.0.9/include/freetype/devel/ftoption.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/dlg/dlg.h` & `cgl-py-0.0.9/include/freetype/include/dlg/dlg.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/dlg/output.h` & `cgl-py-0.0.9/include/freetype/include/dlg/output.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/ftconfig.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/ftconfig.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/ftheader.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/ftheader.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/ftmodule.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/ftmodule.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/ftoption.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/ftoption.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/ftstdlib.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/ftstdlib.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/integer-types.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/integer-types.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/mac-support.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/mac-support.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/config/public-macros.h` & `cgl-py-0.0.9/include/freetype/include/freetype/config/public-macros.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/freetype.h` & `cgl-py-0.0.9/include/freetype/include/freetype/freetype.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftadvanc.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftadvanc.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftbbox.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftbbox.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftbdf.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftbdf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftbitmap.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftbitmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftbzip2.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftbzip2.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftcache.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftcache.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftchapters.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftchapters.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftcid.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftcid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftcolor.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftcolor.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftdriver.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftdriver.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/fterrdef.h` & `cgl-py-0.0.9/include/freetype/include/freetype/fterrdef.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/fterrors.h` & `cgl-py-0.0.9/include/freetype/include/freetype/fterrors.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftfntfmt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftfntfmt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftgasp.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftgasp.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftglyph.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftglyph.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftgxval.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftgxval.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftgzip.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftgzip.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftimage.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftimage.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftincrem.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftincrem.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftlcdfil.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftlcdfil.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftlist.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftlist.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftlogging.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftlogging.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftlzw.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftlzw.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftmac.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftmac.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftmm.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftmm.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftmodapi.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftmodapi.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftmoderr.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftmoderr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftotval.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftotval.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftoutln.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftoutln.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftparams.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftparams.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftpfr.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftpfr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftrender.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftrender.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftsizes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftsizes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftsnames.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftsnames.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftstroke.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftstroke.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftsynth.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftsynth.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftsystem.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftsystem.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/fttrigon.h` & `cgl-py-0.0.9/include/freetype/include/freetype/fttrigon.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/fttypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/fttypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ftwinfnt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ftwinfnt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/autohint.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/autohint.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/cffotypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/cffotypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/cfftypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/cfftypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/compiler-macros.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/compiler-macros.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftcalc.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftcalc.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftdebug.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftdebug.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftdrv.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftdrv.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftgloadr.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftgloadr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/fthash.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/fthash.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftmemory.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftmemory.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftmmtypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftmmtypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftobjs.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftpsprop.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftpsprop.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftrfork.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftrfork.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftserv.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftserv.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftstream.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftstream.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/fttrace.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/fttrace.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/ftvalid.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/ftvalid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/psaux.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/psaux.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/pshints.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/pshints.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svbdf.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svbdf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svcfftl.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svcfftl.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svcid.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svcid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svfntfmt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svfntfmt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svgldict.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svgldict.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svgxval.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svgxval.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svkern.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svkern.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svmetric.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svmetric.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svmm.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svmm.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svotval.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svotval.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpfr.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpfr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpostnm.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpostnm.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svprop.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svprop.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpscmap.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpscmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svpsinfo.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svpsinfo.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svsfnt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svsfnt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svttcmap.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svttcmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svtteng.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svtteng.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svttglyf.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svttglyf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/services/svwinfnt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/services/svwinfnt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/sfnt.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/sfnt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/svginterface.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/svginterface.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/t1types.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/t1types.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/tttypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/tttypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/internal/wofftypes.h` & `cgl-py-0.0.9/include/freetype/include/freetype/internal/wofftypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/otsvg.h` & `cgl-py-0.0.9/include/freetype/include/freetype/otsvg.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/t1tables.h` & `cgl-py-0.0.9/include/freetype/include/freetype/t1tables.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/ttnameid.h` & `cgl-py-0.0.9/include/freetype/include/freetype/ttnameid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/tttables.h` & `cgl-py-0.0.9/include/freetype/include/freetype/tttables.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/freetype/tttags.h` & `cgl-py-0.0.9/include/freetype/include/freetype/tttags.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/include/ft2build.h` & `cgl-py-0.0.9/include/freetype/include/ft2build.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afblue.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afblue.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afcjk.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afcjk.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afcover.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afcover.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afdummy.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afdummy.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/aferrors.h` & `cgl-py-0.0.9/include/freetype/src/autofit/aferrors.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afglobal.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afglobal.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afhints.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afhints.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afindic.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afindic.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/aflatin.h` & `cgl-py-0.0.9/include/freetype/src/autofit/aflatin.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afloader.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afloader.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afmodule.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afmodule.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afranges.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afranges.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afscript.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afscript.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afshaper.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afshaper.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afstyles.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afstyles.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/aftypes.h` & `cgl-py-0.0.9/include/freetype/src/autofit/aftypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afws-decl.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afws-decl.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/afws-iter.h` & `cgl-py-0.0.9/include/freetype/src/autofit/afws-iter.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/autofit/ft-hb.h` & `cgl-py-0.0.9/include/freetype/src/autofit/ft-hb.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/base/ftbase.h` & `cgl-py-0.0.9/include/freetype/src/base/ftbase.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/base/md5.h` & `cgl-py-0.0.9/include/freetype/src/base/md5.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/bdf/bdf.h` & `cgl-py-0.0.9/include/freetype/src/bdf/bdf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/bdf/bdfdrivr.h` & `cgl-py-0.0.9/include/freetype/src/bdf/bdfdrivr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/bdf/bdferror.h` & `cgl-py-0.0.9/include/freetype/src/bdf/bdferror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftccache.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftccache.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftccback.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftccback.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcerror.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcerror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcglyph.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcglyph.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcimage.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcimage.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcmanag.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcmanag.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcmru.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcmru.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cache/ftcsbits.h` & `cgl-py-0.0.9/include/freetype/src/cache/ftcsbits.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffcmap.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffcmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffdrivr.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffdrivr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cfferrs.h` & `cgl-py-0.0.9/include/freetype/src/cff/cfferrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffgload.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffgload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffload.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffobjs.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cffparse.h` & `cgl-py-0.0.9/include/freetype/src/cff/cffparse.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cff/cfftoken.h` & `cgl-py-0.0.9/include/freetype/src/cff/cfftoken.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/ciderrs.h` & `cgl-py-0.0.9/include/freetype/src/cid/ciderrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidgload.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidgload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidload.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidobjs.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidparse.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidparse.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidriver.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidriver.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/cid/cidtoken.h` & `cgl-py-0.0.9/include/freetype/src/cid/cidtoken.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvalid.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvalid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvcommn.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvcommn.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxverror.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxverror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvfeat.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvfeat.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmod.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmod.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmort.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmort.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gxvalid/gxvmorx.h` & `cgl-py-0.0.9/include/freetype/src/gxvalid/gxvmorx.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/crc32.h` & `cgl-py-0.0.9/include/freetype/src/gzip/crc32.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/ftzconf.h` & `cgl-py-0.0.9/include/freetype/src/gzip/ftzconf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/gzguts.h` & `cgl-py-0.0.9/include/freetype/src/gzip/gzguts.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/inffixed.h` & `cgl-py-0.0.9/include/freetype/src/gzip/inffixed.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/inflate.h` & `cgl-py-0.0.9/include/freetype/src/gzip/inflate.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/inftrees.h` & `cgl-py-0.0.9/include/freetype/src/gzip/inftrees.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/zlib.h` & `cgl-py-0.0.9/include/freetype/src/gzip/zlib.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/gzip/zutil.h` & `cgl-py-0.0.9/include/freetype/src/gzip/zutil.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/lzw/ftzopen.h` & `cgl-py-0.0.9/include/freetype/src/lzw/ftzopen.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/otvalid/otvalid.h` & `cgl-py-0.0.9/include/freetype/src/otvalid/otvalid.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/otvalid/otvcommn.h` & `cgl-py-0.0.9/include/freetype/src/otvalid/otvcommn.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/otvalid/otverror.h` & `cgl-py-0.0.9/include/freetype/src/otvalid/otverror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/otvalid/otvgpos.h` & `cgl-py-0.0.9/include/freetype/src/otvalid/otvgpos.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/otvalid/otvmod.h` & `cgl-py-0.0.9/include/freetype/src/otvalid/otvmod.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pcf/pcf.h` & `cgl-py-0.0.9/include/freetype/src/pcf/pcf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pcf/pcfdrivr.h` & `cgl-py-0.0.9/include/freetype/src/pcf/pcfdrivr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pcf/pcferror.h` & `cgl-py-0.0.9/include/freetype/src/pcf/pcferror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pcf/pcfread.h` & `cgl-py-0.0.9/include/freetype/src/pcf/pcfread.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pcf/pcfutil.h` & `cgl-py-0.0.9/include/freetype/src/pcf/pcfutil.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrcmap.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrcmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrdrivr.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrdrivr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrerror.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrerror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrgload.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrgload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrload.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrobjs.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrsbit.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrsbit.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pfr/pfrtypes.h` & `cgl-py-0.0.9/include/freetype/src/pfr/pfrtypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/afmparse.h` & `cgl-py-0.0.9/include/freetype/src/psaux/afmparse.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/cffdecode.h` & `cgl-py-0.0.9/include/freetype/src/psaux/cffdecode.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psarrst.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psarrst.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psauxerr.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psauxerr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psauxmod.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psauxmod.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psblues.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psblues.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psconv.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psconv.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/pserror.h` & `cgl-py-0.0.9/include/freetype/src/psaux/pserror.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psfixed.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psfixed.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psfont.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psfont.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psft.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psft.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psglue.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psglue.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/pshints.h` & `cgl-py-0.0.9/include/freetype/src/psaux/pshints.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psintrp.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psintrp.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psobjs.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psread.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psread.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/psstack.h` & `cgl-py-0.0.9/include/freetype/src/psaux/psstack.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/pstypes.h` & `cgl-py-0.0.9/include/freetype/src/psaux/pstypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/t1cmap.h` & `cgl-py-0.0.9/include/freetype/src/psaux/t1cmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psaux/t1decode.h` & `cgl-py-0.0.9/include/freetype/src/psaux/t1decode.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pshinter/pshalgo.h` & `cgl-py-0.0.9/include/freetype/src/pshinter/pshalgo.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pshinter/pshglob.h` & `cgl-py-0.0.9/include/freetype/src/pshinter/pshglob.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pshinter/pshmod.h` & `cgl-py-0.0.9/include/freetype/src/pshinter/pshmod.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pshinter/pshnterr.h` & `cgl-py-0.0.9/include/freetype/src/pshinter/pshnterr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/pshinter/pshrec.h` & `cgl-py-0.0.9/include/freetype/src/pshinter/pshrec.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psnames/psmodule.h` & `cgl-py-0.0.9/include/freetype/src/psnames/psmodule.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psnames/psnamerr.h` & `cgl-py-0.0.9/include/freetype/src/psnames/psnamerr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/psnames/pstables.h` & `cgl-py-0.0.9/include/freetype/src/psnames/pstables.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/raster/ftmisc.h` & `cgl-py-0.0.9/include/freetype/src/raster/ftmisc.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/raster/ftraster.h` & `cgl-py-0.0.9/include/freetype/src/raster/ftraster.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/raster/ftrend1.h` & `cgl-py-0.0.9/include/freetype/src/raster/ftrend1.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/raster/rasterrs.h` & `cgl-py-0.0.9/include/freetype/src/raster/rasterrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sdf/ftsdf.h` & `cgl-py-0.0.9/include/freetype/src/sdf/ftsdf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sdf/ftsdfcommon.h` & `cgl-py-0.0.9/include/freetype/src/sdf/ftsdfcommon.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sdf/ftsdferrs.h` & `cgl-py-0.0.9/include/freetype/src/sdf/ftsdferrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sdf/ftsdfrend.h` & `cgl-py-0.0.9/include/freetype/src/sdf/ftsdfrend.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/pngshim.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/pngshim.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/sfdriver.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/sfdriver.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/sferrors.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/sferrors.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/sfobjs.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/sfobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/sfwoff.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/sfwoff.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/sfwoff2.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/sfwoff2.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttbdf.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttbdf.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttcmap.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttcmap.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttcmapc.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttcmapc.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttcolr.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttcolr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttcpal.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttcpal.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttkern.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttkern.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttload.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttmtx.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttmtx.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttpost.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttpost.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttsbit.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttsbit.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/ttsvg.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/ttsvg.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/sfnt/woff2tags.h` & `cgl-py-0.0.9/include/freetype/src/sfnt/woff2tags.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/smooth/ftgrays.h` & `cgl-py-0.0.9/include/freetype/src/smooth/ftgrays.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/smooth/ftsmerrs.h` & `cgl-py-0.0.9/include/freetype/src/smooth/ftsmerrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/smooth/ftsmooth.h` & `cgl-py-0.0.9/include/freetype/src/smooth/ftsmooth.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/svg/ftsvg.h` & `cgl-py-0.0.9/include/freetype/src/svg/ftsvg.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/svg/svgtypes.h` & `cgl-py-0.0.9/include/freetype/src/svg/svgtypes.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttdriver.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttdriver.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/tterrors.h` & `cgl-py-0.0.9/include/freetype/src/truetype/tterrors.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttgload.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttgload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttgxvar.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttgxvar.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttinterp.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttinterp.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttobjs.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttobjs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttpload.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttpload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/truetype/ttsubpix.h` & `cgl-py-0.0.9/include/freetype/src/truetype/ttsubpix.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1afm.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1afm.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1driver.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1driver.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1errors.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1errors.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1gload.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1gload.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1load.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1load.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1objs.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1objs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1parse.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1parse.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type1/t1tokens.h` & `cgl-py-0.0.9/include/freetype/src/type1/t1tokens.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type42/t42drivr.h` & `cgl-py-0.0.9/include/freetype/src/type42/t42drivr.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type42/t42error.h` & `cgl-py-0.0.9/include/freetype/src/type42/t42error.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type42/t42objs.h` & `cgl-py-0.0.9/include/freetype/src/type42/t42objs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type42/t42parse.h` & `cgl-py-0.0.9/include/freetype/src/type42/t42parse.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/type42/t42types.h` & `cgl-py-0.0.9/include/freetype/src/type42/t42types.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/winfonts/fnterrs.h` & `cgl-py-0.0.9/include/freetype/src/winfonts/fnterrs.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/freetype/src/winfonts/winfnt.h` & `cgl-py-0.0.9/include/freetype/src/winfonts/winfnt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glad/include/KHR/khrplatform.h` & `cgl-py-0.0.9/include/glad/include/KHR/khrplatform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glad/include/glad/glad.h` & `cgl-py-0.0.9/include/glad/include/glad/glad.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/getopt.h` & `cgl-py-0.0.9/include/glfw/deps/getopt.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/glad/gl.h` & `cgl-py-0.0.9/include/glfw/deps/glad/gl.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/glad/gles2.h` & `cgl-py-0.0.9/include/glfw/deps/glad/gles2.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/glad/vulkan.h` & `cgl-py-0.0.9/include/glfw/deps/glad/vulkan.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/linmath.h` & `cgl-py-0.0.9/include/glfw/deps/linmath.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/mingw/_mingw_dxhelper.h` & `cgl-py-0.0.9/include/glfw/deps/mingw/_mingw_dxhelper.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/mingw/dinput.h` & `cgl-py-0.0.9/include/glfw/deps/mingw/dinput.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/mingw/xinput.h` & `cgl-py-0.0.9/include/glfw/deps/mingw/xinput.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/nuklear.h` & `cgl-py-0.0.9/include/glfw/deps/nuklear.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/nuklear_glfw_gl2.h` & `cgl-py-0.0.9/include/glfw/deps/nuklear_glfw_gl2.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/stb_image_write.h` & `cgl-py-0.0.9/include/glfw/deps/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/tinycthread.h` & `cgl-py-0.0.9/include/glfw/deps/tinycthread.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/deps/vs2008/stdint.h` & `cgl-py-0.0.9/include/glfw/deps/vs2008/stdint.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/include/GLFW/glfw3.h` & `cgl-py-0.0.9/include/glfw/include/GLFW/glfw3.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/include/GLFW/glfw3native.h` & `cgl-py-0.0.9/include/glfw/include/GLFW/glfw3native.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/cocoa_joystick.h` & `cgl-py-0.0.9/include/glfw/src/cocoa_joystick.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/cocoa_platform.h` & `cgl-py-0.0.9/include/glfw/src/cocoa_platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/cocoa_time.h` & `cgl-py-0.0.9/include/glfw/src/cocoa_time.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/internal.h` & `cgl-py-0.0.9/include/glfw/src/internal.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/linux_joystick.h` & `cgl-py-0.0.9/include/glfw/src/linux_joystick.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/mappings.h` & `cgl-py-0.0.9/include/glfw/src/mappings.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/null_joystick.h` & `cgl-py-0.0.9/include/glfw/src/null_joystick.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/null_platform.h` & `cgl-py-0.0.9/include/glfw/src/null_platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/platform.h` & `cgl-py-0.0.9/include/glfw/src/platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/posix_poll.h` & `cgl-py-0.0.9/include/glfw/src/posix_poll.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/posix_thread.h` & `cgl-py-0.0.9/include/glfw/src/posix_thread.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/posix_time.h` & `cgl-py-0.0.9/include/glfw/src/posix_time.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/win32_joystick.h` & `cgl-py-0.0.9/include/glfw/src/win32_joystick.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/win32_platform.h` & `cgl-py-0.0.9/include/glfw/src/win32_platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/win32_thread.h` & `cgl-py-0.0.9/include/glfw/src/win32_thread.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/win32_time.h` & `cgl-py-0.0.9/include/glfw/src/win32_time.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/wl_platform.h` & `cgl-py-0.0.9/include/glfw/src/wl_platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/x11_platform.h` & `cgl-py-0.0.9/include/glfw/src/x11_platform.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/include/glfw/src/xkb_unicode.h` & `cgl-py-0.0.9/include/glfw/src/xkb_unicode.h`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/cgl.lib` & `cgl-py-0.0.9/lib/cgl.lib`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/freetype.lib` & `cgl-py-0.0.9/lib/freetype.lib`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/glad.lib` & `cgl-py-0.0.9/lib/glad.lib`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/glfw3.lib` & `cgl-py-0.0.9/lib/glfw3.lib`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/libcgl.a` & `cgl-py-0.0.9/lib/libcgl.a`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/libfreetype.a` & `cgl-py-0.0.9/lib/libfreetype.a`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/libglad.a` & `cgl-py-0.0.9/lib/libglad.a`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/lib/libglfw3.a` & `cgl-py-0.0.9/lib/libglfw3.a`

 * *Files identical despite different names*

### Comparing `cgl-py-0.0.8/setup.py` & `cgl-py-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if platform.system() == 'Windows':
         return []
     else:
         return ["-Wl,-rpath=$ORIGIN/lib/."]
 
 requirements = ["PyOpenGL", "glfw", "Cython", "Pillow"] 
 
-version = '0.0.8'
+version = '0.0.9'
 
 readme = 'Coming Soon ...'
 
 required_libraries = ['cgl', 'glfw3', 'glad', 'freetype']
 
 if platform.system() == 'Windows':
     required_libraries.append('user32')
```

