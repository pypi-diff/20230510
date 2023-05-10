# Comparing `tmp/blindai-0.6.1.post2.tar.gz` & `tmp/blindai-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blindai-0.6.1.post2.tar", max compression
+gzip compressed data, was "blindai-0.6.2.tar", max compression
```

## Comparing `blindai-0.6.1.post2.tar` & `blindai-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     9415 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/README.md
--rw-r--r--   0        0        0      964 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/Intel_SGX_Provisioning_Certification_RootCA.pem
--rw-r--r--   0        0        0       51 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/__init__.py
--rw-r--r--   0        0        0    14117 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/_dcap_attestation.py
--rw-r--r--   0        0        0     2807 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/_preprocess_audio.py
--rw-r--r--   0        0        0       45 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/api.py
--rw-r--r--   0        0        0     3566 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/audio.py
--rwxr-xr-x   0        0        0    30892 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/client.py
--rw-r--r--   0        0        0      524 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/core.py
--rw-r--r--   0        0        0     2815 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/manifest.toml
--rw-r--r--   0        0        0     2815 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/manifest_cloud.toml
--rw-r--r--   0        0        0     3553 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/testing.py
--rw-r--r--   0        0        0     1600 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/blindai/utils.py
--rw-r--r--   0        0        0     1311 2020-04-16 12:00:00.000000 blindai-0.6.1.post2/pyproject.toml
--rw-r--r--   0        0        0    10834 1970-01-01 00:00:00.000000 blindai-0.6.1.post2/PKG-INFO
+-rw-r--r--   0        0        0     7936 2020-04-16 12:00:00.000000 blindai-0.6.2/README.md
+-rw-r--r--   0        0        0      964 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/Intel_SGX_Provisioning_Certification_RootCA.pem
+-rw-r--r--   0        0        0       51 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/__init__.py
+-rw-r--r--   0        0        0    14117 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/_dcap_attestation.py
+-rw-r--r--   0        0        0     2807 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/_preprocess_audio.py
+-rw-r--r--   0        0        0       45 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/api.py
+-rw-r--r--   0        0        0     3566 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/audio.py
+-rwxr-xr-x   0        0        0    30927 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/client.py
+-rw-r--r--   0        0        0      524 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/core.py
+-rw-r--r--   0        0        0     2815 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/manifest.toml
+-rw-r--r--   0        0        0     3553 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/testing.py
+-rw-r--r--   0        0        0     1600 2020-04-16 12:00:00.000000 blindai-0.6.2/blindai/utils.py
+-rw-r--r--   0        0        0     1305 2020-04-16 12:00:00.000000 blindai-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9349 1970-01-01 00:00:00.000000 blindai-0.6.2/PKG-INFO
```

### Comparing `blindai-0.6.1.post2/README.md` & `blindai-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: blindai
+Version: 0.6.2
+Summary: BlindAI Core / API is an open-source and easy-to-use Python library allowing you to query AI models with assurances that your private data will remain private
+Home-page: https://github.com/mithril-security/blindai
+Author: Mithril Security
+Author-email: contact@mithrilsecurity.io
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: torch
+Requires-Dist: cbor2 (>=5.4.3,<6.0.0)
+Requires-Dist: cryptography (>=39.0.1,<40.0.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
+Requires-Dist: numpy (>=1.23.5,<1.24)
+Requires-Dist: openai-whisper (>=20230308,<20230309)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: sgx-dcap-quote-verify-python (>=0.0.3,<0.0.4)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: torch (>=1.13.1,<2.0.0) ; extra == "torch"
+Requires-Dist: torchaudio (==0.13.1)
+Requires-Dist: transformers (==4.26.1)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Documentation, https://blindai.mithrilsecurity.io
+Project-URL: Repository, https://github.com/mithril-security/blindai
+Description-Content-Type: text/markdown
+
 <a name="readme-top"></a>
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![Apache License][license-shield]][license-url]
@@ -45,70 +76,66 @@
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#-getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
+        <li><a href="#blindai-api">BlindAI API</a></li>
+        <li><a href="#blindai-core">BlindAI Core</a></li>
       </ul>
     </li>
     <li><a href="#-usage">Usage</a></li>
     <li><a href="#-getting-help">Getting Help</a></li>
     <li><a href="#-license">License</a></li>
     <li><a href="#-contact">Contact</a></li>
   </ol>
 </details>
 
 <!-- ABOUT THE PROJECT -->
 ## 🔒 About The Project
 
-BlindAI is an **open-source solution** allowing users to query popular AI models or serve their own models with **assurances that users' private data will remain private**. The querying of models is done via our **easy-to-use BlindAI Python library**.
-
-Data sent by users to the AI model is kept **confidential at all times**. Neither the AI service provider nor the Cloud provider (if applicable), can see the data.
+**BlindAI** is an **open-source solution** to query and deploy AI models while **guaranteeing data privacy**. The querying of models is done via our **easy-to-use Python library**.
 
-Confidentiality is assured by hardware-enforced **Trusted Execution Environments**. We explain how they keep data and models safe in detail [here](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/confidential_computing/).
+Data sent by users to the AI model is kept **confidential at all times** by hardware-enforced **Trusted Execution Environments**. We explain how they keep data and models safe in detail [here](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/confidential_computing/).
 
 There are two main scenarios for BlindAI:
 
-- **BlindAI**: Using BlindAI to query popular AI models hosted by Mithril Security.
-- **BlindAI.Core**: Using BlindAI's underlying technology to host your own BlindAI server instance to securely deploy your own models.
+- **BlindAI API**: Using BlindAI to query popular AI models hosted by Mithril Security.
+- **BlindAI Core**: Using BlindAI's underlying technology to host your own BlindAI server instance to securely deploy your own models.
 
-You can find our more about BlindAI and BlindAI.Core [here](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/blindai_structure/).
+You can find our more about BlindAI API and BlindAI Core [here](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/blindai_structure/).
 
 ### Built With 
 
 [![Rust][Rust]][Rust-url] [![Python][Python]][Python-url] [![Intel-SGX][Intel-SGX]][Intel-sgx-url] [![Tract][Tract]][tract-url]
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- GETTING STARTED -->
 ## 🚀 Getting Started
 
-We strongly recommend for you to get started with our [Quick tour](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/quick-tour/) to discover BlindAI with a hands-on example using [COVID-Net](https://github.com/lindawangg/COVID-Net).
+We strongly recommend for you to get started with our [Quick tour](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/quick-tour/) to discover BlindAI with the open-source model Whisper.
 
 But here’s a taste of what using BlindAI could look like 🍒
 
-### BlindAI
+### BlindAI API
 
 ```py
-transcript = blindai_preview.api.Audio.transcribe(
+transcript = blindai.api.Audio.transcribe(
     file="patient_104678.wav"
 )
 print(transcript)
 
 The patient is a 55-year old male with known coronary artery disease.
 ```
 
 ### BlindAI.Core
 
-### AI company's side
-
-#### Uploading and deleting models
+#### AI company's side: uploading and deleting models
 
 An AI company AI company want to provide their model as an an easy-to-use service. They upload it to the server, which is assigned a model ID.
 
 ```py
 response = client_1.upload_model(model="./COVID-Net-CXR-2.onnx")
 MODEL_ID = response.model_id
 print(MODEL_ID)
@@ -119,71 +146,32 @@
 When collaborating with clients is done, the AI company can delete their model from the server.
 
 ```py
 # AI company deletes model after use
 client_1.delete_model(MODEL_ID)
 ```
 
-### Client's side
-
-#### Running a model on confidential data
+#### Client's side: running a model on confidential data
 
 The client wants to feed their confidential data to the model while protecting it from third-party access. They connect and run the model on the following confidential image.
 
 ![](https://github.com/mithril-security/blindai/blob/main/docs/assets/positive_image.png)
 
 ```py
 pos_ret = client_2.run_model(MODEL_ID, positive)
 print("Probability of Covid for positive image is", pos_ret.output[0].as_flat()[0][1])
 
 Probability of Covid for positive image is 0.890598714351654
 ```
 
 _For more examples, please refer to the [Documentation](https://blindai.mithrilsecurity.io/en/latest/)_
 
-### BlindAI.Core Installation
-
-**🥇 Recommended 🥇**
-
-#### Deploying BlindAI on Azure DCsv3 VM
-
-+ ✅ No requirement to have your own Intel SGX-ready device or a particular distribution. 
-+ ✅ Secure. Hardware security guarantees protect your data and model from any third-party access.
-+ ❌ Can be more expensive than local deployment.
-
-You can deploy the server in your Azure DCsv3 VM using our docker image with the following command:
-
-```bash
-docker run -it -e BLINDAI_AZURE_DCS3_PATCH=1 -p 9923:9923 -p 9924:9924 \
---device /dev/sgx/enclave --device /dev/sgx/provision \
--v /var/run/aesmd/aesm.socket:/var/run/aesmd/aesm.socket \
-mithrilsecuritysas/blindai-server:latest /root/start.sh
-```
-
-For alternative deployment methods (*on-premise, testing only...*) or more information, visit [our installation guide](https://blindai.mithrilsecurity.io/en/latest/docs/tutorials/core/installation/).
-
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-<!-- ROADMAP -->
-<!--
-## 🎯 Roadmap
-
-WRITE DOWN THE FEATURES WE **ALREADY** IMPLEMENTED. NOTHING SATISFYING LIKE A LIST WITH CHECKED BOXES.
-
-WE CAN ALSO RENAME THAT PART **KEY FEATURES**
-
-- [ ] Feature 1
-- [ ] Feature 2
-- [ ] Feature 3
-    - [ ] Nested Feature
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>-->
-
 <!-- GETTING HELP -->
-
 ## 🙋 Getting help
 
 * Go to our [Discord](https://discord.com/invite/TxEHagpWd4) #support channel
 * Report bugs by [opening an issue on our BlindAI GitHub](https://github.com/mithril-security/blindai/issues)
 * [Book a meeting](https://calendly.com/contact-mithril-security/15mins?month=2023-03) with us
 
 
@@ -227,7 +215,8 @@
 [Rust-url]: https://www.rust-lang.org/fr
 [Intel-SGX]: https://img.shields.io/badge/SGX-FFD43B?style=for-the-badge&logo=intel&logoColor=black
 [Intel-sgx-url]: https://www.intel.fr/content/www/fr/fr/architecture-and-technology/software-guard-extensions.html
 [Tract]: https://img.shields.io/badge/Tract-FFD43B?style=for-the-badge
 [tract-url]: https://github.com/mithril-security/tract/tree/6e4620659837eebeaba40ab3eeda67d33a99c7cf
 
 <!-- Done using https://github.com/othneildrew/Best-README-Template -->
+
```

#### html2text {}

```diff
@@ -1,10 +1,29 @@
- [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![Apache License][license-shield]][license-url]
+Metadata-Version: 2.1 Name: blindai Version: 0.6.2 Summary: BlindAI Core / API
+is an open-source and easy-to-use Python library allowing you to query AI
+models with assurances that your private data will remain private Home-page:
+https://github.com/mithril-security/blindai Author: Mithril Security Author-
+email: contact@mithrilsecurity.io Requires-Python: >=3.8,<4.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Provides-Extra: torch Requires-Dist: cbor2 (>=5.4.3,<6.0.0)
+Requires-Dist: cryptography (>=39.0.1,<40.0.0) Requires-Dist: ffmpeg-python
+(>=0.2.0,<0.3.0) Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0) Requires-
+Dist: numpy (>=1.23.5,<1.24) Requires-Dist: openai-whisper
+(>=20230308,<20230309) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
+sgx-dcap-quote-verify-python (>=0.0.3,<0.0.4) Requires-Dist: toml
+(>=0.10.2,<0.11.0) Requires-Dist: torch (>=1.13.1,<2.0.0) ; extra == "torch"
+Requires-Dist: torchaudio (==0.13.1) Requires-Dist: transformers (==4.26.1)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL: Documentation,
+https://blindai.mithrilsecurity.io Project-URL: Repository, https://github.com/
+mithril-security/blindai Description-Content-Type: text/markdown  [!
+[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
+[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![Apache License][license-shield]][license-url]
                                     [Logo]
                              ****** BlindAI ******
  [![Website][website-shield]][website-url] [![Blog][blog-shield]][blog-url] [!
                   [LinkedIn][linkedin-shield]][linkedin-url]
 BlindAI is an AI privacy solution, allowing users to query popular AI models or
  serve their own models whilst ensuring that users' data remains private every
                                step of the way.
@@ -12,75 +31,59 @@
                              Explore_the_docs_Â»
 
                    Try_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Getting_Started
-          o Prerequisites
-          o Installation
+          o BlindAI_API
+          o BlindAI_Core
    3. Usage
    4. Getting_Help
    5. License
    6. Contact
-  ## ð About The Project BlindAI is an **open-source solution** allowing
-users to query popular AI models or serve their own models with **assurances
-that users' private data will remain private**. The querying of models is done
-via our **easy-to-use BlindAI Python library**. Data sent by users to the AI
-model is kept **confidential at all times**. Neither the AI service provider
-nor the Cloud provider (if applicable), can see the data. Confidentiality is
-assured by hardware-enforced **Trusted Execution Environments**. We explain how
-they keep data and models safe in detail [here](https://
-blindai.mithrilsecurity.io/en/latest/docs/getting-started/
-confidential_computing/). There are two main scenarios for BlindAI: -
-**BlindAI**: Using BlindAI to query popular AI models hosted by Mithril
-Security. - **BlindAI.Core**: Using BlindAI's underlying technology to host
-your own BlindAI server instance to securely deploy your own models. You can
-find our more about BlindAI and BlindAI.Core [here](https://
+  ## ð About The Project **BlindAI** is an **open-source solution** to query
+and deploy AI models while **guaranteeing data privacy**. The querying of
+models is done via our **easy-to-use Python library**. Data sent by users to
+the AI model is kept **confidential at all times** by hardware-enforced
+**Trusted Execution Environments**. We explain how they keep data and models
+safe in detail [here](https://blindai.mithrilsecurity.io/en/latest/docs/
+getting-started/confidential_computing/). There are two main scenarios for
+BlindAI: - **BlindAI API**: Using BlindAI to query popular AI models hosted by
+Mithril Security. - **BlindAI Core**: Using BlindAI's underlying technology to
+host your own BlindAI server instance to securely deploy your own models. You
+can find our more about BlindAI API and BlindAI Core [here](https://
 blindai.mithrilsecurity.io/en/latest/docs/getting-started/blindai_structure/).
 ### Built With [![Rust][Rust]][Rust-url] [![Python][Python]][Python-url] [!
 [Intel-SGX][Intel-SGX]][Intel-sgx-url] [![Tract][Tract]][tract-url]
                                                                   (back_to_top)
  ## ð Getting Started We strongly recommend for you to get started with our
 [Quick tour](https://blindai.mithrilsecurity.io/en/latest/docs/getting-started/
-quick-tour/) to discover BlindAI with a hands-on example using [COVID-Net]
-(https://github.com/lindawangg/COVID-Net). But hereâs a taste of what using
-BlindAI could look like ð ### BlindAI ```py transcript =
-blindai_preview.api.Audio.transcribe( file="patient_104678.wav" ) print
-(transcript) The patient is a 55-year old male with known coronary artery
-disease. ``` ### BlindAI.Core ### AI company's side #### Uploading and deleting
+quick-tour/) to discover BlindAI with the open-source model Whisper. But
+hereâs a taste of what using BlindAI could look like ð ### BlindAI API
+```py transcript = blindai.api.Audio.transcribe( file="patient_104678.wav" )
+print(transcript) The patient is a 55-year old male with known coronary artery
+disease. ``` ### BlindAI.Core #### AI company's side: uploading and deleting
 models An AI company AI company want to provide their model as an an easy-to-
 use service. They upload it to the server, which is assigned a model ID. ```py
 response = client_1.upload_model(model="./COVID-Net-CXR-2.onnx") MODEL_ID =
 response.model_id print(MODEL_ID) 8afcdab8-209e-4b93-9403-f3ea2dc0c3ae ``` When
 collaborating with clients is done, the AI company can delete their model from
 the server. ```py # AI company deletes model after use client_1.delete_model
-(MODEL_ID) ``` ### Client's side #### Running a model on confidential data The
+(MODEL_ID) ``` #### Client's side: running a model on confidential data The
 client wants to feed their confidential data to the model while protecting it
 from third-party access. They connect and run the model on the following
 confidential image. ![](https://github.com/mithril-security/blindai/blob/main/
 docs/assets/positive_image.png) ```py pos_ret = client_2.run_model(MODEL_ID,
 positive) print("Probability of Covid for positive image is", pos_ret.output
 [0].as_flat()[0][1]) Probability of Covid for positive image is
 0.890598714351654 ``` _For more examples, please refer to the [Documentation]
-(https://blindai.mithrilsecurity.io/en/latest/)_ ### BlindAI.Core Installation
-**ð¥ Recommended ð¥** #### Deploying BlindAI on Azure DCsv3 VM + â No
-requirement to have your own Intel SGX-ready device or a particular
-distribution. + â Secure. Hardware security guarantees protect your data and
-model from any third-party access. + â Can be more expensive than local
-deployment. You can deploy the server in your Azure DCsv3 VM using our docker
-image with the following command: ```bash docker run -it -
-e BLINDAI_AZURE_DCS3_PATCH=1 -p 9923:9923 -p 9924:9924 \ --device /dev/sgx/
-enclave --device /dev/sgx/provision \ -v /var/run/aesmd/aesm.socket:/var/run/
-aesmd/aesm.socket \ mithrilsecuritysas/blindai-server:latest /root/start.sh ```
-For alternative deployment methods (*on-premise, testing only...*) or more
-information, visit [our installation guide](https://blindai.mithrilsecurity.io/
-en/latest/docs/tutorials/core/installation/).
+(https://blindai.mithrilsecurity.io/en/latest/)_
                                                                   (back_to_top)
-   ## ð Getting help * Go to our [Discord](https://discord.com/invite/
+ ## ð Getting help * Go to our [Discord](https://discord.com/invite/
 TxEHagpWd4) #support channel * Report bugs by [opening an issue on our BlindAI
 GitHub](https://github.com/mithril-security/blindai/issues) * [Book a meeting]
 (https://calendly.com/contact-mithril-security/15mins?month=2023-03) with us
 ## ð License Distributed under the Apache License, version 2.0. See
 [`LICENSE.md`](https://www.apache.org/licenses/LICENSE-2.0) for more
 information.  ## ð Contact Mithril Security - [@MithrilSecurity](https://
 twitter.com/MithrilSecurity) - contact@mithrilsecurity.io Project Link: [https:
```

### Comparing `blindai-0.6.1.post2/blindai/Intel_SGX_Provisioning_Certification_RootCA.pem` & `blindai-0.6.2/blindai/Intel_SGX_Provisioning_Certification_RootCA.pem`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/_dcap_attestation.py` & `blindai-0.6.2/blindai/_dcap_attestation.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/_preprocess_audio.py` & `blindai-0.6.2/blindai/_preprocess_audio.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/audio.py` & `blindai-0.6.2/blindai/audio.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/client.py` & `blindai-0.6.2/blindai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import os
 import contextlib
 import socket
+import sys
 
 import numpy as np
 import cbor2 as cbor
 
 from hashlib import sha256
 import platform
 import getpass
@@ -552,15 +553,15 @@
             .hex(),
             platform_name=uname.system,
             platform_arch=uname.machine,
             platform_version=uname.version,
             platform_release=uname.release,
             user_agent="blindai_python",
             user_agent_version=app_version,
-            is_colab=False,
+            is_colab="google.colab" in sys.modules,
         )
 
         if hazmat_http_on_unattested_port:
             self._unattested_url = f"http://{addr}:{unattested_server_port}"
         else:
             self._unattested_url = f"https://{addr}:{unattested_server_port}"
 
@@ -792,15 +793,15 @@
 from functools import wraps
 
 
 def connect(
     addr: str,
     unattested_server_port: int = 9923,
     attested_server_port: int = 9924,
-    model_management_port: int = 9924,
+    model_management_port: int = 9925,
     hazmat_manifest_path: Optional[pathlib.Path] = None,
     hazmat_http_on_unattested_port=False,
     simulation_mode: bool = False,
     use_cloud_manifest: bool = False,
 ) -> BlindAiConnection:
     """Connect to a BlindAi server.
```

### Comparing `blindai-0.6.1.post2/blindai/core.py` & `blindai-0.6.2/blindai/core.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/manifest.toml` & `blindai-0.6.2/blindai/manifest.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Enclave manifest file for production
 # Determines which enclaves are to be accepted by
 # the client
 
 # Enclave measurement
 # MRENCLAVE represents the enclave's contents and build process
-mr_enclave = "7be31f9b2efcc2994239a5986dc391484ed2604ce89f32694baacf703e546126"
+mr_enclave = "2b6d7ab943ab55a5dc7d2a8015f550c25332493b847ebc87b9e382303f5fa5cf"
 
 # Set to true to allow enclave running in DEBUG mode 
 # A production service should never allow debug-mode enclaves
 allow_debug = false
 
 # Enclave attributes are formed of : 
 #  * attributes_flags
```

### Comparing `blindai-0.6.1.post2/blindai/testing.py` & `blindai-0.6.2/blindai/testing.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/blindai/utils.py` & `blindai-0.6.2/blindai/utils.py`

 * *Files identical despite different names*

### Comparing `blindai-0.6.1.post2/pyproject.toml` & `blindai-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blindai"
-version = "0.6.1-post2"
+version = "0.6.2"
 description = "BlindAI Core / API is an open-source and easy-to-use Python library allowing you to query AI models with assurances that your private data will remain private"
 authors = ["Mithril Security <contact@mithrilsecurity.io>"]
 readme = "README.md"
 documentation = "https://blindai.mithrilsecurity.io"
 repository = "https://github.com/mithril-security/blindai"
 
 [tool.poetry.dependencies]
```

