# Comparing `tmp/SeedrClient-0.1.2.tar.gz` & `tmp/SeedrClient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeedrClient-0.1.2.tar", last modified: Fri Jul 28 10:54:01 2023, max compression
+gzip compressed data, was "SeedrClient-0.1.3.tar", last modified: Sat Jul 29 12:16:26 2023, max compression
```

## Comparing `SeedrClient-0.1.2.tar` & `SeedrClient-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/SeedrClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/seedr_client/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/seedr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/SeedrClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 12:16:26.000000 SeedrClient-0.1.3/src/SeedrClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:16:26.087308 SeedrClient-0.1.3/src/seedr_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-29 12:16:05.000000 SeedrClient-0.1.3/src/seedr_client/seedr_handler.py
```

### Comparing `SeedrClient-0.1.2/setup.py` & `SeedrClient-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.2/src/seedr_client/seedr_handler.py` & `SeedrClient-0.1.3/src/seedr_client/seedr_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,27 @@
 from torrentool.api import Torrent
 from .errors import (
     InvalidLogin,
     InvalidToken,
     LoginRequired,
     InvalidTorrent,
     DriveLimit,
-    BadLeeching
+    BadLeeching,
 )
 
 
 class SeedrHandler:
-    def __init__(self, email=None, password=None, access_token=None, aria2c_secret=None, download_directory="."):
+    def __init__(
+        self,
+        email=None,
+        password=None,
+        access_token=None,
+        aria2c_secret=None,
+        download_directory=".",
+    ):
         self.rate_limit = 1
         self.email = email
         self.password = password
         self.access_token = access_token
         self.base_folder_url = "https://www.seedr.cc/api/folder"
         self.base_oauth_url = "https://www.seedr.cc/oauth_test"
         # This is the list of file types Seedr client is not allowed to download,
@@ -40,28 +47,31 @@
         self.aria2 = None
         self.aria2c_secret = aria2c_secret
         self.seedr_download_options = {"user_agent": "Mozilla/5.0"}
         self.download_directory = download_directory
 
     @staticmethod
     def contains_bad_token(response_text):
-        return any(fail_resp in response_text for fail_resp in ["invalid_token", "expired_token"])
+        return any(
+            fail_resp in response_text
+            for fail_resp in ["invalid_token", "expired_token"]
+        )
 
     @staticmethod
     def bytes_to_mb_gb(byte):
         """
         A simple function that converts Bytes to Megabytes if value
         is less than 1 Gigabyte else returns value in Gigabytes
 
         :param byte: The value in Bytes to be converted
         :type byte: int
         :return: The converted value in MB or GB based on logic
         :rtype: str
         """
-        mb = byte / (1024 ** 2)
+        mb = byte / (1024**2)
         if mb >= 1024:
             gb = mb / 1024
             return f"{round(gb, 2)} GB"
         return f"{round(mb, 2)} MB"
 
     def list_contents(self, response_json):
         """
@@ -73,25 +83,27 @@
         :rtype: dict
         """
         content = {
             "folders": [
                 {
                     "folder_id": folder["id"],
                     "folder_name": folder["name"],
-                    "size": self.bytes_to_mb_gb(folder["size"])
-                } for folder in response_json["folders"]
+                    "size": self.bytes_to_mb_gb(folder["size"]),
+                }
+                for folder in response_json["folders"]
             ],
             "files": [
                 {
                     "folder_file_id": file["folder_file_id"],
                     "file_name": file["name"],
                     "size": self.bytes_to_mb_gb(file["size"]),
-                    "folder_path": response_json["fullname"]
-                } for file in response_json["files"]
-            ]
+                    "folder_path": response_json["fullname"],
+                }
+                for file in response_json["files"]
+            ],
         }
         return content
 
     @staticmethod
     def is_op_success(response_text):
         """
         Checks if there is a success code in the response provided by the api call and returns the appropriate boolean
@@ -108,29 +120,31 @@
     def is_login_success(self):
         """
         Checks if the access token is valid
 
         :return: Returns True if the token is valid, False if it isn't
         :rtype: bool
         """
-        response = requests.get(f"{self.base_folder_url}?access_token={self.access_token}")
+        response = requests.get(
+            f"{self.base_folder_url}?access_token={self.access_token}"
+        )
         if self.contains_bad_token(response_text=response.text):
             return False
         else:
             return True
 
     def is_request_failed(self, response_text, requested_on):
         """
         Checks for any failed codes in the response and if there is any, then it raises
         the appropriate error code with detail, else returns false
 
         :param response_text: The text response received by Seedr api to the request made by the previous method
         :type response_text: str
         :param requested_on: A string that is either "file" or "folder" based on what kinda file system operations was
-        going on in the previous method
+            going on in the previous method
         :type requested_on: str
         :return: Returns False if no fail code
         :rtype: bool
         """
         if "access_denied" in response_text:
             # TODO add a way to notify when this happens
             raise FileNotFoundError(f"{requested_on.title()} not found in drive")
@@ -148,15 +162,15 @@
         """
         if self.email and self.password:
             data = {
                 "grant_type": "password",
                 "client_id": "seedr_chrome",
                 "type": "login",
                 "username": self.email,
-                "password": self.password
+                "password": self.password,
             }
             response = requests.post(f"{self.base_oauth_url}/token.php", data=data)
             if "access_token" in response.text:
                 self.access_token = json.loads(response.text)["access_token"]
             else:
                 # TODO add a way to notify when this happens
                 raise InvalidLogin("Invalid username and password combination.")
@@ -171,37 +185,42 @@
     def get_drive(self):
         """
         Gets details about the drive's space, active torrents, and all downloaded files and folders
         Note: This is the same as the get_folder method except seedr api does not ask for a folder id,
         additionally we are able top display a few additional details, including active torrents
 
         :return: A dictionary containing, available and used drive space, active torrents and its details, downloaded
-        folders and files and their details
+            folders and files and their details
         :rtype: dict
         """
-        response = requests.get(f"{self.base_folder_url}?access_token={self.access_token}")
+        response = requests.get(
+            f"{self.base_folder_url}?access_token={self.access_token}"
+        )
         if self.contains_bad_token(response_text=response.text):
             # TODO add a way to notify when this happens
             raise InvalidToken("Invalid/Expired access token.")
         else:
             response_json = json.loads(response.text)
             drive = {
                 "space": {
                     "total": self.bytes_to_mb_gb(response_json["space_max"]),
-                    "used": self.bytes_to_mb_gb(response_json["space_used"])
+                    "used": self.bytes_to_mb_gb(response_json["space_used"]),
                 },
-                "parent_folder_id": response_json["folder_id"] if response_json["parent"] == -1 else None,
+                "parent_folder_id": response_json["folder_id"]
+                if response_json["parent"] == -1
+                else None,
                 "torrents": [
                     {
                         "name": torrent["name"],
                         "torrent_id": torrent["id"],
                         "progress": torrent["progress"],
-                        "progress_url": torrent["progress_url"]
-                    } for torrent in response_json["torrents"]
-                ]
+                        "progress_url": torrent["progress_url"],
+                    }
+                    for torrent in response_json["torrents"]
+                ],
             }
             drive = drive | self.list_contents(response_json=response_json)
             self.drive_size = response_json["space_max"]
             return drive
 
     def get_folder(self, folder_id):
         """
@@ -209,109 +228,124 @@
         the folder id that is passed if it exists
 
         :param folder_id: The unique id associated with the folder that you need the info about
         :type folder_id: int
         :return: A dictionary contains a list of all files and folders in the associated folder
         :rtype: dict
         """
-        response = requests.get(f"{self.base_folder_url}/{str(folder_id)}?access_token={self.access_token}")
+        response = requests.get(
+            f"{self.base_folder_url}/{str(folder_id)}?access_token={self.access_token}"
+        )
         response_text = response.text
-        if not self.is_request_failed(response_text=response_text, requested_on="folder"):
+        if not self.is_request_failed(
+            response_text=response_text, requested_on="folder"
+        ):
             response_json = json.loads(response_text)
             if folder_id == response_json["folder_id"]:
-                folder = {
-                    "folder_name": response_json["fullname"]
-                }
+                folder = {"folder_name": response_json["fullname"]}
                 folder = folder | self.list_contents(response_json=response_json)
                 return folder
             else:
                 # TODO add a way to notify when this happens
-                raise LookupError("Provided folder id does not match the received folder id")
+                raise LookupError(
+                    "Provided folder id does not match the received folder id"
+                )
 
     def get_file(self, folder_file_id):
         """
         This method returns the name and the download url associated with the file id that is passed
 
         :param folder_file_id: The unique id associated with the file you need the info about
         :type folder_file_id: int
         :return: A dictionary containing file name and download url
         :rtype: dict
         """
-        data = {"access_token": self.access_token, "func": "fetch_file", "folder_file_id": str(folder_file_id)}
+        data = {
+            "access_token": self.access_token,
+            "func": "fetch_file",
+            "folder_file_id": str(folder_file_id),
+        }
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_text = response.text
         if not self.is_request_failed(response_text=response_text, requested_on="file"):
             response_json = json.loads(response_text)
-            file = {
-                "name": response_json["name"],
-                "download_url": response_json["url"]
-            }
+            file = {"name": response_json["name"], "download_url": response_json["url"]}
             return file
 
     def add_torrent(self, torrent=None, wishlist_id=None, folder_id=-1):
         """
         This function allows you to pass either torrent file or magnet uri or a wishlist id, to start downloading
-        by Seedr. It returns the name and ID of the torrent on success.
+        by Seedr.
 
         Note: If magnet uri is passed instead of a torrent file which is the preferred method, and if the peers in the
         torrent is lower than 3 or if the torrent is completely dead then this function might not be able to add the
         torrent due to the underlying logic which requires the meta info of the torrent. This is a drawback of this
         approach as this helps avoid wasting time checking if there is enough storage space, but can't use the Seedr's
         cache, which works even if there is no seeders. If there is enough requests to correct this approach I will add
         a timeout logic to the method in next iteration. For now try supplying torrents file instead of the magnet uri.
 
         :param torrent: The torrent file or magnet uri that you want to add to be leeched/downloaded
         :type torrent: str
         :param wishlist_id: The wishlist id that you want to add from your Seedr wishlist
         :type wishlist_id: int
         :param folder_id: The folder you want the torrent to be downloaded to. Defaults to parent.
         :type folder_id: int
-        :return:
-        :rtype:
+        :return: If successful returns the name and ID of the torrent.
+        :rtype: dict
         """
         if torrent:
             if self.torrent_regex.match(torrent):
                 pass
             elif self.magnet_regex.match(torrent):
                 # TODO Add a timeout wrapper, which will jump right to adding the torrent instead
-                temp_torrent_file_path = os.path.join(tempfile.gettempdir(), f"temp{randrange(1, 10**4):04}.torrent")
-                subprocess.run(["ih2torrent", "--file", temp_torrent_file_path, torrent])
+                temp_torrent_file_path = os.path.join(
+                    tempfile.gettempdir(), f"temp{randrange(1, 10**4):04}.torrent"
+                )
+                subprocess.run(
+                    ["ih2torrent", "--file", temp_torrent_file_path, torrent]
+                )
                 torrent = temp_torrent_file_path
             else:
                 raise InvalidTorrent(
                     f"The torrent passed is invalid, please verify it fix it.\nTorrent/Magnet: {torrent}"
                 )
             torrent_info = Torrent.from_file(torrent)
             if self.drive_size >= torrent_info.total_size:
                 torrent_magnet_uri = torrent_info.magnet_link
             else:
                 print(self.drive_size, torrent_info.total_size)
-                raise DriveLimit("The torrent is larger than the total available space in the drive")
+                raise DriveLimit(
+                    "The torrent is larger than the total available space in the drive"
+                )
         elif wishlist_id:
             torrent_magnet_uri = None
         else:
-            raise TypeError("add_torrent() is missing an argument. At least one argument needs to be passed")
+            raise TypeError(
+                "add_torrent() is missing an argument. At least one argument needs to be passed"
+            )
 
         data = {
-            'access_token': self.access_token,
-            'func': 'add_torrent',
-            'torrent_magnet': torrent_magnet_uri,
-            'wishlist_id': wishlist_id,
-            'folder_id': folder_id
+            "access_token": self.access_token,
+            "func": "add_torrent",
+            "torrent_magnet": torrent_magnet_uri,
+            "wishlist_id": wishlist_id,
+            "folder_id": folder_id,
         }
 
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_json = json.loads(response.text)
         if response_json["result"]:
             return {
                 "torrent_id": response_json["user_torrent_id"],
-                "file_name": response_json["title"]
+                "file_name": response_json["title"],
             }
         else:
-            raise BadLeeching(f"The provided Torrent couldn't be leeched/downloaded to the drive.\n {data=}")
+            raise BadLeeching(
+                f"The provided Torrent couldn't be leeched/downloaded to the drive.\n {data=}"
+            )
 
     def download_folder(self, folder_id, builtin_downloader=True):
         content = self.get_folder(folder_id=folder_id)
         sleep(self.rate_limit)
         download_list = content["files"]
         next_list_folders = content["folders"]
         while True:
@@ -327,40 +361,42 @@
                 break
         # This loop checks if there is any file that matches the list of extensions that are to be excluded and if
         # present will remove them from the list
         temp_download_list = []
         for item in download_list:
             temp_item_ext = item["file_name"].split(".")[-1]
             if temp_item_ext not in self.exclude_file_type:
-                item["folder_path"] = os.path.join(self.download_directory, *item["folder_path"].split("/"), "")
+                item["folder_path"] = os.path.join(
+                    self.download_directory, *item["folder_path"].split("/"), ""
+                )
                 temp_download_list.append(item)
         download_list = temp_download_list
         for i in range(len(download_list)):
-            download_list[i]["download_url"] = self.get_file(download_list[i]["folder_file_id"])["download_url"]
+            download_list[i]["download_url"] = self.get_file(
+                download_list[i]["folder_file_id"]
+            )["download_url"]
             sleep(self.rate_limit)
         if not builtin_downloader:
             return download_list
         download_list = sorted(download_list, key=lambda d: d["size"])
         # Only runs if aria2p client hasn't already been initiated
         if not self.aria2:
             self.aria2 = aria2p.API(
                 aria2p.Client(
-                    host="http://localhost",
-                    port=6800,
-                    secret=self.aria2c_secret
+                    host="http://localhost", port=6800, secret=self.aria2c_secret
                 )
             )
         download_queue = []
         # Adds each url obtained from previous steps one by one with priorities given for smallest files first
         for i in range(len(download_list)):
             download_adder = self.aria2.add(
                 uri=download_list[i]["download_url"],
                 # TODO make the directory data dynamic, such that each file is downloaded to the appropriate folder
                 options={"dir": download_list[i]["folder_path"]},
-                position=i
+                position=i,
             )
             download_queue.append(download_adder[0].gid)
         while True:
             # TODO FUTURE show progress real time
             temp_download_queue = []
             for gid in download_queue:
                 download_info = self.aria2.get_download(gid=gid)
@@ -381,36 +417,38 @@
         :type folder_id: int
         :return: Returns True or False based on success
         :rtype: bool
         """
         data = {
             "access_token": self.access_token,
             "func": "delete",
-            "delete_arr": '[{"type":"folder","id":"' + str(folder_id) + '"}]'
+            "delete_arr": '[{"type":"folder","id":"' + str(folder_id) + '"}]',
         }
         # TODO Correct this stub to follow DRY
         # TODO add a conditional statement to prevent deletion of parent folder
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_text = response.text
-        if not self.is_request_failed(response_text=response_text, requested_on="folder"):
+        if not self.is_request_failed(
+            response_text=response_text, requested_on="folder"
+        ):
             return self.is_op_success(response_text=response_text)
 
     def delete_file(self, folder_file_id):
         """
         This method deletes the file associated with the id that is passed and returns True on success
 
         :param folder_file_id: The id of the file you wish to delete
         :type folder_file_id: int
         :return: Returns True or False based on success
         :rtype: bool
         """
         data = {
             "access_token": self.access_token,
             "func": "delete",
-            "delete_arr": '[{"type":"file","id":"' + str(folder_file_id) + '"}]'
+            "delete_arr": '[{"type":"file","id":"' + str(folder_file_id) + '"}]',
         }
         # TODO Correct this stub to follow DRY
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_text = response.text
         if not self.is_request_failed(response_text=response_text, requested_on="file"):
             return self.is_op_success(response_text=response_text)
 
@@ -420,21 +458,23 @@
 
         :param torrent_id: The id of the active torrent you wish to delete
         :type torrent_id: int
         :return: Returns True or False based on success
         :rtype: bool
         """
         data = {
-            'access_token': self.access_token,
-            'func': 'delete',
-            'delete_arr': f'[{{"type":"torrent","id":{torrent_id}}}]'
+            "access_token": self.access_token,
+            "func": "delete",
+            "delete_arr": f'[{{"type":"torrent","id":{torrent_id}}}]',
         }
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_text = response.text
-        if not self.is_request_failed(response_text=response_text, requested_on="torrent"):
+        if not self.is_request_failed(
+            response_text=response_text, requested_on="torrent"
+        ):
             return self.is_op_success(response_text=response_text)
 
     def delete_all(self):
         """
         This method deletes all the content within the drive, whether it downloaded
         to the drive or being downloaded.
```

