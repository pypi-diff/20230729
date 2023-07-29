# Comparing `tmp/tomodachi_testcontainers-0.2.1.tar.gz` & `tmp/tomodachi_testcontainers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.2.1.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.2.2.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.2.1.tar` & `tomodachi_testcontainers-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.1/LICENSE
--rw-r--r--   0        0        0    26475 2023-07-27 14:17:21.581583 tomodachi_testcontainers-0.2.1/README.md
--rw-r--r--   0        0        0     3649 2023-07-27 15:28:09.358579 tomodachi_testcontainers-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     2918 2023-07-27 15:28:03.606413 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    27664 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.2/LICENSE
+-rw-r--r--   0        0        0    26649 2023-07-29 08:49:13.268083 tomodachi_testcontainers-0.2.2/README.md
+-rw-r--r--   0        0        0     3734 2023-07-29 08:49:20.113888 tomodachi_testcontainers-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     2465 2023-07-29 06:48:22.554642 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     3855 2023-07-29 08:49:13.268726 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1346 2023-07-29 07:46:42.840748 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    27838 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.2/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.2.1/LICENSE` & `tomodachi_testcontainers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/README.md` & `tomodachi_testcontainers-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,15 @@
 by setting it in the shell before running `pytest`.
 
 | Environment Variable                      | Description                                                                                                                   |
 | :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
 | `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
 | `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
 | `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
+| `DOCKER_BUILDKIT`                         | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit in `EphemeralDockerImage`                                                      |
 
 ## Changing default Docker network
 
 By default, testcontainers are started in the default `bridge` Docker network.
 Sometimes it's useful to start containers in a different network, e.g. a network
 specifically dedicated for running automated tests.
```

### Comparing `tomodachi_testcontainers-0.2.1/pyproject.toml` & `tomodachi_testcontainers-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.2.1"
+version = "0.2.2"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -46,21 +46,23 @@
 flake8-simplify = "^0.20.0"
 flake8-use-pathlib = "^0.3.0"
 flake8-warnings = "^0.4.0"
 httpx = "^0.24.1"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pre-commit = ">=3.3.3"
+protobuf = "^4.23.4"
 pydantic = "^2.0.2"
 pylint = "^2.17.4"
 pytest-cov = "^4.1.0"
 pytest-env = "^0.8.2"
-ruff = "^0.0.277"
+ruff = ">=0.0.277,<0.0.281"
 structlog = "^23.1.0"
 tomodachi = "^0.25.0"
+types-protobuf = "^4.23.0.2"
 
 [tool.poetry.extras]
 sftp = ["asyncssh"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -162,8 +164,9 @@
 junit_family = "xunit2"
 testpaths = ["tests"]
 norecursedirs = [".venv", "__pycache__", ".git"]
 log_cli_level = "INFO"
 env = [
     "TESTCONTAINER_DOCKER_NETWORK=tomodachi-testcontainers",
     "TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile",
+    "DOCKER_BUILDKIT=1",
 ]
```

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any, Dict, List, Protocol, Type, TypeVar, Union
+from typing import Any, List, Protocol, Type, TypeVar, Union
 
 from types_aiobotocore_sns import SNSClient
 from types_aiobotocore_sqs import SQSClient
 
 MessageType = TypeVar("MessageType")
 
 
@@ -39,22 +39,26 @@
     message_type: Type[MessageType],
     max_messages: int = 10,
 ) -> List[MessageType]:
     get_queue_url_response = await sqs_client.get_queue_url(QueueName=queue_name)
     queue_url = get_queue_url_response["QueueUrl"]
 
     received_messages_response = await sqs_client.receive_message(QueueUrl=queue_url, MaxNumberOfMessages=max_messages)
+    received_messages = received_messages_response.get("Messages")
+    if not received_messages:
+        return []
 
     parsed_messages: List[MessageType] = []
-    for message in received_messages_response["Messages"]:
-        parsed_message = await envelope.parse_message(json.loads(message["Body"])["Message"])
+    for received_message in received_messages:
+        payload = json.loads(received_message["Body"])["Message"]
+        parsed_message = await envelope.parse_message(payload=payload, proto_class=message_type)
         parsed_messages.append(parsed_message[0]["data"])
     return parsed_messages
 
 
-async def publish(sns_client: SNSClient, topic: str, data: Dict, envelope: TomodachiSNSSQSEnvelope) -> None:
+async def publish(sns_client: SNSClient, topic: str, data: Any, envelope: TomodachiSNSSQSEnvelope) -> None:
     message = await envelope.build_message(service={}, topic=topic, data=data)
 
     create_topic_response = await sns_client.create_topic(Name=topic)
     topic_arn = create_topic_response["TopicArn"]
 
     await sns_client.publish(TopicArn=topic_arn, Message=message)
```

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
-import pathlib
+import subprocess  # nosec: B404
+from pathlib import Path
 from typing import Any, Dict, Iterator, Optional, Tuple, cast
 
 import testcontainers.core.container
 from docker.errors import ImageNotFound
 from docker.models.images import Image as DockerImage
 from testcontainers.core.docker_client import DockerClient
 from testcontainers.core.utils import inside_container
@@ -32,47 +33,69 @@
 
     def get_container_gateway_ip(self) -> str:
         container = self.get_docker_client().get_container(self.get_wrapped_container().id)
         return container["NetworkSettings"]["Networks"][self.network]["Gateway"]
 
 
 class EphemeralDockerImage:
-    def __init__(self, dockerfile: pathlib.Path, docker_client_kw: Optional[Dict] = None) -> None:
+    def __init__(self, dockerfile: Path, docker_client_kw: Optional[Dict] = None) -> None:
         self.client = DockerClient(**(docker_client_kw or {}))
         self.image = self.build_image(dockerfile)
 
     def __enter__(self) -> DockerImage:
         return self.image
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.remove_image()
 
-    def build_image(self, path: pathlib.Path) -> DockerImage:
+    def build_image(self, path: Path) -> DockerImage:
         if path.is_dir():
             dockerfile_dir = path
             dockerfile_name = ""
         else:
             dockerfile_dir = path.parent
             dockerfile_name = path.name
 
+        if os.getenv("DOCKER_BUILDKIT"):
+            return self._build_with_docker_buildkit(dockerfile_dir, dockerfile_name)
+
+        return self._build_with_docker_client(dockerfile_dir, dockerfile_name)
+
+    def remove_image(self) -> None:
+        self.client.client.images.remove(image=str(self.image.id))
+
+    def _build_with_docker_buildkit(self, dockerfile_dir: Path, dockerfile_name: str) -> DockerImage:
+        filepath = dockerfile_dir / dockerfile_name
+
+        cmd = ["docker", "build", "-q", "--rm=true"]
+        if filepath.is_file():
+            cmd.extend(["-f", str(filepath)])
+        cmd.append(str(dockerfile_dir))
+
+        result = subprocess.run(  # nosec: B603
+            cmd,
+            shell=False,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            check=True,
+        )
+        image_id = result.stdout.decode("utf-8").strip()
+        return cast(DockerImage, self.client.client.images.get(image_id))
+
+    def _build_with_docker_client(self, dockerfile_dir: Path, dockerfile_name: str) -> DockerImage:
         image, _ = cast(
             Tuple[DockerImage, Iterator],
             self.client.client.images.build(
                 path=str(dockerfile_dir),
                 dockerfile=str(dockerfile_name),
                 forcerm=True,
             ),
         )
         return image
 
-    def remove_image(self) -> None:
-        self.client.client.images.remove(image=str(self.image.id))
-
 
-def get_docker_image(image_id: str, docker_client_kw: Optional[Dict] = None) -> Optional[DockerImage]:
+def get_docker_image(image_id: str, docker_client_kw: Optional[Dict] = None) -> DockerImage:
     client = DockerClient(**(docker_client_kw or {}))
-    if not image_id:
-        return None
     try:
         return cast(DockerImage, client.client.images.get(image_id))
     except ImageNotFound:
         return cast(DockerImage, client.client.images.pull(image_id))
```

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/moto.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
-import pathlib
+from pathlib import Path
 from typing import Generator
 
 import pytest
 from docker.models.images import Image as DockerImage
 
 from tomodachi_testcontainers.containers import EphemeralDockerImage, get_docker_image
 
 
 @pytest.fixture(scope="session")
 def tomodachi_image() -> Generator[DockerImage, None, None]:
-    if image := get_docker_image(os.environ.get("TOMODACHI_TESTCONTAINER_IMAGE_ID", "")):
-        yield image
+    if image_id := os.environ.get("TOMODACHI_TESTCONTAINER_IMAGE_ID"):
+        yield get_docker_image(image_id)
     else:
-        dockerfile = pathlib.Path(os.environ.get("TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH", "."))
+        dockerfile = Path(os.environ.get("TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH", "."))
         with EphemeralDockerImage(dockerfile) as image:
             yield image
```

### Comparing `tomodachi_testcontainers-0.2.1/PKG-INFO` & `tomodachi_testcontainers-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -507,14 +507,15 @@
 by setting it in the shell before running `pytest`.
 
 | Environment Variable                      | Description                                                                                                                   |
 | :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
 | `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
 | `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
 | `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
+| `DOCKER_BUILDKIT`                         | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit in `EphemeralDockerImage`                                                      |
 
 ## Changing default Docker network
 
 By default, testcontainers are started in the default `bridge` Docker network.
 Sometimes it's useful to start containers in a different network, e.g. a network
 specifically dedicated for running automated tests.
```

