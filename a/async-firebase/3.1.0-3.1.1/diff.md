# Comparing `tmp/async_firebase-3.1.0.tar.gz` & `tmp/async_firebase-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_firebase-3.1.0.tar", max compression
+gzip compressed data, was "async_firebase-3.1.1.tar", max compression
```

## Comparing `async_firebase-3.1.0.tar` & `async_firebase-3.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-04-11 15:56:14.529060 async_firebase-3.1.0/LICENSE
--rw-r--r--   0        0        0     8292 2023-04-11 15:56:14.529060 async_firebase-3.1.0/README.md
--rw-r--r--   0        0        0      194 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/__init__.py
--rw-r--r--   0        0        0     7906 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/base.py
--rw-r--r--   0        0        0    23182 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/client.py
--rw-r--r--   0        0        0     1547 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/encoders.py
--rw-r--r--   0        0        0     8142 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/errors.py
--rw-r--r--   0        0        0    16820 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/messages.py
--rw-r--r--   0        0        0    12977 2023-04-11 15:56:14.529060 async_firebase-3.1.0/async_firebase/utils.py
--rw-r--r--   0        0        0     1677 2023-04-11 15:56:14.533060 async_firebase-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     9394 1970-01-01 00:00:00.000000 async_firebase-3.1.0/setup.py
--rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 async_firebase-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-10 12:55:54.782004 async_firebase-3.1.1/LICENSE
+-rw-r--r--   0        0        0     8292 2023-05-10 12:55:54.782004 async_firebase-3.1.1/README.md
+-rw-r--r--   0        0        0      194 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/__init__.py
+-rw-r--r--   0        0        0     7906 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/base.py
+-rw-r--r--   0        0        0    23182 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/client.py
+-rw-r--r--   0        0        0     1547 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/encoders.py
+-rw-r--r--   0        0        0     8142 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/errors.py
+-rw-r--r--   0        0        0    16839 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/messages.py
+-rw-r--r--   0        0        0    12977 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/utils.py
+-rw-r--r--   0        0        0     1673 2023-05-10 12:55:54.782004 async_firebase-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9394 1970-01-01 00:00:00.000000 async_firebase-3.1.1/setup.py
+-rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 async_firebase-3.1.1/PKG-INFO
```

### Comparing `async_firebase-3.1.0/LICENSE` & `async_firebase-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/README.md` & `async_firebase-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/async_firebase/base.py` & `async_firebase-3.1.1/async_firebase/base.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/async_firebase/client.py` & `async_firebase-3.1.1/async_firebase/client.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/async_firebase/encoders.py` & `async_firebase-3.1.1/async_firebase/encoders.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/async_firebase/errors.py` & `async_firebase-3.1.1/async_firebase/errors.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/async_firebase/messages.py` & `async_firebase-3.1.1/async_firebase/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     webpush: an instance of ``messages.WebpushConfig`` (optional).
     apns: an instance of ``messages.ApnsConfig`` (optional).
     token: the registration token of the device to which the message should be sent.
     topic: name of the Firebase topic to which the message should be sent (optional).
     condition: the Firebase condition to which the message should be sent (optional).
     """
 
-    token: str
+    token: t.Optional[str] = None
     data: t.Dict[str, str] = field(default_factory=dict)
     notification: t.Optional[Notification] = field(default=None)
     android: t.Optional[AndroidConfig] = field(default=None)
     webpush: t.Optional[WebpushConfig] = field(default=None)
     apns: t.Optional[APNSConfig] = field(default=None)
     topic: t.Optional[str] = None
     condition: t.Optional[str] = None
```

### Comparing `async_firebase-3.1.0/async_firebase/utils.py` & `async_firebase-3.1.1/async_firebase/utils.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.0/pyproject.toml` & `async_firebase-3.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-firebase"
-version = "3.1.0"
+version = "3.1.1"
 description = "Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way."
 license = "MIT"
 authors = [
     "Oleksandr Omyshev <oomyshev@healthjoy.com>"
 ]
 maintainers = [
     "Healthjoy Developers <developers@healthjoy.com>",
@@ -29,25 +29,25 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 
 google-auth = "~2.6.0"
 httpx = ">=0.23.0,<1.0.0"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "~2.20"
-cryptography = "~3.4.7"
+pre-commit = "~2.21"
+cryptography = "~39.0.1"
 Faker = "~15.3"
 
 # tests
-pytest = "~6.2.2"
-pytest-asyncio = "~0.20"
+pytest = "~7.3"
+pytest-asyncio = "~0.21"
 pytest-benchmark = "~4.0.0"
-pytest-cov = "~2.12.1"
+pytest-cov = "~4.0.0"
 pytest-freezegun = "~0.4.2"
-pytest-httpx = "~0.21.2"
+pytest-httpx = "~0.22"
 black = "^22.10.0"
 mypy = "~0.991"
 
 [tool.isort]
 atomic = true
 force_grid_wrap = 0
 include_trailing_comma = true
```

### Comparing `async_firebase-3.1.0/setup.py` & `async_firebase-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-auth>=2.6.0,<2.7.0', 'httpx>=0.23.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'async-firebase',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.',
     'long_description': '# async-firebase is a lightweight asynchronous client to interact with Firebase Cloud Messaging for sending push notification to Android and iOS devices\n\n[![PyPI download month](https://img.shields.io/pypi/dm/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI version fury.io](https://badge.fury.io/py/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI license](https://img.shields.io/pypi/l/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![CI](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml/badge.svg)](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml)\n[![Codacy coverage](https://img.shields.io/codacy/coverage/b6a59cdf5ca64eab9104928d4f9bbb97?logo=codacy)](https://app.codacy.com/gh/healthjoy/async-firebase/dashboard)\n\n\n  * Free software: MIT license\n  * Requires: Python 3.7+\n\n## Features\n\n  * Extremely lightweight and does not rely on ``firebase-admin`` which is hefty\n  * Send push notifications to Android and iOS devices\n  * Send Multicast push notification to Android and iOS devices\n  * Send Web push notifications\n  * Set TTL (time to live) for notifications\n  * Set priority for notifications\n  * Set collapse-key for notifications\n  * Dry-run mode for testing purpose\n\n## Installation\n```shell script\n$ pip install async-firebase\n```\n\n## Getting started\n### async-firebase < 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    response = await client.push(device_token=device_token, android=android_config)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    response = await client.push(device_token=device_token, apns=apns_config)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    response = await client.push(device_token=device_token, apns=apns_config)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### async-firebase >= 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    message = Message(android=android_config, token=device_token)\n    response = await client.send(message)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.send(message)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps, Message\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token: str = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.send(message)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## License\n\n``async-firebase`` is offered under the MIT license.\n\n## Source code\n\nThe latest developer version is available in a GitHub repository:\n[https://github.com/healthjoy/async-firebase](https://github.com/healthjoy/async-firebase)\n',
     'author': 'Oleksandr Omyshev',
     'author_email': 'oomyshev@healthjoy.com',
     'maintainer': 'Healthjoy Developers',
     'maintainer_email': 'developers@healthjoy.com',
     'url': 'https://github.com/healthjoy/async-firebase',
```

### Comparing `async_firebase-3.1.0/PKG-INFO` & `async_firebase-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-firebase
-Version: 3.1.0
+Version: 3.1.1
 Summary: Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.
 Home-page: https://github.com/healthjoy/async-firebase
 License: MIT
 Keywords: async,asyncio,firebase,fcm,python3,push-notifications
 Author: Oleksandr Omyshev
 Author-email: oomyshev@healthjoy.com
 Maintainer: Healthjoy Developers
```

