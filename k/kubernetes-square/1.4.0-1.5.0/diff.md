# Comparing `tmp/kubernetes_square-1.4.0.tar.gz` & `tmp/kubernetes_square-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes_square-1.4.0.tar", max compression
+gzip compressed data, was "kubernetes_square-1.5.0.tar", max compression
```

## Comparing `kubernetes_square-1.4.0.tar` & `kubernetes_square-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.4.0/LICENSE
--rw-r--r--   0        0        0      761 2023-07-22 06:51:23.778235 kubernetes_square-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3531 2023-07-22 06:18:28.743886 kubernetes_square-1.4.0/resources/defaultconfig.yaml
--rw-r--r--   0        0        0     1382 2023-07-22 06:51:23.778235 kubernetes_square-1.4.0/square/__init__.py
--rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.4.0/square/__main__.py
--rw-r--r--   0        0        0     4897 2023-07-22 06:18:28.711887 kubernetes_square-1.4.0/square/cfgfile.py
--rw-r--r--   0        0        0     2452 2023-07-22 06:08:22.385613 kubernetes_square-1.4.0/square/dotdict.py
--rw-r--r--   0        0        0     8551 2023-07-22 06:18:28.731886 kubernetes_square-1.4.0/square/dtypes.py
--rw-r--r--   0        0        0    33705 2023-07-22 06:18:28.683888 kubernetes_square-1.4.0/square/k8s.py
--rw-r--r--   0        0        0    14837 2023-07-22 06:18:28.743886 kubernetes_square-1.4.0/square/main.py
--rw-r--r--   0        0        0    39290 2023-07-22 06:18:28.747886 kubernetes_square-1.4.0/square/manio.py
--rw-r--r--   0        0        0    29846 2023-07-22 06:18:28.735886 kubernetes_square-1.4.0/square/square.py
--rw-r--r--   0        0        0     2068 2023-07-22 06:18:28.739886 kubernetes_square-1.4.0/square/yaml_io.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 kubernetes_square-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.5.0/LICENSE
+-rw-r--r--   0        0        0      701 2023-07-29 08:50:02.005888 kubernetes_square-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3531 2023-07-22 06:18:28.743886 kubernetes_square-1.5.0/resources/defaultconfig.yaml
+-rw-r--r--   0        0        0     1376 2023-07-29 08:50:02.005888 kubernetes_square-1.5.0/square/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.5.0/square/__main__.py
+-rw-r--r--   0        0        0     4858 2023-07-23 05:29:00.549037 kubernetes_square-1.5.0/square/cfgfile.py
+-rw-r--r--   0        0        0     2452 2023-07-22 06:08:22.385613 kubernetes_square-1.5.0/square/dotdict.py
+-rw-r--r--   0        0        0     8427 2023-07-23 06:08:32.331674 kubernetes_square-1.5.0/square/dtypes.py
+-rw-r--r--   0        0        0    31412 2023-07-23 06:08:32.331674 kubernetes_square-1.5.0/square/k8s.py
+-rw-r--r--   0        0        0    14826 2023-07-23 05:29:00.549037 kubernetes_square-1.5.0/square/main.py
+-rw-r--r--   0        0        0    38762 2023-07-29 08:50:06.777865 kubernetes_square-1.5.0/square/manio.py
+-rw-r--r--   0        0        0    29780 2023-07-29 08:50:06.781865 kubernetes_square-1.5.0/square/square.py
+-rw-r--r--   0        0        0     2068 2023-07-22 06:18:28.739886 kubernetes_square-1.5.0/square/yaml_io.py
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 kubernetes_square-1.5.0/PKG-INFO
```

### Comparing `kubernetes_square-1.4.0/LICENSE` & `kubernetes_square-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.4.0/pyproject.toml` & `kubernetes_square-1.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 [tool.poetry]
 name = "kubernetes-square"
-version = "1.4.0"
+version = "1.5.0"
 description = ""
 authors = ["Oliver Nagy <olitheolix@gmail.com>"]
 packages = [
     { include = "square" },
 ]
 include = ["resources/defaultconfig.yaml"]
 
 
 [tool.poetry.dependencies]
 backoff = "*"
 colorama = "*"
 colorlog = "*"
-google = "*"
-google-api-python-client = "*"
+httpx = "*"
 jsonpatch = "*"
 pydantic = ">=2.0"
 python = ">=3.10"
 pyyaml = "*"
-requests = ">=2.31"
 
 [tool.poetry.dev-dependencies]
 bumpversion = "*"
 flake8 = "*"
 flake8-isort = "*"
 ipython = ">=8.10"
 isort = "*"
 pytest = ">=7.2"
 pytest-cov = "*"
 pytest-dotenv = "*"
 pytest-flake8 = "*"
-requests-mock = "*"
+respx = "*"
 sh = "*"
 
 [tool.poetry.scripts]
 square = 'square.main:main'
 
 [build-system]
 requires = ["poetry>=1.2"]
```

### Comparing `kubernetes_square-1.4.0/resources/defaultconfig.yaml` & `kubernetes_square-1.5.0/resources/defaultconfig.yaml`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.4.0/square/__init__.py` & `kubernetes_square-1.5.0/square/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import pathlib
 import sys
+from pathlib import Path
 
 from . import square
 from .cfgfile import load
 
-__version__ = '1.4.0'
+__version__ = '1.5.0'
 
 
 # ---------------------------------------------------------------------------
 # Global Runtime Constants
 # ---------------------------------------------------------------------------
 # Determine the base folder. This is usually the folder of this very file, but
 # will be different if we run inside a bundle produced by PyInstaller.
 if getattr(sys, '_MEIPASS', None):
-    BASE_DIR = pathlib.Path(getattr(sys, '_MEIPASS'))
+    BASE_DIR = Path(getattr(sys, '_MEIPASS'))
 else:
-    BASE_DIR = pathlib.Path(__file__).parent.parent
+    BASE_DIR = Path(__file__).parent.parent
 
 # Square will source all its default values from this configuration file. The
 # only exceptions are the namespaces. By default, Square will target all the
 # namespaces whereas the specimen only declares "default" unless the user
 # explicitly says otherwise via the command line arguments or ".square.yaml".
 DEFAULT_CONFIG_FILE = BASE_DIR / "resources" / "defaultconfig.yaml"
 DEFAULT_CONFIG, err = load(DEFAULT_CONFIG_FILE)
```

### Comparing `kubernetes_square-1.4.0/square/cfgfile.py` & `kubernetes_square-1.5.0/square/cfgfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 dangerous, for Square to compute diffs on such field or patch them.
 
 This module defines utility functions to define these filters.
 
 """
 import copy
 import logging
+from pathlib import Path
 from types import SimpleNamespace
 from typing import Tuple
 
 import pydantic
 import yaml
 
-from square.dtypes import Config, Filepath
+from square.dtypes import Config
 
 from .dtypes import FiltersKind
 
 # Convenience.
 logit = logging.getLogger("square")
 
 
@@ -92,22 +93,21 @@
         # and only key as the comparative element).
         dst.sort(key=lambda _: _ if isinstance(_, str) else tuple(_.keys())[0])
 
     _update(src, dst)
     return dst
 
 
-def load(fname: Filepath) -> Tuple[Config, bool]:
+def load(fname: Path) -> Tuple[Config, bool]:
     """Parse the Square configuration file `fname` and return it as a `Config`."""
-    err_resp = Config(folder=Filepath(""), kubeconfig=Filepath("")), True
-    fname = Filepath(fname)
+    err_resp = Config(folder=Path(), kubeconfig=Path()), True
 
     # Load the configuration file.
     try:
-        raw = yaml.safe_load(Filepath(fname).read_text())
+        raw = yaml.safe_load(fname.read_text())
     except FileNotFoundError as e:
         logit.error(f"Cannot load config file <{fname}>: {e.args[1]}")
         return err_resp
     except yaml.YAMLError as exc:
         msg = f"Could not parse YAML file {fname}"
 
         # Special case: parser supplied location information.
```

### Comparing `kubernetes_square-1.4.0/square/dotdict.py` & `kubernetes_square-1.5.0/square/dotdict.py`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.4.0/square/dtypes.py` & `kubernetes_square-1.5.0/square/dtypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import pathlib
+from pathlib import Path
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Set, Tuple
 
 from pydantic import BaseModel, Field
 
-# All files in Square have this type.
-Filepath = pathlib.Path
-
 # Square will first save/deploy the resources in this list in this order.
 # Afterwards it will move on to all those resources not in this list. The order
 # in which it does that is undefined.
 DEFAULT_PRIORITIES = (
     # Custom Resources should come first.
     "CustomResourceDefinition",
 
@@ -36,16 +33,16 @@
 )
 
 
 # -----------------------------------------------------------------------------
 #                                  Kubernetes
 # -----------------------------------------------------------------------------
 class K8sClientCert(NamedTuple):
-    crt: Filepath = Filepath()
-    key: Filepath = Filepath()
+    crt: Path = Path()
+    key: Path = Path()
 
 
 class MetaManifest(NamedTuple):
     """Minimum amount of information to uniquely identify a K8s resource.
 
     The primary purpose of this tuple is to provide an immutable UUID that
     we can use as keys in dictionaries and sets.
@@ -72,18 +69,18 @@
 class K8sConfig(NamedTuple):
     """Everything we need to know to connect and authenticate with Kubernetes."""
     url: str = ""               # Kubernetes API
     token: str = ""             # Optional access token (eg Minikube).
 
     # Certificate authority credentials and self signed client certificate.
     # Used to authenticate to eg GKE.
-    ca_cert: Filepath = Filepath()
+    ca_cert: Path = Path()
     client_cert: Optional[K8sClientCert] = None
 
-    # A persistent session from the "requests" library for this cluster.
+    # HttpX client to access the cluster.
     client: Any = None
 
     # Kubernetes version and name.
     version: str = ""
     name: str = ""
 
     # Kubernetes API endpoints (see k8s.compile_api_endpoints).
@@ -217,18 +214,18 @@
 FiltersKind = List[str | dict]
 Filters = Dict[str, FiltersKind]
 
 
 class Config(BaseModel):
     """Uniform interface into top level Square API."""
     # Path to local manifests eg "./foo"
-    folder: Filepath
+    folder: Path
 
     # Path to Kubernetes credentials.
-    kubeconfig: Filepath
+    kubeconfig: Path
 
     # Kubernetes context (use `None` to use the default).
     kubecontext: Optional[str] = None
 
     # Only operate on resources that match the selectors.
     selectors: Selectors = Selectors()
 
@@ -247,10 +244,10 @@
 
     version: str = ""
 
 
 # -----------------------------------------------------------------------------
 #                                 Miscellaneous
 # -----------------------------------------------------------------------------
-LocalManifests = Dict[Filepath, Tuple[MetaManifest, dict]]
-LocalManifestLists = Dict[Filepath, List[Tuple[MetaManifest, dict]]]
+LocalManifests = Dict[Path, Tuple[MetaManifest, dict]]
+LocalManifestLists = Dict[Path, List[Tuple[MetaManifest, dict]]]
 SquareManifests = Dict[MetaManifest, dict]
```

### Comparing `kubernetes_square-1.4.0/square/k8s.py` & `kubernetes_square-1.5.0/square/k8s.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 import base64
 import json
 import logging
 import os
-import pathlib
 import re
+import ssl
 import subprocess
 import tempfile
-import warnings
 from collections import defaultdict
-from typing import Dict, List, Optional, Set, Tuple, cast
+from pathlib import Path
+from typing import Dict, List, Optional, Set, Tuple
 
 import backoff
-import google.auth
-import google.auth.exceptions
-import google.auth.transport.requests
-import requests
+import httpx
 import yaml
 
-from square.dtypes import (
-    Filepath, K8sClientCert, K8sConfig, K8sResource, MetaManifest,
-)
+from square.dtypes import K8sClientCert, K8sConfig, K8sResource, MetaManifest
 
-FNAME_TOKEN = Filepath("/var/run/secrets/kubernetes.io/serviceaccount/token")
-FNAME_CERT = Filepath("/var/run/secrets/kubernetes.io/serviceaccount/ca.crt")
+FNAME_TOKEN = Path("/var/run/secrets/kubernetes.io/serviceaccount/token")
+FNAME_CERT = Path("/var/run/secrets/kubernetes.io/serviceaccount/ca.crt")
 
 
 # Convenience: global logger instance to avoid repetitive code.
 logit = logging.getLogger("square")
 
 
-def load_kubeconfig(fname: Filepath,
+def load_kubeconfig(kubeconf_path: Path,
                     context: Optional[str]) -> Tuple[str, dict, dict, bool]:
-    """Return user name and user- and cluster information.
+    """Return user name as well as user- and cluster information.
 
     Return None on error.
 
     Inputs:
-        fname: Filepath
+        kubeconf_path: Path
             Path to kubeconfig file, eg "~/.kube/config.yaml"
         context: Optional[str]
-            Kubeconf context. Use `None` to get the default context.
+            Kubeconf context. Use `None` to select the default context.
 
     Returns:
         name, user info, cluster info
 
     """
     # Load `kubeconfig`.
     try:
-        kubeconf = yaml.safe_load(open(fname))
+        kubeconf = yaml.safe_load(open(kubeconf_path))
     except (IOError, PermissionError) as err:
         logit.error(f"{err}")
         return ("", {}, {}, True)
 
     # Find the user and cluster information based on the specified `context`.
     try:
         # Use default context unless specified.
@@ -78,44 +73,43 @@
         # Unpack the cluster- and user information.
         cluster_name = cluster_info[0]["name"]
         cluster_info_out = cluster_info[0]["cluster"]
         cluster_info_out["name"] = cluster_name
         user_info = user_info[0]["user"]
         del cluster_info
     except (KeyError, TypeError):
-        logit.error(f"Kubeconfig YAML file <{fname}> is invalid")
+        logit.error(f"Kubeconfig YAML file <{kubeconf_path}> is invalid")
         return ("", {}, {}, True)
 
     # Success. The explicit `dicts()` are to satisfy MyPy.
-    logit.info(f"Loaded {ctx} from Kubeconfig file <{fname}>")
+    logit.info(f"Loaded {ctx} from Kubeconfig file <{kubeconf_path}>")
     return (username, dict(user_info), dict(cluster_info_out), False)
 
 
 def load_incluster_config(
-        fname_token: Filepath = FNAME_TOKEN,
-        fname_cert: Filepath = FNAME_CERT) -> Tuple[K8sConfig, bool]:
+        fname_token: Path = FNAME_TOKEN,
+        fname_cert: Path = FNAME_CERT) -> Tuple[K8sConfig, bool]:
     """Return K8s access config from Pod service account.
 
     Returns None if we are not running in a Pod.
 
     Inputs:
         kubconfig: str
             Name of kubeconfig file.
     Returns:
-        Config
+        K8sConfig
 
     """
-    # Every K8s pod has this.
+    # These exist inside every Kubernetes pod.
     server_ip = os.getenv('KUBERNETES_PORT_443_TCP_ADDR', None)
+    fname_cert = Path(fname_cert)
+    fname_token = Path(fname_token)
 
-    fname_cert = pathlib.Path(fname_cert)
-    fname_token = pathlib.Path(fname_token)
-
-    # Sanity checks: URL and service account files either exist, or we are not
-    # actually inside a Pod.
+    # Sanity checks: URL and service account must exist, or we are not running
+    # inside a Pod.
     try:
         assert server_ip is not None
         assert fname_cert.exists()
         assert fname_token.exists()
     except AssertionError:
         logit.debug("Could not find incluster (service account) credentials.")
         return K8sConfig(), True
@@ -128,244 +122,177 @@
         ca_cert=fname_cert,
         client_cert=None,
         version="",
         name="",
     ), False
 
 
-def load_gke_config(
-        fname: Filepath,
-        context: Optional[str],
-        disable_warnings: bool = False) -> Tuple[K8sConfig, bool]:
-    """Return K8s access config for GKE cluster described in `kubeconfig`.
-
-    Returns None if `kubeconfig` does not exist or could not be parsed.
-
-    Inputs:
-        kubconfig: str
-            Name of kubeconfig file.
-        context: str
-            Kubeconf context. Use `None` to use default context.
-        disable_warnings: bool
-            Whether or not do disable GCloud warnings.
-
-    Returns:
-        Config
-
-    """
-    # Parse the kubeconfig file.
-    _, _, cluster, err = load_kubeconfig(fname, context)
-    if err:
-        return (K8sConfig(), True)
-
-    # Unpack the self signed certificate (Google does not register the K8s API
-    # server certificate with a public CA).
-    try:
-        ssl_ca_cert_data = base64.b64decode(cluster["certificate-authority-data"])
-    except KeyError:
-        logit.debug(f"Context {context} in <{fname}> is not a GKE config")
-        return (K8sConfig(), True)
-
-    # Save the certificate to a temporary file. This is only necessary because
-    # the requests library will need a path to the CA file - unfortunately, we
-    # cannot just pass it the content.
-    _, tmp = tempfile.mkstemp(text=False)
-    ssl_ca_cert = Filepath(tmp)
-    ssl_ca_cert.write_bytes(ssl_ca_cert_data)
-
-    with warnings.catch_warnings(record=disable_warnings):
-        try:
-            cred, _ = google.auth.default(
-                scopes=['https://www.googleapis.com/auth/cloud-platform']
-            )
-            cred.refresh(google.auth.transport.requests.Request())
-            token = cred.token
-        except google.auth.exceptions.DefaultCredentialsError as e:
-            logit.error(str(e))
-            return (K8sConfig(), True)
-
-    # Return the config data.
-    logit.info("Assuming GKE cluster.")
-    return K8sConfig(
-        url=cluster["server"],
-        token=cast(str, token),
-        ca_cert=ssl_ca_cert,
-        client_cert=None,
-        version="",
-        name=cluster["name"],
-    ), False
-
-
-def load_eks_config(
-        fname: Filepath,
-        context: Optional[str],
-        _: bool = False) -> Tuple[K8sConfig, bool]:
-    """Return K8s access config for EKS cluster described in `kubeconfig`.
+def load_authenticator_config(kubeconf_path: Path,
+                              context: Optional[str]) -> Tuple[K8sConfig, bool]:
+    """Return K8s config based on authenticator app specified in `kubeconfig`.
 
     Returns None if `kubeconfig` does not exist or could not be parsed.
 
     Inputs:
-        fname: Filepath
-            Kubeconfig file.
-        context: str
-            Kubeconf context. Use `None` to use default context.
-        disable_warnings: bool (unused)
-            Not used. It only exists for consistency with `load_gke_config` to
-            make those functions generic.
+        kubeconf_path: Path
+            Path to kubeconfig file, eg "~/.kube/config.yaml"
+        context: Optional[str]
+            Kubeconf context. Use `None` to select the default context.
 
     Returns:
-        Config
+        K8sConfig
 
     """
     # Parse the kubeconfig file.
-    user, cluster, err = load_kubeconfig(fname, context)[1:]
+    user, cluster, err = load_kubeconfig(kubeconf_path, context)[1:]
     if err:
         return (K8sConfig(), True)
 
     # Get a copy of all env vars. We will pass that one along to the
     # sub-process, plus the env vars specified in the kubeconfig file.
     env = os.environ.copy()
 
     # Unpack the self signed certificate (AWS does not register the K8s API
     # server certificate with a public CA).
     try:
         ssl_ca_cert_data = base64.b64decode(cluster["certificate-authority-data"])
         cmd = user["exec"]["command"]
-        args = user["exec"]["args"]
+        args = user["exec"].get("args", [])
         env_kubeconf = user["exec"].get("env", [])
     except KeyError:
-        logit.debug(f"Context {context} in <{fname}> is not an EKS config")
+        logit.debug(
+            f"Context {context} in <{kubeconf_path}> does not use authenticator app"
+        )
         return (K8sConfig(), True)
 
     # Convert a None value (valid value in YAML) to an empty list of env vars.
     env_kubeconf = env_kubeconf if env_kubeconf else []
 
-    # Save the certificate to a temporary file. This is only necessary because
-    # the Requests library will need a path to the CA file - unfortunately, we
-    # cannot just pass it the content.
+    # Save the certificate to a temporary file because Httpx expects it that way.
     tmp = tempfile.mkstemp(text=False)[1]
-    ssl_ca_cert = Filepath(tmp)
+    ssl_ca_cert = Path(tmp)
     ssl_ca_cert.write_bytes(ssl_ca_cert_data)
 
     # Compile the name, arguments and env vars for the command specified in kubeconf.
     cmd_args = [cmd] + args
     env_kubeconf = {_["name"]: _["value"] for _ in env_kubeconf}
     env.update(env_kubeconf)
-    logit.debug(f"Requesting EKS certificate: {cmd_args} with envs: {env_kubeconf}")
+    logit.debug(f"Authenticator app: {cmd_args} with envs: {env_kubeconf}")
 
     # Pre-format the command for the log message.
     log_cmd = (
-        f"kubeconf={fname} kubectx={context} "
+        f"kubeconf={kubeconf_path} kubectx={context} "
         f"cmd={cmd_args}  env={env_kubeconf}"
     )
 
     # Run the specified command to produce the access token. That program must
     # produce a YAML document on stdout that specifies the bearer token.
     try:
         out = subprocess.run(cmd_args, stdout=subprocess.PIPE, env=env)
         token = yaml.safe_load(out.stdout.decode("utf8"))["status"]["token"]
     except FileNotFoundError:
         logit.error(f"Could not find {cmd} application to get token ({log_cmd})")
         return (K8sConfig(), True)
     except (KeyError, yaml.YAMLError):
-        logit.error(f"Token manifest produce by {cmd_args} is corrupt ({log_cmd})")
+        logit.error(f"Token manifest produced by {cmd_args} is corrupt ({log_cmd})")
         return (K8sConfig(), True)
     except TypeError:
         logit.error(f"The YAML token produced by {cmd_args} is corrupt ({log_cmd})")
         return (K8sConfig(), True)
 
-    # Return the config data.
-    logit.info("Assuming EKS cluster.")
+    # Return the Kubernetes access configuration.
+    logit.info("Assuming generic cluster.")
     return K8sConfig(
         url=cluster["server"],
         token=token,
         ca_cert=ssl_ca_cert,
         client_cert=None,
         version="",
         name=cluster["name"],
     ), False
 
 
-def load_minikube_config(fname: Filepath,
+def load_minikube_config(kubeconf_path: Path,
                          context: Optional[str]) -> Tuple[K8sConfig, bool]:
     """Load minikube configuration from `fname`.
 
     Return None on error.
 
     Inputs:
-        fname: Filepath
+        kubeconf_path: Path
             Path to kubeconfig file, eg "~/.kube/config.yaml"
-        context: str
-            Kubeconf context. Use `None` to select default context.
+        context: Optional[str]
+            Kubeconf context. Use `None` to select the default context.
 
     Returns:
-        Config
+        K8sConfig
 
     """
     # Parse the kubeconfig file.
-    _, user, cluster, err = load_kubeconfig(fname, context)
+    _, user, cluster, err = load_kubeconfig(kubeconf_path, context)
     if err:
         return (K8sConfig(), True)
 
     # Minikube uses client certificates to authenticate. We need to pass those
-    # to the HTTP client of our choice when we create the session.
+    # to the HTTP client of our choice
     try:
         client_cert = K8sClientCert(
-            crt=Filepath(user["client-certificate"]),
-            key=Filepath(user["client-key"]),
+            crt=Path(user["client-certificate"]),
+            key=Path(user["client-key"]),
         )
 
-        # Return the config data.
+        # Return the Kubernetes access configuration.
         logit.info("Assuming Minikube cluster.")
         return K8sConfig(
             url=cluster["server"],
             token="",
-            ca_cert=Filepath(cluster["certificate-authority"]),
+            ca_cert=Path(cluster["certificate-authority"]),
             client_cert=client_cert,
             version="",
             name=cluster["name"],
         ), False
     except KeyError:
-        logit.debug(f"Context {context} in <{fname}> is not a Minikube config")
+        logit.debug(f"Context {context} in <{kubeconf_path}> is not a Minikube config")
         return (K8sConfig(), True)
 
 
-def load_kind_config(fname: Filepath, context: Optional[str]) -> Tuple[K8sConfig, bool]:
+def load_kind_config(kubeconf_path: Path,
+                     context: Optional[str]) -> Tuple[K8sConfig, bool]:
     """Load Kind configuration from `fname`.
 
     https://github.com/bsycorp/kind
 
     Kind is just another Minikube cluster. The only notable difference
     is that it does not store its credentials as files but directly in
     the Kubeconfig file. This function will copy those files into /tmp.
 
     Return None on error.
 
     Inputs:
-        kubconfig: str
-            Path to kubeconfig for Kind cluster.
-        context: str
-            Kubeconf context. Use `None` to use default context.
+        kubeconf_path: Path
+            Path to kubeconfig file, eg "~/.kube/config.yaml"
+        context: Optional[str]
+            Kubeconf context. Use `None` to select the default context.
 
     Returns:
-        Config
+        K8sConfig
 
     """
     # Parse the kubeconfig file.
-    _, user, cluster, err = load_kubeconfig(fname, context)
+    _, user, cluster, err = load_kubeconfig(kubeconf_path, context)
     if err:
         return (K8sConfig(), True)
 
     # Kind and Minikube use client certificates to authenticate. We need to
-    # pass those to the HTTP client of our choice when we create the session.
+    # pass those to the HTTP client of our choice.
     try:
         client_crt = base64.b64decode(user["client-certificate-data"]).decode()
         client_key = base64.b64decode(user["client-key-data"]).decode()
         client_ca = base64.b64decode(cluster["certificate-authority-data"]).decode()
-        path = Filepath(tempfile.mkdtemp())
+        path = Path(tempfile.mkdtemp())
         p_client_crt = path / "kind-client.crt"
         p_client_key = path / "kind-client.key"
         p_ca = path / "kind.ca"
         p_client_crt.write_text(client_crt)
         p_client_key.write_text(client_key)
         p_ca.write_text(client_ca)
         client_cert = K8sClientCert(crt=p_client_crt, key=p_client_key)
@@ -377,89 +304,95 @@
             token="",
             ca_cert=p_ca,
             client_cert=client_cert,
             version="",
             name=cluster["name"],
         ), False
     except KeyError:
-        logit.debug(f"Context {context} in <{fname}> is not a Minikube config")
+        logit.debug(
+            f"Context {context} in <{kubeconf_path}> is not a Minikube config"
+        )
         return (K8sConfig(), True)
 
 
-def load_auto_config(
-        fname: Filepath,
-        context: Optional[str],
-        disable_warnings: bool = False) -> Tuple[K8sConfig, bool]:
+def load_auto_config(kubeconf_path: Path,
+                     context: Optional[str]) -> Tuple[K8sConfig, bool]:
     """Automagically find and load the correct K8s configuration.
 
-    This function will load several possible configuration options and returns
-    the first one with a match. The order is as follows:
+    This function will sequentially load all supported authentication schemes
+    until one fits.
 
-    1) `load_incluster_config`
-    2) `load_gke_config`
+    1) `load_authenticator_config`
+    2) `load_incluster_config`
+    3) `load_kind_config`
+    4) `load_minikube_config`
 
     Inputs:
-        fname: str
+        kubeconf_path: Path
             Path to kubeconfig file, eg "~/.kube/config.yaml"
-            Use `None` to find out automatically or for incluster credentials.
-
-        context: str
-            Kubeconf context. Use `None` to use default context.
+        context: Optional[str]
+            Kubeconf context. Use `None` to select the default context.
 
     Returns:
-        Config
+        K8sConfig
 
     """
-    conf, err = load_incluster_config()
+    conf, err = load_authenticator_config(kubeconf_path, context)
     if not err:
         return conf, False
-    logit.debug("Incluster config failed")
+    logit.debug("Authenticator config failed")
 
-    conf, err = load_minikube_config(fname, context)
+    conf, err = load_incluster_config()
     if not err:
         return conf, False
-    logit.debug("Minikube config failed")
+    logit.debug("Incluster config failed")
 
-    conf, err = load_kind_config(fname, context)
+    conf, err = load_kind_config(kubeconf_path, context)
     if not err:
         return conf, False
     logit.debug("KIND config failed")
 
-    conf, err = load_eks_config(fname, context, disable_warnings)
-    if not err:
-        return conf, False
-    logit.debug("EKS config failed")
-
-    conf, err = load_gke_config(fname, context, disable_warnings)
+    conf, err = load_minikube_config(kubeconf_path, context)
     if not err:
         return conf, False
-    logit.debug("GKE config failed")
+    logit.debug("Minikube config failed")
 
-    logit.error(f"Could not find a valid configuration in <{fname}>")
+    logit.error(f"Could not find a valid configuration in <{kubeconf_path}>")
     return (K8sConfig(), True)
 
 
-def session(k8sconfig: K8sConfig):
-    """Return configured `requests` session."""
-    # Plain session.
-    sess = requests.Session()
-
-    # Load the CA file (necessary for self signed certs to avoid https warning).
-    sess.verify = str(k8sconfig.ca_cert)
+def create_httpx_client(k8sconfig: K8sConfig) -> Tuple[httpx.Client, bool]:
+    """Return configured HttpX client."""
+    # Configure Httpx client with the K8s service account token.
+    cafile = None if str(k8sconfig.ca_cert) == "." else k8sconfig.ca_cert
+    ssl_context = ssl.create_default_context(cafile=cafile)
 
     # Add the client certificate, if the cluster uses those to authenticate users.
     if k8sconfig.client_cert is not None:
-        sess.cert = (str(k8sconfig.client_cert.crt), str(k8sconfig.client_cert.key))
+        cert = (k8sconfig.client_cert.crt, k8sconfig.client_cert.key)
+    else:
+        cert = None
 
-    # Add the bearer token if this cluster uses them to authenticate users.
-    if k8sconfig.token is not None:
-        sess.headers.update({'authorization': f'Bearer {k8sconfig.token}'})
+    # Construct the HttpX client.
+    try:
+        client = httpx.Client(verify=ssl_context, cert=cert)  # type: ignore
+    except ssl.SSLError:
+        logit.error("Invalid certificates")
+        return httpx.Client(), True
+    except FileNotFoundError:
+        # If the certificate files do not exist then we have a bug somewhere.
+        logit.error("Bug: certificate files do not exist")
+        return httpx.Client(), True
+
+    # Add the bearer token if we have one.
+    if k8sconfig.token != "":
+        client.headers.update({'authorization': f'Bearer {k8sconfig.token}'})
 
-    # Return the configured session object.
-    return sess
+    # Return the configured client object.
+    return client, False
 
 
 def resource(k8sconfig: K8sConfig, meta: MetaManifest) -> Tuple[K8sResource, bool]:
     """Return `K8sResource` object.
 
     That object will contain the full path to a resource, eg.
     https://1.2.3.4/api/v1/namespace/foo/services.
@@ -546,35 +479,38 @@
         method: str,
         url: str,
         payload: Optional[dict | list],
         headers: Optional[dict]) -> Tuple[dict, bool]:
     """Return response of web request made with `client`.
 
     Inputs:
-        client: `requests` session with correct K8s certificates.
+        client: HttpX client with correct K8s certificates.
         url: str
             Eg `https://1.2.3.4/api/v1/namespaces`)
         payload: dict
             Anything that can be JSON encoded, usually a K8s manifest.
         headers: dict
             Request headers. These will *not* replace the existing request
             headers dictionary (eg the access tokens), but augment them.
 
     Returns:
         (dict, int): the JSON response and the HTTP status code.
 
     """
     # Define the maximum number of tries and exceptions we want to retry on.
     max_tries = 21
-    web_exceptions = (requests.exceptions.RequestException, )
+    web_exceptions = (httpx.RequestError, )
 
     def on_backoff(details):
         """Log a warning whenever we retry."""
-        tries = details["tries"]
-        logit.warning(f"Backing off on {url} (Attempt {tries}/{max_tries-1})")
+        tries, exc = details["tries"], details["exception"]
+        logit.warning(
+            f"Backing off on {url}. Attempt {tries}/{max_tries-1}. "
+            f"Reason: {exc}"
+        )
 
     """
     Use linear backoff. The backoff is not exponential because the most
     prevalent use case for this backoff we have seen so far is to wait for
     new resource endpoints to become available. These may take a few seconds,
     or tens of seconds to do so. If we used an exponential strategy we may
     end up waiting for a very long time for no good reason. The time between
@@ -653,19 +589,17 @@
     err = (code != 201)
     if err:
         logit.error(f"{code} - POST - {url} - {resp}")
     return (resp, err)
 
 
 def version(k8sconfig: K8sConfig) -> Tuple[K8sConfig, bool]:
-    """Return new `k8sconfig` with version number of K8s API.
+    """Return copy of `k8sconfig` but with current Kubernetes version.
 
-    Contact the K8s API, query its version via `client` and return `k8sconfig`
-    with an updated `version` field. All other field in `k8sconfig` will remain
-    intact.
+    All other fields in the provided `k8sconfig` will remain the same.
 
     Inputs:
         k8sconfig: K8sConfig
 
     Returns:
         K8sConfig
 
@@ -677,54 +611,51 @@
         logit.error(f"Could not interrogate {k8sconfig.name} ({url})")
         return (K8sConfig(), True)
 
     # Construct the version number of the K8s API.
     major, minor = resp['major'], resp['minor']
     version = f"{major}.{minor}"
 
-    # If we are talking to GKE, the version string may now be "1.10+". It
-    # simply indicates that GKE is running version 1.10.x. We need to remove
-    # the "+" because the version string is important in `square`, for instance
-    # to determines which URLs to contact, which fields are valid.
-    version = version.replace("+", "")
-
     # Return an updated `K8sconfig` tuple.
     k8sconfig = k8sconfig._replace(version=version)
     return (k8sconfig, False)
 
 
 def cluster_config(
-        kubeconfig: Filepath,
+        kubeconfig: Path,
         context: Optional[str]) -> Tuple[K8sConfig, bool]:
-    """Return web session to K8s API.
+    """Return the `K8sConfig` to connect to the API.
 
-    This will read the Kubernetes credentials, contact Kubernetes to
-    interrogate its version and then return the configuration and web-session.
+    This will read the Kubernetes credentials, create a client and use it to
+    fetch the Kubernetes version.
 
     Inputs:
-        kubeconfig: str
+        kubeconfig: Path
             Path to kubeconfig file.
         context: str
             Kubernetes context to use (can be `None` to use default).
 
     Returns:
         K8sConfig
 
     """
-    # Read Kubeconfig file and use it to create a `requests` client session.
-    # That session will have the proper security certificates and headers so
-    # that subsequent calls to K8s need not deal with it anymore.
+    # Create a HttpX client based on the Kubeconfig file. It will have the
+    # proper certificates and headers to connect to K8s.
     kubeconfig = kubeconfig.expanduser()
     try:
         # Parse Kubeconfig file.
-        k8sconfig, err = load_auto_config(kubeconfig, context, disable_warnings=True)
+        k8sconfig, err = load_auto_config(kubeconfig, context)
+        assert not err
+
+        # Configure a HttpX client for this cluster.
+        client, err = create_httpx_client(k8sconfig)
         assert not err
 
-        # Configure web session.
-        k8sconfig = k8sconfig._replace(client=session(k8sconfig))
+        # Add the web client to the `k8sconfig` object.
+        k8sconfig = k8sconfig._replace(client=client)
         assert k8sconfig.client
 
         # Contact the K8s API to update version field in `k8sconfig`.
         k8sconfig, err = version(k8sconfig)
         assert not err and k8sconfig
 
         # Populate the `k8sconfig.apis` field.
```

### Comparing `kubernetes_square-1.4.0/square/main.py` & `kubernetes_square-1.5.0/square/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import argparse
 import logging
 import os
+from pathlib import Path
 from typing import Any, Dict, Optional, Tuple
 
 import colorama
 
 import square
 import square.k8s
 import square.square
 from square import DEFAULT_CONFIG_FILE, __version__
-from square.dtypes import Config, Filepath, GroupBy, Selectors
+from square.dtypes import Config, GroupBy, Selectors
 
 # Convenience: global logger instance to avoid repetitive code.
 logit = logging.getLogger("square")
 
 
 def parse_commandline_args():
     """Return parsed command line."""
@@ -162,51 +163,51 @@
         cmdline_param: SimpleNamespace
 
     Returns:
         Config, err
 
     """
     err_resp = Config(
-        folder=Filepath(""),
-        kubeconfig=Filepath(""),
+        folder=Path(""),
+        kubeconfig=Path(""),
         kubecontext=None,
         selectors=Selectors(),
         groupby=GroupBy(label="", order=[]),
         priorities=[],
     ), True
 
     # Convenience.
     p = cmdline_param
 
     # Load the default configuration unless the user specified an explicit one.
     if p.configfile:
         logit.info(f"Loading configuration file <{p.configfile}>")
-        cfg, err = square.cfgfile.load(p.configfile)
+        cfg, err = square.cfgfile.load(Path(p.configfile))
 
         # Look for `--kubeconfig`. Defaults to the value in config file.
         kubeconfig = p.kubeconfig or cfg.kubeconfig
     else:
         # Pick the configuration file. Depends on whether the user specified
         # `--no-config`, `--config` and if `.square.yaml` exists.
         default_cfg = DEFAULT_CONFIG_FILE
-        dot_square = Filepath(".square.yaml")
+        dot_square = Path(".square.yaml")
 
         if p.no_config:
             cfg_file = default_cfg
         else:
             cfg_file = dot_square if dot_square.exists() else default_cfg
 
         logit.info(f"Loading configuration file <{cfg_file}>")
         cfg, err = square.cfgfile.load(cfg_file)
 
         # Determine which Kubeconfig to use. The order is: `--kubeconfig`,
         # `--config`, `.square`, `KUBECONFIG` environment variable.
         if cfg_file == default_cfg:
             kubeconfig = p.kubeconfig or os.getenv("KUBECONFIG", "")
-            cfg.folder = Filepath.cwd()
+            cfg.folder = Path.cwd()
         else:
             kubeconfig = p.kubeconfig or str(cfg.kubeconfig) or os.getenv("KUBECONFIG", "")  # noqa
 
         del dot_square, default_cfg
 
         # Abort if neither `--kubeconfig` nor the KUBECONFIG environment variable exist.
         if not kubeconfig:
@@ -215,16 +216,16 @@
     if err:
         return err_resp
 
     # Override the folder if user specified "--folder".
     folder = cfg.folder if p.folder is None else p.folder
 
     # Expand the user's home folder, ie if the path contains a "~".
-    folder = Filepath(folder).expanduser()
-    kubeconfig = Filepath(kubeconfig).expanduser()
+    folder = Path(folder).expanduser()
+    kubeconfig = Path(kubeconfig).expanduser()
 
     # ------------------------------------------------------------------------
     # GroupBy (determines the folder hierarchy that GET will create).
     # In : `--groupby ns kind label=app`
     # Out: GroupBy(order=["ns", "kind", "label"], label="app")
     # ------------------------------------------------------------------------
     # Unpack the ordering and replace all `label=*` with `label`.
@@ -263,15 +264,15 @@
     # ------------------------------------------------------------------------
     # General: folder, kubeconfig, kubecontext, ...
     # ------------------------------------------------------------------------
     kinds = set(p.kinds) if p.kinds else cfg.selectors.kinds
 
     # Use the value from the (default) config file unless the user overrode
     # them on the command line.
-    kubeconfig = Filepath(kubeconfig)
+    kubeconfig = Path(kubeconfig)
     kubecontext = p.kubecontext or cfg.kubecontext
     namespaces = cfg.selectors.namespaces if p.namespaces is None else p.namespaces
     sel_labels = cfg.selectors.labels if p.labels is None else p.labels
     priorities = p.priorities or cfg.priorities
     selectors = Selectors(kinds=kinds, namespaces=namespaces, labels=sel_labels)
 
     # Use filters from (default) config file because they cannot be specified
@@ -384,15 +385,15 @@
     # Print version information and quit.
     if param.parser == "version":
         print(__version__)
         return 0
 
     # Create a default ".square.yaml" in the current folder and quit.
     if param.parser == "config":
-        fname = Filepath(param.folder or ".") / ".square.yaml"
+        fname = Path(param.folder or ".") / ".square.yaml"
         fname.parent.mkdir(parents=True, exist_ok=True)
         fname.write_text(DEFAULT_CONFIG_FILE.read_text())
         print(
             f"Created configuration file <{fname}>.\n"
             "Please open the file in an editor and adjust the values, most notably "
             "`kubeconfig` and `selectors.[kinds | namespaces | labels]`."
         )
```

### Comparing `kubernetes_square-1.4.0/square/manio.py` & `kubernetes_square-1.5.0/square/manio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import collections
 import copy
 import difflib
 import logging
 import multiprocessing
-import pathlib
+from pathlib import Path
 from typing import DefaultDict, Dict, Iterable, List, Optional, Tuple, cast
 
 import yaml.parser
 import yaml.scanner
 
 import square.cfgfile
 import square.dotdict
 import square.k8s
 from square.dtypes import (
-    Config, Filepath, Filters, FiltersKind, GroupBy, K8sConfig, K8sResource,
-    KindName, LocalManifestLists, MetaManifest, Selectors, SquareManifests,
+    Config, Filters, FiltersKind, GroupBy, K8sConfig, K8sResource, KindName,
+    LocalManifestLists, MetaManifest, Selectors, SquareManifests,
 )
 from square.yaml_io import Dumper, Loader
 
 # Convenience: global logger instance to avoid repetitive code.
 logit = logging.getLogger("square")
 DotDict = square.dotdict.DotDict
 
@@ -173,15 +173,15 @@
         manifest["kind"] = kind
         manifest['apiVersion'] = apiversion
         if select(manifest, selectors):
             manifests[make_meta(manifest)] = manifest
     return (manifests, False)
 
 
-def _parse_worker(fname: Filepath,
+def _parse_worker(fname: Path,
                   yaml_str: str) -> Tuple[List[dict], bool]:
     logit.debug(f"Parsing <{fname}>")
 
     # Decode the YAML documents in the current file.
     try:
         manifests = list(yaml.load_all(yaml_str, Loader=Loader))
         return manifests, False
@@ -191,22 +191,22 @@
         logit.error(
             f"Cannot YAML parse <{fname}>"
             f" - {err.problem} - Line {line}"
         )
         return ([], True)
 
 
-def parse(file_yaml: Dict[Filepath, str],
+def parse(file_yaml: Dict[Path, str],
           selectors: Selectors) -> Tuple[LocalManifestLists, bool]:
     """Parse all YAML strings from `file_yaml` into `LocalManifestLists`.
 
     Exclude all manifests that do not satisfy the `selectors`.
 
     Inputs:
-        file_yaml: Dict[Filepath, str]
+        file_yaml: Dict[Path, str]
             Raw data as returned by `load_files`.
         selectors: Selectors
             Skip all manifests that do not match these `selectors`.
 
     Returns:
         LocalManifestLists: The YAML parsed manifests of each file.
 
@@ -300,23 +300,23 @@
 def sync(local_manifests: LocalManifestLists,
          server_manifests: SquareManifests,
          selectors: Selectors,
          groupby: GroupBy) -> Tuple[LocalManifestLists, bool]:
     """Update the local manifests with the server values and return the result.
 
     Inputs:
-        local_manifests: Dict[Filepath, Tuple[MetaManifest, dict]]
+        local_manifests: Dict[Path, Tuple[MetaManifest, dict]]
         server_manifests: Dict[MetaManifest, dict]
         selectors: Selectors
             Only operate on resources that match the selectors.
         groupby: GroupBy
             Specify relationship between new manifests and file names.
 
     Returns:
-        Dict[Filepath, List[Tuple[MetaManifest, dict]]]
+        Dict[Path, List[Tuple[MetaManifest, dict]]]
 
     """
     # Avoid side effects.
     server_manifests = copy.deepcopy(server_manifests)
 
     # Only retain server manifests that match the selectors.
     server_manifests = {
@@ -344,15 +344,15 @@
         for idx, (meta, _) in enumerate(local_manifests[fname]):
             meta_to_fname[meta] = (fname, idx)
             del meta
         del fname
 
     # Make a copy of the local manifests to avoid side effects for the caller.
     # Also put it into a default dict for convenience.
-    out_add_mod: DefaultDict[Filepath, List[Tuple[MetaManifest, dict]]]
+    out_add_mod: DefaultDict[Path, List[Tuple[MetaManifest, dict]]]
     out_add_mod = collections.defaultdict(list)
     out_add_mod.update(copy.deepcopy(local_manifests))
     del local_manifests
 
     # If the server's meta manifest exists locally then update the local one,
     # otherwise add it to the catchall YAML file.
     for meta, manifest in server_manifests.items():
@@ -377,35 +377,35 @@
         out_add_mod_del[fname] = pruned
 
     return (out_add_mod_del, False)
 
 
 def filename_for_manifest(
         meta: MetaManifest, manifest: dict,
-        grouping: GroupBy) -> Tuple[Filepath, bool]:
+        grouping: GroupBy) -> Tuple[Path, bool]:
     """Return the file for the manifest based on `groupby`.
 
     Inputs:
         meta: MetaManifest
         manifest: dict
         groupby: GroupBy
 
     Output:
-        Filepath
+        Path
 
     """
     # --- Sanity checks ---
     if not set(grouping.order).issubset({"ns", "kind", "label"}):
         logit.error(f"Invalid resource ordering: {grouping.order}")
-        return Filepath(), True
+        return Path(), True
 
     if "label" in grouping.order:
         if len(grouping.label) == 0:
             logit.error("Must specify a non-empty label when grouping by it")
-            return Filepath(), True
+            return Path(), True
 
     # Convenience: reliably extract a label dictionary even when the original
     # manifest has none.
     labels = manifest.get("metadata", {}).get("labels", {})
 
     # Helper LookUpTable that contains the values for all those groups the
     # "--groupby" command line option accepts. We will use this LUT below to
@@ -427,15 +427,15 @@
     # "--groupby" option on the command line.
     path_constituents = [lut[_] for _ in grouping.order]
     path = str.join("/", path_constituents)
 
     # Default to the catch-all `_other.yaml` resource if the order did not
     # produce a file name. This typically happens when `grouping.order = []`.
     path = "_other.yaml" if path == "" else f"{path}.yaml"
-    return Filepath(path), False
+    return Path(path), False
 
 
 def diff(local: dict, server: dict) -> Tuple[str, bool]:
     """Return the human readable diff between the `local` and `server` manifest.
 
     The diff shows the necessary changes to transition the `server` manifest
     into the state of the `local` manifest.
@@ -678,31 +678,28 @@
         if srv_token and not loc_token:
             loc_secrets.append({"name": srv_token})
             local_manifests[meta]["secrets"] = loc_secrets
 
     return (local_manifests, False)
 
 
-def save_files(folder: Filepath, file_data: Dict[Filepath, str]) -> bool:
+def save_files(folder: Path, file_data: Dict[Path, str]) -> bool:
     """Save all `file_data` under `folder`.
 
     All paths in `file_data` are relative to `folder`.
 
     Inputs:
-        folder: Filepath
-        file_data: Dict[Filepath, str]
+        folder: Path
+        file_data: Dict[Path, str]
             The file name (relative to `folder`) and its content.
 
     Returns:
         None
 
     """
-    # Python's `pathlib.Path` objects are simply nicer to work with...
-    folder = pathlib.Path(folder)
-
     # Delete all YAML files under `folder`. This avoids stale manifests.
     try:
         for fp in folder.rglob("*.yaml"):
             logit.info(f"Removing stale <{fp}>")
             fp.unlink()
     except (IOError, PermissionError) as err:
         logit.error(f"{err}")
@@ -728,16 +725,16 @@
             return True
 
     # Tell caller that all files were successfully written.
     return False
 
 
 def load_files(
-        folder: Filepath,
-        fnames: Iterable[Filepath]) -> Tuple[Dict[Filepath, str], bool]:
+        folder: Path,
+        fnames: Iterable[Path]) -> Tuple[Dict[Path, str], bool]:
     """Load all `fnames` in `folder` and return their content.
 
     This is a convenience function for Square to recursively load all manifests
     in a given manifest folder. It will either return the content of all files,
     or an error. In particular, it will never return only a sub-set of files.
 
     The elements of `fname` can have sub-paths, eg `foo/bar/file.txt` is valid
@@ -745,107 +742,100 @@
 
     Inputs:
         folder: Path
         fnames: Iterable[str|Path]
             The file names relative to `folder`.
 
     Returns:
-        Dict[Filepath, str]: the file names (relative to `folder`) and their
+        Dict[Path, str]: the file names (relative to `folder`) and their
         content as a string.
 
     """
-    # Python's `pathlib.Path` objects are simply nicer to work with...
-    folder = pathlib.Path(folder)
-
     # Load each file and store its name and content in the `out` dictionary.
-    out: Dict[Filepath, str] = {}
+    out: Dict[Path, str] = {}
     for fname_rel in fnames:
         # Construct absolute file path.
         fname_abs = folder / fname_rel
         logit.debug(f"Loading {fname_abs}")
 
         # Read the file. Abort on error.
         try:
-            # The str() is necessary because `fname_rel` may be a `pathlib.Path`.
             out[fname_rel] = fname_abs.read_text()
         except FileNotFoundError:
             logit.error(f"Could not find <{fname_abs}>")
             return ({}, True)
 
     # Return the read files.
     return (out, False)
 
 
-def load_manifests(folder: Filepath,
+def load_manifests(folder: Path,
                    selectors: Selectors) -> Tuple[SquareManifests,
                                                   LocalManifestLists, bool]:
     """Return all K8s manifest found in `folder`.
 
     Recursively load all "*.yaml" files in `folder` and return those manifests
     that match the `selectors`.
 
     It will either return all manifests or none, if there was an error. In
     particular, it will never return only a sub-set of files (cf `load_files`).
 
     NOTE: this is merely a wrapper around the various low-level functions to
     load and parse YAML files.
 
     Input:
-        folder: Filepath
+        folder: Path
         selectors: Selectors
 
     Returns:
         (local manifest without file info, local manifests with file info)
 
     """
-    # Python's `pathlib.Path` objects are simply nicer to work with...
-    folder = pathlib.Path(folder)
-
     # Compile the list of all YAML files in `folder` but only store their path
     # relative to `folder`.
     fnames = [(_.relative_to(folder), _.name) for _ in folder.rglob("*.yaml")]
     fnames = [path for path, name in fnames if not name.startswith(".")]
 
     try:
         # Load the files and abort on error.
         fdata_raw, err = load_files(folder, fnames)
         assert not err and fdata_raw is not None
 
         # Return the YAML parsed manifests.
         man_files, err = parse(fdata_raw, selectors)
         assert not err and man_files is not None
 
-        # Remove the Filepath dimension.
+        # Remove the Path dimension.
         man_meta, err = compile_square_manifests(man_files)
         assert not err and man_meta is not None
     except AssertionError:
         return ({}, {}, True)
 
     # Return the file based manifests and unpacked manifests.
     return (man_meta, man_files, False)
 
 
 def sort_manifests(
         file_manifests: LocalManifestLists,
         priority: List[str]
-) -> Tuple[Dict[Filepath, List[dict]], bool]:
+) -> Tuple[Dict[Path, List[dict]], bool]:
     """Sort the manifests in each `file_manifests` by their `priority`.
 
     The returned data contains only the manifests without the `MetaData`. The
     idea is to pass that data directly to `save_files`.
 
     Inputs:
         file_manifests: the manifests that should go into each file.
         priority: List[str]
             Sort the manifest in this order, or alphabetically at the end if
             not in the list.
 
     """
     # Sort the manifests in each file.
-    out: Dict[Filepath, List[dict]] = {}
+    out: Dict[Path, List[dict]] = {}
     for fname, manifests in file_manifests.items():
         # Group the manifests by their "kind" in order of `priority` and sort
         # each group alphabetically.
         man_sorted: list = []
         for kind in priority:
             # Partition the manifest list into the current `kind` and the rest.
             tmp = [_ for _ in manifests if _[0].kind == kind]
@@ -874,35 +864,35 @@
 
         # Assign the grouped and sorted list of manifests to the output dict.
         out[fname] = man_clean
 
     return out, False
 
 
-def save(folder: Filepath,
+def save(folder: Path,
          manifests: LocalManifestLists,
          priority: List[str]) -> bool:
     """Saves all `manifests` as YAMLs in `folder`.
 
     Input:
-        folder: Filepath
+        folder: Path
             Source folder.
-        file_manifests: Dict[Filepath, Tuple(MetaManifest, dict)]
+        file_manifests: Dict[Path, Tuple(MetaManifest, dict)]
             Names of files and their Python dicts to save as YAML.
         priority: List[str]
             Sort the manifest in this order, or alphabetically at the end if
             not in the list.
 
     Returns:
         None
 
     """
     # Sort the manifest in each file by priority. Ignore the error flag because
     # `sort_manifests` always succeeds.
-    # out: Dict[FilePath, List[dict]]
+    # out: Dict[Path, List[dict]]
     out, _ = sort_manifests(manifests, priority)
 
     # Ignore all files without manifests, ie empty files.
     out_nonempty = {k: v for k, v in out.items() if len(v) > 0}
     del out
 
     # Ensure that our list of manifests does not contain any `DotDicts`
@@ -913,16 +903,16 @@
     }
     del out_nonempty
 
     # Ignore all hidden files.
     out_clean = {k: v for k, v in out_clean.items() if not k.name.startswith(".")}
 
     # Convert all manifest dicts into YAML strings.
-    out_final: Dict[Filepath, str] = {}
-    fname: Filepath = Filepath()
+    out_final: Dict[Path, str] = {}
+    fname: Path = Path()
     try:
         for fname, v in out_clean.items():
             out_final[fname] = yaml.dump_all(v, default_flow_style=False,
                                              Dumper=Dumper)
     except yaml.YAMLError as e:
         logit.error(
             f"YAML error. Cannot create <{fname}>: {e.args[0]} <{str(e.args[1])}>"
```

### Comparing `kubernetes_square-1.4.0/square/square.py` & `kubernetes_square-1.5.0/square/square.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,15 +683,15 @@
     if not all([valid_label(_) for _ in cfg.selectors.labels]):
         logit.error(f"Invalid labels: {cfg.selectors.labels}")
         return True
 
     # Sort the plan according to `cfg.priority`.
     plan, plan_err = sort_plan(cfg, plan)
 
-    # Create properly configured "Requests" session to talk to the K8s API.
+    # Get an HttpX client to talk to the K8s API.
     k8sconfig, k8s_err = k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
 
     # Abort if we could not get the plan or establish the K8s session.
     if plan_err or k8s_err:
         return True
 
     # Convert "Selectors.kinds" to their canonical names.
@@ -738,15 +738,15 @@
     """
     # Sanity check labels.
     if not all([valid_label(_) for _ in cfg.selectors.labels]):
         logit.error(f"Invalid labels: {cfg.selectors.labels}")
         return DeploymentPlan(tuple(), tuple(), tuple()), True
 
     try:
-        # Create properly configured Requests session to talk to K8s API.
+        # Get an HttpX client to talk to the K8s API.
         k8sconfig, err = k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
         assert not err
 
         # Convert "Selectors.kinds" to their canonical names.
         cfg = translate_resource_kinds(cfg, k8sconfig)
 
         # Load manifests from local files.
@@ -775,15 +775,15 @@
     """Download all K8s manifests and merge them into local files."""
     # Sanity check labels.
     if not all([valid_label(_) for _ in cfg.selectors.labels]):
         logit.error(f"Invalid labels: {cfg.selectors.labels}")
         return True
 
     try:
-        # Create properly configured Requests session to talk to K8s API.
+        # Get an HttpX client to talk to the K8s API.
         k8sconfig, err = k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
         assert not err
 
         # Convert "Selectors.kinds" to their canonical names.
         cfg = translate_resource_kinds(cfg, k8sconfig)
 
         # Use a wildcard Selector to ensure `manio.load` will read _all_ local
```

### Comparing `kubernetes_square-1.4.0/square/yaml_io.py` & `kubernetes_square-1.5.0/square/yaml_io.py`

 * *Files identical despite different names*

