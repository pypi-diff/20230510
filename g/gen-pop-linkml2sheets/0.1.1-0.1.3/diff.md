# Comparing `tmp/gen_pop_linkml2sheets-0.1.1.tar.gz` & `tmp/gen_pop_linkml2sheets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_pop_linkml2sheets-0.1.1.tar", max compression
+gzip compressed data, was "gen_pop_linkml2sheets-0.1.3.tar", max compression
```

## Comparing `gen_pop_linkml2sheets-0.1.1.tar` & `gen_pop_linkml2sheets-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4231 2023-05-10 12:49:52.108547 gen_pop_linkml2sheets-0.1.1/README.md
--rw-r--r--   0        0        0     2365 2023-05-10 13:26:33.708634 gen_pop_linkml2sheets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-10 12:49:52.112547 gen_pop_linkml2sheets-0.1.1/src/gen_pop_linkml2sheets/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.1/src/gen_pop_linkml2sheets/generate_and_populate_template.py
--rw-r--r--   0        0        0     4953 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.3/README.md
+-rw-r--r--   0        0        0     2365 2023-05-10 13:45:10.707541 gen_pop_linkml2sheets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-10 12:49:52.112547 gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/generate_and_populate_template.py
+-rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.3/PKG-INFO
```

### Comparing `gen_pop_linkml2sheets-0.1.1/LICENSE.md` & `gen_pop_linkml2sheets-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.1/README.md` & `gen_pop_linkml2sheets-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -95,27 +95,30 @@
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Feature 1
 - [ ] Feature 2
 - [ ] Feature 3
-  - [ ] Nested Feature
+    - [ ] Nested Feature
 
-See the [open issues](https://github.com/turbomam/gen-pop-linkml2sheets/issues) for a full list of proposed features (and known issues).
+See the [open issues](https://github.com/turbomam/gen-pop-linkml2sheets/issues) for a full list of proposed features (
+and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
+contributions you make are **greatly appreciated**.
 
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also
+simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
@@ -130,12 +133,16 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTACT -->
 
 ## Contact
 
+Based on https://gotofritz.net/blog/creating-a-poetry-driven-python-project-template-with-cookiecutter/
+
+Esp, `cookiecutter gh:gotofritz/cookiecutter-gotofritz-poetry`
+
 Fritz, [@your_name@mastodon.social](https://mastodon.social/@your_name)
 
 Project Link: [https://github.com/gotofritz/german-learning](https://github.com/gotofritz/german-learning)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -25,26 +25,28 @@
 m spacy download de_core_news_sm` 1. Run with [TODO]
                                                                   (back_to_top)
  ## Usage [TODO] Use this space to show useful examples of how a project can be
 used.
                                                                   (back_to_top)
  ## Roadmap - [ ] Feature 1 - [ ] Feature 2 - [ ] Feature 3 - [ ] Nested
 Feature See the [open issues](https://github.com/turbomam/gen-pop-
-linkml2sheets/issues) for a full list of proposed features (and known issues).
+linkml2sheets/issues) for a full list of proposed features ( and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE.md](./LICENSE.md)
 for more information.
                                                                   (back_to_top)
- ## Contact Fritz, [@your_name@mastodon.social](https://mastodon.social/
-@your_name) Project Link: [https://github.com/gotofritz/german-learning](https:
-//github.com/gotofritz/german-learning)
+ ## Contact Based on https://gotofritz.net/blog/creating-a-poetry-driven-
+python-project-template-with-cookiecutter/ Esp, `cookiecutter gh:gotofritz/
+cookiecutter-gotofritz-poetry` Fritz, [@your_name@mastodon.social](https://
+mastodon.social/@your_name) Project Link: [https://github.com/gotofritz/german-
+learning](https://github.com/gotofritz/german-learning)
                                                                   (back_to_top)
```

### Comparing `gen_pop_linkml2sheets-0.1.1/pyproject.toml` & `gen_pop_linkml2sheets-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "gen-pop-linkml2sheets"
-version = "0.1.1"
+version = "0.1.3"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/gen-pop-linkml2sheets"
 repository = "https://github.com/turbomam/gen-pop-linkml2sheets"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 linkml = "^1.5.2"
-pandas = "^2.0.1"
+pandas = "^1.3.4"
 schemasheets = "^0.1.21"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-sugar = "^0.9.5"
 pytest-clarity = "^1.0.1"
 pytest-random-order = "^1.0.4"
```

### Comparing `gen_pop_linkml2sheets-0.1.1/src/gen_pop_linkml2sheets/generate_and_populate_template.py` & `gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/generate_and_populate_template.py`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.1/PKG-INFO` & `gen_pop_linkml2sheets-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gen-pop-linkml2sheets
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/turbomam/gen-pop-linkml2sheets
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: linkml (>=1.5.2,<2.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
 Project-URL: Repository, https://github.com/turbomam/gen-pop-linkml2sheets
 Description-Content-Type: text/markdown
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 
 <a name="readme-top"></a>
@@ -115,27 +115,30 @@
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Feature 1
 - [ ] Feature 2
 - [ ] Feature 3
-  - [ ] Nested Feature
+    - [ ] Nested Feature
 
-See the [open issues](https://github.com/turbomam/gen-pop-linkml2sheets/issues) for a full list of proposed features (and known issues).
+See the [open issues](https://github.com/turbomam/gen-pop-linkml2sheets/issues) for a full list of proposed features (
+and known issues).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
+contributions you make are **greatly appreciated**.
 
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also
+simply open an issue with the tag "enhancement".
 Don't forget to give the project a star! Thanks again!
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
@@ -150,13 +153,17 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- CONTACT -->
 
 ## Contact
 
+Based on https://gotofritz.net/blog/creating-a-poetry-driven-python-project-template-with-cookiecutter/
+
+Esp, `cookiecutter gh:gotofritz/cookiecutter-gotofritz-poetry`
+
 Fritz, [@your_name@mastodon.social](https://mastodon.social/@your_name)
 
 Project Link: [https://github.com/gotofritz/german-learning](https://github.com/gotofritz/german-learning)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.1 Summary: Home-
+Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.3 Summary: Home-
 page: https://github.com/turbomam/gen-pop-linkml2sheets License: MIT Author:
 Mark Andrew Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Requires-
-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
+Dist: pandas (>=1.3.4,<2.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
 Project-URL: Repository, https://github.com/turbomam/gen-pop-linkml2sheets
 Description-Content-Type: text/markdown
 ****** Single step population of linkml2sheets usage reports, with useful
 columns only ******
 Single step population of linkml2sheets usage reports, with useful columns only
  Repo | Report_Bug | Releases
 
@@ -34,26 +34,28 @@
 m spacy download de_core_news_sm` 1. Run with [TODO]
                                                                   (back_to_top)
  ## Usage [TODO] Use this space to show useful examples of how a project can be
 used.
                                                                   (back_to_top)
  ## Roadmap - [ ] Feature 1 - [ ] Feature 2 - [ ] Feature 3 - [ ] Nested
 Feature See the [open issues](https://github.com/turbomam/gen-pop-
-linkml2sheets/issues) for a full list of proposed features (and known issues).
+linkml2sheets/issues) for a full list of proposed features ( and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE.md](./LICENSE.md)
 for more information.
                                                                   (back_to_top)
- ## Contact Fritz, [@your_name@mastodon.social](https://mastodon.social/
-@your_name) Project Link: [https://github.com/gotofritz/german-learning](https:
-//github.com/gotofritz/german-learning)
+ ## Contact Based on https://gotofritz.net/blog/creating-a-poetry-driven-
+python-project-template-with-cookiecutter/ Esp, `cookiecutter gh:gotofritz/
+cookiecutter-gotofritz-poetry` Fritz, [@your_name@mastodon.social](https://
+mastodon.social/@your_name) Project Link: [https://github.com/gotofritz/german-
+learning](https://github.com/gotofritz/german-learning)
                                                                   (back_to_top)
```

