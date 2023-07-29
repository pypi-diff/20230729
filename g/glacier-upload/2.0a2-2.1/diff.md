# Comparing `tmp/glacier_upload-2.0a2.tar.gz` & `tmp/glacier_upload-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier_upload-2.0a2.tar", max compression
+gzip compressed data, was "glacier_upload-2.1.tar", max compression
```

## Comparing `glacier_upload-2.0a2.tar` & `glacier_upload-2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35141 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/LICENSE
--rw-r--r--   0        0        0     4463 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/README.md
--rw-r--r--   0        0        0     1244 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/src/glacier_upload/__init__.py
--rw-r--r--   0        0        0     3546 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/src/glacier_upload/archives.py
--rw-r--r--   0        0        0     4869 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/src/glacier_upload/cli.py
--rw-r--r--   0        0        0     2417 2023-01-22 12:13:31.849411 glacier_upload-2.0a2/src/glacier_upload/inventories.py
--rw-r--r--   0        0        0     9828 2023-01-22 12:13:31.853412 glacier_upload-2.0a2/src/glacier_upload/upload.py
--rw-r--r--   0        0        0     1604 2023-01-22 12:13:31.853412 glacier_upload-2.0a2/src/glacier_upload/utils/tree_hash.py
--rw-r--r--   0        0        0     5517 1970-01-01 00:00:00.000000 glacier_upload-2.0a2/setup.py
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 glacier_upload-2.0a2/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-07-29 02:58:46.590072 glacier_upload-2.1/LICENSE
+-rw-r--r--   0        0        0     4642 2023-07-29 02:58:46.590072 glacier_upload-2.1/README.md
+-rw-r--r--   0        0        0     1234 2023-07-29 02:58:46.590072 glacier_upload-2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 02:58:46.590072 glacier_upload-2.1/src/glacier_upload/__init__.py
+-rw-r--r--   0        0        0     7105 2023-07-29 02:58:46.590072 glacier_upload-2.1/src/glacier_upload/archives.py
+-rw-r--r--   0        0        0     5027 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/cli.py
+-rw-r--r--   0        0        0     2417 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/inventories.py
+-rw-r--r--   0        0        0     9783 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/upload.py
+-rw-r--r--   0        0        0     1604 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/utils/tree_hash.py
+-rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 glacier_upload-2.1/setup.py
+-rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 glacier_upload-2.1/PKG-INFO
```

### Comparing `glacier_upload-2.0a2/LICENSE` & `glacier_upload-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.0a2/README.md` & `glacier_upload-2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)
 [![License-GPLv3](https://img.shields.io/github/license/tbumi/glacier-upload)](https://github.com/tbumi/glacier-upload/blob/main/LICENSE)
 
 A helper tool to upload and manage archives in
 [Amazon S3 Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html)
 Vaults. Amazon S3 Glacier is a cloud storage service that is optimized for long
-term storage for a relatively cheap price.
+term storage for a relatively cheap price. NOT to be confused with Amazon S3
+with Glacier (Instant Retrieval, Flexible Retrieval, and Deep Archive) tier
+storage, which uses the S3 API and does not deal with vaults and archives.
 
 ## Installation
 
 Minimum required Python version is 3.9. To install, run this in your terminal:
 
 ```
 $ pip install glacier_upload
@@ -19,17 +21,17 @@
 
 ## Usage
 
 ### Prerequisites
 
 To upload an archive to Amazon S3 Glacier vault, ensure you have:
 
--   Created an AWS account
--   Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management
-    Console
+- Created an AWS account
+- Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management
+  Console
 
 ### Uploading an archive
 
 An upload can be performed by running `glacier upload` followed by the vault
 name and the file name(s) that you want to upload.
 
 ```
```

### Comparing `glacier_upload-2.0a2/pyproject.toml` & `glacier_upload-2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glacier-upload"
-version = "2.0a2"
+version = "2.1"
 description = "A helper tool to upload and manage archives in AWS Glacier Vaults"
 authors = ["Trapsilo Bumi <tbumi@thpd.io>"]
 license = "GPL-3.0+"
 readme = "README.md"
 packages = [{include = "glacier_upload", from = "src"}]
 repository = "https://github.com/tbumi/glacier-upload"
 keywords = ["AWS", "glacier", "upload", "multipart"]
@@ -20,23 +20,22 @@
     "Topic :: System :: Archiving :: Compression",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.47"
 click = "^8.1.3"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<24.0"
 flake8 = "^6.0.0"
-mypy = "^0.991"
+mypy = ">=0.991,<1.4"
 isort = "^5.11.4"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pre-commit = "^2.21.0"
+pre-commit = ">=2.21,<4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 glacier = "glacier_upload.cli:glacier_cli"
```

### Comparing `glacier_upload-2.0a2/src/glacier_upload/cli.py` & `glacier_upload-2.1/src/glacier_upload/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,26 +117,33 @@
     Initiate or get an archive retrieval job.
     """
     pass
 
 
 @archive_group.command(name="init-retrieval")
 @click.option("-d", "--description", help="Description of this job")
+@click.option(
+    "-t",
+    "--tier",
+    help="Retrieval tier (Expedited, Standard, or Bulk)",
+    default="Standard",
+    show_default=True,
+)
 @click.argument("vault_name")
 @click.argument("archive_id")
-def init_archive_retrieval(vault_name, archive_id, description):
+def init_archive_retrieval(vault_name, archive_id, description, tier):
     """
     Initiate retrieval for the archive designated by ARCHIVE_ID in VAULT_NAME.
 
     To retrieve an archive from glacier, use this function. Because of the
     way archives are stored in glacier, it will take some time to retrieve
     the archive. To check the status and retrieve the archive, run
     glacier-get-archive with the vault name and job ID returned by this function.
     """
-    return archives.init_retrieval(vault_name, archive_id, description)
+    return archives.init_retrieval(vault_name, archive_id, description, tier)
 
 
 @archive_group.command(name="get")
 @click.argument("vault_name")
 @click.argument("job_id")
 @click.argument(
     "file_name",
```

### Comparing `glacier_upload-2.0a2/src/glacier_upload/inventories.py` & `glacier_upload-2.1/src/glacier_upload/inventories.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.0a2/src/glacier_upload/upload.py` & `glacier_upload-2.1/src/glacier_upload/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import tarfile
 import tempfile
 import threading
 import traceback
 
 import boto3
 import click
+from tqdm import tqdm
 
 from .utils.tree_hash import calculate_total_tree_hash, calculate_tree_hash
 
 SINGLE_UPLOAD_THRESHOLD_BYTES = 100 * 1024 * 1024  # 100 MB
 MAX_UPLOAD_ATTEMPTS = 10  # 10 retries for each part before failing
 
 # ref: https://docs.aws.amazon.com/amazonglacier/latest/dev/uploading-archive-mpu.html
@@ -151,23 +152,22 @@
         try:
             paginator = glacier.get_paginator("list_parts")
             response = paginator.paginate(vaultName=vault_name, uploadId=upload_id)
             parts = list(response.search("Parts"))
         except glacier.exceptions.ResourceNotFoundException as e:
             raise click.ClickException(e.response["Error"]["Message"])
 
-        with click.progressbar(parts, label="Verifying uploaded parts") as bar:
-            for part_data in bar:
-                byte_start = int(part_data["RangeInBytes"].partition("-")[0])
-                file_to_upload.seek(byte_start)
-                part = file_to_upload.read(part_size_bytes)
-                checksum = calculate_tree_hash(part, part_size_bytes)
+        for part_data in tqdm(parts, desc="Verifying uploaded parts"):
+            byte_start = int(part_data["RangeInBytes"].partition("-")[0])
+            file_to_upload.seek(byte_start)
+            part = file_to_upload.read(part_size_bytes)
+            checksum = calculate_tree_hash(part, part_size_bytes)
 
-                if checksum == part_data["SHA256TreeHash"]:
-                    part_list[byte_start] = checksum
+            if checksum == part_data["SHA256TreeHash"]:
+                part_list[byte_start] = checksum
 
     click.echo("Spawning threads...")
     with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
         fileblock = threading.Lock()
         futures_list = {}
         for byte_pos in [
             part for part, checksum in part_list.items() if checksum is None
```

### Comparing `glacier_upload-2.0a2/src/glacier_upload/utils/tree_hash.py` & `glacier_upload-2.1/src/glacier_upload/utils/tree_hash.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.0a2/setup.py` & `glacier_upload-2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 packages = \
 ['glacier_upload', 'glacier_upload.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.26.47,<2.0.0', 'click>=8.1.3,<9.0.0']
+['boto3>=1.26.47,<2.0.0', 'click>=8.1.3,<9.0.0', 'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['glacier = glacier_upload.cli:glacier_cli']}
 
 setup_kwargs = {
     'name': 'glacier-upload',
-    'version': '2.0a2',
+    'version': '2.1',
     'description': 'A helper tool to upload and manage archives in AWS Glacier Vaults',
-    'long_description': '# glacier-upload\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)\n[![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)\n[![License-GPLv3](https://img.shields.io/github/license/tbumi/glacier-upload)](https://github.com/tbumi/glacier-upload/blob/main/LICENSE)\n\nA helper tool to upload and manage archives in\n[Amazon S3 Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html)\nVaults. Amazon S3 Glacier is a cloud storage service that is optimized for long\nterm storage for a relatively cheap price.\n\n## Installation\n\nMinimum required Python version is 3.9. To install, run this in your terminal:\n\n```\n$ pip install glacier_upload\n```\n\n## Usage\n\n### Prerequisites\n\nTo upload an archive to Amazon S3 Glacier vault, ensure you have:\n\n-   Created an AWS account\n-   Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management\n    Console\n\n### Uploading an archive\n\nAn upload can be performed by running `glacier upload` followed by the vault\nname and the file name(s) that you want to upload.\n\n```\nglacier upload VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n`FILE_NAME` can be one or more files or directories.\n\nThe script will:\n\n1. Read the file(s)\n2. Consolidate them into a `.tar.xz` archive if multiple `FILE_NAME`s are\n   specified or `FILE_NAME` is one or more directories\n3. Upload the file in one go if the file is less than 100 MB in size, or\n4. Split the file into chunks\n5. Spawn a number of threads that will upload the chunks in parallel. Note that\n   it will not read the entire file into memory, but only parts of the file as\n   it processes the chunks.\n6. Return the archive ID when complete. Consider saving this archive ID in a\n   safe place for retrieval purposes, because Amazon Glacier does not provide a\n   list of archives in realtime. See the "Requesting an inventory" section below\n   for details.\n\nThere are additional options to customize your upload, such as adding a\ndescription to the archive or configuring the number of threads or the size of\nparts. Run `glacier upload --help` for more information.\n\nIf a multipart upload is interrupted in the middle (because of an exception,\ninterrupted manually, or other reason), the script will show you the upload ID.\nThat upload ID can be used to resume the upload, using the same command but\nadding the `--upload-id` option, like so:\n\n```\nglacier upload --upload-id UPLOAD_ID VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n### Retrieving an archive\n\nRetrieving an archive in glacier requires two steps. First, initiate a\n"retrieval job" using:\n\n```\nglacier archive init-retrieval VAULT_NAME ARCHIVE_ID\n```\n\nTo see a list of archive IDs in a vault, see "Requesting an inventory" below.\n\nThen, the retrieval job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the archive if it has been\ncompleted.\n\n```\nglacier archive get VAULT_NAME JOB_ID FILE_NAME\n```\n\n### Requesting an inventory\n\nVaults do not provide realtime access to a list of their contents. To know what\na vault contains, you need to request an inventory of the archive, in a similar\nmanner to retrieving an archive. To initiate an inventory, run:\n\n```\nglacier inventory init-retrieval VAULT_NAME\n```\n\nThen, the inventory job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the inventory if it has been\ncompleted.\n\n```\nglacier inventory get VAULT_NAME JOB_ID\n```\n\n### Deleting an archive, deleting an upload job, creating/deleting a vault, etc.\n\nAll jobs other than uploading an archive and requesting/downloading an inventory\nor archive can be done using the AWS CLI. Those functionalities are not\nimplemented here to avoid duplication of work, and minimize maintenance efforts\nof this package.\n\n## Contributing\n\nContributions and/or bug fixes are welcome! Just make sure you\'ve read the below\nrequirements, then feel free to fork, make a topic branch, make your changes,\nand submit a PR.\n\n### Development Requirements\n\nBefore committing to this repo, install [poetry](https://python-poetry.org/) on\nyour local machine, then run these commands to setup your environment:\n\n```sh\npoetry install\npre-commit install\n```\n\nAll code is formatted with [black](https://github.com/psf/black). Consider\ninstalling an integration for it in your favourite text editor.\n',
+    'long_description': '# glacier-upload\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)\n[![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)\n[![License-GPLv3](https://img.shields.io/github/license/tbumi/glacier-upload)](https://github.com/tbumi/glacier-upload/blob/main/LICENSE)\n\nA helper tool to upload and manage archives in\n[Amazon S3 Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html)\nVaults. Amazon S3 Glacier is a cloud storage service that is optimized for long\nterm storage for a relatively cheap price. NOT to be confused with Amazon S3\nwith Glacier (Instant Retrieval, Flexible Retrieval, and Deep Archive) tier\nstorage, which uses the S3 API and does not deal with vaults and archives.\n\n## Installation\n\nMinimum required Python version is 3.9. To install, run this in your terminal:\n\n```\n$ pip install glacier_upload\n```\n\n## Usage\n\n### Prerequisites\n\nTo upload an archive to Amazon S3 Glacier vault, ensure you have:\n\n- Created an AWS account\n- Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management\n  Console\n\n### Uploading an archive\n\nAn upload can be performed by running `glacier upload` followed by the vault\nname and the file name(s) that you want to upload.\n\n```\nglacier upload VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n`FILE_NAME` can be one or more files or directories.\n\nThe script will:\n\n1. Read the file(s)\n2. Consolidate them into a `.tar.xz` archive if multiple `FILE_NAME`s are\n   specified or `FILE_NAME` is one or more directories\n3. Upload the file in one go if the file is less than 100 MB in size, or\n4. Split the file into chunks\n5. Spawn a number of threads that will upload the chunks in parallel. Note that\n   it will not read the entire file into memory, but only parts of the file as\n   it processes the chunks.\n6. Return the archive ID when complete. Consider saving this archive ID in a\n   safe place for retrieval purposes, because Amazon Glacier does not provide a\n   list of archives in realtime. See the "Requesting an inventory" section below\n   for details.\n\nThere are additional options to customize your upload, such as adding a\ndescription to the archive or configuring the number of threads or the size of\nparts. Run `glacier upload --help` for more information.\n\nIf a multipart upload is interrupted in the middle (because of an exception,\ninterrupted manually, or other reason), the script will show you the upload ID.\nThat upload ID can be used to resume the upload, using the same command but\nadding the `--upload-id` option, like so:\n\n```\nglacier upload --upload-id UPLOAD_ID VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n### Retrieving an archive\n\nRetrieving an archive in glacier requires two steps. First, initiate a\n"retrieval job" using:\n\n```\nglacier archive init-retrieval VAULT_NAME ARCHIVE_ID\n```\n\nTo see a list of archive IDs in a vault, see "Requesting an inventory" below.\n\nThen, the retrieval job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the archive if it has been\ncompleted.\n\n```\nglacier archive get VAULT_NAME JOB_ID FILE_NAME\n```\n\n### Requesting an inventory\n\nVaults do not provide realtime access to a list of their contents. To know what\na vault contains, you need to request an inventory of the archive, in a similar\nmanner to retrieving an archive. To initiate an inventory, run:\n\n```\nglacier inventory init-retrieval VAULT_NAME\n```\n\nThen, the inventory job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the inventory if it has been\ncompleted.\n\n```\nglacier inventory get VAULT_NAME JOB_ID\n```\n\n### Deleting an archive, deleting an upload job, creating/deleting a vault, etc.\n\nAll jobs other than uploading an archive and requesting/downloading an inventory\nor archive can be done using the AWS CLI. Those functionalities are not\nimplemented here to avoid duplication of work, and minimize maintenance efforts\nof this package.\n\n## Contributing\n\nContributions and/or bug fixes are welcome! Just make sure you\'ve read the below\nrequirements, then feel free to fork, make a topic branch, make your changes,\nand submit a PR.\n\n### Development Requirements\n\nBefore committing to this repo, install [poetry](https://python-poetry.org/) on\nyour local machine, then run these commands to setup your environment:\n\n```sh\npoetry install\npre-commit install\n```\n\nAll code is formatted with [black](https://github.com/psf/black). Consider\ninstalling an integration for it in your favourite text editor.\n',
     'author': 'Trapsilo Bumi',
     'author_email': 'tbumi@thpd.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tbumi/glacier-upload',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `glacier_upload-2.0a2/PKG-INFO` & `glacier_upload-2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glacier-upload
-Version: 2.0a2
+Version: 2.1
 Summary: A helper tool to upload and manage archives in AWS Glacier Vaults
 Home-page: https://github.com/tbumi/glacier-upload
 License: GPL-3.0+
 Keywords: AWS,glacier,upload,multipart
 Author: Trapsilo Bumi
 Author-email: tbumi@thpd.io
 Requires-Python: >=3.9,<4.0
@@ -20,27 +20,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Dist: boto3 (>=1.26.47,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/tbumi/glacier-upload
 Description-Content-Type: text/markdown
 
 # glacier-upload
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)
 [![License-GPLv3](https://img.shields.io/github/license/tbumi/glacier-upload)](https://github.com/tbumi/glacier-upload/blob/main/LICENSE)
 
 A helper tool to upload and manage archives in
 [Amazon S3 Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html)
 Vaults. Amazon S3 Glacier is a cloud storage service that is optimized for long
-term storage for a relatively cheap price.
+term storage for a relatively cheap price. NOT to be confused with Amazon S3
+with Glacier (Instant Retrieval, Flexible Retrieval, and Deep Archive) tier
+storage, which uses the S3 API and does not deal with vaults and archives.
 
 ## Installation
 
 Minimum required Python version is 3.9. To install, run this in your terminal:
 
 ```
 $ pip install glacier_upload
@@ -48,17 +51,17 @@
 
 ## Usage
 
 ### Prerequisites
 
 To upload an archive to Amazon S3 Glacier vault, ensure you have:
 
--   Created an AWS account
--   Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management
-    Console
+- Created an AWS account
+- Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management
+  Console
 
 ### Uploading an archive
 
 An upload can be performed by running `glacier upload` followed by the vault
 name and the file name(s) that you want to upload.
 
 ```
```

