# Comparing `tmp/lazyinit-0.0.27.tar.gz` & `tmp/lazyinit-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.27.tar", last modified: Thu Jul 27 11:55:42 2023, max compression
+gzip compressed data, was "lazyinit-0.0.28.tar", last modified: Sat Jul 29 00:33:34 2023, max compression
```

## Comparing `lazyinit-0.0.27.tar` & `lazyinit-0.0.28.tar`

### file list

```diff
@@ -1,346 +1,350 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.741329 lazyinit-0.0.27/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.657138 lazyinit-0.0.27/.git/
--rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/COMMIT_EDITMSG
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:12.000000 lazyinit-0.0.27/.git/FETCH_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/ORIG_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.27/.git/config
--rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/description
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660115 lazyinit-0.0.27/.git/hooks/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/post-update.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-push.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/update.sample
--rw-r--r--   0 dengyifan   (501) staff       (20)     4305 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/index
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660328 lazyinit-0.0.27/.git/info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/info/exclude
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660519 lazyinit-0.0.27/.git/logs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/logs/HEAD
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.644592 lazyinit-0.0.27/.git/logs/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660707 lazyinit-0.0.27/.git/logs/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/logs/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.644643 lazyinit-0.0.27/.git/logs/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661167 lazyinit-0.0.27/.git/logs/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)     4396 2023-07-27 10:59:16.000000 lazyinit-0.0.27/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)     1739 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/logs/refs/remotes/origin/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653260 lazyinit-0.0.27/.git/objects/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661354 lazyinit-0.0.27/.git/objects/00/
--r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661618 lazyinit-0.0.27/.git/objects/01/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.662081 lazyinit-0.0.27/.git/objects/04/
--r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
--r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.662468 lazyinit-0.0.27/.git/objects/05/
--r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
--r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.663379 lazyinit-0.0.27/.git/objects/0a/
--r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664161 lazyinit-0.0.27/.git/objects/0e/
--r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
--r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664457 lazyinit-0.0.27/.git/objects/11/
--r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664670 lazyinit-0.0.27/.git/objects/14/
--r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665038 lazyinit-0.0.27/.git/objects/1c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665346 lazyinit-0.0.27/.git/objects/1f/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665935 lazyinit-0.0.27/.git/objects/22/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
--r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.666155 lazyinit-0.0.27/.git/objects/24/
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.666495 lazyinit-0.0.27/.git/objects/28/
--r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667034 lazyinit-0.0.27/.git/objects/2a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667374 lazyinit-0.0.27/.git/objects/2b/
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667729 lazyinit-0.0.27/.git/objects/2d/
--r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668077 lazyinit-0.0.27/.git/objects/2e/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668654 lazyinit-0.0.27/.git/objects/32/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
--r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668975 lazyinit-0.0.27/.git/objects/33/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.669298 lazyinit-0.0.27/.git/objects/38/
--r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.671372 lazyinit-0.0.27/.git/objects/39/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.671966 lazyinit-0.0.27/.git/objects/3d/
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
--r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.672204 lazyinit-0.0.27/.git/objects/40/
--r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.674376 lazyinit-0.0.27/.git/objects/41/
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.675423 lazyinit-0.0.27/.git/objects/43/
--r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.679494 lazyinit-0.0.27/.git/objects/4d/
--r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.679870 lazyinit-0.0.27/.git/objects/52/
--r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.683917 lazyinit-0.0.27/.git/objects/55/
--r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.684280 lazyinit-0.0.27/.git/objects/56/
--r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.684525 lazyinit-0.0.27/.git/objects/5a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.685339 lazyinit-0.0.27/.git/objects/5e/
--r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.687164 lazyinit-0.0.27/.git/objects/5f/
--r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
--r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.689767 lazyinit-0.0.27/.git/objects/60/
--r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.690559 lazyinit-0.0.27/.git/objects/63/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
--r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.695061 lazyinit-0.0.27/.git/objects/64/
--r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.695832 lazyinit-0.0.27/.git/objects/67/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696122 lazyinit-0.0.27/.git/objects/69/
--r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696572 lazyinit-0.0.27/.git/objects/6a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696892 lazyinit-0.0.27/.git/objects/6b/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697393 lazyinit-0.0.27/.git/objects/6c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
--r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697594 lazyinit-0.0.27/.git/objects/6d/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697877 lazyinit-0.0.27/.git/objects/6e/
--r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.698630 lazyinit-0.0.27/.git/objects/6f/
--r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.698908 lazyinit-0.0.27/.git/objects/73/
--r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.701500 lazyinit-0.0.27/.git/objects/74/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
--r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.702074 lazyinit-0.0.27/.git/objects/7e/
--r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705056 lazyinit-0.0.27/.git/objects/7f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705283 lazyinit-0.0.27/.git/objects/80/
--r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705799 lazyinit-0.0.27/.git/objects/83/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
--r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706085 lazyinit-0.0.27/.git/objects/84/
--r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706481 lazyinit-0.0.27/.git/objects/86/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706786 lazyinit-0.0.27/.git/objects/87/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707142 lazyinit-0.0.27/.git/objects/88/
--r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707335 lazyinit-0.0.27/.git/objects/89/
--r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707536 lazyinit-0.0.27/.git/objects/8b/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707731 lazyinit-0.0.27/.git/objects/8f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/8f/821694556aac2a278c288de223659193dd2489
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707919 lazyinit-0.0.27/.git/objects/91/
--r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.708276 lazyinit-0.0.27/.git/objects/96/
--r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.708449 lazyinit-0.0.27/.git/objects/99/
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.709226 lazyinit-0.0.27/.git/objects/9c/
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.709688 lazyinit-0.0.27/.git/objects/9d/
--r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
--r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.710409 lazyinit-0.0.27/.git/objects/a0/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
--r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
--r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.710852 lazyinit-0.0.27/.git/objects/a1/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
--r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711120 lazyinit-0.0.27/.git/objects/a3/
--r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711562 lazyinit-0.0.27/.git/objects/a8/
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711838 lazyinit-0.0.27/.git/objects/a9/
--r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.712541 lazyinit-0.0.27/.git/objects/aa/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
--r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
--r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.712822 lazyinit-0.0.27/.git/objects/ad/
--r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.713312 lazyinit-0.0.27/.git/objects/ae/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
--r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.713889 lazyinit-0.0.27/.git/objects/af/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
--r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714429 lazyinit-0.0.27/.git/objects/b0/
--r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714654 lazyinit-0.0.27/.git/objects/b1/
--r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714852 lazyinit-0.0.27/.git/objects/b4/
--r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715454 lazyinit-0.0.27/.git/objects/b6/
--r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
--r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715703 lazyinit-0.0.27/.git/objects/b7/
--r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715905 lazyinit-0.0.27/.git/objects/bb/
--r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.717916 lazyinit-0.0.27/.git/objects/bc/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
--r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
--r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.718304 lazyinit-0.0.27/.git/objects/c1/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.718629 lazyinit-0.0.27/.git/objects/c4/
--r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719218 lazyinit-0.0.27/.git/objects/c5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
--r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719398 lazyinit-0.0.27/.git/objects/c7/
--r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719594 lazyinit-0.0.27/.git/objects/c9/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719929 lazyinit-0.0.27/.git/objects/ca/
--r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.720567 lazyinit-0.0.27/.git/objects/cc/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
--r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721044 lazyinit-0.0.27/.git/objects/cd/
--r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721183 lazyinit-0.0.27/.git/objects/ce/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721362 lazyinit-0.0.27/.git/objects/d9/
--r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721625 lazyinit-0.0.27/.git/objects/da/
--r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721886 lazyinit-0.0.27/.git/objects/de/
--r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722116 lazyinit-0.0.27/.git/objects/df/
--r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722304 lazyinit-0.0.27/.git/objects/e4/
--r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722564 lazyinit-0.0.27/.git/objects/e6/
--r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722956 lazyinit-0.0.27/.git/objects/e8/
--r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
--r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723417 lazyinit-0.0.27/.git/objects/eb/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
--r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723620 lazyinit-0.0.27/.git/objects/ec/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723884 lazyinit-0.0.27/.git/objects/ef/
--r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724354 lazyinit-0.0.27/.git/objects/f0/
--r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
--r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724563 lazyinit-0.0.27/.git/objects/f1/
--r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724760 lazyinit-0.0.27/.git/objects/f2/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724965 lazyinit-0.0.27/.git/objects/f5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725160 lazyinit-0.0.27/.git/objects/f6/
--r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653492 lazyinit-0.0.27/.git/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725360 lazyinit-0.0.27/.git/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653560 lazyinit-0.0.27/.git/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725997 lazyinit-0.0.27/.git/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-27 10:59:16.000000 lazyinit-0.0.27/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/refs/remotes/origin/master
--rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.27/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-27 11:55:42.740970 lazyinit-0.0.27/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.27/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.727707 lazyinit-0.0.27/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.27/lazyinit/__init__.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.731268 lazyinit-0.0.27/lazyinit/__pycache__/
--rw-r--r--   0 dengyifan   (501) staff       (20)     8725 2023-07-26 04:15:42.000000 lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.27/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8781 2023-07-27 11:55:34.000000 lazyinit-0.0.27/lazyinit/init.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732083 lazyinit-0.0.27/lazyinit/lazydl/
--rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732198 lazyinit-0.0.27/lazyinit/lazydl/configs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1569 2023-07-25 13:48:22.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/default_config.yaml
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732335 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732612 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/baseline.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)    74072 2023-07-25 04:24:11.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)      644 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/overfit_test.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.27/lazyinit/lazydl/minist.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/requirements.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.27/lazyinit/lazydl/start.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.734697 lazyinit-0.0.27/lazyinit/ranger/
--rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.27/lazyinit/ranger/.DS_Store
--rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.737118 lazyinit-0.0.27/lazyinit/ranger/colorschemes/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/default.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/jungle.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/zenburn.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/commands.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.740667 lazyinit-0.0.27/lazyinit/ranger/plugins/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rc-sample.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rc.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rifle.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/scope.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.27/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.27/lazyinit/redis.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.27/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6724 2023-07-27 11:48:11.000000 lazyinit-0.0.27/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.728692 lazyinit-0.0.27/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)    10070 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.27/push.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-27 11:55:42.741397 lazyinit-0.0.27/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-27 11:55:39.000000 lazyinit-0.0.27/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.781598 lazyinit-0.0.28/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.721032 lazyinit-0.0.28/.git/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/COMMIT_EDITMSG
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:30:33.000000 lazyinit-0.0.28/.git/FETCH_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.28/.git/ORIG_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.28/.git/config
+-rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/description
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.723903 lazyinit-0.0.28/.git/hooks/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/post-update.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/hooks/update.sample
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4305 2023-07-26 15:01:28.000000 lazyinit-0.0.28/.git/index
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.724086 lazyinit-0.0.28/.git/info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/info/exclude
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.724233 lazyinit-0.0.28/.git/logs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.28/.git/logs/HEAD
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.706020 lazyinit-0.0.28/.git/logs/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.724432 lazyinit-0.0.28/.git/logs/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.28/.git/logs/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.706073 lazyinit-0.0.28/.git/logs/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.724895 lazyinit-0.0.28/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6437 2023-07-28 14:15:58.000000 lazyinit-0.0.28/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1953 2023-07-28 04:10:06.000000 lazyinit-0.0.28/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.714111 lazyinit-0.0.28/.git/objects/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.725091 lazyinit-0.0.28/.git/objects/00/
+-r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.725396 lazyinit-0.0.28/.git/objects/01/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.725873 lazyinit-0.0.28/.git/objects/04/
+-r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
+-r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.726258 lazyinit-0.0.28/.git/objects/05/
+-r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
+-r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.726956 lazyinit-0.0.28/.git/objects/0a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.727745 lazyinit-0.0.28/.git/objects/0e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
+-r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.728011 lazyinit-0.0.28/.git/objects/11/
+-r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.728203 lazyinit-0.0.28/.git/objects/14/
+-r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.728357 lazyinit-0.0.28/.git/objects/1c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.28/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.728627 lazyinit-0.0.28/.git/objects/1f/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.729158 lazyinit-0.0.28/.git/objects/22/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.28/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
+-r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.729351 lazyinit-0.0.28/.git/objects/24/
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.729628 lazyinit-0.0.28/.git/objects/28/
+-r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.729900 lazyinit-0.0.28/.git/objects/2a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.730171 lazyinit-0.0.28/.git/objects/2b/
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.730444 lazyinit-0.0.28/.git/objects/2d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.730643 lazyinit-0.0.28/.git/objects/2e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.731097 lazyinit-0.0.28/.git/objects/32/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
+-r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.731375 lazyinit-0.0.28/.git/objects/33/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.28/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.731646 lazyinit-0.0.28/.git/objects/38/
+-r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.732323 lazyinit-0.0.28/.git/objects/39/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.28/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.732798 lazyinit-0.0.28/.git/objects/3d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
+-r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.733037 lazyinit-0.0.28/.git/objects/40/
+-r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.28/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.733408 lazyinit-0.0.28/.git/objects/41/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.733742 lazyinit-0.0.28/.git/objects/43/
+-r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.734147 lazyinit-0.0.28/.git/objects/4d/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.734342 lazyinit-0.0.28/.git/objects/52/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.28/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.734561 lazyinit-0.0.28/.git/objects/55/
+-r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.734930 lazyinit-0.0.28/.git/objects/56/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.735173 lazyinit-0.0.28/.git/objects/5a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.735540 lazyinit-0.0.28/.git/objects/5e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.735960 lazyinit-0.0.28/.git/objects/5f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
+-r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.736393 lazyinit-0.0.28/.git/objects/60/
+-r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.737075 lazyinit-0.0.28/.git/objects/63/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
+-r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.737303 lazyinit-0.0.28/.git/objects/64/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.737577 lazyinit-0.0.28/.git/objects/67/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.737776 lazyinit-0.0.28/.git/objects/69/
+-r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.738024 lazyinit-0.0.28/.git/objects/6a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.738307 lazyinit-0.0.28/.git/objects/6b/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.738783 lazyinit-0.0.28/.git/objects/6c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
+-r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.738997 lazyinit-0.0.28/.git/objects/6d/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.739267 lazyinit-0.0.28/.git/objects/6e/
+-r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.739658 lazyinit-0.0.28/.git/objects/6f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.739935 lazyinit-0.0.28/.git/objects/73/
+-r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.740747 lazyinit-0.0.28/.git/objects/74/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
+-r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.740981 lazyinit-0.0.28/.git/objects/7e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.741248 lazyinit-0.0.28/.git/objects/7f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.741483 lazyinit-0.0.28/.git/objects/80/
+-r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.741859 lazyinit-0.0.28/.git/objects/83/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.28/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
+-r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.742131 lazyinit-0.0.28/.git/objects/84/
+-r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.742395 lazyinit-0.0.28/.git/objects/86/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.28/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.742600 lazyinit-0.0.28/.git/objects/87/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.28/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.742735 lazyinit-0.0.28/.git/objects/88/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.742900 lazyinit-0.0.28/.git/objects/89/
+-r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.743087 lazyinit-0.0.28/.git/objects/8b/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.28/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.743226 lazyinit-0.0.28/.git/objects/8f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/8f/821694556aac2a278c288de223659193dd2489
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.743401 lazyinit-0.0.28/.git/objects/91/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.743751 lazyinit-0.0.28/.git/objects/96/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.743954 lazyinit-0.0.28/.git/objects/99/
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.744396 lazyinit-0.0.28/.git/objects/9c/
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.744778 lazyinit-0.0.28/.git/objects/9d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
+-r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.745525 lazyinit-0.0.28/.git/objects/a0/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
+-r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
+-r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.746030 lazyinit-0.0.28/.git/objects/a1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
+-r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.746311 lazyinit-0.0.28/.git/objects/a3/
+-r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.746806 lazyinit-0.0.28/.git/objects/a8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.747509 lazyinit-0.0.28/.git/objects/a9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-28 04:10:06.000000 lazyinit-0.0.28/.git/objects/a9/7852c14503686493d3218632fbbb52dd42628b
+-r--r--r--   0 dengyifan   (501) staff       (20)      557 2023-07-28 04:10:06.000000 lazyinit-0.0.28/.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4
+-r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.748222 lazyinit-0.0.28/.git/objects/aa/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
+-r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
+-r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.748494 lazyinit-0.0.28/.git/objects/ad/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.749008 lazyinit-0.0.28/.git/objects/ae/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
+-r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.749856 lazyinit-0.0.28/.git/objects/af/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
+-r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.750568 lazyinit-0.0.28/.git/objects/b0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.28/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.750865 lazyinit-0.0.28/.git/objects/b1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.751104 lazyinit-0.0.28/.git/objects/b4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.754063 lazyinit-0.0.28/.git/objects/b6/
+-r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
+-r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.754325 lazyinit-0.0.28/.git/objects/b7/
+-r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.28/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.754518 lazyinit-0.0.28/.git/objects/bb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.755580 lazyinit-0.0.28/.git/objects/bc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
+-r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.28/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
+-r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.756260 lazyinit-0.0.28/.git/objects/c1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.756756 lazyinit-0.0.28/.git/objects/c4/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.28/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.757304 lazyinit-0.0.28/.git/objects/c5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
+-r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.757493 lazyinit-0.0.28/.git/objects/c7/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.757884 lazyinit-0.0.28/.git/objects/c9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.758055 lazyinit-0.0.28/.git/objects/ca/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.759065 lazyinit-0.0.28/.git/objects/cc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
+-r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.759644 lazyinit-0.0.28/.git/objects/cd/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.28/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.759802 lazyinit-0.0.28/.git/objects/ce/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.759976 lazyinit-0.0.28/.git/objects/d2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      163 2023-07-28 04:10:06.000000 lazyinit-0.0.28/.git/objects/d2/99be9b16073ba179c8b1558984116cd0eb9f3b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.760269 lazyinit-0.0.28/.git/objects/d9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.760552 lazyinit-0.0.28/.git/objects/da/
+-r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.760983 lazyinit-0.0.28/.git/objects/de/
+-r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.762072 lazyinit-0.0.28/.git/objects/df/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.762326 lazyinit-0.0.28/.git/objects/e4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.28/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.762611 lazyinit-0.0.28/.git/objects/e6/
+-r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.763009 lazyinit-0.0.28/.git/objects/e8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
+-r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.763462 lazyinit-0.0.28/.git/objects/eb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
+-r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.763803 lazyinit-0.0.28/.git/objects/ec/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.764417 lazyinit-0.0.28/.git/objects/ef/
+-r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.764926 lazyinit-0.0.28/.git/objects/f0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
+-r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.28/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.765130 lazyinit-0.0.28/.git/objects/f1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-26 04:07:28.000000 lazyinit-0.0.28/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.765564 lazyinit-0.0.28/.git/objects/f2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.765888 lazyinit-0.0.28/.git/objects/f5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.28/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.766097 lazyinit-0.0.28/.git/objects/f6/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.28/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.714348 lazyinit-0.0.28/.git/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.766295 lazyinit-0.0.28/.git/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.28/.git/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.714406 lazyinit-0.0.28/.git/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.771381 lazyinit-0.0.28/.git/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-28 14:15:58.000000 lazyinit-0.0.28/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-28 04:10:06.000000 lazyinit-0.0.28/.git/refs/remotes/origin/master
+-rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.28/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      379 2023-07-29 00:33:34.781364 lazyinit-0.0.28/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.28/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.774130 lazyinit-0.0.28/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.28/lazyinit/__init__.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.775353 lazyinit-0.0.28/lazyinit/__pycache__/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      179 2023-07-27 12:30:23.000000 lazyinit-0.0.28/lazyinit/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)    10748 2023-07-27 12:30:23.000000 lazyinit-0.0.28/lazyinit/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.28/lazyinit/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.28/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8549 2023-07-29 00:29:14.000000 lazyinit-0.0.28/lazyinit/init.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.776356 lazyinit-0.0.28/lazyinit/lazydl/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.28/lazyinit/lazydl/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.776788 lazyinit-0.0.28/lazyinit/lazydl/configs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1375 2023-07-29 00:33:21.000000 lazyinit-0.0.28/lazyinit/lazydl/configs/default_config.yaml
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.717614 lazyinit-0.0.28/lazyinit/lazydl/configs/exps/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.777136 lazyinit-0.0.28/lazyinit/lazydl/configs/exps/exp1/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.28/lazyinit/lazydl/configs/exps/exp1/baseline.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1152 2023-07-29 00:31:59.000000 lazyinit-0.0.28/lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.28/lazyinit/lazydl/minist.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.28/lazyinit/lazydl/requirements.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.28/lazyinit/lazydl/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.28/lazyinit/lazydl/start.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.778095 lazyinit-0.0.28/lazyinit/ranger/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.28/lazyinit/ranger/.DS_Store
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.779001 lazyinit-0.0.28/lazyinit/ranger/colorschemes/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/default.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/jungle.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/snow.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/snow.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/colorschemes/zenburn.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/commands.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.781066 lazyinit-0.0.28/lazyinit/ranger/plugins/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/devicons.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/devicons.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/devicons_linemode.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/plugins/devicons_linemode.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/rc-sample.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/rc.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/rifle.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.28/lazyinit/ranger/scope.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.28/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.28/lazyinit/redis.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-29 00:29:59.000000 lazyinit-0.0.28/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6724 2023-07-27 11:48:11.000000 lazyinit-0.0.28/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-29 00:33:34.774959 lazyinit-0.0.28/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      379 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)    10230 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-29 00:33:34.000000 lazyinit-0.0.28/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.28/push.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-29 00:33:34.781659 lazyinit-0.0.28/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      844 2023-07-29 00:33:26.000000 lazyinit-0.0.28/setup.py
```

### Comparing `lazyinit-0.0.27/.git/hooks/commit-msg.sample` & `lazyinit-0.0.28/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/fsmonitor-watchman.sample` & `lazyinit-0.0.28/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/pre-commit.sample` & `lazyinit-0.0.28/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/pre-push.sample` & `lazyinit-0.0.28/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/pre-rebase.sample` & `lazyinit-0.0.28/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/pre-receive.sample` & `lazyinit-0.0.28/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/prepare-commit-msg.sample` & `lazyinit-0.0.28/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/push-to-checkout.sample` & `lazyinit-0.0.28/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/hooks/update.sample` & `lazyinit-0.0.28/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/index` & `lazyinit-0.0.28/.git/index`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/logs/HEAD` & `lazyinit-0.0.28/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/logs/refs/heads/master` & `lazyinit-0.0.28/.git/logs/refs/heads/master`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/logs/refs/remotes/origin/master` & `lazyinit-0.0.28/.git/logs/refs/remotes/origin/master`

 * *Files 9% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 0041c04b20be6b4bbd75a815bebf7084805f8712 bce5df5b3fb9303de75d9ba662475c2e0940387e {553192215@qq.com} <553192215@qq.com> 1690285280 +0800	update by push
 bce5df5b3fb9303de75d9ba662475c2e0940387e e4632035cac16d026cc02de90ae31aef87867116 {553192215@qq.com} <553192215@qq.com> 1690293654 +0800	update by push
 e4632035cac16d026cc02de90ae31aef87867116 5f9cbd2428e9c98934938c6677d49d4c9563df8d {553192215@qq.com} <553192215@qq.com> 1690342595 +0800	fetch --progress --prune --recurse-submodules=on-demand origin: fast-forward
 5f9cbd2428e9c98934938c6677d49d4c9563df8d 9d1f61df1650e8ae0165c5d3e1f47e8384a76e25 {553192215@qq.com} <553192215@qq.com> 1690344452 +0800	update by push
 9d1f61df1650e8ae0165c5d3e1f47e8384a76e25 3d5d200d32889f9867e73ddd61f8de5d54006cca {553192215@qq.com} <553192215@qq.com> 1690347612 +0800	update by push
 3d5d200d32889f9867e73ddd61f8de5d54006cca 142068ef3450523a0e5f073bd62eec3746405639 {553192215@qq.com} <553192215@qq.com> 1690354475 +0800	update by push
 142068ef3450523a0e5f073bd62eec3746405639 875e7c9d32e4d678ba2fbacb46a4a3de3402a717 {553192215@qq.com} <553192215@qq.com> 1690359383 +0800	fetch: fast-forward
+875e7c9d32e4d678ba2fbacb46a4a3de3402a717 a995569e1ac0accec5b1acc68f0ab077023bc4f4 {553192215@qq.com} <553192215@qq.com> 1690517406 +0800	fetch --progress --prune --recurse-submodules=on-demand origin: fast-forward
```

### Comparing `lazyinit-0.0.27/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063` & `lazyinit-0.0.28/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9` & `lazyinit-0.0.28/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6` & `lazyinit-0.0.28/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead` & `lazyinit-0.0.28/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d` & `lazyinit-0.0.28/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae` & `lazyinit-0.0.28/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8` & `lazyinit-0.0.28/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34` & `lazyinit-0.0.28/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d` & `lazyinit-0.0.28/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3` & `lazyinit-0.0.28/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7` & `lazyinit-0.0.28/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3` & `lazyinit-0.0.28/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9` & `lazyinit-0.0.28/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd` & `lazyinit-0.0.28/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd` & `lazyinit-0.0.28/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb` & `lazyinit-0.0.28/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d` & `lazyinit-0.0.28/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1` & `lazyinit-0.0.28/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b` & `lazyinit-0.0.28/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f` & `lazyinit-0.0.28/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084` & `lazyinit-0.0.28/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4` & `lazyinit-0.0.28/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04` & `lazyinit-0.0.28/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66` & `lazyinit-0.0.28/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86` & `lazyinit-0.0.28/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25` & `lazyinit-0.0.28/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717` & `lazyinit-0.0.28/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c` & `lazyinit-0.0.28/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c` & `lazyinit-0.0.28/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0` & `lazyinit-0.0.28/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef` & `lazyinit-0.0.28/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e` & `lazyinit-0.0.28/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd` & `lazyinit-0.0.28/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083` & `lazyinit-0.0.28/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d` & `lazyinit-0.0.28/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875` & `lazyinit-0.0.28/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b` & `lazyinit-0.0.28/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487` & `lazyinit-0.0.28/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477` & `lazyinit-0.0.28/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb` & `lazyinit-0.0.28/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76` & `lazyinit-0.0.28/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45` & `lazyinit-0.0.28/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c` & `lazyinit-0.0.28/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01` & `lazyinit-0.0.28/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385` & `lazyinit-0.0.28/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893` & `lazyinit-0.0.28/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586` & `lazyinit-0.0.28/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd` & `lazyinit-0.0.28/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d` & `lazyinit-0.0.28/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c` & `lazyinit-0.0.28/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591` & `lazyinit-0.0.28/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943` & `lazyinit-0.0.28/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac` & `lazyinit-0.0.28/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463` & `lazyinit-0.0.28/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b` & `lazyinit-0.0.28/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e` & `lazyinit-0.0.28/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23` & `lazyinit-0.0.28/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c` & `lazyinit-0.0.28/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb` & `lazyinit-0.0.28/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91` & `lazyinit-0.0.28/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-311.pyc` & `lazyinit-0.0.28/lazyinit/__pycache__/utils.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xc994c064 (Wed Jul 26 03:36:41 2023 UTC)
-files sz: 4862
+moddate:  0x7b59c264 (Thu Jul 27 11:48:11 2023 UTC)
+files sz: 6724
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a03640064026c045a
-      04640064026c055a05640064036c066d075a07010002006507a6000000ab
-      0000000000000000005a08640484005a09640b640684015a0a640784005a
-      0b640c640a84015a0c64025300
+      04640064026c055a05640064036c066d075a070100640064026c085a0864
+      0064046c096d0a5a0a010002006507a6000000ab0000000000000000005a
+      0b640584005a0c640e640784015a0d640884005a0e640f640a84015a0f64
+      10640d84015a1064025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('BeautifulSoup',))
                  6 IMPORT_NAME              0 (bs4)
                  8 IMPORT_FROM              1 (BeautifulSoup)
                 10 STORE_NAME               1 (BeautifulSoup)
@@ -38,80 +39,98 @@
      5          38 LOAD_CONST               0 (0)
                 40 LOAD_CONST               3 (('Console',))
                 42 IMPORT_NAME              6 (rich.console)
                 44 IMPORT_FROM              7 (Console)
                 46 STORE_NAME               7 (Console)
                 48 POP_TOP
    
-     7          50 PUSH_NULL
-                52 LOAD_NAME                7 (Console)
-                54 PRECALL                  0
-                58 CALL                     0
-                68 STORE_NAME               8 (console)
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               2 (None)
+                54 IMPORT_NAME              8 (subprocess)
+                56 STORE_NAME               8 (subprocess)
    
-     9          70 LOAD_CONST               4 (<code object package_installed, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 9>)
-                72 MAKE_FUNCTION            0
-                74 STORE_NAME               9 (package_installed)
+     7          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               4 (('track',))
+                62 IMPORT_NAME              9 (rich.progress)
+                64 IMPORT_FROM             10 (track)
+                66 STORE_NAME              10 (track)
+                68 POP_TOP
    
-    20          76 LOAD_CONST              11 (('green',))
-                78 LOAD_CONST               6 (<code object echo, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 20>)
-                80 MAKE_FUNCTION            1 (defaults)
-                82 STORE_NAME              10 (echo)
+     9          70 PUSH_NULL
+                72 LOAD_NAME                7 (Console)
+                74 PRECALL                  0
+                78 CALL                     0
+                88 STORE_NAME              11 (console)
    
-    23          84 LOAD_CONST               7 (<code object run_cmd, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 23>)
-                86 MAKE_FUNCTION            0
-                88 STORE_NAME              11 (run_cmd)
+    11          90 LOAD_CONST               5 (<code object package_installed, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 11>)
+                92 MAKE_FUNCTION            0
+                94 STORE_NAME              12 (package_installed)
    
-    45          90 LOAD_CONST              12 (('11.8', '3.9'))
-                92 LOAD_CONST              10 (<code object show_available_version, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 45>)
-                94 MAKE_FUNCTION            1 (defaults)
-                96 STORE_NAME              12 (show_available_version)
-                98 LOAD_CONST               2 (None)
-               100 RETURN_VALUE
+    22          96 LOAD_CONST              14 (('green',))
+                98 LOAD_CONST               7 (<code object echo, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 22>)
+               100 MAKE_FUNCTION            1 (defaults)
+               102 STORE_NAME              13 (echo)
+   
+    26         104 LOAD_CONST               8 (<code object run_cmd_inactivate, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 26>)
+               106 MAKE_FUNCTION            0
+               108 STORE_NAME              14 (run_cmd_inactivate)
+   
+    58         110 LOAD_CONST              15 ((True,))
+               112 LOAD_CONST              10 (<code object run_cmd, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 58>)
+               114 MAKE_FUNCTION            1 (defaults)
+               116 STORE_NAME              15 (run_cmd)
+   
+    97         118 LOAD_CONST              16 (('11.8', '3.9'))
+               120 LOAD_CONST              13 (<code object show_available_version, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 97>)
+               122 MAKE_FUNCTION            1 (defaults)
+               124 STORE_NAME              16 (show_available_version)
+               126 LOAD_CONST               2 (None)
+               128 RETURN_VALUE
    consts
       0
       ('BeautifulSoup',)
       None
       ('Console',)
+      ('track',)
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970009007401000000000000000000006a0100000000000000007c00a6
             010000ab0100000000000000000100640153002300740000000000000000
             0000006a0200000000000000002400720401005900640253007700780359
             007701
-           9           0 RESUME                   0
+          11           0 RESUME                   0
          
-          13           2 NOP
+          15           2 NOP
          
-          14           4 LOAD_GLOBAL              1 (NULL + pkg_resources)
+          16           4 LOAD_GLOBAL              1 (NULL + pkg_resources)
                       16 LOAD_ATTR                1 (get_distribution)
                       26 LOAD_FAST                0 (package_name)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 POP_TOP
          
-          18          44 LOAD_CONST               1 (True)
+          20          44 LOAD_CONST               1 (True)
                       46 RETURN_VALUE
                  >>   48 PUSH_EXC_INFO
          
-          15          50 LOAD_GLOBAL              0 (pkg_resources)
+          17          50 LOAD_GLOBAL              0 (pkg_resources)
                       62 LOAD_ATTR                2 (DistributionNotFound)
                       72 CHECK_EXC_MATCH
                       74 POP_JUMP_FORWARD_IF_FALSE     4 (to 84)
                       76 POP_TOP
          
-          16          78 POP_EXCEPT
+          18          78 POP_EXCEPT
                       80 LOAD_CONST               2 (False)
                       82 RETURN_VALUE
          
-          15     >>   84 RERAISE                  0
+          17     >>   84 RERAISE                  0
                  >>   86 COPY                     3
                       88 POP_EXCEPT
                       90 RERAISE                  1
          ExceptionTable:
            4 to 42 -> 48 [0]
            48 to 76 -> 86 [1] lasti
            84 to 84 -> 86 [1] lasti
@@ -121,29 +140,29 @@
             False
          names      ('pkg_resources', 'get_distribution', 'DistributionNotFound')
          varnames   ('package_name',)
          freevars   ()
          cellvars   ()
          filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
          name       'package_installed'
-         firstlineno 9
+         firstlineno 11
          lnotab 0x02040201280406fd1c0106ff
       'green'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             000000000000007c007c01ac01a6020000ab020000000000000000010064
             005300
-          20           0 RESUME                   0
+          22           0 RESUME                   0
          
-          21           2 LOAD_GLOBAL              0 (console)
+          23           2 LOAD_GLOBAL              0 (console)
                       14 LOAD_METHOD              1 (print)
                       36 LOAD_FAST                0 (msg)
                       38 LOAD_FAST                1 (color)
                       40 KW_NAMES                 1
                       42 PRECALL                  2
                       46 CALL                     2
                       56 POP_TOP
@@ -154,142 +173,455 @@
             ('style',)
          names      ('console', 'print')
          varnames   ('msg', 'color')
          freevars   ()
          cellvars   ()
          filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
          name       'echo'
-         firstlineno 20
+         firstlineno 22
          lnotab 0x0201
       code
          argcount  : 1
-         nlocals   : 5
+         nlocals   : 4
+         stacksize : 6
+         flags     : 3
+         code
+            0x97007401000000000000000000007c00740200000000000000000000a6
+            020000ab020000000000000000727b7c007d017405000000000000000000
+            0064017c017a000000a6010000ab01000000000000000001000900740700
+            0000000000000000006a0400000000000000007c01a6010000ab01000000
+            00000000007d027c0264036b03000000007249740b000000000000000000
+            006404a00600000000000000000000000000000000000000007c01a60100
+            00ab0100000000000000006405a6020000ab020000000000000000010074
+            0b000000000000000000006406a6010000ab010000000000000000010074
+            0f00000000000000000000a6000000ab0000000000000000007d017c0164
+            076b020000000072027c0253006e027c0253008c6667007d037411000000
+            000000000000007c0064086402ac09a6030000ab03000000000000000044
+            005d797d0174050000000000000000000064017c017a000000a6010000ab
+            010000000000000000010009007407000000000000000000006a04000000
+            00000000007c01a6010000ab0100000000000000007d027c0264036b0300
+            0000007248740b000000000000000000006404a006000000000000000000
+            00000000000000000000007c01a6010000ab0100000000000000006405a6
+            020000ab0200000000000000000100740b000000000000000000006406a6
+            010000ab0100000000000000000100740f00000000000000000000a60000
+            00ab0000000000000000007d017c0164076b020000000072016e036e016e
+            018c648c7a7c035300
+          26           0 RESUME                   0
+         
+          27           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                      14 LOAD_FAST                0 (cmd_list)
+                      16 LOAD_GLOBAL              2 (str)
+                      28 PRECALL                  2
+                      32 CALL                     2
+                      42 POP_JUMP_FORWARD_IF_FALSE   123 (to 290)
+         
+          28          44 LOAD_FAST                0 (cmd_list)
+                      46 STORE_FAST               1 (cmd)
+         
+          29          48 LOAD_GLOBAL              5 (NULL + print)
+                      60 LOAD_CONST               1 ('\n')
+                      62 LOAD_FAST                1 (cmd)
+                      64 BINARY_OP                0 (+)
+                      68 PRECALL                  1
+                      72 CALL                     1
+                      82 POP_TOP
+         
+          30          84 NOP
+         
+          31     >>   86 LOAD_GLOBAL              7 (NULL + os)
+                      98 LOAD_ATTR                4 (system)
+                     108 LOAD_FAST                1 (cmd)
+                     110 PRECALL                  1
+                     114 CALL                     1
+                     124 STORE_FAST               2 (exitcode)
+         
+          32         126 LOAD_FAST                2 (exitcode)
+                     128 LOAD_CONST               3 (0)
+                     130 COMPARE_OP               3 (!=)
+                     136 POP_JUMP_FORWARD_IF_FALSE    73 (to 284)
+         
+          33         138 LOAD_GLOBAL             11 (NULL + echo)
+                     150 LOAD_CONST               4 ('执行 {} 失败！')
+                     152 LOAD_METHOD              6 (format)
+                     174 LOAD_FAST                1 (cmd)
+                     176 PRECALL                  1
+                     180 CALL                     1
+                     190 LOAD_CONST               5 ('#FF6AB3')
+                     192 PRECALL                  2
+                     196 CALL                     2
+                     206 POP_TOP
+         
+          34         208 LOAD_GLOBAL             11 (NULL + echo)
+                     220 LOAD_CONST               6 ('可通过在下方修改命令继续执行，或者直接按下回车键结束操作：')
+                     222 PRECALL                  1
+                     226 CALL                     1
+                     236 POP_TOP
+         
+          35         238 LOAD_GLOBAL             15 (NULL + input)
+                     250 PRECALL                  0
+                     254 CALL                     0
+                     264 STORE_FAST               1 (cmd)
+         
+          36         266 LOAD_FAST                1 (cmd)
+                     268 LOAD_CONST               7 ('')
+                     270 COMPARE_OP               2 (==)
+                     276 POP_JUMP_FORWARD_IF_FALSE     2 (to 282)
+         
+          37         278 LOAD_FAST                2 (exitcode)
+                     280 RETURN_VALUE
+         
+          36     >>  282 JUMP_FORWARD             2 (to 288)
+         
+          39     >>  284 LOAD_FAST                2 (exitcode)
+                     286 RETURN_VALUE
+         
+          30     >>  288 JUMP_BACKWARD          102 (to 86)
+         
+          41     >>  290 BUILD_LIST               0
+                     292 STORE_FAST               3 (outputs)
+         
+          42         294 LOAD_GLOBAL             17 (NULL + track)
+                     306 LOAD_FAST                0 (cmd_list)
+                     308 LOAD_CONST               8 ('命令执行中')
+                     310 LOAD_CONST               2 (True)
+                     312 KW_NAMES                 9
+                     314 PRECALL                  3
+                     318 CALL                     3
+                     328 GET_ITER
+                 >>  330 FOR_ITER               121 (to 574)
+                     332 STORE_FAST               1 (cmd)
+         
+          43         334 LOAD_GLOBAL              5 (NULL + print)
+                     346 LOAD_CONST               1 ('\n')
+                     348 LOAD_FAST                1 (cmd)
+                     350 BINARY_OP                0 (+)
+                     354 PRECALL                  1
+                     358 CALL                     1
+                     368 POP_TOP
+         
+          44         370 NOP
+         
+          45     >>  372 LOAD_GLOBAL              7 (NULL + os)
+                     384 LOAD_ATTR                4 (system)
+                     394 LOAD_FAST                1 (cmd)
+                     396 PRECALL                  1
+                     400 CALL                     1
+                     410 STORE_FAST               2 (exitcode)
+         
+          46         412 LOAD_FAST                2 (exitcode)
+                     414 LOAD_CONST               3 (0)
+                     416 COMPARE_OP               3 (!=)
+                     422 POP_JUMP_FORWARD_IF_FALSE    72 (to 568)
+         
+          47         424 LOAD_GLOBAL             11 (NULL + echo)
+                     436 LOAD_CONST               4 ('执行 {} 失败！')
+                     438 LOAD_METHOD              6 (format)
+                     460 LOAD_FAST                1 (cmd)
+                     462 PRECALL                  1
+                     466 CALL                     1
+                     476 LOAD_CONST               5 ('#FF6AB3')
+                     478 PRECALL                  2
+                     482 CALL                     2
+                     492 POP_TOP
+         
+          48         494 LOAD_GLOBAL             11 (NULL + echo)
+                     506 LOAD_CONST               6 ('可通过在下方修改命令继续执行，或者直接按下回车键结束操作：')
+                     508 PRECALL                  1
+                     512 CALL                     1
+                     522 POP_TOP
+         
+          49         524 LOAD_GLOBAL             15 (NULL + input)
+                     536 PRECALL                  0
+                     540 CALL                     0
+                     550 STORE_FAST               1 (cmd)
+         
+          50         552 LOAD_FAST                1 (cmd)
+                     554 LOAD_CONST               7 ('')
+                     556 COMPARE_OP               2 (==)
+                     562 POP_JUMP_FORWARD_IF_FALSE     1 (to 566)
+         
+          51         564 JUMP_FORWARD             3 (to 572)
+         
+          50     >>  566 JUMP_FORWARD             1 (to 570)
+         
+          53     >>  568 JUMP_FORWARD             1 (to 572)
+         
+          44     >>  570 JUMP_BACKWARD          100 (to 372)
+                 >>  572 JUMP_BACKWARD          122 (to 330)
+         
+          55     >>  574 LOAD_FAST                3 (outputs)
+                     576 RETURN_VALUE
+         consts
+            None
+            '\n'
+            True
+            0
+            '执行 {} 失败！'
+            '#FF6AB3'
+            '可通过在下方修改命令继续执行，或者直接按下回车键结束操作：'
+            ''
+            '命令执行中'
+            ('description', 'transient')
+         names      ('isinstance', 'str', 'print', 'os', 'system', 'echo', 'format', 'input', 'track')
+         varnames   ('cmd_list', 'cmd', 'exitcode', 'outputs')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
+         name       'run_cmd_inactivate'
+         firstlineno 26
+         lnotab
+            0x02012a0104012401020128010c0146011e011c010c0104ff020304f702
+            0b040128012401020128010c0146011e011c010c0102ff020302f7040b
+      True
+      code
+         argcount  : 2
+         nlocals   : 6
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00740200000000000000000000a6
-            020000ab02000000000000000073037c0067017d0067007d017c0044005d
-            9a7d020900740400000000000000000000a0030000000000000000000000
-            0000000000000000007c02a6010000ab0100000000000000005c0200007d
-            037d047c0364026b0300000000725d7409000000000000000000006403a0
-            0500000000000000000000000000000000000000007c02a6010000ab0100
-            000000000000006404a6020000ab02000000000000000001007409000000
-            000000000000006405a6010000ab0100000000000000000100740d000000
-            00000000000000a6000000ab0000000000000000007d027c0264066b0200
-            00000072167c01a00700000000000000000000000000000000000000007c
-            04a6010000ab01000000000000000001006e186e167c01a0070000000000
+            020000ab02000000000000000072a27c007d027c01721274050000000000
+            000000000064017c027a000000a6010000ab010000000000000000010009
+            007407000000000000000000006a0400000000000000007c02a6010000ab
+            0100000000000000005c0200007d037d047c0364036b0300000000726b74
+            0b000000000000000000006404a006000000000000000000000000000000
+            00000000007c02a6010000ab0100000000000000006405a6020000ab0200
+            000000000000000100740b000000000000000000006406a0060000000000
             0000000000000000000000000000007c04a6010000ab0100000000000000
-            0001006e018c978c9b7c015300
-          23           0 RESUME                   0
+            00a6010000ab0100000000000000000100740b0000000000000000000064
+            07a6010000ab0100000000000000000100740f00000000000000000000a6
+            000000ab0000000000000000007d027c0264086b020000000072027c0453
+            006e027c0453008c8b67007d057411000000000000000000007c00640964
+            02ac0aa6030000ab03000000000000000044005dca7d027c017212740500
+            00000000000000000064017c027a000000a6010000ab0100000000000000
+            00010009007407000000000000000000006a0400000000000000007c02a6
+            010000ab0100000000000000005c0200007d037d047c0364036b03000000
+            00727f740b000000000000000000006404a0060000000000000000000000
+            0000000000000000007c02a6010000ab0100000000000000006405a60200
+            00ab0200000000000000000100740b000000000000000000006406a00600
+            000000000000000000000000000000000000007c04a6010000ab01000000
+            0000000000a6010000ab0100000000000000000100740b00000000000000
+            0000006407a6010000ab0100000000000000000100740f00000000000000
+            000000a6000000ab0000000000000000007d027c0264086b020000000072
+            167c05a00900000000000000000000000000000000000000007c04a60100
+            00ab01000000000000000001006e186e167c05a009000000000000000000
+            00000000000000000000007c04a6010000ab01000000000000000001006e
+            018cb38ccb7c055300
+          58           0 RESUME                   0
          
-          24           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          59           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (cmd_list)
-                      16 LOAD_GLOBAL              2 (list)
+                      16 LOAD_GLOBAL              2 (str)
                       28 PRECALL                  2
                       32 CALL                     2
-                      42 POP_JUMP_FORWARD_IF_TRUE     3 (to 50)
+                      42 POP_JUMP_FORWARD_IF_FALSE   162 (to 368)
+         
+          60          44 LOAD_FAST                0 (cmd_list)
+                      46 STORE_FAST               2 (cmd)
          
-          25          44 LOAD_FAST                0 (cmd_list)
-                      46 BUILD_LIST               1
-                      48 STORE_FAST               0 (cmd_list)
-         
-          26     >>   50 BUILD_LIST               0
-                      52 STORE_FAST               1 (outputs)
-         
-          27          54 LOAD_FAST                0 (cmd_list)
-                      56 GET_ITER
-                 >>   58 FOR_ITER               154 (to 368)
-                      60 STORE_FAST               2 (cmd)
-         
-          28          62 NOP
-         
-          29     >>   64 LOAD_GLOBAL              4 (subprocess)
-                      76 LOAD_METHOD              3 (getstatusoutput)
-                      98 LOAD_FAST                2 (cmd)
-                     100 PRECALL                  1
-                     104 CALL                     1
-                     114 UNPACK_SEQUENCE          2
-                     118 STORE_FAST               3 (exitcode)
-                     120 STORE_FAST               4 (output)
-         
-          30         122 LOAD_FAST                3 (exitcode)
-                     124 LOAD_CONST               2 (0)
-                     126 COMPARE_OP               3 (!=)
-                     132 POP_JUMP_FORWARD_IF_FALSE    93 (to 320)
-         
-          31         134 LOAD_GLOBAL              9 (NULL + echo)
-                     146 LOAD_CONST               3 ('执行 {} 失败！')
-                     148 LOAD_METHOD              5 (format)
-                     170 LOAD_FAST                2 (cmd)
-                     172 PRECALL                  1
-                     176 CALL                     1
-                     186 LOAD_CONST               4 ('#FF6AB3')
-                     188 PRECALL                  2
-                     192 CALL                     2
-                     202 POP_TOP
-         
-          32         204 LOAD_GLOBAL              9 (NULL + echo)
-                     216 LOAD_CONST               5 ('可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：')
-                     218 PRECALL                  1
-                     222 CALL                     1
-                     232 POP_TOP
-         
-          33         234 LOAD_GLOBAL             13 (NULL + input)
-                     246 PRECALL                  0
-                     250 CALL                     0
-                     260 STORE_FAST               2 (cmd)
-         
-          34         262 LOAD_FAST                2 (cmd)
-                     264 LOAD_CONST               6 ('')
-                     266 COMPARE_OP               2 (==)
-                     272 POP_JUMP_FORWARD_IF_FALSE    22 (to 318)
-         
-          35         274 LOAD_FAST                1 (outputs)
-                     276 LOAD_METHOD              7 (append)
-                     298 LOAD_FAST                4 (output)
+          61          48 LOAD_FAST                1 (show_cmd)
+                      50 POP_JUMP_FORWARD_IF_FALSE    18 (to 88)
+         
+          62          52 LOAD_GLOBAL              5 (NULL + print)
+                      64 LOAD_CONST               1 ('\n')
+                      66 LOAD_FAST                2 (cmd)
+                      68 BINARY_OP                0 (+)
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 POP_TOP
+         
+          63     >>   88 NOP
+         
+          64     >>   90 LOAD_GLOBAL              7 (NULL + subprocess)
+                     102 LOAD_ATTR                4 (getstatusoutput)
+                     112 LOAD_FAST                2 (cmd)
+                     114 PRECALL                  1
+                     118 CALL                     1
+                     128 UNPACK_SEQUENCE          2
+                     132 STORE_FAST               3 (exitcode)
+                     134 STORE_FAST               4 (output)
+         
+          65         136 LOAD_FAST                3 (exitcode)
+                     138 LOAD_CONST               3 (0)
+                     140 COMPARE_OP               3 (!=)
+                     146 POP_JUMP_FORWARD_IF_FALSE   107 (to 362)
+         
+          66         148 LOAD_GLOBAL             11 (NULL + echo)
+                     160 LOAD_CONST               4 ('执行 {} 失败！')
+                     162 LOAD_METHOD              6 (format)
+                     184 LOAD_FAST                2 (cmd)
+                     186 PRECALL                  1
+                     190 CALL                     1
+                     200 LOAD_CONST               5 ('#FF6AB3')
+                     202 PRECALL                  2
+                     206 CALL                     2
+                     216 POP_TOP
+         
+          67         218 LOAD_GLOBAL             11 (NULL + echo)
+                     230 LOAD_CONST               6 ('错误信息：\n{}')
+                     232 LOAD_METHOD              6 (format)
+                     254 LOAD_FAST                4 (output)
+                     256 PRECALL                  1
+                     260 CALL                     1
+                     270 PRECALL                  1
+                     274 CALL                     1
+                     284 POP_TOP
+         
+          68         286 LOAD_GLOBAL             11 (NULL + echo)
+                     298 LOAD_CONST               7 ('可通过在下方修改命令继续执行，或者直接按下回车键结束操作：')
                      300 PRECALL                  1
                      304 CALL                     1
                      314 POP_TOP
          
-          36         316 JUMP_FORWARD            24 (to 366)
-         
-          34     >>  318 JUMP_FORWARD            22 (to 364)
-         
-          38     >>  320 LOAD_FAST                1 (outputs)
-                     322 LOAD_METHOD              7 (append)
-                     344 LOAD_FAST                4 (output)
-                     346 PRECALL                  1
-                     350 CALL                     1
-                     360 POP_TOP
+          69         316 LOAD_GLOBAL             15 (NULL + input)
+                     328 PRECALL                  0
+                     332 CALL                     0
+                     342 STORE_FAST               2 (cmd)
+         
+          70         344 LOAD_FAST                2 (cmd)
+                     346 LOAD_CONST               8 ('')
+                     348 COMPARE_OP               2 (==)
+                     354 POP_JUMP_FORWARD_IF_FALSE     2 (to 360)
+         
+          71         356 LOAD_FAST                4 (output)
+                     358 RETURN_VALUE
+         
+          70     >>  360 JUMP_FORWARD             2 (to 366)
+         
+          73     >>  362 LOAD_FAST                4 (output)
+                     364 RETURN_VALUE
+         
+          63     >>  366 JUMP_BACKWARD          139 (to 90)
+         
+          75     >>  368 BUILD_LIST               0
+                     370 STORE_FAST               5 (outputs)
+         
+          76         372 LOAD_GLOBAL             17 (NULL + track)
+                     384 LOAD_FAST                0 (cmd_list)
+                     386 LOAD_CONST               9 ('命令执行中')
+                     388 LOAD_CONST               2 (True)
+                     390 KW_NAMES                10
+                     392 PRECALL                  3
+                     396 CALL                     3
+                     406 GET_ITER
+                 >>  408 FOR_ITER               202 (to 814)
+                     410 STORE_FAST               2 (cmd)
+         
+          77         412 LOAD_FAST                1 (show_cmd)
+                     414 POP_JUMP_FORWARD_IF_FALSE    18 (to 452)
+         
+          78         416 LOAD_GLOBAL              5 (NULL + print)
+                     428 LOAD_CONST               1 ('\n')
+                     430 LOAD_FAST                2 (cmd)
+                     432 BINARY_OP                0 (+)
+                     436 PRECALL                  1
+                     440 CALL                     1
+                     450 POP_TOP
+         
+          79     >>  452 NOP
+         
+          80     >>  454 LOAD_GLOBAL              7 (NULL + subprocess)
+                     466 LOAD_ATTR                4 (getstatusoutput)
+                     476 LOAD_FAST                2 (cmd)
+                     478 PRECALL                  1
+                     482 CALL                     1
+                     492 UNPACK_SEQUENCE          2
+                     496 STORE_FAST               3 (exitcode)
+                     498 STORE_FAST               4 (output)
+         
+          81         500 LOAD_FAST                3 (exitcode)
+                     502 LOAD_CONST               3 (0)
+                     504 COMPARE_OP               3 (!=)
+                     510 POP_JUMP_FORWARD_IF_FALSE   127 (to 766)
+         
+          82         512 LOAD_GLOBAL             11 (NULL + echo)
+                     524 LOAD_CONST               4 ('执行 {} 失败！')
+                     526 LOAD_METHOD              6 (format)
+                     548 LOAD_FAST                2 (cmd)
+                     550 PRECALL                  1
+                     554 CALL                     1
+                     564 LOAD_CONST               5 ('#FF6AB3')
+                     566 PRECALL                  2
+                     570 CALL                     2
+                     580 POP_TOP
+         
+          83         582 LOAD_GLOBAL             11 (NULL + echo)
+                     594 LOAD_CONST               6 ('错误信息：\n{}')
+                     596 LOAD_METHOD              6 (format)
+                     618 LOAD_FAST                4 (output)
+                     620 PRECALL                  1
+                     624 CALL                     1
+                     634 PRECALL                  1
+                     638 CALL                     1
+                     648 POP_TOP
+         
+          84         650 LOAD_GLOBAL             11 (NULL + echo)
+                     662 LOAD_CONST               7 ('可通过在下方修改命令继续执行，或者直接按下回车键结束操作：')
+                     664 PRECALL                  1
+                     668 CALL                     1
+                     678 POP_TOP
+         
+          85         680 LOAD_GLOBAL             15 (NULL + input)
+                     692 PRECALL                  0
+                     696 CALL                     0
+                     706 STORE_FAST               2 (cmd)
+         
+          86         708 LOAD_FAST                2 (cmd)
+                     710 LOAD_CONST               8 ('')
+                     712 COMPARE_OP               2 (==)
+                     718 POP_JUMP_FORWARD_IF_FALSE    22 (to 764)
+         
+          87         720 LOAD_FAST                5 (outputs)
+                     722 LOAD_METHOD              9 (append)
+                     744 LOAD_FAST                4 (output)
+                     746 PRECALL                  1
+                     750 CALL                     1
+                     760 POP_TOP
+         
+          88         762 JUMP_FORWARD            24 (to 812)
+         
+          86     >>  764 JUMP_FORWARD            22 (to 810)
+         
+          90     >>  766 LOAD_FAST                5 (outputs)
+                     768 LOAD_METHOD              9 (append)
+                     790 LOAD_FAST                4 (output)
+                     792 PRECALL                  1
+                     796 CALL                     1
+                     806 POP_TOP
          
-          39         362 JUMP_FORWARD             1 (to 366)
+          91         808 JUMP_FORWARD             1 (to 812)
          
-          28     >>  364 JUMP_BACKWARD          151 (to 64)
-                 >>  366 JUMP_BACKWARD          155 (to 58)
+          79     >>  810 JUMP_BACKWARD          179 (to 454)
+                 >>  812 JUMP_BACKWARD          203 (to 408)
          
-          41     >>  368 LOAD_FAST                1 (outputs)
-                     370 RETURN_VALUE
+          93     >>  814 LOAD_FAST                5 (outputs)
+                     816 RETURN_VALUE
          consts
             None
+            '\n'
             True
             0
             '执行 {} 失败！'
             '#FF6AB3'
-            '可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：'
+            '错误信息：\n{}'
+            '可通过在下方修改命令继续执行，或者直接按下回车键结束操作：'
             ''
-         names      ('isinstance', 'list', 'subprocess', 'getstatusoutput', 'echo', 'format', 'input', 'append')
-         varnames   ('cmd_list', 'outputs', 'cmd', 'exitcode', 'output')
+            '命令执行中'
+            ('description', 'transient')
+         names      ('isinstance', 'str', 'print', 'subprocess', 'getstatusoutput', 'echo', 'format', 'input', 'track', 'append')
+         varnames   ('cmd_list', 'show_cmd', 'cmd', 'exitcode', 'output', 'outputs')
          freevars   ()
          cellvars   ()
          filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
          name       'run_cmd'
-         firstlineno 23
+         firstlineno 58
          lnotab
-            0x02012a0106010401080102013a010c0146011e011c010c012a0102fe02
-            042a0102f5040d
+            0x02012a0104010401240102012e010c01460144011e011c010c0104ff02
+            0304f6020c040128010401240102012e010c01460144011e011c010c012a
+            0102fe02042a0102f4040e
       '11.8'
       '3.9'
       code
          argcount  : 2
          nlocals   : 18
          stacksize : 7
          flags     : 3
@@ -391,56 +723,56 @@
             0da6010000ab0100000000000000007c086a060000000000000000640519
             0000000000000000007600721064257c086a060000000000000000640519
             0000000000000000007a0000007d106427a0090000000000000000000000
             0000000000000000007c0ea6010000ab0100000000000000007c086a0600
             000000000000006405190000000000000000007600721064257c086a0600
             000000000000006405190000000000000000007a0000007d118c9c7c0f7c
             107c1166035300
-          45           0 RESUME                   0
+          97           0 RESUME                   0
          
-          46           2 LOAD_CONST               1 ('https://download.pytorch.org/whl/torch_stable.html')
+          98           2 LOAD_CONST               1 ('https://download.pytorch.org/whl/torch_stable.html')
                        4 STORE_FAST               2 (url)
          
-          47           6 LOAD_GLOBAL              1 (NULL + rq)
+          99           6 LOAD_GLOBAL              1 (NULL + rq)
                       18 LOAD_ATTR                1 (get)
                       28 LOAD_FAST                2 (url)
                       30 PRECALL                  1
                       34 CALL                     1
                       44 LOAD_ATTR                2 (text)
                       54 STORE_FAST               3 (html)
          
-          48          56 LOAD_GLOBAL              7 (NULL + BeautifulSoup)
+         100          56 LOAD_GLOBAL              7 (NULL + BeautifulSoup)
                       68 LOAD_FAST                3 (html)
                       70 LOAD_CONST               2 ('html.parser')
                       72 PRECALL                  2
                       76 CALL                     2
                       86 STORE_FAST               4 (soup)
          
-          49          88 BUILD_LIST               0
+         101          88 BUILD_LIST               0
                       90 STORE_FAST               5 (available_items)
          
-          50          92 BUILD_LIST               0
+         102          92 BUILD_LIST               0
                       94 STORE_FAST               6 (backup_items)
          
-          51          96 LOAD_GLOBAL              9 (NULL + enumerate)
+         103          96 LOAD_GLOBAL              9 (NULL + enumerate)
                      108 LOAD_FAST                4 (soup)
                      110 LOAD_METHOD              5 (find_all)
                      132 LOAD_CONST               3 ('a')
                      134 PRECALL                  1
                      138 CALL                     1
                      148 PRECALL                  1
                      152 CALL                     1
                      162 GET_ITER
                  >>  164 EXTENDED_ARG             1
                      166 FOR_ITER               319 (to 806)
                      168 UNPACK_SEQUENCE          2
                      172 STORE_FAST               7 (i)
                      174 STORE_FAST               8 (item)
          
-          52         176 LOAD_CONST               4 ('-linux_x86_64.whl')
+         104         176 LOAD_CONST               4 ('-linux_x86_64.whl')
                      178 LOAD_FAST                8 (item)
                      180 LOAD_ATTR                6 (attrs)
                      190 LOAD_CONST               5 ('href')
                      192 BINARY_SUBSCR
                      202 CONTAINS_OP              0
                      204 EXTENDED_ARG             1
                      206 POP_JUMP_FORWARD_IF_FALSE   297 (to 802)
@@ -449,15 +781,15 @@
                      212 LOAD_ATTR                6 (attrs)
                      222 LOAD_CONST               5 ('href')
                      224 BINARY_SUBSCR
                      234 CONTAINS_OP              1
                      236 EXTENDED_ARG             1
                      238 POP_JUMP_FORWARD_IF_FALSE   281 (to 802)
          
-          53         240 LOAD_CONST               7 ('/torch-')
+         105         240 LOAD_CONST               7 ('/torch-')
                      242 LOAD_FAST                8 (item)
                      244 LOAD_ATTR                6 (attrs)
                      254 LOAD_CONST               5 ('href')
                      256 BINARY_SUBSCR
                      266 CONTAINS_OP              0
                      268 POP_JUMP_FORWARD_IF_TRUE    30 (to 330)
                      270 LOAD_CONST               8 ('/torchvision-')
@@ -471,32 +803,32 @@
                      302 LOAD_FAST                8 (item)
                      304 LOAD_ATTR                6 (attrs)
                      314 LOAD_CONST               5 ('href')
                      316 BINARY_SUBSCR
                      326 CONTAINS_OP              0
                      328 POP_JUMP_FORWARD_IF_FALSE   236 (to 802)
          
-          54     >>  330 LOAD_FAST                8 (item)
+         106     >>  330 LOAD_FAST                8 (item)
                      332 LOAD_ATTR                6 (attrs)
                      342 LOAD_CONST               5 ('href')
                      344 BINARY_SUBSCR
                      354 LOAD_METHOD              7 (startswith)
                      376 LOAD_CONST              10 ('cu')
                      378 PRECALL                  1
                      382 CALL                     1
                      392 POP_JUMP_FORWARD_IF_FALSE   204 (to 802)
          
-          55         394 LOAD_FAST                6 (backup_items)
+         107         394 LOAD_FAST                6 (backup_items)
                      396 LOAD_METHOD              8 (append)
                      418 LOAD_FAST                8 (item)
                      420 PRECALL                  1
                      424 CALL                     1
                      434 POP_TOP
          
-          56         436 LOAD_CONST              11 ('-cp{}-')
+         108         436 LOAD_CONST              11 ('-cp{}-')
                      438 LOAD_METHOD              9 (format)
                      460 LOAD_FAST                1 (python_version)
                      462 LOAD_METHOD             10 (replace)
                      484 LOAD_CONST              12 ('.')
                      486 LOAD_CONST              13 ('')
                      488 PRECALL                  2
                      492 CALL                     2
@@ -505,15 +837,15 @@
                      516 LOAD_FAST                8 (item)
                      518 LOAD_ATTR                6 (attrs)
                      528 LOAD_CONST               5 ('href')
                      530 BINARY_SUBSCR
                      540 CONTAINS_OP              0
                      542 POP_JUMP_FORWARD_IF_FALSE   129 (to 802)
          
-          57         544 LOAD_CONST              14 ('cu{}')
+         109         544 LOAD_CONST              14 ('cu{}')
                      546 LOAD_METHOD              9 (format)
                      568 LOAD_FAST                0 (cuda_version)
                      570 LOAD_METHOD             10 (replace)
                      592 LOAD_CONST              12 ('.')
                      594 LOAD_CONST              13 ('')
                      596 PRECALL                  2
                      600 CALL                     2
@@ -538,110 +870,110 @@
                      732 LOAD_FAST                8 (item)
                      734 LOAD_ATTR                6 (attrs)
                      744 LOAD_CONST               5 ('href')
                      746 BINARY_SUBSCR
                      756 CONTAINS_OP              0
                      758 POP_JUMP_FORWARD_IF_FALSE    21 (to 802)
          
-          58         760 LOAD_FAST                5 (available_items)
+         110         760 LOAD_FAST                5 (available_items)
                      762 LOAD_METHOD              8 (append)
                      784 LOAD_FAST                8 (item)
                      786 PRECALL                  1
                      790 CALL                     1
                      800 POP_TOP
                  >>  802 EXTENDED_ARG             1
                      804 JUMP_BACKWARD          321 (to 164)
          
-          60     >>  806 LOAD_GLOBAL             23 (NULL + len)
+         112     >>  806 LOAD_GLOBAL             23 (NULL + len)
                      818 LOAD_FAST                5 (available_items)
                      820 PRECALL                  1
                      824 CALL                     1
                      834 LOAD_CONST              15 (0)
                      836 COMPARE_OP               2 (==)
                      842 POP_JUMP_FORWARD_IF_FALSE   139 (to 1122)
          
-          61         844 LOAD_GLOBAL             25 (NULL + print)
+         113         844 LOAD_GLOBAL             25 (NULL + print)
                      856 LOAD_CONST              16 ('未找到可用的版本！')
                      858 PRECALL                  1
                      862 CALL                     1
                      872 POP_TOP
          
-          62         874 LOAD_GLOBAL             25 (NULL + print)
+         114         874 LOAD_GLOBAL             25 (NULL + print)
                      886 LOAD_CONST              17 ('可选的 CUDA 版本号：\n')
                      888 LOAD_GLOBAL             27 (NULL + set)
-                     900 LOAD_CONST              18 (<code object <listcomp>, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 62>)
+                     900 LOAD_CONST              18 (<code object <listcomp>, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 114>)
                      902 MAKE_FUNCTION            0
                      904 LOAD_FAST                6 (backup_items)
                      906 GET_ITER
                      908 PRECALL                  0
                      912 CALL                     0
                      922 PRECALL                  1
                      926 CALL                     1
                      936 PRECALL                  2
                      940 CALL                     2
                      950 POP_TOP
          
-          63         952 LOAD_GLOBAL             25 (NULL + print)
+         115         952 LOAD_GLOBAL             25 (NULL + print)
                      964 LOAD_CONST              19 ('可选的 Python 版本号：\n')
                      966 LOAD_GLOBAL             27 (NULL + set)
-                     978 LOAD_CONST              20 (<code object <listcomp>, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 63>)
+                     978 LOAD_CONST              20 (<code object <listcomp>, file "/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py", line 115>)
                      980 MAKE_FUNCTION            0
                      982 LOAD_FAST                6 (backup_items)
                      984 GET_ITER
                      986 PRECALL                  0
                      990 CALL                     0
                     1000 PRECALL                  1
                     1004 CALL                     1
                     1014 PRECALL                  2
                     1018 CALL                     2
                     1028 POP_TOP
          
-          64        1030 LOAD_GLOBAL             29 (NULL + input)
+         116        1030 LOAD_GLOBAL             29 (NULL + input)
                     1042 LOAD_CONST              21 ('请重新输入兼容的 CUDA 版本号：')
                     1044 PRECALL                  1
                     1048 CALL                     1
                     1058 STORE_FAST               0 (cuda_version)
          
-          65        1060 LOAD_GLOBAL             29 (NULL + input)
+         117        1060 LOAD_GLOBAL             29 (NULL + input)
                     1072 LOAD_CONST              22 ('请重新输入兼容的 Python 版本号：')
                     1074 PRECALL                  1
                     1078 CALL                     1
                     1088 STORE_FAST               1 (python_version)
          
-          66        1090 LOAD_GLOBAL             31 (NULL + show_available_version)
+         118        1090 LOAD_GLOBAL             31 (NULL + show_available_version)
                     1102 LOAD_FAST                0 (cuda_version)
                     1104 LOAD_FAST                1 (python_version)
                     1106 PRECALL                  2
                     1110 CALL                     2
                     1120 RETURN_VALUE
          
-          68     >> 1122 BUILD_LIST               0
+         120     >> 1122 BUILD_LIST               0
                     1124 STORE_FAST               9 (torch_version)
          
-          69        1126 BUILD_LIST               0
+         121        1126 BUILD_LIST               0
                     1128 STORE_FAST              10 (torchvision_version)
          
-          70        1130 BUILD_LIST               0
+         122        1130 BUILD_LIST               0
                     1132 STORE_FAST              11 (torchaudio_version)
          
-          71        1134 LOAD_FAST                5 (available_items)
+         123        1134 LOAD_FAST                5 (available_items)
                     1136 GET_ITER
                  >> 1138 EXTENDED_ARG             1
                     1140 FOR_ITER               294 (to 1730)
                     1142 STORE_FAST               8 (item)
          
-          72        1144 LOAD_CONST              23 ('torch-')
+         124        1144 LOAD_CONST              23 ('torch-')
                     1146 LOAD_FAST                8 (item)
                     1148 LOAD_ATTR                6 (attrs)
                     1158 LOAD_CONST               5 ('href')
                     1160 BINARY_SUBSCR
                     1170 CONTAINS_OP              0
                     1172 POP_JUMP_FORWARD_IF_FALSE    82 (to 1338)
          
-          73        1174 LOAD_FAST                9 (torch_version)
+         125        1174 LOAD_FAST                9 (torch_version)
                     1176 LOAD_METHOD              8 (append)
                     1198 LOAD_FAST                8 (item)
                     1200 LOAD_ATTR                6 (attrs)
                     1210 LOAD_CONST               5 ('href')
                     1212 BINARY_SUBSCR
                     1222 LOAD_METHOD             16 (split)
                     1244 LOAD_CONST              24 ('-')
@@ -655,23 +987,23 @@
                     1300 CALL                     1
                     1310 LOAD_CONST              15 (0)
                     1312 BINARY_SUBSCR
                     1322 PRECALL                  1
                     1326 CALL                     1
                     1336 POP_TOP
          
-          74     >> 1338 LOAD_CONST              27 ('torchvision-')
+         126     >> 1338 LOAD_CONST              27 ('torchvision-')
                     1340 LOAD_FAST                8 (item)
                     1342 LOAD_ATTR                6 (attrs)
                     1352 LOAD_CONST               5 ('href')
                     1354 BINARY_SUBSCR
                     1364 CONTAINS_OP              0
                     1366 POP_JUMP_FORWARD_IF_FALSE    82 (to 1532)
          
-          75        1368 LOAD_FAST               10 (torchvision_version)
+         127        1368 LOAD_FAST               10 (torchvision_version)
                     1370 LOAD_METHOD              8 (append)
                     1392 LOAD_FAST                8 (item)
                     1394 LOAD_ATTR                6 (attrs)
                     1404 LOAD_CONST               5 ('href')
                     1406 BINARY_SUBSCR
                     1416 LOAD_METHOD             16 (split)
                     1438 LOAD_CONST              24 ('-')
@@ -685,23 +1017,23 @@
                     1494 CALL                     1
                     1504 LOAD_CONST              15 (0)
                     1506 BINARY_SUBSCR
                     1516 PRECALL                  1
                     1520 CALL                     1
                     1530 POP_TOP
          
-          76     >> 1532 LOAD_CONST              28 ('torchaudio-')
+         128     >> 1532 LOAD_CONST              28 ('torchaudio-')
                     1534 LOAD_FAST                8 (item)
                     1536 LOAD_ATTR                6 (attrs)
                     1546 LOAD_CONST               5 ('href')
                     1548 BINARY_SUBSCR
                     1558 CONTAINS_OP              0
                     1560 POP_JUMP_FORWARD_IF_FALSE    82 (to 1726)
          
-          77        1562 LOAD_FAST               11 (torchaudio_version)
+         129        1562 LOAD_FAST               11 (torchaudio_version)
                     1564 LOAD_METHOD              8 (append)
                     1586 LOAD_FAST                8 (item)
                     1588 LOAD_ATTR                6 (attrs)
                     1598 LOAD_CONST               5 ('href')
                     1600 BINARY_SUBSCR
                     1610 LOAD_METHOD             16 (split)
                     1632 LOAD_CONST              24 ('-')
@@ -717,54 +1049,54 @@
                     1700 BINARY_SUBSCR
                     1710 PRECALL                  1
                     1714 CALL                     1
                     1724 POP_TOP
                  >> 1726 EXTENDED_ARG             1
                     1728 JUMP_BACKWARD          296 (to 1138)
          
-          79     >> 1730 LOAD_GLOBAL             35 (NULL + echo)
+         131     >> 1730 LOAD_GLOBAL             35 (NULL + echo)
                     1742 LOAD_CONST              29 ('可选的 torch 版本号：')
                     1744 PRECALL                  1
                     1748 CALL                     1
                     1758 POP_TOP
          
-          80        1760 LOAD_GLOBAL              9 (NULL + enumerate)
+         132        1760 LOAD_GLOBAL              9 (NULL + enumerate)
                     1772 LOAD_GLOBAL             27 (NULL + set)
                     1784 LOAD_FAST                9 (torch_version)
                     1786 PRECALL                  1
                     1790 CALL                     1
                     1800 PRECALL                  1
                     1804 CALL                     1
                     1814 GET_ITER
                  >> 1816 FOR_ITER                43 (to 1904)
                     1818 UNPACK_SEQUENCE          2
                     1822 STORE_FAST               7 (i)
                     1824 STORE_FAST               8 (item)
          
-          81        1826 LOAD_GLOBAL             25 (NULL + print)
+         133        1826 LOAD_GLOBAL             25 (NULL + print)
                     1838 LOAD_CONST              30 ('{}、 {}')
                     1840 LOAD_METHOD              9 (format)
                     1862 LOAD_FAST                7 (i)
                     1864 LOAD_CONST              25 (1)
                     1866 BINARY_OP                0 (+)
                     1870 LOAD_FAST                8 (item)
                     1872 PRECALL                  2
                     1876 CALL                     2
                     1886 PRECALL                  1
                     1890 CALL                     1
                     1900 POP_TOP
                     1902 JUMP_BACKWARD           44 (to 1816)
          
-          82     >> 1904 LOAD_GLOBAL             29 (NULL + input)
+         134     >> 1904 LOAD_GLOBAL             29 (NULL + input)
                     1916 LOAD_CONST              31 ('请选择 torch 版本号，输入序号即可：')
                     1918 PRECALL                  1
                     1922 CALL                     1
                     1932 STORE_FAST              12 (selected_torch_version)
          
-          83        1934 LOAD_GLOBAL             37 (NULL + list)
+         135        1934 LOAD_GLOBAL             37 (NULL + list)
                     1946 LOAD_GLOBAL             27 (NULL + set)
                     1958 LOAD_FAST                9 (torch_version)
                     1960 PRECALL                  1
                     1964 CALL                     1
                     1974 PRECALL                  1
                     1978 CALL                     1
                     1988 LOAD_GLOBAL             39 (NULL + int)
@@ -772,54 +1104,54 @@
                     2002 PRECALL                  1
                     2006 CALL                     1
                     2016 LOAD_CONST              25 (1)
                     2018 BINARY_OP               10 (-)
                     2022 BINARY_SUBSCR
                     2032 STORE_FAST              12 (selected_torch_version)
          
-          84        2034 LOAD_GLOBAL             25 (NULL + print)
+         136        2034 LOAD_GLOBAL             25 (NULL + print)
                     2046 LOAD_CONST              32 ('可选的 torchvision 版本号：')
                     2048 PRECALL                  1
                     2052 CALL                     1
                     2062 POP_TOP
          
-          85        2064 LOAD_GLOBAL              9 (NULL + enumerate)
+         137        2064 LOAD_GLOBAL              9 (NULL + enumerate)
                     2076 LOAD_GLOBAL             27 (NULL + set)
                     2088 LOAD_FAST               10 (torchvision_version)
                     2090 PRECALL                  1
                     2094 CALL                     1
                     2104 PRECALL                  1
                     2108 CALL                     1
                     2118 GET_ITER
                  >> 2120 FOR_ITER                43 (to 2208)
                     2122 UNPACK_SEQUENCE          2
                     2126 STORE_FAST               7 (i)
                     2128 STORE_FAST               8 (item)
          
-          86        2130 LOAD_GLOBAL             25 (NULL + print)
+         138        2130 LOAD_GLOBAL             25 (NULL + print)
                     2142 LOAD_CONST              30 ('{}、 {}')
                     2144 LOAD_METHOD              9 (format)
                     2166 LOAD_FAST                7 (i)
                     2168 LOAD_CONST              25 (1)
                     2170 BINARY_OP                0 (+)
                     2174 LOAD_FAST                8 (item)
                     2176 PRECALL                  2
                     2180 CALL                     2
                     2190 PRECALL                  1
                     2194 CALL                     1
                     2204 POP_TOP
                     2206 JUMP_BACKWARD           44 (to 2120)
          
-          87     >> 2208 LOAD_GLOBAL             29 (NULL + input)
+         139     >> 2208 LOAD_GLOBAL             29 (NULL + input)
                     2220 LOAD_CONST              33 ('请选择 torchvision 版本号，输入序号即可：')
                     2222 PRECALL                  1
                     2226 CALL                     1
                     2236 STORE_FAST              13 (selected_torchvision_version)
          
-          88        2238 LOAD_GLOBAL             37 (NULL + list)
+         140        2238 LOAD_GLOBAL             37 (NULL + list)
                     2250 LOAD_GLOBAL             27 (NULL + set)
                     2262 LOAD_FAST               10 (torchvision_version)
                     2264 PRECALL                  1
                     2268 CALL                     1
                     2278 PRECALL                  1
                     2282 CALL                     1
                     2292 LOAD_GLOBAL             39 (NULL + int)
@@ -827,54 +1159,54 @@
                     2306 PRECALL                  1
                     2310 CALL                     1
                     2320 LOAD_CONST              25 (1)
                     2322 BINARY_OP               10 (-)
                     2326 BINARY_SUBSCR
                     2336 STORE_FAST              13 (selected_torchvision_version)
          
-          89        2338 LOAD_GLOBAL             25 (NULL + print)
+         141        2338 LOAD_GLOBAL             25 (NULL + print)
                     2350 LOAD_CONST              34 ('可选的 torchaudio 版本号：')
                     2352 PRECALL                  1
                     2356 CALL                     1
                     2366 POP_TOP
          
-          90        2368 LOAD_GLOBAL              9 (NULL + enumerate)
+         142        2368 LOAD_GLOBAL              9 (NULL + enumerate)
                     2380 LOAD_GLOBAL             27 (NULL + set)
                     2392 LOAD_FAST               11 (torchaudio_version)
                     2394 PRECALL                  1
                     2398 CALL                     1
                     2408 PRECALL                  1
                     2412 CALL                     1
                     2422 GET_ITER
                  >> 2424 FOR_ITER                43 (to 2512)
                     2426 UNPACK_SEQUENCE          2
                     2430 STORE_FAST               7 (i)
                     2432 STORE_FAST               8 (item)
          
-          91        2434 LOAD_GLOBAL             25 (NULL + print)
+         143        2434 LOAD_GLOBAL             25 (NULL + print)
                     2446 LOAD_CONST              30 ('{}、 {}')
                     2448 LOAD_METHOD              9 (format)
                     2470 LOAD_FAST                7 (i)
                     2472 LOAD_CONST              25 (1)
                     2474 BINARY_OP                0 (+)
                     2478 LOAD_FAST                8 (item)
                     2480 PRECALL                  2
                     2484 CALL                     2
                     2494 PRECALL                  1
                     2498 CALL                     1
                     2508 POP_TOP
                     2510 JUMP_BACKWARD           44 (to 2424)
          
-          92     >> 2512 LOAD_GLOBAL             29 (NULL + input)
+         144     >> 2512 LOAD_GLOBAL             29 (NULL + input)
                     2524 LOAD_CONST              35 ('请选择 torchaudio 版本号，输入序号即可：')
                     2526 PRECALL                  1
                     2530 CALL                     1
                     2540 STORE_FAST              14 (selected_torchaudio_version)
          
-          93        2542 LOAD_GLOBAL             37 (NULL + list)
+         145        2542 LOAD_GLOBAL             37 (NULL + list)
                     2554 LOAD_GLOBAL             27 (NULL + set)
                     2566 LOAD_FAST               11 (torchaudio_version)
                     2568 PRECALL                  1
                     2572 CALL                     1
                     2582 PRECALL                  1
                     2586 CALL                     1
                     2596 LOAD_GLOBAL             39 (NULL + int)
@@ -882,95 +1214,95 @@
                     2610 PRECALL                  1
                     2614 CALL                     1
                     2624 LOAD_CONST              25 (1)
                     2626 BINARY_OP               10 (-)
                     2630 BINARY_SUBSCR
                     2640 STORE_FAST              14 (selected_torchaudio_version)
          
-          95        2642 LOAD_CONST              13 ('')
+         147        2642 LOAD_CONST              13 ('')
                     2644 STORE_FAST              15 (torch_url)
          
-          96        2646 LOAD_CONST              13 ('')
+         148        2646 LOAD_CONST              13 ('')
                     2648 STORE_FAST              16 (torchvision_url)
          
-          97        2650 LOAD_CONST              13 ('')
+         149        2650 LOAD_CONST              13 ('')
                     2652 STORE_FAST              17 (torchaudio_url)
          
-          98        2654 LOAD_GLOBAL              9 (NULL + enumerate)
+         150        2654 LOAD_GLOBAL              9 (NULL + enumerate)
                     2666 LOAD_FAST                5 (available_items)
                     2668 PRECALL                  1
                     2672 CALL                     1
                     2682 GET_ITER
                  >> 2684 FOR_ITER               155 (to 2996)
                     2686 UNPACK_SEQUENCE          2
                     2690 STORE_FAST               7 (i)
                     2692 STORE_FAST               8 (item)
          
-          99        2694 LOAD_CONST              36 ('/torch-{}')
+         151        2694 LOAD_CONST              36 ('/torch-{}')
                     2696 LOAD_METHOD              9 (format)
                     2718 LOAD_FAST               12 (selected_torch_version)
                     2720 PRECALL                  1
                     2724 CALL                     1
                     2734 LOAD_FAST                8 (item)
                     2736 LOAD_ATTR                6 (attrs)
                     2746 LOAD_CONST               5 ('href')
                     2748 BINARY_SUBSCR
                     2758 CONTAINS_OP              0
                     2760 POP_JUMP_FORWARD_IF_FALSE    16 (to 2794)
          
-         100        2762 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
+         152        2762 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
                     2764 LOAD_FAST                8 (item)
                     2766 LOAD_ATTR                6 (attrs)
                     2776 LOAD_CONST               5 ('href')
                     2778 BINARY_SUBSCR
                     2788 BINARY_OP                0 (+)
                     2792 STORE_FAST              15 (torch_url)
          
-         101     >> 2794 LOAD_CONST              38 ('/torchvision-{}')
+         153     >> 2794 LOAD_CONST              38 ('/torchvision-{}')
                     2796 LOAD_METHOD              9 (format)
                     2818 LOAD_FAST               13 (selected_torchvision_version)
                     2820 PRECALL                  1
                     2824 CALL                     1
                     2834 LOAD_FAST                8 (item)
                     2836 LOAD_ATTR                6 (attrs)
                     2846 LOAD_CONST               5 ('href')
                     2848 BINARY_SUBSCR
                     2858 CONTAINS_OP              0
                     2860 POP_JUMP_FORWARD_IF_FALSE    16 (to 2894)
          
-         102        2862 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
+         154        2862 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
                     2864 LOAD_FAST                8 (item)
                     2866 LOAD_ATTR                6 (attrs)
                     2876 LOAD_CONST               5 ('href')
                     2878 BINARY_SUBSCR
                     2888 BINARY_OP                0 (+)
                     2892 STORE_FAST              16 (torchvision_url)
          
-         103     >> 2894 LOAD_CONST              39 ('/torchaudio-{}')
+         155     >> 2894 LOAD_CONST              39 ('/torchaudio-{}')
                     2896 LOAD_METHOD              9 (format)
                     2918 LOAD_FAST               14 (selected_torchaudio_version)
                     2920 PRECALL                  1
                     2924 CALL                     1
                     2934 LOAD_FAST                8 (item)
                     2936 LOAD_ATTR                6 (attrs)
                     2946 LOAD_CONST               5 ('href')
                     2948 BINARY_SUBSCR
                     2958 CONTAINS_OP              0
                     2960 POP_JUMP_FORWARD_IF_FALSE    16 (to 2994)
          
-         104        2962 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
+         156        2962 LOAD_CONST              37 ('https://download.pytorch.org/whl/')
                     2964 LOAD_FAST                8 (item)
                     2966 LOAD_ATTR                6 (attrs)
                     2976 LOAD_CONST               5 ('href')
                     2978 BINARY_SUBSCR
                     2988 BINARY_OP                0 (+)
                     2992 STORE_FAST              17 (torchaudio_url)
                  >> 2994 JUMP_BACKWARD          156 (to 2684)
          
-         106     >> 2996 LOAD_FAST               15 (torch_url)
+         158     >> 2996 LOAD_FAST               15 (torch_url)
                     2998 LOAD_FAST               16 (torchvision_url)
                     3000 LOAD_FAST               17 (torchaudio_url)
                     3002 BUILD_TUPLE              3
                     3004 RETURN_VALUE
          consts
             None
             'https://download.pytorch.org/whl/torch_stable.html'
@@ -997,15 +1329,15 @@
                flags     : 19
                code
                   0x970067007c005d3c7d017c016a00000000000000000064001900000000
                   0000000000a00100000000000000000000000000000000000000006401a6
                   010000ab010000000000000000640219000000000000000000a002000000
                   000000000000000000000000000000000064036404a6020000ab02000000
                   000000000091028c3d5300
-                62           0 RESUME                   0
+               114           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                60 (to 128)
                              8 STORE_FAST               1 (item)
                             10 LOAD_FAST                1 (item)
                             12 LOAD_ATTR                0 (attrs)
                             22 LOAD_CONST               0 ('href')
@@ -1032,29 +1364,29 @@
                   ''
                names      ('attrs', 'split', 'replace')
                varnames   ('.0', 'item')
                freevars   ()
                cellvars   ()
                filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
                name       '<listcomp>'
-               firstlineno 62
+               firstlineno 114
                lnotab 0x
             '可选的 Python 版本号：\n'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d3c7d017c016a00000000000000000064001900000000
                   0000000000a00100000000000000000000000000000000000000006401a6
                   010000ab010000000000000000640219000000000000000000a002000000
                   000000000000000000000000000000000064036404a6020000ab02000000
                   000000000091028c3d5300
-                63           0 RESUME                   0
+               115           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                60 (to 128)
                              8 STORE_FAST               1 (item)
                             10 LOAD_FAST                1 (item)
                             12 LOAD_ATTR                0 (attrs)
                             22 LOAD_CONST               0 ('href')
@@ -1081,15 +1413,15 @@
                   ''
                names      ('attrs', 'split', 'replace')
                varnames   ('.0', 'item')
                freevars   ()
                cellvars   ()
                filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
                name       '<listcomp>'
-               firstlineno 63
+               firstlineno 115
                lnotab 0x
             '请重新输入兼容的 CUDA 版本号：'
             '请重新输入兼容的 Python 版本号：'
             'torch-'
             '-'
             1
             '%'
@@ -1108,23 +1440,24 @@
             '/torchaudio-{}'
          names      ('rq', 'get', 'text', 'BeautifulSoup', 'enumerate', 'find_all', 'attrs', 'startswith', 'append', 'format', 'replace', 'len', 'print', 'set', 'input', 'show_available_version', 'split', 'echo', 'list', 'int')
          varnames   ('cuda_version', 'python_version', 'url', 'html', 'soup', 'available_items', 'backup_items', 'i', 'item', 'torch_version', 'torchvision_version', 'torchaudio_version', 'selected_torch_version', 'selected_torchvision_version', 'selected_torchaudio_version', 'torch_url', 'torchvision_url', 'torchaudio_url')
          freevars   ()
          cellvars   ()
          filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
          name       'show_available_version'
-         firstlineno 45
+         firstlineno 97
          lnotab
             0x020104013201200104010401500140015a0140012a016c01d8012e0226
             011e014e014e011e011e0120020401040104010a011e01a4011e01a4011e
             01a8021e0142014e011e0164011e0142014e011e0164011e0142014e011e
             0164020401040104012801440120014401200144012202
       ('green',)
+      (True,)
       ('11.8', '3.9')
-   names      ('bs4', 'BeautifulSoup', 'requests', 'rq', 'pkg_resources', 'os', 'rich.console', 'Console', 'console', 'package_installed', 'echo', 'run_cmd', 'show_available_version')
+   names      ('bs4', 'BeautifulSoup', 'requests', 'rq', 'pkg_resources', 'os', 'rich.console', 'Console', 'subprocess', 'rich.progress', 'track', 'console', 'package_installed', 'echo', 'run_cmd_inactivate', 'run_cmd', 'show_available_version')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dengyifan/Desktop/Github仓库/lazyinit/lazyinit/utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010801080108010c021402060b08030616
+   lnotab 0x00ff02010c010801080108010c0108010c021402060b080406200827
```

### Comparing `lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-38.pyc` & `lazyinit-0.0.28/lazyinit/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/bash_config.txt` & `lazyinit-0.0.28/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/init.py` & `lazyinit-0.0.28/lazyinit/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,29 +32,28 @@
         run_cmd(bash, show_cmd=False)
         echo("运行 {} 以完成配置（运行后需要重启工具）".format("source ~/.bashrc"), "yellow")
         exit(0)
         
     echo("")
     echo("")
     echo("")
-    echo("      _____                          _      ____                  _")
-    echo("     |  __ \\                        | |    |  _ \\                | |")
-    echo("     | |__) |____      _____ _ __ __| |    | |_) |_   _          | |")
-    echo("     |  ___/ _ \\ \\ /\\ / / _ \\ '__/ _` |    |  _ <| | | |     _   | |")
-    echo("     | |  | (_) \\ V  V /  __/ | | (_| |    | |_) | |_| |    | |__| |")
-    echo("     |_|   \\___/ \\_/\\_/ \\___|_|  \\__,_|    |____/ \\__, |     \\____/")
-    echo("                                                   __/ |")
-    echo("                                                  |___/")
+    echo("")
+    echo("")
+    echo("         __                         __  ___      __                ____")
+    echo("        / /   ____ _____  __  __   /  |/  /___ _/ /_____  _____   / __ )__  _________  __")
+    echo("       / /   / __ `/_  / / / / /  / /|_/ / __ `/ //_/ _ \\/ ___/  / __  / / / / ___/ / / /")
+    echo("      / /___/ /_/ / / /_/ /_/ /  / /  / / /_/ / ,< /  __(__  )  / /_/ / /_/ (__  ) /_/ /")
+    echo("     /_____/\\__,_/ /___/\\__, /  /_/  /_/\\__,_/_/|_|\\___/____/  /_____/\\__,_/____/\\__, /")
+    echo("                       /____/                                                   /____/")
     echo("")
     echo("")
     echo("")
-    echo("             欢迎使用服务器环境初始化工具 lazydl-init ！", "green")
     echo("")
-    echo("   本工具将会帮助您初始化服务器环境，下面是功能菜单，可输入序号进行配置", "green")
 
+ 
     step = "-1"
     while step != "0":
         if step != "-1":
             echo("\n是否继续配置？（y/n）", "yellow")
             conti = input()
             if conti != "y":
                 break
```

### Comparing `lazyinit-0.0.27/lazyinit/lazydl/configs/default_config.yaml` & `lazyinit-0.0.28/lazyinit/lazydl/configs/default_config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # @package _global_
 
 defaults:
   - override hydra/hydra_logging: colorlog
   - override hydra/job_logging: colorlog
   - _self_
 
-comet_api_key: lGIPkizDNha2kLEsqNDinrAgP
+comet_api_key: 
 comet_project_name: Default Project
 
-dingding_secret: SEC86418ce8939ca7ff3d2442ead039cec1d6cb765b01d7971e20b2c69ab2069eb3
-dingding_access_token: 5f7199dea2b58e5c765fc3573335e0f558207ecf75304114c5015e2a6b4fed58
+dingding_secret: 
+dingding_access_token: 
 
 visibale_cuda: all
 
-huggingface_hub_token: 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
+huggingface_hub_token: 
 
 # 处理器类型
 # 如果为 gpu，共有以下几种选择：
 # 自动选择需要加上 ^ 符号，即 ^[GPU 数量]，如 ^2 表示自动选择 2 块显卡
 # 手动选择直接列出需要使用的显卡编号，如 0,1 表示使用 0 号和 1 号显卡
-processing_unit: cpu  # 必需
+processing_unit: ^1  # 必需
 # 是否排队等待处理器
 queuing: False  # 必需
 # 选择的处理器最小空闲显存，单位为 GB
 processing_unit_min_free_memory: 2
 # 选择的处理器最小空闲显存比例
 processing_unit_min_free_memory_ratio: 0.1
 # 处理器选择，程序自动填充，不需要手动填写
```

### Comparing `lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/baseline.yaml` & `lazyinit-0.0.28/lazyinit/lazydl/configs/exps/exp1/baseline.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/lazydl/minist.py` & `lazyinit-0.0.28/lazyinit/lazydl/minist.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/lazydl/run.py` & `lazyinit-0.0.28/lazyinit/lazydl/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/.DS_Store` & `lazyinit-0.0.28/lazyinit/ranger/.DS_Store`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/colorschemes/default.py` & `lazyinit-0.0.28/lazyinit/ranger/colorschemes/default.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/colorschemes/jungle.py` & `lazyinit-0.0.28/lazyinit/ranger/colorschemes/jungle.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.py` & `lazyinit-0.0.28/lazyinit/ranger/colorschemes/snow.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.pyo` & `lazyinit-0.0.28/lazyinit/ranger/colorschemes/snow.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/colorschemes/zenburn.py` & `lazyinit-0.0.28/lazyinit/ranger/colorschemes/zenburn.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/commands.py` & `lazyinit-0.0.28/lazyinit/ranger/commands.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.py` & `lazyinit-0.0.28/lazyinit/ranger/plugins/devicons.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.pyo` & `lazyinit-0.0.28/lazyinit/ranger/plugins/devicons.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.pyo` & `lazyinit-0.0.28/lazyinit/ranger/plugins/devicons_linemode.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/rc-sample.conf` & `lazyinit-0.0.28/lazyinit/ranger/rc-sample.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/rc.conf` & `lazyinit-0.0.28/lazyinit/ranger/rc.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/rifle.conf` & `lazyinit-0.0.28/lazyinit/ranger/rifle.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/ranger/scope.sh` & `lazyinit-0.0.28/lazyinit/ranger/scope.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/redis.conf` & `lazyinit-0.0.28/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit/run.py` & `lazyinit-0.0.28/lazyinit/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 def run():
     
     # project_path = "/Users/dengyifan/Desktop/Github仓库/zheinit/zheinit/ProjectTemplate"
     project_path = os.getcwd()
     echo("")
     echo("")
     echo("")
-    echo("      _____                          _      ____                  _")
-    echo("     |  __ \\                        | |    |  _ \\                | |")
-    echo("     | |__) |____      _____ _ __ __| |    | |_) |_   _          | |")
-    echo("     |  ___/ _ \\ \\ /\\ / / _ \\ '__/ _` |    |  _ <| | | |     _   | |")
-    echo("     | |  | (_) \\ V  V /  __/ | | (_| |    | |_) | |_| |    | |__| |")
-    echo("     |_|   \\___/ \\_/\\_/ \\___|_|  \\__,_|    |____/ \\__, |     \\____/")
-    echo("                                                   __/ |")
-    echo("                                                  |___/")
     echo("")
     echo("")
+    echo("         __                         __  ___      __                ____")
+    echo("        / /   ____ _____  __  __   /  |/  /___ _/ /_____  _____   / __ )__  _________  __")
+    echo("       / /   / __ `/_  / / / / /  / /|_/ / __ `/ //_/ _ \\/ ___/  / __  / / / / ___/ / / /")
+    echo("      / /___/ /_/ / / /_/ /_/ /  / /  / / /_/ / ,< /  __(__  )  / /_/ / /_/ (__  ) /_/ /")
+    echo("     /_____/\\__,_/ /___/\\__, /  /_/  /_/\\__,_/_/|_|\\___/____/  /_____/\\__,_/____/\\__, /")
+    echo("                       /____/                                                   /____/")
     echo("")
-    echo("                      欢迎使用 zhei 项目启动器！")
+    echo("")
+    echo("")
+    echo("                                  欢迎使用 LadyDL 项目启动器！")
     echo("")
     echo("当前工作目录为：{}".format(project_path))
     
     # 获取可选的项目名
     projects = os.listdir(os.path.join(project_path, "configs/exps"))
     echo("\n可选的项目名：")
     for i, project in enumerate(projects):
```

### Comparing `lazyinit-0.0.27/lazyinit/utils.py` & `lazyinit-0.0.28/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/lazyinit.egg-info/SOURCES.txt` & `lazyinit-0.0.28/lazyinit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,16 @@
 .git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
 .git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
 .git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
 .git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
 .git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
 .git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
 .git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
+.git/objects/a9/7852c14503686493d3218632fbbb52dd42628b
+.git/objects/a9/95569e1ac0accec5b1acc68f0ab077023bc4f4
 .git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
 .git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
 .git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
 .git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
 .git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
 .git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
 .git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
@@ -148,14 +150,15 @@
 .git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
 .git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
 .git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
 .git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
 .git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
 .git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
 .git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
+.git/objects/d2/99be9b16073ba179c8b1558984116cd0eb9f3b
 .git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
 .git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
 .git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
 .git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
 .git/objects/e4/632035cac16d026cc02de90ae31aef87867116
 .git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
 .git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
@@ -182,25 +185,25 @@
 lazyinit/utils.py
 lazyinit.egg-info/PKG-INFO
 lazyinit.egg-info/SOURCES.txt
 lazyinit.egg-info/dependency_links.txt
 lazyinit.egg-info/entry_points.txt
 lazyinit.egg-info/requires.txt
 lazyinit.egg-info/top_level.txt
+lazyinit/__pycache__/__init__.cpython-311.pyc
 lazyinit/__pycache__/utils.cpython-311.pyc
 lazyinit/__pycache__/utils.cpython-38.pyc
 lazyinit/lazydl/README.md
 lazyinit/lazydl/minist.py
 lazyinit/lazydl/requirements.txt
 lazyinit/lazydl/run.py
 lazyinit/lazydl/start.py
 lazyinit/lazydl/configs/default_config.yaml
-lazyinit/lazydl/configs/exps/overfit_test.yaml
-lazyinit/lazydl/configs/exps/focusl/baseline.yaml
-lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml
+lazyinit/lazydl/configs/exps/exp1/baseline.yaml
+lazyinit/lazydl/configs/exps/exp1/exp_plan.yaml
 lazyinit/ranger/.DS_Store
 lazyinit/ranger/README.md
 lazyinit/ranger/commands.py
 lazyinit/ranger/rc-sample.conf
 lazyinit/ranger/rc.conf
 lazyinit/ranger/rifle.conf
 lazyinit/ranger/scope.sh
```

### Comparing `lazyinit-0.0.27/push.sh` & `lazyinit-0.0.28/push.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.27/setup.py` & `lazyinit-0.0.28/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.27',
+    version='0.0.28',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
-    description=u'Init zhei environment.',
+    description=u'Init lazydl environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'bs4',
         'requests',
         'rich',
```

