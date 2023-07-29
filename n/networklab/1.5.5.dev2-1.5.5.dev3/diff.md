# Comparing `tmp/networklab-1.5.5.dev2.tar.gz` & `tmp/networklab-1.5.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.5.dev2.tar", last modified: Thu Jul 27 16:26:33 2023, max compression
+gzip compressed data, was "networklab-1.5.5.dev3.tar", last modified: Sat Jul 29 06:48:57 2023, max compression
```

## Comparing `networklab-1.5.5.dev2.tar` & `networklab-1.5.5.dev3.tar`

### file list

```diff
@@ -1,644 +1,644 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.277910 networklab-1.5.5.dev2/
--rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/LICENSE.md
--rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/MANIFEST.in
--rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-27 16:26:33.277752 networklab-1.5.5.dev2/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)     3030 2023-07-11 15:49:20.000000 networklab-1.5.5.dev2/README.md
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.084218 networklab-1.5.5.dev2/netsim/
--rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-07-27 16:26:10.000000 networklab-1.5.5.dev2/netsim/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/addressing.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.085687 networklab-1.5.5.dev2/netsim/ansible/
--rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     2899 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/config.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/create-config.ansible
--rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.5.dev2/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     3460 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/initial-config.ansible
--rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.5.dev2/netsim/ansible/missing.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.086356 networklab-1.5.5.dev2/netsim/ansible/tasks/
--rw-r--r--   0 pipi       (501) staff       (20)      720 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.091019 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3196 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2250 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.094916 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.098052 networklab-1.5.5.dev2/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.098444 networklab-1.5.5.dev2/netsim/ansible/tasks/frr/
--rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)      243 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/frr/mpls-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.098680 networklab-1.5.5.dev2/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.098930 networklab-1.5.5.dev2/netsim/ansible/tasks/linux/
--rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.099169 networklab-1.5.5.dev2/netsim/ansible/tasks/nxos/
--rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.099913 networklab-1.5.5.dev2/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.100179 networklab-1.5.5.dev2/netsim/ansible/tasks/vmx/
--rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.5.dev2/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.100410 networklab-1.5.5.dev2/netsim/ansible/templates/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.102062 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/
--rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1267 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.108872 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/
--rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     8056 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3504 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.109213 networklab-1.5.5.dev2/netsim/ansible/templates/eigrp/
--rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.111503 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/
--rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1631 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1853 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1239 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.113456 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/
--rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.5.dev2/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.125534 networklab-1.5.5.dev2/netsim/ansible/templates/initial/
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     5288 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3945 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1706 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.126276 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      923 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3481 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2026 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3479 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4863 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.5.dev2/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.129098 networklab-1.5.5.dev2/netsim/ansible/templates/isis/
--rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.5.dev2/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.160609 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/
--rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      562 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1159 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      342 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.171917 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/
--rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1964 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.173894 networklab-1.5.5.dev2/netsim/ansible/templates/sr/
--rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.174174 networklab-1.5.5.dev2/netsim/ansible/templates/srv6/
--rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.178170 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/
--rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.195717 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.201975 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/
--rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1929 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2234 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/api.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.206501 networklab-1.5.5.dev2/netsim/augment/
--rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/augment/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/augment/components.py
--rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/augment/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     6452 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/augment/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)    18000 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/augment/groups.py
--rw-r--r--   0 pipi       (501) staff       (20)    40803 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/augment/links.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/augment/main.py
--rw-r--r--   0 pipi       (501) staff       (20)    12868 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/augment/nodes.py
--rw-r--r--   0 pipi       (501) staff       (20)     2810 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/augment/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     7621 2023-07-13 14:26:22.000000 networklab-1.5.5.dev2/netsim/augment/topology.py
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/callback.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.216593 networklab-1.5.5.dev2/netsim/cli/
--rwxr-xr-x   0 pipi       (501) staff       (20)     9773 2023-07-27 05:51:10.000000 networklab-1.5.5.dev2/netsim/cli/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.5.dev2/netsim/cli/alias.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1716 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     4169 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.5.dev2/netsim/cli/collect.py
--rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.5.dev2/netsim/cli/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     5545 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/connect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/cli/create.py
--rw-r--r--   0 pipi       (501) staff       (20)     7029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/cli/down.py
--rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.5.dev2/netsim/cli/empty.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6323 2023-07-27 06:04:59.000000 networklab-1.5.5.dev2/netsim/cli/external_commands.py
--rw-r--r--   0 pipi       (501) staff       (20)     1583 2023-07-13 14:12:56.000000 networklab-1.5.5.dev2/netsim/cli/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/cli/initial.py
--rw-r--r--   0 pipi       (501) staff       (20)     2043 2023-07-13 14:28:37.000000 networklab-1.5.5.dev2/netsim/cli/inspect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2027 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/install.py
--rw-r--r--   0 pipi       (501) staff       (20)     9994 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.5.dev2/netsim/cli/read.py
--rw-r--r--   0 pipi       (501) staff       (20)     1424 2023-07-13 14:13:04.000000 networklab-1.5.5.dev2/netsim/cli/report.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/cli/restart.py
--rw-r--r--   0 pipi       (501) staff       (20)     9161 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/show.py
--rw-r--r--   0 pipi       (501) staff       (20)     4774 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     3431 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/cli/test.py
--rw-r--r--   0 pipi       (501) staff       (20)    10868 2023-07-27 10:32:32.000000 networklab-1.5.5.dev2/netsim/cli/up.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.5.dev2/netsim/cli/usage.py
--rw-r--r--   0 pipi       (501) staff       (20)     2287 2023-07-13 14:38:47.000000 networklab-1.5.5.dev2/netsim/cli/usage.txt
--rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/cli/version.py
--rw-r--r--   0 pipi       (501) staff       (20)      752 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/common.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.218790 networklab-1.5.5.dev2/netsim/data/
--rw-r--r--   0 pipi       (501) staff       (20)     4332 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/data/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/data/filemaps.py
--rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/data/global_vars.py
--rw-r--r--   0 pipi       (501) staff       (20)    20638 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/data/types.py
--rw-r--r--   0 pipi       (501) staff       (20)    19573 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/data/validate.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.220265 networklab-1.5.5.dev2/netsim/defaults/
--rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/defaults/addressing.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2452 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/defaults/attributes.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/defaults/automation.yml
--rw-r--r--   0 pipi       (501) staff       (20)      610 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/defaults/hints.yml
--rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/defaults/multilab.yml
--rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/defaults/ports.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.227779 networklab-1.5.5.dev2/netsim/devices/
--rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/arubacx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/asav.py
--rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/devices/asav.yml
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/csr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/eos.py
--rw-r--r--   0 pipi       (501) staff       (20)     1642 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1210 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/iosv.py
--rw-r--r--   0 pipi       (501) staff       (20)     1449 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/iosv.yml
--rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/junos.py
--rw-r--r--   0 pipi       (501) staff       (20)      757 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/devices/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      923 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1355 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/devices/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1671 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/devices/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      932 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/devices/unknown.py
--rw-r--r--   0 pipi       (501) staff       (20)      115 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/devices/unknown.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/vmx.py
--rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/vmx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/vptx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1638 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/devices/vptx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/devices/vsrx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1275 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/devices/vsrx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/devices/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.079751 networklab-1.5.5.dev2/netsim/extra/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.228082 networklab-1.5.5.dev2/netsim/extra/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.5.dev2/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.234242 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.234754 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2162 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.5.dev2/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.235187 networklab-1.5.5.dev2/netsim/extra/multilab/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.235742 networklab-1.5.5.dev2/netsim/extra/multilab/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.5.dev2/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.5.dev2/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.5.dev2/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.235969 networklab-1.5.5.dev2/netsim/extra/none/
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/extra/none/none.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.236561 networklab-1.5.5.dev2/netsim/extra/proxy-arp/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.237226 networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.238329 networklab-1.5.5.dev2/netsim/install/
--rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.5.dev2/netsim/install/ansible.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     3619 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/containerlab.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.5.dev2/netsim/install/grpc.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.241711 networklab-1.5.5.dev2/netsim/install/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.241945 networklab-1.5.5.dev2/netsim/install/libvirt/asav/
--rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/install/libvirt/asav.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.5.dev2/netsim/install/libvirt/csr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.5.dev2/netsim/install/libvirt/eos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/install/libvirt/iosv.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.242475 networklab-1.5.5.dev2/netsim/install/libvirt/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.5.dev2/netsim/install/libvirt/iosxr/iosxr_config.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.5.dev2/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.5.dev2/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.244349 networklab-1.5.5.dev2/netsim/install/libvirt/vptx/
--rw-r--r--   0 pipi       (501) staff       (20)     1994 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 pipi       (501) staff       (20)     1089 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      654 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2552 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.248440 networklab-1.5.5.dev2/netsim/install/libvirt/vsrx/
--rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.5.dev2/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 pipi       (501) staff       (20)     3185 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/install/libvirt.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.5.dev2/netsim/install/ubuntu.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.256817 networklab-1.5.5.dev2/netsim/modules/
--rw-r--r--   0 pipi       (501) staff       (20)    23644 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/_dataplane.py
--rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/_routing.py
--rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.5.dev2/netsim/modules/bfd.py
--rw-r--r--   0 pipi       (501) staff       (20)      724 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/bfd.yml
--rw-r--r--   0 pipi       (501) staff       (20)    21025 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/modules/bgp.py
--rw-r--r--   0 pipi       (501) staff       (20)     1843 2023-07-13 14:46:51.000000 networklab-1.5.5.dev2/netsim/modules/bgp.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.5.dev2/netsim/modules/eigrp.py
--rw-r--r--   0 pipi       (501) staff       (20)      318 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/eigrp.yml
--rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/evpn.py
--rw-r--r--   0 pipi       (501) staff       (20)     1119 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/evpn.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/gateway.py
--rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/gateway.yml
--rw-r--r--   0 pipi       (501) staff       (20)      141 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/modules/isis.py
--rw-r--r--   0 pipi       (501) staff       (20)     1074 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/isis.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/mpls.py
--rw-r--r--   0 pipi       (501) staff       (20)     1060 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/mpls.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3764 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/ospf.py
--rw-r--r--   0 pipi       (501) staff       (20)     1389 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/ospf.yml
--rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/modules/sr.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/sr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.5.dev2/netsim/modules/srv6.py
--rw-r--r--   0 pipi       (501) staff       (20)      518 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/srv6.yml
--rw-r--r--   0 pipi       (501) staff       (20)    58909 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/modules/vlan.py
--rw-r--r--   0 pipi       (501) staff       (20)     1246 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/vlan.yml
--rw-r--r--   0 pipi       (501) staff       (20)    22607 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/modules/vrf.py
--rw-r--r--   0 pipi       (501) staff       (20)      458 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/vrf.yml
--rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/modules/vxlan.py
--rw-r--r--   0 pipi       (501) staff       (20)      591 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/modules/vxlan.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.259894 networklab-1.5.5.dev2/netsim/outputs/
--rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/outputs/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     7386 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/outputs/common.py
--rw-r--r--   0 pipi       (501) staff       (20)    10023 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/d2.py
--rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/outputs/d2.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2805 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)      255 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/format.py
--rw-r--r--   0 pipi       (501) staff       (20)     7556 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/outputs/graph.yml
--rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/outputs/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.5.dev2/netsim/outputs/json.py
--rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.5.dev2/netsim/outputs/none.py
--rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/outputs/provider.py
--rw-r--r--   0 pipi       (501) staff       (20)     2235 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/report.py
--rw-r--r--   0 pipi       (501) staff       (20)     2893 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/outputs/tools.py
--rw-r--r--   0 pipi       (501) staff       (20)     1678 2023-07-13 14:21:52.000000 networklab-1.5.5.dev2/netsim/outputs/yaml.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.262997 networklab-1.5.5.dev2/netsim/providers/
--rw-r--r--   0 pipi       (501) staff       (20)     9311 2023-07-27 16:25:46.000000 networklab-1.5.5.dev2/netsim/providers/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/providers/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)      989 2023-07-27 16:25:46.000000 networklab-1.5.5.dev2/netsim/providers/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.5.dev2/netsim/providers/external.py
--rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/providers/external.yml
--rw-r--r--   0 pipi       (501) staff       (20)    13565 2023-07-27 16:25:46.000000 networklab-1.5.5.dev2/netsim/providers/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1157 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/providers/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.5.dev2/netsim/providers/virtualbox.py
--rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/providers/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)     8373 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/read_topology.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.263287 networklab-1.5.5.dev2/netsim/templates/
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.5.dev2/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.081153 networklab-1.5.5.dev2/netsim/templates/provider/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.263566 networklab-1.5.5.dev2/netsim/templates/provider/clab/
--rw-r--r--   0 pipi       (501) staff       (20)     3857 2023-07-27 16:25:46.000000 networklab-1.5.5.dev2/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.263823 networklab-1.5.5.dev2/netsim/templates/provider/clab/frr/
--rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.264137 networklab-1.5.5.dev2/netsim/templates/provider/clab/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.5.dev2/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.264432 networklab-1.5.5.dev2/netsim/templates/provider/external/
--rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.5.dev2/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.271216 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)      683 2023-07-27 10:09:42.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      952 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 15:22:47.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 pipi       (501) staff       (20)     2728 2023-06-10 16:45:53.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.273234 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/
--rw-r--r--   0 pipi       (501) staff       (20)      818 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2023-06-25 16:15:11.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.273970 networklab-1.5.5.dev2/netsim/templates/tests/
--rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.5.dev2/netsim/templates/tests/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.5.dev2/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.5.dev2/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.275016 networklab-1.5.5.dev2/netsim/tools/
--rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/tools/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/tools/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      614 2023-05-15 07:05:40.000000 networklab-1.5.5.dev2/netsim/tools/graphite.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.275170 networklab-1.5.5.dev2/netsim/tools/suzieq/
--rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/tools/suzieq.yml
--rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/netsim/topology-defaults.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.276489 networklab-1.5.5.dev2/netsim/utils/
--rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/netsim/utils/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     2216 2023-07-27 05:43:15.000000 networklab-1.5.5.dev2/netsim/utils/files.py
--rw-r--r--   0 pipi       (501) staff       (20)     4079 2023-07-09 07:35:25.000000 networklab-1.5.5.dev2/netsim/utils/log.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.5.dev2/netsim/utils/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     1784 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/utils/strings.py
--rw-r--r--   0 pipi       (501) staff       (20)     5411 2023-07-09 07:35:01.000000 networklab-1.5.5.dev2/netsim/utils/templates.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.277314 networklab-1.5.5.dev2/networklab.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)    21652 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       51 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/entry_points.txt
--rw-r--r--   0 pipi       (501) staff       (20)      120 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        7 2023-07-27 16:26:33.000000 networklab-1.5.5.dev2/networklab.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-27 06:49:41.000000 networklab-1.5.5.dev2/requirements.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-07-27 16:26:33.277948 networklab-1.5.5.dev2/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.5.dev2/setup.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-27 16:26:33.277446 networklab-1.5.5.dev2/tests/
--rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.5.dev2/tests/test_transformation.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099838 networklab-1.5.5.dev3/
+-rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/LICENSE.md
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/MANIFEST.in
+-rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-29 06:48:57.099691 networklab-1.5.5.dev3/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)     3030 2023-07-11 15:49:20.000000 networklab-1.5.5.dev3/README.md
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.899815 networklab-1.5.5.dev3/netsim/
+-rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-07-29 06:48:30.000000 networklab-1.5.5.dev3/netsim/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/addressing.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.901251 networklab-1.5.5.dev3/netsim/ansible/
+-rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     2899 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/config.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/create-config.ansible
+-rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.5.dev3/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3460 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.5.dev3/netsim/ansible/missing.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.901965 networklab-1.5.5.dev3/netsim/ansible/tasks/
+-rw-r--r--   0 pipi       (501) staff       (20)      720 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.906272 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3196 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2250 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.912504 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.912962 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913316 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)      555 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      243 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/frr/mpls-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913556 networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913782 networklab-1.5.5.dev3/netsim/ansible/tasks/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.913987 networklab-1.5.5.dev3/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.914703 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.914974 networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.915213 networklab-1.5.5.dev3/netsim/ansible/templates/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.920670 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1267 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.927242 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     8056 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3504 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.927577 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.929749 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/
+-rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1631 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1853 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1239 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.931944 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/
+-rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.948049 networklab-1.5.5.dev3/netsim/ansible/templates/initial/
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     5288 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3945 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1706 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.948907 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      923 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3481 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2026 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3479 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4863 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.952394 networklab-1.5.5.dev3/netsim/ansible/templates/isis/
+-rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.961886 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/
+-rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      562 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1159 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      342 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.982613 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/
+-rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1964 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.984503 networklab-1.5.5.dev3/netsim/ansible/templates/sr/
+-rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.984794 networklab-1.5.5.dev3/netsim/ansible/templates/srv6/
+-rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.990761 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.019325 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.026113 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1929 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2234 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/api.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.028975 networklab-1.5.5.dev3/netsim/augment/
+-rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/augment/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/augment/components.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/augment/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6452 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)    18000 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/groups.py
+-rw-r--r--   0 pipi       (501) staff       (20)    40803 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/links.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/main.py
+-rw-r--r--   0 pipi       (501) staff       (20)    12868 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/augment/nodes.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2810 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/augment/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7621 2023-07-13 14:26:22.000000 networklab-1.5.5.dev3/netsim/augment/topology.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/callback.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.035974 networklab-1.5.5.dev3/netsim/cli/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     9773 2023-07-27 05:51:10.000000 networklab-1.5.5.dev3/netsim/cli/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.5.dev3/netsim/cli/alias.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1716 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4169 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.5.dev3/netsim/cli/collect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.5.dev3/netsim/cli/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5545 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/connect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/cli/create.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7029 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/cli/down.py
+-rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/cli/empty.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6323 2023-07-27 06:04:59.000000 networklab-1.5.5.dev3/netsim/cli/external_commands.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1583 2023-07-13 14:12:56.000000 networklab-1.5.5.dev3/netsim/cli/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/cli/initial.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2043 2023-07-13 14:28:37.000000 networklab-1.5.5.dev3/netsim/cli/inspect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2027 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/install.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9994 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.5.dev3/netsim/cli/read.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1424 2023-07-13 14:13:04.000000 networklab-1.5.5.dev3/netsim/cli/report.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/cli/restart.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9161 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/show.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4774 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3431 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/cli/test.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10868 2023-07-27 10:32:32.000000 networklab-1.5.5.dev3/netsim/cli/up.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.5.dev3/netsim/cli/usage.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2287 2023-07-13 14:38:47.000000 networklab-1.5.5.dev3/netsim/cli/usage.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/cli/version.py
+-rw-r--r--   0 pipi       (501) staff       (20)      752 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/common.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.037158 networklab-1.5.5.dev3/netsim/data/
+-rw-r--r--   0 pipi       (501) staff       (20)     4332 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/data/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/data/filemaps.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/data/global_vars.py
+-rw-r--r--   0 pipi       (501) staff       (20)    20638 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/data/types.py
+-rw-r--r--   0 pipi       (501) staff       (20)    19573 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/data/validate.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.038754 networklab-1.5.5.dev3/netsim/defaults/
+-rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/addressing.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2557 2023-07-29 06:38:12.000000 networklab-1.5.5.dev3/netsim/defaults/attributes.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/automation.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      610 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/defaults/hints.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/multilab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/defaults/ports.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.051513 networklab-1.5.5.dev3/netsim/devices/
+-rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/arubacx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/asav.py
+-rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/devices/asav.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/csr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/eos.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1642 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1210 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/iosv.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1449 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/iosv.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/junos.py
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/devices/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      923 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1355 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1671 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/devices/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      932 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/unknown.py
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/devices/unknown.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vmx.py
+-rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/vmx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vptx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1638 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/devices/vptx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/devices/vsrx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1275 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/devices/vsrx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/devices/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.895416 networklab-1.5.5.dev3/netsim/extra/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.051789 networklab-1.5.5.dev3/netsim/extra/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.5.dev3/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.056629 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057173 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2162 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.5.dev3/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057453 networklab-1.5.5.dev3/netsim/extra/multilab/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.057979 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.5.dev3/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.058248 networklab-1.5.5.dev3/netsim/extra/none/
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/extra/none/none.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.059147 networklab-1.5.5.dev3/netsim/extra/proxy-arp/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.059969 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.061263 networklab-1.5.5.dev3/netsim/install/
+-rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.5.dev3/netsim/install/ansible.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3619 2023-07-27 16:30:58.000000 networklab-1.5.5.dev3/netsim/install/containerlab.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.5.dev3/netsim/install/grpc.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.064869 networklab-1.5.5.dev3/netsim/install/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.065165 networklab-1.5.5.dev3/netsim/install/libvirt/asav/
+-rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.5.dev3/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosv.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.065390 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr/iosxr_config.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.5.dev3/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.5.dev3/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.066251 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1994 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1089 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      654 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2552 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.066427 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.5.dev3/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3185 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/install/libvirt.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.5.dev3/netsim/install/ubuntu.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.074822 networklab-1.5.5.dev3/netsim/modules/
+-rw-r--r--   0 pipi       (501) staff       (20)    23644 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/_dataplane.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/_routing.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.5.dev3/netsim/modules/bfd.py
+-rw-r--r--   0 pipi       (501) staff       (20)      724 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/bfd.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    21025 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/modules/bgp.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1843 2023-07-13 14:46:51.000000 networklab-1.5.5.dev3/netsim/modules/bgp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.5.dev3/netsim/modules/eigrp.py
+-rw-r--r--   0 pipi       (501) staff       (20)      318 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/eigrp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/evpn.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1119 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/evpn.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/gateway.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1029 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/gateway.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      141 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/modules/isis.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1074 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/isis.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/mpls.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1060 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/mpls.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3764 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/ospf.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1389 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/ospf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/modules/sr.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/sr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.5.dev3/netsim/modules/srv6.py
+-rw-r--r--   0 pipi       (501) staff       (20)      518 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/srv6.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    58909 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/modules/vlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1246 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vlan.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    22607 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/modules/vrf.py
+-rw-r--r--   0 pipi       (501) staff       (20)      458 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vrf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/modules/vxlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)      591 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/modules/vxlan.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.078291 networklab-1.5.5.dev3/netsim/outputs/
+-rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7386 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/common.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10023 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/d2.py
+-rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/d2.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2805 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/format.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7556 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/outputs/graph.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/outputs/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.5.dev3/netsim/outputs/json.py
+-rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.5.dev3/netsim/outputs/none.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/outputs/provider.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2235 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/report.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2893 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/outputs/tools.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1678 2023-07-13 14:21:52.000000 networklab-1.5.5.dev3/netsim/outputs/yaml.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.080599 networklab-1.5.5.dev3/netsim/providers/
+-rw-r--r--   0 pipi       (501) staff       (20)     9311 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/providers/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/providers/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)      989 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/providers/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.5.dev3/netsim/providers/external.py
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/providers/external.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    13611 2023-07-27 16:28:14.000000 networklab-1.5.5.dev3/netsim/providers/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1157 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/providers/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.5.dev3/netsim/providers/virtualbox.py
+-rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/providers/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     8373 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/read_topology.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.080876 networklab-1.5.5.dev3/netsim/templates/
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.5.dev3/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:56.896657 networklab-1.5.5.dev3/netsim/templates/provider/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081132 networklab-1.5.5.dev3/netsim/templates/provider/clab/
+-rw-r--r--   0 pipi       (501) staff       (20)     3857 2023-07-27 16:25:46.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081366 networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081573 networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.081809 networklab-1.5.5.dev3/netsim/templates/provider/external/
+-rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.5.dev3/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.092400 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)      683 2023-07-27 10:09:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      952 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2023-06-25 15:22:47.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 pipi       (501) staff       (20)     2728 2023-06-10 16:45:53.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.094733 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 pipi       (501) staff       (20)      818 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2023-06-25 16:15:11.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.095517 networklab-1.5.5.dev3/netsim/templates/tests/
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.5.dev3/netsim/templates/tests/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.5.dev3/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.5.dev3/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.096596 networklab-1.5.5.dev3/netsim/tools/
+-rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      614 2023-05-15 07:05:40.000000 networklab-1.5.5.dev3/netsim/tools/graphite.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.096769 networklab-1.5.5.dev3/netsim/tools/suzieq/
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/tools/suzieq.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/netsim/topology-defaults.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.098310 networklab-1.5.5.dev3/netsim/utils/
+-rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/netsim/utils/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2216 2023-07-27 05:43:15.000000 networklab-1.5.5.dev3/netsim/utils/files.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4079 2023-07-09 07:35:25.000000 networklab-1.5.5.dev3/netsim/utils/log.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.5.dev3/netsim/utils/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1784 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/utils/strings.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5411 2023-07-09 07:35:01.000000 networklab-1.5.5.dev3/netsim/utils/templates.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099220 networklab-1.5.5.dev3/networklab.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)     3744 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)    21652 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       51 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      120 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        7 2023-07-29 06:48:56.000000 networklab-1.5.5.dev3/networklab.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-27 06:49:41.000000 networklab-1.5.5.dev3/requirements.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-07-29 06:48:57.099878 networklab-1.5.5.dev3/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.5.dev3/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-07-29 06:48:57.099383 networklab-1.5.5.dev3/tests/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.5.dev3/tests/test_transformation.py
```

### Comparing `networklab-1.5.5.dev2/LICENSE.md` & `networklab-1.5.5.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/PKG-INFO` & `networklab-1.5.5.dev3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.5.dev2
+Version: 1.5.5.dev3
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.5.dev2/README.md` & `networklab-1.5.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/addressing.py` & `networklab-1.5.5.dev3/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/collect-configs.ansible` & `networklab-1.5.5.dev3/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/config.ansible` & `networklab-1.5.5.dev3/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/create-config.ansible` & `networklab-1.5.5.dev3/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/initial-config.ansible` & `networklab-1.5.5.dev3/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/create-config.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.5.dev3/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.5.dev3/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/api.py` & `networklab-1.5.5.dev3/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/components.py` & `networklab-1.5.5.dev3/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/config.py` & `networklab-1.5.5.dev3/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/devices.py` & `networklab-1.5.5.dev3/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/groups.py` & `networklab-1.5.5.dev3/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/links.py` & `networklab-1.5.5.dev3/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/main.py` & `networklab-1.5.5.dev3/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/nodes.py` & `networklab-1.5.5.dev3/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/plugin.py` & `networklab-1.5.5.dev3/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/augment/topology.py` & `networklab-1.5.5.dev3/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/callback.py` & `networklab-1.5.5.dev3/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/__init__.py` & `networklab-1.5.5.dev3/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/ansible.py` & `networklab-1.5.5.dev3/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/clab.py` & `networklab-1.5.5.dev3/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/collect.py` & `networklab-1.5.5.dev3/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/config.py` & `networklab-1.5.5.dev3/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/connect.py` & `networklab-1.5.5.dev3/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/create.py` & `networklab-1.5.5.dev3/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/down.py` & `networklab-1.5.5.dev3/netsim/cli/down.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/external_commands.py` & `networklab-1.5.5.dev3/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/graph.py` & `networklab-1.5.5.dev3/netsim/cli/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/initial.py` & `networklab-1.5.5.dev3/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/inspect.py` & `networklab-1.5.5.dev3/netsim/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/install.py` & `networklab-1.5.5.dev3/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/libvirt.py` & `networklab-1.5.5.dev3/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/read.py` & `networklab-1.5.5.dev3/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/report.py` & `networklab-1.5.5.dev3/netsim/cli/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/restart.py` & `networklab-1.5.5.dev3/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/show.py` & `networklab-1.5.5.dev3/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/status.py` & `networklab-1.5.5.dev3/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/test.py` & `networklab-1.5.5.dev3/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/up.py` & `networklab-1.5.5.dev3/netsim/cli/up.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/cli/usage.txt` & `networklab-1.5.5.dev3/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/common.py` & `networklab-1.5.5.dev3/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/data/__init__.py` & `networklab-1.5.5.dev3/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/data/filemaps.py` & `networklab-1.5.5.dev3/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/data/global_vars.py` & `networklab-1.5.5.dev3/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/data/types.py` & `networklab-1.5.5.dev3/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/data/validate.py` & `networklab-1.5.5.dev3/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/defaults/attributes.yml` & `networklab-1.5.5.dev3/netsim/defaults/attributes.yml`

 * *Files 11% similar despite different names*

```diff
@@ -48,14 +48,19 @@
   module: list
   device: id
   box: str
   id: { type: int, min_value: 1, max_value: 150 }
   config: list
   group: list
   role: id
+  mgmt:
+    ipv4: { type: ipv4, use: id }
+    ipv6: { type: ipv6, use: id }
+    mac: str
+    ifname: str
   mtu: { type: int, min_value: 64, max_value: 65535 }
   loopback:
     ipv4: { type: ipv4, use: prefix }
     ipv6: { type: ipv6, use: prefix }
   provider: id
   cpu:
   memory: int
```

### Comparing `networklab-1.5.5.dev2/netsim/defaults/hints.yml` & `networklab-1.5.5.dev3/netsim/defaults/hints.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/__init__.py` & `networklab-1.5.5.dev3/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/arubacx.py` & `networklab-1.5.5.dev3/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/arubacx.yml` & `networklab-1.5.5.dev3/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/asav.py` & `networklab-1.5.5.dev3/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/asav.yml` & `networklab-1.5.5.dev3/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/csr.yml` & `networklab-1.5.5.dev3/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/cumulus.yml` & `networklab-1.5.5.dev3/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.5.dev3/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/dellos10.yml` & `networklab-1.5.5.dev3/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/eos.py` & `networklab-1.5.5.dev3/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/eos.yml` & `networklab-1.5.5.dev3/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/frr.yml` & `networklab-1.5.5.dev3/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/iosv.py` & `networklab-1.5.5.dev3/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/iosv.yml` & `networklab-1.5.5.dev3/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/iosxr.yml` & `networklab-1.5.5.dev3/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/junos.py` & `networklab-1.5.5.dev3/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/linux.yml` & `networklab-1.5.5.dev3/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/none.yml` & `networklab-1.5.5.dev3/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/nxos.yml` & `networklab-1.5.5.dev3/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/routeros7.yml` & `networklab-1.5.5.dev3/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/srlinux.yml` & `networklab-1.5.5.dev3/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/sros.yml` & `networklab-1.5.5.dev3/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/unknown.py` & `networklab-1.5.5.dev3/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vmx.py` & `networklab-1.5.5.dev3/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vmx.yml` & `networklab-1.5.5.dev3/netsim/devices/vmx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vptx.py` & `networklab-1.5.5.dev3/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vptx.yml` & `networklab-1.5.5.dev3/netsim/devices/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vsrx.py` & `networklab-1.5.5.dev3/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vsrx.yml` & `networklab-1.5.5.dev3/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/devices/vyos.yml` & `networklab-1.5.5.dev3/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc` & `networklab-1.5.5.dev3/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/frr.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.5.dev3/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc` & `networklab-1.5.5.dev3/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/multilab/plugin.py` & `networklab-1.5.5.dev3/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.5.dev3/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/ansible.sh` & `networklab-1.5.5.dev3/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/containerlab.sh` & `networklab-1.5.5.dev3/netsim/install/containerlab.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
 # Install a specific version of Containerlab
-CONTAINERLAB_VERSION="0.41.2"
+CONTAINERLAB_VERSION="0.43.0"
 
 cat <<EOM
 Docker/Containerlab Installation Script
 =====================================================================
 This script installs Docker and containerlab on a Debian or Ubuntu
 system. The script was tested on Debian 11.3 and Ubuntu 20.04.
```

### Comparing `networklab-1.5.5.dev2/netsim/install/grpc.sh` & `networklab-1.5.5.dev3/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/arubacx.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.5.dev3/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/csr.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/eos.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.5.dev3/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/iosv.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.5.dev3/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/nxos.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.5.dev3/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vptx/run.sh` & `networklab-1.5.5.dev3/netsim/install/libvirt/vptx/run.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vptx.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.5.5.dev3/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.5.dev3/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.5.dev3/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/libvirt.sh` & `networklab-1.5.5.dev3/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/install/ubuntu.sh` & `networklab-1.5.5.dev3/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/__init__.py` & `networklab-1.5.5.dev3/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/_dataplane.py` & `networklab-1.5.5.dev3/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/_routing.py` & `networklab-1.5.5.dev3/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/bfd.py` & `networklab-1.5.5.dev3/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/bfd.yml` & `networklab-1.5.5.dev3/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/bgp.py` & `networklab-1.5.5.dev3/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/bgp.yml` & `networklab-1.5.5.dev3/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/evpn.py` & `networklab-1.5.5.dev3/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/evpn.yml` & `networklab-1.5.5.dev3/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/gateway.py` & `networklab-1.5.5.dev3/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/gateway.yml` & `networklab-1.5.5.dev3/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/isis.py` & `networklab-1.5.5.dev3/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/isis.yml` & `networklab-1.5.5.dev3/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/mpls.py` & `networklab-1.5.5.dev3/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/mpls.yml` & `networklab-1.5.5.dev3/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/ospf.py` & `networklab-1.5.5.dev3/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/ospf.yml` & `networklab-1.5.5.dev3/netsim/modules/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/srv6.py` & `networklab-1.5.5.dev3/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/srv6.yml` & `networklab-1.5.5.dev3/netsim/modules/srv6.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/vlan.py` & `networklab-1.5.5.dev3/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/vlan.yml` & `networklab-1.5.5.dev3/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/vrf.py` & `networklab-1.5.5.dev3/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/vxlan.py` & `networklab-1.5.5.dev3/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/modules/vxlan.yml` & `networklab-1.5.5.dev3/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/__init__.py` & `networklab-1.5.5.dev3/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/ansible.py` & `networklab-1.5.5.dev3/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/common.py` & `networklab-1.5.5.dev3/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/d2.py` & `networklab-1.5.5.dev3/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/d2.yml` & `networklab-1.5.5.dev3/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/devices.py` & `networklab-1.5.5.dev3/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/graph.py` & `networklab-1.5.5.dev3/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/graphite.py` & `networklab-1.5.5.dev3/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/provider.py` & `networklab-1.5.5.dev3/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/report.py` & `networklab-1.5.5.dev3/netsim/outputs/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/tools.py` & `networklab-1.5.5.dev3/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/outputs/yaml.py` & `networklab-1.5.5.dev3/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/providers/__init__.py` & `networklab-1.5.5.dev3/netsim/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/providers/clab.py` & `networklab-1.5.5.dev3/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/providers/clab.yml` & `networklab-1.5.5.dev3/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/providers/external.py` & `networklab-1.5.5.dev3/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/providers/libvirt.py` & `networklab-1.5.5.dev3/netsim/providers/libvirt.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,24 +197,26 @@
 
 class Libvirt(_Provider):
 
   """
   post_transform hook: mark multi-provider links as LAN links
   """
   def pre_transform(self, topology: Box) -> None:
+    if not 'links' in topology:
+      _Provider.pre_transform(self,topology)
+      return
+
     for l in topology.links:                                     # Set 'uplink' attribute on 'public' links
       if not l.get('libvirt.public',False):                      # Skip links without 'public' attribute
         continue
       if l.get('libvirt.uplink',''):                             # Skip links with 'uplink' attribute
         continue
       l.libvirt.uplink = 'eth0'                                  # Default uplink name is eth0
 
     _Provider.pre_transform(self,topology)
-    if not 'links' in topology:
-      return
 
     for l in topology.links:
       if l.get('libvirt.uplink',None):                           # Set 'public' attribute if the link has an uplink
         if not 'public' in l.libvirt:                            # ... but no 'public' libvirt attr
           l.libvirt.public = 'bridge'                            # ... default mode is bridge (MACVTAP)
 
       if l.get('libvirt.provider',None):
```

### Comparing `networklab-1.5.5.dev2/netsim/providers/libvirt.yml` & `networklab-1.5.5.dev3/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/read_topology.py` & `networklab-1.5.5.dev3/netsim/read_topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/external/external.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.5.dev3/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/tools/__init__.py` & `networklab-1.5.5.dev3/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/tools/graphite.py` & `networklab-1.5.5.dev3/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/tools/graphite.yml` & `networklab-1.5.5.dev3/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/tools/suzieq.yml` & `networklab-1.5.5.dev3/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/topology-defaults.yml` & `networklab-1.5.5.dev3/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/utils/files.py` & `networklab-1.5.5.dev3/netsim/utils/files.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/utils/log.py` & `networklab-1.5.5.dev3/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/utils/status.py` & `networklab-1.5.5.dev3/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/utils/strings.py` & `networklab-1.5.5.dev3/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/netsim/utils/templates.py` & `networklab-1.5.5.dev3/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/networklab.egg-info/PKG-INFO` & `networklab-1.5.5.dev3/networklab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.5.dev2
+Version: 1.5.5.dev3
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.5.dev2/networklab.egg-info/SOURCES.txt` & `networklab-1.5.5.dev3/networklab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/setup.py` & `networklab-1.5.5.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.5.dev2/tests/test_transformation.py` & `networklab-1.5.5.dev3/tests/test_transformation.py`

 * *Files identical despite different names*

