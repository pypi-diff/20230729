# Comparing `tmp/beanclerk-0.0.4.tar.gz` & `tmp/beanclerk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanclerk-0.0.4.tar", last modified: Wed Jul 26 15:20:38 2023, max compression
+gzip compressed data, was "beanclerk-0.0.5.tar", last modified: Sat Jul 29 11:17:41 2023, max compression
```

## Comparing `beanclerk-0.0.4.tar` & `beanclerk-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.896668 beanclerk-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-26 15:20:27.000000 beanclerk-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-07-26 15:20:38.896668 beanclerk-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-26 15:20:27.000000 beanclerk-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/bean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/banka_creditas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-26 15:20:27.000000 beanclerk-0.0.4/beanclerk/importers/fio_banka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/beanclerk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 15:20:38.000000 beanclerk-0.0.4/beanclerk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-26 15:20:27.000000 beanclerk-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:20:38.896668 beanclerk-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:38.892667 beanclerk-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-26 15:20:27.000000 beanclerk-0.0.4/tests/test_clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 15:20:27.000000 beanclerk-0.0.4/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.968478 beanclerk-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.960477 beanclerk-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.960477 beanclerk-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.github/workflows/publishing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 11:17:29.000000 beanclerk-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-29 11:17:29.000000 beanclerk-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-07-29 11:17:41.968478 beanclerk-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-29 11:17:29.000000 beanclerk-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/bean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-29 11:17:29.000000 beanclerk-0.0.5/beanclerk/importers/fio_banka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/beanclerk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 11:17:41.000000 beanclerk-0.0.5/beanclerk.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-07-29 11:17:29.000000 beanclerk-0.0.5/build_venv
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-29 11:17:29.000000 beanclerk-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:17:41.968478 beanclerk-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.964477 beanclerk-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/beanclerk-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:41.968478 beanclerk-0.0.5/tests/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/banka_creditas_transactions.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/fio_banka_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/test_banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/importers/test_fio_banka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/ledger.beancount
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/test_clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-29 11:17:29.000000 beanclerk-0.0.5/tests/test_config.py
```

### Comparing `beanclerk-0.0.4/LICENSE` & `beanclerk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.4/PKG-INFO` & `beanclerk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -374,25 +374,30 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
 Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
 
 1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
-2. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
+1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+
+**Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
+
+**Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
 Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. So it does not have to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or even solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
@@ -410,36 +415,79 @@
 ```
 
 Confirm successful installation by running:
 ```
 bean-clerk -h
 ```
 
-## Usage (work in progress)
+## Usage
 
 ### Configuration
 
-Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory, or a path to the config file may be set by the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
+Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
 Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+
+```
+...
+No categorization rule matches the following transaction:
+Transaction(
+    meta={
+        'id': '10000000002',
+        'account_id': '2345678901',
+        'account_name': 'Pavel, Žák',
+        'bank_id': '2010',
+        'bank_name': 'Fio banka, a.s.',
+        'type': 'Příjem převodem uvnitř banky',
+        'specification': 'test specification',
+        'bic': 'TESTBICXXXX',
+        'order_id': '30000000002',
+        'payer_reference': 'test payer reference'
+    },
+    date=datetime.date(2023, 1, 3),
+    flag='*',
+    payee=None,
+    narration='',
+    tags=frozenset(),
+    links=frozenset(),
+    postings=[
+        Posting(
+            account='Assets:Banks:Fio:Checking',
+            units=500.0 CZK,
+            cost=None,
+            price=None,
+            flag=None,
+            meta={}
+        )
+    ]
+)
+Available actions:
+'r': reload config (you should add a new rule first)
+'i': import as-is (transaction remains unbalanced)
+...
+```
+
 ## Contributing
 
-Set up a development environment:
+Contributions are welcome. Make sure to create an issue first so we can discuss it.
+
+Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
 
-Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
-
 Run tests:
 ```bash
 pytest
 ```
+
+Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `beanclerk-0.0.4/README.md` & `beanclerk-0.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
 Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
 
 1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
-2. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
+1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+
+**Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
+
+**Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
 Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. So it does not have to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or even solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
@@ -43,36 +48,79 @@
 ```
 
 Confirm successful installation by running:
 ```
 bean-clerk -h
 ```
 
-## Usage (work in progress)
+## Usage
 
 ### Configuration
 
-Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory, or a path to the config file may be set by the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
+Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
 Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+
+```
+...
+No categorization rule matches the following transaction:
+Transaction(
+    meta={
+        'id': '10000000002',
+        'account_id': '2345678901',
+        'account_name': 'Pavel, Žák',
+        'bank_id': '2010',
+        'bank_name': 'Fio banka, a.s.',
+        'type': 'Příjem převodem uvnitř banky',
+        'specification': 'test specification',
+        'bic': 'TESTBICXXXX',
+        'order_id': '30000000002',
+        'payer_reference': 'test payer reference'
+    },
+    date=datetime.date(2023, 1, 3),
+    flag='*',
+    payee=None,
+    narration='',
+    tags=frozenset(),
+    links=frozenset(),
+    postings=[
+        Posting(
+            account='Assets:Banks:Fio:Checking',
+            units=500.0 CZK,
+            cost=None,
+            price=None,
+            flag=None,
+            meta={}
+        )
+    ]
+)
+Available actions:
+'r': reload config (you should add a new rule first)
+'i': import as-is (transaction remains unbalanced)
+...
+```
+
 ## Contributing
 
-Set up a development environment:
+Contributions are welcome. Make sure to create an issue first so we can discuss it.
+
+Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
 
-Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
-
 Run tests:
 ```bash
 pytest
 ```
+
+Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `beanclerk-0.0.4/beanclerk/bean_helpers.py` & `beanclerk-0.0.5/beanclerk/bean_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Helpers for Beancount"""
+"""Helpers for Beancount."""
 from collections.abc import Generator
 from datetime import date
 from typing import TypeVar
 
 from beancount.core.account import is_valid
 from beancount.core.data import (
     EMPTY_SET,
```

### Comparing `beanclerk-0.0.4/beanclerk/clerk.py` & `beanclerk-0.0.5/beanclerk/clerk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Clerk operations
+"""Clerk operations.
 
 This module provides operations consumed by the CLI.
 
-TODO:
+Todo:
     * handle exceptions
     * Python docs recommend to use utf-8 encoding for reading and writing files
     * validate txns coming from importers:
         * check that txns have only 1 posting
         * check that txns have id in their metadata
     * Test fn append_entry_to_file.
 """
@@ -285,15 +285,14 @@
         from_date (date | None): the first date to import
         to_date (date | None): the last date to import
 
     Raises:
         ClerkError: raised if there are errors in the input file
         ClerkError: raised if the initial import date cannot be determined
     """
-    """For each configured importer, import transactions and print import status."""
     config = load_config(config_file)
     entries, errors, _ = load_file(config.input_file)
     if errors != []:
         # TODO: format errors via beancount.parser.printer.format_errors
         raise ClerkError(f"Errors in the input file: {errors}")
 
     for account_config in config.accounts:
```

### Comparing `beanclerk-0.0.4/beanclerk/cli.py` & `beanclerk-0.0.5/beanclerk/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Beanclerk command-line interface"""
+"""Beanclerk command-line interface."""
 
 from datetime import date
 from pathlib import Path
 
 import click
 
 from .clerk import import_transactions
@@ -11,14 +11,15 @@
 CONFIG_FILE = "beanclerk-config.yml"
 
 
 @click.group(
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=False,
 )
+@click.version_option()
 @click.option(
     "-c",
     "--config-file",
     default=Path.cwd() / CONFIG_FILE,
     type=click.Path(path_type=Path),
     help=f"Path to a config file; defaults to `{CONFIG_FILE}` in the current working directory.",  # noqa: E501
 )
@@ -40,15 +41,15 @@
     """A convenience date type for Click.
 
     Converts dates to a date (instead of datetime).
     """
 
     name = "date"
 
-    def convert(self, value, param, ctx):
+    def convert(self, value, param, ctx):  # noqa: D102
         if isinstance(value, date):
             return value
         try:
             return date.fromisoformat(value)
         except ValueError:
             self.fail(
                 f"'{value}' is not a valid date format ({_ISO_DATE_FMT})",
```

### Comparing `beanclerk-0.0.4/beanclerk/config.py` & `beanclerk-0.0.5/beanclerk/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Configuration file parsing and validation.
 
 Notes:
     * If a validator modifies a value, it should always return the same type:
     https://github.com/pydantic/pydantic/discussions/3997
 
-TODO:
+Todo:
     * Add missing field validators.
 """
 # Disabling due to Pydantic notation (`cls` instead of `self`).
 # ruff: noqa: N805
 
 import importlib
 import os
@@ -20,49 +20,54 @@
 from pydantic_settings import BaseSettings
 
 from .bean_helpers import check_account_name
 from .exceptions import ConfigError
 from .importers import ApiImporterProtocol
 
 
-class BaseModelStrict(BaseModel):
+class _BaseModelStrict(BaseModel):
     model_config = ConfigDict(extra="forbid")
 
 
 class AccountConfig(BaseModel):
-    """Account config model
+    """Account config model.
 
     Allows extra fields to support custom configuration of importers.
     """
 
     account: str
     importer: str
 
     model_config = ConfigDict(extra="allow")  # allows access to extra fields
 
     @field_validator("account")
     def name_is_valid(cls, name: str) -> str:
+        """Validate account name."""
         check_account_name(name)
         return name
 
 
-class MatchCategories(BaseModelStrict):
+class MatchCategories(_BaseModelStrict):
+    """Match categories model."""
+
     metadata: dict[str, str]
 
 
-class CategorizationRule(BaseModelStrict):
+class CategorizationRule(_BaseModelStrict):
+    """Categorization rule model."""
+
     matches: MatchCategories
     account: str
     flag: str | None = None
     payee: str | None = None
     narration: str | None = None
 
 
 class Config(BaseSettings):
-    """Beanclerk config
+    """Beanclerk config model.
 
     Most attributes are defined in a config file. Config is a Pydantic
     model, and raises a `pydantic.ValidationError` on invalid fields.
     """
 
     vars: Any = None  # noqa: A003
     input_file: Path
@@ -72,16 +77,19 @@
     # fields not present in the config file
     config_file: Path
 
     model_config = ConfigDict(extra="forbid")
 
     @field_validator("input_file")
     def input_file_exists(cls, input_file: Path) -> Path:
-        # Side effects:
-        #   * expands user (`~`) and environment variables
+        """Validate input file exists.
+
+        Side effects:
+            * expands user (`~`) and environment variables
+        """
         filename: str = os.path.expandvars(input_file.expanduser())
         if not os.path.isabs(filename):  # noqa: PTH117
             filename = os.path.normpath(Path.cwd() / filename)
         input_file = Path(filename)
         if not input_file.exists():
             raise ValueError(f"Input file '{input_file}' does not exist")
         return input_file
@@ -108,15 +116,15 @@
         raise ConfigError(str(exc)) from exc
 
 
 def load_importer(account_config: AccountConfig) -> ApiImporterProtocol:
     """Return an instance of importer defined in the account config.
 
     Args:
-        account_config (AccountConfig)
+        account_config (AccountConfig): an account configuration
 
     Raises:
         ConfigError: Raised when the importer cannot be loaded
 
     Returns:
         ApiImporterProtocol: an instance of a particular importer implementing
             the API Importer Protocol
```

### Comparing `beanclerk-0.0.4/beanclerk/importers/__init__.py` & `beanclerk-0.0.5/beanclerk/importers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""API Importer Protocol and utilities for custom importers"""
+"""API Importer Protocol and utilities for custom importers."""
 
 import abc
 from datetime import date
 from typing import Any
 
 from beancount.core.data import Amount, Transaction
 
@@ -22,15 +22,15 @@
     for k, v in d.items():
         if not (v is None or v == ""):
             meta[k] = str(v)
     return meta
 
 
 class ApiImporterProtocol(abc.ABC):
-    """API Importer Protocol for custom importers
+    """API Importer Protocol for custom importers.
 
     All API importers must comply with this interface. Make sure to implement
     all methods decorated with `@abc.abstractmethod`. There are no restrictions
     on other methods, variables or properties.
     """
 
     @abc.abstractmethod
```

### Comparing `beanclerk-0.0.4/beanclerk/importers/banka_creditas.py` & `beanclerk-0.0.5/beanclerk/importers/banka_creditas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Banka Creditas a.s.
 
-TODO:
+Todo:
     This module is a work in progress. It needs a major rework.
 
 docs:
     https://www.creditas.cz/firma/creditas-api/
 """
 
 import base64
@@ -45,15 +45,15 @@
         body=body,
     )
     # TODO: handle other exceptions
     return base64.b64decode(data.export)
 
 
 # FIXME: This function has to be turned into a class implementing ApiImporterProtocol.
-def get_transactions(
+def get_transactions(  # noqa: D103
     token: str,
     account_id: str,
     bean_account: str,
     from_date: date,
 ) -> tuple[list[Transaction], Amount]:
     # TODO: handle etree.XMLSyntaxError
     # TODO: handle other exceptions
```

### Comparing `beanclerk-0.0.4/beanclerk/importers/fio_banka.py` & `beanclerk-0.0.5/beanclerk/importers/fio_banka.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """API importer for Fio banka, a.s.
 
-TODO:
+Todo:
     * handle fio_banka exceptions
 
 docs:
     https://www.fio.cz/bank-services/internetbanking-api
 """
 
 from datetime import date
@@ -13,24 +13,25 @@
 from beancount.core.data import Amount, Transaction
 
 from ..bean_helpers import create_posting, create_transaction
 from . import ApiImporterProtocol, TransactionReport, prepare_meta
 
 
 class ApiImporter(ApiImporterProtocol):
-    """API importer for Fio banka, a.s.
-
-    Args:
-        token (str): Fio banka API token
-    """
+    """API importer for Fio banka, a.s."""
 
     def __init__(self, token: str) -> None:
+        """Initialize the importer.
+
+        Args:
+            token (str): _description_
+        """
         self._token = token
 
-    def fetch_transactions(
+    def fetch_transactions(  # noqa: D102
         self,
         bean_account: str,
         from_date: date,
         to_date: date,
     ) -> TransactionReport:
         client = fio_banka.Account(self._token)
         statement = client.periods(from_date, to_date, fio_banka.TransactionsFmt.JSON)
```

### Comparing `beanclerk-0.0.4/beanclerk.egg-info/PKG-INFO` & `beanclerk-0.0.5/beanclerk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -374,25 +374,30 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/beanclerk/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/beanclerk/main)
 
 ## Description
 
 Beanclerk is an extension for [Beancount](https://github.com/beancount/beancount) (a useful tool for managing personal finance), automating some areas not addressed by Beancount itself, namely:
 
 1. [_Network downloads_](https://beancount.github.io/docs/importing_external_data.html#automating-network-downloads): As some financial institutions start to provide access to their services via APIs, it is more convenient and less error-prone to use them instead of a manual download and multi-step import process from CSV (or similar) reports. Compared to these reports, APIs usually have a stable specification and provide transaction IDs, making the importing process (e.g. checking for duplicates) much easier. Therefore, inspired by Beancount [Importer Protocol](https://beancount.github.io/docs/importing_external_data.html#writing-an-importer), Beanclerk proposes a simple [API Importer Protocol](https://github.com/peberanek/beanclerk/blob/main/beanclerk/importers/__init__.py) that aims to support any compatible API.
-2. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
+1. [_Automated categorization_](https://beancount.github.io/docs/importing_external_data.html#automatic-categorization): With growing number of new transactions, manual categorization quickly becomes repetitive, boring and therefore error-prone. So, why not to leave the hard part for machines and then just tweak the details?
     * As the first step, Beanclerk provides a way to define rules for automated categorization.
     * The future step is to augment it by machine-learning capabilities (e.g. via integration of the [Smart Importer](https://github.com/beancount/smart_importer)). (Btw, it might be also interesting to use machine-learning to discover hidden patterns or to provide predictions about our financial behavior.)
+1. _Automatic insertion of new transactions_: Beanclerk _appends_ new transactions to the Beancount input file (i.e. the ledger) defined in the configuration. It saves the step of doing this manually. (I don't care about the precise position of new transactions in the ledger because reporting tools like [Fava](https://github.com/beancount/fava) can sort them out anyway.) Consider to keep your ledger under a version control (e.g. via Git) to make any changes transparent and easy to review.
+
+**Beanclerk is still a rather 'rough' prototype.** You may encounter some unhandled exceptions and the API may change significantly in the future.
+
+**Beanclerk is currently tested on Linux only.**
 
 ### Existing importers
 
 Currently, there is 1 built-in importer for [Fio banka](https://www.fio.cz/). I plan to add another for [Banka Creditas](https://www.creditas.cz/), and, maybe, for some crypto exchanges. (All importers may move into separate repos in the future so the user may install only those they actually need).
 
 ### Notes
 
-I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. So it does not have to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or even solutions to the areas described above:
+I started Beanclerk primarily to try out some Python packages and to get better in software development by automating my daily workflow. Beanclerk does not aspire to be super inovative or unique. Actually, there are a couple of interesting projects of similar sort, which may provide inspiration or alternative solutions to the areas described above:
 
 * [beancount-import](https://github.com/jbms/beancount-import): Web UI for semi-automatically importing external data into beancount.
 * [finance-dl](https://github.com/jbms/finance-dl): Tools for automatically downloading/scraping personal financial data.
 * [beancount_reds_importers](https://github.com/redstreet/beancount_reds_importers): Simple ingesting tools for Beancount (plain text, double entry accounting software). More importantly, a framework to allow you to easily write your own importers.
 * [smart_importer](https://github.com/beancount/smart_importer): Augment Beancount importers with machine learning functionality.
 * [autobean](https://github.com/SEIAROTg/autobean): A collection of plugins and scripts that help automating bookkeeping with beancount.
 
@@ -410,36 +415,79 @@
 ```
 
 Confirm successful installation by running:
 ```
 bean-clerk -h
 ```
 
-## Usage (work in progress)
+## Usage
 
 ### Configuration
 
-Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory, or a path to the config file may be set by the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
+Beanclerk needs a configuration file. By default, it searches for `beanclerk-config.yml` in the current working directory. Or, set a path to the config file via the `-c` (or `--config-file`) option. For the latest example of a config file, see [`tests/beanclerk-config.yml`](tests/beanclerk-config.yml).
 
 ### Running the import
 
 Beanclerk currently implements a single command `import`. When running it for the first time, it is necessary to use at least the `--from-date` option to set the date to start the import from. (At the moment, Beanclerk runs import for all configured accounts.)
 
 ```
 bean-clerk import --from-date 2023-01-01
 ```
 
+Once Beanclerk encounters a transaction without a matching categorization rule, it prompts the user to resolve the situation:
+
+```
+...
+No categorization rule matches the following transaction:
+Transaction(
+    meta={
+        'id': '10000000002',
+        'account_id': '2345678901',
+        'account_name': 'Pavel, Žák',
+        'bank_id': '2010',
+        'bank_name': 'Fio banka, a.s.',
+        'type': 'Příjem převodem uvnitř banky',
+        'specification': 'test specification',
+        'bic': 'TESTBICXXXX',
+        'order_id': '30000000002',
+        'payer_reference': 'test payer reference'
+    },
+    date=datetime.date(2023, 1, 3),
+    flag='*',
+    payee=None,
+    narration='',
+    tags=frozenset(),
+    links=frozenset(),
+    postings=[
+        Posting(
+            account='Assets:Banks:Fio:Checking',
+            units=500.0 CZK,
+            cost=None,
+            price=None,
+            flag=None,
+            meta={}
+        )
+    ]
+)
+Available actions:
+'r': reload config (you should add a new rule first)
+'i': import as-is (transaction remains unbalanced)
+...
+```
+
 ## Contributing
 
-Set up a development environment:
+Contributions are welcome. Make sure to create an issue first so we can discuss it.
+
+Set up a development environment for playing with the source code:
 ```bash
 ./build_venv
 source venv/bin/activate
 pre-commit install  # https://pre-commit.com/
 ```
 
-Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
-
 Run tests:
 ```bash
 pytest
 ```
+
+Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `beanclerk-0.0.4/pyproject.toml` & `beanclerk-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=61.0", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beanclerk"
-version = "0.0.4"
+dynamic = ["version"]
 authors = [{ name = "Petr Beranek", email = "petrberanek.mail@gmail.com" }]
 license = { file = "LICENSE" }
 description = "Automation for Beancount"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["accounting", "finance", "beancount", "automation", "API"]
 classifiers = [
@@ -36,14 +36,16 @@
 
 [project.optional-dependencies]
 devel = ["pre-commit~=3.3", "pytest~=7.4"]
 
 [project.scripts]
 bean-clerk = "beanclerk.cli:cli"
 
+[tool.setuptools_scm]
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 # TODO: Use https://docs.pydantic.dev/dev-v2/integrations/mypy/
 [tool.mypy]
 ignore_missing_imports = true
 
@@ -51,14 +53,15 @@
 # https://beta.ruff.rs/docs/rules/
 select = [
   "F",   # pyflakes
   "E",   # pycodestyle
   "C90", # mccabe
   "I",   # isort
   "N",   # pep8-naming
+  "D",   # pydocstyle
   "UP",  # pyupgrade
   "YTT", # flake8-2020
   "S",   # flake8-bandit
   "BLE", # flake8-blind-except
   "FBT", # flake8-boolean-trap
   "B",   # flake8-bugbear
   "A",   # flake8-builtins
@@ -88,13 +91,17 @@
   # These may break temporarily commented-out code
   "F401",
   "F841",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = [
+  "D",
   "S",
   "ARG001", # pytest fixtures and mock functions often violate this
 ]
 
 [tool.ruff.pylint]
 max-args = 7
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `beanclerk-0.0.4/tests/test_clerk.py` & `beanclerk-0.0.5/tests/test_clerk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests of the clerk module.
 
-TODO:
+Todo:
     * Some tests are rather incomplete or a mess (mostly sanity only;
     multiple tests, share the same test data). Improve them.
     * Test fn append_entry_to_file.
 """
 from datetime import date
 from decimal import Decimal
 from pathlib import Path
```

### Comparing `beanclerk-0.0.4/tests/test_config.py` & `beanclerk-0.0.5/tests/test_config.py`

 * *Files identical despite different names*

