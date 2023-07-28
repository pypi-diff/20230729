# Comparing `tmp/discord-webhook-1.2.0.tar.gz` & `tmp/discord-webhook-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-webhook-1.2.0.tar", max compression
+gzip compressed data, was "discord-webhook-1.2.1.tar", max compression
```

## Comparing `discord-webhook-1.2.0.tar` & `discord-webhook-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      172 2023-07-24 19:51:39.962891 discord-webhook-1.2.0/discord_webhook/__init__.py
--rw-r--r--   0        0        0     1027 2023-05-24 20:56:22.801847 discord-webhook-1.2.0/discord_webhook/__main__.py
--rw-r--r--   0        0        0     7127 2023-07-20 21:31:33.181731 discord-webhook-1.2.0/discord_webhook/async_webhook.py
--rw-r--r--   0        0        0        0 2022-11-13 20:16:03.212707 discord-webhook-1.2.0/discord_webhook/py.typed
--rw-r--r--   0        0        0    19367 2023-07-24 19:51:39.963894 discord-webhook-1.2.0/discord_webhook/webhook.py
--rw-r--r--   0        0        0      626 2023-07-24 19:51:39.964891 discord-webhook-1.2.0/discord_webhook/webhook_exceptions.py
--rw-r--r--   0        0        0     1093 2022-11-13 20:16:03.211707 discord-webhook-1.2.0/LICENSE
--rw-r--r--   0        0        0     1160 2023-07-24 19:56:07.714452 discord-webhook-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12311 2023-07-11 19:35:36.873610 discord-webhook-1.2.0/README.md
--rw-r--r--   0        0        0    13248 1970-01-01 00:00:00.000000 discord-webhook-1.2.0/setup.py
--rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 discord-webhook-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-24 19:51:39.962891 discord-webhook-1.2.1/discord_webhook/__init__.py
+-rw-r--r--   0        0        0     1027 2023-05-24 20:56:22.801847 discord-webhook-1.2.1/discord_webhook/__main__.py
+-rw-r--r--   0        0        0     7127 2023-07-20 21:31:33.181731 discord-webhook-1.2.1/discord_webhook/async_webhook.py
+-rw-r--r--   0        0        0        0 2022-11-13 20:16:03.212707 discord-webhook-1.2.1/discord_webhook/py.typed
+-rw-r--r--   0        0        0    19363 2023-07-28 22:44:02.774631 discord-webhook-1.2.1/discord_webhook/webhook.py
+-rw-r--r--   0        0        0      626 2023-07-24 19:51:39.964891 discord-webhook-1.2.1/discord_webhook/webhook_exceptions.py
+-rw-r--r--   0        0        0     1093 2022-11-13 20:16:03.211707 discord-webhook-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1160 2023-07-28 22:47:09.742473 discord-webhook-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12311 2023-07-11 19:35:36.873610 discord-webhook-1.2.1/README.md
+-rw-r--r--   0        0        0    13248 1970-01-01 00:00:00.000000 discord-webhook-1.2.1/setup.py
+-rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 discord-webhook-1.2.1/PKG-INFO
```

### Comparing `discord-webhook-1.2.0/discord_webhook/__main__.py` & `discord-webhook-1.2.1/discord_webhook/__main__.py`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.2.0/discord_webhook/async_webhook.py` & `discord-webhook-1.2.1/discord_webhook/async_webhook.py`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.2.0/discord_webhook/webhook.py` & `discord-webhook-1.2.1/discord_webhook/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         self.content = kwargs.get("content")
         self.embeds = kwargs.get("embeds", [])
         self.files = kwargs.get("files", {})
         self.id = kwargs.get("id")
         self.proxies = kwargs.get("proxies")
         self.rate_limit_retry = kwargs.get("rate_limit_retry", False)
         self.timeout = kwargs.get("timeout")
-        self.tts = kwargs.get("timeout", False)
+        self.tts = kwargs.get("tts", False)
         self.url = url
         self.username = kwargs.get("username", False)
 
     def add_embed(self, embed: Union[DiscordEmbed, Dict[str, Any]]) -> None:
         """
         Add an embedded rich content.
         :param embed: embed object or dict
```

### Comparing `discord-webhook-1.2.0/discord_webhook/webhook_exceptions.py` & `discord-webhook-1.2.1/discord_webhook/webhook_exceptions.py`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.2.0/LICENSE` & `discord-webhook-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.2.0/pyproject.toml` & `discord-webhook-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-webhook"
-version = "1.2.0"
+version = "1.2.1"
 description = "Easily send Discord webhooks with Python"
 authors = ["lovvskillz <14542790+lovvskillz@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "discord_webhook"}]
 repository = "https://github.com/lovvskillz/python-discord-webhook"
 keywords = ["discord", "webhook"]
```

### Comparing `discord-webhook-1.2.0/README.md` & `discord-webhook-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-webhook-1.2.0/setup.py` & `discord-webhook-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'async': ['httpx>=0.23.0,<0.24.0']}
 
 entry_points = \
 {'console_scripts': ['discord_webhook = discord_webhook.__main__:main']}
 
 setup_kwargs = {
     'name': 'discord-webhook',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Easily send Discord webhooks with Python',
     'long_description': '# Python Discord webhook\n\n[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://raw.githubusercontent.com/lovvskillz/python-discord-webhook/master/LICENSE)\n[![PyPI version](https://badge.fury.io/py/discord-webhook.svg)](https://badge.fury.io/py/discord-webhook)\n[![Downloads](https://pepy.tech/badge/discord-webhook)](https://pepy.tech/project/discord-webhook)\n\nEasily send Discord webhooks with Python (also has [async support](#async-support))\n\n## Install\n\nInstall via pip:\n```\npip install discord-webhook\n```\n\n## Examples\n\n* [Basic Webhook](#basic-webhook)\n* [Create Multiple Instances / Use multiple URLs](#create-multiple-instances)\n* [Get Webhook by ID](#get-webhook-by-id)\n* [Manage Being Rate Limited](#manage-being-rate-limited)\n* [Embedded Content](#webhook-with-embedded-content)\n* [Edit Webhook Message](#edit-webhook-messages)\n* [Delete Webhook Message](#delete-webhook-messages)\n* [Send Files](#send-files)\n* [Remove Embeds and Files](#remove-embeds-and-files)\n* [Allowed Mentions](#allowed-mentions)\n* [Use Proxies](#use-proxies)\n* [Timeout](#timeout)\n* [Async Support](#async-support)\n\n### Basic Webhook\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message")\nresponse = webhook.execute()\n```\n\n### Create multiple instances\nIf you want to use multiple URLs you need to create multiple instances.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# you can provide any kwargs except url\nwebhook1, webhook2 = DiscordWebhook.create_batch(urls=["first url", "second url"], content="Webhook Message")\nresponse1 = webhook1.execute()\nresponse2 = webhook2.execute()\n```\n![Image](img/multiple_urls.png "Multiple Urls Result")\n\n### Get Webhook by ID\nYou can access a webhook that has already been sent by providing the ID.\n\n````python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", id="your webhook message id")\n# now you could delete or edit the webhook\n# ...\n````\n\n### Manage being Rate Limited\n\n```python\nfrom discord_webhook import DiscordWebhook\n\n# if rate_limit_retry is True then in the event that you are being rate \n# limited by Discord your webhook will automatically be sent once the \n# rate limit has been lifted\nwebhook = DiscordWebhook(url="your webhook url", rate_limit_retry=True, content="Webhook Message")\nresponse = webhook.execute()\n```\n\n![Image](img/basic_webhook.png "Basic Example Result")\n\n### Webhook with Embedded Content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\n# create embed object for webhook\n# you can set the color as a decimal (color=242424) or hex (color="03b2f8") number\nembed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/simple_embed.png "Basic Embed Example Result")\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\n# create embed object for webhook\nembed = DiscordEmbed(title="Your Title", description="Lorem ipsum dolor sit", color="03b2f8")\n\n# set author\nembed.set_author(name="Author Name", url="author url", icon_url="author icon url")\n\n# set image\nembed.set_image(url="your image url")\n\n# set thumbnail\nembed.set_thumbnail(url="your thumbnail url")\n\n# set footer\nembed.set_footer(text="Embed Footer Text", icon_url="URL of icon")\n\n# set timestamp (default is now) accepted types are int, float and datetime\nembed.set_timestamp()\n\n# add fields to embed\nembed.add_embed_field(name="Field 1", value="Lorem ipsum")\nembed.add_embed_field(name="Field 2", value="dolor sit")\n\n# add embed object to webhook\nwebhook.add_embed(embed)\n\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed.png "Basic Embed Example Result")\n\nThis is another example with embedded content\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_author(name="Author Name", url="https://github.com/lovvskillz", icon_url="https://avatars0.githubusercontent.com/u/14542790")\nembed.set_footer(text="Embed Footer Text")\nembed.set_timestamp()\nembed.add_embed_field(name="Field 1", value="Lorem ipsum")\nembed.add_embed_field(name="Field 2", value="dolor sit")\nembed.add_embed_field(name="Field 3", value="amet consetetur")\nembed.add_embed_field(name="Field 4", value="sadipscing elitr")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed2.png "Example Embed Result")\n\nBy Default, the Embed fields are placed side by side. We can arrange them in a new line by setting `inline=False` as follows:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url", username="New Webhook Username")\n\nembed = DiscordEmbed(\n    title="Embed Title", description="Your Embed Description", color="03b2f8"\n)\nembed.set_author(\n    name="Author Name",\n    url="https://github.com/lovvskillz",\n    icon_url="https://avatars0.githubusercontent.com/u/14542790",\n)\nembed.set_footer(text="Embed Footer Text")\nembed.set_timestamp()\n# Set `inline=False` for the embed field to occupy the whole line\nembed.add_embed_field(name="Field 1", value="Lorem ipsum", inline=False)\nembed.add_embed_field(name="Field 2", value="dolor sit", inline=False)\nembed.add_embed_field(name="Field 3", value="amet consetetur")\nembed.add_embed_field(name="Field 4", value="sadipscing elitr")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n![Image](img/extended_embed3.png "Example Non-Inline Embed Result")\n\n### Edit Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook content before edit")\nwebhook.execute()\nwebhook.content = "After Edit"\nsleep(10)\nwebhook.edit()\n```\n\n### Delete Webhook Messages\n\n```python\nfrom discord_webhook import DiscordWebhook\nfrom time import sleep\n\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Content")\nwebhook.execute()\nsleep(10)\nwebhook.delete()\n```\n\n### Send Files\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example2.jpg")\n\nresponse = webhook.execute()\n```\n\n![Image](img/webhook_files.png "Example Files Result")\n\nYou can use uploaded attachments in Embeds:\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_thumbnail(url="attachment://example.jpg")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute()\n```\n\n### Remove Embeds and Files\n\n```python\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\nwebhook = DiscordWebhook(url="your webhook url")\n\nwith open("path/to/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\nembed.set_thumbnail(url="attachment://example.jpg")\n\nwebhook.add_embed(embed)\nresponse = webhook.execute(remove_embeds=True)\n# webhook.embeds will be empty after webhook is executed\n# You could also manually call the function webhook.remove_embeds()\n```\n\n`.remove_file()` removes the given file\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nwebhook = DiscordWebhook(url="your webhook url", username="Webhook with files")\n\n# send two images\nwith open("path/to/first/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example.jpg")\nwith open("path/to/second/image.jpg", "rb") as f:\n    webhook.add_file(file=f.read(), filename="example2.jpg")\n# remove "example.jpg"\nwebhook.remove_file("example.jpg")\n# only "example2.jpg" is sent to the webhook\nresponse = webhook.execute()\n```\n\n### Allowed Mentions\n\nLook into the [Discord Docs](https://discord.com/developers/docs/resources/channel#allowed-mentions-object) for examples and for more explanation\n\nThis example would only ping user `123` and `124` but not everyone else.\n\n```python\nfrom discord_webhook import DiscordWebhook\n\ncontent = "@everyone say hello to our new friends <@123> and <@124>"\nallowed_mentions = {\n    "users": ["123", "124"]\n}\n\nwebhook = DiscordWebhook(url="your webhook url", content=content, allowed_mentions=allowed_mentions)\nresponse = webhook.execute()\n```\n\n### Use Proxies\n\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  "http": "http://10.10.1.10:3128",\n  "https": "http://10.10.1.10:1080",\n}\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message", proxies=proxies)\nresponse = webhook.execute()\n```\nor\n```python\nfrom discord_webhook import DiscordWebhook\n\nproxies = {\n  "http": "http://10.10.1.10:3128",\n  "https": "http://10.10.1.10:1080",\n}\nwebhook = DiscordWebhook(url="your webhook url", content="Webhook Message")\nwebhook.set_proxies(proxies)\nresponse = webhook.execute()\n```\n\n### Timeout\n\n```python\nfrom requests.exceptions import Timeout\nfrom discord_webhook import DiscordWebhook, DiscordEmbed\n\n# We will set ridiculously low timeout threshold for testing purposes\nwebhook = DiscordWebhook(url="your webhook url", timeout=0.1)\n\n# You can also set timeout later using\n# webhook.timeout = 0.1\n\nembed = DiscordEmbed(title="Embed Title", description="Your Embed Description", color="03b2f8")\n\nwebhook.add_embed(embed)\n\n# Handle timeout exception\ntry:\n    response = webhook.execute()\nexcept Timeout as err:\n    print(f"Oops! Connection to Discord timed out: {err}")\n```\n\n### Async support\nIn order to use the async version, you need to install the package using:\n```\npip install discord-webhook[async]\n```\nExample usage:\n```python\nimport asyncio\nfrom discord_webhook import AsyncDiscordWebhook\n\n\nasync def send_webhook(message):\n    webhook = AsyncDiscordWebhook(url="your webhook url", content=message)\n    await webhook.execute()\n\n\nasync def main():\n    await asyncio.gather(\n        send_webhook("Async webhook message 1"),\n        send_webhook("Async webhook message 2"),\n    )  # sends both messages asynchronously\n\n\nasyncio.run(main())\n```\n\n### Use CLI\n\n```\nusage: discord_webhook [-h] -u URL [URL ...] -c CONTENT [--username USERNAME]\n                       [--avatar_url AVATAR_URL]\n\nTrigger discord webhook(s).\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u URL [URL ...], --url URL [URL ...]\n                        Webhook(s) url(s)\n  -c CONTENT, --content CONTENT\n                        Message content\n  --username USERNAME   override the default username of the webhook\n  --avatar_url AVATAR_URL\n                        override the default avatar of the webhook\n```\n\n## Development\n\n### Dev Setup\nThis project uses [Poetry](https://python-poetry.org/docs/) for dependency management and packaging.\n\nInstall Poetry and add Poetry to [Path](https://python-poetry.org/docs/#installation).\n\n**Debian / Ubuntu / Mac**\n\n`curl -sSL https://install.python-poetry.org | python3 -`\n\n**Windows**\n\nopen powershell and run: `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`\n\nInstall dependencies: `poetry install`\n\nInstall the defined pre-commit hooks: `poetry run pre-commit install`\n\nActivate the virtualenv: `poetry shell`',
     'author': 'lovvskillz',
     'author_email': '14542790+lovvskillz@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lovvskillz/python-discord-webhook',
```

### Comparing `discord-webhook-1.2.0/PKG-INFO` & `discord-webhook-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-webhook
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easily send Discord webhooks with Python
 Home-page: https://github.com/lovvskillz/python-discord-webhook
 License: MIT
 Keywords: discord,webhook
 Author: lovvskillz
 Author-email: 14542790+lovvskillz@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

