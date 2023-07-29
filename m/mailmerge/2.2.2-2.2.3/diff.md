# Comparing `tmp/mailmerge-2.2.2.tar.gz` & `tmp/mailmerge-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailmerge-2.2.2.tar", last modified: Tue Jul 11 12:40:42 2023, max compression
+gzip compressed data, was "mailmerge-2.2.3.tar", last modified: Sat Jul 29 01:20:24 2023, max compression
```

## Comparing `mailmerge-2.2.2.tar` & `mailmerge-2.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.063787 mailmerge-2.2.2/
--rw-rw-r--   0 awdeorio   (501) staff       (20)      384 2021-06-07 18:37:26.000000 mailmerge-2.2.2/.pylintrc
--rw-rw-r--   0 awdeorio   (501) staff       (20)      849 2021-10-08 13:05:33.000000 mailmerge-2.2.2/CONTRIBUTING.md
--rw-rw-r--   0 awdeorio   (501) staff       (20)     1080 2019-05-14 18:36:54.000000 mailmerge-2.2.2/LICENSE
--rw-rw-r--   0 awdeorio   (501) staff       (20)      228 2021-07-16 23:01:53.000000 mailmerge-2.2.2/MANIFEST.in
--rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-11 12:40:42.063641 mailmerge-2.2.2/PKG-INFO
--rw-rw-r--   0 awdeorio   (501) staff       (20)    13269 2022-10-05 18:36:38.000000 mailmerge-2.2.2/README.md
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.061043 mailmerge-2.2.2/mailmerge/
--rw-rw-r--   0 awdeorio   (501) staff       (20)      234 2021-07-16 17:58:04.000000 mailmerge-2.2.2/mailmerge/__init__.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    12596 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/__main__.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)      240 2021-07-16 17:58:04.000000 mailmerge-2.2.2/mailmerge/exceptions.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     4866 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/sendmail_client.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    13496 2023-07-11 12:40:31.000000 mailmerge-2.2.2/mailmerge/template_message.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.061776 mailmerge-2.2.2/mailmerge.egg-info/
--rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/PKG-INFO
--rw-rw-r--   0 awdeorio   (501) staff       (20)      793 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/SOURCES.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)        1 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/dependency_links.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       54 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/entry_points.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)      147 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/requires.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2023-07-11 12:40:42.000000 mailmerge-2.2.2/mailmerge.egg-info/top_level.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       38 2023-07-11 12:40:42.063820 mailmerge-2.2.2/setup.cfg
--rw-rw-r--   0 awdeorio   (501) staff       (20)     1281 2023-07-11 12:40:31.000000 mailmerge-2.2.2/setup.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.062885 mailmerge-2.2.2/tests/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       97 2021-07-16 17:58:04.000000 mailmerge-2.2.2/tests/__init__.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     3455 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_helpers.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    30347 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_main.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    19537 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_main_output.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     3619 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_ratelimit.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    14167 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_sendmail_client.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    28193 2023-07-11 12:40:31.000000 mailmerge-2.2.2/tests/test_template_message.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    13866 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/test_template_message_encodings.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-11 12:40:42.063476 mailmerge-2.2.2/tests/testdata/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_1.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       24 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_17.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)     5617 2019-11-01 17:36:28.000000 mailmerge-2.2.2/tests/testdata/attachment_2.pdf
--rw-rw-r--   0 awdeorio   (501) staff       (20)      697 2021-06-07 18:37:26.000000 mailmerge-2.2.2/tests/testdata/attachment_3.jpg
--rw-rw-r--   0 awdeorio   (501) staff       (20)       36 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/testdata/mailmerge_database_with_BOM.csv
--rw-rw-r--   0 awdeorio   (501) staff       (20)      222 2021-10-08 13:05:33.000000 mailmerge-2.2.2/tests/utils.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-29 01:20:24.576827 mailmerge-2.2.3/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      384 2021-06-07 18:37:26.000000 mailmerge-2.2.3/.pylintrc
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      849 2021-10-08 13:05:33.000000 mailmerge-2.2.3/CONTRIBUTING.md
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1080 2019-05-14 18:36:54.000000 mailmerge-2.2.3/LICENSE
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      228 2021-07-16 23:01:53.000000 mailmerge-2.2.3/MANIFEST.in
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-29 01:20:24.576670 mailmerge-2.2.3/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13269 2023-07-18 21:00:43.000000 mailmerge-2.2.3/README.md
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-29 01:20:24.574039 mailmerge-2.2.3/mailmerge/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      234 2021-07-16 17:58:04.000000 mailmerge-2.2.3/mailmerge/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13005 2023-07-29 01:20:08.000000 mailmerge-2.2.3/mailmerge/__main__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      240 2021-07-16 17:58:04.000000 mailmerge-2.2.3/mailmerge/exceptions.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     6924 2023-07-29 01:20:08.000000 mailmerge-2.2.3/mailmerge/sendmail_client.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13496 2023-07-11 12:40:31.000000 mailmerge-2.2.3/mailmerge/template_message.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-29 01:20:24.574762 mailmerge-2.2.3/mailmerge.egg-info/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13652 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      793 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/SOURCES.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        1 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/dependency_links.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       54 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/entry_points.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      147 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/requires.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2023-07-29 01:20:24.000000 mailmerge-2.2.3/mailmerge.egg-info/top_level.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       38 2023-07-29 01:20:24.576858 mailmerge-2.2.3/setup.cfg
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1281 2023-07-29 01:20:08.000000 mailmerge-2.2.3/setup.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-29 01:20:24.575906 mailmerge-2.2.3/tests/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       97 2021-07-16 17:58:04.000000 mailmerge-2.2.3/tests/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     3455 2023-07-11 12:40:31.000000 mailmerge-2.2.3/tests/test_helpers.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    30347 2023-07-11 12:40:31.000000 mailmerge-2.2.3/tests/test_main.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    19537 2021-10-08 13:05:33.000000 mailmerge-2.2.3/tests/test_main_output.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     3619 2021-10-08 13:05:33.000000 mailmerge-2.2.3/tests/test_ratelimit.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    18267 2023-07-29 01:20:08.000000 mailmerge-2.2.3/tests/test_sendmail_client.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    28193 2023-07-11 12:40:31.000000 mailmerge-2.2.3/tests/test_template_message.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    13866 2021-10-08 13:05:33.000000 mailmerge-2.2.3/tests/test_template_message_encodings.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2023-07-29 01:20:24.576500 mailmerge-2.2.3/tests/testdata/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2019-11-01 17:36:28.000000 mailmerge-2.2.3/tests/testdata/attachment_1.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       24 2019-11-01 17:36:28.000000 mailmerge-2.2.3/tests/testdata/attachment_17.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     5617 2019-11-01 17:36:28.000000 mailmerge-2.2.3/tests/testdata/attachment_2.pdf
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      697 2021-06-07 18:37:26.000000 mailmerge-2.2.3/tests/testdata/attachment_3.jpg
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       36 2021-10-08 13:05:33.000000 mailmerge-2.2.3/tests/testdata/mailmerge_database_with_BOM.csv
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      222 2021-10-08 13:05:33.000000 mailmerge-2.2.3/tests/utils.py
```

### Comparing `mailmerge-2.2.2/CONTRIBUTING.md` & `mailmerge-2.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/LICENSE` & `mailmerge-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/PKG-INFO` & `mailmerge-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailmerge
-Version: 2.2.2
+Version: 2.2.3
 Summary: A simple, command line mail merge tool
 Home-page: https://github.com/awdeorio/mailmerge/
 Author: Andrew DeOrio
 Author-email: awdeorio@umich.edu
 License: MIT
 Keywords: mail merge,mailmerge,email
 Requires-Python: >=3.6
```

### Comparing `mailmerge-2.2.2/README.md` & `mailmerge-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/mailmerge/__main__.py` & `mailmerge-2.2.3/mailmerge/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,24 @@
             # [smtp_server]
             # host = newman.eecs.umich.edu
             # port = 25
             # security = PLAIN
             # username = YOUR_USERNAME_HERE
             # ratelimit = 0
 
+            # Example: XOAUTH
+            # Enter your token at the password prompt.  For Microsoft OAuth
+            # authentication, a token can be obtained with the oauth2ms tool
+            # https://github.com/harishkrupo/oauth2ms
+            # [smtp_server]
+            # host = smtp.office365.com
+            # port = 587
+            # security = XOAUTH
+            # username = username@example.com
+
             # Example: No security
             # [smtp_server]
             # host = newman.eecs.umich.edu
             # port = 25
             # ratelimit = 0
         """))
     print(textwrap.dedent(f"""\
```

### Comparing `mailmerge-2.2.2/mailmerge/template_message.py` & `mailmerge-2.2.3/mailmerge/template_message.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/mailmerge.egg-info/PKG-INFO` & `mailmerge-2.2.3/mailmerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailmerge
-Version: 2.2.2
+Version: 2.2.3
 Summary: A simple, command line mail merge tool
 Home-page: https://github.com/awdeorio/mailmerge/
 Author: Andrew DeOrio
 Author-email: awdeorio@umich.edu
 License: MIT
 Keywords: mail merge,mailmerge,email
 Requires-Python: >=3.6
```

### Comparing `mailmerge-2.2.2/mailmerge.egg-info/SOURCES.txt` & `mailmerge-2.2.3/mailmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/setup.py` & `mailmerge-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 setuptools.setup(
     name="mailmerge",
     description="A simple, command line mail merge tool",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    version="2.2.2",
+    version="2.2.3",
     author="Andrew DeOrio",
     author_email="awdeorio@umich.edu",
     url="https://github.com/awdeorio/mailmerge/",
     license="MIT",
     packages=["mailmerge"],
     keywords=["mail merge", "mailmerge", "email"],
     install_requires=[
```

### Comparing `mailmerge-2.2.2/tests/test_helpers.py` & `mailmerge-2.2.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/test_main.py` & `mailmerge-2.2.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/test_main_output.py` & `mailmerge-2.2.3/tests/test_main_output.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/test_ratelimit.py` & `mailmerge-2.2.3/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/test_sendmail_client.py` & `mailmerge-2.2.3/tests/test_sendmail_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Andrew DeOrio <awdeorio@umich.edu>
 """
 import textwrap
 import socket
 import smtplib
 import email
 import email.parser
+import base64
+import ssl
 import pytest
 from mailmerge import SendmailClient, MailmergeError
 
 
 def test_smtp(mocker, tmp_path):
     """Verify SMTP library calls."""
     config_path = tmp_path/"server.conf"
@@ -246,14 +248,98 @@
     smtp = mock_smtp.return_value.__enter__.return_value
     assert smtp.ehlo.call_count == 2
     assert smtp.starttls.call_count == 1
     assert smtp.login.call_count == 1
     assert smtp.sendmail.call_count == 1
 
 
+def test_security_xoauth(mocker, tmp_path):
+    """Verify XOAUTH security configuration."""
+    # Config for XOAUTH SMTP server
+    config_path = tmp_path/"server.conf"
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = smtp.office365.com
+        port = 587
+        security = XOAUTH
+        username = username@example.com
+    """))
+
+    # Simple template
+    sendmail_client = SendmailClient(config_path, dry_run=False)
+    message = email.message_from_string("Hello world")
+
+    # Mock SMTP
+    mock_smtp = mocker.patch('smtplib.SMTP')
+    mock_smtp_ssl = mocker.patch('smtplib.SMTP_SSL')
+
+    # Mock the password entry
+    mock_getpass = mocker.patch('getpass.getpass')
+    mock_getpass.return_value = "password"
+
+    # Send a message
+    sendmail_client.sendmail(
+        sender="test@test.com",
+        recipients=["test@test.com"],
+        message=message,
+    )
+
+    # Verify SMTP library calls
+    assert mock_getpass.call_count == 1
+    assert mock_smtp.call_count == 1
+    assert mock_smtp_ssl.call_count == 0
+    smtp = mock_smtp.return_value.__enter__.return_value
+    assert smtp.ehlo.call_count == 2
+    assert smtp.starttls.call_count == 1
+    assert smtp.login.call_count == 0
+    assert smtp.docmd.call_count == 2
+    assert smtp.sendmail.call_count == 1
+
+    # Verify authentication token format.  The first call to docmd() is always
+    # the same.  Second call to docmd() contains a base64 encoded username and
+    # password.
+    assert smtp.docmd.call_args_list[0].args[0] == "AUTH XOAUTH2"
+    user_pass = smtp.docmd.call_args_list[1].args[0]
+    user_pass = base64.b64decode(user_pass)
+    assert user_pass == \
+        b'user=username@example.com\x01auth=Bearer password\x01\x01'
+
+
+def test_security_xoauth_bad_username(mocker, tmp_path):
+    """Verify exception is thrown for UTF-8 username."""
+    # Config for XOAUTH SMTP server
+    config_path = tmp_path/"server.conf"
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = smtp.office365.com
+        port = 587
+        security = XOAUTH
+        username = Laȝamon@example.com
+    """))
+
+    # Simple template
+    sendmail_client = SendmailClient(config_path, dry_run=False)
+    message = email.message_from_string("Hello world")
+
+    # Mock the password entry
+    mock_getpass = mocker.patch('getpass.getpass')
+    mock_getpass.return_value = "password"
+
+    # Send a message
+    with pytest.raises(MailmergeError) as err:
+        sendmail_client.sendmail(
+            sender="test@test.com",
+            recipients=["test@test.com"],
+            message=message,
+        )
+
+    # Verify exception string
+    assert "Username and XOAUTH access token must be ASCII" in str(err.value)
+
+
 def test_security_plain(mocker, tmp_path):
     """Verify plain security configuration."""
     # Config for Plain SMTP server
     config_path = tmp_path/"server.conf"
     config_path.write_text(textwrap.dedent("""\
         [smtp_server]
         host = newman.eecs.umich.edu
@@ -289,15 +375,15 @@
     assert smtp.ehlo.call_count == 0
     assert smtp.starttls.call_count == 0
     assert smtp.login.call_count == 1
     assert smtp.sendmail.call_count == 1
 
 
 def test_security_ssl(mocker, tmp_path):
-    """Verify open (Never) security configuration."""
+    """Verify SSL/TLS security configuration."""
     # Config for SSL SMTP server
     config_path = tmp_path/"server.conf"
     config_path.write_text(textwrap.dedent("""\
         [smtp_server]
         host = smtp.mail.umich.edu
         port = 465
         security = SSL/TLS
@@ -308,14 +394,18 @@
     sendmail_client = SendmailClient(config_path, dry_run=False)
     message = email.message_from_string("Hello world")
 
     # Mock SMTP
     mock_smtp = mocker.patch('smtplib.SMTP')
     mock_smtp_ssl = mocker.patch('smtplib.SMTP_SSL')
 
+    # Mock SSL
+    mock_ssl_create_default_context = \
+        mocker.patch('ssl.create_default_context')
+
     # Mock the password entry
     mock_getpass = mocker.patch('getpass.getpass')
     mock_getpass.return_value = "password"
 
     # Send a message
     sendmail_client.sendmail(
         sender="test@test.com",
@@ -323,21 +413,61 @@
         message=message,
     )
 
     # Verify SMTP library calls
     assert mock_getpass.call_count == 1
     assert mock_smtp.call_count == 0
     assert mock_smtp_ssl.call_count == 1
+    assert mock_ssl_create_default_context.called
+    assert "context" in mock_smtp_ssl.call_args[1]  # SSL cert chain
     smtp = mock_smtp_ssl.return_value.__enter__.return_value
     assert smtp.ehlo.call_count == 0
     assert smtp.starttls.call_count == 0
     assert smtp.login.call_count == 1
     assert smtp.sendmail.call_count == 1
 
 
+def test_ssl_error(mocker, tmp_path):
+    """Verify SSL/TLS with an SSL error."""
+    # Config for SSL SMTP server
+    config_path = tmp_path/"server.conf"
+    config_path.write_text(textwrap.dedent("""\
+        [smtp_server]
+        host = smtp.mail.umich.edu
+        port = 465
+        security = SSL/TLS
+        username = YOUR_USERNAME_HERE
+    """))
+
+    # Simple template
+    sendmail_client = SendmailClient(config_path, dry_run=False)
+    message = email.message_from_string("Hello world")
+
+    # Mock ssl.create_default_context() to raise an exception
+    mocker.patch(
+        'ssl.create_default_context',
+        side_effect=ssl.SSLError(1, "CERTIFICATE_VERIFY_FAILED")
+    )
+
+    # Mock the password entry
+    mock_getpass = mocker.patch('getpass.getpass')
+    mock_getpass.return_value = "password"
+
+    # Send a message
+    with pytest.raises(MailmergeError) as err:
+        sendmail_client.sendmail(
+            sender="test@test.com",
+            recipients=["test@test.com"],
+            message=message,
+        )
+
+    # Verify exception string
+    assert "CERTIFICATE_VERIFY_FAILED" in str(err.value)
+
+
 def test_missing_username(tmp_path):
     """Verify exception on missing username."""
     config_path = tmp_path/"server.conf"
     config_path.write_text(textwrap.dedent("""\
         [smtp_server]
         host = smtp.mail.umich.edu
         port = 465
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mailmerge-2.2.2/tests/test_template_message.py` & `mailmerge-2.2.3/tests/test_template_message.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/test_template_message_encodings.py` & `mailmerge-2.2.3/tests/test_template_message_encodings.py`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/testdata/attachment_2.pdf` & `mailmerge-2.2.3/tests/testdata/attachment_2.pdf`

 * *Files identical despite different names*

### Comparing `mailmerge-2.2.2/tests/testdata/attachment_3.jpg` & `mailmerge-2.2.3/tests/testdata/attachment_3.jpg`

 * *Files identical despite different names*

