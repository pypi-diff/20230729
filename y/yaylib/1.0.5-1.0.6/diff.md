# Comparing `tmp/yaylib-1.0.5.tar.gz` & `tmp/yaylib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.5.tar", last modified: Sun Jul 23 06:21:11 2023, max compression
+gzip compressed data, was "yaylib-1.0.6.tar", last modified: Sat Jul 29 08:11:48 2023, max compression
```

## Comparing `yaylib-1.0.5.tar` & `yaylib-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 06:21:11.943815 yaylib-1.0.5/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    10828 2023-07-23 06:21:11.943815 yaylib-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9964 2023-07-18 08:52:45.000000 yaylib-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 06:21:11.945118 yaylib-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1584 2023-07-21 11:06:20.000000 yaylib-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 06:21:11.905046 yaylib-1.0.5/tests/
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.5/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-23 06:21:11.913358 yaylib-1.0.5/yaylib/
--rw-rw-rw-   0        0        0      664 2023-07-21 11:06:20.000000 yaylib-1.0.5/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 06:21:11.942810 yaylib-1.0.5/yaylib/api/
--rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.5/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10255 2023-07-19 13:28:39.000000 yaylib-1.0.5/yaylib/api/api.py
--rw-rw-rw-   0        0        0     9429 2023-07-23 06:18:02.000000 yaylib-1.0.5/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2699 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    15017 2023-07-21 11:06:20.000000 yaylib-1.0.5/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8224 2023-07-20 07:15:23.000000 yaylib-1.0.5/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33686 2023-07-22 09:13:37.000000 yaylib-1.0.5/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    23744 2023-07-19 12:23:37.000000 yaylib-1.0.5/yaylib/api/user.py
--rw-rw-rw-   0        0        0    86548 2023-07-21 11:06:20.000000 yaylib-1.0.5/yaylib/client.py
--rw-rw-rw-   0        0        0    19309 2023-07-23 06:21:04.000000 yaylib-1.0.5/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.5/yaylib/errors.py
--rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.5/yaylib/models.py
--rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.5/yaylib/responses.py
--rw-rw-rw-   0        0        0     4473 2023-07-20 07:15:24.000000 yaylib-1.0.5/yaylib/utils.py
--rw-rw-rw-   0        0        0     9374 2023-07-21 12:27:01.000000 yaylib-1.0.5/yaylib/websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-23 06:21:11.930194 yaylib-1.0.5/yaylib.egg-info/
--rw-rw-rw-   0        0        0    10828 2023-07-23 06:21:11.000000 yaylib-1.0.5/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-07-23 06:21:11.000000 yaylib-1.0.5/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 06:21:11.000000 yaylib-1.0.5/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-23 06:21:11.000000 yaylib-1.0.5/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-23 06:21:11.000000 yaylib-1.0.5/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.989841 yaylib-1.0.6/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0    12824 2023-07-29 08:11:48.988645 yaylib-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11961 2023-07-29 04:57:25.000000 yaylib-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:11:48.989841 yaylib-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-07-24 11:24:25.000000 yaylib-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.943778 yaylib-1.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:22:00.000000 yaylib-1.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-07-28 03:15:02.000000 yaylib-1.0.6/tests/config.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.6/tests/test_user.py
+-rw-rw-rw-   0        0        0     1908 2023-07-28 03:21:48.000000 yaylib-1.0.6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.951038 yaylib-1.0.6/yaylib/
+-rw-rw-rw-   0        0        0      668 2023-07-25 06:44:17.000000 yaylib-1.0.6/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.988645 yaylib-1.0.6/yaylib/api/
+-rw-rw-rw-   0        0        0      715 2023-07-25 06:44:11.000000 yaylib-1.0.6/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10523 2023-07-28 01:49:59.000000 yaylib-1.0.6/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9429 2023-07-23 06:18:02.000000 yaylib-1.0.6/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2713 2023-07-28 02:06:00.000000 yaylib-1.0.6/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14964 2023-07-29 04:53:58.000000 yaylib-1.0.6/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8347 2023-07-28 02:06:16.000000 yaylib-1.0.6/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33686 2023-07-22 09:13:37.000000 yaylib-1.0.6/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    23744 2023-07-19 12:23:37.000000 yaylib-1.0.6/yaylib/api/user.py
+-rw-rw-rw-   0        0        0     9409 2023-07-28 13:12:41.000000 yaylib-1.0.6/yaylib/api/websocket.py
+-rw-rw-rw-   0        0        0    86741 2023-07-29 04:54:07.000000 yaylib-1.0.6/yaylib/client.py
+-rw-rw-rw-   0        0        0    18801 2023-07-29 08:11:00.000000 yaylib-1.0.6/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.6/yaylib/errors.py
+-rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.6/yaylib/models.py
+-rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.6/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4649 2023-07-28 02:06:59.000000 yaylib-1.0.6/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:48.974284 yaylib-1.0.6/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    12824 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 08:11:48.000000 yaylib-1.0.6/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.5/LICENSE` & `yaylib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/PKG-INFO` & `yaylib-1.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: yaylib
-Version: 1.0.5
-Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
-Home-page: https://github.com/qvco/yaylib
-Download-URL: https://github.com/qvco/yaylib
-Author: Qvco, Konn
-Author-email: nikola.desuga@gmail.com
-Maintainer: Qvco, Konn
-Maintainer-email: nikola.desuga@gmail.com
-License: MIT
-Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
@@ -91,14 +73,63 @@
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
+### yaylib 利用で実現できること
+
+<table>
+    <tr>
+        <th>カテゴリ</th>
+        <th>「yaylib」で自動化できること</th>
+        <th>応用先</th>
+    </tr>
+    <tr>
+		<td>データ収集の効率化</td>
+		<td>
+            <li>投稿情報取得</li>
+            <li>ユーザー情報取得</li>
+            <li>人気のワード取得</li>
+            <li>フォロー/フォロワー情報取得</li>
+        </td>
+		<td>
+            <li>SNSデータマーケティング</li>
+            <li>トレンド解析</li>
+            <li>ニーズ調査</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(投稿関連)</td>
+		<td>
+            <li>投稿する</li>
+            <li>リツイートする</li>
+            <li>いいねする</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(ユーザー関連)</td>
+		<td>
+            <li>フォローする/フォロー解除する</li>
+            <li>ブロックする/ブロック解除する</li>
+            <li>ミュートする/ミュート解除する</li>
+            <li>DMを送る</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+</table>
+
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -113,18 +144,14 @@
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
 ```
 
-<p align="center">
-    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
-</p>
-
 #### ✨ 画像と一緒に投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -141,28 +168,32 @@
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post("Hello with yaylib!", in_reply_to=373189088)
+api.create_post(
+    "Hello with yaylib!",
+    in_reply_to=返信先の投稿ID,
+    mention_ids=[返信先のユーザーID]
+)
 ```
 
 #### ✨ タイムラインを 100 件取得する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
 timeline = api.get_timeline(number=100)
 
 for post in timeline.posts:
-    print(post.user.nickname)  # 投稿者
+    print(post.user.nickname)  # 投稿者名
     print(post.text)  # 本文
     print(post.likes_count)  # いいね数
     print(post.reposts_count)  # (´∀｀∩)↑age↑の数
     print(post.in_reply_to_post_count)  # 返信の数
 ```
 
 #### ✨ タイムラインをキーワードで検索して「いいね」する
@@ -193,14 +224,42 @@
 
 timeline = api.get_timeline(number=15)
 
 for post in timeline.posts:
     api.follow_user(post.user.id)
 ```
 
+#### ✨ リアルタイムでチャットを取得する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+
+class ChatBot(yaylib.ChatRoomEventHandler):
+
+    def on_request(self, total_count: int):
+        # チャットリクエストを承認する
+        chat_room = api.get_chat_requests(number=1).chat_rooms[0]
+        api.accept_chat_requests(chat_room_ids=[chat_room.id])
+        self.on_message(chat_room)
+
+    def on_message(self, chat_room):
+        # メッセージを出力する
+        print(chat_room.last_message.text)
+
+
+ws_token = api.get_web_socket_token()
+
+bot = ChatBot()
+bot.run(ws_token)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## :crown: yaylib で誕生したロボットたち
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.5 Summary: This Python package
-provides an easy-to-use interface for accessing data from Yay! (https://
-yay.space/). With this API Client, you can retrieve user profiles, posts,
-comments, and other content from Yay!, as well as perform common tasks like
-liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
-Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
-nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
-nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -42,47 +30,69 @@
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
-æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
+å©ç¨ã§å®ç¾ã§ãããã¨
+ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
+                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
+ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
+                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
+                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
+ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
+(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
+                               ããã­ãã
+                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
+ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
+(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
+                               DMãéã
+#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
+api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
+api.create_post("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-shared_url="https://github.com/qvco/yaylib") ```
-                            [Writing Text Threads]
-#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+shared_url="https://github.com/qvco/yaylib") ``` #### â¨
+ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
 ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
 ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
 attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
 import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
-password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
-```python import yaylib api = yaylib.Client() timeline = api.get_timeline
-(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
-print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
-(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
-(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+password="ãã¹ã¯ã¼ã") api.create_post( "Hello with yaylib!",
+in_reply_to=è¿ä¿¡åã®æç¨¿ID, mention_ids=[è¿ä¿¡åã®ã¦ã¼ã¶ã¼ID] )
+``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã ```python import yaylib
+api = yaylib.Client() timeline = api.get_timeline(number=100) for post in
+timeline.posts: print(post.user.nickname) # æç¨¿èå print(post.text) #
+æ¬æ print(post.likes_count) # ããã­æ° print(post.reposts_count) #
+(Â´âï½â©)âageâã®æ° print(post.in_reply_to_post_count) # è¿ä¿¡ã®æ°
+``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
 post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
-timeline.posts: api.follow_user(post.user.id) ```
+timeline.posts: api.follow_user(post.user.id) ``` #### â¨
+ãªã¢ã«ã¿ã¤ã ã§ãã£ãããåå¾ãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") class ChatBot(yaylib.ChatRoomEventHandler): def
+on_request(self, total_count: int): #
+ãã£ãããªã¯ã¨ã¹ããæ¿èªãã chat_room = api.get_chat_requests
+(number=1).chat_rooms[0] api.accept_chat_requests(chat_room_ids=[chat_room.id])
+self.on_message(chat_room) def on_message(self, chat_room): #
+ã¡ãã»ã¼ã¸ãåºåãã print(chat_room.last_message.text) ws_token =
+api.get_web_socket_token() bot = ChatBot() bot.run(ws_token) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
```

### Comparing `yaylib-1.0.5/README.md` & `yaylib-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: yaylib
+Version: 1.0.6
+Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
+Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib
+Author: Qvco, Konn
+Author-email: nikola.desuga@gmail.com
+Maintainer: Qvco, Konn
+Maintainer-email: nikola.desuga@gmail.com
+License: MIT
+Keywords: yay,yaylib,api,bot,tool,client,library,wrapper,ボット,ライブラリ,ツール
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
@@ -73,14 +91,63 @@
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
+### yaylib 利用で実現できること
+
+<table>
+    <tr>
+        <th>カテゴリ</th>
+        <th>「yaylib」で自動化できること</th>
+        <th>応用先</th>
+    </tr>
+    <tr>
+		<td>データ収集の効率化</td>
+		<td>
+            <li>投稿情報取得</li>
+            <li>ユーザー情報取得</li>
+            <li>人気のワード取得</li>
+            <li>フォロー/フォロワー情報取得</li>
+        </td>
+		<td>
+            <li>SNSデータマーケティング</li>
+            <li>トレンド解析</li>
+            <li>ニーズ調査</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(投稿関連)</td>
+		<td>
+            <li>投稿する</li>
+            <li>リツイートする</li>
+            <li>いいねする</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(ユーザー関連)</td>
+		<td>
+            <li>フォローする/フォロー解除する</li>
+            <li>ブロックする/ブロック解除する</li>
+            <li>ミュートする/ミュート解除する</li>
+            <li>DMを送る</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+</table>
+
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -95,18 +162,14 @@
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
 ```
 
-<p align="center">
-    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
-</p>
-
 #### ✨ 画像と一緒に投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -123,28 +186,32 @@
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post("Hello with yaylib!", in_reply_to=373189088)
+api.create_post(
+    "Hello with yaylib!",
+    in_reply_to=返信先の投稿ID,
+    mention_ids=[返信先のユーザーID]
+)
 ```
 
 #### ✨ タイムラインを 100 件取得する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
 timeline = api.get_timeline(number=100)
 
 for post in timeline.posts:
-    print(post.user.nickname)  # 投稿者
+    print(post.user.nickname)  # 投稿者名
     print(post.text)  # 本文
     print(post.likes_count)  # いいね数
     print(post.reposts_count)  # (´∀｀∩)↑age↑の数
     print(post.in_reply_to_post_count)  # 返信の数
 ```
 
 #### ✨ タイムラインをキーワードで検索して「いいね」する
@@ -175,14 +242,42 @@
 
 timeline = api.get_timeline(number=15)
 
 for post in timeline.posts:
     api.follow_user(post.user.id)
 ```
 
+#### ✨ リアルタイムでチャットを取得する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+
+class ChatBot(yaylib.ChatRoomEventHandler):
+
+    def on_request(self, total_count: int):
+        # チャットリクエストを承認する
+        chat_room = api.get_chat_requests(number=1).chat_rooms[0]
+        api.accept_chat_requests(chat_room_ids=[chat_room.id])
+        self.on_message(chat_room)
+
+    def on_message(self, chat_room):
+        # メッセージを出力する
+        print(chat_room.last_message.text)
+
+
+ws_token = api.get_web_socket_token()
+
+bot = ChatBot()
+bot.run(ws_token)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## :crown: yaylib で誕生したロボットたち
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.6 Summary:
+åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
+ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
+Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
+qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
+Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
+Keywords:
+yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -30,47 +41,69 @@
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
-æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
+å©ç¨ã§å®ç¾ã§ãããã¨
+ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
+                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
+ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
+                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
+                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
+ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
+(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
+                               ããã­ãã
+                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
+ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
+(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
+                               DMãéã
+#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
+api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
+api.create_post("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-shared_url="https://github.com/qvco/yaylib") ```
-                            [Writing Text Threads]
-#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+shared_url="https://github.com/qvco/yaylib") ``` #### â¨
+ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
 ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
 ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
 attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
 import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
-password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
-```python import yaylib api = yaylib.Client() timeline = api.get_timeline
-(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
-print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
-(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
-(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+password="ãã¹ã¯ã¼ã") api.create_post( "Hello with yaylib!",
+in_reply_to=è¿ä¿¡åã®æç¨¿ID, mention_ids=[è¿ä¿¡åã®ã¦ã¼ã¶ã¼ID] )
+``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã ```python import yaylib
+api = yaylib.Client() timeline = api.get_timeline(number=100) for post in
+timeline.posts: print(post.user.nickname) # æç¨¿èå print(post.text) #
+æ¬æ print(post.likes_count) # ããã­æ° print(post.reposts_count) #
+(Â´âï½â©)âageâã®æ° print(post.in_reply_to_post_count) # è¿ä¿¡ã®æ°
+``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
 post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
-timeline.posts: api.follow_user(post.user.id) ```
+timeline.posts: api.follow_user(post.user.id) ``` #### â¨
+ãªã¢ã«ã¿ã¤ã ã§ãã£ãããåå¾ãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") class ChatBot(yaylib.ChatRoomEventHandler): def
+on_request(self, total_count: int): #
+ãã£ãããªã¯ã¨ã¹ããæ¿èªãã chat_room = api.get_chat_requests
+(number=1).chat_rooms[0] api.accept_chat_requests(chat_room_ids=[chat_room.id])
+self.on_message(chat_room) def on_message(self, chat_room): #
+ã¡ãã»ã¼ã¸ãåºåãã print(chat_room.last_message.text) ws_token =
+api.get_web_socket_token() bot = ChatBot() bot.run(ws_token) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
```

### Comparing `yaylib-1.0.5/setup.py` & `yaylib-1.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup, find_packages
 from yaylib import __version__
 
 name = "yaylib"
 author = "Qvco, Konn"
 author_email = "nikola.desuga@gmail.com"
-description = "This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts."
+description = "同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。"
 long_description_content_type = "text/markdown"
 license = "MIT"
 url = "https://github.com/qvco/yaylib"
 
 keywords = [
     "yay",
     "yaylib",
     "api",
     "bot",
+    "tool",
     "client",
     "library",
     "wrapper",
     "ボット",
     "ライブラリ",
+    "ツール",
 ]
 
 install_requires = [
     "httpx>=0.17.1",
     "Pillow>=9.3.0",
     "cryptography>=41.0.1",
     "websocket-client>=1.6.0",
```

### Comparing `yaylib-1.0.5/tests/test_call.py` & `yaylib-1.0.6/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_cassandra.py` & `yaylib-1.0.6/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_chat.py` & `yaylib-1.0.6/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_group.py` & `yaylib-1.0.6/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_misc.py` & `yaylib-1.0.6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_post.py` & `yaylib-1.0.6/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_review.py` & `yaylib-1.0.6/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_thread.py` & `yaylib-1.0.6/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/tests/test_user.py` & `yaylib-1.0.6/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/__init__.py` & `yaylib-1.0.6/yaylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .client import *
 from .config import *
 from .errors import *
 from .models import *
 from .responses import *
 from .utils import *
-from .websocket import *
+from .api.websocket import *
 
 __version__ = Configs.YAYLIB_VERSION
 __all__ = [
     "Client",
     "config",
     "errors",
     "models",
```

### Comparing `yaylib-1.0.5/yaylib/api/__init__.py` & `yaylib-1.0.6/yaylib/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,8 +36,9 @@
     "review",
     "search",
     "thread",
     "twitter",
     "user_identity",
     "user",
     "wallet",
+    "websocket",
 ]
```

### Comparing `yaylib-1.0.5/yaylib/api/api.py` & `yaylib-1.0.6/yaylib/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         proxy: str = None,
         max_retries=3,
         backoff_factor=1.0,
         timeout=30,
         err_lang="ja",
         base_path=current_path + "/config/",
         save_session=True,
+        session_filename="session",
         loglevel=logging.INFO,
     ):
         self.yaylib_version = Configs.YAYLIB_VERSION
         self.api_version = Configs.YAY_API_VERSION
         self.api_key = Configs.YAY_API_KEY
         self.fernet = None
         self.secret_key = None
@@ -73,14 +74,15 @@
         self.max_retries = max_retries
         self.retry_statuses = [500, 502, 503, 504]
         self.backoff_factor = backoff_factor
         self.timeout = timeout
         self.err_lang = err_lang
         self.base_path = base_path
         self.save_session = save_session
+        self.session_filename = session_filename
 
         self._generate_all_uuids()
         self.session = httpx.Client(proxies=self.proxy, timeout=self.timeout)
         self.session.headers.update(Configs.REQUEST_HEADERS)
         self.session.headers.update({"X-Device-Uuid": self.device_uuid})
         if access_token:
             self.session.headers.setdefault("Authorization", f"Bearer {access_token}")
@@ -115,15 +117,16 @@
         headers=None,
         access_token=None,
     ):
         headers = headers or self.session.headers
 
         if access_token is not None:
             headers["Authorization"] = f"Bearer {access_token}"
-        elif not user_auth and "Authorization" in headers:
+
+        if not user_auth and "Authorization" in headers:
             del headers["Authorization"]
 
         response = None
         backoff_duration = 0
         auth_retry_count = 0
         max_auth_retries = 2
 
@@ -140,46 +143,49 @@
 
             response = self.session.request(
                 method, endpoint, params=params, json=payload, headers=headers
             )
 
             if self.save_session is True and response.status_code == 401:
                 if "/api/v1/oauth/token" in endpoint:
-                    os.remove(self.base_path + "session.json")
+                    os.remove(self.base_path + self.session_filename + ".json")
                     message = "Refresh token expired. Try logging in again."
                     raise AuthenticationError(message)
 
                 auth_retry_count += 1
                 self.logger.debug("Access token expired. Refreshing tokens...")
 
                 if auth_retry_count < max_auth_retries:
-                    session = load_session(base_path=self.base_path)
+                    session = load_session(
+                        base_path=self.base_path, session_filename=self.session_filename
+                    )
 
                     if session is not None and self.fernet is not None:
                         session = decrypt(fernet=self.fernet, session=session)
                         refresh_token = session["refresh_token"]
                         response = get_token(
                             self,
                             grant_type="refresh_token",
                             refresh_token=refresh_token,
                         )
                         save_session(
                             base_path=self.base_path,
+                            session_filename=self.session_filename,
                             fernet=self.fernet,
                             access_token=response.access_token,
                             refresh_token=response.refresh_token,
                             user_id=response.user_id,
                         )
                         self.session.headers[
                             "Authorization"
                         ] = f"Bearer {response.access_token}"
                         continue
 
                 else:
-                    os.remove(self.base_path + "session.json")
+                    os.remove(self.base_path + self.session_filename + ".json")
                     message = (
                         "Maximum authentication retries exceeded. Try logging in again."
                     )
                     raise AuthenticationError(message)
 
             if response.status_code not in self.retry_statuses:
                 break
@@ -275,9 +281,9 @@
                 return response
             except ValueError:
                 return response
         else:
             return response
 
     def _generate_all_uuids(self):
-        self.device_uuid = generate_uuid()[0]
-        self.uuid, self.url_uuid = generate_uuid()
+        self.device_uuid = generate_uuid(True)
+        self.uuid = generate_uuid(True)
```

### Comparing `yaylib-1.0.5/yaylib/api/call.py` & `yaylib-1.0.6/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/cassandra.py` & `yaylib-1.0.6/yaylib/api/cassandra.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from ..config import Configs
+from ..config import Configs, Endpoints
 from ..responses import ActivitiesResponse
 
 
 def get_user_activities(self, access_token: str = None, **params) -> ActivitiesResponse:
     """
 
     Parameters
@@ -70,11 +70,11 @@
 def received_notification(
     self, pid: str, type: str, opened_at: int = None, access_token: str = None
 ):
     # TODO: opened_atはnullalbeか確認する
     self._check_authorization(access_token)
     return self._make_request(
         "POST",
-        endpoint=f"{Configs.YAY_API_URL}/api/received_push_notifications",
+        endpoint=f"{Endpoints.BASE_API_URL}/api/received_push_notifications",
         payload={"pid": pid, "type": type, "opened_at": opened_at},
         access_token=access_token,
     )
```

### Comparing `yaylib-1.0.5/yaylib/api/chat.py` & `yaylib-1.0.6/yaylib/api/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,16 @@
     MessageResponse,
     MessagesResponse,
     StickerPacksResponse,
     UnreadStatusResponse,
 )
 
 
-def accept_chat_request(self, chat_room_ids: List[int], access_token: str = None):
+def accept_chat_requests(self, chat_room_ids: List[int], access_token: str = None):
     self._check_authorization(access_token)
-    chat_room_ids = (
-        [chat_room_ids] if not isinstance(chat_room_ids, list) else chat_room_ids
-    )
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
         payload={"chat_room_ids": chat_room_ids},
         access_token=access_token,
     )
     self.logger.info("Accepted chat requests")
@@ -249,20 +246,27 @@
         params=params,
         data_type=MessagesResponse,
         access_token=access_token,
     ).messages
 
 
 def get_request_chat_rooms(
-    self, from_timestamp: int = None, access_token: str = None
+    self, access_token: str = None, **params
 ) -> ChatRoomsResponse:
+    """
+
+    Parameters:
+    ----------
+
+        - number: int (optional)
+        - from_timestamp: int (optional)
+        - access_token: str (optional)
+
+    """
     self._check_authorization(access_token)
-    params = {}
-    if from_timestamp:
-        params["from_timestamp"] = from_timestamp
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.CHAT_ROOMS_V1}/request_list",
         params=params,
         data_type=ChatRoomsResponse,
         access_token=access_token,
     )
@@ -312,15 +316,15 @@
 def invite_to_chat(
     self, chat_room_id: int, user_ids: List[int], access_token: str = None
 ):
     self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/invite",
-        payload={"with_user_ids[]": user_ids},
+        payload={"with_user_ids": user_ids},
         access_token=access_token,
     )
     self.logger.info("Invited users to the chatroom.")
     return response
 
 
 def kick_users_from_chat(
@@ -457,15 +461,15 @@
 
 
 def unhide_chat(self, chat_room_ids: int, access_token: str = None):
     self._check_authorization(access_token)
     response = self._make_request(
         "DELETE",
         endpoint=f"{Endpoints.HIDDEN_V1}/chats",
-        params={"chat_room_ids[]": chat_room_ids},
+        params={"chat_room_ids": chat_room_ids},
         access_token=access_token,
     )
     self.logger.info("Unhid the chatrooms")
     return response
 
 
 def unpin_chat(self, chat_room_id: int, access_token: str = None):
```

### Comparing `yaylib-1.0.5/yaylib/api/group.py` & `yaylib-1.0.6/yaylib/api/group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/login.py` & `yaylib-1.0.6/yaylib/api/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             "email": email,
             "password": password,
             "email_grant_token": email_grant_token,
         },
         data_type=LoginUpdateResponse,
         access_token=access_token,
     )
-    self.logger.info(self, fname="Your email has been changed.")
+    self.logger.info("Your email has been changed.")
     return response
 
 
 def change_password(
     self, current_password: str, new_password: str, access_token: str = None
 ) -> LoginUpdateResponse:
     response = self._make_request(
@@ -71,29 +71,29 @@
             "api_key": self.api_key,
             "current_password": current_password,
             "password": new_password,
         },
         data_type=LoginUpdateResponse,
         access_token=access_token,
     )
-    self.logger.info(self, fname="Your password has been changed..")
+    self.logger.info("Your password has been changed..")
     return response
 
 
 def get_token(
     self,
     grant_type: str,
     refresh_token: str = None,
     email: str = None,
     password: str = None,
     access_token: str = None,
 ) -> TokenResponse:
     return self._make_request(
         "POST",
-        endpoint=f"{Configs.YAY_API_URL}/api/v1/oauth/token",
+        endpoint=f"{Endpoints.BASE_API_URL}/api/v1/oauth/token",
         payload={
             "grant_type": grant_type,
             "email": email,
             "password": password,
             "refresh_token": refresh_token,
         },
         data_type=TokenResponse,
@@ -111,15 +111,19 @@
         return False
 
 
 def login_with_email(
     self, email: str, password: str, secret_key: str = None
 ) -> LoginUserResponse:
     if self.save_session:
-        session = load_session(base_path=self.base_path, check_email=email)
+        session = load_session(
+            base_path=self.base_path,
+            session_filename=self.session_filename,
+            check_email=email,
+        )
         if session is not None and secret_key is not None:
             self.secret_key = secret_key
             self.fernet = Fernet(secret_key)
             session = decrypt(fernet=self.fernet, session=session)
             self.session.headers.setdefault(
                 "Authorization", f"Bearer {session['access_token']}"
             )
@@ -156,14 +160,15 @@
             f"Your 'secret_key' for {Colors.BOLD + email + Colors.RESET} is: {Colors.OKGREEN + secret_key.decode() + Colors.RESET}",
             "Please copy and securely store this key in a safe location.",
             "For more information, visit: https://github.com/qvco/yaylib/blob/master/docs/API-Reference/login/login.md",
         )
 
         save_session(
             base_path=self.base_path,
+            session_filename=self.session_filename,
             fernet=self.fernet,
             access_token=response.access_token,
             refresh_token=response.refresh_token,
             user_id=response.user_id,
             email=email,
         )
```

### Comparing `yaylib-1.0.5/yaylib/api/misc.py` & `yaylib-1.0.6/yaylib/api/misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/post.py` & `yaylib-1.0.6/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/review.py` & `yaylib-1.0.6/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/thread.py` & `yaylib-1.0.6/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/api/user.py` & `yaylib-1.0.6/yaylib/api/user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/client.py` & `yaylib-1.0.6/yaylib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 from .api.cassandra import (
     get_user_activities,
     get_user_merged_activities,
     received_notification,
 )
 from .api.chat import (
-    accept_chat_request,
+    accept_chat_requests,
     check_unread_status,
     create_group_chat,
     create_private_chat,
     delete_background,
     delete_message,
     edit_chat_room,
     get_chatable_users,
@@ -337,14 +337,15 @@
         - proxy: str - (optional)
         - max_retries: int - (optional)
         - backoff_factor: float - (optional)
         - timeout: int - (optional)
         - err_lang: str - (optional)
         - base_path: str - (optional)
         - save_session: bool - (optional)
+        - session_filename: str - (optional)
         - loglevel: int - (optional)
 
     <https://github.com/qvco/yaylib>
 
     ---
 
     ### Yay! (nanameue, Inc.) API Client
@@ -607,28 +608,28 @@
     def received_notification(
         self, pid: str, type: str, opened_at: int = None, access_token: str = None
     ) -> dict:
         return received_notification(self, pid, type, opened_at, access_token)
 
     # -CHAT
 
-    def accept_chat_request(
+    def accept_chat_requests(
         self, chat_room_ids: List[int], access_token: str = None
     ) -> dict:
         """
 
         チャットリクエストを承認します
 
         Parameters
         ----------
 
             - chat_room_ids: List[int] - (required)
 
         """
-        return accept_chat_request(self, chat_room_ids, access_token)
+        return accept_chat_requests(self, chat_room_ids, access_token)
 
     def check_unread_status(
         self, from_time: int, access_token: str = None
     ) -> UnreadStatusResponse:
         """
 
         チャットの未読ステータスを確認します
@@ -791,23 +792,30 @@
         ---------------
             - from_message_id: int - (optional)
             - to_message_id: int - (optional)
 
         """
         return get_messages(self, chat_room_id, access_token, **params)
 
-    def get_request_chat_rooms(
-        self, from_timestamp: int = None, access_token: str = None
+    def get_chat_requests(
+        self, access_token: str = None, **params
     ) -> ChatRoomsResponse:
         """
 
         チャットリクエストを取得します
 
+        Parameters:
+        ----------
+
+            - number: int (optional)
+            - from_timestamp: int (optional)
+            - access_token: str (optional)
+
         """
-        return get_request_chat_rooms(self, from_timestamp, access_token)
+        return get_request_chat_rooms(self, access_token, **params)
 
     def get_chat_room(self, chat_room_id: int, access_token: str = None) -> ChatRoom:
         """
 
         チャットルームの詳細を取得します
 
         """
```

### Comparing `yaylib-1.0.5/yaylib/errors.py` & `yaylib-1.0.6/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/models.py` & `yaylib-1.0.6/yaylib/models.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/responses.py` & `yaylib-1.0.6/yaylib/responses.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.5/yaylib/utils.py` & `yaylib-1.0.6/yaylib/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,18 +48,20 @@
 def console_print(*args):
     print("\n")
     for arg in args:
         print(arg)
     print("\n")
 
 
-def generate_uuid() -> tuple:
+def generate_uuid(uuid_type: bool = True) -> tuple:
     generated_uuid = str(uuid.uuid4())
-    url_uuid = generated_uuid.replace("-", "")
-    return generated_uuid, url_uuid
+    if uuid_type:
+        return generated_uuid
+    else:
+        return generated_uuid.replace("-", "")
 
 
 def parse_datetime(timestamp: int) -> str:
     if timestamp is not None:
         return str(datetime.fromtimestamp(timestamp))
     return timestamp
 
@@ -86,41 +88,44 @@
         }
     )
     return session
 
 
 def save_session(
     base_path: str,
+    session_filename: str,
     fernet,
     access_token: str,
     refresh_token: str,
     user_id: int,
     email: str = None,
 ):
-    session = load_session(base_path=base_path)
+    session = load_session(base_path=base_path, session_filename=session_filename)
     updated_session = {
         "access_token": access_token,
         "refresh_token": refresh_token,
         "user_id": user_id,
         "email": email,
     }
     if email is None:
         updated_session["email"] = session.get("email")
 
     updated_session = encrypt(fernet, updated_session)
 
-    with open(base_path + "session.json", "w") as f:
+    with open(base_path + session_filename + ".json", "w") as f:
         json.dump(updated_session, f, indent=4)
 
 
-def load_session(base_path: str, fernet=None, check_email: str = None):
-    if not os.path.exists(base_path + "session.json"):
+def load_session(
+    base_path: str, session_filename: str, fernet=None, check_email: str = None
+):
+    if not os.path.exists(base_path + session_filename + ".json"):
         return None
 
-    with open(base_path + "session.json", "r") as f:
+    with open(base_path + session_filename + ".json", "r") as f:
         session = json.load(f)
 
     result = all(
         key in session for key in ("access_token", "refresh_token", "user_id", "email")
     )
     session = None if result is False else session
```

### Comparing `yaylib-1.0.5/yaylib/websocket.py` & `yaylib-1.0.6/yaylib/api/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import json
 import websocket
 
-from .config import Configs
-from .models import Message, ChatRoom, GroupUpdatesEvent
-from .responses import ChannelResponse
+from ..config import Configs
+from ..models import Message, ChatRoom, GroupUpdatesEvent
+from ..responses import ChannelResponse
 
 
 class WebSocketBaseHandler(object):
     """イベントハンドラーの基底クラス"""
 
     def __init__(self):
         self.ws = None
@@ -81,15 +81,15 @@
         >>> class MyHandler(yaylib.MessageEventHandler):
         >>>     def on_message(self, message):
         >>>         print(message.text)
         >>>
         >>> api = yaylib.Client()
         >>>
         >>> ws_token = api.get_web_socket_token()
-        >>> bot = MyHandler()
+        >>> bot = MyHandler(chat_room_id=12345)
         >>> bot.run(ws_token)
 
     """
 
     def __init__(self, chat_room_id: int):
         super().__init__()
         self.chat_room_id = chat_room_id
@@ -278,15 +278,15 @@
         >>> class MyHandler(yaylib.GroupPostEventHandler):
         >>>     def on_post(self, group_id):
         >>>         print(group_id)
         >>>
         >>> api = yaylib.Client()
         >>>
         >>> ws_token = api.get_web_socket_token()
-        >>> bot = MyHandler()
+        >>> bot = MyHandler(group_id=12345)
         >>> bot.run(ws_token)
 
     """
 
     def __init__(self, group_id: int):
         super().__init__()
         self.group_id = group_id
```

### Comparing `yaylib-1.0.5/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.6/yaylib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.5
-Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
+Version: 1.0.6
+Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
+Keywords: yay,yaylib,api,bot,tool,client,library,wrapper,ボット,ライブラリ,ツール
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
@@ -91,14 +91,63 @@
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
+### yaylib 利用で実現できること
+
+<table>
+    <tr>
+        <th>カテゴリ</th>
+        <th>「yaylib」で自動化できること</th>
+        <th>応用先</th>
+    </tr>
+    <tr>
+		<td>データ収集の効率化</td>
+		<td>
+            <li>投稿情報取得</li>
+            <li>ユーザー情報取得</li>
+            <li>人気のワード取得</li>
+            <li>フォロー/フォロワー情報取得</li>
+        </td>
+		<td>
+            <li>SNSデータマーケティング</li>
+            <li>トレンド解析</li>
+            <li>ニーズ調査</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(投稿関連)</td>
+		<td>
+            <li>投稿する</li>
+            <li>リツイートする</li>
+            <li>いいねする</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+    <tr>
+		<td>アカウント操作<br>(ユーザー関連)</td>
+		<td>
+            <li>フォローする/フォロー解除する</li>
+            <li>ブロックする/ブロック解除する</li>
+            <li>ミュートする/ミュート解除する</li>
+            <li>DMを送る</li>
+        </td>
+		<td>
+            <li>Yay! 自動運用</li>
+            <li>Yay! Bot開発</li>
+        </td>
+	</tr>
+</table>
+
 #### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -113,18 +162,14 @@
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
 ```
 
-<p align="center">
-    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
-</p>
-
 #### ✨ 画像と一緒に投稿を作成する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
@@ -141,28 +186,32 @@
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post("Hello with yaylib!", in_reply_to=373189088)
+api.create_post(
+    "Hello with yaylib!",
+    in_reply_to=返信先の投稿ID,
+    mention_ids=[返信先のユーザーID]
+)
 ```
 
 #### ✨ タイムラインを 100 件取得する
 
 ```python
 import yaylib
 
 api = yaylib.Client()
 
 timeline = api.get_timeline(number=100)
 
 for post in timeline.posts:
-    print(post.user.nickname)  # 投稿者
+    print(post.user.nickname)  # 投稿者名
     print(post.text)  # 本文
     print(post.likes_count)  # いいね数
     print(post.reposts_count)  # (´∀｀∩)↑age↑の数
     print(post.in_reply_to_post_count)  # 返信の数
 ```
 
 #### ✨ タイムラインをキーワードで検索して「いいね」する
@@ -193,14 +242,42 @@
 
 timeline = api.get_timeline(number=15)
 
 for post in timeline.posts:
     api.follow_user(post.user.id)
 ```
 
+#### ✨ リアルタイムでチャットを取得する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+
+class ChatBot(yaylib.ChatRoomEventHandler):
+
+    def on_request(self, total_count: int):
+        # チャットリクエストを承認する
+        chat_room = api.get_chat_requests(number=1).chat_rooms[0]
+        api.accept_chat_requests(chat_room_ids=[chat_room.id])
+        self.on_message(chat_room)
+
+    def on_message(self, chat_room):
+        # メッセージを出力する
+        print(chat_room.last_message.text)
+
+
+ws_token = api.get_web_socket_token()
+
+bot = ChatBot()
+bot.run(ws_token)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## :crown: yaylib で誕生したロボットたち
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.5 Summary: This Python package
-provides an easy-to-use interface for accessing data from Yay! (https://
-yay.space/). With this API Client, you can retrieve user profiles, posts,
-comments, and other content from Yay!, as well as perform common tasks like
-liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
-Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
-nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
-nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.6 Summary:
+åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
+ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
+Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
+qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
+Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
+Keywords:
+yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
@@ -42,47 +41,69 @@
 > **Note** >
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
 [https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
-3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
-æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-("Hello with yaylib!") ``` #### â¨
+3994884d2ba3]](https://github.com/qvco) Quick Example ### yaylib
+å©ç¨ã§å®ç¾ã§ãããã¨
+ã«ãã´ãª       ãyaylibãã§èªååã§ãããã¨     å¿ç¨å
+                               æç¨¿æå ±åå¾                                         SNSãã¼ã¿ãã¼ã±ãã£ã³ã°
+ãã¼ã¿åé�ã¦ã¼ã¶ã¼æå ±åå¾                             ãã¬ã³ãè§£æ
+                               äººæ°ã®ã¯ã¼ãåå¾                             ãã¼ãºèª¿æ»
+                               ãã©ã­ã¼/ãã©ã­ã¯ã¼æå ±åå¾
+ã¢ã«ã¦ã³ã�æç¨¿ãã                                                     Yay! èªåéç¨
+(æç¨¿é¢é£)     ãªãã¤ã¼ããã                                   Yay! Botéçº
+                               ããã­ãã
+                               ãã©ã­ã¼ãã/ãã©ã­ã¼è§£é¤ãã
+ã¢ã«ã¦ã³ã�ãã­ãã¯ãã/ãã­ãã¯è§£é¤ãYay! èªåéç¨
+(ã¦ã¼ã¶ã¼é¢ãã¥ã¼ããã/ãã¥ã¼ãè§£é¤ãYay! Botéçº
+                               DMãéã
+#### â¨ æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client()
+api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã")
+api.create_post("Hello with yaylib!") ``` #### â¨
 åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-shared_url="https://github.com/qvco/yaylib") ```
-                            [Writing Text Threads]
-#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+shared_url="https://github.com/qvco/yaylib") ``` #### â¨
+ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
 yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
 ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
 ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
 attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
 import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
-password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
-in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
-```python import yaylib api = yaylib.Client() timeline = api.get_timeline
-(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
-print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
-(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
-(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+password="ãã¹ã¯ã¼ã") api.create_post( "Hello with yaylib!",
+in_reply_to=è¿ä¿¡åã®æç¨¿ID, mention_ids=[è¿ä¿¡åã®ã¦ã¼ã¶ã¼ID] )
+``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã ```python import yaylib
+api = yaylib.Client() timeline = api.get_timeline(number=100) for post in
+timeline.posts: print(post.user.nickname) # æç¨¿èå print(post.text) #
+æ¬æ print(post.likes_count) # ããã­æ° print(post.reposts_count) #
+(Â´âï½â©)âageâã®æ° print(post.in_reply_to_post_count) # è¿ä¿¡ã®æ°
+``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
 post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
-timeline.posts: api.follow_user(post.user.id) ```
+timeline.posts: api.follow_user(post.user.id) ``` #### â¨
+ãªã¢ã«ã¿ã¤ã ã§ãã£ãããåå¾ãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") class ChatBot(yaylib.ChatRoomEventHandler): def
+on_request(self, total_count: int): #
+ãã£ãããªã¯ã¨ã¹ããæ¿èªãã chat_room = api.get_chat_requests
+(number=1).chat_rooms[0] api.accept_chat_requests(chat_room_ids=[chat_room.id])
+self.on_message(chat_room) def on_message(self, chat_room): #
+ã¡ãã»ã¼ã¸ãåºåãã print(chat_room.last_message.text) ws_token =
+api.get_web_socket_token() bot = ChatBot() bot.run(ws_token) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
```

### Comparing `yaylib-1.0.5/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.6/yaylib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE
 README.md
 setup.py
+tests/__init__.py
+tests/config.py
 tests/test_call.py
 tests/test_cassandra.py
 tests/test_chat.py
 tests/test_group.py
 tests/test_misc.py
 tests/test_post.py
 tests/test_review.py
 tests/test_thread.py
 tests/test_user.py
+tests/test_utils.py
 yaylib/__init__.py
 yaylib/client.py
 yaylib/config.py
 yaylib/errors.py
 yaylib/models.py
 yaylib/responses.py
 yaylib/utils.py
-yaylib/websocket.py
 yaylib.egg-info/PKG-INFO
 yaylib.egg-info/SOURCES.txt
 yaylib.egg-info/dependency_links.txt
 yaylib.egg-info/requires.txt
 yaylib.egg-info/top_level.txt
 yaylib/api/__init__.py
 yaylib/api/api.py
@@ -30,8 +32,9 @@
 yaylib/api/chat.py
 yaylib/api/group.py
 yaylib/api/login.py
 yaylib/api/misc.py
 yaylib/api/post.py
 yaylib/api/review.py
 yaylib/api/thread.py
-yaylib/api/user.py
+yaylib/api/user.py
+yaylib/api/websocket.py
```

