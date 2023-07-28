# Comparing `tmp/st-paywall-0.1.3.tar.gz` & `tmp/st-paywall-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-paywall-0.1.3.tar", last modified: Thu Jul 13 05:42:18 2023, max compression
+gzip compressed data, was "st-paywall-0.1.4.tar", last modified: Fri Jul 28 22:23:14 2023, max compression
```

## Comparing `st-paywall-0.1.3.tar` & `st-paywall-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.704770 st-paywall-0.1.3/
--rw-r--r--   0 trichards   (501) staff       (20)     7311 2023-07-13 05:42:18.704561 st-paywall-0.1.3/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     7054 2023-07-13 05:37:47.000000 st-paywall-0.1.3/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      396 2023-07-13 03:05:04.000000 st-paywall-0.1.3/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-13 05:42:18.704820 st-paywall-0.1.3/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.697859 st-paywall-0.1.3/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.701305 st-paywall-0.1.3/src/st_paywall/
--rw-r--r--   0 trichards   (501) staff       (20)       36 2023-07-10 04:34:35.000000 st-paywall-0.1.3/src/st_paywall/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     2089 2023-07-13 05:28:47.000000 st-paywall-0.1.3/src/st_paywall/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1218 2023-07-13 05:26:48.000000 st-paywall-0.1.3/src/st_paywall/buymeacoffee_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-10 04:34:35.000000 st-paywall-0.1.3/src/st_paywall/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1243 2023-07-13 05:31:13.000000 st-paywall-0.1.3/src/st_paywall/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-13 05:42:18.703538 st-paywall-0.1.3/src/st_paywall.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     7311 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      369 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-13 05:42:18.000000 st-paywall-0.1.3/src/st_paywall.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-28 22:23:14.245184 st-paywall-0.1.4/
+-rw-r--r--   0 trichards   (501) staff       (20)     3422 2023-07-28 22:23:14.244977 st-paywall-0.1.4/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     3166 2023-07-28 21:28:03.000000 st-paywall-0.1.4/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      392 2023-07-28 21:28:32.000000 st-paywall-0.1.4/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-28 22:23:14.245252 st-paywall-0.1.4/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-28 22:23:14.239776 st-paywall-0.1.4/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-28 22:23:14.242485 st-paywall-0.1.4/src/st_paywall/
+-rw-r--r--   0 trichards   (501) staff       (20)       45 2023-07-28 21:28:03.000000 st-paywall-0.1.4/src/st_paywall/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2278 2023-07-28 21:28:03.000000 st-paywall-0.1.4/src/st_paywall/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1414 2023-07-28 21:28:03.000000 st-paywall-0.1.4/src/st_paywall/buymeacoffee_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     3045 2023-07-28 21:28:03.000000 st-paywall-0.1.4/src/st_paywall/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1529 2023-07-28 21:28:03.000000 st-paywall-0.1.4/src/st_paywall/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-28 22:23:14.244616 st-paywall-0.1.4/src/st_paywall.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     3422 2023-07-28 22:23:14.000000 st-paywall-0.1.4/src/st_paywall.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      369 2023-07-28 22:23:14.000000 st-paywall-0.1.4/src/st_paywall.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-28 22:23:14.000000 st-paywall-0.1.4/src/st_paywall.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-28 22:23:14.000000 st-paywall-0.1.4/src/st_paywall.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       11 2023-07-28 22:23:14.000000 st-paywall-0.1.4/src/st_paywall.egg-info/top_level.txt
```

### Comparing `st-paywall-0.1.3/src/st_paywall/aggregate_auth.py` & `st-paywall-0.1.4/src/st_paywall/aggregate_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 import streamlit as st
 from .google_auth import get_logged_in_user_email, show_login_button
 from .stripe_auth import get_customer_emails, redirect_button
 from .buymeacoffee_auth import get_bmac_payers
 
 payment_provider = st.secrets.get("payment_provider", "stripe")
 
+
 def add_auth(required=True):
     if required:
         require_auth()
     else:
         optional_auth()
 
+
 def require_auth():
     user_email = get_logged_in_user_email()
 
     if not user_email:
         show_login_button()
         st.stop()
     if payment_provider == "stripe":
         customer_emails = get_customer_emails()
     elif payment_provider == "bmac":
         customer_emails = get_bmac_payers()
+    else:
+        raise ValueError("payment_provider must be 'stripe' or 'bmac'")
 
     if user_email not in customer_emails:
-        redirect_button(text="Subscribe now!",
-                        customer_email=user_email,
-                        payment_provider=payment_provider)
+        redirect_button(
+            text="Subscribe now!",
+            customer_email=user_email,
+            payment_provider=payment_provider,
+        )
         st.session_state.user_subscribed = False
         st.stop()
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.sidebar.button("Logout", type="primary"):
         del st.session_state.email
         del st.session_state.user_subscribed
         st.experimental_rerun()
 
+
 def optional_auth():
     user_email = get_logged_in_user_email()
     if payment_provider == "stripe":
         customer_emails = get_customer_emails()
     elif payment_provider == "bmac":
         customer_emails = get_bmac_payers()
+    else:
+        raise ValueError("payment_provider must be 'stripe' or 'bmac'")
 
     if not user_email:
         show_login_button()
         st.session_state.email = ""
         st.sidebar.markdown("")
 
     if user_email and user_email not in customer_emails:
-        redirect_button(text="Subscribe now!", customer_email="", payment_provider=payment_provider)
+        redirect_button(
+            text="Subscribe now!", customer_email="", payment_provider=payment_provider
+        )
         st.sidebar.markdown("")
         st.session_state.user_subscribed = False
 
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
     if st.session_state.email != "":
         if st.sidebar.button("Logout", type="primary"):
             del st.session_state.email
             del st.session_state.user_subscribed
-            st.experimental_rerun()
+            st.experimental_rerun()
```

### Comparing `st-paywall-0.1.3/src/st_paywall/buymeacoffee_auth.py` & `st-paywall-0.1.4/src/st_paywall/buymeacoffee_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,43 @@
+from __future__ import annotations
 import requests
 import streamlit as st
-bmac_api = st.secrets["bmac_api_key"]
+
 
 def extract_payer_emails(json_response):
     payer_emails = []
 
-    for item in json_response['data']:
-        payer_email = item['payer_email']
+    for item in json_response["data"]:
+        payer_email = item["payer_email"]
         payer_emails.append(payer_email)
 
     return payer_emails
 
-def get_bmac_payers(access_token=bmac_api, one_time=False):
-    if one_time == False:
+
+def get_bmac_payers(access_token: str | None = None, one_time: bool = False):
+    if access_token is None:
+        access_token = st.secrets["bmac_api_key"]
+
+    if one_time is False:
         url = "https://developers.buymeacoffee.com/api/v1/subscriptions?status=active"
         headers = {"Authorization": f"Bearer {access_token}"}
         response = requests.get(url, headers=headers)
 
         if response.status_code == 200:
             return extract_payer_emails(response.json())
         else:
-            raise Exception(f"Error fetching active subscriptions: {response.status_code} - {response.text}")
+            raise Exception(
+                "Error fetching active subscriptions: "
+                f"{response.status_code} - {response.text}"
+            )
     else:
         url = "https://developers.buymeacoffee.com/api/v1/supporters"
         headers = {"Authorization": f"Bearer {access_token}"}
         response = requests.get(url, headers=headers)
 
         if response.status_code == 200:
             return extract_payer_emails(response.json())
         else:
-            raise Exception(f"Error fetching active subscriptions: {response.status_code} - {response.text}")
+            raise Exception(
+                "Error fetching active subscriptions: "
+                f"{response.status_code} - {response.text}"
+            )
```

### Comparing `st-paywall-0.1.3/src/st_paywall/google_auth.py` & `st-paywall-0.1.4/src/st_paywall/google_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import asyncio
+from typing import Optional
 
 import jwt
 import streamlit as st
 from httpx_oauth.clients.google import GoogleOAuth2
+from httpx_oauth.oauth2 import OAuth2Token
 
 testing_mode = st.secrets.get("testing_mode", False)
 
 
 client_id = st.secrets["client_id"]
 client_secret = st.secrets["client_secret"]
-redirect_url = st.secrets["redirect_url_test"] if testing_mode else st.secrets["redirect_url"]
+redirect_url = (
+    st.secrets["redirect_url_test"] if testing_mode else st.secrets["redirect_url"]
+)
 
 client = GoogleOAuth2(client_id=client_id, client_secret=client_secret)
 
 
 def decode_user(token: str):
     """
     :param token: jwt token
     :return:
     """
     decoded_data = jwt.decode(jwt=token, options={"verify_signature": False})
 
     return decoded_data
 
 
-async def get_authorization_url(client: GoogleOAuth2, redirect_url: str):
+async def get_authorization_url(client: GoogleOAuth2, redirect_url: str) -> str:
     authorization_url = await client.get_authorization_url(
         redirect_url,
         scope=["email"],
         extras_params={"access_type": "offline"},
     )
     return authorization_url
 
 
 def markdown_button(
-    url: str, text: str | None = None, color="#FD504D", sidebar: bool = True
+    url: str, text: Optional[str] = None, color="#FD504D", sidebar: bool = True
 ):
     markdown = st.sidebar.markdown if sidebar else st.markdown
 
     markdown(
         f"""
     <a href="{url}" target="_blank">
         <div style="
@@ -63,22 +67,26 @@
         </div>
     </a>
     """,
         unsafe_allow_html=True,
     )
 
 
-async def get_access_token(client: GoogleOAuth2, redirect_url: str, code: str):
+async def get_access_token(
+    client: GoogleOAuth2, redirect_url: str, code: str
+) -> OAuth2Token:
     token = await client.get_access_token(code, redirect_url)
     return token
 
 
-def get_access_token_from_query_params(client: GoogleOAuth2, redirect_url: str) -> str:
+def get_access_token_from_query_params(
+    client: GoogleOAuth2, redirect_url: str
+) -> OAuth2Token:
     query_params = st.experimental_get_query_params()
-    code = query_params["code"]
+    code = query_params["code"][0]
     token = asyncio.run(
         get_access_token(client=client, redirect_url=redirect_url, code=code)
     )
     # Clear query params
     st.experimental_set_query_params()
     return token
 
@@ -86,15 +94,15 @@
 def show_login_button():
     authorization_url = asyncio.run(
         get_authorization_url(client=client, redirect_url=redirect_url)
     )
     markdown_button(authorization_url, "Login with Google")
 
 
-def get_logged_in_user_email() -> str | None:
+def get_logged_in_user_email() -> Optional[str]:
     if "email" in st.session_state:
         return st.session_state.email
 
     try:
         token_from_params = get_access_token_from_query_params(client, redirect_url)
     except KeyError:
         return None
```

### Comparing `st-paywall-0.1.3/src/st_paywall/stripe_auth.py` & `st-paywall-0.1.4/src/st_paywall/stripe_auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import streamlit as st
 import stripe
 import urllib.parse
 
-testing_mode = st.secrets.get("testing_mode", False)
-stripe.api_key = st.secrets["stripe_api_key_test"] if testing_mode else st.secrets["stripe_api_key"]
-stripe_link = st.secrets["stripe_link_test"] if testing_mode else st.secrets["stripe_link"]
+
+def get_api_key() -> str:
+    testing_mode = st.secrets.get("testing_mode", False)
+    return (
+        st.secrets["stripe_api_key_test"]
+        if testing_mode
+        else st.secrets["stripe_api_key"]
+    )
 
 
 def redirect_button(
     text: str,
     customer_email: str,
     color="#FD504D",
     payment_provider: str = "stripe",
 ):
+    testing_mode = st.secrets.get("testing_mode", False)
+    stripe.api_key = get_api_key()
+    stripe_link = (
+        st.secrets["stripe_link_test"] if testing_mode else st.secrets["stripe_link"]
+    )
     encoded_email = urllib.parse.quote(customer_email)
     if payment_provider == "stripe":
         button_url = f"{stripe_link}?prefilled_email={encoded_email}"
     elif payment_provider == "bmac":
         button_url = f"{st.secrets['bmac_link']}"
+    else:
+        raise ValueError("payment_provider must be 'stripe' or 'bmac'")
 
     st.sidebar.markdown(
         f"""
     <a href="{button_url}" target="_blank">
         <div style="
             display: inline-block;
             padding: 0.5em 1em;
@@ -34,12 +46,13 @@
     </a>
     """,
         unsafe_allow_html=True,
     )
 
 
 def get_customer_emails():
+    stripe.api_key = get_api_key()
     customers = stripe.Customer.list()
     emails = []
     for i in customers["data"]:
         emails.append(i["email"])
     return emails
```

